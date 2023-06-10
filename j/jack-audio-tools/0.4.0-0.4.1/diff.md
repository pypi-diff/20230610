# Comparing `tmp/jack-audio-tools-0.4.0.tar.gz` & `tmp/jack-audio-tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jack-audio-tools-0.4.0.tar", last modified: Fri Feb  5 14:42:42 2021, max compression
+gzip compressed data, was "jack-audio-tools-0.4.1.tar", last modified: Sat Jun 10 14:35:51 2023, max compression
```

## Comparing `jack-audio-tools-0.4.0.tar` & `jack-audio-tools-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-02-05 14:42:42.417728 jack-audio-tools-0.4.0/
--rw-r--r--   0 chris     (1000) users      (100)     1079 2021-02-05 14:39:47.000000 jack-audio-tools-0.4.0/LICENSE
--rw-r--r--   0 chris     (1000) users      (100)       16 2019-11-26 17:06:49.000000 jack-audio-tools-0.4.0/MANIFEST.in
--rw-r--r--   0 chris     (1000) users      (100)     7906 2021-02-05 14:42:42.416728 jack-audio-tools-0.4.0/PKG-INFO
--rw-r--r--   0 chris     (1000) users      (100)     5419 2021-02-05 14:29:24.000000 jack-audio-tools-0.4.0/README.md
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-02-05 14:42:42.412728 jack-audio-tools-0.4.0/carla/
--rwxr-xr-x   0 chris     (1000) users      (100)     6294 2019-11-16 17:21:06.000000 jack-audio-tools-0.4.0/carla/carxp2lv2presets.py
--rw-r--r--   0 chris     (1000) users      (100)     4272 2019-11-14 01:17:32.000000 jack-audio-tools-0.4.0/carla/loadcarxp.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-02-05 14:42:42.413728 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/
--rw-r--r--   0 chris     (1000) users      (100)     7906 2021-02-05 14:42:42.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) users      (100)      583 2021-02-05 14:42:42.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) users      (100)        1 2021-02-05 14:42:42.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) users      (100)      665 2021-02-05 14:42:42.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) users      (100)        1 2019-10-13 19:16:52.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/not-zip-safe
--rw-r--r--   0 chris     (1000) users      (100)       90 2021-02-05 14:42:42.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) users      (100)       15 2021-02-05 14:42:42.000000 jack-audio-tools-0.4.0/jack_audio_tools.egg-info/top_level.txt
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-02-05 14:42:42.413728 jack-audio-tools-0.4.0/jackdbus/
--rwxr-xr-x   0 chris     (1000) users      (100)    10317 2021-02-05 14:38:03.000000 jack-audio-tools-0.4.0/jackdbus/jackmonitor.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-02-05 14:42:42.414728 jack-audio-tools-0.4.0/lv2/
--rwxr-xr-x   0 chris     (1000) users      (100)     2045 2020-08-15 11:07:53.000000 jack-audio-tools-0.4.0/lv2/grep.py
--rwxr-xr-x   0 chris     (1000) users      (100)     1451 2019-11-16 18:26:43.000000 jack-audio-tools-0.4.0/lv2/list_plugin_presets.py
--rw-r--r--   0 chris     (1000) users      (100)    22883 2019-11-26 18:54:09.000000 jack-audio-tools-0.4.0/lv2/plugin_info.py
--rw-r--r--   0 chris     (1000) users      (100)      839 2019-11-14 01:08:29.000000 jack-audio-tools-0.4.0/lv2/plugin_uris.py
--rw-r--r--   0 chris     (1000) users      (100)       38 2021-02-05 14:42:42.417728 jack-audio-tools-0.4.0/setup.cfg
--rwxr-xr-x   0 chris     (1000) users      (100)     2759 2021-02-05 14:33:46.000000 jack-audio-tools-0.4.0/setup.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-02-05 14:42:42.415728 jack-audio-tools-0.4.0/transport/
--rwxr-xr-x   0 chris     (1000) users      (100)     3529 2019-10-13 19:26:59.000000 jack-audio-tools-0.4.0/transport/midi_to_transport.py
--rwxr-xr-x   0 chris     (1000) users      (100)     3570 2019-10-13 19:26:59.000000 jack-audio-tools-0.4.0/transport/rtmidi_to_transport.py
--rwxr-xr-x   0 chris     (1000) users      (100)     5039 2019-10-13 19:26:59.000000 jack-audio-tools-0.4.0/transport/timebase_master.py
--rwxr-xr-x   0 chris     (1000) users      (100)     1992 2019-10-13 19:26:59.000000 jack-audio-tools-0.4.0/transport/transporter.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-10 14:35:51.592664 jack-audio-tools-0.4.1/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1203 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/.gitignore
+-rw-r--r--   0 chris     (1000) chris     (1000)     1079 2023-06-10 14:34:55.000000 jack-audio-tools-0.4.1/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)       16 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/MANIFEST.in
+-rw-r--r--   0 chris     (1000) chris     (1000)     6349 2023-06-10 14:35:51.592664 jack-audio-tools-0.4.1/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     5419 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-10 14:35:51.589663 jack-audio-tools-0.4.1/carla/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     6276 2023-06-10 14:17:13.000000 jack-audio-tools-0.4.1/carla/carxp2lv2presets.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4272 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/carla/loadcarxp.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-10 14:35:51.590664 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6349 2023-06-10 14:35:51.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      609 2023-06-10 14:35:51.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-06-10 14:35:51.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      664 2023-06-10 14:35:51.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-06-10 13:53:32.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/not-zip-safe
+-rw-r--r--   0 chris     (1000) chris     (1000)       90 2023-06-10 14:35:51.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       15 2023-06-10 14:35:51.000000 jack-audio-tools-0.4.1/jack_audio_tools.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-10 14:35:51.590664 jack-audio-tools-0.4.1/jackdbus/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)    10317 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/jackdbus/jackmonitor.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-10 14:35:51.591664 jack-audio-tools-0.4.1/lv2/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2045 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/lv2/grep.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1451 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/lv2/list_plugin_presets.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    22883 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/lv2/plugin_info.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      839 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/lv2/plugin_uris.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      104 2023-06-10 14:34:55.000000 jack-audio-tools-0.4.1/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-06-10 14:35:51.592664 jack-audio-tools-0.4.1/setup.cfg
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2799 2023-06-10 14:34:55.000000 jack-audio-tools-0.4.1/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-10 14:35:51.591664 jack-audio-tools-0.4.1/transport/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     3529 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/transport/midi_to_transport.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     3570 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/transport/rtmidi_to_transport.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     5039 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/transport/timebase_master.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1992 2023-06-10 13:46:04.000000 jack-audio-tools-0.4.1/transport/transporter.py
```

### Comparing `jack-audio-tools-0.4.0/LICENSE` & `jack-audio-tools-0.4.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2021 Christopher Arndt
+Copyright (c) 2019-2023 Christopher Arndt
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jack-audio-tools-0.4.0/PKG-INFO` & `jack-audio-tools-0.4.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,225 +1,226 @@
 Metadata-Version: 2.1
 Name: jack-audio-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: A collection of utilities and tools for the JACK audio ecosystem
 Home-page: https://github.com/SpotlightKid/jack-audio-tools
 Author: Christopher Arndt
 Author-email: info@chrisarndt.de
 License: MIT License
