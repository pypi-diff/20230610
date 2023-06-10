# Comparing `tmp/eqalert-3.5.2.tar.gz` & `tmp/eqalert-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqalert-3.5.2.tar", last modified: Fri Jun  2 00:05:00 2023, max compression
+gzip compressed data, was "eqalert-3.5.3.tar", last modified: Sat Jun 10 14:52:32 2023, max compression
```

## Comparing `eqalert-3.5.2.tar` & `eqalert-3.5.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:05:00.567552 eqalert-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-06-02 00:05:00.567552 eqalert-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-02 00:04:40.000000 eqalert-3.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:05:00.563552 eqalert-3.5.2/eqa/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61968 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/eqalert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:05:00.563552 eqalert-3.5.2/eqa/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   108095 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/action.py
--rw-r--r--   0 runner    (1001) docker     (123)   468426 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    76369 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/encounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)   488202 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/lib/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:05:00.567552 eqalert-3.5.2/eqa/sound/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/sound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/sound/tick.wav
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-02 00:04:40.000000 eqalert-3.5.2/eqa/sound/tock.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:05:00.567552 eqalert-3.5.2/eqalert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-06-02 00:05:00.000000 eqalert-3.5.2/eqalert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-02 00:05:00.000000 eqalert-3.5.2/eqalert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:05:00.000000 eqalert-3.5.2/eqalert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 00:05:00.000000 eqalert-3.5.2/eqalert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 00:05:00.000000 eqalert-3.5.2/eqalert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-02 00:05:00.000000 eqalert-3.5.2/eqalert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 00:05:00.567552 eqalert-3.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-02 00:04:40.000000 eqalert-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.728043 eqalert-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-10 14:52:32.728043 eqalert-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-10 14:52:18.000000 eqalert-3.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.720043 eqalert-3.5.3/eqa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62129 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/eqalert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.724043 eqalert-3.5.3/eqa/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123206 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580055 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)   488202 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.724043 eqalert-3.5.3/eqa/sound/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/sound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/sound/tick.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/sound/tock.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.728043 eqalert-3.5.3/eqalert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-10 14:52:32.728043 eqalert-3.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-10 14:52:18.000000 eqalert-3.5.3/setup.py
```

### Comparing `eqalert-3.5.2/PKG-INFO` & `eqalert-3.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.2
+Version: 3.5.3
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
@@ -38,27 +38,29 @@
 $ cd eqalert
 $ docker compose build
 $ docker compose run eqalert
 ```
 
 > Note: If running through docker after installing and running on your host, update or regenerate `~/.eqa/config/settings.json` to reflect local container paths in `/home/eqalert`
 
+
 ## Getting Started
 
 Start things up
 ```sh
 $ eqalert
 ```
 
 You should now see `~/.eqa/` with the following structure
 ```
 $HOME/.eqa
         ⎿ config/
           ⎿ line-alerts/
         ⎿ data/
+          ⎿ timers/
         ⎿ encounters/
         ⎿ log/
           ⎿ debug/
         ⎿ sound/
 ```
 
 Spot check these default paths generated in `config/settings.json`
@@ -72,14 +74,15 @@
       "everquest_files": "[$HOME]/.wine/drive_c/Program Files/Sony/EverQuest/",
       "sound": "[$HOME/.eqa/]sound/",
       "tmp_sound": "/tmp/eqa/sound/"
     },
 ```
 > Press `0` to reload your configs or restart the program if any changes were made.  Though generally, it's a good idea to stop eqalert before manually editing your config files.
 
+
 ## Data
 
 ### Spell Timers
 
 EQ Alert will generate a file for spell timers in `data/spell-timers.json` by default by parsing `spells_us.txt` in your EverQuest directory.
 
 This file will only regenerate if it is missing, malformed, or a newer `spells_us.txt` file is present.
@@ -88,40 +91,54 @@
 
 EQ Alert will generate/overwrite `data/spell-casters.json` each version.  This file contains which classes can cast a given buff which timers should be made for.
 
 ### Spell Lines
 
 Many spells cast in EverQuest share the same log output lines.  EQ Alert will generate/overwrite `data/spell-lines.json` each version as a mapping of which possible spells a given output line could be associated to.
 
+### Spell Items
+
+EQ Alert will generate/overwrite `data/spell-items.json` each version as a mapping of which items a given spell could be cast by.
+
 ### Players
 
 EQ Alert uses in-game `/who` output to keep an up-to-date list of each seen players class, level, and guild organized by server in `data/players.json` for alerting spell duration.
 
+### Saved Timers
+
+If the active character is changed or EQ Alert is stopped, all active timers are saved to a file in `data/timers/` by the previously active character and server name.  This file is consumed when the parser sets that character as active again, adding all non-expired timers back to the timer list.
+
+
+## Encounters
+
+When encounter parse saving is enabled, complete encounter reports are saved under `encounters/[zone_name]/[date]/` as the time stamp of the encounter and the encounter target.
+
 
 ## Controls
 
 ### Keyboard Controls
 
 #### Global
   - 0       : Reload config
   - 1       : Events
   - 2       : State
   - 3       : Parse
   - 4       : Settings
   - q / esc : Quit
-  - h       : Help
+  - h       : Help pop-up
+  - t       : Timers pop-up
 
 #### Events
   - c       : Clear event box
   - d       : Toggle debug mode
   - e       : Toggle encounter parsing
   - m       : Toggle global audio mute
   - p       : Toggle encounter parse save
   - r       : Toggle raid mode
-  - t       : Toggle automatic mob respawn timers
+  - y       : Toggle automatic mob respawn timers
 
 #### Settings
   - up      : Up in selection
   - down    : Down in selection
   - right   : Selection options
   - left    : Selection options
   - space   : Select
```

### Comparing `eqalert-3.5.2/README.md` & `eqalert-3.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,29 @@
 $ cd eqalert
 $ docker compose build
 $ docker compose run eqalert
 ```
 
 > Note: If running through docker after installing and running on your host, update or regenerate `~/.eqa/config/settings.json` to reflect local container paths in `/home/eqalert`
 
+
 ## Getting Started
 
 Start things up
 ```sh
 $ eqalert
 ```
 
 You should now see `~/.eqa/` with the following structure
 ```
 $HOME/.eqa
         ⎿ config/
           ⎿ line-alerts/
         ⎿ data/
+          ⎿ timers/
         ⎿ encounters/
         ⎿ log/
           ⎿ debug/
         ⎿ sound/
 ```
 
 Spot check these default paths generated in `config/settings.json`
@@ -61,14 +63,15 @@
       "everquest_files": "[$HOME]/.wine/drive_c/Program Files/Sony/EverQuest/",
       "sound": "[$HOME/.eqa/]sound/",
       "tmp_sound": "/tmp/eqa/sound/"
     },
 ```
 > Press `0` to reload your configs or restart the program if any changes were made.  Though generally, it's a good idea to stop eqalert before manually editing your config files.
 
+
 ## Data
 
 ### Spell Timers
 
 EQ Alert will generate a file for spell timers in `data/spell-timers.json` by default by parsing `spells_us.txt` in your EverQuest directory.
 
 This file will only regenerate if it is missing, malformed, or a newer `spells_us.txt` file is present.
@@ -77,40 +80,54 @@
 
 EQ Alert will generate/overwrite `data/spell-casters.json` each version.  This file contains which classes can cast a given buff which timers should be made for.
 
 ### Spell Lines
 
 Many spells cast in EverQuest share the same log output lines.  EQ Alert will generate/overwrite `data/spell-lines.json` each version as a mapping of which possible spells a given output line could be associated to.
 
+### Spell Items
+
+EQ Alert will generate/overwrite `data/spell-items.json` each version as a mapping of which items a given spell could be cast by.
+
 ### Players
 
 EQ Alert uses in-game `/who` output to keep an up-to-date list of each seen players class, level, and guild organized by server in `data/players.json` for alerting spell duration.
 
+### Saved Timers
+
+If the active character is changed or EQ Alert is stopped, all active timers are saved to a file in `data/timers/` by the previously active character and server name.  This file is consumed when the parser sets that character as active again, adding all non-expired timers back to the timer list.
+
+
+## Encounters
+
+When encounter parse saving is enabled, complete encounter reports are saved under `encounters/[zone_name]/[date]/` as the time stamp of the encounter and the encounter target.
+
 
 ## Controls
 
 ### Keyboard Controls
 
 #### Global
   - 0       : Reload config
   - 1       : Events
   - 2       : State
   - 3       : Parse
   - 4       : Settings
   - q / esc : Quit
-  - h       : Help
+  - h       : Help pop-up
+  - t       : Timers pop-up
 
 #### Events
   - c       : Clear event box
   - d       : Toggle debug mode
   - e       : Toggle encounter parsing
   - m       : Toggle global audio mute
   - p       : Toggle encounter parse save
   - r       : Toggle raid mode
-  - t       : Toggle automatic mob respawn timers
+  - y       : Toggle automatic mob respawn timers
 
 #### Settings
   - up      : Up in selection
   - down    : Down in selection
   - right   : Selection options
   - left    : Selection options
   - space   : Select
```

### Comparing `eqalert-3.5.2/eqa/eqalert.py` & `eqalert-3.5.3/eqa/eqalert.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,17 @@
 
         # Generate spell-lines.json
         eqa_config.update_spell_lines(data_path, version)
 
         # Generate spell-casters.json
         eqa_config.update_spell_casters(data_path, version)
 
+        # Generate spell-items.json
+        eqa_config.update_spell_items(data_path, version)
+
         # Generate Players List File
         player_data_file = data_path + "players.json"
         if not os.path.isfile(player_data_file):
             eqa_config.generate_players_file(player_data_file, version)
         else:
             eqa_config.validate_players_file(player_data_file, version)
 
@@ -272,14 +275,15 @@
             target=eqa_keys.process,
             args=(
                 state,
                 configs,
                 display_q,
                 keyboard_q,
                 system_q,
+                timer_q,
                 cfg_reload,
                 exit_flag,
             ),
         )
         process_keys.daemon = True
         process_keys.start()
 
@@ -768,14 +772,15 @@
                             target=eqa_keys.process,
                             args=(
                                 state,
                                 configs,
                                 display_q,
                                 keyboard_q,
                                 system_q,
+                                timer_q,
                                 cfg_reload,
                                 exit_flag,
                             ),
                         )
                         process_keys.daemon = True
                         process_keys.start()
```

### Comparing `eqalert-3.5.2/eqa/lib/action.py` & `eqalert-3.5.3/eqa/lib/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,19 @@
         )
 
         # Spell Caster Data
         spell_casters = eqa_config.get_spell_casters(
             configs.settings.config["settings"]["paths"]["data"]
         )
 
