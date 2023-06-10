# Comparing `tmp/ovos_tts_plugin_piper-0.0.1a1-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_piper-0.0.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10997 bytes, number of entries: 10
--rw-r--r--  2.0 unx    11670 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper/__init__.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper/engine.py
--rw-r--r--  2.0 unx      178 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      948 b- defN 23-Apr-30 18:10 ovos_tts_plugin_piper-0.0.1a1.dist-info/RECORD
-10 files, 30029 bytes uncompressed, 9337 bytes compressed:  68.9%
+Zip file size: 11115 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    11941 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper/__init__.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper/engine.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jun-10 02:35 ovos_tts_plugin_piper-0.0.1a2.dist-info/RECORD
+10 files, 30300 bytes uncompressed, 9455 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: ovos_tts_plugin_piper/engine.py
 Comment: 
 
 Filename: ovos_tts_plugin_piper/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/LICENSE
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/METADATA
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/WHEEL
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/top_level.txt
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/zip-safe
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.1a1.dist-info/RECORD
+Filename: ovos_tts_plugin_piper-0.0.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_piper/__init__.py

```diff
@@ -179,14 +179,18 @@
             lang (str): optional lang override
             speaker (int): optional speaker override
 
         Returns:
             tuple ((str) file location, (str) generated phonemes)
         """
         lang = lang or self.lang
+        # HACK: bug in some neon-core versions - neon_audio.tts.neon:_get_tts:198 - INFO - Legacy Neon TTS signature found 
+        if isinstance(speaker, dict):
+            LOG.warning("Legacy Neon TTS signature found, pass speaker as a str")
+            speaker = None
         wav_bytes = self.engine.synthesize(sentence,
                                            speaker_id=speaker or self.speaker,
                                            length_scale=self.length_scale,
                                            noise_scale=self.noise_scale,
                                            noise_w=self.noise_w)
         with open(wav_file, "wb") as f:
             f.write(wav_bytes)
```

## ovos_tts_plugin_piper/version.py

```diff
@@ -1,8 +1,8 @@
 
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 1
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_piper-0.0.1a1.dist-info/LICENSE` & `ovos_tts_plugin_piper-0.0.1a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_piper-0.0.1a1.dist-info/METADATA` & `ovos_tts_plugin_piper-0.0.1a2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-piper
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: piper tts plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-piper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft plugin tts OVOS OpenVoiceOS
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_piper-0.0.1a1.dist-info/RECORD` & `ovos_tts_plugin_piper-0.0.1a2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ovos_tts_plugin_piper/__init__.py,sha256=y_aMNE95UepdgAS7HRgDCV2adDSl2-H-BA9dlBclnJs,11670
+ovos_tts_plugin_piper/__init__.py,sha256=i_13K29JY_mQ5PRTUzrIASjlp8fIpWfLaTIdKsMB0ao,11941
 ovos_tts_plugin_piper/engine.py,sha256=WEB-2Uu9cmN3UQrltWYbB0PH1H0X03Fg6OnGXW-GS0s,4518
-ovos_tts_plugin_piper/version.py,sha256=JtQ5WIvPkKYhMy7MovRWxkh0y9SR_ws2nUwI1F8uCq0,178
-ovos_tts_plugin_piper-0.0.1a1.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_piper-0.0.1a1.dist-info/METADATA,sha256=0XCZwSAc60ZgIW4mN6AxLzuLV86YEDayyVdEw0n_8r0,1065
-ovos_tts_plugin_piper-0.0.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_piper-0.0.1a1.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
-ovos_tts_plugin_piper-0.0.1a1.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
-ovos_tts_plugin_piper-0.0.1a1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_piper-0.0.1a1.dist-info/RECORD,,
+ovos_tts_plugin_piper/version.py,sha256=6kpz-k7Zi2OO60IgEO_0PvzOXww-72qVhaIQzS0W5w0,178
+ovos_tts_plugin_piper-0.0.1a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_piper-0.0.1a2.dist-info/METADATA,sha256=_E0CX-hSVoL9ElxAkHWYc0vf6Ex6keANkq5s93Q3Q6M,1065
+ovos_tts_plugin_piper-0.0.1a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_piper-0.0.1a2.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
+ovos_tts_plugin_piper-0.0.1a2.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
+ovos_tts_plugin_piper-0.0.1a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_piper-0.0.1a2.dist-info/RECORD,,
```