-Description: # jack-audio-tools
-        
-        A collection of utilities and tools for the [JACK] audio ecosystem
-        
-        
-        ## JACK Transport
-        
-        The scripts in the `jackaudiotools.transport` package query or manipulate the
-        JACK transport state.
-        
-        They require the [JACK-Client] package to be installed, which will be installed
-        automatically, when you install the `jack-audio-tools` distribution via `pip`:
-        
-            pip install jack-audio-tools
-        
-        
-        ### `jack-midi-to-transport`
-        
-        JACK client which allows to control transport state via MIDI.
-        
-        The client provides a MIDI input and converts received MIDI system real-time
-        and MIDI machine control (MMC) messages into JACK transport commands.
-        
-        The following MIDI messages, when received, start the JACK transport:
-        
-        * `START` (System Real-time)
-        * `CONTINUE` (System Real-time)
-        * `PLAY` (MMC)
-        * `DEFERRED PLAY` (MMC)
-        
-        These messages stop the transport:
-        
-        * `STOP` (System Real-time)
-        * `STOP` (MMC)
-        * `PAUSE` (MMC)
-        * `RESET` (MMC)
-        
-        And these rewind the transport to frame zero:
-        
-        * `REWIND` (MMC)
-        * `RESET` (MMC)
-        
-        MMC messages are ignored, if the device number in the MMC System Exclusive
-        message does not match the client's device number (set with the -d command
-        line option).
-        
-        If the client's device number is set to 127 (the default), it matches all
-        MMC message device numbers.
-        
-        
-        ### `jack-rtmidi-to-transport`
-        
-        JACK client which allows to control transport state via MIDI.
-        
-        A variant of `midi_to_transport`, which uses the [python-rtmidi] package
-        as a MIDI backend instead of JACK-Client, which is slightly more efficient,
-        because MIDI input processing is happening in a C++ thread instead of a
-        Python callback.
-        
-        To use it, specify the `rtmidi` extra dependency when installing the
-        `jack-audio-tools` distribution via `pip`:
-        
-            pip install "jack-audio-tools[rtmidi]"
-        
-        
-        ### `jack-timebase-master`
-        
-        A simple JACK timebase master, which provides  musical timing related
-        information (i.e. currents bar, beats per bar, beat denominator, BPM etc.)
-        to other JACK clients.
-        
-        
-        ### `jack-transporter`
-        
-        Query or change the JACK transport state.
-        
-        
-        ## JACK D-BUS
-        
-        The scripts in the `jackaudiotools.jackdbus` package interface with the JACK
-        D-BUS service to query information about the status of the JACK server and/or
-        control its operation.
-        
-        These scripts require the [PyGobject]  and [dbus-python] packages to be
-        installed. To install these, specify the `dbus` extra dependency when
-        installing the `jack-audio-tools` distribution via `pip`:
-        
-            pip install "jack-audio-tools[dbus]"
-        
-        
-        ### `jack-dbus-monitor`
-        
-        This script monitors the JACK server via D-BUS and runs a command on status
-        changes and optionally at a given interval passing some JACK stats in the
-        environment.
-        
-        Here is an example shell script to use as a command:
-        
-        ```bash
-        #!/bin/bash
-        
-        event="$1"  # 'start', 'stop' or 'status'
-        echo "JACK event: $event"
-        
-        if [[ "$event" = "status" ]]; then
-            echo "IS_STARTED: $IS_STARTED"
-            echo "IS_REALTIME: $IS_REALTIME"
-            echo "PERIOD: $PERIOD"
-            echo "LATENCY: $LATENCY"
-            echo "LOAD: $LOAD"
-            echo "XRUNS: $XRUNS"
-            echo "SAMPLERATE: $SAMPLERATE"
-        fi
-        ```
-        
-        Save this as `jack_status.sh` and use it like so:
-        
-        ```console
-        jack-dbus-monitor --interval-stats 1000 ./jack_status.sh
-        ```
-        
-        
-        ## LV2
-        
-        The scripts in the `jackaudiotools.lv2` package help with querying information
-        from the [LV2] plugins installed on the system.
-        
-        They require the [lilv] Python bindings to be installed. Unfortunately, these
-        can not be installed from the Python Package Index. Instead, install a recent
-        version of the `lilv` library, either from your distribution's package
-        repository or from source.
-        
-        
-        ### `lv2-grep`
-        
-        Print URIs of all installed LV2 plugins matching the given regular expression.
-        
-        Can optionally output the list of matching plugins in JSON format, where each
-        list item is an object with the plugin name and uri and optionally the list of
-        categories the plugin belongs to, as properties.
-        
-        
-        ### `lv2-plugin-uris`
-        
-        Print a list of all URIs associated with an LV2 plugin.
-        
-        
-        ### `lv2-list-plugin-presets`
-        
-        List all presets of an LV2 plugin with the given URI.
-        
-        
-        ### `lv2-plugin-info`
-        
-        Generate a JSON document with information about a single or all installed LV2
-        plugins. This allows plugin meta data to be loaded quickly in other programs.
-        
-        Depending on the number of plugins installed on your system, this script may
-        run for several seconds or even minutes and produce an output file of several
-        megabytes in size.
-        
-        
-        ## Carla
-        
-        The scripts in the `jackaudiotools.carla` package manipulate or query [Carla]
-        project files.
-        
-        
-        ### `carxp2lv2presets`
-        
-        Export plugin settings from a Carla project file (.carxp) as LV2 preset bundles.
-        
-        This script requires the [rdflib] package to be installed. To install it,
-        specify the `rdflib` extra dependency when installing the `jack-audio-tools`
-        distribution via `pip`:
-        
-            pip install "jack-audio-tools[rdflib]"
-        
-        
-        ## License
-        
-        This software is distributed under the MIT License.
-        
-        See the file [LICENSE](./LICENSE) for more information.
-        
-        
-        ## Author
-        
-        This software is written by *Christopher Arndt*.
-        
-        
-        [carla]: https://kx.studio/Applications:Carla
-        [dbus-python]: https://pypi.org/project/dbus-python
-        [jack-client]: https://pypi.org/project/JACK-Client
-        [jack]: https://jackaudio.org/
-        [lilv]: http://drobilla.net/software/lilv
-        [lv2]: http://lv2plug.in/
-        [PyGObject]: https://pypi.org/project/PyGobject
-        [python-rtmidi]: https://pypi.org/project/python-rtmidi
-        [rdflib]: https://pypi.org/project/rdflib
-        
 Keywords: jack,jackaudio,LV2,carla,MIDI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: rtmidi
 Provides-Extra: rdflib
 Provides-Extra: dbus