+        # Spell Item Data
+        spell_items = eqa_config.get_spell_items(
+            configs.settings.config["settings"]["paths"]["data"]
+        )
+
         # Player Data
         player_list = eqa_config.get_players_file(
             configs.settings.config["settings"]["paths"]["data"], state.server
         )
 
         # Class Mapping
         class_mapping = {
@@ -293,14 +298,15 @@
                                 line_time,
                                 check_line,
                                 spell_casting_buffer_other,
                                 spell_casting_buffer_you,
                                 spell_timers,
                                 spell_lines,
                                 spell_casters,
+                                spell_items,
                                 player_list,
                             )
                     ## Self Spell Timers
                     if state.spell_timer_self:
                         if re.fullmatch(r"^spell\_.+\_you_on$", line_type) is not None:
                             action_spell_timer(
                                 state,
@@ -310,14 +316,15 @@
                                 line_time,
                                 check_line,
                                 spell_casting_buffer_other,
                                 spell_casting_buffer_you,
                                 spell_timers,
                                 spell_lines,
                                 spell_casters,
+                                spell_items,
                                 player_list,
                             )
                         elif (
                             re.fullmatch(r"^spell\_.+\_you_off$", line_type) is not None
                         ):
                             action_spell_remove_timer(
                                 state, timer_q, spell_lines, line_type, check_line
@@ -789,33 +796,160 @@
             "acton spell remove timer: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
+def action_spell_timer_player_click_check(
+    spell_land_time,
+    cast_start_time,
+    cast_duration,
+    caster_name,
+    caster_level,
+    caster_class,
+    check_spell,
+    spell_items,
+    item,
+):
+    """Check if a given player could click a given spell"""
+
+    try:
+        if cast_duration > 0:
+            if (
+                action_spell_timer_cast_check(
+                    spell_land_time, cast_start_time, cast_duration
+                )
+                == 0
+            ):
+                if check_spell in spell_items["spells"].keys():
+                    # If the player class can cast this spell
+                    if (
+                        caster_class
+                        in spell_items["spells"][check_spell][item]["classes"].keys()
+                    ):
+                        # If that players level can cast this spell
+                        if (
+                            spell_items["spells"][check_spell][item]["classes"][
+                                caster_class
+                            ]
+                            <= caster_level
+                        ):
+                            return [caster_name, caster_level, check_spell]
+        else:
+            if check_spell in spell_items["spells"].keys():
+                if (
+                    caster_class
+                    in spell_items["spells"][check_spell][item]["classes"].keys()
+                ):
+                    # If that players level can cast this spell
+                    if (
+                        spell_items["spells"][check_spell][item]["classes"][
+                            caster_class
+                        ]
+                        <= caster_level
+                    ):
+                        return [caster_name, caster_level, check_spell]
+
+        return None
+
+    except Exception as e:
+        eqa_settings.log(
+            "acton spell timer player click check: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
+def action_spell_timer_player_cast_check(
+    spell_land_time,
+    cast_start_time,
+    cast_duration,
+    caster_name,
+    caster_level,
+    caster_class,
+    check_spell,
+    spell_casters,
+):
+    """Check if a given player could cast a given spell"""
+
+    try:
+        if (
+            action_spell_timer_cast_check(
+                spell_land_time, cast_start_time, cast_duration
+            )
+            == 0
+        ):
+            if check_spell in spell_casters["spells"].keys():
+                # If the player class can cast this spell
+                if (
+                    caster_class
+                    in spell_casters["spells"][check_spell]["classes"].keys()
+                ):
+                    # If that players level can cast this spell
+                    if (
+                        spell_casters["spells"][check_spell]["classes"][caster_class]
+                        <= caster_level
+                    ):
+                        return [caster_name, caster_level, check_spell]
+
+        return None
+
+    except Exception as e:
+        eqa_settings.log(
+            "acton spell timer player cast check: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
+def action_spell_timer_cast_check(spell_land_time, cast_start_time, cast_duration):
+    """Return int (spell landed - spell cast - spell cast duration)"""
+    try:
+        cast_land_duration_diff = int(
+            (
+                datetime.datetime.strptime(spell_land_time, "%H:%M:%S.%f")
+                - datetime.datetime.strptime(cast_start_time, "%H:%M:%S.%f")
+                - datetime.timedelta(seconds=float(cast_duration))
+            ).total_seconds()
+        )
+
+        return cast_land_duration_diff
+
+    except Exception as e:
+        eqa_settings.log(
+            "acton spell timer cast check: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
 def action_spell_timer(
     state,
     configs,
     timer_q,
     line_type,
     line_time,
     line,
     spell_casting_buffer_other,
     spell_casting_buffer_you,
     spell_timers,
     spell_lines,
     spell_casters,
+    spell_items,
     player_list,
 ):
     """Set timer for spell duration"""
 
     try:
         is_spell_line = False
-        find_time = False
+        identified_spell_level = None
 
         if re.fullmatch(r"^spell\_line\_[a-zA-Z\s\_]+\_you\_on", line_type) is not None:
             target = state.char.lower()
             spell_line = re.findall(
                 r"(?<=spell\_line\_)[a-zA-Z\s\_]+(?=\_you\_on)", line_type
             )[0]
             is_spell_line = True
@@ -837,358 +971,520 @@
                 0
             ]
             # TODO: Find way to reliably pull multi-word NPC names from spell_*_other_on () sans spell_line_
             target = re.findall(r"(?:^|(?:[.!?]\s))(\w+)", line)[0].lower()
 
         # If this is a spell cast line output shared by more than one spell
         if is_spell_line:
-            if state.debug:
-                eqa_settings.log("spell line found: " + line_type)
             # Determine possible spells
             if line_type in spell_lines["spell_lines"].keys():
                 possible_spells = spell_lines["spell_lines"][line_type].keys()
-                if state.debug:
-                    eqa_settings.log("possible spells: " + str(possible_spells))
-                check_for_spells = []
-                # Retrieve casting requirements for each possible spell
-                for possible_spell in possible_spells:
-                    if possible_spell in spell_casters["spells"].keys():
-                        # Validate a player cast this spell
-                        ## TODO: later try and guess npc/item only spells with vague messages, for now thats too much guessing
-                        if spell_casters["spells"][possible_spell]["classes"]:
-                            check_for_spells.append(
-                                {
-                                    "spell": possible_spell,
-                                    "classes": spell_casters["spells"][possible_spell][
-                                        "classes"
-                                    ].keys(),
-                                }
-                            )
 
-                # First check if the player could have cast this
-                if spell_casting_buffer_you and state.char_level is not None:
-                    # If the most recent player cast spell is in the possible spell list
-                    if (
-                        spell_casting_buffer_you["spell"]
-                        in spell_lines["spell_lines"][line_type].keys()
-                        and spell_casting_buffer_you["spell"]
-                        in spell_casters["spells"].keys()
-                    ):
-                        if state.debug:
-                            eqa_settings.log(
-                                "Checking if cast for: "
-                                + spell_casting_buffer_you["spell"]
-                                + " occurred "
-                                + spell_timers["spells"][
+                # First check if the active player could have cast this
+                if (
+                    spell_casting_buffer_you
+                    and state.char_level is not None
+                    and state.char_class is not None
+                ):
+                    if spell_casting_buffer_you["spell"] in possible_spells:
+                        cast_duration = spell_timers["spells"][
+                            spell_casting_buffer_you["spell"]
+                        ]["cast_time"]
+                        identified = action_spell_timer_player_cast_check(
+                            line_time,
+                            spell_casting_buffer_you["time"],
+                            cast_duration,
+                            state.char.lower(),
+                            state.char_level,
+                            state.char_class.lower(),
+                            spell_casting_buffer_you["spell"],
+                            spell_casters,
+                        )
+                        if identified is not None:
+                            identified_spell_caster = identified[0]
+                            identified_spell_level = identified[1]
+                            identified_spell = identified[2]
+                            identified_spell_target = target
+
+                        # Check if active player could have clicked this spell
+                        elif spell_casters["spells"][spell_casting_buffer_you["spell"]][
+                            "item"
+                        ]:
+                            for item in spell_items["spells"][
+                                spell_casting_buffer_you["spell"]
+                            ]:
+                                cast_duration = spell_items["spells"][
                                     spell_casting_buffer_you["spell"]
-                                ]["cast_time"]
-                                + " seconds ago"
-                            )
-                        # If most recent player cast spell occurred spell time ago to this spell landing
-                        if (
-                            int(
-                                (
-                                    datetime.datetime.strptime(line_time, "%H:%M:%S.%f")
-                                    - datetime.datetime.strptime(
-                                        spell_casting_buffer_you["time"], "%H:%M:%S.%f"
-                                    )
-                                    - datetime.timedelta(
-                                        seconds=float(
-                                            spell_timers["spells"][
-                                                spell_casting_buffer_you["spell"]
-                                            ]["cast_time"]
-                                        )
+                                ][item]["cast"]
+                                if cast_duration > 0:
+                                    identified = action_spell_timer_player_click_check(
+                                        line_time,
+                                        spell_casting_buffer_you["time"],
+                                        cast_duration,
+                                        state.char.lower(),
+                                        state.char_level,
+                                        state.char_class.lower(),
+                                        spell_casting_buffer_you["spell"],
+                                        spell_items,
+                                        item,
                                     )
-                                ).total_seconds()
-                            )
-                            == 0
-                        ):
-                            identified_spell_caster = state.char.lower()
-                            identified_spell_level = state.char_level
-                            identified_spell = spell_casting_buffer_you["spell"]
-                            identified_spell_target = target
-                            find_time = True
+                                    if identified is not None:
+                                        identified_spell_caster = identified[0]
+                                        identified_spell_level = identified[1]
+                                        identified_spell = identified[2]
+                                        identified_spell_target = target
 
-                # Then check spell cast buffer other cast time ago for each possible spell
-                if not find_time:
+                # Check if another player could have cast this
+                if identified_spell_level is None:
                     # For each possible spell
-                    for spell_caster in check_for_spells:
-                        # Retrieve cast time for the possible spell
-                        cast_time = spell_timers["spells"][
-                            spell_caster["spell"]
-                        ]  # this is way too hard to read
-                        # Check each event in spell cast buffer other if it occurred possible spell cast time ago
+                    for check_spell in possible_spells:
+                        # Check each recent cast event
                         for recent_cast_event in spell_casting_buffer_other:
-                            # If this spell event coincides with a spell cast event cast time ago
-                            if (
-                                int(
-                                    (
-                                        datetime.datetime.strptime(
-                                            line_time, "%H:%M:%S.%f"
-                                        )
-                                        - datetime.datetime.strptime(
-                                            recent_cast_event["time"], "%H:%M:%S.%f"
-                                        )
-                                        - datetime.timedelta(
-                                            seconds=float(
-                                                spell_timers["spells"][
-                                                    spell_caster["spell"]
-                                                ]["cast_time"]
-                                            )
-                                        )
-                                    ).total_seconds()
-                                )
-                                == 0
-                            ):
-                                # Check if caster is able to cast potential spell
-                                if recent_cast_event["caster"] in player_list.keys():
-                                    player_class = player_list[
-                                        recent_cast_event["caster"]
-                                    ]["class"]
-                                    player_level = player_list[
-                                        recent_cast_event["caster"]
-                                    ]["level"]
-                                    # If we know this players class and level
-                                    if player_class is not None and player_level > 0:
-                                        # If the player class can cast this spell
-                                        if (
-                                            player_class
-                                            in spell_casters["spells"][
-                                                spell_caster["spell"]
-                                            ]["classes"].keys()
-                                        ):
-                                            # If that players level can cast this spell
+                            caster_name = recent_cast_event["caster"]
+                            cast_duration = spell_timers["spells"][check_spell][
+                                "cast_time"
+                            ]
+                            # If we know the class/level of the caster
+                            if caster_name in player_list.keys():
+                                caster_class = player_list[caster_name]["class"]
+                                caster_level = player_list[caster_name]["level"]
+                                if caster_class is not None and caster_level > 0:
+                                    # Check if another player could cast this possible spell
+                                    identified = action_spell_timer_player_cast_check(
+                                        line_time,
+                                        recent_cast_event["time"],
+                                        cast_duration,
+                                        caster_name,
+                                        caster_level,
+                                        caster_class,
+                                        check_spell,
+                                        spell_casters,
+                                    )
+                                    if identified is not None:
+                                        if identified_spell_level is not None:
                                             if (
-                                                int(
-                                                    spell_casters["spells"][
-                                                        spell_caster["spell"]
-                                                    ]["classes"][player_class]
-                                                )
-                                                <= player_level
+                                                spell_casters["spells"][
+                                                    identified_spell
+                                                ]["classes"][
+                                                    player_list[
+                                                        identified_spell_caster
+                                                    ]["class"]
+                                                ]
+                                                < spell_casters["spells"][
+                                                    identified[2]
+                                                ]["classes"][
+                                                    player_list[identified[0]]["class"]
+                                                ]
                                             ):
-                                                if not find_time:
-                                                    identified_spell_caster = (
-                                                        recent_cast_event["caster"]
+                                                identified_spell_caster = identified[0]
+                                                identified_spell_level = identified[1]
+                                                identified_spell = identified[2]
+                                                identified_spell_target = target
+                                        else:
+                                            identified_spell_caster = identified[0]
+                                            identified_spell_level = identified[1]
+                                            identified_spell = identified[2]
+                                            identified_spell_target = target
+                                    # Check if another player used a clicky
+                                    elif check_spell in spell_casters["spells"].keys():
+                                        if spell_casters["spells"][check_spell]["item"]:
+                                            for item in spell_items["spells"][
+                                                check_spell
+                                            ]:
+                                                cast_duration = spell_items["spells"][
+                                                    check_spell
+                                                ][item]["cast"]
+                                                # Non-zero click casts have spell casting messages
+                                                if cast_duration > 0:
+                                                    identified = action_spell_timer_player_click_check(
+                                                        line_time,
+                                                        recent_cast_event["time"],
+                                                        cast_duration,
+                                                        caster_name,
+                                                        caster_level,
+                                                        caster_class,
+                                                        check_spell,
+                                                        spell_items,
+                                                        item,
                                                     )
-                                                    identified_spell_level = (
-                                                        player_list[
-                                                            identified_spell_caster
+                                                    if identified is not None:
+                                                        identified_spell_caster = (
+                                                            identified[0]
+                                                        )
+                                                        identified_spell_level = (
+                                                            identified[1]
+                                                        )
+                                                        idenfitied_spell = identified[2]
+                                                        identified_spell_target = target
+                                                # Instant click cast event but self only spell
+                                                elif spell_casters["spells"][
+                                                    check_spell
+                                                ]["self"]:
+                                                    if target in player_list.keys():
+                                                        caster_name = target
+                                                        caster_level = player_list[
+                                                            target
                                                         ]["level"]
-                                                    )
-                                                    identified_spell = spell_caster[
-                                                        "spell"
-                                                    ]
-                                                    identified_spell_target = target
-                                                    find_time = True
-                                                # Favor matched spell with highest level casting requirements
-                                                elif int(
-                                                    spell_casters["spells"][
-                                                        identified_spell
-                                                    ]["classes"][
-                                                        player_list[
-                                                            identified_spell_caster
-                                                        ]["class"]
-                                                    ]
-                                                ) < int(
-                                                    spell_casters["spells"][
-                                                        identified_spell
-                                                    ]["classes"][
-                                                        player_list[
-                                                            recent_cast_event["caster"]
+                                                        caster_class = player_list[
+                                                            target
                                                         ]["class"]
-                                                    ]
+                                                    if (
+                                                        caster_class is not None
+                                                        and caster_level > 0
+                                                    ):
+                                                        identified = action_spell_timer_player_click_check(
+                                                            line_time,
+                                                            recent_cast_event["time"],
+                                                            cast_duration,
+                                                            caster_name,
+                                                            caster_level,
+                                                            caster_class,
+                                                            check_spell,
+                                                            spell_items,
+                                                            item,
+                                                        )
+                                                        if identified is not None:
+                                                            identified_spell_caster = (
+                                                                identified[0]
+                                                            )
+                                                            identified_spell_level = (
+                                                                identified[1]
+                                                            )
+                                                            idenfitied_spell = (
+                                                                identified[2]
+                                                            )
+                                                            identified_spell_target = (
+                                                                target
+                                                            )
+
+                # Haven't found anything yet, check if it could be an instant click (these have no casting messages)
+                if identified_spell_level is None and target == state.char.lower():
+                    for check_spell in possible_spells:
+                        if check_spell in spell_items["spells"].keys():
+                            for item in spell_items["spells"][check_spell]:
+                                if (
+                                    spell_items["spells"][check_spell][item]["cast"]
+                                    == 0
+                                ):
+                                    identified = action_spell_timer_player_click_check(
+                                        line_time,
+                                        line_time,
+                                        0,
+                                        state.char.lower(),
+                                        state.char_level,
+                                        state.char_class.lower(),
+                                        check_spell,
+                                        spell_items,
+                                        item,
+                                    )
+                                    if identified is not None:
+                                        identified_spell_caster = identified[0]
+                                        identified_spell_level = identified[1]
+                                        identified_spell = identified[2]
+                                        identified_spell_target = target
+
+                # Time to guess the spell level
+                if identified_spell_level is None and state.spell_timer_guess:
+                    # For each possible spell
+                    for check_spell in possible_spells:
+                        # Check each recent cast event
+                        for recent_cast_event in spell_casting_buffer_other:
+                            # If this is a known npc spell, just set to current player level
+                            if (
+                                spell_casters["spells"][check_spell]["npc"]
+                                and state.char_level is not None
+                                and identified_spell_level is None
+                            ):
+                                identified_spell_caster = recent_cast_event["caster"]
+                                identified_spell_level = state.char_level
+                                identified_spell = check_spell
+                                identified_spell_target = target
+
+                            # If a player could cast this
+                            player_level_could_cast = False
+                            if (
+                                spell_casters["spells"][check_spell]["classes"]
+                                and identified_spell_level is None
+                                or spell_casters["spells"][check_spell]["item"]
+                            ):
+                                # Check if the current player level could cast this (assuming it is a grouped peer or target mob)
+                                for any_class in spell_casters["spells"][check_spell][
+                                    "classes"
+                                ]:
+                                    if state.char_level is not None:
+                                        if (
+                                            state.char_level
+                                            >= spell_casters["spells"][check_spell][
+                                                "classes"
+                                            ][any_class]
+                                        ):
+                                            player_level_could_cast = True
+
+                                        if (
+                                            identified_spell_level is None
+                                            and spell_casters["spells"][check_spell][
+                                                "item"
+                                            ]
+                                        ):
+                                            for item in spell_items["spells"][
+                                                check_spell
+                                            ]:
+                                                if (
+                                                    spell_items["spells"][check_spell][
+                                                        item
+                                                    ]["cast"]
+                                                    == 0
                                                 ):
-                                                    identified_spell_caster = (
-                                                        recent_cast_event["caster"]
-                                                    )
-                                                    identified_spell_level = (
-                                                        player_list[
-                                                            identified_spell_caster
-                                                        ]["level"]
-                                                    )
-                                                    identified_spell = spell_caster[
-                                                        "spell"
-                                                    ]
-                                                    identified_spell_target = target
-                                # TODO: Maybe add an option to assume your player level if player data is not found and your level is sufficient to cast the identified spell?
+                                                    for clickable_class in spell_items[
+                                                        "spells"
+                                                    ][check_spell][item]["classes"]:
+                                                        if (
+                                                            spell_items["spells"][
+                                                                check_spell
+                                                            ][item]["classes"][
+                                                                clickable_class
+                                                            ]
+                                                            <= state.char_level
+                                                        ):
+                                                            player_level_could_cast = (
+                                                                True
+                                                            )
+
+                                        if player_level_could_cast:
+                                            identified_spell_level = state.char_level
+                                        else:
+                                            identified_spell_level = 60
+
+                                        identified_spell_caster = recent_cast_event[
+                                            "caster"
+                                        ]
+                                        identified_spell = check_spell
+                                        identified_spell_target = target
 
         # We know the spell which landed
         else:
-            if state.debug:
-                eqa_settings.log("Checking for spell: " + spell)
             # If we have spell_caster info on this spell
             if spell in spell_casters["spells"].keys():
-                # Check if player has cast anything
-                if spell_casting_buffer_you and state.char_level is not None:
-                    # If the spell cast by the player is in the spell casters file
-                    if (
-                        spell_casting_buffer_you["spell"]
-                        in spell_casters["spells"].keys()
-                    ):
-                        # If most recent player cast spell occurred spell time ago to this spell landing
-                        if (
-                            int(
-                                (
-                                    datetime.datetime.strptime(line_time, "%H:%M:%S.%f")
-                                    - datetime.datetime.strptime(
-                                        spell_casting_buffer_you["time"], "%H:%M:%S.%f"
-                                    )
-                                    - datetime.timedelta(
-                                        seconds=float(
-                                            spell_timers["spells"][
-                                                spell_casting_buffer_you["spell"]
-                                            ]["cast_time"]
-                                        )
-                                    )
-                                ).total_seconds()
-                            )
-                            == 0
-                        ):
-                            identified_spell_caster = state.char.lower()
-                            identified_spell_level = state.char_level
-                            identified_spell = spell_casting_buffer_you["spell"]
+                # If what just landed is what the active player last cast
+                if (
+                    spell_casting_buffer_you
+                    and state.char_level is not None
+                    and state.char_class is not None
+                ):
+                    if spell == spell_casting_buffer_you["spell"]:
+                        # First check if the active player could have cast this
+                        cast_duration = spell_timers["spells"][
+                            spell_casting_buffer_you["spell"]
+                        ]["cast_time"]
+                        identified = action_spell_timer_player_cast_check(
+                            line_time,
+                            spell_casting_buffer_you["time"],
+                            cast_duration,
+                            state.char.lower(),
+                            state.char_level,
+                            state.char_class.lower(),
+                            spell_casting_buffer_you["spell"],
+                            spell_casters,
+                        )
+                        if identified is not None:
+                            identified_spell_caster = identified[0]
+                            identified_spell_level = identified[1]
+                            identified_spell = identified[2]
                             identified_spell_target = target
-                            find_time = True
-                        # This spell has no listed classes listed and can be an item cast and you cast it
-                        elif (
-                            not spell_casters["spells"][spell]["classes"]
-                            and spell_casters["spells"][spell]["item"]
+
+                        # Check if active player could have clicked this spell
+                        elif spell_casters["spells"][spell]["item"]:
+                            for item in spell_items["spells"][spell]:
+                                cast_duration = spell_items["spells"][spell][item][
+                                    "cast"
+                                ]
+                                if cast_duration > 0:
+                                    identified = action_spell_timer_player_click_check(
+                                        line_time,
+                                        spell_casting_buffer_you["time"],
+                                        cast_duration,
+                                        state.char.lower(),
+                                        state.char_level,
+                                        state.char_class.lower(),
+                                        spell,
+                                        spell_items,
+                                        item,
+                                    )
+                                    if identified is not None:
+                                        identified_spell_caster = identified[0]
+                                        identified_spell_level = identified[1]
+                                        identified_spell = identified[2]
+                                        identified_spell_target = target
+
+                # Check if another player cast this spell
+                if identified_spell_level is None:
+                    for recent_cast_event in spell_casting_buffer_other:
+                        caster_name = recent_cast_event["caster"]
+                        cast_duration = spell_timers["spells"][spell]["cast_time"]
+                        # If we know the class/level of the caster
+                        if caster_name in player_list.keys():
+                            caster_class = player_list[caster_name]["class"]
+                            caster_level = player_list[caster_name]["level"]
+                            if caster_class is not None and caster_level > 0:
+                                # Check if another player could cast this possible spell
+                                identified = action_spell_timer_player_cast_check(
+                                    line_time,
+                                    recent_cast_event["time"],
+                                    cast_duration,
+                                    caster_name,
+                                    caster_level,
+                                    caster_class,
+                                    spell,
+                                    spell_casters,
+                                )
+                                if identified is not None:
+                                    identified_spell_caster = identified[0]
+                                    identified_spell_level = identified[1]
+                                    identified_spell = identified[2]
+                                    identified_spell_target = target
+                                # Check if another player used a clicky
+                                elif spell_casters["spells"][spell]["item"]:
+                                    for item in spell_items["spells"][spell]:
+                                        cast_duration = spell_items["spells"][spell][
+                                            item
+                                        ]["cast"]
+                                        # Non-zero click casts have spell casting messages
+                                        if cast_duration > 0:
+                                            identified = (
+                                                action_spell_timer_player_click_check(
+                                                    line_time,
+                                                    recent_cast_event["time"],
+                                                    cast_duration,
+                                                    caster_name,
+                                                    caster_level,
+                                                    caster_class,
+                                                    spell,
+                                                    spell_items,
+                                                    item,
+                                                )
+                                            )
+                                            if identified is not None:
+                                                identified_spell_caster = identified[0]
+                                                identified_spell_level = identified[1]
+                                                identified_spell = identified[2]
+                                                identified_spell_target = target
+                                        # Instant click cast event but self only spell
+                                        elif (
+                                            spell_casters["spells"][spell]["self"]
+                                            and recent_cast_event["caster"] == target
+                                        ):
+                                            identified = (
+                                                action_spell_timer_player_click_check(
+                                                    line_time,
+                                                    recent_cast_event["time"],
+                                                    cast_duration,
+                                                    caster_name,
+                                                    caster_level,
+                                                    caster_class,
+                                                    spell,
+                                                    spell_items,
+                                                    item,
+                                                )
+                                            )
+                                            if identified is not None:
+                                                identified_spell_caster = identified[0]
+                                                identified_spell_level = identified[1]
+                                                identified_spell = identified[2]
+                                                identified_spell_target = target
+
+                # Haven't found anything yet, check if it could be an instant click (these have no casting messages)
+                if identified_spell_level is None and target == state.char.lower():
+                    if spell in spell_items["spells"].keys():
+                        for item in spell_items["spells"][spell]:
+                            if spell_items["spells"][spell][item]["cast"] == 0:
+                                identified = action_spell_timer_player_click_check(
+                                    line_time,
+                                    line_time,
+                                    0,
+                                    state.char.lower(),
+                                    state.char_level,
+                                    state.char_class.lower(),
+                                    spell,
+                                    spell_items,
+                                    item,
+                                )
+                                if identified is not None:
+                                    identified_spell_caster = identified[0]
+                                    identified_spell_level = identified[1]
+                                    identified_spell = identified[2]
+                                    identified_spell_target = target
+
+                # Time to guess the spell level
+                if identified_spell_level is None and state.spell_timer_guess:
+                    for recent_cast_event in spell_casting_buffer_other:
+                        # If this is a known npc only spell, just set to current player level
+                        if (
+                            spell_casters["spells"][spell]["npc"]
+                            and state.char_level is not None
+                            and identified_spell_level is None
                         ):
-                            identified_spell_caster = state.char.lower()
+                            identified_spell_caster = recent_cast_event["caster"]
                             identified_spell_level = state.char_level
-                            identified_spell = spell_casting_buffer_you["spell"]
+                            identified_spell = spell
                             identified_spell_target = target
-                            find_time = True
-                        # The spell cannot be cast by your class and can be an item cast and you cast it but not spell cast time ago
-                        # elif (
-                        #    state.char_class.lower()
-                        #    not in spell_casters["spells"][spell]["classes"].keys()
-                        #    and spell_casters["spells"][spell]["item"]
-                        # ):
-                        #    # TODO: This is where item cast durations would be checked
-                        #    if state.spell_timer_guess:
-                        #        identified_spell_caster = state.char.lower()
-                        #        identified_spell_level = state.char_level
-                        #        identified_spell = spell_casting_buffer_you["spell"]
-                        #        identified_spell_target = target
-                        #        find_time = True
 
-                # Check for matching spell cast event
-                if not find_time:
-                    for recent_cast_event in spell_casting_buffer_other:
-                        if state.debug:
-                            eqa_settings.log("Checking " + recent_cast_event["caster"])
+                        # If a player could cast this
+                        player_level_could_cast = False
                         if (
-                            int(
-                                (
-                                    datetime.datetime.strptime(line_time, "%H:%M:%S.%f")
-                                    - datetime.datetime.strptime(
-                                        recent_cast_event["time"], "%H:%M:%S.%f"
-                                    )
-                                    - datetime.timedelta(
-                                        seconds=float(
-                                            spell_timers["spells"][spell]["cast_time"]
-                                        )
-                                    )
-                                ).total_seconds()
-                            )
-                            == 0
+                            spell_casters["spells"][spell]["classes"]
+                            and identified_spell_level is None
                         ):
-                            if state.debug:
-                                eqa_settings.log(
-                                    "Checking player info for "
-                                    + recent_cast_event["caster"]
-                                )
-                            # Do we have player info on the likely caster?
-                            if recent_cast_event["caster"] in player_list.keys():
-                                player_class = player_list[recent_cast_event["caster"]][
-                                    "class"
-                                ]
-                                player_level = player_list[recent_cast_event["caster"]][
-                                    "level"
-                                ]
-                                if player_class is not None and player_level > 0:
+                            # Check if the current player level could cast this (assuming it is a grouped peer or target mob)
+                            for any_class in spell_casters["spells"][spell]["classes"]:
+                                if (
+                                    state.char_level is not None
+                                    and identified_spell_level is None
+                                ):
                                     if (
-                                        player_class
-                                        in spell_casters["spells"][spell][
-                                            "classes"
-                                        ].keys()
+                                        state.char_level
+                                        >= spell_casters["spells"][spell]["classes"][
+                                            any_class
+                                        ]
                                     ):
-                                        player_level = int(
-                                            player_list[recent_cast_event["caster"]][
-                                                "level"
-                                            ]
-                                        )
-                                        if (
-                                            int(
-                                                spell_casters["spells"][spell][
-                                                    "classes"
-                                                ][player_class]
-                                            )
-                                            <= player_level
-                                        ):
-                                            identified_spell_caster = recent_cast_event[
-                                                "caster"
-                                            ]
-                                            identified_spell_level = player_list[
-                                                identified_spell_caster
-                                            ]["level"]
-                                            identified_spell = spell
-                                            identified_spell_target = target
-                                            find_time = True
-                                            if state.debug:
-                                                eqa_settings.log(
-                                                    "Found spell cast by "
-                                                    + identified_spell_caster
-                                                )
-                            # Time to guess the spell level
-                            elif state.spell_timer_guess:
-                                if state.debug:
-                                    eqa_settings.log("Into spell guessing territory")
-                                player_level_could_cast = False
-                                # If a player could cast this
-                                if spell_casters["spells"][spell]["classes"]:
-                                    # Check if the current player level could cast this (assuming it is a grouped peer or target mob)
-                                    for caster_class in spell_casters["spells"][spell][
-                                        "classes"
-                                    ]:
-                                        if state.char_level is not None:
-                                            if state.char_level >= int(
-                                                spell_casters["spells"][spell][
-                                                    "classes"
-                                                ][caster_class]
+                                        player_level_could_cast = True
+
+                                    if (
+                                        identified_spell_level is None
+                                        and spell_casters["spells"][spell]["item"]
+                                    ):
+                                        for item in spell_items["spells"][spell]:
+                                            if (
+                                                spell_items["spells"][spell][item][
+                                                    "cast"
+                                                ]
+                                                == 0
                                             ):
-                                                player_level_could_cast = True
+                                                for clickable_class in spell_items[
+                                                    "spells"
+                                                ][spell][item]["classes"]:
+                                                    if (
+                                                        spell_items["spells"][spell][
+                                                            item
+                                                        ]["classes"][clickable_class]
+                                                        <= state.char_level
+                                                    ):
+                                                        player_level_could_cast = True
 
                                     if player_level_could_cast:
                                         identified_spell_level = state.char_level
                                     else:
                                         identified_spell_level = 60
 
                                     identified_spell_caster = recent_cast_event[
                                         "caster"
                                     ]
                                     identified_spell = spell
                                     identified_spell_target = target
-                                    find_time = True
-
-                                # If this is a known npc only spell, just set to current player level
-                                elif (
-                                    spell_casters["spells"][spell]["npc"]
-                                    and state.char_level is not None
-                                ):
-                                    identified_spell_caster = recent_cast_event[
-                                        "caster"
-                                    ]
-                                    identified_spell_level = state.char_level
-                                    identified_spell = spell
-                                    identified_spell_target = target
-                                    find_time = True
 
-        if find_time:
+        if identified_spell_level is not None:
             make_timer = True
 
             # Guild Only Filter
             if state.spell_timer_guild_only and state.char_guild is not None:
                 # If this was cast by myself or another player
                 if identified_spell_caster in player_list.keys():
                     # If a guildie didn't cast it
```

### Comparing `eqalert-3.5.2/eqa/lib/config.py` & `eqalert-3.5.3/eqa/lib/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -109,28 +109,28 @@
         ## Pets
         config_path_line_pets = base_path + "config/line-alerts/pets.json"
         json_data = open(config_path_line_pets, "r", encoding="utf-8")
         config_file_line_alerts = json.load(json_data)
         json_data.close()
         line_alerts["line"].update(config_file_line_alerts["line"])
 
-        ## Chat Recieved NPC
-        config_path_line_chat_recieved_npc = (
+        ## Chat Received NPC
+        config_path_line_chat_received_npc = (
             base_path + "config/line-alerts/chat-received-npc.json"
         )
-        json_data = open(config_path_line_chat_recieved_npc, "r", encoding="utf-8")
+        json_data = open(config_path_line_chat_received_npc, "r", encoding="utf-8")
         config_file_line_alerts = json.load(json_data)
         json_data.close()
         line_alerts["line"].update(config_file_line_alerts["line"])
 
-        ## Chat Recieved
-        config_path_line_chat_recieved = (
+        ## Chat Received
+        config_path_line_chat_received = (
             base_path + "config/line-alerts/chat-received.json"
         )
-        json_data = open(config_path_line_chat_recieved, "r", encoding="utf-8")
+        json_data = open(config_path_line_chat_received, "r", encoding="utf-8")
         config_file_line_alerts = json.load(json_data)
         json_data.close()
         line_alerts["line"].update(config_file_line_alerts["line"])
 
         ## Chat Sent
         config_path_line_chat_sent = base_path + "config/line-alerts/chat-sent.json"
         json_data = open(config_path_line_chat_sent, "r", encoding="utf-8")
@@ -492,4685 +492,5400 @@
             "get spell casters: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
+def get_spell_items(data_path):
+    """Return spell items file"""
+
+    try:
+        spell_items_file = data_path + "spell-items.json"
+        json_data = open(spell_items_file, "r", encoding="utf-8")
+        spell_items = json.load(json_data)
+        json_data.close()
+
+        return spell_items
+
+    except Exception as e:
+        eqa_settings.log(
+            "get spell items: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
 def update_spell_casters(data_path, version):
     """Update data/spell-casters.json"""
 
     new_spell_caster_data = """
-
 {
   "spells": {
     "aanyas_quickening": {
       "classes": {
-        "enchanter": "53"
+        "enchanter": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "accuracy": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "acid_jet": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "acumen": {
       "classes": {
         "shaman": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "adorning_grace": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "adroitness": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aegis": {
       "classes": {
         "cleric": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "aegis_of_bathezid": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aegis_of_ro": {
       "classes": {
         "magician": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "aegolism": {
       "classes": {
         "cleric": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "affliction": {
       "classes": {
         "shaman": 19
       },
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "agility": {
       "classes": {
         "shaman": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "agilmentes_aria_of_eagles": {
       "classes": {
         "bard": 31
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "alacrity": {
       "classes": {
-        "enchanter": "24",
+        "enchanter": 24,
         "shaman": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "allure": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "allure_of_death": {
       "classes": {
         "necromancer": 20
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "allure_of_the_wild": {
       "classes": {
         "druid": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "alluring_aura": {
       "classes": {
         "shaman": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "alluring_whispers": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "aloe_sweat": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "ancient_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "anthem_de_arms": {
       "classes": {
         "bard": 10
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "arch_lich": {
       "classes": {
         "necromancer": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "arch_shielding": {
       "classes": {
-        "enchanter": "44",
+        "enchanter": 44,
         "magician": 44,
         "necromancer": 44,
         "wizard": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "armor_of_faith": {
       "classes": {
         "cleric": 39,
         "paladin": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "armor_of_protection": {
       "classes": {
         "cleric": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "asphyxiate": {
       "classes": {
-        "enchanter": "59"
+        "enchanter": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "assiduous_vision": {
       "classes": {
         "shaman": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "asystole": {
       "classes": {
         "necromancer": 44,
         "shadow knight": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "atols_spectral_shackles": {
       "classes": {
         "wizard": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "augment": {
       "classes": {
-        "enchanter": "56"
+        "enchanter": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "augment_death": {
       "classes": {
         "necromancer": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "augmentation": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "augmentation_of_death": {
       "classes": {
         "necromancer": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "aura_of_antibody": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_battle": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_black_petals": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_blue_petals": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_cold": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_green_petals": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_heat": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_marr": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_purity": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_red_petals": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "aura_of_white_petals": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "avatar": {
       "classes": {
-        "shaman": "60"
+        "shaman": 60
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "avatar_snare": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "bane_of_nife": {
       "classes": {
         "shaman": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "banshee_aura": {
       "classes": {
         "necromancer": 16,
         "shadow knight": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "barbcoat": {
       "classes": {
         "druid": 19,
         "ranger": 30
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "barrier_of_combustion": {
       "classes": {
         "magician": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "barrier_of_force": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "battery_vision": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "bedlam": {
       "classes": {
-        "enchanter": "58"
+        "enchanter": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "befriend_animal": {
       "classes": {
         "druid": 14,
         "shaman": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "beguile": {
       "classes": {
-        "enchanter": "24"
+        "enchanter": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "beguile_animals": {
       "classes": {
         "druid": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "beguile_plants": {
       "classes": {
         "druid": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "beguile_undead": {
       "classes": {
         "necromancer": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "bellowing_winds": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "berserker_madness_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "berserker_madness_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "berserker_madness_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "berserker_madness_iv": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "berserker_spirit": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "berserker_strength": {
       "classes": {
-        "enchanter": "20"
+        "enchanter": 20
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "bind_sight": {
       "classes": {
-        "enchanter": "8",
+        "enchanter": 8,
         "ranger": 22,
         "wizard": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "bladecoat": {
       "classes": {
         "druid": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "blessing_of_nature": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "blessing_of_the_grove": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": true
+      "self": true
     },
     "blinding_fear": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "blinding_luminance": {
       "classes": {
         "cleric": 34,
         "shaman": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "blinding_poison_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
+    },
+    "blinding_poison_ii": {
+      "classes": {},
+      "item": true,
+      "npc": true,
+      "self": false
     },
     "blinding_poison_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "blinding_step": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "blood_claw": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "bobbing_corpse": {
       "classes": {
         "shadow knight": 55
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "boil_blood": {
       "classes": {
         "necromancer": 29,
         "shadow knight": 53
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "boiling_blood": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "boltrans_agacerie": {
       "classes": {
-        "enchanter": "53"
+        "enchanter": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "bond_of_death": {
       "classes": {
         "necromancer": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "bonds_of_force": {
       "classes": {
         "wizard": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "bonds_of_tunare": {
       "classes": {
         "druid": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "bone_melt": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "boon_of_immolation": {
       "classes": {
         "magician": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "boon_of_the_clear_mind": {
       "classes": {
-        "enchanter": "52"
+        "enchanter": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "boon_of_the_garou": {
       "classes": {
-        "enchanter": "44"
+        "enchanter": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "bramblecoat": {
       "classes": {
         "druid": 29,
         "ranger": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "bravery": {
       "classes": {
         "cleric": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "breath_of_ro": {
       "classes": {
         "druid": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "breath_of_the_dead": {
       "classes": {
         "necromancer": 24,
         "shadow knight": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "breath_of_the_sea": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "breeze": {
       "classes": {
-        "enchanter": "16"
+        "enchanter": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "brilliance": {
       "classes": {
-        "enchanter": "44"
+        "enchanter": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "brittle_haste_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "brittle_haste_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "brittle_haste_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "brittle_haste_iv": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "bulwark_of_faith": {
       "classes": {
         "cleric": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "burnout": {
       "classes": {
-        "magician": 255
+        "magician": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "burnout_ii": {
       "classes": {
         "magician": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "burnout_iii": {
       "classes": {
         "magician": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "burnout_iv": {
       "classes": {
         "magician": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "burrowing_scarab": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "burst_of_strength": {
       "classes": {
         "shaman": 14
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cadeau_of_flame": {
       "classes": {
         "magician": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cajole_undead": {
       "classes": {
         "necromancer": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "calimony": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "call_of_bones": {
       "classes": {
         "necromancer": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "call_of_earth": {
       "classes": {
         "ranger": 50
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "call_of_karana": {
       "classes": {
         "druid": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "call_of_sky": {
       "classes": {
         "ranger": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "call_of_the_predator": {
       "classes": {
         "ranger": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "calm": {
       "classes": {
         "cleric": 19,
         "enchanter": "20",
         "paladin": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "calm_animal": {
       "classes": {
         "druid": 19,
         "ranger": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "camouflage": {
       "classes": {
         "druid": 5,
         "ranger": 15
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "captain_nalots_quickening": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "cascading_darkness": {
       "classes": {
         "necromancer": 49,
         "shadow knight": 59
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "cassindras_chant_of_clarity": {
       "classes": {
         "bard": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cassindras_elegy": {
       "classes": {
         "bard": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cassindras_insipid_ditty": {
       "classes": {
         "bard": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cast_sight": {
       "classes": {
-        "enchanter": "34"
+        "enchanter": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "celerity": {
       "classes": {
-        "enchanter": "39",
+        "enchanter": 39,
         "shaman": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "celestial_cleansing": {
       "classes": {
         "paladin": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "celestial_healing": {
       "classes": {
         "cleric": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "celestial_tranquility": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "center": {
       "classes": {
         "cleric": 9,
         "paladin": 22
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cessation_of_cor": {
       "classes": {
         "necromancer": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "chant_of_battle": {
       "classes": {
         "bard": 1
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "charisma": {
       "classes": {
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "chase_the_moon": {
       "classes": {
-        "enchanter": "16"
+        "enchanter": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "chill_bones": {
       "classes": {
         "necromancer": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "chill_of_unlife": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "chill_sight": {
       "classes": {
         "ranger": 56,
         "wizard": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "chilling_embrace": {
       "classes": {
         "necromancer": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "chloroplast": {
       "classes": {
         "druid": 44,
         "ranger": 55,
         "shaman": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "choke": {
       "classes": {
-        "enchanter": "12"
+        "enchanter": 12
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "chords_of_dissonance": {
       "classes": {
         "bard": 2
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "cindas_charismatic_carillon": {
       "classes": {
         "bard": 11
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "circle_of_summer": {
       "classes": {
         "druid": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "circle_of_winter": {
       "classes": {
         "druid": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "clarity": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "clarity_ii": {
       "classes": {
-        "enchanter": "54"
+        "enchanter": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "clinging_darkness": {
       "classes": {
         "necromancer": 4,
         "shadow knight": 15
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "clockwork_poison": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "cloud": {
       "classes": {
-        "enchanter": "20"
+        "enchanter": 20
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "cloud_of_disempowerment": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "cloud_of_fear": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "cloud_of_silence": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "cog_boost": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "cohesion": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "composition_of_ervaj": {
       "classes": {
         "bard": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "courage": {
       "classes": {
         "cleric": 1,
         "paladin": 9
       },
+      "item": false,
       "npc": false,
-      "item": true
+      "self": false
     },
     "creeping_crud": {
       "classes": {
         "druid": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "creeping_vision": {
       "classes": {
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "cripple": {
       "classes": {
-        "enchanter": "53",
+        "enchanter": 53,
         "shaman": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "crissions_pixie_strike": {
       "classes": {
         "bard": 28
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "curse_of_the_simple_mind": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "curse_of_the_spirits": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "dance_of_the_blade": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "daring": {
       "classes": {
         "cleric": 19,
         "paladin": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "dark_pact": {
       "classes": {
         "necromancer": 8
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "dawncall": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "dazzle": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "dead_man_floating": {
       "classes": {
         "necromancer": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "dead_men_floating": {
       "classes": {
         "necromancer": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "deadeye": {
       "classes": {
         "necromancer": 8,
         "shadow knight": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "deadly_poison": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "deadly_velium_poison": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "death_pact": {
       "classes": {
         "cleric": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "deftness": {
       "classes": {
         "shaman": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "deliriously_nimble": {
       "classes": {
         "shaman": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "demi_lich": {
       "classes": {
         "necromancer": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "denons_bereavement": {
       "classes": {
         "bard": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "denons_disruptive_discord": {
       "classes": {
         "bard": 18
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "desperate_hope": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "devouring_darkness": {
       "classes": {
         "necromancer": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "dexterity": {
       "classes": {
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "dexterous_aura": {
       "classes": {
         "shaman": 1
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "diamondskin": {
       "classes": {
         "necromancer": 44,
         "shadow knight": 59,
         "wizard": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "dictate": {
       "classes": {
-        "enchanter": "60"
+        "enchanter": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "disease": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "disease_cloud": {
       "classes": {
         "necromancer": 1,
         "shadow knight": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "diseased_cloud": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "disempower": {
       "classes": {
-        "enchanter": "16",
+        "enchanter": 16,
         "shaman": 14
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "divine_aura": {
       "classes": {
         "cleric": 1,
         "paladin": 55
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "divine_barrier": {
       "classes": {
         "cleric": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "divine_favor": {
       "classes": {
         "paladin": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "divine_glory": {
       "classes": {
         "paladin": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "divine_intervention": {
       "classes": {
         "cleric": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "divine_might": {
       "classes": {
         "paladin": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "divine_purpose": {
       "classes": {
         "paladin": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "divine_strength": {
       "classes": {
         "paladin": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "dizzy_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "dizzy_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "dizzy_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "dizzy_iv": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "dominate_undead": {
       "classes": {
         "necromancer": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "dooming_darkness": {
       "classes": {
         "necromancer": 29,
         "shadow knight": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "draconic_rage": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "dragon_charm": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "dragon_roar": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "drifting_death": {
       "classes": {
         "druid": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "drones_of_doom": {
       "classes": {
         "druid": 34,
         "ranger": 54
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "drowsy": {
       "classes": {
         "shaman": 5
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "dulsehound": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "dyns_dizzying_draught": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "earthcall": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "earthelementalattack": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "ebbing_strength": {
       "classes": {
-        "enchanter": "12"
+        "enchanter": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "echinacea_infusion": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "elemental_armor": {
       "classes": {
         "magician": 44,
         "wizard": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "elemental_maelstrom": {
       "classes": {
         "magician": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "elemental_rhythms": {
       "classes": {
         "bard": 9
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "elemental_shield": {
       "classes": {
         "magician": 20,
         "wizard": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "embrace_of_the_kelpmaiden": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "endure_cold": {
       "classes": {
         "cleric": 14,
         "druid": 9,
         "necromancer": 4,
         "ranger": 22,
         "shadow knight": 15,
         "shaman": 1
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "endure_disease": {
       "classes": {
         "cleric": 14,
         "druid": 19,
         "paladin": 39,
         "shadow knight": 30,
         "shaman": 9,
         "necromancer": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "endure_fire": {
       "classes": {
         "cleric": 9,
         "druid": 1,
         "ranger": 9,
         "shaman": 5
       },
+      "item": false,
       "npc": false,
-      "item": true
+      "self": false
     },
     "endure_magic": {
       "classes": {
         "cleric": 19,
         "druid": 34,
-        "enchanter": "20",
+        "enchanter": 20,
         "paladin": 30,
         "shaman": 19
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "endure_poison": {
       "classes": {
         "cleric": 9,
         "druid": 19,
         "paladin": 22,
         "shaman": 14
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "enduring_breath": {
       "classes": {
         "druid": 9,
-        "enchanter": "12",
+        "enchanter": 12,
         "ranger": 22,
         "shaman": 14
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "energy_sap": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "enfeeblement": {
       "classes": {
-        "enchanter": "4"
+        "enchanter": 4
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "engulfing_darkness": {
       "classes": {
         "necromancer": 12,
         "shadow knight": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "enlightenment": {
       "classes": {
-        "enchanter": "57"
+        "enchanter": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "enslave_death": {
       "classes": {
         "necromancer": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "ensnare": {
       "classes": {
         "druid": 29,
         "ranger": 51
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "enthrall": {
       "classes": {
-        "enchanter": "16"
+        "enchanter": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "entrance": {
       "classes": {
-        "enchanter": "34"
+        "enchanter": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "envenomed_bolt": {
       "classes": {
         "necromancer": 51,
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "envenomed_breath": {
       "classes": {
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "everlasting_breath": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "expedience": {
       "classes": {
         "magician": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "extended_regeneration": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "eye_of_confusion": {
       "classes": {
-        "enchanter": "8"
+        "enchanter": 8
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "eye_of_tallon": {
       "classes": {
         "magician": 57,
         "wizard": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "eye_of_zomm": {
       "classes": {
         "magician": 8,
         "wizard": 8
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "eyes_of_the_cat": {
       "classes": {
         "ranger": 30
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "fascination": {
       "classes": {
-        "enchanter": "52"
+        "enchanter": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "feast_of_blood": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "feckless_might": {
       "classes": {
-        "enchanter": "20"
+        "enchanter": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "feeble_poison": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "feedback": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self ": false
     },
     "feet_like_cat": {
       "classes": {
         "ranger": 15,
         "shaman": 5
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "fellspine": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "feral_spirit": {
       "classes": {
         "druid": 19
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "fetter": {
       "classes": {
-        "enchanter": "58",
+        "enchanter": 58,
         "wizard": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "fiery_might": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "fire": {
       "classes": {
         "druid": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "firefist": {
       "classes": {
         "druid": 9,
         "ranger": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "fist_of_water": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "fixation_of_ro": {
       "classes": {
         "druid": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "flame_lick": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "flash_of_light": {
       "classes": {
         "cleric": 1,
         "paladin": 9,
         "shaman": 1
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "fleeting_fury": {
       "classes": {
         "shaman": 5
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "flesh_rot_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "flesh_rot_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "flesh_rot_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "flurry": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "focus_of_spirit": {
       "classes": {
         "shaman": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "forlorn_deeds": {
       "classes": {
-        "enchanter": "57"
+        "enchanter": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "form_of_the_great_bear": {
       "classes": {
         "shaman": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "form_of_the_great_wolf": {
       "classes": {
         "druid": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "form_of_the_howler": {
       "classes": {
         "druid": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "form_of_the_hunter": {
       "classes": {
         "druid": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "fortitude": {
       "classes": {
         "cleric": 55
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "freezing_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "frenzied_strength": {
       "classes": {
         "cleric": 34,
         "paladin": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "frenzy": {
       "classes": {
         "shaman": 19
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "froglok_poison": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "frost_storm": {
       "classes": {
         "wizard": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "frostbite": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "frostreavers_blessing": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "fufils_curtailing_chant": {
       "classes": {
-        "bard": "30"
+        "bard": 30
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "fungal_regrowth": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "fungus_spores": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "furious_strength": {
       "classes": {
         "shaman": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "fury": {
       "classes": {
         "shaman": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "garzicors_vengeance": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "gasping_embrace": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "gaze": {
       "classes": {
         "wizard": 12
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "gift_of_brilliance": {
       "classes": {
-        "enchanter": "60"
+        "enchanter": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "gift_of_insight": {
       "classes": {
-        "enchanter": "55"
+        "enchanter": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "gift_of_magic": {
       "classes": {
-        "enchanter": "34"
+        "enchanter": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "gift_of_pure_thought": {
       "classes": {
-        "enchanter": "59"
+        "enchanter": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "girdle_of_karana": {
       "classes": {
         "druid": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "glamour": {
       "classes": {
         "shaman": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "glamour_of_kintaz": {
       "classes": {
-        "enchanter": "54"
+        "enchanter": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "glamour_of_tunare": {
       "classes": {
         "druid": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "glimpse": {
       "classes": {
         "druid": 4,
         "ranger": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "graveyard_dust": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "grease_injection": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "greater_shielding": {
       "classes": {
-        "enchanter": "34",
+        "enchanter": 34,
         "magician": 34,
         "necromancer": 34,
         "wizard": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "greater_wolf_form": {
       "classes": {
         "druid": 34,
         "ranger": 56
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "greenmist": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "grim_aura": {
       "classes": {
         "necromancer": 4,
         "shadow knight": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "group_resist_magic": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "guard": {
       "classes": {
         "cleric": 29,
         "paladin": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "guardian": {
       "classes": {
         "shaman": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "guardian_rhythms": {
       "classes": {
         "bard": 17
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "harmony": {
       "classes": {
         "druid": 5,
         "ranger": 22
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "harmshield": {
       "classes": {
         "necromancer": 20
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "harpy_voice": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "haste": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "haze": {
       "classes": {
-        "enchanter": "4"
+        "enchanter": 4
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "health": {
       "classes": {
         "shaman": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "heart_flutter": {
       "classes": {
         "necromancer": 16,
         "shadow knight": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "heat_blood": {
       "classes": {
         "necromancer": 12,
         "shadow knight": 30
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "heat_sight": {
       "classes": {
         "wizard": 16
       },
+      "item": false,
       "npc": false,
-      "item": true
+      "self": true
     },
     "heroic_bond": {
       "classes": {
         "cleric": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "heroism": {
       "classes": {
         "cleric": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "holy_armor": {
       "classes": {
         "cleric": 5,
         "paladin": 15
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "hug": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "hymn_of_restoration": {
       "classes": {
         "bard": 6
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "ice": {
       "classes": {
         "druid": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "ice_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "ice_strike": {
       "classes": {
         "shaman": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "ignite_blood": {
       "classes": {
         "necromancer": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "ignite_bones": {
       "classes": {
         "necromancer": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "ikatiars_revenge": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "immolate": {
       "classes": {
         "druid": 29,
         "ranger": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "immolating_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "impart_strength": {
       "classes": {
         "necromancer": 8
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "incapacitate": {
       "classes": {
-        "enchanter": "44",
+        "enchanter": 44,
         "shaman": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "infectious_cloud": {
       "classes": {
         "necromancer": 16,
         "shaman": 19
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "inferno_shield": {
       "classes": {
         "magician": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "inner_fire": {
       "classes": {
         "shaman": 1
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "insidious_decay": {
       "classes": {
         "shaman": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "insidious_fever": {
       "classes": {
         "shaman": 19
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "insidious_malady": {
       "classes": {
         "shaman": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "insight": {
       "classes": {
-        "enchanter": "255"
+        "enchanter": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "insipid_weakness": {
       "classes": {
-        "enchanter": "34"
+        "enchanter": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "inspire_fear": {
       "classes": {
         "cleric": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "intensify_death": {
       "classes": {
         "necromancer": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "invigor": {
       "classes": {
         "cleric": 9,
         "druid": 14,
-        "enchanter": "24",
+        "enchanter": 24,
         "paladin": 22,
         "ranger": 30,
         "shaman": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "jonthans_inspiration": {
       "classes": {
         "bard": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "jonthans_provocation": {
       "classes": {
         "bard": 45
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "jonthans_whistling_warsong": {
       "classes": {
         "bard": 7
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "kazumis_note_of_preservation": {
       "classes": {
         "bard": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "kelins_lucid_lullaby": {
       "classes": {
         "bard": 15
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "kelins_lugubrious_lament": {
       "classes": {
         "bard": 8
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "kilvas_skin_of_flame": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "kylies_venom": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "languid_pace": {
       "classes": {
-        "enchanter": "12"
+        "enchanter": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "largarns_lamentation": {
       "classes": {
-        "enchanter": "55"
+        "enchanter": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "largos_absonant_binding": {
       "classes": {
         "bard": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "largos_melodic_binding": {
       "classes": {
         "bard": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "leach": {
       "classes": {
         "necromancer": 12
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "leatherskin": {
       "classes": {
         "necromancer": 24,
         "wizard": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "legacy_of_spike": {
       "classes": {
         "druid": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "legacy_of_thorn": {
       "classes": {
         "druid": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "lesser_shielding": {
       "classes": {
-        "enchanter": "8",
+        "enchanter": 8,
         "magician": 8,
         "necromancer": 8,
         "wizard": 8
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "levitate": {
       "classes": {
         "druid": 14,
-        "enchanter": "16",
+        "enchanter": 16,
         "ranger": 39,
         "shaman": 14,
         "wizard": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "levitation": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "lich": {
       "classes": {
         "necromancer": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "listless_power": {
       "classes": {
-        "enchanter": "29",
+        "enchanter": 29,
         "shaman": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "lower_resists_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "lower_resists_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "lower_resists_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "lower_resists_iv": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "lull": {
       "classes": {
         "cleric": 1,
-        "enchanter": "1",
+        "enchanter": 1,
         "paladin": 15
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "lull_animal": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "lyssas_solidarity_of_vision": {
       "classes": {
         "bard": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "lyssas_veracious_concord": {
       "classes": {
         "bard": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "magi_curse": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "magnify": {
       "classes": {
         "wizard": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "major_shielding": {
       "classes": {
-        "enchanter": "24",
+        "enchanter": 24,
         "magician": 24,
         "necromancer": 24,
         "wizard": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "mala": {
       "classes": {
         "magician": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "malevolent_grasp": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "malo": {
       "classes": {
         "shaman": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "malosi": {
       "classes": {
         "magician": 51,
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "malosini": {
       "classes": {
         "magician": 58,
         "shaman": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "mana_flare": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "mana_shroud": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "manasink": {
       "classes": {
         "wizard": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "manaskin": {
       "classes": {
         "necromancer": 52,
         "wizard": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "maniacal_strength": {
       "classes": {
         "shaman": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "manticore_poison": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "mark_of_karn": {
       "classes": {
         "cleric": 56
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "mask_of_the_hunter": {
       "classes": {
         "druid": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "mcvaxius_berserker_crescendo": {
       "classes": {
         "bard": 42
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "mcvaxius_rousing_rondo": {
       "classes": {
         "bard": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "melody_of_ervaj": {
       "classes": {
         "bard": 50
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "mesmerization": {
       "classes": {
-        "enchanter": "16"
+        "enchanter": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "mesmerize": {
       "classes": {
-        "enchanter": "4"
+        "enchanter": 4
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "mesmerizing_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "mind_cloud": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "minion_of_hate": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": true
+      "self": false
     },
     "minor_shielding": {
       "classes": {
-        "enchanter": "1",
+        "enchanter": 1,
         "magician": 1,
         "necromancer": 1,
         "wizard": 1
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "mist": {
       "classes": {
-        "enchanter": "12"
+        "enchanter": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "mortal_deftness": {
       "classes": {
         "shaman": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "muscle_lock_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "muscle_lock_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "muscle_lock_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "muscle_lock_iv": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "mystic_precision": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "naltrons_mark": {
       "classes": {
         "cleric": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "natures_melody": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "natureskin": {
       "classes": {
         "druid": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "nillipus_march_of_the_wee": {
       "classes": {
         "bard": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "nimble": {
       "classes": {
         "shaman": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "nivs_harmonic": {
       "classes": {
         "bard": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "nivs_melody_of_preservation": {
       "classes": {
         "bard": 47
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "null_aura": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "numb_the_dead": {
       "classes": {
         "necromancer": 4,
         "shadow knight": 15
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "obscure": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "obsidian_shatter": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "occlusion_of_sound": {
       "classes": {
         "bard": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "okeils_flickering_flame": {
       "classes": {
         "wizard": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "okeils_radiation": {
       "classes": {
         "wizard": 4
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "one_hundred_blows": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "overwhelming_splendor": {
       "classes": {
-        "enchanter": "56"
+        "enchanter": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "pacify": {
       "classes": {
         "cleric": 39,
-        "enchanter": "39",
+        "enchanter": 39,
         "paladin": 51
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "pack_chloroplast": {
       "classes": {
         "druid": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "pack_regeneration": {
       "classes": {
         "druid": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "pack_spirit": {
       "classes": {
         "druid": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "pact_of_shadow": {
       "classes": {
         "necromancer": 44
       },
+      "item": false,
       "npc": false,
-      "item": true
+      "self": false
     },
     "panic": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "panic_animal": {
       "classes": {
         "druid": 1,
         "ranger": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "panic_the_dead": {
       "classes": {
         "cleric": 29,
         "necromancer": 29,
         "shadow knight": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "paralyzing_poison_i": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "paralyzing_poison_ii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "paralyzing_poison_iii": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "phantom_armor": {
       "classes": {
         "magician": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "phantom_chain": {
       "classes": {
         "magician": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "phantom_leather": {
       "classes": {
         "magician": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "phantom_plate": {
       "classes": {
         "magician": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "plague": {
       "classes": {
         "necromancer": 52,
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "plagueratdisease": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "plainsight": {
       "classes": {
         "wizard": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "poison": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "poison_bolt": {
       "classes": {
         "necromancer": 4
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "poison_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "power": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "pox_of_bertoxxulous": {
       "classes": {
         "shaman": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "primal_avatar": {
       "classes": {
         "shaman": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "primal_essence": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "prime_healers_blessing": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": true
+      "self": true
     },
     "protect": {
       "classes": {
         "shaman": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "protection_of_the_glades": {
       "classes": {
         "druid": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "psalm_of_cooling": {
       "classes": {
         "bard": 33
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "psalm_of_mystic_shielding": {
       "classes": {
         "bard": 41
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "psalm_of_purity": {
       "classes": {
         "bard": 37
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "psalm_of_vitality": {
       "classes": {
         "bard": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "psalm_of_warmth": {
       "classes": {
         "bard": 25
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "purifying_rhythms": {
       "classes": {
         "bard": 13
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "putrefy_flesh": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "putrid_breath": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "pyrocruor": {
       "classes": {
         "necromancer": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "quickness": {
       "classes": {
-        "enchanter": "16",
+        "enchanter": 16,
         "shaman": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "quivering_veil_of_xarn": {
       "classes": {
         "necromancer": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "rabies": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "radiant_visage": {
       "classes": {
-        "enchanter": "34"
+        "enchanter": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "rage": {
       "classes": {
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "rage_of_tallon": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": true
+      "self": true
     },
     "rage_of_vallon": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "rage_of_zek": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "rampage": {
       "classes": {
-        "enchanter": "39"
+        "enchanter": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "rapture": {
       "classes": {
-        "enchanter": "59"
+        "enchanter": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "reckless_health": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "reckless_strength": {
       "classes": {
         "cleric": 5,
         "paladin": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "regeneration": {
       "classes": {
         "druid": 34,
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "regrowth": {
       "classes": {
         "druid": 54,
         "shaman": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "regrowth_of_the_grove": {
       "classes": {
         "druid": 58
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "rejuvenation": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "repulse_animal": {
       "classes": {
         "druid": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "resist_cold": {
       "classes": {
         "cleric": 39,
         "druid": 34,
         "necromancer": 24,
         "ranger": 55,
         "shadow knight": 39,
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "resist_disease": {
       "classes": {
         "cleric": 39,
         "druid": 44,
         "necromancer": 34,
         "paladin": 51,
         "shaman": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "resist_fire": {
       "classes": {
         "cleric": 34,
         "druid": 24,
         "ranger": 49,
         "shaman": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "resist_magic": {
       "classes": {
         "cleric": 44,
         "druid": 49,
-        "enchanter": "39",
+        "enchanter": 39,
         "paladin": 55,
         "shaman": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "resist_poison": {
       "classes": {
         "cleric": 34,
         "druid": 44,
         "shaman": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "resistance_to_magic": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "resistant_skin": {
       "classes": {
         "wizard": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "resolution": {
       "classes": {
         "cleric": 44,
         "paladin": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "rest_the_dead": {
       "classes": {
         "necromancer": 24,
         "shadow knight": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "resurrection_effects": {
       "classes": {},
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "riotous_health": {
       "classes": {
         "shaman": 54
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "rising_dexterity": {
       "classes": {
         "shaman": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "rodricks_gift": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "ros_fiery_sundering": {
       "classes": {
         "druid": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "rotting_flesh": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "rubicite_aura": {
       "classes": {},
       "npc": false,
-      "item": true
+      "item": false
     },
     "rune_i": {
       "classes": {
-        "enchanter": "16"
+        "enchanter": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "rune_ii": {
       "classes": {
-        "enchanter": "24"
+        "enchanter": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "rune_iii": {
       "classes": {
-        "enchanter": "34"
+        "enchanter": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "rune_iv": {
       "classes": {
-        "enchanter": "44"
+        "enchanter": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "rune_v": {
       "classes": {
-        "enchanter": "52"
+        "enchanter": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "savage_spirit": {
       "classes": {
         "druid": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "scale_of_wolf": {
       "classes": {
         "druid": 24,
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "scale_skin": {
       "classes": {
         "shaman": 5
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "scarab_storm": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "scent_of_darkness": {
       "classes": {
         "necromancer": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "scent_of_dusk": {
       "classes": {
         "necromancer": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "scent_of_shadow": {
       "classes": {
         "necromancer": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "scent_of_terris": {
       "classes": {
         "necromancer": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "scorching_skin": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "scourge": {
       "classes": {
         "necromancer": 39,
         "shaman": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "screaming_mace": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "screaming_terror": {
       "classes": {
         "necromancer": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "sear": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "sebilite_pox": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "see_invisible": {
       "classes": {
         "druid": 14,
-        "enchanter": "8",
+        "enchanter": 8,
         "magician": 16,
         "ranger": 39,
         "wizard": 4
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "seething_fury": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": true
+      "self": true
     },
     "selos_accelerando": {
       "classes": {
         "bard": 4
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "selos_assonant_strane": {
       "classes": {
         "bard": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "selos_chords_of_cessation": {
       "classes": {
         "bard": 48
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "selos_consonant_chain": {
       "classes": {
         "bard": 23
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "selos_song_of_travel": {
       "classes": {
         "bard": 51
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "serpent_sight": {
       "classes": {
-        "enchanter": "12",
+        "enchanter": 12,
         "shaman": 9
       },
+      "item": false,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shade": {
       "classes": {
-        "enchanter": "39"
+        "enchanter": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shadow": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shadow_compact": {
       "classes": {
         "necromancer": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shadow_sight": {
       "classes": {
         "necromancer": 24,
         "shadow knight": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shadow_vortex": {
       "classes": {
         "necromancer": 20,
         "shadow knight": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shadowbond": {
       "classes": {
         "necromancer": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shallow_breath": {
       "classes": {
-        "enchanter": "1"
+        "enchanter": 1
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "share_wolf_form": {
       "classes": {
         "druid": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shauris_sonorous_clouding": {
       "classes": {
         "bard": 19
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shield_of_barbs": {
       "classes": {
         "druid": 19
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shield_of_blades": {
       "classes": {
         "druid": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shield_of_brambles": {
       "classes": {
         "druid": 29,
         "ranger": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shield_of_fire": {
       "classes": {
         "magician": 8
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shield_of_flame": {
       "classes": {
         "magician": 20
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shield_of_lava": {
       "classes": {
         "magician": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shield_of_song": {
       "classes": {
         "bard": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shield_of_spikes": {
       "classes": {
         "druid": 39,
         "ranger": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shield_of_the_magi": {
       "classes": {
-        "enchanter": "54",
+        "enchanter": 54,
         "magician": 54,
         "necromancer": 54,
         "wizard": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "shield_of_thistles": {
       "classes": {
         "druid": 9,
         "ranger": 30
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shield_of_words": {
       "classes": {
         "cleric": 49,
         "paladin": 60
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shielding": {
       "classes": {
-        "enchanter": "16",
+        "enchanter": 16,
         "magician": 16,
         "necromancer": 16,
         "wizard": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "shieldskin": {
       "classes": {
         "necromancer": 16,
         "shadow knight": 34,
         "wizard": 16
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "shifting_shield": {
       "classes": {
         "shaman": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shifting_sight": {
       "classes": {
-        "enchanter": "20",
+        "enchanter": 20,
         "wizard": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shiftless_deeds": {
       "classes": {
-        "enchanter": "44"
+        "enchanter": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "shroud_of_death": {
       "classes": {
         "shadow knight": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "shroud_of_hate": {
       "classes": {
         "shadow knight": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shroud_of_pain": {
       "classes": {
         "shadow knight": 50
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shroud_of_the_spirits": {
       "classes": {
         "shaman": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "shroud_of_undeath": {
       "classes": {
         "shadow knight": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "sicken": {
       "classes": {
         "shaman": 5
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "sight": {
       "classes": {
         "wizard": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "sight_graft": {
       "classes": {
         "necromancer": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "silver_skin": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "siphon_strength": {
       "classes": {
         "necromancer": 1,
         "shadow knight": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "siphon_strength_recourse": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": true
     },
     "skin_like_diamond": {
       "classes": {
         "druid": 39,
         "ranger": 54
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "skin_like_nature": {
       "classes": {
         "druid": 49,
         "ranger": 59
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "skin_like_rock": {
       "classes": {
         "druid": 14,
         "ranger": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "skin_like_steel": {
       "classes": {
         "druid": 24,
         "ranger": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "skin_like_wood": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "skin_of_the_shadow": {
       "classes": {
         "necromancer": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "skunkspray": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "slime_mist": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "snare": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "solons_bewitching_bravura": {
       "classes": {
         "bard": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "solons_charismatic_concord": {
       "classes": {
         "bard": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "solons_song_of_the_sirens": {
       "classes": {
         "bard": 27
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "song_of_midnight": {
       "classes": {
         "bard": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "song_of_the_deep_seas": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "song_of_twilight": {
       "classes": {
         "bard": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "soothe": {
       "classes": {
         "cleric": 9,
-        "enchanter": "8",
+        "enchanter": 8,
         "paladin": 30
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "soul_bond": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "soul_consumption": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "soul_well": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "speed_of_the_shissar": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "spikecoat": {
       "classes": {
         "druid": 39,
         "ranger": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "spin_the_bottle": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "spirit_armor": {
       "classes": {
         "cleric": 19,
         "necromancer": 16,
         "paladin": 30
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "spirit_of_bear": {
       "classes": {
         "shaman": 9
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spirit_of_cat": {
       "classes": {
         "shaman": 19
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "spirit_of_cheetah": {
       "classes": {
         "druid": 24,
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "spirit_of_monkey": {
       "classes": {
         "shaman": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spirit_of_oak": {
       "classes": {
         "druid": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "spirit_of_ox": {
       "classes": {
         "shaman": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "spirit_of_scale": {
       "classes": {
         "druid": 53,
         "shaman": 52
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spirit_of_snake": {
       "classes": {
         "shaman": 14
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spirit_of_wolf": {
       "classes": {
         "druid": 14,
         "ranger": 30,
         "shaman": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "spirit_quickening": {
       "classes": {
         "shaman": 50
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spirit_sight": {
       "classes": {
         "shaman": 9
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spirit_strength": {
       "classes": {
         "shaman": 19
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "splurt": {
       "classes": {
         "necromancer": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "spook_the_dead": {
       "classes": {
         "cleric": 1,
         "necromancer": 12,
         "paladin": 9,
         "shadow knight": 22
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "stability": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "stalking_probe": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "stalwart_regeneration": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "stamina": {
       "classes": {
         "shaman": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "steal_strength": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "steam_overload": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "steelskin": {
       "classes": {
         "necromancer": 34,
         "shadow knight": 56,
         "wizard": 34
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "stinging_swarm": {
       "classes": {
         "druid": 14,
         "ranger": 30
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "storm_strength": {
       "classes": {
         "druid": 44,
         "ranger": 53
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "stream_of_acid": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "strength": {
       "classes": {
         "shaman": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "strength_of_earth": {
       "classes": {
         "druid": 9,
         "ranger": 30
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "strength_of_nature": {
       "classes": {
         "ranger": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "strength_of_stone": {
       "classes": {
         "druid": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "strength_of_the_kunzar": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "strengthen": {
       "classes": {
-        "enchanter": "1",
+        "enchanter": 1,
         "shaman": 1
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "strengthen_death": {
       "classes": {
         "shadow knight": 29
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "strike_of_thunder": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "strong_disease": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "strong_poison": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "suffocate": {
       "classes": {
-        "enchanter": "29"
+        "enchanter": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "suffocating_sphere": {
       "classes": {
-        "enchanter": "4"
+        "enchanter": 4
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "sunbeam": {
       "classes": {
         "druid": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "sunskin": {
       "classes": {
         "cleric": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "surge_of_enfeeblement": {
       "classes": {
         "necromancer": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "swarm_of_retribution": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "swarming_pain": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "swift_like_the_wind": {
       "classes": {
-        "enchanter": "49"
+        "enchanter": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "swift_spirit": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": true
     },
     "sympathetic_aura": {
       "classes": {
-        "enchanter": "20"
+        "enchanter": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tagars_insects": {
       "classes": {
         "shaman": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "tainted_breath": {
       "classes": {
         "shaman": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "talisman_of_altuna": {
       "classes": {
         "shaman": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_jasinth": {
       "classes": {
         "shaman": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_kragg": {
       "classes": {
         "shaman": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_shadoo": {
       "classes": {
         "shaman": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_the_brute": {
       "classes": {
         "shaman": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_the_cat": {
       "classes": {
         "shaman": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_the_raptor": {
       "classes": {
         "shaman": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_the_rhino": {
       "classes": {
         "shaman": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_the_serpent": {
       "classes": {
         "shaman": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "talisman_of_tnarg": {
       "classes": {
         "shaman": 34
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tarews_aquatic_ayre": {
       "classes": {
         "bard": 16
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tashan": {
       "classes": {
-        "enchanter": "4"
+        "enchanter": 4
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "tashani": {
       "classes": {
-        "enchanter": "20"
+        "enchanter": 20
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "tashania": {
       "classes": {
-        "enchanter": "44"
+        "enchanter": 44
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "tashanian": {
       "classes": {
-        "enchanter": "255"
+        "enchanter": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "telescope": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "tepid_deeds": {
       "classes": {
-        "enchanter": "24"
+        "enchanter": 24
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "terrorize_animal": {
       "classes": {
         "druid": 19
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "the_unspoken_word": {
       "classes": {
         "cleric": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "thistlecoat": {
       "classes": {
         "druid": 9,
         "ranger": 15
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "thorncoat": {
       "classes": {
         "druid": 49,
         "ranger": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "thorny_shield": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "thrall_of_bones": {
       "classes": {
         "necromancer": 54
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "thunder_blast": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "tigirs_insects": {
       "classes": {
         "shaman": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "torment": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "torment_of_argli": {
       "classes": {
-        "enchanter": "56"
+        "enchanter": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "torment_of_shadows": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "torpor": {
       "classes": {
         "shaman": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "track_corpse": {
       "classes": {
         "necromancer": 20
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "travelerboots": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "treeform": {
       "classes": {
         "druid": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "trepidation": {
       "classes": {
         "cleric": 57,
-        "enchanter": "56",
+        "enchanter": 56,
         "necromancer": 56
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tumultuous_strength": {
       "classes": {
         "shaman": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tunares_request": {
       "classes": {
         "druid": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "turgurs_insects": {
       "classes": {
         "shaman": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "turning_of_the_unnatural": {
       "classes": {
-        "cleric": 255
+        "cleric": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tuyens_chant_of_flame": {
       "classes": {
         "bard": 38
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "tuyens_chant_of_frost": {
       "classes": {
         "bard": 46
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "ultravision": {
       "classes": {
-        "enchanter": "29",
+        "enchanter": 29,
         "shaman": 29
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "umbra": {
       "classes": {
-        "enchanter": "57"
+        "enchanter": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "unfailing_reverence": {
       "classes": {
         "shaman": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "valiant_companion": {
       "classes": {
         "magician": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "valor": {
       "classes": {
         "cleric": 34,
         "paladin": 49
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "vampire_charm": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "velocity": {
       "classes": {
         "magician": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "vengeance_of_the_glades": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "venom_of_the_snake": {
       "classes": {
         "necromancer": 34,
         "shaman": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "vexing_mordinia": {
       "classes": {
         "necromancer": 57
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "vigor": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": true
     },
     "vision": {
       "classes": {
         "shaman": 19
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "visions_of_grandeur": {
       "classes": {
-        "enchanter": "60"
+        "enchanter": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "voice_graft": {
       "classes": {
         "necromancer": 16
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "voice_of_the_berserker": {
       "classes": {
         "shaman": 59
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": true
     },
     "wake_of_tranquility": {
       "classes": {
         "cleric": 55,
-        "enchanter": "51"
+        "enchanter": 51
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "walking_sleep": {
       "classes": {
         "shaman": 14
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "wandering_mind": {
       "classes": {
-        "enchanter": "39"
+        "enchanter": 39
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wave_of_enfeeblement": {
       "classes": {
         "necromancer": 12,
         "shadow knight": 30
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wave_of_fear": {
       "classes": {
         "cleric": 24
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wave_of_heat": {
       "classes": {},
+      "item": false,
       "npc": true,
-      "item": false
+      "self": false
     },
     "waves_of_the_deep_sea": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "weak_poison": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "weaken": {
       "classes": {
-        "enchanter": "1"
+        "enchanter": 1
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "weakness": {
       "classes": {
-        "enchanter": "44"
+        "enchanter": 44
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "whirl_till_you_hurl": {
       "classes": {
-        "enchanter": "12"
+        "enchanter": 12
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "whirlwind": {
       "classes": {},
+      "item": true,
       "npc": true,
-      "item": true
+      "self": false
     },
     "wind_of_tishani": {
       "classes": {
-        "enchanter": "55"
+        "enchanter": 55
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wind_of_tishanian": {
       "classes": {
-        "enchanter": "60"
+        "enchanter": 60
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "winged_death": {
       "classes": {
         "druid": 53
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wolf_form": {
       "classes": {
         "druid": 24,
         "ranger": 49
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wonderous_rapidity": {
       "classes": {
-        "enchanter": "58"
+        "enchanter": 58
       },
+      "item": false,
       "npc": false,
-      "item": false
+      "self": false
     },
     "wrath_of_nature": {
       "classes": {},
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     },
     "yaulp": {
       "classes": {
         "cleric": 1,
         "paladin": 9
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "yaulp_ii": {
       "classes": {
         "cleric": 19,
         "paladin": 39
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "yaulp_iii": {
       "classes": {
         "cleric": 44,
         "paladin": 56
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": true
     },
     "yaulp_iv": {
       "classes": {
         "cleric": 53,
         "paladin": 60
       },
+      "item": true,
       "npc": false,
-      "item": true
+      "self": false
     }
   },
   "version": "%s"
 }
 """
 
     try:
@@ -5196,14 +5911,4708 @@
             "update spell casters: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
+def update_spell_items(data_path, version):
+    """Update data/spell-items.json"""
+
+    new_spell_items_data = """
+{
+  "spells": {
+    "accuracy": {
+      "potion_of_accuracy": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "adroitness": {
+      "potion_of_adroitness": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aegis_of_bathezid": {
+      "regal_band_of_bathezid": {
+        "cast": 0,
+        "classes": {
+          "bard": 49,
+          "cleric": 49,
+          "druid": 49,
+          "enchanter": 49,
+          "magician": 49,
+          "monk": 49,
+          "necromancer": 49,
+          "paladin": 49,
+          "ranger": 49,
+          "rogue": 49,
+          "shadow knight": 49,
+          "shaman": 49,
+          "warrior": 49,
+          "wizard": 49
+        }
+      }
+    },
+    "alacrity": {
+      "bracelet_of_the_spirits": {
+        "cast": 0,
+        "classes": {
+          "shaman": 45
+        }
+      },
+      "elder_shamans_ceremonial_bracelet": {
+        "cast": 0,
+        "classes": {
+          "shaman": 45
+        }
+      },
+      "sandals_of_alacrity": {
+        "cast": 0,
+        "classes": {
+          "monk": 45
+        }
+      }
+    },
+    "allure_of_death": {
+      "wand_of_darkness": {
+        "cast": 0,
+        "classes": {
+          "  necromancer": 20
+        }
+      }
+    },
+    "alluring_whispers": {
+      "shissar_focus_staff": {
+        "cast": 16,
+        "classes": {
+          "  enchanter": 50
+        }
+      }
+    },
+    "aloe_sweat": {
+      "disciple_symbol_of_tunare": {
+        "cast": 4,
+        "classes": {
+          "cleric": 15,
+          "druid": 15
+        }
+      }
+    },
+    "arch_shielding": {
+      "tri-plated_golden_hackle_hammer": {
+        "cast": 0.1,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "armor_of_faith": {
+      "donals_gauntlets_of_mourning": {
+        "cast": 10,
+        "classes": {
+          "cleric": 45
+        }
+      }
+    },
+    "augment_death": {
+      "pantaloons_of_the_bonecaster": {
+        "cast": 15,
+        "classes": {
+          "necromancer": 50
+        }
+      },
+      "plague_bearers_trousers": {
+        "cast": 15,
+        "classes": {
+          "necromancer": 50
+        }
+      },
+      "rotting_trousers": {
+        "cast": 15,
+        "classes": {
+          "necromancer": 50
+        }
+      },
+      "warlocks_pantaloons": {
+        "cast": 15,
+        "classes": {
+          "necromancer": 50
+        }
+      }
+    },
+    "aura_of_antibody": {
+      "10_dose_greater_potion_of_antibody": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_battle": {
+      "fearsome_shield": {
+        "cast": 0,
+        "classes": {
+          "cleric": 0,
+          "paladin": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      },
+      "pauldrons_of_ferocity": {
+        "cast": 0,
+        "classes": {
+          "paladin": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "aura_of_black_petals": {
+      "black_flower_of_functionality": {
+        "cast": 2,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_blue_petals": {
+      "blue_flower_of_functionality": {
+        "cast": 2,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_cold": {
+      "10_dose_greater_potion_of_cold": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_green_petals": {
+      "green_flower_of_functionality": {
+        "cast": 2,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_heat": {
+      "10_dose_greater_potion_of_heat": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_marr": {
+      "frothy_goblin_tonic": {
+        "cast": 0,
+        "classes": {
+          "bard": 25,
+          "cleric": 25,
+          "druid": 25,
+          "enchanter": 25,
+          "magician": 25,
+          "monk": 25,
+          "necromancer": 25,
+          "paladin": 25,
+          "ranger": 25,
+          "rogue": 25,
+          "shadow knight": 25,
+          "shaman": 25,
+          "warrior": 25,
+          "wizard": 25
+        }
+      }
+    },
+    "aura_of_purity": {
+      "10_dose_greater_potion_of_purity": {
+        "cast": 4,
+        "classes": {
+          "bard": 25,
+          "cleric": 25,
+          "druid": 25,
+          "enchanter": 25,
+          "magician": 25,
+          "monk": 25,
+          "necromancer": 25,
+          "paladin": 25,
+          "ranger": 25,
+          "rogue": 25,
+          "shadow knight": 25,
+          "shaman": 25,
+          "warrior": 25,
+          "wizard": 25
+        }
+      }
+    },
+    "aura_of_red_petals": {
+      "red_flower_of_functionality": {
+        "cast": 2,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "aura_of_white_petals": {
+      "white_flower_of_functionality": {
+        "cast": 2,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "avatar": {
+      "primal_weapon": {
+        "  cast": 0,
+        "  classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "barrier_of_force": {
+      "staff_of_the_four": {
+        "cast": 15,
+        "classes": {
+          "wizard": 50
+        }
+      }
+    },
+    "battery_vision": {
+      "clockwork_watchman_helm": {
+        "cast": 6,
+        "classes": {
+          "cleric": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "befriend_animal": {
+      "pouch_of_mistletoe_powder": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "beguile_plants": {
+      "dark_oak_shillelagh": {
+        "cast": 0,
+        "classes": {
+          "druid": 29
+        }
+      }
+    },
+    "berserker_madness_i": {
+      "maddening_sap": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "berserker_madness_ii": {
+      "zek_frost": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "berserker_madness_iii": {
+      "essence_of_rallos": {
+        "cast": 0,
+        "classes": {
+          "bard": 40,
+          "cleric": 40,
+          "druid": 40,
+          "enchanter": 40,
+          "magician": 40,
+          "monk": 40,
+          "necromancer": 40,
+          "paladin": 40,
+          "ranger": 40,
+          "rogue": 40,
+          "shadow knight": 40,
+          "shaman": 40,
+          "warrior": 40,
+          "wizard": 40
+        }
+      }
+    },
+    "berserker_madness_iv": {
+      "warlords_rage": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "berserker_strength": {
+      "braided_beard_of_the_coldain": {
+        "cast": 0,
+        "classes": {
+          "bard": 40,
+          "cleric": 40,
+          "druid": 40,
+          "enchanter": 40,
+          "magician": 40,
+          "monk": 40,
+          "necromancer": 40,
+          "paladin": 40,
+          "ranger": 40,
+          "rogue": 40,
+          "shadow knight": 40,
+          "shaman": 40,
+          "warrior": 40,
+          "wizard": 40
+        }
+      },
+      "polished_granite_tomahawk": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "warrior": 10
+        }
+      },
+      "shadow_rager": {
+        "cast": 0,
+        "classes": {
+          "rogue": 0
+        }
+      }
+    },
+    "blessing_of_nature": {
+      "razor_fang_of_xygoz": {
+        "  cast": 0,
+        "classes": {
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "blinding_luminance": {
+      "bioluminescent_orb": {
+        "cast": 5,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "blinding_poison_i": {
+      "retinal_deactivator": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "blinding_poison_ii": {
+      "eyeburn_solution": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "blinding_poison_iii": {
+      "shadowveil_hemlock": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      },
+      "wrapped_entropy_serpent_spine": {
+        "cast": 0,
+        "classes": {
+          "bard": 1,
+          "paladin": 1,
+          "ranger": 1,
+          "rogue": 1,
+          "shadow knight": 1,
+          "warrior": 1
+        }
+      }
+    },
+    "blinding_step": {
+      "murkey_vial": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "blood_claw": {
+      "stiletto_of_the_bloodclaw": {
+        "cast": 0,
+        "classes": {
+          "necromancer": 18,
+          "rogue": 18,
+          "shadow knight": 18
+        }
+      }
+    },
+    "bobbing_corpse": {
+      "shaidin_revenant_bauble": {
+        "cast": 1.5,
+        "classes": {
+          "necromancer": 49,
+          "shadow knight": 49
+        }
+      }
+    },
+    "boil_blood": {
+      "blood_fire": {
+        "cast": 0,
+        "classes": {
+          "warrior": 46
+        }
+      }
+    },
+    "boiling_blood": {
+      "narandis_lance": {
+        "cast": 0,
+        "classes": {
+          "paladin": 55,
+          "shadow knight": 55,
+          "warrior": 55
+        }
+      }
+    },
+    "bonds_of_force": {
+      "alkabors_cap_of_binding": {
+        "cast": 0,
+        "classes": {
+          "wizard": 49
+        }
+      }
+    },
+    "bone_melt": {
+      "paebala_warbone": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "monk": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "bramblecoat": {
+      "jaundiced_bone_breastplate": {
+        "cast": 12,
+        "classes": {
+          "shaman": 45
+        }
+      }
+    },
+    "breath_of_the_dead": {
+      "aqualung": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "breath_of_the_sea": {
+      "wavecrasher": {
+        "cast": 0,
+        "classes": {
+          "bard": 1,
+          "paladin": 1,
+          "ranger": 1,
+          "rogue": 1,
+          "shadow knight": 1,
+          "warrior": 1
+        }
+      }
+    },
+    "brittle_haste_i": {
+      "delusional_swiftness": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "brittle_haste_ii": {
+      "xegonys_curse": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "brittle_haste_iii": {
+      "paradoxical_peptide": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "brittle_haste_iv": {
+      "rending_swiftness": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "burnout_iii": {
+      "arch_mages_pantaloons": {
+        "cast": 15,
+        "classes": {
+          "magician": 46
+        }
+      },
+      "mask_of_empowerment": {
+        "cast": 0,
+        "classes": {
+          "magician": 45
+        }
+      },
+      "robe_of_burning_rage": {
+        "cast": 8,
+        "classes": {
+          "magician": 50
+        }
+      }
+    },
+    "burrowing_scarab": {
+      "death_scarab_gland": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "calimony": {
+      "10_dose_potion_of_stinging_wort": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "call_of_earth": {
+      "golden_leaf_breastplate": {
+        "cast": 10,
+        "classes": {
+          "ranger": 50
+        }
+      }
+    },
+    "calm": {
+      "regent_symbol_of_quellious": {
+        "cast": 4,
+        "classes": {
+          "cleric": 20
+        }
+      }
+    },
+    "captain_nalots_quickening": {
+      "eyepatch_of_plunder": {
+        "cast": 3.5,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "cascading_darkness": {
+      "wand_of_darkness": {
+        "cast": 0,
+        "classes": {
+          "necromancer": 45
+        }
+      }
+    },
+    "celestial_tranquility": {
+      "celestial_fists": {
+        "cast": 0,
+        "classes": {
+          "monk": 50
+        }
+      }
+    },
+    "chant_of_battle": {
+      "harmonic_spear": {
+        "cast": 0,
+        "classes": {
+          "bard": 45
+        }
+      }
+    },
+    "chill_sight": {
+      "bangle_of_the_invoker": {
+        "cast": 3,
+        "classes": {
+          "wizard": 50
+        }
+      },
+      "darksight_dagger": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 44,
+          "magician": 44,
+          "necromancer": 44,
+          "wizard": 44
+        }
+      },
+      "eye_of_innoruuk": {
+        "cast": 0,
+        "classes": {
+          "wizard": 0
+        }
+      }
+    },
+    "chloroplast": {
+      "elder_spiritists_breastplate": {
+        "cast": 12,
+        "classes": {
+          "druid": 45
+        }
+      },
+      "skull_engraved_coin": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "choke": {
+      "packmasters_lash": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "warrior": 20
+        }
+      },
+      "whip_of_strangulation": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "warrior": 10
+        }
+      }
+    },
+    "clarity": {
+      "beguilers_trousers": {
+        "cast": 15,
+        "classes": {
+          "enchanter": 50
+        }
+      },
+      "clarifying_spores": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "coin_depicting_innoruuk": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "rod_of_infinite_thought": {
+        "cast": 7,
+        "classes": {
+          "enchanter": 46
+        }
+      },
+      "rod_of_unbound_thought": {
+        "cast": 0,
+        "classes": {
+          "wizard": 46
+        }
+      }
+    },
+    "clinging_darkness": {
+      "reagent_symbol_of_innoruuk": {
+        "cast": 6,
+        "classes": {
+          "cleric": 15,
+          "shaman": 15
+        }
+      },
+      "sceptre_of_the_forlorn": {
+        "cast": 0,
+        "classes": {
+          "necromancer": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "clockwork_poison": {
+      "trochilic_skean": {
+        "cast": 0,
+        "classes": {
+          "bard": 46,
+          "ranger": 46,
+          "rogue": 46,
+          "warrior": 46
+        }
+      }
+    },
+    "cloud": {
+      "runed_sea_shell": {
+        "cast": 6,
+        "classes": {
+          "bard": 12,
+          "cleric": 12,
+          "druid": 12,
+          "enchanter": 12,
+          "magician": 12,
+          "monk": 12,
+          "necromancer": 12,
+          "paladin": 12,
+          "ranger": 12,
+          "rogue": 12,
+          "shadow knight": 12,
+          "shaman": 12,
+          "warrior": 12,
+          "wizard": 12
+        }
+      }
+    },
+    "cog_boost": {
+      "clockwork_watchman_vambraces": {
+        "cast": 5,
+        "classes": {
+          "cleric": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "cohesion": {
+      "greater_potion_of_cohesion": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "creeping_vision": {
+      "eye_of _narandi": {
+        "cast": 1,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "curse_of_the_spirits": {
+      "spear_of_fate": {
+        "cast": 9,
+        "classes": {
+          "shaman": 50
+        }
+      }
+    },
+    "dance_of_the_blade": {
+      "singing_short_sword": {
+        "cast": 0,
+        "classes": {
+          "bard": 46
+        }
+      }
+    },
+    "daring": {
+      "deepwater_helm": {
+        "cast": 10,
+        "classes": {
+          "paladin": 45
+        }
+      }
+    },
+    "dawncall": {
+      "dawncaller_blade_of_the_morning": {
+        "cast": 0,
+        "classes": {
+          "paladin": 50
+        }
+      },
+      "great_spear_of_dawn": {
+        "cast": 0,
+        "classes": {
+          "paladin": 50,
+          "shadow knight": 50
+        }
+      }
+    },
+    "dead_man_floating": {
+      "robe_of_adversity": {
+        "cast": 12,
+        "classes": {
+          "necromancer": 50
+        }
+      }
+    },
+    "deadeye": {
+      "blood_ember_helm": {
+        "cast": 6,
+        "classes": {
+          "shadow knight": 45
+        }
+      },
+      "fright_forged_helm": {
+        "cast": 0,
+        "classes": {
+          "cleric": 10
+        }
+      }
+    },
+    "deadly_poison": {
+      "ancient_venom_sack": {
+        "cast": 0,
+        "classes": {
+          "rogue": 30
+        }
+      }
+    },
+    "deftness": {
+      "jaundiced_bone_gauntlets": {
+        "cast": 10,
+        "classes": {
+          "shaman": 45
+        }
+      }
+    },
+    "desperate_hope": {
+      "serpent_blood_potion": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "diamondskin": {
+      "diamond_rod": {
+        "cast": 6,
+        "classes": {
+          "wizard": 46
+        }
+      }
+    },
+    "disease": {
+      "a_vile_substance": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "disease_cloud": {
+      "gobline_plaguebeads": {
+        "cast": 0,
+        "classes": {
+          "necromancer": 5,
+          "shadow knight": 5
+        }
+      },
+      "initiate_ymbol_of_bertoxxulous": {
+        "cast": 4,
+        "classes": {
+          "cleric": 0
+        }
+      },
+      "bloody_dirk": {
+        "cast": 0,
+        "classes": {
+          "rogue": 15
+        }
+      },
+      "rotwood_club": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 18
+        }
+      },
+      "very_rusty_dagger": {
+        "cast": 0,
+        "classes": {
+          "rogue": 0,
+          "shadow knight": 0
+        }
+      }
+    },
+    "disempower": {
+      "stalagterror_spine_spear": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 0
+        }
+      }
+    },
+    "divine_aura": {
+      "shiny_brass_idol": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "earring_of_the_frozen_skull": {
+        "cast": 1,
+        "classes": {
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "shaman": 0,
+          "wizard": 0
+        }
+      },
+      "protection_of_the_dain": {
+        "cast": 2.5,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "dizzy_i": {
+      "sweet_lathyris": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "dizzy_ii": {
+      "languid_lixt_wing": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "dizzy_iii": {
+      "crippling_peptide": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "dizzy_iv": {
+      "twisting_disorientation": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "dooming_darkness": {
+      "nightfall": {
+        "cast": 0,
+        "classes": {
+          "rogue": 50
+        }
+      }
+    },
+    "draconic_rage": {
+      "potion_of_draconic_rage": {
+        "cast": 3,
+        "classes": {
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "warrior": 30
+        }
+      }
+    },
+    "drones_of_doom": {
+      "elder_spiritists_vambraces": {
+        "cast": 8,
+        "classes": {
+          "druid": 45
+        }
+      },
+      "nature_walkers_bracer": {
+        "cast": 7.5,
+        "classes": {
+          "druid": 50
+        }
+      },
+      "staff_of_the_earthcaller": {
+        "cast": 0,
+        "classes": {
+          "druid": 40
+        }
+      }
+    },
+    "drowsy": {
+      "canyoneer_pike": {
+        "cast": 0,
+        "classes": {
+          "rogue": 5,
+          "warrior": 5
+        }
+      }
+    },
+    "dulsehound": {
+      "potion_of_dulsehound": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "earthcall": {
+      "earthcaller": {
+        "cast": 0,
+        "classes": {
+          "ranger": 50
+        }
+      }
+    },
+    "echinacea_infusion": {
+      "initiate_symbol_of_tunare": {
+        "cast": 4,
+        "classes": {
+          "cleric": 5,
+          "druid": 5
+        }
+      }
+    },
+    "elemental_armor": {
+      "icicle_pantaloons": {
+        "cast": 15,
+        "classes": {
+          "wizard": 50
+        }
+      },
+      "diamond_encrusted_staff": {
+        "cast": 20,
+        "classes": {
+          "wizard": 50
+        }
+      },
+      "sages_pantaloons": {
+        "cast": 0,
+        "classes": {
+          "wizard": 50
+        }
+      }
+    },
+    "endure_magic": {
+      "deepwater_boots": {
+        "cast": 5,
+        "classes": {
+          "paladin": 45
+        }
+      }
+    },
+    "enduring_breath": {
+      "moss_mask": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "energy_sap": {
+      "willsapper": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "engulfing_darkness": {
+      "serrated_bone_dirk": {
+        "cast": 0,
+        "classes": {
+          "rogue": 27
+        }
+      },
+      "blood_ember_gauntlets": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 45
+        }
+      },
+      "obtenebrate_claymore": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 35,
+          "warrior": 35
+        }
+      }
+    },
+    "ensnare": {
+      "tanglewood_shield": {
+        "cast": 4,
+        "classes": {
+          "druid": 35,
+          "ranger": 35
+        }
+      },
+      "sap_encrusted_branch": {
+        "cast": 0,
+        "classes": {
+          "cleric": 49,
+          "druid": 49,
+          "monk": 49,
+          "ranger": 49,
+          "shaman": 49
+        }
+      },
+      "spear_of_constriction": {
+        "cast": 0,
+        "classes": {
+          "ranger": 50,
+          "shaman": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "envenomed_breath": {
+      "sword_of_the_shissar": {
+        "cast": 0,
+        "classes": {
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      },
+      "wand_of_the_black_dragon_eye": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 50,
+          "magician": 50,
+          "necromancer": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "everlasting_breath": {
+      "10_dose_potion_of_aquatic_haunt": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "enchanted_velium_mask": {
+        "cast": 2,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "extended_regeneration": {
+      "blood_of_the_dhampyre": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "eye_of_zomm": {
+      "holgresh_elder_beads": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "singing_steel_helm": {
+        "cast": 8,
+        "classes": {
+          "bard": 45
+        }
+      },
+      "clay_bracelet": {
+        "cast": 0,
+        "classes": {
+          "magician": 20
+        }
+      }
+    },
+    "feast_of_blood": {
+      "mrylokars_dagger_of_vengeance": {
+        "cast": 0,
+        "classes": {
+          "rogue": 0
+        }
+      }
+    },
+    "feet_like_cat": {
+      "cat_o_nine_tails": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "fellspine": {
+      "fellspines_tail": {
+        "cast": 0,
+        "classes": {
+          "paladin": 55,
+          "ranger": 55,
+          "shadow knight": 55
+        }
+      }
+    },
+    "fiery_might": {
+      "chestplate_of_fiery_might": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "firefist": {
+      "golden_star_slippers": {
+        "cast": 7,
+        "classes": {
+          "monk": 50
+        }
+      },
+      "berserkers_ring": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "monk": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "fleeting_fury": {
+      "iksar_berserker_club": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "monk": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10
+        }
+      }
+    },
+    "flesh_rot_i": {
+      "solvent_gangrene": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "flesh_rot_ii": {
+      "fester": {
+        "cast": 0,
+        "classes": {
+          "rogue": 49
+        }
+      }
+    },
+    "flesh_rot_iii": {
+      "visceral_rot": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "flurry": {
+      "10_dose_adrenaline_tap": {
+        "cast": 8,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "form_of_the_great_wolf": {
+      "lycanthropic_staff": {
+        "cast": 16,
+        "classes": {
+          "druid": 50
+        }
+      }
+    },
+    "fortitude": {
+      "invigorating_spores": {
+        "cast": 10,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "froglok_poison": {
+      "malevolent_runeblade": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "rogue": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "frostbite": {
+      "frostbringer": {
+        "cast": 0,
+        "classes": {
+          "paladin": 0,
+          "ranger": 40,
+          "shadow knight": 40,
+          "warrior": 40
+        }
+      },
+      "efreeti_ice_staff": {
+        "cast": 0,
+        "classes": {
+          "monk": 50
+        }
+      }
+    },
+    "frostreavers_blessing": {
+      "cast": 0,
+      "classes": {
+        "bard": 0,
+        "cleric": 0,
+        "druid": 0,
+        "enchanter": 0,
+        "magician": 0,
+        "monk": 0,
+        "necromancer": 0,
+        "paladin": 0,
+        "ranger": 0,
+        "rogue": 0,
+        "shadow knight": 0,
+        "shaman": 0,
+        "warrior": 0,
+        "wizard": 0
+      }
+    },
+    "fungal_regrowth": {
+      "fungus_covered_great_staff": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "fungus_spores": {
+      "fungus_spores": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "furious_strength": {
+      "jaundiced_bone_vambraces": {
+        "cast": 10,
+        "classes": {
+          "shaman": 45
+        }
+      }
+    },
+    "fury": {
+      "songweavers_mantle": {
+        "cast": 0,
+        "classes": {
+          "bard": 45
+        }
+      }
+    },
+    "garzicors_vengeance": {
+      "ethereal_bladed_naginata": {
+        "cast": 0,
+        "classes": {
+          "paladin": 50,
+          "ranger": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "gasping_embrace": {
+      "robe_of_smothering": {
+        "cast": 8,
+        "classes": {
+          "enchanter": 50
+        }
+      }
+    },
+    "gaze": {
+      "acumen_mask": {
+        "cast": 0,
+        "classes": {
+          "wizard": 20
+        }
+      }
+    },
+    "glamour": {
+      "jaundiced_bone_helm": {
+        "cast": 10,
+        "classes": {
+          "shaman": 45
+        }
+      },
+      "luminary_two_handed_sword": {
+        "cast": 0,
+        "classes": {
+          "paladin": 26,
+          "ranger": 26,
+          "shadow knight": 26,
+          "warrior": 26
+        }
+      }
+    },
+    "glimpse": {
+      "preserved_split_paw_eye": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "graveyard_dust": {
+      "potion_of_graveyard_dust": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "grease_injection": {
+      "clockwork_watchman_greaves": {
+        "cast": 4,
+        "classes": {
+          "cleric": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "greater_wolf_form": {
+      "lupine_dagger": {
+        "cast": 0,
+        "classes": {
+          "ranger": 45
+        }
+      }
+    },
+    "greenmist": {
+      "greenmist": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 45
+        }
+      }
+    },
+    "grim_aura": {
+      "shrunken_goblin_skull_earring": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "guard": {
+      "bone_amulet_of_blade_turning": {
+        "cast": 4,
+        "classes": {
+          "cleric": 20,
+          "druid": 20,
+          "shaman": 20
+        }
+      },
+      "star_of_the_guardian": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "paladin": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "harmshield": {
+      "duennan_shielding_ring": {
+        "cast": 0,
+        "classes": {
+          "magician": 0
+        }
+      }
+    },
+    "haste": {
+      "ashenwood_short_spear": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "health": {
+      "jaundiced_bone_greaves": {
+        "cast": 10,
+        "classes": {
+          "shaman": 45
+        }
+      }
+    },
+    "heat_blood": {
+      "ivory_handled_falcion": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 0
+        }
+      }
+    },
+    "hug": {
+      "twisted_druid_doll": {
+        "cast": 1,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "ignite_bones": {
+      "bone_bracelet_of_condemnation": {
+        "cast": 15,
+        "classes": {
+          "necromancer": 40
+        }
+      }
+    },
+    "ikatiars_revenge": {
+      "ikatiars_stinger": {
+        "cast": 0,
+        "classes": {
+          "rogue": 50,
+          "shadow knight": 50
+        }
+      }
+    },
+    "incapacitate": {
+      "cracked_claw_of_zlandicar": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "infectious_cloud": {
+      "rotted_staff": {
+        "cast": 0,
+        "classes": {
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "necromancer": 50,
+          "shaman": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "inferno_shield": {
+      "lava_potion": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "insidious_fever": {
+      "sarnak_flesh_harvester": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "insight": {
+      "potion_of_wisdom": {
+        "cast": 0,
+        "classes": {
+          "bard": 15,
+          "cleric": 15,
+          "druid": 15,
+          "enchanter": 15,
+          "magician": 15,
+          "monk": 15,
+          "necromancer": 15,
+          "paladin": 15,
+          "ranger": 15,
+          "rogue": 15,
+          "shadow knight": 15,
+          "shaman": 15,
+          "warrior": 15,
+          "wizard": 15
+        }
+      }
+    },
+    "insipid_weakness": {
+      "withered_staff": {
+        "cast": 10,
+        "classes": {
+          "enchanter": 46
+        }
+      }
+    },
+    "kilvas_skin_of_flame": {
+      "kilvas_skin_of_flame": {
+        "cast": 10,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "kylies_venom": {
+      "dragonspine_rapier": {
+        "cast": 0,
+        "classes": {
+          "rogue": 46
+        }
+      }
+    },
+    "leach": {
+      "soulfiend_lance": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 25
+        }
+      }
+    },
+    "lesser_shielding": {
+      "cobalt_vambraces": {
+        "cast": 9,
+        "classes": {
+          "warrior": 45
+        }
+      }
+    },
+    "levitate": {
+      "pegasus_feather_cloak": {
+        "cast": 6,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "potion_of_antiweight": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "levitation": {
+      "summoned_ring_of_levitation": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "ravener_tail_whip": {
+        "cast": 6,
+        "classes": {
+          "bard": 25,
+          "rogue": 25,
+          "warrior": 25
+        }
+      }
+    },
+    "lower_resists_i": {
+      "festering_nettle": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "lower_resists_ii": {
+      "cast": 0,
+      "classes": {
+        "bard": 20,
+        "cleric": 20,
+        "druid": 20,
+        "enchanter": 20,
+        "magician": 20,
+        "monk": 20,
+        "necromancer": 20,
+        "paladin": 20,
+        "ranger": 20,
+        "rogue": 20,
+        "shadow knight": 20,
+        "shaman": 20,
+        "warrior": 20,
+        "wizard": 20
+      }
+    },
+    "lower_resists_iii": {
+      "cyclic_vertigo": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "lower_resists_iv": {
+      "susceptible_essence": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "lull": {
+      "initiate_symbol_of_quellious": {
+        "cast": 4,
+        "classes": {
+          "cleric": 0
+        }
+      }
+    },
+    "major_shielding": {
+      "blood_ember_breastplate": {
+        "cast": 10,
+        "classes": {
+          "shadow knight": 45
+        }
+      },
+      "stave_of_shielding": {
+        "cast": 0,
+        "classes": {
+          "paladin": 50,
+          "shadow knight": 50,
+          "monk": 50
+        }
+      }
+    },
+    "malevolent_grasp": {
+      "malevolence": {
+        "cast": 0,
+        "classes": {
+          "cleric": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "mana_flare": {
+      "pitted_iron_ring": {
+        "cast": 5,
+        "classes": {
+          "enchanter": 50,
+          "magician": 50,
+          "necromancer": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "mark_of_karn": {
+      "templars_chestplate": {
+        "cast": 9,
+        "classes": {
+          "cleric": 46
+        }
+      }
+    },
+    "muscle_lock_i": {
+      "tserrinas_whip": {
+        "cast": 0,
+        "classes": {
+          "bard": 35,
+          "paladin": 35,
+          "ranger": 35,
+          "rogue": 35,
+          "shadow knight": 35,
+          "warrior": 35
+        }
+      }
+    },
+    "muscle_lock_ii": {
+      "lethargic_bliss": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "muscle_lock_iii": {
+      "pacifying_whisper": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "muscle_lock_iv": {
+      "spirit_of_sloth": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "mystic_precision": {
+      "clockwork_watchman_boots": {
+        "cast": 4,
+        "classes": {
+          "cleric": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "natures_melody": {
+      "natures_melody": {
+        "cast": 0,
+        "classes": {
+          "bard": 0
+        }
+      }
+    },
+    "nimble": {
+      "jaundiced_bone_boots": {
+        "cast": 10,
+        "classes": {
+          "shaman": 45
+        }
+      }
+    },
+    "nivs_melody_of_preservation": {
+      "breath_of_harmony": {
+        "cast": 0,
+        "classes": {
+          "bard": 50
+        }
+      }
+    },
+    "null_aura": {
+      "10_dose_greater_null_potion": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "obsidian_shatter": {
+      "obsidian_shard": {
+        "cast": 0,
+        "classes": {
+          "bard": 16,
+          "enchanter": 16,
+          "magician": 16,
+          "necromancer": 16,
+          "ranger": 16,
+          "rogue": 16,
+          "shadow knight": 16,
+          "shaman": 16,
+          "warrior": 16,
+          "wizard": 16
+        }
+      }
+    },
+    "okeils_radiation": {
+      "boots_of_the_invoker": {
+        "cast": 3,
+        "classes": {
+          "wizard": 50
+        }
+      }
+    },
+    "one_hundred_blows": {
+      "tranquil_staff": {
+        "cast": 0,
+        "classes": {
+          "monk": 50
+        }
+      }
+    },
+    "pacify": {
+      "donals_bracer_of_mourning": {
+        "cast": 7,
+        "classes": {
+          "cleric": 45
+        }
+      }
+    },
+    "panic_animal": {
+      "disciple_symbol_of_cazic_thule": {
+        "cast": 2,
+        "classes": {
+          "cleric": 5,
+          "shaman": 5
+        }
+      }
+    },
+    "paralyzing_poison_i": {
+      "spine_break": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "paralyzing_poison_ii": {
+      "kinectic_suppresant": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "paralyzing_poison_iii": {
+      "stiffening_ergot": {
+        "cast": 0,
+        "classes": {
+          "bard": 30,
+          "cleric": 30,
+          "druid": 30,
+          "enchanter": 30,
+          "magician": 30,
+          "monk": 30,
+          "necromancer": 30,
+          "paladin": 30,
+          "ranger": 30,
+          "rogue": 30,
+          "shadow knight": 30,
+          "shaman": 30,
+          "warrior": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "phantom_plate": {
+      "shissar_guardian_staff": {
+        "cast": 10,
+        "classes": {
+          "magician": 50
+        }
+      }
+    },
+    "poison": {
+      "infestation": {
+        "cast": 0,
+        "classes": {
+          "bard": 1,
+          "ranger": 1,
+          "rogue": 1,
+          "warrior": 1
+        }
+      },
+      "pondfish_spine": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
+      }
+    },
+    "poison_bolt": {
+      "a_scorpion_telson": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "power": {
+      "10_dose_potion_of_power": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "primal_essence": {
+      "hammer_of_the_dragonborn": {
+        "cast": 8,
+        "classes": {
+          "shaman": 35
+        }
+      }
+    },
+    "rage_of_vallon": {
+      "blade_of_strategy": {
+        "cast": 0,
+        "classes": {
+          "warrior": 50
+        }
+      }
+    },
+    "rage_of_zek": {
+      "jagged_blade_of_war": {
+        "cast": 0,
+        "classes": {
+          "warrior": 50
+        }
+      }
+    },
+    "rampage": {
+      "axe_of_the_slayers": {
+        "cast": 0,
+        "classes": {
+          "warrior": 30
+        }
+      },
+      "thornstinger": {
+        "cast": 0,
+        "classes": {
+          "rogue": 45
+        }
+      },
+      "vehement_sword_of_reivaj": {
+        "cast": 0,
+        "classes": {
+          "paladin": 45,
+          "shadow knight": 45,
+          "warrior": 45
+        }
+      }
+    },
+    "reckless_health": {
+      "crimson_potion": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "reckless_strength": {
+      "cobalt_gauntlets": {
+        "cast": 10,
+        "classes": {
+          "warrior": 45
+        }
+      },
+      "glowing_club": {
+        "cast": 0,
+        "classes": {
+          "ranger": 1
+        }
+      }
+    },
+    "regeneration": {
+      "pliable_goo": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      },
+      "spiroc_healers_cloak": {
+        "cast": 0,
+        "classes": {
+          "ranger": 45
+        }
+      }
+    },
+    "regrowth_of_the_grove": {
+      "nature_walkers_chestguard": {
+        "cast": 9,
+        "classes": {
+          "druid": 45
+        }
+      }
+    },
+    "rejuvenation": {
+      "10_dose_potion_of_rejuvenation": {
+        "cast": 12,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "resist_cold": {
+      "frozen_turban": {
+        "cast": 25,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "resist_magic": {
+      "waters_of_impenetrable_aura": {
+        "cast": 13.5,
+        "classes": {
+          "cleric": 50
+        }
+      }
+    },
+    "resistance_to_magic": {
+      "vial_of_vampire_blood": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "cleric": 50,
+          "druid": 50,
+          "enchanter": 50,
+          "magician": 50,
+          "monk": 50,
+          "necromancer": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "shaman": 50,
+          "warrior": 50,
+          "wizard": 50
+        }
+      }
+    },
+    "riotous_health": {
+      "rune_crafters_breastplate": {
+        "cast": 9,
+        "classes": {
+          "shaman": 45
+        }
+      }
+    },
+    "rodricks_gift": {
+      "dirk_of_the_traitor": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "rune_iii": {
+      "rod_of_warding_winds": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 45
+        }
+      },
+      "runed_blade": {
+        "cast": 0,
+        "classes": {
+          "paladin": 46,
+          "ranger": 46,
+          "warrior": 46
+        }
+      }
+    },
+    "rune_iv": {
+      "beguilers_robe": {
+        "cast": 30,
+        "classes": {
+          "enchanter": 46
+        }
+      }
+    },
+    "scale_of_wolf": {
+      "crazy_cleric_boots": {
+        "cast": 0,
+        "classes": {
+          "cleric": 45
+        }
+      },
+      "earring_of_twisted_leaves": {
+        "cast": 4.5,
+        "classes": {
+          "druid": 49,
+          "shaman": 49
+        }
+      },
+      "maleficent_boots": {
+        "cast": 0,
+        "classes": {
+          "necromancer": 45
+        }
+      },
+      "mischievous_dazzler_shoes": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 45
+        }
+      },
+      "monkey_hide_boots": {
+        "cast": 0,
+        "classes": {
+          "monk": 45
+        }
+      },
+      "shamanistic_shenannigan_boots": {
+        "cast": 0,
+        "classes": {
+          "shaman": 45
+        }
+      },
+      "sly_summoners_boots": {
+        "cast": 0,
+        "classes": {
+          "magician": 45
+        }
+      },
+      "twisted_nature_boots": {
+        "cast": 0,
+        "classes": {
+          "druid": 45
+        }
+      }
+    },
+    "scent_of_darkness": {
+      "nightshade_scented_staff": {
+        "cast": 8,
+        "classes": {
+          "necromancer": 50
+        }
+      }
+    },
+    "scorching_skin": {
+      "10_dose_kilvas_blistering_flesh": {
+        "cast": 10,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "scourge": {
+      "blight_hammer_of_the_scourge": {
+        "cast": 0,
+        "classes": {
+          "shaman": 30
+        }
+      }
+    },
+    "screaming_mace": {
+      "screaming_mace": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "monk": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10
+        }
+      }
+    },
+    "sear": {
+      "burynaibane_spider_fang": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "sebilite_pox": {
+      "feverblade_bane_of_the_shissar": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "see_invisible": {
+      "bracer_of_the_hidden": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      }
+    },
+    "selos_song_of_travel": {
+      "breastplate_of_twilight": {
+        "cast": 5.5,
+        "classes": {
+          "bard": 46
+        }
+      }
+    },
+    "shadow": {
+      "crescent_blades_of_luclin": {
+        "cast": 0,
+        "classes": {
+          "bard": 40,
+          "ranger": 40,
+          "rogue": 40,
+          "shadow knight": 40,
+          "warrior": 40
+        }
+      }
+    },
+    "shadow_vortex": {
+      "cazic_quill": {
+        "cast": 0,
+        "classes": {
+          "rogue": 35
+        }
+      },
+      "twisted_oak_staff": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "shallow_breath": {
+      "water_crystal_staff": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "share_wolf_form": {
+      "elder_spiritists_bracer": {
+        "cast": 12,
+        "classes": {
+          "druid": 45
+        }
+      }
+    },
+    "shield_of_brambles": {
+      "yannikil": {
+        "cast": 0,
+        "classes": {
+          "ranger": 45
+        }
+      }
+    },
+    "shield_of_flame": {
+      "singing_steel_bracer": {
+        "cast": 5,
+        "classes": {
+          "bard": 45
+        }
+      },
+      "blazing_vambraces": {
+        "cast": 0,
+        "classes": {
+          "bard": 45,
+          "cleric": 45,
+          "paladin": 45,
+          "shadow knight": 45,
+          "warrior": 45
+        }
+      },
+      "charred_black_staff": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "shield_of_lava": {
+      "arch_mages_robe": {
+        "cast": 16,
+        "classes": {
+          "magician": 50
+        }
+      },
+      "summoners_robe": {
+        "cast": 14,
+        "classes": {
+          "magician": 50
+        }
+      },
+      "ros_breath": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "shield_of_thistles": {
+      "two_handed_practice_sword": {
+        "cast": 0,
+        "classes": {
+          "paladin": 22,
+          "ranger": 22,
+          "shadow knight": 22,
+          "warrior": 22
+        }
+      }
+    },
+    "shield_of_words": {
+      "runed_protectors_breastplate": {
+        "cast": 15,
+        "classes": {
+          "paladin": 45
+        }
+      },
+      "shissar_protection_staff": {
+        "cast": 7,
+        "classes": {
+          "cleric": 50
+        }
+      }
+    },
+    "shieldskin": {
+      "dragon_tooth_choker": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "monk": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "shifting_shield": {
+      "potion_of_spirit_shield": {
+        "cast": 12,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "shiftless_deeds": {
+      "slowstone_amber": {
+        "cast": 2.5,
+        "classes": {
+          "monk": 45
+        }
+      },
+      "writ_of_dizok": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 49
+        }
+      }
+    },
+    "sicken": {
+      "dark_spear_of_venom": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 45
+        }
+      },
+      "slime_crystal_staff": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "silver_skin": {
+      "silver_whip_of_rage": {
+        "cast": 0,
+        "classes": {
+          "  bard": 46,
+          "  paladin": 46,
+          "  ranger": 46,
+          "  rogue": 46,
+          "  shadow knight": 46,
+          "  warrior": 46
+        }
+      }
+    },
+    "siphon_strength": {
+      "discple_symbol_of_innoruuk": {
+        "  cast": 6,
+        "classes": {
+          "cleric": 5,
+          "shaman": 5
+        }
+      }
+    },
+    "skin_like_diamond": {
+      "elder_spiritists_greaves": {
+        "cast": 12,
+        "classes": {
+          "druid": 45
+        }
+      }
+    },
+    "skin_like_nature": {
+      "robe_of_the_spring": {
+        "cast": 12,
+        "classes": {
+          "druid": 50
+        }
+      }
+    },
+    "skin_like_rock": {
+      "mountain_death_belt": {
+        "cast": 6,
+        "classes": {
+          "cleric": 0,
+          "paladin": 0,
+          "rogue": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "snare": {
+      "ball_of_burlap_yarn": {
+        "cast": 5,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "earring_of_woven_bark": {
+        "cast": 4.5,
+        "classes": {
+          "druid": 49,
+          "ranger": 49
+        }
+      },
+      "elder_spiritists_gauntlets": {
+        "cast": 4,
+        "classes": {
+          "druid": 45
+        }
+      },
+      "tolans_darkwood_gauntlets": {
+        "cast": 4,
+        "classes": {
+          "ranger": 45
+        }
+      },
+      "silken_whip_of_ensnaring": {
+        "cast": 0,
+        "classes": {
+          "ranger": 50,
+          "warrior": 50
+        }
+      },
+      "glaive_of_marltek": {
+        "cast": 0,
+        "classes": {
+          "druid": 15,
+          "ranger": 15,
+          "rogue": 15,
+          "warrior": 15
+        }
+      },
+      "anklesmasher": {
+        "cast": 0,
+        "classes": {
+          "bard": 49,
+          "monk": 49,
+          "ranger": 49,
+          "rogue": 49,
+          "shadow knight": 49,
+          "warrior": 49
+        }
+      }
+    },
+    "song_of_the_deep_seas": {
+      "natures_melody": {
+        "cast": 0,
+        "classes": {
+          "bard": 46
+        }
+      },
+      "sirens_song_dagger_of_the_sea": {
+        "cast": 0,
+        "classes": {
+          "bard": 46
+        }
+      }
+    },
+    "soothe": {
+      "deepwater_vambraces": {
+        "cast": 7,
+        "classes": {
+          "paladin": 45
+        }
+      },
+      "disciple_symbol_of_quellious": {
+        "cast": 4,
+        "classes": {
+          "cleric": 0
+        }
+      }
+    },
+    "soul_bond": {
+      "zealots_incarnadine_sword": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "soul_consumption": {
+      "innoruuks_curse": {
+        "cast": 0,
+        "classes": {
+          "shadow knight": 50
+        }
+      }
+    },
+    "soul_well": {
+      "shissar_deathspeaker_staff": {
+        "cast": 13.5,
+        "classes": {
+          "necromancer": 50
+        }
+      }
+    },
+    "speed_of_the_shissar": {
+      "staff_of_the_serpent": {
+        "cast": 6,
+        "classes": {
+          "enchanter": 50
+        }
+      }
+    },
+    "spikecoat": {
+      "girdle_of_living_thorns": {
+        "cast": 0,
+        "classes": {
+          "bard": 51,
+          "cleric": 51,
+          "druid": 51,
+          "enchanter": 51,
+          "magician": 51,
+          "monk": 51,
+          "necromancer": 51,
+          "paladin": 51,
+          "ranger": 51,
+          "rogue": 51,
+          "shadow knight": 51,
+          "shaman": 51,
+          "warrior": 51,
+          "wizard": 51
+        }
+      }
+    },
+    "spin_the_bottle": {
+      "spinning_orb_of_confusion": {
+        "cast": 0,
+        "classes": {
+          "bard": 46,
+          "cleric": 46,
+          "druid": 46,
+          "enchanter": 46,
+          "magician": 46,
+          "monk": 46,
+          "necromancer": 46,
+          "paladin": 46,
+          "ranger": 46,
+          "rogue": 46,
+          "shadow knight": 46,
+          "shaman": 46,
+          "warrior": 46,
+          "wizard": 46
+        }
+      }
+    },
+    "spirit_armor": {
+      "shieldstorm": {
+        "cast": 0,
+        "classes": {
+          "paladin": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "spirit_of_cat": {
+      "kejaar_totem": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "spirit_of_cheetah": {
+      "aerated_pauldrons": {
+        "cast": 0,
+        "classes": {
+          "warrior": 45
+        }
+      }
+    },
+    "spirit_of_ox": {
+      "golden_star_pants": {
+        "cast": 20,
+        "classes": {
+          "monk": 50
+        }
+      }
+    },
+    "spirit_of_wolf": {
+      "black_fur_boots": {
+        "cast": 0,
+        "classes": {
+          "shaman": 10
+        }
+      },
+      "10_dose_blood_of_the_wolf": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      },
+      "blood_orchid_katana": {
+        "cast": 8,
+        "classes": {
+          "bard": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      },
+      "nature_walkers_boots": {
+        "cast": 5.5,
+        "classes": {
+          "druid": 50
+        }
+      },
+      "watchman_boots": {
+        "cast": 0,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "warrior": 10
+        }
+      }
+    },
+    "spirit_strength": {
+      "deepwater_greaves": {
+        "cast": 10,
+        "classes": {
+          "paladin": 45
+        }
+      }
+    },
+    "spook_the_dead": {
+      "initiate_symbol_of_tunare": {
+        "cast": 2,
+        "classes": {
+          "cleric": 0,
+          "shaman": 0
+        }
+      }
+    },
+    "stability": {
+      "potion_of_stability": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "stalking_probe": {
+      "stalking_probe": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "stalwart_regeneration": {
+      "bark_potion": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "steal_strength": {
+      "beetle_stinger": {
+        "cast": 0,
+        "classes": {
+          "shaman": 30,
+          "warrior": 30
+        }
+      },
+      "shaded_torch": {
+        "cast": 0,
+        "classes": {
+          "bard": 25,
+          "monk": 25,
+          "rogue": 25,
+          "ranger": 25,
+          "warrior": 25
+        }
+      }
+    },
+    "steam_overload": {
+      "clockwork_watchman_gauntlets": {
+        "cast": 5,
+        "classes": {
+          "cleric": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "steelskin": {
+      "sword_of_rile": {
+        "cast": 0,
+        "classes": {
+          "paladin": 40,
+          "ranger": 40,
+          "shadow knight": 40,
+          "warrior": 40
+        }
+      },
+      "mystic_cloak": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 30,
+          "magician": 30,
+          "necromancer": 30,
+          "wizard": 30
+        }
+      }
+    },
+    "stinging_swarm": {
+      "tolans_darkwood_vambraces": {
+        "cast": 4,
+        "classes": {
+          "ranger": 45
+        }
+      }
+    },
+    "storm_strength": {
+      "woven_frost_giant_beard": {
+        "cast": 0,
+        "classes": {
+          "bard": 35,
+          "cleric": 35,
+          "druid": 35,
+          "enchanter": 35,
+          "magician": 35,
+          "monk": 35,
+          "necromancer": 35,
+          "paladin": 35,
+          "ranger": 35,
+          "rogue": 35,
+          "shadow knight": 35,
+          "shaman": 35,
+          "warrior": 35,
+          "wizard": 35
+        }
+      }
+    },
+    "strength_of_earth": {
+      "mrylokars_vambraces": {
+        "cast": 10,
+        "classes": {
+          "rogue": 45
+        }
+      }
+    },
+    "strength_of_the_kunzar": {
+      "cobalt_boots": {
+        "cast": 10,
+        "classes": {
+          "warrior": 45
+        }
+      },
+      "kunzar_hex_amulet": {
+        "cast": 6,
+        "classes": {
+          "paladin": 0,
+          "ranger": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "strengthen": {
+      "initiate_symbol_of_brell_serilis": {
+        "cast": 4,
+        "classes": {
+          "cleric": 0
+        }
+      }
+    },
+    "strike_of_thunder": {
+      "thunder_runed_great_sword": {
+        "cast": 0,
+        "classes": {
+          "paladin": 45,
+          "shadow knight": 45,
+          "warrior": 45
+        }
+      }
+    },
+    "strong_disease": {
+      "chelaki_tail": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "paladin": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "strong_poison": {
+      "licsh_der_pavs": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "warrior": 20
+        }
+      }
+    },
+    "suffocate": {
+      "nevederias_horn": {
+        "cast": 0,
+        "classes": {
+          "ranger": 46,
+          "rogue": 46,
+          "warrior": 46
+        }
+      }
+    },
+    "sunbeam": {
+      "blazing_breastplate_of_fennin_ro": {
+        "cast": 4,
+        "classes": {
+          "bard": 45,
+          "cleric": 45,
+          "paladin": 45,
+          "shadow knight": 45,
+          "warrior": 45
+        }
+      }
+    },
+    "swarming_pain": {
+      "braid_of_golden_hair": {
+        "cast": 0,
+        "classes": {
+          "bard": 45,
+          "paladin": 45,
+          "ranger": 45,
+          "rogue": 45,
+          "shadow knight": 45,
+          "warrior": 45
+        }
+      }
+    },
+    "swift_like_the_wind": {
+      "wand_of_swiftness": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 45
+        }
+      }
+    },
+    "tagars_insects": {
+      "garduk": {
+        "cast": 0,
+        "classes": {
+          "shaman": 46
+        }
+      },
+      "swarmcaller": {
+        "casat": 0,
+        "classes": {
+          "ranger": 46
+        }
+      }
+    },
+    "tainted_breath": {
+      "poisoned_whip": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "warrior": 0
+        }
+      }
+    },
+    "tashan": {
+      "howling_werewolf_claws": {
+        "cast": 0,
+        "classes": {
+          "bard": 4,
+          "paladin": 4,
+          "ranger": 4,
+          "rogue": 4,
+          "shadow knight": 4,
+          "warrior": 4
+        }
+      }
+    },
+    "tashani": {
+      "journeymans_walking_stick": {
+        "cast": 0,
+        "classes": {
+          "bard": 35,
+          "cleric": 35,
+          "druid": 35,
+          "monk": 35,
+          "paladin": 35,
+          "ranger": 35,
+          "rogue": 35,
+          "shaman": 35,
+          "shadow knight": 35,
+          "warrior": 35
+        }
+      },
+      "falgiron_staff": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "tashania": {
+      "orb_of_tishan": {
+        "cast": 0,
+        "classes": {
+          "bard": 40,
+          "enchanter": 40,
+          "magician": 40,
+          "necromancer": 40,
+          "wizard": 40
+        }
+      },
+      "shissar_nullifier_staff": {
+        "cast": 2,
+        "classes": {
+          "enchanter": 50
+        }
+      }
+    },
+    "telescope": {
+      "telescopic_eyepatch": {
+        "cast": 1,
+        "classes": {
+          "bard": 10,
+          "cleric": 10,
+          "druid": 10,
+          "enchanter": 10,
+          "magician": 10,
+          "monk": 10,
+          "necromancer": 10,
+          "paladin": 10,
+          "ranger": 10,
+          "rogue": 10,
+          "shadow knight": 10,
+          "shaman": 10,
+          "warrior": 10,
+          "wizard": 10
+        }
+      },
+      "spyglass": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "tepid_deeds": {
+      "truncheon_of_doom": {
+        "cast": 0,
+        "classes": {
+          "warrior": 50
+        }
+      }
+    },
+    "thorny_shield": {
+      "cloak_of_thorns": {
+        "cast": 0,
+        "classes": {
+          "druid": 46,
+          "ranger": 46,
+          "warrior": 46
+        }
+      }
+    },
+    "torment": {
+      "black_blade_of_tormenting": {
+        "cast": 0,
+        "classes": {
+          "bard": 46,
+          "ranger": 46,
+          "rogue": 46,
+          "shadow knight": 46,
+          "warrior": 46
+        }
+      }
+    },
+    "torment_of_shadows": {
+      "scythe_of_the_shadowed_soul": {
+        "cast": 9,
+        "classes": {
+          "necromancer": 50
+        }
+      }
+    },
+    "travelerboots": {
+      "travelers_boots": {
+        "cast": 1.5,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "treeform": {
+      "maple_leaf_mask": {
+        "cast": 10,
+        "classes": {
+          "druid": 20,
+          "enchanter": 20
+        }
+      }
+    },
+    "ultravision": {
+      "mrylokars_helm": {
+        "cast": 10,
+        "classes": {
+          "rogue": 45
+        }
+      },
+      "rune_crafters_bracer": {
+        "cast": 8,
+        "classes": {
+          "shaman": 45
+        }
+      },
+      "crown_of_hatred": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "valor": {
+      "donals_vambraces_of_mourning": {
+        "cast": 12,
+        "classes": {
+          "cleric": 45
+        }
+      }
+    },
+    "vigor": {
+      "potion_of_vigor": {
+        "cast": 4,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "voice_graft": {
+      "sentient_two_handed_axe": {
+        "cast": 2,
+        "classes": {
+          "shadow knight": 20
+        }
+      },
+      "preserved_chokidai_vocal_cords": {
+        "cast": 4,
+        "classes": {
+          "bard": 49,
+          "druid": 49,
+          "enchanter": 49,
+          "magician": 49,
+          "necromancer": 49,
+          "shaman": 49,
+          "shadow knight": 49
+        }
+      }
+    },
+    "walking_sleep": {
+      "midnight_mallet": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "waves_of_the_deep_sea": {
+      "trident_of_the_deep_sea": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "rogue": 50,
+          "shadow knight": 50,
+          "warrior": 50
+        }
+      }
+    },
+    "weak_poison": {
+      "crookstinger": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "weaken": {
+      "initiate_symbol_of_innoruuk": {
+        "cast": 6,
+        "classes": {
+          "cleric": 0,
+          "shaman": 0
+        }
+      },
+      "dagger_of_dropping": {
+        "cast": 0,
+        "classes": {
+          "enchanter": 0,
+          "magician": 0,
+          "necromancer": 0,
+          "rogue": 0,
+          "wizard": 0
+        }
+      }
+    },
+    "whirlwind": {
+      "windstriker": {
+        "cast": 0,
+        "classes": {
+          "ranger": 50
+        }
+      }
+    },
+    "wrath_of_nature": {
+      "nature_walkers_scimitar": {
+        "cast": 9,
+        "classes": {
+          "druid": 50
+        }
+      }
+    },
+    "yaulp": {
+      "initiate_symbol_of_rallos_zek": {
+        "cast": 4,
+        "classes": {
+          "shaman": 0
+        }
+      },
+      "hammer_of_rage": {
+        "cast": 0,
+        "classes": {
+          "cleric": 40,
+          "paladin": 40,
+          "ranger": 40,
+          "shaman": 40,
+          "shadow knight": 40,
+          "warrior": 40
+        }
+      }
+    },
+    "yaulp_ii": {
+      "donals_helm_of_mourning": {
+        "cast": 1,
+        "classes": {
+          "cleric": 45
+        }
+      },
+      "mask_of_war": {
+        "cast": 2,
+        "classes": {
+          "bard": 35,
+          "cleric": 35,
+          "druid": 35,
+          "enchanter": 35,
+          "magician": 35,
+          "monk": 35,
+          "necromancer": 35,
+          "paladin": 35,
+          "ranger": 35,
+          "rogue": 35,
+          "shadow knight": 35,
+          "shaman": 35,
+          "warrior": 35,
+          "wizard": 35
+        }
+      }
+    },
+    "yaulp_iii": {
+      "warhammer_of_divine_grace": {
+        "cast": 0,
+        "classes": {
+          "cleric": 40
+        }
+      }
+    },
+    "yaulp_iv": {
+      "claw_of_phara_dar": {
+        "cast": 0,
+        "classes": {
+          "bard": 50,
+          "ranger": 50,
+          "rogue": 50,
+          "warrior": 50
+        }
+      }
+    }
+  },
+  "version": "%s"
+}
+"""
+
+    try:
+        spell_items_path = data_path + "spell-items.json"
+        generate = True
+
+        if os.path.isfile(spell_items_path):
+            json_data = open(spell_items_path, "r", encoding="utf-8")
+            spell_items = json.load(json_data)
+            json_data.close()
+
+            if spell_items["version"] == version:
+                generate = False
+
+        if generate:
+            print("    - generating spell-items.json")
+            f = open(spell_items_path, "w", encoding="utf-8")
+            f.write(new_spell_items_data % (version))
+            f.close()
+
+    except Exception as e:
+        eqa_settings.log(
+            "update spell items: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
 def update_spell_lines(data_path, version):
     """Update data/spell-lines.json"""
 
     new_spell_lines_data = """
 {
   "spell_lines": {
     "spell_line_potion_you_on": {
@@ -8223,15 +13632,15 @@
         configs.settings.config["settings"]["timers"]["spell"]["filter"].update(
             {
                 "yours_only": state.spell_timer_yours_only,
             }
         )
         configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "other": str(state.spell_timer_other),
+                "other": state.spell_timer_other,
             }
         )
         configs.settings.config["settings"]["timers"]["spell"].update(
             {
                 "self": state.spell_timer_self,
             }
         )
@@ -18096,15 +23505,15 @@
       "sound": false
     }
   },
   "version": "%s"
 }
 """
 
-    new_line_chat_recieved_npc_config = """
+    new_line_chat_received_npc_config = """
 {
   "line": {
     "say_npc": {
       "alert": {},
       "reaction": false,
       "sound": false
     },
@@ -18129,15 +23538,15 @@
       "sound": false
     }
   },
   "version": "%s"
 }
 """
 
-    new_line_chat_recieved_config = """
+    new_line_chat_received_config = """
 {
   "line": {
     "auction": {
       "alert": {},
       "reaction": false,
       "sound": false
     },
@@ -18202,17 +23611,19 @@
         "sunder": "raid",
         "tash": "raid"
       },
       "reaction": "alert",
       "sound": "look at guild"
     },
     "ooc": {
-      "alert": {},
-      "reaction": false,
-      "sound": false
+      "alert": {
+        "train": "solo_group_only"
+      },
+      "reaction": "alert",
+      "sound": "watch out"
     },
     "say": {
       "alert": {
         "help": true,
         "spot": "raid"
       },
       "reaction": "alert",
@@ -18220,17 +23631,19 @@
     },
     "say_unknown_tongue": {
       "alert": {},
       "reaction": false,
       "sound": false
     },
     "shout": {
-      "alert": {},
-      "reaction": false,
-      "sound": false
+      "alert": {
+        "train": "solo_group_only"
+      },
+      "reaction": "alert",
+      "sound": "watch out"
     },
     "shout_unknown_tongue": {
       "alert": {},
       "reaction": false,
       "sound": false
     },
     "tell": {
@@ -20551,25 +25964,25 @@
             generated = True
 
         ### Chat Received NPC
         generated_received_npc = write_config(
             base_path,
             "line-alerts/chat-received-npc",
             version,
-            new_line_chat_recieved_npc_config,
+            new_line_chat_received_npc_config,
         )
         if generated_received_npc:
             generated = True
 
         ### Chat Received
         generated_received = write_config(
             base_path,
             "line-alerts/chat-received",
             version,
-            new_line_chat_recieved_config,
+            new_line_chat_received_config,
         )
         if generated_received:
             generated = True
 
         ### Chat Sent
         generated_sent = write_config(
             base_path, "line-alerts/chat-sent", version, new_line_chat_sent_config
```

### Comparing `eqalert-3.5.2/eqa/lib/curses.py` & `eqalert-3.5.3/eqa/lib/curses.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
    GNU General Public License for more details.
    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 
 import curses
+import heapq
 import os
 import sys
 import time
 import math
 import random
 import re
 from datetime import datetime
@@ -42,14 +43,15 @@
     page = "events"
     last_page = "events"
     s_setting = "character"
     s_char = 0
     s_opt = "debug"
     s_line = 0
     encounter_report = None
+    timers = None
 
     try:
         while not exit_flag.is_set() and not cfg_reload.is_set():
             # Sleep between empty checks
             if display_q.qsize() < 1:
                 time.sleep(0.01)
 
@@ -86,39 +88,53 @@
                         configs,
                         s_setting,
                         s_char,
                         s_opt,
                         s_line,
                         encounter_report,
                         version,
+                        timers,
                     )
 
                 ## Display Draw
                 elif display_event.type == "draw":
                     if display_event.screen == "help":
                         if page == "help":
                             page = last_page
+                        elif page != "timers":
+                            last_page = page
+                            page = display_event.screen
                         else:
+                            page = display_event.screen
+                    elif display_event.screen == "timers":
+                        if page == "timers":
+                            page = last_page
+                        elif page != "help":
                             last_page = page
+                            timers = display_event.payload
+                            page = display_event.screen
+                        else:
+                            timers = display_event.payload
                             page = display_event.screen
                     elif display_event.screen == "redraw":
-                        if page == "help":
+                        if page == "help" or page == "timers":
                             draw_page(
                                 stdscr,
                                 page,
                                 events,
                                 debug_events,
                                 state,
                                 configs,
                                 s_setting,
                                 s_char,
                                 s_opt,
                                 s_line,
                                 encounter_report,
                                 version,
+                                timers,
                             )
                     else:
                         page = display_event.screen
 
                     draw_page(
                         stdscr,
                         page,
@@ -128,14 +144,15 @@
                         configs,
                         s_setting,
                         s_char,
                         s_opt,
                         s_line,
                         encounter_report,
                         version,
+                        timers,
                     )
 
                 ## Draw Update
                 elif display_event.type == "event":
                     if display_event.screen == "events":
                         events.append(display_event)
                         if page == "events":
@@ -148,14 +165,15 @@
                                 configs,
                                 s_setting,
                                 s_char,
                                 s_opt,
                                 s_line,
                                 encounter_report,
                                 version,
+                                timers,
                             )
                     elif display_event.screen == "debug":
                         debug_events.append(display_event)
                         draw_page(
                             stdscr,
                             page,
                             events,
@@ -164,14 +182,15 @@
                             configs,
                             s_setting,
                             s_char,
                             s_opt,
                             s_line,
                             encounter_report,
                             version,
+                            timers,
                         )
                     elif display_event.screen == "clear":
                         events = []
                         debug_events = []
                         draw_page(
                             stdscr,
                             page,
@@ -181,14 +200,15 @@
                             configs,
                             s_setting,
                             s_char,
                             s_opt,
                             s_line,
                             encounter_report,
                             version,
+                            timers,
                         )
                 display_q.task_done()
 
     except Exception as e:
         eqa_settings.log(
             "display: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -208,14 +228,15 @@
     configs,
     s_setting,
     s_char,
     s_opt,
     s_line,
     encounter_report,
     version,
+    timers,
 ):
     y, x = stdscr.getmaxyx()
     try:
         if x >= 80 and y >= 40:
             if page == "events":
                 draw_events_frame(
                     stdscr, state, events, debug_events, encounter_report, version
@@ -226,14 +247,17 @@
                 draw_settings(
                     stdscr, state, configs, s_setting, s_char, s_opt, s_line, version
                 )
             elif page == "parse":
                 draw_parse(stdscr, state, encounter_report, version)
             elif page == "help":
                 draw_help(stdscr)
+            elif page == "timers":
+                copy_timers = timers.copy()
+                draw_timers(stdscr, copy_timers)
         else:
             draw_toosmall(stdscr)
     except Exception as e:
         eqa_settings.log(
             "draw_page: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1248,15 +1272,15 @@
         stdscr.addstr(23, 18, str(state.debug), curses.color_pair(3))
 
         # mute state
         stdscr.addstr(24, 5, "Mute", curses.color_pair(2))
         stdscr.addstr(24, 16, ": ", curses.color_pair(1))
         stdscr.addstr(24, 18, str(state.mute), curses.color_pair(3))
 
-        # enounter parse state
+        # encounter parse state
         stdscr.addstr(25, 5, "Encounter", curses.color_pair(2))
         stdscr.addstr(25, 16, ": ", curses.color_pair(1))
         stdscr.addstr(25, 18, str(state.encounter_parse), curses.color_pair(3))
 
         # consider evaluation state
         stdscr.addstr(26, 5, "Consider", curses.color_pair(2))
         stdscr.addstr(26, 16, ": ", curses.color_pair(1))
@@ -1918,14 +1942,138 @@
             "draw settings options: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
+def draw_timers(stdscr, timers):
+    """Draw timers pop up"""
+
+    try:
+        y, x = stdscr.getmaxyx()
+
+        timer_scr = stdscr.derwin(
+            int(y / 2) + int(y / 4), int(x / 2) + int(x / 4), int(y / 8), int(x / 8)
+        )
+        timer_scr.clear()
+        timer_scr.box()
+
+        timer_y, timer_x = timer_scr.getmaxyx()
+        mid_timer_y = int(timer_y / 2)
+        mid_timer_x = int(timer_x / 2)
+
+        # Title
+        timer_scr.addstr(2, mid_timer_x - 7, "Active Timers", curses.color_pair(2))
+
+        # Ensure there are timers to show
+        if timers is not None:
+            if len(timers) > 0:
+                print_timer_y = 4
+                now = datetime.now()
+                ## Show timers
+                while len(timers) > 0:
+                    ### Break if there are more timers than room
+                    if print_timer_y > int(timer_y * 0.9):
+                        break
+                    ### Get timer
+                    timer = heapq.heappop(timers)
+                    ### Duration remaining
+                    time_remaining = timer.time - now
+                    time_remaining_days = time_remaining.days
+                    time_remaining_seconds = time_remaining.seconds
+                    timer_hours = (
+                        time_remaining_days * 24 + time_remaining_seconds // 3600
+                    )
+                    timer_minutes = (time_remaining_seconds % 3600) // 60
+                    timer_seconds = time_remaining_seconds % 60
+                    if timer_minutes < 1 and timer_hours == 0:
+                        color = 6
+                    elif timer_minutes < 2 and timer_hours == 0:
+                        color = 4
+                    elif timer_minutes < 5 and timer_hours == 0:
+                        color = 2
+                    else:
+                        color = 5
+                    timer_scr.addstr(
+                        print_timer_y, 5, f"{timer_hours:02}", curses.color_pair(color)
+                    )
+                    timer_scr.addstr(
+                        print_timer_y,
+                        5 + len(f"{timer_hours:02}"),
+                        ":",
+                        curses.color_pair(1),
+                    )
+                    timer_scr.addstr(
+                        print_timer_y,
+                        6 + len(f"{timer_hours:02}"),
+                        f"{timer_minutes:02}",
+                        curses.color_pair(color),
+                    )
+                    timer_scr.addstr(
+                        print_timer_y,
+                        8 + len(f"{timer_hours:02}"),
+                        ":",
+                        curses.color_pair(1),
+                    )
+                    timer_scr.addstr(
+                        print_timer_y,
+                        9 + len(f"{timer_hours:02}"),
+                        f"{timer_seconds:02}",
+                        curses.color_pair(color),
+                    )
+                    timestamp_len = 11 + len(f"{timer_hours:02}")
+                    ### Timer details
+                    if timer.type == "spell":
+                        timer_scr.addstr(
+                            print_timer_y,
+                            2 + timestamp_len,
+                            timer.caster,
+                            curses.color_pair(3),
+                        )
+                        timer_scr.addch(
+                            print_timer_y,
+                            2 + timestamp_len + len(timer.caster),
+                            curses.ACS_RARROW,
+                        )
+                        timer_scr.addstr(
+                            print_timer_y,
+                            4 + timestamp_len + len(timer.caster),
+                            timer.target,
+                            curses.color_pair(3),
+                        )
+                        timer_scr.addstr(
+                            print_timer_y,
+                            6 + timestamp_len + len(timer.caster) + len(timer.target),
+                            timer.spell.replace("_", " "),
+                            curses.color_pair(color),
+                        )
+                    else:
+                        message = timer.payload
+                        timer_scr.addstr(
+                            print_timer_y,
+                            2 + timestamp_len,
+                            message,
+                            curses.color_pair(3),
+                        )
+                    print_timer_y = print_timer_y + 2
+            else:
+                draw_mascot_message(timer_scr, "No active timers")
+        else:
+            draw_mascot_message(timer_scr, "No active timers")
+
+    except Exception as e:
+        eqa_settings.log(
+            "draw timers: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
 def draw_help(stdscr):
     """Draw help"""
 
     try:
         y, x = stdscr.getmaxyx()
 
         helpscr = stdscr.derwin(
```

### Comparing `eqalert-3.5.2/eqa/lib/encounter.py` & `eqalert-3.5.3/eqa/lib/encounter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1493,17 +1493,17 @@
                 not_this_encounter.append(event)
 
         encounter_stack = not_this_encounter
 
         ## Scrape This Encounter Events
         pet_and_target_same = False
         this_encounter_events = len(this_encounter)
-        target_melee_damage_recieved = {}
+        target_melee_damage_received = {}
         target_melee_damage_done = {}
-        target_spell_damage_recieved = {}
+        target_spell_damage_received = {}
         target_spell_damage_done = {}
         encounter_target_damage_total = {}
         encounter_target_damage_done_total = {}
         encounter_target_spell_total = {}
         encounter_target_spell_done_total = {}
         target_block = {}
         target_dodge = {}
@@ -1575,18 +1575,18 @@
                         else:
                             target_rune[target] += 1
                     else:
                         if target not in encounter_target_damage_total.keys():
                             encounter_target_damage_total[target] = int(result)
                         else:
                             encounter_target_damage_total[target] += int(result)
-                        if source not in target_melee_damage_recieved.keys():
-                            target_melee_damage_recieved[source] = int(result)
+                        if source not in target_melee_damage_received.keys():
+                            target_melee_damage_received[source] = int(result)
                         else:
-                            target_melee_damage_recieved[source] += int(result)
+                            target_melee_damage_received[source] += int(result)
                 elif source == encounter_target:
                     if result == "block":
                         if source not in source_block.keys():
                             source_block[source] = 1
                         else:
                             source_block[source] += 1
                     elif result == "dodge":
@@ -1635,18 +1635,18 @@
                         encounter_casts[source] = 1
                     else:
                         encounter_casts[source] += 1
                 else:
                     if source == "Unknown" and target != encounter_target:
                         source = encounter_target
                     if target == encounter_target:
-                        if source not in target_spell_damage_recieved.keys():
-                            target_spell_damage_recieved[source] = int(result)
-                        elif source in target_spell_damage_recieved.keys():
-                            target_spell_damage_recieved[source] += int(result)
+                        if source not in target_spell_damage_received.keys():
+                            target_spell_damage_received[source] = int(result)
+                        elif source in target_spell_damage_received.keys():
+                            target_spell_damage_received[source] += int(result)
                         if target not in encounter_target_spell_total.keys():
                             encounter_target_spell_total[target] = int(result)
                         elif target in encounter_target_spell_total.keys():
                             encounter_target_spell_total[target] += int(result)
                     elif source == encounter_target:
                         if target not in target_spell_damage_done.keys():
                             target_spell_damage_done[target] = int(result)
@@ -1831,24 +1831,24 @@
                 encounter_report["participants"][l_part] = {}
                 activity = (
                     int(sorted_encounter_activity[participant])
                     / int(this_encounter_events)
                 ) * 100
                 encounter_report["participants"][l_part]["activity"] = str(activity)
                 total_damage = 0
-                if participant in target_melee_damage_recieved.keys():
+                if participant in target_melee_damage_received.keys():
                     encounter_report["participants"][l_part]["melee_damage_done"] = str(
-                        target_melee_damage_recieved[participant]
+                        target_melee_damage_received[participant]
                     )
-                    total_damage += int(target_melee_damage_recieved[participant])
-                if participant in target_spell_damage_recieved.keys():
+                    total_damage += int(target_melee_damage_received[participant])
+                if participant in target_spell_damage_received.keys():
                     encounter_report["participants"][l_part]["spell_damage_done"] = str(
-                        target_spell_damage_recieved[participant]
+                        target_spell_damage_received[participant]
                     )
-                    total_damage += int(target_spell_damage_recieved[participant])
+                    total_damage += int(target_spell_damage_received[participant])
                 if total_damage > 0 and int(encounter_duration) > 0:
                     encounter_report["participants"][l_part]["melee_dps_done"] = str(
                         total_damage / int(encounter_duration)
                     )
                 total_damage = 0
                 if participant in target_melee_damage_done.keys():
                     encounter_report["participants"][l_part][
```

### Comparing `eqalert-3.5.2/eqa/lib/keys.py` & `eqalert-3.5.3/eqa/lib/keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 def process(
     state,
     configs,
     display_q,
     keyboard_q,
     system_q,
+    timer_q,
     cfg_reload,
     exit_flag,
 ):
     """
     Process: keyboard_q
     Produce: display_q, system_q
     """
@@ -103,14 +104,16 @@
                     page = "settings"
                 elif key == ord("h"):
                     display_q.put(
                         eqa_struct.display(
                             eqa_settings.eqa_time(), "draw", "help", None
                         )
                     )
+                elif key == ord("t"):
+                    timer_q.put(eqa_struct.timer(None, "draw_timers", None, None))
                 elif key == ord("0"):
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "reload_config",
                             None,
@@ -162,15 +165,15 @@
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "mute",
                                 "toggle",
                                 "all",
                             )
                         )
-                    elif key == ord("t"):
+                    elif key == ord("y"):
                         if not state.auto_mob_timer:
                             system_q.put(
                                 eqa_struct.message(
                                     eqa_settings.eqa_time(),
                                     "system",
                                     "timer",
                                     "mob",
```

### Comparing `eqalert-3.5.2/eqa/lib/log.py` & `eqalert-3.5.3/eqa/lib/log.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/lib/parser.py` & `eqalert-3.5.3/eqa/lib/parser.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/lib/settings.py` & `eqalert-3.5.3/eqa/lib/settings.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/lib/sound.py` & `eqalert-3.5.3/eqa/lib/sound.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/lib/state.py` & `eqalert-3.5.3/eqa/lib/state.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/lib/struct.py` & `eqalert-3.5.3/eqa/lib/struct.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/lib/timer.py` & `eqalert-3.5.3/eqa/lib/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,21 @@
                             # If the zone duration is more than a minute, give up something is wrong
                             if adjustment <= 45:
                                 timers = self_spell_timer_drift(
                                     state, timers, adjustment
                                 )
                 elif timer_event.type == "zoning":
                     zoning_start_time = timer_event.time
+                elif timer_event.type == "draw_timers":
+                    draw_timers = timers.copy()
+                    display_q.put(
+                        eqa_struct.display(
+                            eqa_settings.eqa_time(), "draw", "timers", draw_timers
+                        )
+                    )
                 elif timer_event.type == "clear":
                     timers = []
 
                 timer_q.task_done()
 
             # Check timers
             if len(timers) > 0:
```

### Comparing `eqalert-3.5.2/eqa/lib/watch.py` & `eqalert-3.5.3/eqa/lib/watch.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/sound/tick.wav` & `eqalert-3.5.3/eqa/sound/tick.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqa/sound/tock.wav` & `eqalert-3.5.3/eqa/sound/tock.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/eqalert.egg-info/PKG-INFO` & `eqalert-3.5.3/eqalert.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.2
+Version: 3.5.3
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
@@ -38,27 +38,29 @@
 $ cd eqalert
 $ docker compose build
 $ docker compose run eqalert
 ```
 
 > Note: If running through docker after installing and running on your host, update or regenerate `~/.eqa/config/settings.json` to reflect local container paths in `/home/eqalert`
 
+
 ## Getting Started
 
 Start things up
 ```sh
 $ eqalert
 ```
 
 You should now see `~/.eqa/` with the following structure
 ```
 $HOME/.eqa
         ⎿ config/
           ⎿ line-alerts/
         ⎿ data/
+          ⎿ timers/
         ⎿ encounters/
         ⎿ log/
           ⎿ debug/
         ⎿ sound/
 ```
 
 Spot check these default paths generated in `config/settings.json`
@@ -72,14 +74,15 @@
       "everquest_files": "[$HOME]/.wine/drive_c/Program Files/Sony/EverQuest/",
       "sound": "[$HOME/.eqa/]sound/",
       "tmp_sound": "/tmp/eqa/sound/"
     },
 ```
 > Press `0` to reload your configs or restart the program if any changes were made.  Though generally, it's a good idea to stop eqalert before manually editing your config files.
 
+
 ## Data
 
 ### Spell Timers
 
 EQ Alert will generate a file for spell timers in `data/spell-timers.json` by default by parsing `spells_us.txt` in your EverQuest directory.
 
 This file will only regenerate if it is missing, malformed, or a newer `spells_us.txt` file is present.
@@ -88,40 +91,54 @@
 
 EQ Alert will generate/overwrite `data/spell-casters.json` each version.  This file contains which classes can cast a given buff which timers should be made for.
 
 ### Spell Lines
 
 Many spells cast in EverQuest share the same log output lines.  EQ Alert will generate/overwrite `data/spell-lines.json` each version as a mapping of which possible spells a given output line could be associated to.
 
+### Spell Items
+
+EQ Alert will generate/overwrite `data/spell-items.json` each version as a mapping of which items a given spell could be cast by.
+
 ### Players
 
 EQ Alert uses in-game `/who` output to keep an up-to-date list of each seen players class, level, and guild organized by server in `data/players.json` for alerting spell duration.
 
+### Saved Timers
+
+If the active character is changed or EQ Alert is stopped, all active timers are saved to a file in `data/timers/` by the previously active character and server name.  This file is consumed when the parser sets that character as active again, adding all non-expired timers back to the timer list.
+
+
+## Encounters
+
+When encounter parse saving is enabled, complete encounter reports are saved under `encounters/[zone_name]/[date]/` as the time stamp of the encounter and the encounter target.
+
 
 ## Controls
 
 ### Keyboard Controls
 
 #### Global
   - 0       : Reload config
   - 1       : Events
   - 2       : State
   - 3       : Parse
   - 4       : Settings
   - q / esc : Quit
-  - h       : Help
+  - h       : Help pop-up
+  - t       : Timers pop-up
 
 #### Events
   - c       : Clear event box
   - d       : Toggle debug mode
   - e       : Toggle encounter parsing
   - m       : Toggle global audio mute
   - p       : Toggle encounter parse save
   - r       : Toggle raid mode
-  - t       : Toggle automatic mob respawn timers
+  - y       : Toggle automatic mob respawn timers
 
 #### Settings
   - up      : Up in selection
   - down    : Down in selection
   - right   : Selection options
   - left    : Selection options
   - space   : Select
```

### Comparing `eqalert-3.5.2/eqalert.egg-info/SOURCES.txt` & `eqalert-3.5.3/eqalert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.2/setup.py` & `eqalert-3.5.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 
-# read the contents of your README file
+# read the contents of README.md
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="eqalert",
-    version="3.5.2",
+    version="3.5.3",
     author="M Geitz",
     author_email="git@geitz.xyz",
     install_requires=[
         "playsound>=1.3.0",
         "gtts>=2.3.1",
     ],
     python_requires=">=3.9.2",
```

