# Comparing `tmp/ovos_tts_plugin_mimic3_server-0.0.2a1-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_mimic3_server-0.0.2a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13505 bytes, number of entries: 9
--rw-r--r--  2.0 unx    60739 b- defN 23-Mar-14 18:08 ovos_tts_plugin_mimic3_server/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1141 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      232 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      932 b- defN 23-Mar-14 18:09 ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/RECORD
-9 files, 74693 bytes uncompressed, 11839 bytes compressed:  84.1%
+Zip file size: 13624 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    61039 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1141 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jun-10 02:13 ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/RECORD
+9 files, 74993 bytes uncompressed, 11958 bytes compressed:  84.1%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_tts_plugin_mimic3_server/__init__.py
 Comment: 
 
 Filename: ovos_tts_plugin_mimic3_server/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/LICENSE
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/METADATA
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/WHEEL
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/top_level.txt
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/zip-safe
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/RECORD
+Filename: ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_mimic3_server/__init__.py

```diff
@@ -55,14 +55,18 @@
                 config["voice"] = voice
             else:
                 LOG.warning("Default mimic3 voice not set!")
         super().__init__(lang, config, audio_ext='wav', ssml_tags=ssml_tags)
         self.url = self.config.get("url")
 
     def _validate_args_combo(self, lang=None, voice=None, speaker=None):
+        # HACK: bug in some neon-core versions - neon_audio.tts.neon:_get_tts:198 - INFO - Legacy Neon TTS signature found 
+        if isinstance(speaker, dict):
+            LOG.warning("Legacy Neon TTS signature found, pass speaker as a str")
+            speaker = None
         if voice:
             if "#" in voice:
                 voice, new_speaker = voice.split("#")
                 if speaker and speaker != new_speaker:
                     LOG.warning(f"speaker defined twice! choosing {new_speaker} over {speaker} for voice: {voice}")
                 speaker = new_speaker
         elif lang:
@@ -74,15 +78,15 @@
                 raise ValueError(f"Selected lang {lang} is not supported!")
         elif speaker:
             pass  # TODO validate speaker is valid for default voice
         else:
             LOG.debug("using mimic3 default config, no voice requested")
             return self.voice
 
-        if speaker and not voice.endswith(f"#{speaker}"):
+        if speaker and isinstance(speaker, str) and not voice.endswith(f"#{speaker}"):
             voice = f"{voice}#{speaker}"
 
         if lang:
             a, b = lang.split("-")
             lang = f"{a}_{b.upper()}"
 
             if "/" in voice:
```

## ovos_tts_plugin_mimic3_server/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/LICENSE` & `ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/METADATA` & `ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-mimic3-server
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: Mimic3 server plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-mimic3-server
 Author: OpenVoiceOS
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Keywords: mycroft ovos plugin tts
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/RECORD` & `ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ovos_tts_plugin_mimic3_server/__init__.py,sha256=e3OMW2-JtKhYfsKQAhNzuUojXhDFLU23MuK2bMHA9Cs,60739
-ovos_tts_plugin_mimic3_server/version.py,sha256=RQUQPmSSpGFvMzBFjxHGeZbeIC--EWTSsSe__A3_--s,177
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/METADATA,sha256=T7uRGux9KsYoRTwOG_Wtx2oq-EenF5kEGr-Mspwt1eM,1141
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/entry_points.txt,sha256=x5t7BhCFh8FXbqVALhQ79zAlXZ-8ae27fZ13XmTl3I0,232
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/top_level.txt,sha256=VZkZE4gABAKozVkyVeGK6eI8KYtEgKfly5eywr9fuaA,30
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_mimic3_server-0.0.2a1.dist-info/RECORD,,
+ovos_tts_plugin_mimic3_server/__init__.py,sha256=rjXTiMdNWcelF8CDuD2Rd2Frvv4R32--e1mEyETTNDs,61039
+ovos_tts_plugin_mimic3_server/version.py,sha256=afVkQ7_AdQfLgFZ-hJN_LyKZAc5EOc9ZSwssDiyGXfM,177
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/METADATA,sha256=YX9w0tqGkR3fJPcJ2a5kbOV8TblX7qtcmZhi6Rjtz0E,1141
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/entry_points.txt,sha256=x5t7BhCFh8FXbqVALhQ79zAlXZ-8ae27fZ13XmTl3I0,232
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/top_level.txt,sha256=VZkZE4gABAKozVkyVeGK6eI8KYtEgKfly5eywr9fuaA,30
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_mimic3_server-0.0.2a2.dist-info/RECORD,,
```