+License-File: LICENSE
+
+# jack-audio-tools
+
+A collection of utilities and tools for the [JACK] audio ecosystem
+
+
+## JACK Transport
+
+The scripts in the `jackaudiotools.transport` package query or manipulate the
+JACK transport state.
+
+They require the [JACK-Client] package to be installed, which will be installed
+automatically, when you install the `jack-audio-tools` distribution via `pip`:
+
+    pip install jack-audio-tools
+
+
+### `jack-midi-to-transport`
+
+JACK client which allows to control transport state via MIDI.
+
+The client provides a MIDI input and converts received MIDI system real-time
+and MIDI machine control (MMC) messages into JACK transport commands.
+
+The following MIDI messages, when received, start the JACK transport:
+
+* `START` (System Real-time)
+* `CONTINUE` (System Real-time)
+* `PLAY` (MMC)
+* `DEFERRED PLAY` (MMC)
+
+These messages stop the transport:
+
+* `STOP` (System Real-time)
+* `STOP` (MMC)
+* `PAUSE` (MMC)
+* `RESET` (MMC)
+
+And these rewind the transport to frame zero:
+
+* `REWIND` (MMC)
+* `RESET` (MMC)
+
+MMC messages are ignored, if the device number in the MMC System Exclusive
+message does not match the client's device number (set with the -d command
+line option).
+
+If the client's device number is set to 127 (the default), it matches all
+MMC message device numbers.
+
+
+### `jack-rtmidi-to-transport`
+
+JACK client which allows to control transport state via MIDI.
+
+A variant of `midi_to_transport`, which uses the [python-rtmidi] package
+as a MIDI backend instead of JACK-Client, which is slightly more efficient,
+because MIDI input processing is happening in a C++ thread instead of a
+Python callback.
+
+To use it, specify the `rtmidi` extra dependency when installing the
+`jack-audio-tools` distribution via `pip`:
+
+    pip install "jack-audio-tools[rtmidi]"
+
+
+### `jack-timebase-master`
+
+A simple JACK timebase master, which provides  musical timing related
+information (i.e. currents bar, beats per bar, beat denominator, BPM etc.)
+to other JACK clients.
+
+
+### `jack-transporter`
+
+Query or change the JACK transport state.
+
+
+## JACK D-BUS
+
+The scripts in the `jackaudiotools.jackdbus` package interface with the JACK
+D-BUS service to query information about the status of the JACK server and/or
+control its operation.
+
+These scripts require the [PyGobject]  and [dbus-python] packages to be
+installed. To install these, specify the `dbus` extra dependency when
+installing the `jack-audio-tools` distribution via `pip`:
+
+    pip install "jack-audio-tools[dbus]"
+
+
+### `jack-dbus-monitor`
+
+This script monitors the JACK server via D-BUS and runs a command on status
+changes and optionally at a given interval passing some JACK stats in the
+environment.
+
+Here is an example shell script to use as a command:
+
+```bash
+#!/bin/bash
+
+event="$1"  # 'start', 'stop' or 'status'
+echo "JACK event: $event"
+
+if [[ "$event" = "status" ]]; then
+    echo "IS_STARTED: $IS_STARTED"
+    echo "IS_REALTIME: $IS_REALTIME"
+    echo "PERIOD: $PERIOD"
+    echo "LATENCY: $LATENCY"
+    echo "LOAD: $LOAD"
+    echo "XRUNS: $XRUNS"
+    echo "SAMPLERATE: $SAMPLERATE"
+fi
+```
+
+Save this as `jack_status.sh` and use it like so:
+
+```console
+jack-dbus-monitor --interval-stats 1000 ./jack_status.sh
+```
+
+
+## LV2
+
+The scripts in the `jackaudiotools.lv2` package help with querying information
+from the [LV2] plugins installed on the system.
+
+They require the [lilv] Python bindings to be installed. Unfortunately, these
+can not be installed from the Python Package Index. Instead, install a recent
+version of the `lilv` library, either from your distribution's package
+repository or from source.
+
+
+### `lv2-grep`
+
+Print URIs of all installed LV2 plugins matching the given regular expression.
+
+Can optionally output the list of matching plugins in JSON format, where each
+list item is an object with the plugin name and uri and optionally the list of
+categories the plugin belongs to, as properties.
+
+
+### `lv2-plugin-uris`
+
+Print a list of all URIs associated with an LV2 plugin.
+
+
+### `lv2-list-plugin-presets`
+
+List all presets of an LV2 plugin with the given URI.
+
+
+### `lv2-plugin-info`
+
+Generate a JSON document with information about a single or all installed LV2
+plugins. This allows plugin meta data to be loaded quickly in other programs.
+
+Depending on the number of plugins installed on your system, this script may
+run for several seconds or even minutes and produce an output file of several
+megabytes in size.
+
+
+## Carla
+
+The scripts in the `jackaudiotools.carla` package manipulate or query [Carla]
+project files.
+
+
+### `carxp2lv2presets`
+
+Export plugin settings from a Carla project file (.carxp) as LV2 preset bundles.
+
+This script requires the [rdflib] package to be installed. To install it,
+specify the `rdflib` extra dependency when installing the `jack-audio-tools`
+distribution via `pip`:
+
+    pip install "jack-audio-tools[rdflib]"
+
+
+## License
+
+This software is distributed under the MIT License.
+
+See the file [LICENSE](./LICENSE) for more information.
+
+
+## Author
+
+This software is written by *Christopher Arndt*.
+
+
+[carla]: https://kx.studio/Applications:Carla
+[dbus-python]: https://pypi.org/project/dbus-python
+[jack-client]: https://pypi.org/project/JACK-Client
+[jack]: https://jackaudio.org/
+[lilv]: http://drobilla.net/software/lilv
+[lv2]: http://lv2plug.in/
+[PyGObject]: https://pypi.org/project/PyGobject
+[python-rtmidi]: https://pypi.org/project/python-rtmidi
+[rdflib]: https://pypi.org/project/rdflib
```

### Comparing `jack-audio-tools-0.4.0/README.md` & `jack-audio-tools-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/carla/carxp2lv2presets.py` & `jack-audio-tools-0.4.1/carla/carxp2lv2presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,25 +67,25 @@
                 # XXX: handle other Atom types?
                 value = Literal(prop.value)
 
             graph.add((state, URIRef(prop.key), value))
 
         graph.add((preset, NS.state.state, state))
 
