# Comparing `tmp/ovos_tts_plugin_mimic3-0.0.1a1-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_mimic3-0.0.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21250 bytes, number of entries: 8
--rw-r--r--  2.0 unx    62742 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3/version.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1738 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      192 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      766 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD
-8 files, 100253 bytes uncompressed, 19884 bytes compressed:  80.2%
+Zip file size: 21360 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    63013 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3/version.py
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3-0.0.1a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1738 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3-0.0.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3-0.0.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3-0.0.1a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3-0.0.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      766 b- defN 23-Jun-10 02:30 ovos_tts_plugin_mimic3-0.0.1a2.dist-info/RECORD
+8 files, 100524 bytes uncompressed, 19994 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_tts_plugin_mimic3/__init__.py
 Comment: 
 
 Filename: ovos_tts_plugin_mimic3/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE
+Filename: ovos_tts_plugin_mimic3-0.0.1a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA
+Filename: ovos_tts_plugin_mimic3-0.0.1a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/WHEEL
+Filename: ovos_tts_plugin_mimic3-0.0.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_mimic3-0.0.1a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/top_level.txt
+Filename: ovos_tts_plugin_mimic3-0.0.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD
+Filename: ovos_tts_plugin_mimic3-0.0.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_mimic3/__init__.py

```diff
@@ -90,14 +90,18 @@
             if lang not in self.default_voices:
                 lang = lang.split("-")[0]
             voice = self.default_voices.get(lang)
             if voice:
                 self.tts.preload_voice(voice)
 
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
```

## ovos_tts_plugin_mimic3/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 1
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE` & `ovos_tts_plugin_mimic3-0.0.1a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA` & `ovos_tts_plugin_mimic3-0.0.1a2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-mimic3
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Text to speech plugin for OpenVoiceOS using Mimic3
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-mimic3
 Author: Michael Hansen
 License: AGPL
 Keywords: mycroft plugin tts mimic mimic3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD` & `ovos_tts_plugin_mimic3-0.0.1a2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_tts_plugin_mimic3/__init__.py,sha256=xCuImKD0YvcmKSvcZ-TIScvogMREWSG6r9pKp6RlSm4,62742
-ovos_tts_plugin_mimic3/version.py,sha256=ngFn7CKVyhopdVfKT4gcARfNTt6vFxPLcvHzSZ4vXJY,177
-ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
-ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA,sha256=9oGtIJU5JodSN8b8JUG3vXG_-laQbN2YIEWSncmHpjI,1738
-ovos_tts_plugin_mimic3-0.0.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_mimic3-0.0.1a1.dist-info/entry_points.txt,sha256=vXVkVOvAevScIuedidXp7Ywp-cmndl7Y5hNSvTzc7QQ,192
-ovos_tts_plugin_mimic3-0.0.1a1.dist-info/top_level.txt,sha256=6lmA5NRKPpK3Zlab3O4ZCwwHshZMyqs-QGMzJ7mqC5o,23
-ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD,,
+ovos_tts_plugin_mimic3/__init__.py,sha256=qBcjZw8G5FJWk8P5AruXDGpbo5nfMiU1LukC741Hskk,63013
+ovos_tts_plugin_mimic3/version.py,sha256=QabbAoPiuLIjnxlTrr_3_4mlDBN2PLYjBj91Rbb2DJc,177
+ovos_tts_plugin_mimic3-0.0.1a2.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
+ovos_tts_plugin_mimic3-0.0.1a2.dist-info/METADATA,sha256=uTrWZMA0xwrsepI7De95w84ICsTEunPeujv82RIbGgM,1738
+ovos_tts_plugin_mimic3-0.0.1a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_mimic3-0.0.1a2.dist-info/entry_points.txt,sha256=vXVkVOvAevScIuedidXp7Ywp-cmndl7Y5hNSvTzc7QQ,192
+ovos_tts_plugin_mimic3-0.0.1a2.dist-info/top_level.txt,sha256=6lmA5NRKPpK3Zlab3O4ZCwwHshZMyqs-QGMzJ7mqC5o,23
+ovos_tts_plugin_mimic3-0.0.1a2.dist-info/RECORD,,
```