-    return graph.serialize(format='turtle').decode()
+    return graph.serialize(format='turtle')
 
 
 def create_manifest(uri, filename):
     graph = get_graph()
     preset = URIRef(filename)
     graph.add((preset, RDF.type, NS.pset.Preset))
     graph.add((preset, NS.lv2.appliesTo, URIRef(uri)))
     graph.add((preset, RDFS.seeAlso, URIRef(filename)))
 
-    return graph.serialize(format='turtle').decode()
+    return graph.serialize(format='turtle')
 
 
 def link_or_copy_path(path, dst, always_copy=False):
     if exists(path):
         success = False
 
         if not always_copy:
```

### Comparing `jack-audio-tools-0.4.0/carla/loadcarxp.py` & `jack-audio-tools-0.4.1/carla/loadcarxp.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/jack_audio_tools.egg-info/PKG-INFO` & `jack-audio-tools-0.4.1/jack_audio_tools.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,225 +1,226 @@
 Metadata-Version: 2.1
 Name: jack-audio-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: A collection of utilities and tools for the JACK audio ecosystem
 Home-page: https://github.com/SpotlightKid/jack-audio-tools
 Author: Christopher Arndt
 Author-email: info@chrisarndt.de
 License: MIT License
-Description: # jack-audio-tools
-        
-        A collection of utilities and tools for the [JACK] audio ecosystem
-        
-        
-        ## JACK Transport
-        
-        The scripts in the `jackaudiotools.transport` package query or manipulate the
-        JACK transport state.
-        
-        They require the [JACK-Client] package to be installed, which will be installed
-        automatically, when you install the `jack-audio-tools` distribution via `pip`:
-        
-            pip install jack-audio-tools
-        
-        
-        ### `jack-midi-to-transport`
-        
-        JACK client which allows to control transport state via MIDI.
-        
-        The client provides a MIDI input and converts received MIDI system real-time
-        and MIDI machine control (MMC) messages into JACK transport commands.
-        
-        The following MIDI messages, when received, start the JACK transport:
-        
-        * `START` (System Real-time)
-        * `CONTINUE` (System Real-time)
-        * `PLAY` (MMC)
-        * `DEFERRED PLAY` (MMC)
-        
-        These messages stop the transport:
-        
-        * `STOP` (System Real-time)
-        * `STOP` (MMC)
-        * `PAUSE` (MMC)
-        * `RESET` (MMC)
-        
-        And these rewind the transport to frame zero:
-        
-        * `REWIND` (MMC)
-        * `RESET` (MMC)
-        
-        MMC messages are ignored, if the device number in the MMC System Exclusive
-        message does not match the client's device number (set with the -d command
-        line option).
-        
-        If the client's device number is set to 127 (the default), it matches all
-        MMC message device numbers.
-        
-        
-        ### `jack-rtmidi-to-transport`
-        
-        JACK client which allows to control transport state via MIDI.
-        
-        A variant of `midi_to_transport`, which uses the [python-rtmidi] package
-        as a MIDI backend instead of JACK-Client, which is slightly more efficient,
-        because MIDI input processing is happening in a C++ thread instead of a
-        Python callback.
-        
-        To use it, specify the `rtmidi` extra dependency when installing the
-        `jack-audio-tools` distribution via `pip`:
-        
-            pip install "jack-audio-tools[rtmidi]"
-        
-        
-        ### `jack-timebase-master`
-        
-        A simple JACK timebase master, which provides  musical timing related
-        information (i.e. currents bar, beats per bar, beat denominator, BPM etc.)
-        to other JACK clients.
-        
-        
-        ### `jack-transporter`
-        
-        Query or change the JACK transport state.
-        
-        
-        ## JACK D-BUS
-        
-        The scripts in the `jackaudiotools.jackdbus` package interface with the JACK
-        D-BUS service to query information about the status of the JACK server and/or
-        control its operation.
-        
-        These scripts require the [PyGobject]  and [dbus-python] packages to be
-        installed. To install these, specify the `dbus` extra dependency when
-        installing the `jack-audio-tools` distribution via `pip`:
-        
-            pip install "jack-audio-tools[dbus]"
-        
-        
-        ### `jack-dbus-monitor`
-        
-        This script monitors the JACK server via D-BUS and runs a command on status
-        changes and optionally at a given interval passing some JACK stats in the
-        environment.
-        
-        Here is an example shell script to use as a command:
-        
-        ```bash
-        #!/bin/bash
-        
-        event="$1"  # 'start', 'stop' or 'status'
-        echo "JACK event: $event"
-        
-        if [[ "$event" = "status" ]]; then
-            echo "IS_STARTED: $IS_STARTED"
-            echo "IS_REALTIME: $IS_REALTIME"
-            echo "PERIOD: $PERIOD"
-            echo "LATENCY: $LATENCY"
-            echo "LOAD: $LOAD"
-            echo "XRUNS: $XRUNS"
-            echo "SAMPLERATE: $SAMPLERATE"
-        fi
-        ```
-        
-        Save this as `jack_status.sh` and use it like so:
-        
-        ```console
-        jack-dbus-monitor --interval-stats 1000 ./jack_status.sh
-        ```
-        
-        
-        ## LV2
-        
-        The scripts in the `jackaudiotools.lv2` package help with querying information
-        from the [LV2] plugins installed on the system.
-        
-        They require the [lilv] Python bindings to be installed. Unfortunately, these
-        can not be installed from the Python Package Index. Instead, install a recent
-        version of the `lilv` library, either from your distribution's package
-        repository or from source.
-        
-        
-        ### `lv2-grep`
-        
-        Print URIs of all installed LV2 plugins matching the given regular expression.
-        
-        Can optionally output the list of matching plugins in JSON format, where each
-        list item is an object with the plugin name and uri and optionally the list of
-        categories the plugin belongs to, as properties.
-        
-        
-        ### `lv2-plugin-uris`
-        
-        Print a list of all URIs associated with an LV2 plugin.
-        
-        
-        ### `lv2-list-plugin-presets`
-        
-        List all presets of an LV2 plugin with the given URI.
-        
-        
-        ### `lv2-plugin-info`
-        
-        Generate a JSON document with information about a single or all installed LV2
-        plugins. This allows plugin meta data to be loaded quickly in other programs.
-        
-        Depending on the number of plugins installed on your system, this script may
-        run for several seconds or even minutes and produce an output file of several
-        megabytes in size.
-        
-        
-        ## Carla
-        
-        The scripts in the `jackaudiotools.carla` package manipulate or query [Carla]
-        project files.
-        
-        
-        ### `carxp2lv2presets`
-        
-        Export plugin settings from a Carla project file (.carxp) as LV2 preset bundles.
-        
-        This script requires the [rdflib] package to be installed. To install it,
-        specify the `rdflib` extra dependency when installing the `jack-audio-tools`
-        distribution via `pip`:
-        
-            pip install "jack-audio-tools[rdflib]"
-        
-        
-        ## License
-        
-        This software is distributed under the MIT License.
-        
-        See the file [LICENSE](./LICENSE) for more information.
-        
-        
-        ## Author
-        
-        This software is written by *Christopher Arndt*.
-        
-        
-        [carla]: https://kx.studio/Applications:Carla
-        [dbus-python]: https://pypi.org/project/dbus-python
-        [jack-client]: https://pypi.org/project/JACK-Client
-        [jack]: https://jackaudio.org/
-        [lilv]: http://drobilla.net/software/lilv
-        [lv2]: http://lv2plug.in/
-        [PyGObject]: https://pypi.org/project/PyGobject
-        [python-rtmidi]: https://pypi.org/project/python-rtmidi
-        [rdflib]: https://pypi.org/project/rdflib
-        
 Keywords: jack,jackaudio,LV2,carla,MIDI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: rtmidi
 Provides-Extra: rdflib
 Provides-Extra: dbus
+License-File: LICENSE
+
+# jack-audio-tools
+
+A collection of utilities and tools for the [JACK] audio ecosystem
+
+
+## JACK Transport
+
+The scripts in the `jackaudiotools.transport` package query or manipulate the
+JACK transport state.
+
+They require the [JACK-Client] package to be installed, which will be installed
+automatically, when you install the `jack-audio-tools` distribution via `pip`:
+
+    pip install jack-audio-tools
+
+
+### `jack-midi-to-transport`
+
+JACK client which allows to control transport state via MIDI.
+
+The client provides a MIDI input and converts received MIDI system real-time
+and MIDI machine control (MMC) messages into JACK transport commands.
+
+The following MIDI messages, when received, start the JACK transport:
+
+* `START` (System Real-time)
+* `CONTINUE` (System Real-time)
+* `PLAY` (MMC)
+* `DEFERRED PLAY` (MMC)
+
+These messages stop the transport:
+
+* `STOP` (System Real-time)
+* `STOP` (MMC)
+* `PAUSE` (MMC)
+* `RESET` (MMC)
+
+And these rewind the transport to frame zero:
+
+* `REWIND` (MMC)
+* `RESET` (MMC)
+
+MMC messages are ignored, if the device number in the MMC System Exclusive
+message does not match the client's device number (set with the -d command
+line option).
+
+If the client's device number is set to 127 (the default), it matches all
+MMC message device numbers.
+
+
+### `jack-rtmidi-to-transport`
+
+JACK client which allows to control transport state via MIDI.
+
+A variant of `midi_to_transport`, which uses the [python-rtmidi] package
+as a MIDI backend instead of JACK-Client, which is slightly more efficient,
+because MIDI input processing is happening in a C++ thread instead of a
+Python callback.
+
+To use it, specify the `rtmidi` extra dependency when installing the
+`jack-audio-tools` distribution via `pip`:
+
+    pip install "jack-audio-tools[rtmidi]"
+
+
+### `jack-timebase-master`
+
+A simple JACK timebase master, which provides  musical timing related
+information (i.e. currents bar, beats per bar, beat denominator, BPM etc.)
+to other JACK clients.
+
+
+### `jack-transporter`
+
+Query or change the JACK transport state.
+
+
+## JACK D-BUS
+
+The scripts in the `jackaudiotools.jackdbus` package interface with the JACK
+D-BUS service to query information about the status of the JACK server and/or
+control its operation.
+
+These scripts require the [PyGobject]  and [dbus-python] packages to be
+installed. To install these, specify the `dbus` extra dependency when
+installing the `jack-audio-tools` distribution via `pip`:
+
+    pip install "jack-audio-tools[dbus]"
+
+
+### `jack-dbus-monitor`
+
+This script monitors the JACK server via D-BUS and runs a command on status
+changes and optionally at a given interval passing some JACK stats in the
+environment.
+
+Here is an example shell script to use as a command:
+
+```bash
+#!/bin/bash
+
+event="$1"  # 'start', 'stop' or 'status'
+echo "JACK event: $event"
+
+if [[ "$event" = "status" ]]; then
+    echo "IS_STARTED: $IS_STARTED"
+    echo "IS_REALTIME: $IS_REALTIME"
+    echo "PERIOD: $PERIOD"
+    echo "LATENCY: $LATENCY"
+    echo "LOAD: $LOAD"
+    echo "XRUNS: $XRUNS"
+    echo "SAMPLERATE: $SAMPLERATE"
+fi
+```
+
+Save this as `jack_status.sh` and use it like so:
+
+```console
+jack-dbus-monitor --interval-stats 1000 ./jack_status.sh
+```
+
+
+## LV2
+
+The scripts in the `jackaudiotools.lv2` package help with querying information
+from the [LV2] plugins installed on the system.
+
+They require the [lilv] Python bindings to be installed. Unfortunately, these
+can not be installed from the Python Package Index. Instead, install a recent
+version of the `lilv` library, either from your distribution's package
+repository or from source.
+
+
+### `lv2-grep`
+
+Print URIs of all installed LV2 plugins matching the given regular expression.
+
+Can optionally output the list of matching plugins in JSON format, where each
+list item is an object with the plugin name and uri and optionally the list of
+categories the plugin belongs to, as properties.
+
+
+### `lv2-plugin-uris`
+
+Print a list of all URIs associated with an LV2 plugin.
+
+
+### `lv2-list-plugin-presets`
+
+List all presets of an LV2 plugin with the given URI.
+
+
+### `lv2-plugin-info`
+
+Generate a JSON document with information about a single or all installed LV2
+plugins. This allows plugin meta data to be loaded quickly in other programs.
+
+Depending on the number of plugins installed on your system, this script may
+run for several seconds or even minutes and produce an output file of several
+megabytes in size.
+
+
+## Carla
+
+The scripts in the `jackaudiotools.carla` package manipulate or query [Carla]
+project files.
+
+
+### `carxp2lv2presets`
+
+Export plugin settings from a Carla project file (.carxp) as LV2 preset bundles.
+
+This script requires the [rdflib] package to be installed. To install it,
+specify the `rdflib` extra dependency when installing the `jack-audio-tools`
+distribution via `pip`:
+
+    pip install "jack-audio-tools[rdflib]"
+
+
+## License
+
+This software is distributed under the MIT License.
+
+See the file [LICENSE](./LICENSE) for more information.
+
+
+## Author
+
+This software is written by *Christopher Arndt*.
+
+
+[carla]: https://kx.studio/Applications:Carla
+[dbus-python]: https://pypi.org/project/dbus-python
+[jack-client]: https://pypi.org/project/JACK-Client
+[jack]: https://jackaudio.org/
+[lilv]: http://drobilla.net/software/lilv
+[lv2]: http://lv2plug.in/
+[PyGObject]: https://pypi.org/project/PyGobject
+[python-rtmidi]: https://pypi.org/project/python-rtmidi
+[rdflib]: https://pypi.org/project/rdflib
```

### Comparing `jack-audio-tools-0.4.0/jack_audio_tools.egg-info/entry_points.txt` & `jack-audio-tools-0.4.1/jack_audio_tools.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,7 @@
 jack-rtmidi-to-transport = jackaudiotools.transport.rtmidi_to_transport:main [rtmidi]
 jack-timebase-master = jackaudiotools.transport.timebase_master:main
 jack-transporter = jackaudiotools.transport.transporter:main
 lv2-grep = jackaudiotools.lv2.grep:main
 lv2-list-plugin-presets = jackaudiotools.lv2.list_plugin_presets:main
 lv2-plugin-info = jackaudiotools.lv2.plugin_info:main
 lv2-plugin-uris = jackaudiotools.lv2.plugin_uris:main
-
```

### Comparing `jack-audio-tools-0.4.0/jackdbus/jackmonitor.py` & `jack-audio-tools-0.4.1/jackdbus/jackmonitor.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/lv2/grep.py` & `jack-audio-tools-0.4.1/lv2/grep.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/lv2/list_plugin_presets.py` & `jack-audio-tools-0.4.1/lv2/list_plugin_presets.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/lv2/plugin_info.py` & `jack-audio-tools-0.4.1/lv2/plugin_info.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/lv2/plugin_uris.py` & `jack-audio-tools-0.4.1/lv2/plugin_uris.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/setup.py` & `jack-audio-tools-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,22 +39,23 @@
 classifiers = """\
 Development Status :: 4 - Beta
 Environment :: Console
 Operating System :: POSIX
 License :: OSI Approved :: MIT License
 Programming Language :: Python
 Programming Language :: Python :: 3 :: Only
-Programming Language :: Python :: 3.7
-Programming Language :: Python :: 3.8
+Programming Language :: Python :: 3.9
+Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Topic :: Multimedia :: Sound/Audio
 """
 
 setup(
     name='jack-audio-tools',
-    version="0.4.0",
+    version="0.4.1",
     description="A collection of utilities and tools for the JACK audio ecosystem",
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     url="https://github.com/SpotlightKid/jack-audio-tools",
     license='MIT License',
     author="Christopher Arndt",
     author_email="info@chrisarndt.de",
```

### Comparing `jack-audio-tools-0.4.0/transport/midi_to_transport.py` & `jack-audio-tools-0.4.1/transport/midi_to_transport.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/transport/rtmidi_to_transport.py` & `jack-audio-tools-0.4.1/transport/rtmidi_to_transport.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/transport/timebase_master.py` & `jack-audio-tools-0.4.1/transport/timebase_master.py`

 * *Files identical despite different names*

### Comparing `jack-audio-tools-0.4.0/transport/transporter.py` & `jack-audio-tools-0.4.1/transport/transporter.py`

 * *Files identical despite different names*

