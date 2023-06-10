# Comparing `tmp/partitura-1.2.2.tar.gz` & `tmp/partitura-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partitura-1.2.2.tar", last modified: Wed May 10 15:57:15 2023, max compression
+gzip compressed data, was "partitura-1.3.0.tar", last modified: Sat Jun 10 09:51:19 2023, max compression
```

## Comparing `partitura-1.2.2.tar` & `partitura-1.3.0.tar`

### file list

```diff
@@ -1,95 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.440728 partitura-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-10 15:57:08.000000 partitura-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 15:57:15.440728 partitura-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-05-10 15:57:08.000000 partitura-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.420727 partitura-1.2.2/partitura/
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.424727 partitura-1.2.2/partitura/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   335762 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/assets/musicxml.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/assets/score_example.krn
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/assets/score_example.mei
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/assets/score_example.mid
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/assets/score_example.musicxml
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/directions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.428727 partitura-1.2.2/partitura/io/
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/exportaudio.py
--rw-r--r--   0 runner    (1001) docker     (123)    18808 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/exportmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    71850 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/exportmei.py
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/exportmidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    35404 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/exportmusicxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/exportparangonada.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importkern.py
--rw-r--r--   0 runner    (1001) docker     (123)    25482 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importmei.py
--rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importmidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importmusicxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importnakamura.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/importparangonada.py
--rw-r--r--   0 runner    (1001) docker     (123)    31691 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/matchfile_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25861 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/matchfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/matchlines_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/matchlines_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/io/musescore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.428727 partitura-1.2.2/partitura/musicanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/key_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32653 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/note_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    31215 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/performance_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/pitch_spelling.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/tonal_tension.py
--rw-r--r--   0 runner    (1001) docker     (123)    35763 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/musicanalysis/voice_separation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)   152020 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.432727 partitura-1.2.2/partitura/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)   113656 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/utils/music.py
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-10 15:57:08.000000 partitura-1.2.2/partitura/utils/synth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.424727 partitura-1.2.2/partitura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 15:57:15.000000 partitura-1.2.2/partitura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-10 15:57:15.000000 partitura-1.2.2/partitura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:57:15.000000 partitura-1.2.2/partitura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 15:57:15.000000 partitura-1.2.2/partitura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 15:57:15.000000 partitura-1.2.2/partitura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:57:15.440728 partitura-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-10 15:57:08.000000 partitura-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:57:15.436727 partitura-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_kern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_key_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_load_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_load_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_match_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    74764 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_match_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_mei.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_merge_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_metrical_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_midi_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_midi_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_nakamura.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_new_divs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_note_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_note_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_octave_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_parangonada.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_part_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_performance_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_pianoroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_pitch_spelling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_quarter_adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_rest_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_time_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_tonal_tension.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_voice_estimation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10275 2023-05-10 15:57:08.000000 partitura-1.2.2/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.524998 partitura-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-10 09:51:11.000000 partitura-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-10 09:51:19.524998 partitura-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-10 09:51:11.000000 partitura-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.512998 partitura-1.3.0/partitura/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.516998 partitura-1.3.0/partitura/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   335762 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/musicxml.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.krn
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.mei
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.mid
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/assets/score_example.musicxml
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/directions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.516998 partitura-1.3.0/partitura/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportaudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71850 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35404 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportmusicxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/exportparangonada.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importkern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26363 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42676 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmusic21.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56313 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importmusicxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importnakamura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/importparangonada.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31691 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchfile_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchlines_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/matchlines_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/io/musescore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.520998 partitura-1.3.0/partitura/musicanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/key_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/note_array_to_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38131 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/note_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/performance_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/performance_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/pitch_spelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/tonal_tension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35763 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/musicanalysis/voice_separation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152462 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.520998 partitura-1.3.0/partitura/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110587 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-06-10 09:51:11.000000 partitura-1.3.0/partitura/utils/synth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.512998 partitura-1.3.0/partitura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:51:19.000000 partitura-1.3.0/partitura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:51:19.524998 partitura-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-10 09:51:11.000000 partitura-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:51:19.524998 partitura-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_kern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_key_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_load_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_load_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_m21_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_match_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74764 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_match_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_mei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_merge_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_metrical_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_midi_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_midi_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_nakamura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_new_divs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_note_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_note_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_octave_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_parangonada.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_part_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_partial_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_performance_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_performance_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_pianoroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_pitch_spelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_quarter_adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_rest_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_time_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_tonal_tension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_voice_estimation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10316 2023-06-10 09:51:11.000000 partitura-1.3.0/tests/test_xml.py
```

### Comparing `partitura-1.2.2/LICENSE` & `partitura-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/PKG-INFO` & `partitura-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: partitura
-Version: 1.2.2
+Version: 1.3.0
 Summary: A package for handling symbolic musical information
 Home-page: https://github.com/CPJKU/partitura
 Author: Maarten Grachten, Carlos Cancino-Chacón, Silvan Peter, Emmanouil Karystinaios, Francesco Foscarin, Thassilo Gadermaier
 Author-email: partitura-users@googlegroups.com
 License: Apache 2.0
 Keywords: music notation musicxml midi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [//]: # (<p align="center"> )
 
 [//]: # (<img src="./partitura/assets/partitura_logo_final.jpg" height="200">)
```

### Comparing `partitura-1.2.2/README.md` & `partitura-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/__init__.py` & `partitura-1.3.0/partitura/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 
 from .io import load_score, load_performance, load_score_as_part, lp
 from .io.musescore import load_via_musescore
 from .io.importmusicxml import load_musicxml, musicxml_to_notearray
 from .io.exportmusicxml import save_musicxml
 from .io.importmei import load_mei
 from .io.importkern import load_kern
+from .io.importmusic21 import load_music21
 from .io.importmidi import load_score_midi, load_performance_midi, midi_to_notearray
 from .io.exportmidi import save_score_midi, save_performance_midi
 from .io.importmatch import load_match
 from .io.exportmatch import save_match
 from .io.importnakamura import load_nakamuramatch, load_nakamuracorresp
 from .io.importparangonada import load_parangonada_csv
 from .io.exportparangonada import save_parangonada_csv, save_csv_for_parangonada
 from .io.exportaudio import save_wav
 from .display import render
 from . import musicanalysis
 from .musicanalysis import make_note_features, compute_note_array, full_note_array
 
+
 # define a version variable
 __version__ = pkg_resources.get_distribution("partitura").version
 
 #: An example MusicXML file for didactic purposes
 EXAMPLE_MUSICXML = pkg_resources.resource_filename(
     "partitura", "assets/score_example.musicxml"
 )
```

### Comparing `partitura-1.2.2/partitura/assets/musicxml.xsd` & `partitura-1.3.0/partitura/assets/musicxml.xsd`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/assets/score_example.mei` & `partitura-1.3.0/partitura/assets/score_example.mei`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/assets/score_example.musicxml` & `partitura-1.3.0/partitura/assets/score_example.musicxml`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/directions.py` & `partitura-1.3.0/partitura/directions.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/display.py` & `partitura-1.3.0/partitura/display.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/__init__.py` & `partitura-1.3.0/partitura/io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .importmidi import load_score_midi, load_performance_midi
 from .musescore import load_via_musescore
 from .importmatch import load_match
 from .importmei import load_mei
 from .importkern import load_kern
 from .importparangonada import load_parangonada_csv
 from .exportparangonada import save_parangonada_csv
+from .importmusic21 import load_music21
 
 from partitura.utils.misc import (
     deprecated_alias,
     deprecated_parameter,
     PathLike,
 )
```

### Comparing `partitura-1.2.2/partitura/io/exportaudio.py` & `partitura-1.3.0/partitura/io/exportaudio.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/exportmatch.py` & `partitura-1.3.0/partitura/io/exportmatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,26 @@
 )
 
 from partitura import score
 from partitura.io.matchfile_base import MatchFile
 
 from partitura.utils.music import (
     seconds_to_midi_ticks,
-    get_time_maps_from_alignment,
 )
 
 from partitura.utils.misc import (
     PathLike,
     deprecated_alias,
     deprecated_parameter,
 )
 
+from partitura.musicanalysis.performance_codec import (
+    get_time_maps_from_alignment
+)
+
 __all__ = ["save_match"]
 
 
 @deprecated_parameter("magaloff_zeilinger_quirk")
 def matchfile_from_alignment(
     alignment: List[dict],
     ppart: PerformedPart,
```

### Comparing `partitura-1.2.2/partitura/io/exportmei.py` & `partitura-1.3.0/partitura/io/exportmei.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/exportmusicxml.py` & `partitura-1.3.0/partitura/io/exportmusicxml.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/exportparangonada.py` & `partitura-1.3.0/partitura/io/exportparangonada.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/importkern.py` & `partitura-1.3.0/partitura/io/importkern.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/importmatch.py` & `partitura-1.3.0/partitura/io/importmatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,22 +580,22 @@
         if not np.isclose(onset_divs, onset_in_divs[ni], atol=divs * 0.01):
             warnings.warn(
                 "Calculated `onset_divs` does not match `OnsetInBeats` " "information!."
             )
             onset_divs = onset_in_divs[ni]
         assert onset_divs >= 0
         assert np.isclose(onset_divs, onset_in_divs[ni], atol=divs * 0.01)
-
+        is_tied = False
         articulations = set()
         if "staccato" in note.ScoreAttributesList or "stac" in note.ScoreAttributesList:
             articulations.add("staccato")
         if "accent" in note.ScoreAttributesList:
             articulations.add("accent")
         if "leftOutTied" in note.ScoreAttributesList:
-            continue
+            is_tied = True
 
         # dictionary with keyword args with which the Note
         # (or GraceNote) will be instantiated
         note_attributes = dict(
             step=note.NoteName,
             octave=note.Octave,
             alter=note.Modifier,
@@ -673,14 +673,31 @@
                 )
 
             else:
                 part_note = score.Note(**note_attributes)
 
             part.add(part_note, onset_divs, offset_divs)
 
+        # Check if the note is tied and if so, add the tie information
+        if is_tied:
+            found = False
+            # iterate over all notes in the Timeline that end at the starting point.
+            for el in part_note.start.iter_ending(score.Note):
+                if isinstance(el, score.Note):
+                    condition = el.step == note_attributes["step"] and el.octave == note_attributes["octave"] and el.alter == note_attributes["alter"]
+                    if condition:
+                        el.tie_next = part_note
+                        part_note.tie_prev = el
+                        found = True
+                        break
+            if not found:
+                warnings.warn(
+                    "Tie information found, but no previous note found to tie to for note {}.".format(part_note.id)
+                )
+
     # add time signatures
     for (ts_beat_time, ts_bar, tsg) in ts:
         ts_beats = tsg.numerator
         ts_beat_type = tsg.denominator
         # check if time signature is in a known measure (from notes)
         if ts_bar in bar_times.keys():
             bar_start_divs = int(divs * (bar_times[ts_bar] - offset))  # in quarters
```

### Comparing `partitura-1.2.2/partitura/io/importmei.py` & `partitura-1.3.0/partitura/io/importmei.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import numpy as np
 
 
 @deprecated_alias(mei_path="filename")
 def load_mei(filename: PathLike) -> score.Score:
     """
-    Loads a Mei score from path and returns a list of Partitura.Part
+    Loads a Mei score from path and returns a partitura Score object.
 
     Parameters
     ----------
     filename : PathLike
         The path to an MEI score.
 
     Returns
@@ -1033,15 +1033,15 @@
                 warnings.warn(
                     f"Warning: tie {tie_el.attrib[self._ns_name('id',XML_NAMESPACE)]} is missing the a startid or endid"
                 )
             else:
                 # remove the # in first position
                 start_id = start_id[1:]
                 end_id = end_id[1:]
-                # set tie prev and tie next in partira note objects
+                # set tie prev and tie next in partitura note objects
                 all_notes_dict[start_id].tie_next = all_notes_dict[end_id]
                 all_notes_dict[end_id].tie_prev = all_notes_dict[start_id]
 
     def _insert_repetitions(self):
         if len(self.repetitions) == 0:
             return
         ## sanitize the found repetitions in case a starting rep is missing
```

### Comparing `partitura-1.2.2/partitura/io/importmidi.py` & `partitura-1.3.0/partitura/io/importmidi.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
 
         for ch, ch_notes in notes.items():
             # if there are any notes, store the notes along with key sig / time
             # sig / tempo information under the key (track_nr, ch_nr)
             if len(ch_notes) > 0:
                 notes_by_track_ch[(track_nr, ch)] = ch_notes
 
+
     tr_ch_keys = sorted(notes_by_track_ch.keys())
     group_part_voice_keys, part_names, group_names = assign_group_part_voice(
         part_voice_assign_mode, tr_ch_keys, track_names_by_track
     )
 
     # for key and time sigs:
     track_to_part_mapping = make_track_to_part_mapping(
```

### Comparing `partitura-1.2.2/partitura/io/importmusicxml.py` & `partitura-1.3.0/partitura/io/importmusicxml.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 PEDAL_DIRECTIONS = {
     "sustain_pedal": score.SustainPedalDirection,
 }
 
 OCTAVE_SHIFTS = {8: 1, 15: 2, 22: 3}
 
+
 def validate_musicxml(xml, debug=False):
     """
     Validate an XML file against an XSD.
 
     Parameters
     ----------
     xml: str
@@ -195,17 +196,15 @@
     """
 
     xml = None
     if isinstance(filename, str):
         if zipfile.is_zipfile(filename):
             with zipfile.ZipFile(filename) as zipped_xml:
                 contained_xml_name = zipped_xml.namelist()[-1]
-                xml = zipped_xml.open(
-                    contained_xml_name
-                )
+                xml = zipped_xml.open(contained_xml_name)
 
     if xml is None:
         xml = filename
 
     if validate:
         validate_musicxml(xml, debug=True)
         # if xml is a file-like object we need to set the read pointer to the
@@ -325,17 +324,17 @@
         position = 0
         ongoing = {}
         doc_order = 0
         # add new page and system at start of part
         _handle_new_page(position, part, ongoing)
         _handle_new_system(position, part, ongoing)
 
-        for measure_el in part_el.xpath("measure"):
+        for mc, measure_el in enumerate(part_el.xpath("measure")):
             position, doc_order = _handle_measure(
-                measure_el, position, part, ongoing, doc_order
+                measure_el, position, part, ongoing, doc_order, mc + 1
             )
 
         # complete unfinished endings
         for o in part.iter_all(score.Ending, mode="ending"):
             if o.start is None:
                 part.add(o, part.measure_map(o.end.t - 1)[0], None)
                 warnings.warn(
@@ -452,21 +451,43 @@
         #             if shift.shift_type == "up":
         #                 note.octave -= OCTAVE_SHIFTS[shift.shift_size] if shift.shift_size in OCTAVE_SHIFTS.keys() else 0
         #             elif shift.shift_type == "down":
         #                 note.octave += OCTAVE_SHIFTS[shift.shift_size] if shift.shift_size in OCTAVE_SHIFTS.keys() else 0
         #     shift.applied = True
 
 
-def _handle_measure(measure_el, position, part, ongoing, doc_order):
-    """
-    Parse a <measure>...</measure> element, adding it and its contents to the
-    part.
+def _handle_measure(measure_el, position, part, ongoing, doc_order, measure_counter):
+    """ Parse a <measure>...</measure> element, adding it and its contents to the part.
+    
+    Parameters
+    ----------
+    measure_el : etree.Element
+        An etree Element instance with a <measure> tag
+    position : int
+        The starting time of the measure
+    part : score.Part
+        The part object to which the measure belongs.
+    ongoing : dict
+        A dict specifying the score.Page and score.System of the measure
+    doc_order : int
+        The index of the first note element in the current measure in the xml file.
+    measure_counter : int
+        The index of the <measure> tag in the xml file, starting from 1
+    
+    Returns
+    -------
+    measure_maxtime : int
+        The ending time of the measure
+    doc_order : int
+        The index of the first note element in the next measure in the xml file.
+        
     """
+    
     # make a measure object
-    measure = make_measure(measure_el)
+    measure = make_measure(measure_el, measure_counter)
 
     # add the start of the measure to the time line
     part.add(measure, position)
 
     # keep track of the position within the measure
     # measure_pos = 0
     measure_start = position
@@ -583,15 +604,15 @@
             warnings.warn("ignoring tag {0}".format(e.tag), stacklevel=2)
 
     for obj in trailing_children:
         part.add(obj, measure_maxtime)
 
     # add end time of measure
     part.add(measure, None, measure_maxtime)
-
+    
     return measure_maxtime, doc_order
 
 
 def _handle_harmony(e, position, part):
     """Handle a <harmony> element."""
     if e.find("function") is not None:
         text = e.find("function").text
@@ -692,21 +713,34 @@
         system_nr = 1
 
     system = score.System(system_nr)
     part.add(system, position)
     ongoing["system"] = system
 
 
-def make_measure(xml_measure):
+def make_measure(xml_measure, measure_counter):
+    """
+    Parameters
+    ----------
+    xml_measure : etree.Element
+        An etree Element instance with a <measure> tag
+    measure_counter : int
+        The index of the <measure> tag in the xml file, starting from 1
+    
+    Returns
+    -------
+    measure : score.Measure
+        A measure object with a number and optional name attribute
+    """
+    
     measure = score.Measure()
-    # try:
-    #     measure.number = int(xml_measure.attrib['number'])
-    # except:
-    #     LOGGER.warn('No number attribute found for measure')
-    measure.number = get_value_from_attribute(xml_measure, "number", int)
+
+    measure.number = measure_counter
+    measure.name = get_value_from_attribute(xml_measure, "number", str)
+
     return measure
 
 
 def _handle_attributes(e, position, part):
     """"""
 
     ts_num = get_value_from_tag(e, "time/beats", int)
```

### Comparing `partitura-1.2.2/partitura/io/importnakamura.py` & `partitura-1.3.0/partitura/io/importnakamura.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/importparangonada.py` & `partitura-1.3.0/partitura/io/importparangonada.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/matchfile_base.py` & `partitura-1.3.0/partitura/io/matchfile_base.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/matchfile_utils.py` & `partitura-1.3.0/partitura/io/matchfile_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,30 +651,30 @@
     @fmt.setter
     def fmt(self, fmt: str) -> None:
         self._fmt = fmt
         for component in self.other_components:
             component.fmt = fmt
 
     def fifths_mode_to_key_name_v0_1_0(self, fifths: int, mode: str) -> str:
-        if mode == "major":
+        if mode in ("major", None, "none", 1):
             keylist = MAJOR_KEYS
             suffix = "major"
         elif mode == "minor":
             keylist = MINOR_KEYS
             suffix = "minor"
 
         step, alter, _ = note_name_to_pitch_spelling(f"{keylist[fifths + 7]}4")
         alter_str = "n" if (alter is None or alter == 0) else ALTER_SIGNS[alter]
         name = f"{step.lower()}{alter_str}"
         ks = f"[{name},{suffix}]"
 
         return ks
 
     def fifths_mode_to_key_name_v0_3_0(self, fifths: int, mode: str) -> str:
-        if mode == "major":
+        if mode in ("major", None, "none", 1):
             keylist = MAJOR_KEYS
             suffix = "Maj"
         elif mode == "minor":
             keylist = MINOR_KEYS
             suffix = "min"
 
         name = keylist[fifths + 7]
```

### Comparing `partitura-1.2.2/partitura/io/matchlines_v0.py` & `partitura-1.3.0/partitura/io/matchlines_v0.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/matchlines_v1.py` & `partitura-1.3.0/partitura/io/matchlines_v1.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/io/musescore.py` & `partitura-1.3.0/partitura/io/musescore.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/musicanalysis/__init__.py` & `partitura-1.3.0/partitura/musicanalysis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     make_note_feats,
     compute_note_array,
     full_note_array,
     make_rest_feats,
     make_rest_features,
 )
 from .performance_codec import encode_performance, decode_performance
+from .performance_features import make_performance_features
+from .note_array_to_score import note_array_to_score
 
 
 __all__ = [
     "estimate_voices",
     "estimate_key",
     "estimate_spelling",
     "estimate_tonaltension",
@@ -32,8 +34,10 @@
     "list_note_feats_functions",
     "make_note_features",
     "make_rest_features",
     "encode_performance",
     "decode_performance",
     "compute_note_array",
     "full_note_array",
+    "make_performance_features",
+    "note_array_to_score"
 ]
```

### Comparing `partitura-1.2.2/partitura/musicanalysis/key_identification.py` & `partitura-1.3.0/partitura/musicanalysis/key_identification.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/musicanalysis/meter.py` & `partitura-1.3.0/partitura/musicanalysis/meter.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/musicanalysis/note_features.py` & `partitura-1.3.0/partitura/musicanalysis/note_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 import numpy as np
 from scipy.interpolate import interp1d
 import partitura.score as score
 
 import types
 from typing import List, Union, Tuple
 from partitura.utils import ensure_notearray, ensure_rest_array
+from partitura.score import ScoreLike
 
 __all__ = [
     "list_note_feats_functions",
+    "list_note_feature_functions",
+    "print_note_feats_functions",
+    "print_note_feature_functions",
+    "make_note_feats", 
     "make_note_features",
-    "make_note_feats",
-    "full_note_array",
-    "compute_note_array",
-    "full_note_array",
     "make_rest_feats",
     "make_rest_features",
+    "compute_note_array",
+    "full_note_array",
 ]
 
 
 class InvalidNoteFeatureException(Exception):
     pass
 
 
@@ -45,15 +48,15 @@
             )
 
 
 def list_note_feats_functions():
     """Return a list of all feature function names defined in this module.
 
     The feature function names listed here can be specified by name in
-    the `make_feature` function. For example:
+    the `make_note_features` and `make_rest_features` functions. For example:
 
     >>> feature, names = make_note_feats(part, ['metrical_feature', 'articulation_feature'])
 
     Returns
     -------
     list
         A list of strings
@@ -68,43 +71,53 @@
         member = getattr(sys.modules[__name__], name)
         if isinstance(member, types.FunctionType) and name.endswith("_feature"):
             bfs.append(name)
     return bfs
 
 
 def make_note_features(
-    part: Union[score.Part, score.PartGroup, List],
+    part: ScoreLike,
     feature_functions: Union[List, str],
     add_idx: bool = False,
+    include_empty_features: bool = True,
+    force_fixed_size: bool = False,
 ) -> Tuple[np.ndarray, List]:
 
     """Compute the specified feature functions for a part.
 
     The function returns the computed feature functions as a N x M
     array, where N equals `len(part.notes_tied)` and M equals the
     total number of descriptors of all feature functions that occur in
     part.
 
-    Furthermore the function returns the names of the feature functions.
+    Furthermore, the function returns the names of the feature functions.
     A list of strings of size M. The names have the name of the
     function prepended to the name of the descriptor. For example if a
     function named `abc_feature` returns descriptors `a`, `b`, and `c`,
     then the list of names returned by `make_feature(part,
     ['abc_feature'])` will be ['abc_feature.a', 'abc_feature.b',
     'abc_feature.c'].
 
     Parameters
     ----------
-    part : Part
-        The score as a Part instance
+    part : ScoreLike
+        A partitura scoreLike object, can be Score, Part, or PartGroup.
     feature_functions : list or str
         A list of feature functions. Elements of the list can be either
         the functions themselves or the names of a feature function as
         strings (or a mix), or the keywork "all". The feature functions specified by name are
         looked up in the `featuremixer.featurefunctions` module.
+    add_idx : bool (default: False)
+        If True, the index of the note in the part is added as a
+        feature. This is useful for debugging.
+    include_empty_features : bool (default: True)
+        If True, features that are empty are included in the output.
+        Otherwise, they are omitted.
+    force_fixed_size : bool (default: False)
+        If True, the output array uses only features that have a fixed size with no new entries added.
 
     Returns
     -------
     feature : ndarray
         The feature functions
     names : list
         The feature names
@@ -131,17 +144,19 @@
 
     for bf in feature_functions:
         if isinstance(bf, str):
             # get function by name from module
             func = getattr(sys.modules[__name__], bf)
         elif isinstance(bf, types.FunctionType):
             func = bf
+        elif force_fixed_size and bf == "time_signature_feature":
+            continue
         else:
             warnings.warn("Ignoring unknown feature function {}".format(bf))
-        bf, bn = func(na, part)
+        bf, bn = func(na, part, include_empty_features=(True if force_fixed_size else include_empty_features))
         # check if the size and number of the feature function are correct
         if bf.size != 0:
             if bf.shape[1] != len(bn):
                 msg = (
                     "number of feature names {} does not equal "
                     "number of feature {}".format(len(bn), bf.shape[1])
                 )
@@ -296,18 +311,20 @@
         feature_names = [n for ns in _names for n in ns]
         return feature_data, feature_names
 
 
 # alias
 make_note_feats = make_note_features
 make_rest_feats = make_rest_features
+list_note_feature_functions = list_note_feats_functions
+print_note_feature_functions = print_note_feats_functions
 
 
 def compute_note_array(
-    part,
+    part : ScoreLike,
     include_pitch_spelling=False,
     include_key_signature=False,
     include_time_signature=False,
     include_metrical_position=False,
     include_grace_notes=False,
     feature_functions=None,
 ):
@@ -377,14 +394,18 @@
         include_grace_notes=include_grace_notes,
     )
 
     if feature_functions is not None:
         feature_data_struct = make_note_feats(part, feature_functions, add_idx=True)
         note_array_joined = np.lib.recfunctions.join_by("id", na, feature_data_struct)
         note_array = note_array_joined.data
+        sort_idx = np.lexsort((note_array["duration_div"], 
+                               note_array["pitch"], 
+                               note_array["onset_div"]))
+        note_array = note_array[sort_idx]
     else:
         note_array = na
     return note_array
 
 
 def full_note_array(part):
     """
@@ -397,24 +418,24 @@
         include_time_signature=True,
         include_metrical_position=True,
         include_grace_notes=True,
         feature_functions="all",
     )
 
 
-def polynomial_pitch_feature(na, part):
+def polynomial_pitch_feature(na, part, **kwargs):
     """Normalize pitch feature."""
     pitches = na["pitch"].astype(float)
     feature_names = ["pitch"]
     max_pitch = 127
     W = pitches / max_pitch
     return np.expand_dims(W, axis=1), feature_names
 
 
-def duration_feature(na, part):
+def duration_feature(na, part, **kwargs):
     """Duration feature.
 
     Parameters
     ----------
     na : structured array
         The Note array for Unified part.
     """
@@ -422,15 +443,15 @@
     feature_names = ["duration"]
     durations_beat = na["duration_beat"]
     W = durations_beat
     W.shape = (-1, 1)
     return W, feature_names
 
 
-def onset_feature(na, part):
+def onset_feature(na, part, **kwargs):
     """Onset feature
 
     Returns:
     * onset : the onset of the note in beats
     * score_position : position of the note in the score between 0 (the beginning of the piece) and 1 (the end of the piece)
 
     TODO:
@@ -442,20 +463,20 @@
     rel_position = normalize(onsets_beat, method="minmax")
 
     W = np.column_stack((onsets_beat, rel_position))
 
     return W, feature_names
 
 
-def relative_score_position_feature(na, part):
-    W, names = onset_feature(na, part)
+def relative_score_position_feature(na, part, **kwargs):
+    W, names = onset_feature(na, part, **kwargs)
     return W[:, 1:], names[1:]
 
 
-def grace_feature(na, part):
+def grace_feature(na, part, **kwargs):
     """Grace feature.
 
     Returns:
     * grace_note : 1 when the note is a grace note, 0 otherwise
     * n_grace : the length of the grace note sequence to which
                 this note belongs (0 for non-grace notes)
     * grace_pos : the (1-based) position of the grace note in
@@ -474,19 +495,19 @@
         else {n.id: n for n in part.rests}
     )
     indices = np.nonzero(na["is_grace"])[0]
     for i, index in enumerate(indices):
         grace = grace_notes[i]
         n_grace = np.count_nonzero(grace_notes["onset_beat"] == grace["onset_beat"])
         W[index, 1] = n_grace
-        W[index, 2] = n_grace - sum(1 for _ in notes[grace["id"]].iter_grace_seq()) + 1
+        W[index, 2] = n_grace - sum(1 for _ in notes[grace["id"]].iter_grace_seq()) + 1 if grace["id"] not in (None, 'None', "") else 0
     return W, feature_names
 
 
-def loudness_direction_feature(na, part):
+def loudness_direction_feature(na, part, **kwargs):
     """The loudness directions in part.
 
     This function returns a varying number of descriptors, depending
     on which directions are present. Some directions are grouped
     together. For example 'decrescendo' and 'diminuendo' are encoded
     together in a descriptor 'loudness_decr'. The descriptor names of
     textual directions such as 'adagio' are the verbatim directions.
@@ -498,116 +519,203 @@
     * loudness_incr : crescendo direction
     * loudness_decr : decrescendo or diminuendo direction
 
     """
 
     onsets = na["onset_div"]
     N = len(onsets)
+    constant = ["ppp", "pp", "p", "mp", "mf", "f", "ff", "fff", "unknown_constant"]
+    impulsive = ["fp", "sf", "sfp", "sfz", "unknown_impulsive"]
+    names = constant + impulsive + ["loudness_incr", "loudness_decr"]
 
     directions = list(part.iter_all(score.LoudnessDirection, include_subclasses=True))
+    if "include_empty_features" in kwargs.keys():
+        force_size = kwargs["include_empty_features"]
+    else:
+        force_size = False
+    if force_size:
+        def to_name(d):
+            if isinstance(d, score.ConstantLoudnessDirection):
+                if d.text in constant:
+                    return d.text
+                else:
+                    return "unknown_constant"
+            elif isinstance(d, score.ImpulsiveLoudnessDirection):
+                if d.text in impulsive:
+                    return d.text
+                else:
+                    return "unknown_impulsive"
+            elif isinstance(d, score.IncreasingLoudnessDirection):
+                return "loudness_incr"
+            elif isinstance(d, score.DecreasingLoudnessDirection):
+                return "loudness_decr"
+    else:
+        def to_name(d):
+            if isinstance(d, score.ConstantLoudnessDirection):
+                return d.text
+            elif isinstance(d, score.ImpulsiveLoudnessDirection):
+                return d.text
+            elif isinstance(d, score.IncreasingLoudnessDirection):
+                return "loudness_incr"
+            elif isinstance(d, score.DecreasingLoudnessDirection):
+                return "loudness_decr"
 
-    def to_name(d):
-        if isinstance(d, score.ConstantLoudnessDirection):
-            return d.text
-        elif isinstance(d, score.ImpulsiveLoudnessDirection):
-            return d.text
-        elif isinstance(d, score.IncreasingLoudnessDirection):
-            return "loudness_incr"
-        elif isinstance(d, score.DecreasingLoudnessDirection):
-            return "loudness_decr"
 
     feature_by_name = {}
     for d in directions:
         j, bf = feature_by_name.setdefault(
             to_name(d), (len(feature_by_name), np.zeros(N))
         )
         bf += feature_function_activation(d)(onsets)
 
-    W = np.empty((len(onsets), len(feature_by_name)))
-    names = [None] * len(feature_by_name)
+    if not force_size:
+        M = len(feature_by_name) if len(feature_by_name) > 0 else 1
+        names = [None] * M
+    W = np.zeros((len(onsets), len(names)))
     for name, (j, bf) in feature_by_name.items():
+        if force_size:
+            j = names.index(name)
+        else:
+            names[j] = name
         W[:, j] = bf
-        names[j] = name
 
     return W, names
 
 
-def tempo_direction_feature(na, part):
+def tempo_direction_feature(na, part, **kwargs):
     """The tempo directions in part.
 
     This function returns a varying number of descriptors, depending
     on which directions are present. Some directions are grouped
     together. For example 'adagio' and 'molto adagio' are encoded
     together in a descriptor 'adagio'.
 
     Some possible descriptors:
     * adagio : directions like 'adagio', 'molto adagio'
 
     """
     onsets = na["onset_div"]
     N = len(onsets)
-
+    constant = ["adagio", "largo", "lento", "grave", "larghetto", "adagietto", "andante",
+                "andantino", "moderato", "allegretto", "allegro", "vivace", "presto", "prestissimo",
+                "unknown_constant"]
+    names = constant + ["tempo_incr", "tempo_decr"]
     directions = list(part.iter_all(score.TempoDirection, include_subclasses=True))
 
-    def to_name(d):
-        if isinstance(d, score.ResetTempoDirection):
-            ref = d.reference_tempo
-            if ref:
-                return ref.text
-            else:
+
+    if "include_empty_features" in kwargs.keys():
+        force_size = kwargs["include_empty_features"]
+    else:
+        force_size = False
+    if force_size:
+        def to_name(d):
+            if isinstance(d, score.ResetTempoDirection):
+                ref = d.reference_tempo
+                if ref:
+                    if ref.text in constant:
+                        return ref.text
+                    else:
+                        return "unknown_constant"
+                else:
+                    if d.text in constant:
+                        return d.text
+                    else:
+                        return "unknown_constant"
+            elif isinstance(d, score.ConstantTempoDirection):
+                if d.text in constant:
+                    return d.text
+                else:
+                    return "unknown_constant"
+            elif isinstance(d, score.IncreasingTempoDirection):
+                return "tempo_incr"
+            elif isinstance(d, score.DecreasingTempoDirection):
+                return "tempo_decr"
+    else:
+        def to_name(d):
+            if isinstance(d, score.ResetTempoDirection):
+                ref = d.reference_tempo
+                if ref:
+                    return ref.text
+                else:
+                    return d.text
+            elif isinstance(d, score.ConstantTempoDirection):
                 return d.text
-        elif isinstance(d, score.ConstantTempoDirection):
-            return d.text
-        elif isinstance(d, score.IncreasingTempoDirection):
-            return "tempo_incr"
-        elif isinstance(d, score.DecreasingTempoDirection):
-            return "tempo_decr"
+            elif isinstance(d, score.IncreasingTempoDirection):
+                return "tempo_incr"
+            elif isinstance(d, score.DecreasingTempoDirection):
+                return "tempo_decr"
 
     feature_by_name = {}
     for d in directions:
         j, bf = feature_by_name.setdefault(
             to_name(d), (len(feature_by_name), np.zeros(N))
         )
         bf += feature_function_activation(d)(onsets)
 
-    W = np.empty((len(onsets), len(feature_by_name)))
-    names = [None] * len(feature_by_name)
+
+    if not force_size:
+        M = len(feature_by_name) if len(feature_by_name) > 0 else 1
+        names = [None] * M
+    W = np.zeros((len(onsets), len(names)))
     for name, (j, bf) in feature_by_name.items():
+        if force_size:
+            j = names.index(name)
+        else:
+            names[j] = name
         W[:, j] = bf
-        names[j] = name
 
     return W, names
 
 
-def articulation_direction_feature(na, part):
+def articulation_direction_feature(na, part, **kwargs):
     """ """
     onsets = na["onset_div"]
     N = len(onsets)
 
     directions = list(
         part.iter_all(score.ArticulationDirection, include_subclasses=True)
     )
+    constant_names = ["staccato", "tenuto", "accent", "marcato", "unknown_articulation"]
 
-    def to_name(d):
-        return d.text
+    if "include_empty_features" in kwargs.keys():
+        force_size = kwargs["include_empty_features"]
+    else:
+        force_size = False
+    if force_size:
+        def to_name(d):
+            if d.text in constant_names:
+                return d.text
+            else:
+                return "unknown_direction"
+    else:
+        def to_name(d):
+            return d.text
 
     feature_by_name = {}
 
     for d in directions:
         j, bf = feature_by_name.setdefault(
             to_name(d), (len(feature_by_name), np.zeros(N))
         )
         bf += feature_function_activation(d)(onsets)
 
-    W = np.empty((len(onsets), len(feature_by_name)))
-    names = [None] * len(feature_by_name)
+    if force_size:
+        W = np.zeros((len(onsets), len(constant_names)))
+        names = constant_names
+    else:
+        M = len(feature_by_name) if len(feature_by_name) > 0 else 1
+        W = np.zeros((len(onsets), M))
+        names = [None] * M
 
     for name, (j, bf) in feature_by_name.items():
+        if force_size:
+            j = names.index(name)
+        else:
+            names[j] = name
         W[:, j] = bf
-        names[j] = name
 
     return W, names
 
 
 def feature_function_activation(direction):
     epsilon = 1e-6
 
@@ -679,15 +787,15 @@
             direction.start.t + epsilon,
         ]
         y = [0, 1, 0]
 
     return interp1d(x, y, bounds_error=False, fill_value=0)
 
 
-def slur_feature(na, part):
+def slur_feature(na, part, **kwargs):
     """Slur feature.
 
     Returns:
     * slur_incr : a ramp function that increases from 0
                   to 1 over the course of the slur
     * slur_decr : a ramp function that decreases from 1
                   to 0 over the course of the slur
@@ -707,15 +815,15 @@
         W[:, 0] += interp1d(x, y_inc, bounds_error=False, fill_value=0)(onsets)
         W[:, 1] += interp1d(x, y_dec, bounds_error=False, fill_value=0)(onsets)
     # Filter out NaN values
     W[np.isnan(W)] = 0.0
     return W, names
 
 
-def articulation_feature(na, part):
+def articulation_feature(na, part, **kwargs):
     """Articulation feature.
 
     This feature returns articulation-related note annotations, such as accents, legato, and tenuto.
 
     Possible descriptors:
     * accent : 1 when the note has an annotated accent sign
     * legato : 1 when the note has an annotated legato sign
@@ -737,38 +845,49 @@
         "falloff",
         "breath-mark",
         "caesura",
         "stress",
         "unstress",
         "soft-accent",
     ]
+    if "include_empty_features" in kwargs:
+        force_size = kwargs["include_empty_features"]
+    else:
+        force_size = False
+
     feature_by_name = {}
     notes = part.notes_tied if not np.all(na["pitch"] == 0) else part.rests
     N = len(notes)
     for i, n in enumerate(notes):
         if n.articulations:
             for art in n.articulations:
                 if art in names:
                     j, bf = feature_by_name.setdefault(
                         art, (len(feature_by_name), np.zeros(N))
                     )
                     bf[i] = 1
 
-    M = len(feature_by_name)
-    W = np.empty((N, M))
-    names = [None] * M
+    if force_size:
+        M = len(names)
+    else:
+        M = len(feature_by_name) if len(feature_by_name) > 0 else 1
+        names = [None] * M
+    W = np.zeros((N, M))
 
     for name, (j, bf) in feature_by_name.items():
+        if force_size:
+            j = names.index(name)
+        else:
+            names[j] = name
         W[:, j] = bf
-        names[j] = name
 
     return W, names
 
 
-def ornament_feature(na, part):
+def ornament_feature(na, part, **kwargs):
     """Ornament feature.
 
     This feature returns ornamentation note annotations,such as trills.
 
     Possible descriptors:
     * trill : 1 when the note has an annotated trill
     * mordent : 1 when the note has an annotated mordent
@@ -799,64 +918,73 @@
         if n.ornaments:
             for art in n.ornaments:
                 if art in names:
                     j, bf = feature_by_name.setdefault(
                         art, (len(feature_by_name), np.zeros(N))
                     )
                     bf[i] = 1
+    if "include_empty_features" in kwargs.keys():
+        fix_size = kwargs["include_empty_features"]
+    else:
+        fix_size = False
+    if fix_size:
+        M = len(names)
+    else:
+        M = len(feature_by_name) if len(feature_by_name) > 0 else 1
+        names = [None] * M
+    W = np.zeros((N, M))
 
-    M = len(feature_by_name)
-    W = np.empty((N, M))
-    names = [None] * M
 
     for name, (j, bf) in feature_by_name.items():
+        if fix_size:
+            j = names.index(name)
+        else:
+            names[j] = name
         W[:, j] = bf
-        names[j] = name
 
     return W, names
 
 
-def staff_feature(na, part):
+def staff_feature(na, part, **kwargs):
     """Staff feature"""
     names = ["staff"]
     notes = {n.id: n.staff for n in part.notes_tied}
-    N = len(notes)
-    W = np.empty((N, 1))
+    N = len(na)
+    W = np.zeros((N, 1))
     for i, n in enumerate(na):
-        W[i, 0] = notes[n["id"]]
-
+        W[i, 0] = notes[n["id"]] if n["id"] not in (None, "None", "") else 0
     return W, names
 
 
 # # for a subset of the articulations do e.g.
 # def staccato_feature(part):
 #     W, names = articulation_feature(part)
 #     if 'staccato' in names:
 #         i = names.index('staccato')
 #         return W[:, i:i + 1], ['staccato']
 #     else:
 #         return np.empty(len(W)), []
 
 
-def fermata_feature(na, part):
+def fermata_feature(na, part, **kwargs):
     """Fermata feature.
 
     Returns:
     * fermata : 1 when the note coincides with a fermata sign.
 
     """
     names = ["fermata"]
     onsets = na["onset_div"]
     W = np.zeros((len(onsets), 1))
     for ferm in part.iter_all(score.Fermata):
         W[onsets == ferm.start.t, 0] = 1
     return W, names
 
 
-def metrical_feature(na, part):
+def metrical_feature(na, part, **kwargs):
     """Metrical feature
 
     This feature encodes the metrical position in the bar. For example
     the first beat in a 3/4 meter is encoded in a binary descriptor
     'metrical_3_4_0', the fifth beat in a 6/8 meter as
     'metrical_6_8_4', etc. Any positions that do not fall on a beat
     are encoded in a feature suffixed '_weak'. For example a note
@@ -888,24 +1016,24 @@
             name = "metrical_{}_{}_weak".format(beats, beat_type)
 
         j, bf = feature_by_name.setdefault(
             name, (len(feature_by_name), np.zeros(len(notes)))
         )
         bf[i] = 1
 
-    W = np.empty((len(notes), len(feature_by_name)))
+    W = np.zeros((len(notes), len(feature_by_name)))
     names = [None] * len(feature_by_name)
     for name, (j, bf) in feature_by_name.items():
         W[:, j] = bf
         names[j] = name
 
     return W, names
 
 
-def metrical_strength_feature(na, part):
+def metrical_strength_feature(na, part, **kwargs):
     """Metrical strength feature
 
     This feature encodes the beat phase (relative position of a note within
     the measure), as well as metrical strength of common time signatures.
     """
     names = [
         "beat_phase",
@@ -916,19 +1044,20 @@
 
     relod = na["rel_onset_div"].astype(float)
     totmd = na["tot_measure_div"].astype(float)
     W = np.zeros((len(na), len(names)))
     W[:, 0] = np.divide(relod, totmd)  # Onset Phase
     W[:, 1] = na["is_downbeat"].astype(float)
     W[:, 2][W[:, 0] == 0.5] = 1.00
-    W[:, 3][np.nonzero(np.add(W[:, 1], W[:, 0]) == 1.00)]
+    W[:, 3][np.nonzero(np.add(W[:, 1], W[:, 0]) == 1.00)] = 1.00
+
     return W, names
 
 
-def time_signature_feature(na, part):
+def time_signature_feature(na, part, **kwargs):
     """TIme Signature feature
     This feature encodes the time signature of the note in two sets of one-hot vectors,
     a one hot encoding of number of beats and a one hot encoding of beat type
     """
 
     ts_map = part.time_signature_map
     possible_beats = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, "other"]
@@ -954,15 +1083,15 @@
             W_types[i, -1] = 1
 
     W = np.column_stack((W_beats, W_types))
 
     return W, names
 
 
-def vertical_neighbor_feature(na, part):
+def vertical_neighbor_feature(na, part, **kwargs):
     """Vertical neighbor feature.
 
     Describes various aspects of simultaneously starting notes.
 
     Returns:
     * n_total :
     * n_above :
@@ -977,15 +1106,15 @@
         "n_total",
         "n_above",
         "n_below",
         "highest_pitch",
         "lowest_pitch",
         "pitch_range",
     ]
-    W = np.empty((len(na), len(names)))
+    W = np.zeros((len(na), len(names)))
     for i, n in enumerate(na):
         neighbors = na[np.where(na["onset_beat"] == n["onset_beat"])]["pitch"]
         max_pitch = np.max(neighbors)
         min_pitch = np.min(neighbors)
         W[i, 0] = len(neighbors) - 1
         W[i, 1] = np.sum(neighbors > n["pitch"])
         W[i, 2] = np.sum(neighbors < n["pitch"])
```

### Comparing `partitura-1.2.2/partitura/musicanalysis/performance_codec.py` & `partitura-1.3.0/partitura/musicanalysis/performance_codec.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,46 +3,39 @@
 """
 This module implements a codec to encode and decode expressive performances to a set of
 expressive parameters.
 """
 from typing import Union, Callable
 import numpy as np
 import numpy.lib.recfunctions as rfn
-
-try:
-    import torch
-except ImportError:
-    # Dummy module to avoid ImportErrors
-    class DummyTorch(object):
-        Tensor = np.ndarray
-
-        def __init__(self):
-            pass
-
-    torch = DummyTorch()
+import warnings
 
 
 from partitura.score import Part, ScoreLike
 from partitura.performance import PerformedPart, PerformanceLike
 from partitura.musicanalysis import note_features
 from partitura.utils.misc import deprecated_alias
-from partitura.utils.generic import interp1d
+from partitura.utils.generic import interp1d, monotonize_times
+from partitura.utils.music import ensure_notearray
 from scipy.misc import derivative
 
 __all__ = ["encode_performance", "decode_performance", "to_matched_score"]
 
 
+#### Full Codecs ####
+
+
 @deprecated_alias(part='score', ppart="performance")
 def encode_performance(
     score: ScoreLike,
     performance: PerformanceLike,
     alignment: list,
     return_u_onset_idx=False,
     beat_normalization: str = "beat_period",  # "beat_period_log", "beat_period_ratio", "beat_period_ratio_log", "beat_period_standardized"
-    tempo_smooth: Union[str, Callable] = "average" 
+    tempo_smooth: Union[str, Callable] = "average"
 ):
     """
     Encode expressive parameters from a matched performance
 
 
     Parameters
     ----------
@@ -51,26 +44,26 @@
     performance : partitura.performance.PerformanceLike
         Performance information, can be a ppart, performance
     alignment : list
         The score--performance alignment, a list of dictionaries
     return_u_onset_idx : bool
         Return the indices of the unique score onsets
     beat_normalization : str (Optional)
-        Return extra columns for normalization parameters. 
+        Return extra columns for normalization parameters.
     tempo_smooth : str (Optional)
-        How the tempo curve is computed. average or derivative. 
-        Can also input a callable function for user-defined tempo curve. 
+        How the tempo curve is computed. average or derivative.
+        Can also input a callable function for user-defined tempo curve.
 
     Returns
     -------
     parameters : structured array
         A performance array with 4 fields: beat_period, velocity,
         timing, and articulation_log.
         If beat_normalization is defined as any method other than beat_period,
-        return the normalization value as extra columns in parameters. 
+        return the normalization value as extra columns in parameters.
     snote_ids : dict
         A dict of snote_ids corresponding to performance notes.
     unique_onset_idxs : list (optional)
         List of unique onset ids. Returned only when return_u_onset_idx
         is set to True.
     """
 
@@ -199,18 +192,19 @@
             )
 
         return ppart, alignment
     else:
 
         return ppart
 
+#### Time and Articulation Codecs ####
 
-def decode_time(score_onsets, 
-                score_durations, 
-                parameters, 
+def decode_time(score_onsets,
+                score_durations,
+                parameters,
                 normalization = "beat_period",
                 *args, **kwargs):
     """
     Decode a performance into onsets and durations in seconds
     for each note in the score.
     """
     score_onsets = score_onsets.astype(float, copy=False)
@@ -221,16 +215,16 @@
         offsets=score_onsets + score_durations,
         unique_onset_idxs=None,
         return_diff=True,
     )
     unique_onset_idxs = score_info["unique_onset_idxs"]
     diff_u_onset_score = score_info["diff_u_onset"]
 
-    # reconstruct the time by the extra parameters, for testing the inversion. 
-    # In practice, always reconstruct the time by beat_period. 
+    # reconstruct the time by the extra parameters, for testing the inversion.
+    # In practice, always reconstruct the time by beat_period.
     if normalization != "beat_period":
         tempo_param_names = list(TEMPO_NORMALIZATION[normalization]['param_names'])
         time_param = np.array(
             [tuple(np.mean(rfn.structured_to_unstructured(parameters[tempo_param_names][uix]), axis=0),) for uix in unique_onset_idxs],
             dtype=[(tp, "f4") for tp in tempo_param_names]
         )
         beat_period = TEMPO_NORMALIZATION[normalization]['rescale'](time_param)
@@ -259,14 +253,37 @@
         )
 
     performance[:, 0] -= np.min(performance[:, 0])
 
     return performance
 
 
+def encode_articulation(
+    score_durations, performed_durations, unique_onset_idxs, beat_period
+):
+    """
+    Encode articulation
+    """
+    articulation = np.zeros_like(score_durations)
+    for idx, bp in zip(unique_onset_idxs, beat_period):
+
+        sd = score_durations[idx]
+        pd = performed_durations[idx]
+
+        # indices of notes with duration 0 (grace notes)
+        grace_mask = sd <= 0
+
+        # Grace notes have an articulation ratio of 1
+        sd[grace_mask] = 1
+        pd[grace_mask] = bp
+        articulation[idx] = np.log2(pd / (bp * sd))
+
+    return articulation
+
+
 def decode_articulation(score_durations, articulation_parameter, beat_period):
     """
     Decode articulation
     """
     art_ratio = 2**articulation_parameter
     dur = art_ratio * score_durations * beat_period
 
@@ -302,22 +319,22 @@
         beat_period, s_onsets, unique_onset_idxs = tempo_smooth(
             score_onsets=score[:, 0],
             performed_onsets=performance[:, 0],
             score_durations=score[:, 1],
             performed_durations=performance[:, 1],
             return_onset_idxs=True,
         )
-    elif tempo_smooth == "average": 
+    elif tempo_smooth == "average":
         beat_period, s_onsets, unique_onset_idxs = tempo_by_average(
             score_onsets=score[:, 0],
             performed_onsets=performance[:, 0],
             score_durations=score[:, 1],
             performed_durations=performance[:, 1],
             return_onset_idxs=True,
-        )   
+        )
     elif tempo_smooth == "derivative":
         beat_period, s_onsets, unique_onset_idxs = tempo_by_derivative(
             score_onsets=score[:, 0],
             performed_onsets=performance[:, 0],
             score_durations=score[:, 1],
             performed_durations=performance[:, 1],
             return_onset_idxs=True,
@@ -434,15 +451,15 @@
     # unique score onsets
     unique_s_onsets = score_info["u_onset"]
     # equivalent onsets
     eq_onsets = perf_info["u_onset"]
 
     # Monotonize times
     eq_onset_mt, unique_s_onsets_mt = monotonize_times(
-        eq_onsets, deltas=unique_s_onsets
+        eq_onsets, x=unique_s_onsets
     )
 
     # Estimate Beat Period
     perf_iois = np.diff(eq_onset_mt)
     s_iois = np.diff(unique_s_onsets_mt)
     beat_period = perf_iois / s_iois
 
@@ -455,14 +472,15 @@
     )
 
     if input_onsets is None:
         input_onsets = unique_s_onsets[:-1]
 
     tempo_curve = tempo_fun(input_onsets)
 
+    assert((tempo_curve >= 0).all())
     if return_onset_idxs:
         return tempo_curve, input_onsets, unique_onset_idxs
     else:
         return tempo_curve, input_onsets
 
 
 def tempo_by_derivative(score_onsets, performed_onsets,
@@ -537,15 +555,15 @@
     # unique score onsets
     unique_s_onsets = score_info['u_onset']
     # equivalent onsets
     eq_onsets = perf_info['u_onset']
 
     # Monotonize times
     eq_onset_mt, unique_s_onsets_mt = monotonize_times(eq_onsets,
-                                                       deltas=unique_s_onsets)
+                                                       x=unique_s_onsets)
     # Function that that interpolates the equivalent performed onsets
     # as a function of the score onset.
     onset_fun = interp1d(unique_s_onsets_mt, eq_onset_mt, kind='linear',
                          fill_value='extrapolate')
 
     if input_onsets is None:
         input_onsets = unique_s_onsets[:-1]
@@ -554,255 +572,340 @@
 
     if return_onset_idxs:
         return tempo_curve, input_onsets, unique_onset_idxs
     else:
         return tempo_curve, input_onsets
 
 
-def get_unique_seq(onsets, offsets, unique_onset_idxs=None, return_diff=False):
-    """
-    Get unique onsets of a sequence of notes
-    """
-    eps = np.finfo(float).eps
-
-    first_time = np.min(onsets)
-
-    # ensure last score time is later than last onset
-    last_time = max(np.max(onsets) + eps, np.max(offsets))
-
-    total_dur = last_time - first_time
-
-    if unique_onset_idxs is None:
-        # unique_onset_idxs = unique_onset_idx(score[:, 0])
-        unique_onset_idxs = get_unique_onset_idxs(onsets)
-
-    u_onset = np.array([np.mean(onsets[uix]) for uix in unique_onset_idxs])
-    # add last offset, so we have as many IOIs as notes
-    u_onset = np.r_[u_onset, last_time]
-
-    output_dict = dict(
-        u_onset=u_onset, total_dur=total_dur, unique_onset_idxs=unique_onset_idxs
-    )
-
-    if return_diff:
-        output_dict["diff_u_onset"] = np.diff(u_onset)
-
-    return output_dict
+#### Alignment Processing ####
 
 
-def get_unique_onset_idxs(
-    onsets, eps: float = 1e-6, return_unique_onsets: bool = False
-):
-    """
-    Get unique onsets and their indices.
-    Parameters
-    ----------
-    onsets : np.ndarray
-        Score onsets in beats.
-    eps : float
-        Small epsilon (for dealing with quantization in symbolic scores).
-        This is particularly useful for dealing with triplets and other
-        similar rhytmical structures that do not have a finite decimal
-        representation.
-    return_unique_onsets : bool (optional)
-        If `True`, returns the unique score onsets.
-    Returns
-    -------
-    unique_onset_idxs : np.ndarray
-        Indices of the unique onsets in the score.
-    unique_onsets : np.ndarray
-        Unique score onsets
-    """
-    # Do not assume that the onsets are sorted
-    # (use a stable sorting algorithm for preserving the order
-    # of elements with the same onset, which is useful e.g. if the
-    # notes within a same onset are ordered by pitch)
-    sort_idx = np.argsort(onsets, kind="mergesort")
-    split_idx = np.where(np.diff(onsets[sort_idx]) > eps)[0] + 1
-    unique_onset_idxs = np.split(sort_idx, split_idx)
-
-    if return_unique_onsets:
-        # Instead of np.unique(onsets)
-        unique_onsets = np.array([onsets[uix].mean() for uix in unique_onset_idxs])
-
-        return unique_onset_idxs, unique_onsets
-    else:
-        return unique_onset_idxs
-
 @deprecated_alias(part='score', ppart="performance")
-def to_matched_score(score: ScoreLike, 
-                     performance: PerformanceLike, 
+def to_matched_score(score: ScoreLike,
+                     performance: PerformanceLike,
                      alignment: list,
                      include_score_markings=False):
     """
     Returns a mixed score-performance note array
     consisting of matched notes in the alignment.
 
     Args:
         score (score.ScoreLike): score information
         performance (performance.PerformanceLike): performance information
         alignment (List(Dict)): an alignment
-        include_score_markings (bool): include dynamcis and articulation 
+        include_score_markings (bool): include dynamcis and articulation
             markings (Optional)
 
     Returns:
         np.ndarray: a minimal, aligned
         score-performance note array
     """
 
     # remove repetitions from aligment note ids
     for a in alignment:
         if a["label"] == "match":
             a["score_id"] = str(a["score_id"])
 
     feature_functions = None
     if include_score_markings:
-        feature_functions = ["loudness_direction_feature", "articulation_feature", 
+        feature_functions = ["loudness_direction_feature", "articulation_feature",
                              "tempo_direction_feature", "slur_feature"]
-        
+
     na = note_features.compute_note_array(score, feature_functions=feature_functions)
     p_na = performance.note_array()
     part_by_id = dict((n['id'], na[na['id'] == n['id']]) for n in na)
     ppart_by_id = dict((n['id'], p_na[p_na['id'] == n['id']]) for n in p_na)
 
     # pair matched score and performance notes
     note_pairs = [
         (part_by_id[a["score_id"]], ppart_by_id[a["performance_id"]])
         for a in alignment
         if (a["label"] == "match" and a["score_id"] in part_by_id)
     ]
-
     ms = []
     # sort according to onset (primary) and pitch (secondary)
     pitch_onset = [(sn['pitch'].item(), sn['onset_div'].item()) for sn, _ in note_pairs]
     sort_order = np.lexsort(list(zip(*pitch_onset)))
     snote_ids = []
     for i in sort_order:
         sn, n = note_pairs[int(i)]
         sn_on, sn_off = [sn['onset_beat'], sn['onset_beat'] + sn['duration_beat']]
         sn_dur = sn_off - sn_on
         # hack for notes with negative durations
         n_dur = max(n["duration_sec"], 60 / 200 * 0.25)
         pair_info = (sn_on, sn_dur, sn['pitch'], n["onset_sec"], n_dur, n["velocity"])
         if include_score_markings:
+            pair_info += (sn['voice'].item(), )
             pair_info += tuple([sn[field].item() for field in sn.dtype.names if "feature" in field])
         ms.append(pair_info)
         snote_ids.append(sn['id'].item())
 
     fields = [
         ("onset", "f4"),
         ("duration", "f4"),
         ("pitch", "i4"),
         ("p_onset", "f4"),
         ("p_duration", "f4"),
         ("velocity", "i4"),
     ]
     if include_score_markings:
+        fields += [("voice", "i4")]
         fields += [(field, sn.dtype.fields[field][0]) for field in sn.dtype.fields if "feature" in field]
 
     return np.array(ms, dtype=fields), snote_ids
 
 
-def encode_articulation(
-    score_durations, performed_durations, unique_onset_idxs, beat_period
+def get_time_maps_from_alignment(
+    ppart_or_note_array, spart_or_note_array, alignment, remove_ornaments=True
 ):
     """
-    Encode articulation
-    """
-    articulation = np.zeros_like(score_durations)
-    for idx, bp in zip(unique_onset_idxs, beat_period):
+    Get time maps to convert performance time (in seconds) to score time (in beats)
+    and visceversa.
 
-        sd = score_durations[idx]
-        pd = performed_durations[idx]
+    Parameters
+    ----------
+    ppart_or_note_array : PerformedPart or structured array
+        The performance information as either PerformedPart or the
+        note_array generated from such an object.
+    spart_or_note_array : Part or structured array
+        Score information as either a Part object or the note array
+        generated from such an object.
+    alignment : list
+        The score--performance alignment, a list of dictionaries.
+        (see `partitura.io.importmatch.alignment_from_matchfile` for reference)
+    remove_ornaments : bool (optional)
+        Whether to consider or not ornaments (including grace notes)
 
-        # indices of notes with duration 0 (grace notes)
-        grace_mask = sd <= 0
+    Returns
+    -------
+    ptime_to_stime_map : scipy.interpolate.interp1d
+        An instance of interp1d (a callable) that maps performance time (in seconds)
+        to score time (in beats).
+    stime_to_ptime_map : scipy.interpolate.interp1d
+        An instance of inter1d (a callable) that maps score time (in beats) to
+        performance time (in seconds).
+
+    Note
+    ----
+    This methods uses the average value of the score onsets of notes that are
+    written in the score as part of a chord (i.e., which start at the same time).
+    """
+    # Ensure that we are using structured note arrays
+    perf_note_array = ensure_notearray(ppart_or_note_array)
+    score_note_array = ensure_notearray(spart_or_note_array)
+
+    # Get indices of the matched notes (notes in the score
+    # for which there is a performance note
+    match_idx = get_matched_notes(score_note_array, perf_note_array, alignment)
+
+    # Get onsets and durations
+    score_onsets = score_note_array[match_idx[:, 0]]["onset_beat"]
+    score_durations = score_note_array[match_idx[:, 0]]["duration_beat"]
+
+    perf_onsets = perf_note_array[match_idx[:, 1]]["onset_sec"]
+
+    # Use only unique onsets
+    score_unique_onsets = np.unique(score_onsets)
+
+    # Remove grace notes
+    if remove_ornaments:
+        # TODO: check that all onsets have a duration?
+        # ornaments (grace notes) do not have a duration
+        score_unique_onset_idxs = np.array(
+            [
+                np.where(np.logical_and(score_onsets == u, score_durations > 0))[0]
+                for u in score_unique_onsets
+            ],
+            dtype=object,
+        )
 
-        # Grace notes have an articulation ratio of 1
-        sd[grace_mask] = 1
-        pd[grace_mask] = bp
-        # Compute log articulation ratio
-        articulation[idx] = np.log2(pd / (bp * sd))
+    else:
+        score_unique_onset_idxs = np.array(
+            [np.where(score_onsets == u)[0] for u in score_unique_onsets],
+            dtype=object,
+        )
 
-    return articulation
+    # For chords, we use the average performed onset as a proxy for
+    # representing the "performeance time" of the position of the score
+    # onsets
+    eq_perf_onsets = np.array(
+        [np.mean(perf_onsets[u]) for u in score_unique_onset_idxs]
+    )
 
+    # Get maps
+    ptime_to_stime_map = interp1d(
+        x=eq_perf_onsets,
+        y=score_unique_onsets,
+        bounds_error=False,
+        fill_value="extrapolate",
+    )
+    stime_to_ptime_map = interp1d(
+        y=eq_perf_onsets,
+        x=score_unique_onsets,
+        bounds_error=False,
+        fill_value="extrapolate",
+    )
+
+    return ptime_to_stime_map, stime_to_ptime_map
+
+
+def get_matched_notes(spart_note_array, ppart_note_array, alignment):
+    """
+    Get the indices of the matched notes in an alignment
 
-def monotonize_times(s, deltas=None):
-    """Interpolate linearly over as many points in `s` as necessary to
-    obtain a monotonic sequence. The minimum and maximum of `s` are
-    prepended and appended, respectively, to ensure monotonicity at
-    the bounds of `s`.
     Parameters
     ----------
-    s : ndarray
-        a sequence of numbers
-    strict : bool
-        when True, return a strictly monotonic sequence (default: True)
-    deltas : 
+    spart_note_array : structured numpy array
+        note_array of the score part
+    ppart_note_array : structured numpy array
+        note_array of the performed part
+    alignment : list
+        The score--performance alignment, a list of dictionaries.
+        (see `partitura.io.importmatch.alignment_from_matchfile` for reference)
 
     Returns
     -------
-    ndarray
-       a monotonic sequence that has been linearly interpolated using a subset of s
+    matched_idxs : np.ndarray
+        A 2D array containing the indices of the matched score and
+        performed notes, where the columns are
+        (index_in_score_note_array, index_in_performance_notearray)
+    """
+    # Get matched notes
+    matched_idxs = []
+    for al in alignment:
+        # Get only matched notes (i.e., ignore inserted or deleted notes)
+        if al["label"] == "match":
+
+            # if ppart_note_array['id'].dtype != type(al['performance_id']):
+            if not isinstance(ppart_note_array["id"], type(al["performance_id"])):
+                p_id = str(al["performance_id"])
+            else:
+                p_id = al["performance_id"]
+
+            p_idx = int(np.where(ppart_note_array["id"] == p_id)[0])
+
+            s_idx = np.where(spart_note_array["id"] == al["score_id"])[0]
+
+            if len(s_idx) > 0:
+                s_idx = int(s_idx)
+                matched_idxs.append((s_idx, p_idx))
+
+    return np.array(matched_idxs)
+
+
+#### Sequence Processing: onset-wise/note-wise/monotonicity/uniqueness ####
+
+
+def get_unique_seq(onsets, offsets, unique_onset_idxs=None, return_diff=False):
+    """
+    Get unique onsets of a sequence of notes
     """
     eps = np.finfo(float).eps
 
-    _s = np.r_[np.min(s) - eps, s, np.max(s) + eps]
-    if deltas is not None:
-        _deltas = np.r_[np.min(deltas) - eps, deltas, np.max(deltas) + eps]
-    else:
-        _deltas = None
-    mask = np.ones(_s.shape[0], dtype=bool)
-    mask[0] = mask[-1] = False
-    idx = np.arange(_s.shape[0])
-    s_mono = interp1d(idx[mask], _s[mask])(idx[1:-1])
-    return _s[mask], _deltas[mask]
+    first_time = np.min(onsets)
+
+    # ensure last score time is later than last onset
+    last_time = max(np.max(onsets) + eps, np.max(offsets))
+
+    total_dur = last_time - first_time
+
+    if unique_onset_idxs is None:
+        # unique_onset_idxs = unique_onset_idx(score[:, 0])
+        unique_onset_idxs = get_unique_onset_idxs(onsets)
+
+    u_onset = np.array([np.mean(onsets[uix]) for uix in unique_onset_idxs])
+    # add last offset, so we have as many IOIs as notes
+    u_onset = np.r_[u_onset, last_time]
+
+    output_dict = dict(
+        u_onset=u_onset, total_dur=total_dur, unique_onset_idxs=unique_onset_idxs
+    )
+
+    if return_diff:
+        output_dict["diff_u_onset"] = np.diff(u_onset)
+
+    return output_dict
+
+
+def get_unique_onset_idxs(
+    onsets, eps: float = 1e-6, return_unique_onsets: bool = False
+):
+    """
+    Get unique onsets and their indices.
+    Parameters
+    ----------
+    onsets : np.ndarray
+        Score onsets in beats.
+    eps : float
+        Small epsilon (for dealing with quantization in symbolic scores).
+        This is particularly useful for dealing with triplets and other
+        similar rhytmical structures that do not have a finite decimal
+        representation.
+    return_unique_onsets : bool (optional)
+        If `True`, returns the unique score onsets.
+    Returns
+    -------
+    unique_onset_idxs : np.ndarray
+        Indices of the unique onsets in the score.
+    unique_onsets : np.ndarray
+        Unique score onsets
+    """
+    # Do not assume that the onsets are sorted
+    # (use a stable sorting algorithm for preserving the order
+    # of elements with the same onset, which is useful e.g. if the
+    # notes within a same onset are ordered by pitch)
+    sort_idx = np.argsort(onsets, kind="mergesort")
+    split_idx = np.where(np.diff(onsets[sort_idx]) > eps)[0] + 1
+    unique_onset_idxs = np.split(sort_idx, split_idx)
+
+    if return_unique_onsets:
+        # Instead of np.unique(onsets)
+        unique_onsets = np.array([onsets[uix].mean() for uix in unique_onset_idxs])
+
+        return unique_onset_idxs, unique_onsets
+    else:
+        return unique_onset_idxs
 
 
 def notewise_to_onsetwise(notewise_inputs, unique_onset_idxs):
     """Agregate basis functions per onset"""
-    if isinstance(notewise_inputs, np.ndarray):
-        if notewise_inputs.ndim == 1:
-            shape = len(unique_onset_idxs)
-        else:
-            shape = (len(unique_onset_idxs),) + notewise_inputs.shape[1:]
-        onsetwise_inputs = np.zeros(shape, dtype=notewise_inputs.dtype)
-    elif isinstance(notewise_inputs, torch.Tensor):
-        onsetwise_inputs = torch.zeros(
-            (len(unique_onset_idxs), notewise_inputs.shape[1]),
-            dtype=notewise_inputs.dtype,
-        )
+    
+    if notewise_inputs.ndim == 1:
+        shape = len(unique_onset_idxs)
+    else:
+        shape = (len(unique_onset_idxs),) + notewise_inputs.shape[1:]
+    onsetwise_inputs = np.zeros(shape, dtype=notewise_inputs.dtype)
+    
 
     for i, uix in enumerate(unique_onset_idxs):
         try:
             onsetwise_inputs[i] = notewise_inputs[uix].mean(0)
         except TypeError:
             for tn in notewise_inputs.dtype.names:
                 onsetwise_inputs[i][tn] = notewise_inputs[uix][tn].mean()
     return onsetwise_inputs
 
 
 def onsetwise_to_notewise(onsetwise_input, unique_onset_idxs):
     """Expand onsetwise predictions for each note"""
     n_notes = sum([len(uix) for uix in unique_onset_idxs])
-    if isinstance(onsetwise_input, np.ndarray):
-        if onsetwise_input.ndim == 1:
-            shape = n_notes
-        else:
-            shape = (n_notes,) + onsetwise_input.shape[1:]
-        notewise_inputs = np.zeros(shape, dtype=onsetwise_input.dtype)
-    elif isinstance(onsetwise_input, torch.Tensor):
-        notewise_inputs = torch.zeros(n_notes, dtype=onsetwise_input.dtype)
+    if onsetwise_input.ndim == 1:
+        shape = n_notes
+    else:
+        shape = (n_notes,) + onsetwise_input.shape[1:]
+    notewise_inputs = np.zeros(shape, dtype=onsetwise_input.dtype)
+    
     for i, uix in enumerate(unique_onset_idxs):
         notewise_inputs[uix] = onsetwise_input[[i]]
     return notewise_inputs
 
 
 #### Temo Parameter Normalizations ####
 
+
 def bp_scale(beat_period):
     return [beat_period]
 
 
 def bp_rescale(tempo_params):
     return tempo_params['beat_period']
```

### Comparing `partitura-1.2.2/partitura/musicanalysis/pitch_spelling.py` & `partitura-1.3.0/partitura/musicanalysis/pitch_spelling.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/musicanalysis/tonal_tension.py` & `partitura-1.3.0/partitura/musicanalysis/tonal_tension.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/musicanalysis/voice_separation.py` & `partitura-1.3.0/partitura/musicanalysis/voice_separation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/performance.py` & `partitura-1.3.0/partitura/performance.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/score.py` & `partitura-1.3.0/partitura/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
         -------
         function
             The mapping function
 
         """
         # operations to avoid None values and filter them efficiently.
         m_it = self.measures
+        
         measures = np.array(
             [
                 [
                     m.start.t,
                     m.end.t,
                     (m_it[i - 1].number if m.number == None else m.number),
                 ]
@@ -2396,30 +2397,35 @@
 
 
 class Measure(TimedObject):
     """A measure
 
     Parameters
     ----------
-    number : int or None, optional
-        The number of the measure. Defaults to None
+    number : int
+        The running count independent of measure regularity/ volta endings, continuously counting up all measures in a musicxml score file and always starting from one.
+    name : string, optional
+        The ID of the measure in a given musicxml score file. Can be a non-number in case of volta endings, irregular measures (i.e., pickup measures in the middle of the piece). Defaults to None
 
     Attributes
     ----------
-    number : intp
+    number : int
+        See parameters
+    name : str
         See parameters
 
     """
 
-    def __init__(self, number=None):
+    def __init__(self, number=None, name=None):
         super().__init__()
         self.number = number
+        self.name = name
 
     def __str__(self):
-        return f"{super().__str__()} number={self.number}"
+        return f"{super().__str__()} number={self.number} name={self.name}"
 
     @property
     def page(self):
         """The page number on which this measure appears, or None if
         there is no associated page.
 
         Returns
@@ -3338,15 +3344,15 @@
                         existing_measure.number = mcounter
                         mcounter += 1
                     continue
 
                 else:
                     measure_end = existing_measure.start.t
 
-            part.add(Measure(number=mcounter), int(measure_start), int(measure_end))
+            part.add(Measure(number=mcounter, name=str(mcounter)), int(measure_start), int(measure_end))
 
             # if measure exists but was not at measure_start,
             # a filler measure is added with number mcounter
             if existing_measure:
                 pos = existing_measure.end.t
                 existing_measure.number = mcounter + 1
                 mcounter = mcounter + 2
```

### Comparing `partitura-1.2.2/partitura/utils/__init__.py` & `partitura-1.3.0/partitura/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from partitura.utils.misc import (
     PathLike,
     get_document_name,
     deprecated_alias,
     deprecated_parameter,
 )
 
+from partitura.utils.normalize import normalize
 
 __all__ = [
     "ensure_notearray",
     "note_array_from_part",
     "ensure_rest_array",
     "compute_pianoroll",
     "compute_pitch_class_pianoroll",
@@ -74,8 +75,9 @@
     "fifths_mode_to_key_name",
     "key_mode_to_int",
     "pitch_spelling_to_midi_pitch",
     "pitch_spelling_to_note_name",
     "show_diff",
     "PrettyPrintTree",
     "synthesize",
+    "normalize"
 ]
```

### Comparing `partitura-1.2.2/partitura/utils/generic.py` & `partitura-1.3.0/partitura/utils/generic.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 This module contains generic class- and numerical-related utilities
 """
 import warnings
 from collections import defaultdict
 
-from typing import Union, Callable, Optional
+from typing import Union, Callable, Optional, Tuple
 
 from textwrap import dedent
 import numpy as np
 from scipy.interpolate import interp1d as sc_interp1d
 
 
 __all__ = ["find_nearest", "iter_current_next", "partition", "iter_subclasses"]
@@ -479,15 +479,15 @@
 def interp1d(
     x: np.ndarray,
     y: np.ndarray,
     dtype: Optional[type] = None,
     axis: int = -1,
     kind: Union[str, int] = "linear",
     copy=True,
-    bounds_error=None,
+    bounds_error=False,
     fill_value=np.nan,
     assume_sorted=False,
 ) -> Callable[[Union[float, int, np.ndarray]], np.ndarray]:
     """
     Interpolate a 1-D function using scipy's interp1d method. This utility allows for
     handling the case where `x` and `y` are only a single value (i.e. have length one,
     which results in a ValueError if using scipy's version directly). It also allows for
@@ -611,11 +611,48 @@
 #             new_states = combine(expand(states[0]), states[1:])
 #             return search_recursive(new_states, success, expand, combine)
 #     except RecursionError:
 #         warnings.warn('search exhausted stack, bailing out')
 #         return None
 
 
+def monotonize_times(
+    s: np.ndarray,
+    x: Optional[np.ndarray] = None,
+) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Interpolate linearly over as many points in `s` as necessary to
+    obtain a monotonic sequence. The minimum and maximum of `s` are
+    prepended and appended, respectively, to ensure monotonicity at
+    the bounds of `s`.
+    Parameters
+    ----------
+    s : np.ndarray
+        a sequence of numbers s(x) which we want to monotonize
+    x : np.ndarray or None
+        The input variable of sequence s(x).
+    Returns
+    -------
+    s_mono: np.ndarray
+       a monotonic sequence that has been linearly interpolated using a subset of s
+    x_mono: np.ndarray
+        The input of the monotonic sequence. 
+    """
+    eps = np.finfo(float).eps
+
+    _s = np.r_[np.min(s) - eps, s, np.max(s) + eps]
+    if x is not None:
+        _x = np.r_[np.min(x) - eps, x, np.max(x) + eps]
+    else:
+        _x = np.r_[-eps, np.arange(len(s)), len(s) - 1 + eps]
+
+    s_mono = np.maximum.accumulate(s)
+    mask = np.r_[False, True, (np.diff(s_mono) != 0), False]
+    x_mono = _x[1:-1]
+    s_mono = interp1d(_x[mask], _s[mask], fill_value="extrapolate")(x_mono)
+    
+    return s_mono, x_mono
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `partitura-1.2.2/partitura/utils/misc.py` & `partitura-1.3.0/partitura/utils/misc.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura/utils/music.py` & `partitura-1.3.0/partitura/utils/music.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 import re
 import warnings
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.sparse import csc_matrix
 from typing import Union, Callable, Optional, TYPE_CHECKING
 from partitura.utils.generic import find_nearest, search, iter_current_next
+import partitura
+from tempfile import TemporaryDirectory
+import os
+
+try:
+    import miditok
+    from miditok.midi_tokenizer import MIDITokenizer
+    import miditoolkit 
+except ImportError:
+    miditok = None
+    miditoolkit = None
+    class MIDITokenizer(object):
+        pass
 
 from partitura.utils.misc import deprecated_alias
 
 if TYPE_CHECKING:
     # Import typing info for typing annotations.
     # For this to work we need to import annotations from __future__
     # Solution from
@@ -725,15 +738,15 @@
 
     """
     global MAJOR_KEYS, MINOR_KEYS
 
     if mode in ("minor", -1):
         keylist = MINOR_KEYS
         suffix = "m"
-    elif mode in ("major", None, 1):
+    elif mode in ("major", None, "none", 1):
         keylist = MAJOR_KEYS
         suffix = ""
     else:
         raise Exception("Unknown mode {}".format(mode))
 
     try:
         name = keylist[fifths + 7]
@@ -1190,15 +1203,15 @@
         Indices of the onsets and offsets of the notes in the piano
         roll (in the same order as the input note_array). This is only`
         returned if `return_idxs` is True. The indices have 4 columns
         (`vertical_position_in_piano_roll`, `onset`, `offset`, `original_midi_pitch`).
         The `vertical_position_in_piano_roll` might be different from
         `original_midi_pitch` depending on the `pitch_margin` and  `piano_range`
         arguments.
-    
+
 
     Examples
     --------
 
     >>> import numpy as np
     >>> from partitura.utils import compute_pianoroll
     >>> note_array = np.array([(60, 0, 1)],\
@@ -1287,14 +1300,15 @@
 ):
     # non-public
     """
     Computes a piano roll from a numpy array with MIDI pitch,
     onset, duration and (optionally) MIDI velocity information. See
     `compute_pianoroll` for a complete description of the
     arguments of this function.
+
     """
 
     # Get pitch, onset, offset from the note_info array
     pr_pitch = note_info[:, 0]
     onset = note_info[:, 1]
     duration = note_info[:, 2]
 
@@ -3054,152 +3068,14 @@
         # ix has to be cast as integer depending on the
         # numpy version...
         pnote_array["onset_sec"][ix.astype(int)] = on
 
     return pnote_array
 
 
-def get_time_maps_from_alignment(
-    ppart_or_note_array, spart_or_note_array, alignment, remove_ornaments=True
-):
-    """
-    Get time maps to convert performance time (in seconds) to score time (in beats)
-    and visceversa.
-
-    Parameters
-    ----------
-    ppart_or_note_array : PerformedPart or structured array
-        The performance information as either PerformedPart or the
-        note_array generated from such an object.
-    spart_or_note_array : Part or structured array
-        Score information as either a Part object or the note array
-        generated from such an object.
-    alignment : list
-        The score--performance alignment, a list of dictionaries.
-        (see `partitura.io.importmatch.alignment_from_matchfile` for reference)
-    remove_ornaments : bool (optional)
-        Whether to consider or not ornaments (including grace notes)
-
-    Returns
-    -------
-    ptime_to_stime_map : scipy.interpolate.interp1d
-        An instance of interp1d (a callable) that maps performance time (in seconds)
-        to score time (in beats).
-    stime_to_ptime_map : scipy.interpolate.interp1d
-        An instance of inter1d (a callable) that maps score time (in beats) to
-        performance time (in seconds).
-
-    Note
-    ----
-    This methods uses the average value of the score onsets of notes that are
-    written in the score as part of a chord (i.e., which start at the same time).
-    """
-    # Ensure that we are using structured note arrays
-    perf_note_array = ensure_notearray(ppart_or_note_array)
-    score_note_array = ensure_notearray(spart_or_note_array)
-
-    # Get indices of the matched notes (notes in the score
-    # for which there is a performance note
-    match_idx = get_matched_notes(score_note_array, perf_note_array, alignment)
-
-    # Get onsets and durations
-    score_onsets = score_note_array[match_idx[:, 0]]["onset_beat"]
-    score_durations = score_note_array[match_idx[:, 0]]["duration_beat"]
-
-    perf_onsets = perf_note_array[match_idx[:, 1]]["onset_sec"]
-
-    # Use only unique onsets
-    score_unique_onsets = np.unique(score_onsets)
-
-    # Remove grace notes
-    if remove_ornaments:
-        # TODO: check that all onsets have a duration?
-        # ornaments (grace notes) do not have a duration
-        score_unique_onset_idxs = np.array(
-            [
-                np.where(np.logical_and(score_onsets == u, score_durations > 0))[0]
-                for u in score_unique_onsets
-            ],
-            dtype=object,
-        )
-
-    else:
-        score_unique_onset_idxs = np.array(
-            [np.where(score_onsets == u)[0] for u in score_unique_onsets],
-            dtype=object,
-        )
-
-    # For chords, we use the average performed onset as a proxy for
-    # representing the "performeance time" of the position of the score
-    # onsets
-    eq_perf_onsets = np.array(
-        [np.mean(perf_onsets[u]) for u in score_unique_onset_idxs]
-    )
-
-    # Get maps
-    ptime_to_stime_map = interp1d(
-        x=eq_perf_onsets,
-        y=score_unique_onsets,
-        bounds_error=False,
-        fill_value="extrapolate",
-    )
-    stime_to_ptime_map = interp1d(
-        y=eq_perf_onsets,
-        x=score_unique_onsets,
-        bounds_error=False,
-        fill_value="extrapolate",
-    )
-
-    return ptime_to_stime_map, stime_to_ptime_map
-
-
-def get_matched_notes(spart_note_array, ppart_note_array, alignment):
-    """
-    Get the indices of the matched notes in an alignment
-
-    Parameters
-    ----------
-    spart_note_array : structured numpy array
-        note_array of the score part
-    ppart_note_array : structured numpy array
-        note_array of the performed part
-    alignment : list
-        The score--performance alignment, a list of dictionaries.
-        (see `partitura.io.importmatch.alignment_from_matchfile` for reference)
-
-    Returns
-    -------
-    matched_idxs : np.ndarray
-        A 2D array containing the indices of the matched score and
-        performed notes, where the columns are
-        (index_in_score_note_array, index_in_performance_notearray)
-    """
-    # Get matched notes
-    matched_idxs = []
-    for al in alignment:
-        # Get only matched notes (i.e., ignore inserted or deleted notes)
-        if al["label"] == "match":
-
-            # if ppart_note_array['id'].dtype != type(al['performance_id']):
-            if not isinstance(ppart_note_array["id"], type(al["performance_id"])):
-                p_id = str(al["performance_id"])
-            else:
-                p_id = al["performance_id"]
-
-            p_idx = int(np.where(ppart_note_array["id"] == p_id)[0])
-
-            s_idx = np.where(spart_note_array["id"] == al["score_id"])[0]
-
-            if len(s_idx) > 0:
-                s_idx = int(s_idx)
-                matched_idxs.append((s_idx, p_idx))
-
-    return np.array(matched_idxs)
-
-
 def generate_random_performance_note_array(
     num_notes: int = 20,
     rng: Union[int, np.random.RandomState] = np.random.RandomState(1984),
     duration: float = 10,
     max_note_duration: float = 2,
     min_note_duration: float = 0.1,
     max_velocity: int = 90,
@@ -3339,46 +3215,46 @@
     clip_note_off : bool
         Clip note_off time to end_time
     reindex_notes : bool
         Reindex notes in slice starting from n0
 
     Returns
     -------
-    ppart_slice :  `PerformedPart` object 
-        A copy of input ppart containing notes, programs and control information 
-        only between `start_time` and `end_time` of ppart
+    ppart_slice :  `PerformedPart` object
+        A copy of input ppart containing notes, programs and control
+        information only between `start_time` and `end_time` of ppart
     """
     from partitura.performance import PerformedPart
 
     if not isinstance(ppart, PerformedPart):
         raise ValueError("Input is not an instance of PerformedPart!")
 
     if start_time > end_time:
         raise ValueError("Start time not less than end time!")
 
     # create a new (empty) instance of a PerformedPart
     # single dummy note added to be able to set sustain_pedal_threshold in __init__
     # -> check `adjust_offsets_w_sustain` in partitura.performance
     ppart_slice = PerformedPart([{'note_on': 0, 'note_off': 0}])
 
-    # get ppq if PerformedPart contains it, 
+    # get ppq if PerformedPart contains it,
     # else skip time_tick info when e.g. created with 'load_performance_midi'
     try:
         ppq = ppart.ppq
         ppart_slice.ppq = ppq
     except AttributeError:
         ppq = None
 
     if ppart.controls:
         controls_slice = []
         for cc in ppart.controls:
             if cc['time'] >= start_time and cc['time'] <= end_time:
                 new_cc = cc.copy()
                 new_cc['time'] -= start_time
-                if ppq: 
+                if ppq:
                     new_cc['time_tick'] = int(2 * ppq * cc['time'])
                 controls_slice.append(new_cc)
         ppart_slice.controls = controls_slice
     
     if ppart.programs:
         programs_slice = []
         for pr in ppart.programs:
@@ -3394,31 +3270,31 @@
     note_id = 0
     for note in ppart.notes: 
         # collect previous sounding notes at start_time
         if note["note_on"] < start_time and note["note_off"] > start_time:
             new_note = note.copy()
             new_note['note_on'] = 0.
             if clip_note_off:
-                new_note['note_off'] = min(note['note_off'] - start_time, end_time)
+                new_note['note_off'] = min(note['note_off'] - start_time, end_time - start_time)
             else: 
                 new_note['note_off'] = note['note_off'] - start_time
             if ppq:
                 new_note['note_on_tick'] = 0
                 new_note['note_off_tick'] = int(2 * ppq * new_note['note_off'])
             if reindex_notes:
-                new_note['id'] = 'n' + str(note_id)
+                new_note['id'] = f"n{note_id}"
                 note_id += 1
             notes_slice.append(new_note)
         # todo - combine both cases
         if note['note_on'] >= start_time: 
             if note['note_on'] < end_time:
                 new_note = note.copy()
                 new_note['note_on'] -= start_time
                 if clip_note_off:
-                    new_note['note_off'] = min(note['note_off'] - start_time, end_time)
+                    new_note['note_off'] = min(note['note_off'] - start_time, end_time - start_time)
                 else: 
                     new_note['note_off'] = note['note_off'] - start_time
                 if ppq:
                     new_note['note_on_tick'] = int(2 * ppq * new_note['note_on'])
                     new_note['note_off_tick'] = int(2 * ppq * new_note['note_off'])
                 if reindex_notes:
                     new_note['id'] = 'n' + str(note_id)
@@ -3437,11 +3313,44 @@
         ppart_slice.id = ppart.id + '_slice_{}s_to_{}s'.format(start_time, end_time)     
     if ppart.part_name:
         ppart_slice.part_name = ppart.part_name 
 
     return ppart_slice
 
 
+def tokenize(score_data : ScoreLike, tokenizer : MIDITokenizer, incomplete_bar_behaviour : str = "pad_bar"):
+    """
+    Tokenize a score using a tokenizer from miditok.
+    Parameters
+    ----------
+    score_data : Score, list, Part, or PartGroup
+        The musical score to be saved. A :class:`partitura.score.Score` object,
+        a :class:`partitura.score.Part`, a :class:`partitura.score.PartGroup` or
+        a list of these.
+    tokenizer : MIDITokenizer
+        A tokenizer from miditok.
+    incomplete_bar_behaviour : str
+        How to handle incomplete bars at the beginning (pickup measures) and
+        during the score. Can be one of 'pad_bar', 'shift', or 'time_sig_change'.
+        See :func:`partitura.io.exportmidi.save_score_midi` for details.
+        Defaults to 'pad_bar'.
+    Returns
+    -------
+    ppart_slice :  `Tokens` object
+        Tokens as produced by the miditok library.
+    """
+
+    if miditok is None or miditoolkit is None:
+        raise ImportError("Miditok and miditoolkit must be installed for this function to work")
+    with TemporaryDirectory() as tmpdir:
+        temp_midi_path = os.path.join(tmpdir, "temp_midi.mid")
+        partitura.io.exportmidi.save_score_midi(score_data, out = temp_midi_path, anacrusis_behavior=incomplete_bar_behaviour, part_voice_assign_mode = 4, minimum_ppq = 480 )
+        midi = miditoolkit.MidiFile(temp_midi_path)
+        tokens = tokenizer(midi)
+    return tokens
+
+
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `partitura-1.2.2/partitura/utils/synth.py` & `partitura-1.3.0/partitura/utils/synth.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/partitura.egg-info/PKG-INFO` & `partitura-1.3.0/partitura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: partitura
-Version: 1.2.2
+Version: 1.3.0
 Summary: A package for handling symbolic musical information
 Home-page: https://github.com/CPJKU/partitura
 Author: Maarten Grachten, Carlos Cancino-Chacón, Silvan Peter, Emmanouil Karystinaios, Francesco Foscarin, Thassilo Gadermaier
 Author-email: partitura-users@googlegroups.com
 License: Apache 2.0
 Keywords: music notation musicxml midi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [//]: # (<p align="center"> )
 
 [//]: # (<img src="./partitura/assets/partitura_logo_final.jpg" height="200">)
```

### Comparing `partitura-1.2.2/partitura.egg-info/SOURCES.txt` & `partitura-1.3.0/partitura.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,58 +23,65 @@
 partitura/io/exportmidi.py
 partitura/io/exportmusicxml.py
 partitura/io/exportparangonada.py
 partitura/io/importkern.py
 partitura/io/importmatch.py
 partitura/io/importmei.py
 partitura/io/importmidi.py
+partitura/io/importmusic21.py
 partitura/io/importmusicxml.py
 partitura/io/importnakamura.py
 partitura/io/importparangonada.py
 partitura/io/matchfile_base.py
 partitura/io/matchfile_utils.py
 partitura/io/matchlines_v0.py
 partitura/io/matchlines_v1.py
 partitura/io/musescore.py
 partitura/musicanalysis/__init__.py
 partitura/musicanalysis/key_identification.py
 partitura/musicanalysis/meter.py
+partitura/musicanalysis/note_array_to_score.py
 partitura/musicanalysis/note_features.py
 partitura/musicanalysis/performance_codec.py
+partitura/musicanalysis/performance_features.py
 partitura/musicanalysis/pitch_spelling.py
 partitura/musicanalysis/tonal_tension.py
 partitura/musicanalysis/voice_separation.py
 partitura/utils/__init__.py
 partitura/utils/generic.py
 partitura/utils/misc.py
 partitura/utils/music.py
+partitura/utils/normalize.py
 partitura/utils/synth.py
 tests/test_deprecations.py
 tests/test_display.py
 tests/test_harmony.py
 tests/test_kern.py
 tests/test_key_estimation.py
 tests/test_load_performance.py
 tests/test_load_score.py
+tests/test_m21_import.py
 tests/test_match_export.py
 tests/test_match_import.py
 tests/test_mei.py
 tests/test_merge_parts.py
 tests/test_metrical_position.py
 tests/test_midi_export.py
 tests/test_midi_import.py
 tests/test_nakamura.py
 tests/test_new_divs.py
 tests/test_note_array.py
 tests/test_note_features.py
 tests/test_octave_shift.py
 tests/test_parangonada.py
 tests/test_part_properties.py
+tests/test_partial_measures.py
 tests/test_performance.py
 tests/test_performance_codec.py
+tests/test_performance_features.py
 tests/test_pianoroll.py
 tests/test_pitch_spelling.py
 tests/test_quarter_adjust.py
 tests/test_rest_array.py
 tests/test_synth.py
 tests/test_time_estimation.py
 tests/test_times.py
```

### Comparing `partitura-1.2.2/setup.py` & `partitura-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Package meta-data.
 NAME = "partitura"
 DESCRIPTION = "A package for handling symbolic musical information"
 KEYWORDS = "music notation musicxml midi"
 URL = "https://github.com/CPJKU/partitura"
 EMAIL = "partitura-users@googlegroups.com"
 AUTHOR = "Maarten Grachten, Carlos Cancino-Chacón, Silvan Peter, Emmanouil Karystinaios, Francesco Foscarin, Thassilo Gadermaier"
-REQUIRES_PYTHON = ">=3.6"
-VERSION = "1.2.2"
+REQUIRES_PYTHON = ">=3.7"
+VERSION = "1.3.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["numpy", "scipy", "lxml", "lark-parser", "xmlschema", "mido"]
 
 # What packages are optional?
 EXTRAS = {}
```

### Comparing `partitura-1.2.2/tests/test_deprecations.py` & `partitura-1.3.0/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_display.py` & `partitura-1.3.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_harmony.py` & `partitura-1.3.0/tests/test_harmony.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_kern.py` & `partitura-1.3.0/tests/test_kern.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_key_estimation.py` & `partitura-1.3.0/tests/test_key_estimation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_load_performance.py` & `partitura-1.3.0/tests/test_load_performance.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_load_score.py` & `partitura-1.3.0/tests/test_load_score.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_match_export.py` & `partitura-1.3.0/tests/test_match_export.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_match_import.py` & `partitura-1.3.0/tests/test_match_import.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_mei.py` & `partitura-1.3.0/tests/test_mei.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-This module contains test functions for MEI export
+This file contains test functions for MEI import
 """
 
 import unittest
 
 from tests import MEI_TESTFILES
 from partitura import load_musicxml, load_mei, EXAMPLE_MEI
 import partitura.score as score
```

### Comparing `partitura-1.2.2/tests/test_merge_parts.py` & `partitura-1.3.0/tests/test_merge_parts.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_metrical_position.py` & `partitura-1.3.0/tests/test_metrical_position.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_midi_export.py` & `partitura-1.3.0/tests/test_midi_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 """
 import logging
 from collections import defaultdict, Counter, OrderedDict
 import unittest
 from tempfile import TemporaryFile
 import mido
 import numpy as np
+from tempfile import TemporaryDirectory
+import os
 
-from partitura import save_score_midi, save_performance_midi, load_performance_midi
+from partitura import save_score_midi, save_performance_midi, load_performance_midi, load_score
 from partitura.utils import partition
 import partitura.score as score
 
 from partitura.performance import PerformedPart, Performance
+from tests import MIDIEXPORT_TESTFILES
 
 LOGGER = logging.getLogger(__name__)
 
 RNG = np.random.RandomState(1984)
 
 
 def get_track_voice_numbers(mid):
@@ -475,7 +478,43 @@
             idx = track_idxs[i * track_length : (i + 1) * track_length]
         else:
             idx = track_idxs[i * track_length :]
         note_array["track"][idx] = i
 
     performed_part = PerformedPart.from_note_array(note_array)
     return performed_part
+
+class TestIncompleteMeasures(unittest.TestCase):
+    def test_timesigchange(self):
+        # test the behavior with the time_sig_change parameter in midi export
+        score_data = load_score(MIDIEXPORT_TESTFILES[0])
+        with TemporaryDirectory() as tmpdir:
+            temp_midi_path = os.path.join(tmpdir, "temp_midi.mid")
+            save_score_midi(score_data, out=temp_midi_path, anacrusis_behavior="time_sig_change", part_voice_assign_mode = 4 )
+            mid_pt = mido.MidiFile(temp_midi_path)
+        ts_messages = [m for m in list(mid_pt.tracks[0]) if isinstance(m,mido.MetaMessage) and m.type == "time_signature"]
+        self.assertTrue(len(ts_messages)==5)
+        self.assertTrue(ts_messages[0].numerator == 1)
+        self.assertTrue(ts_messages[1].numerator == 4)
+        self.assertTrue(ts_messages[2].numerator == 3)
+        self.assertTrue(ts_messages[3].numerator == 1)
+        self.assertTrue(ts_messages[4].numerator == 4)
+
+    def test_pad_bar(self):
+        # test the behavior with the pad_bar parameter in midi export
+        score_data = load_score(MIDIEXPORT_TESTFILES[0])
+        with TemporaryDirectory() as tmpdir:
+            temp_midi_path = os.path.join(tmpdir, "temp_midi.mid")
+            save_score_midi(score_data, out=temp_midi_path, anacrusis_behavior="pad_bar", part_voice_assign_mode = 4 )
+            mid_pt = mido.MidiFile(temp_midi_path)
+        ts_messages = [m for m in list(mid_pt.tracks[0]) if isinstance(m,mido.MetaMessage) and m.type == "time_signature"]
+        self.assertTrue(len(ts_messages)==1)
+        # check the position of the first note_on message
+        all_messages = list(mid_pt.tracks[0])
+        cumulative_position = 0
+        index = 0
+        while not (isinstance(all_messages[index],mido.Message) and all_messages[index].type == "note_on"):
+            cumulative_position += all_messages[index].time
+            index+=1
+        self.assertTrue(cumulative_position==3)
+
+
```

### Comparing `partitura-1.2.2/tests/test_midi_import.py` & `partitura-1.3.0/tests/test_midi_import.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_nakamura.py` & `partitura-1.3.0/tests/test_nakamura.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_new_divs.py` & `partitura-1.3.0/tests/test_new_divs.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_note_features.py` & `partitura-1.3.0/tests/test_note_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             stactest = na["articulation_feature.staccato"] == np.array(
                 [1, 0, 0, 0, 0, 0]
             )
             tentest = na["articulation_feature.tenuto"] == np.array([0, 1, 0, 0, 0, 0])
             trilltest = na["ornament_feature.trill-mark"] == np.array(
                 [0, 0, 1, 0, 0, 0]
             )
-            gracetest = na["grace_feature.grace_note"] == np.array([0, 0, 0, 0, 1, 1])
+            gracetest = na["grace_feature.grace_note"] == np.array([0, 0, 0, 1, 0, 1])
             dyntest = na["loudness_direction_feature.f"] == np.array([0, 0, 0, 1, 1, 1])
             slurtest = na["slur_feature.slur_decr"] == np.array([0, 0, 0, 1, 1, 1])
             self.assertTrue(np.all(stactest), "staccato feature does not match")
             self.assertTrue(np.all(tentest), "tenuto feature does not match")
             self.assertTrue(np.all(trilltest), "trill feature does not match")
             self.assertTrue(np.all(gracetest), "grace feature does not match")
             self.assertTrue(np.all(dyntest), "forte feature does not match")
```

### Comparing `partitura-1.2.2/tests/test_octave_shift.py` & `partitura-1.3.0/tests/test_octave_shift.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_parangonada.py` & `partitura-1.3.0/tests/test_parangonada.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_part_properties.py` & `partitura-1.3.0/tests/test_part_properties.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_performance.py` & `partitura-1.3.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_performance_codec.py` & `partitura-1.3.0/tests/test_performance_codec.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_pianoroll.py` & `partitura-1.3.0/tests/test_pianoroll.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_pitch_spelling.py` & `partitura-1.3.0/tests/test_pitch_spelling.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_quarter_adjust.py` & `partitura-1.3.0/tests/test_quarter_adjust.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_rest_array.py` & `partitura-1.3.0/tests/test_rest_array.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_synth.py` & `partitura-1.3.0/tests/test_synth.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_time_estimation.py` & `partitura-1.3.0/tests/test_time_estimation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_times.py` & `partitura-1.3.0/tests/test_times.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_tonal_tension.py` & `partitura-1.3.0/tests/test_tonal_tension.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_transpose.py` & `partitura-1.3.0/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_utils.py` & `partitura-1.3.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,32 +4,36 @@
 This module contains tests for the utility methods.
 """
 import unittest
 import partitura
 import numpy as np
 
 from partitura.utils import music
-from tests import MATCH_IMPORT_EXPORT_TESTFILES, VOSA_TESTFILES, MOZART_VARIATION_FILES
+from partitura.musicanalysis import performance_codec
+from tests import MATCH_IMPORT_EXPORT_TESTFILES, VOSA_TESTFILES, MOZART_VARIATION_FILES, TOKENIZER_TESTFILES
 
 from scipy.interpolate import interp1d as scinterp1d
 from partitura.utils.generic import interp1d as pinterp1d
+from partitura.utils.music import tokenize
+import miditok
+import miditoolkit
 
 RNG = np.random.RandomState(1984)
 
 
 class TestGetMatchedNotes(unittest.TestCase):
     def test_get_matched_notes(self):
         for fn in MATCH_IMPORT_EXPORT_TESTFILES:
             perf, alignment, scr = partitura.load_match(
                 filename=fn,
                 create_score=True,
             )
             perf_note_array = perf.note_array()
             scr_note_array = scr.note_array()
-            matched_idxs = music.get_matched_notes(
+            matched_idxs = performance_codec.get_matched_notes(
                 spart_note_array=scr_note_array,
                 ppart_note_array=perf_note_array,
                 alignment=alignment,
             )
             scr_pitch = scr_note_array["pitch"][matched_idxs[:, 0]]
             perf_pitch = perf_note_array["pitch"][matched_idxs[:, 1]]
 
@@ -49,15 +53,15 @@
                     dict(label="match", score_id=sid, performance_id=sid)
                     for sid in note_ids
                 ]
 
                 (
                     ptime_to_stime_map,
                     stime_to_ptime_map,
-                ) = music.get_time_maps_from_alignment(
+                ) = performance_codec.get_time_maps_from_alignment(
                     spart_or_note_array=scr[0],
                     ppart_or_note_array=ppart,
                     alignment=alignment,
                     remove_ornaments=True,
                 )
 
                 score_onsets = np.arange(4, 0.5)
@@ -90,15 +94,15 @@
                 self.assertTrue(np.all(pnote_array["velocity"] == vel))
 
                 alignment = [
                     dict(label="match", score_id=sid, performance_id=sid)
                     for sid in snote_array["id"]
                 ]
 
-                matched_idxs = music.get_matched_notes(
+                matched_idxs = performance_codec.get_matched_notes(
                     spart_note_array=snote_array,
                     ppart_note_array=pnote_array,
                     alignment=alignment,
                 )
 
                 # check pitch
                 self.assertTrue(
@@ -431,38 +435,73 @@
                 note_array["onset_sec"] >= start_time,
                 note_array["onset_sec"] <= end_time,
             )
         )
 
         target_note_array = note_array[idx]
 
-        ppart_slice = music.slice_ppart_by_time(
-            ppart=ppart,
-            start_time=start_time,
-            end_time=end_time,
-            clip_note_off=False,
-            reindex_notes=False,
-        )
+        def test_arrays(clip_note_off, reindex_notes):
 
-        slice_note_array = ppart_slice.note_array()
+            # Test without clipping note offs
+            ppart_slice = music.slice_ppart_by_time(
+                ppart=ppart,
+                start_time=start_time,
+                end_time=end_time,
+                clip_note_off=clip_note_off,
+                reindex_notes=reindex_notes,
+            )
+            slice_note_array = ppart_slice.note_array()
 
-        self.assertTrue(len(target_note_array) == len(slice_note_array))
-        self.assertTrue(slice_note_array["onset_sec"].max() <= (end_time - start_time))
-        self.assertTrue(
-            np.isclose(
-                target_note_array["onset_sec"].min() - start_time,
-                slice_note_array["onset_sec"].min(),
+            self.assertTrue(len(target_note_array) == len(slice_note_array))
+            self.assertTrue(
+                slice_note_array["onset_sec"].max() <= (end_time - start_time)
             )
-        )
-        self.assertTrue(
-            np.isclose(
-                target_note_array["onset_sec"].max() - start_time,
-                slice_note_array["onset_sec"].max(),
+
+            if clip_note_off:
+                self.assertTrue(
+                    (
+                        slice_note_array["onset_sec"] + slice_note_array["duration_sec"]
+                    ).max()
+                    <= (end_time - start_time)
+                )
+            else:
+                self.assertTrue(
+                    (
+                        slice_note_array["onset_sec"] + slice_note_array["duration_sec"]
+                    ).max()
+                    >= (end_time - start_time)
+                )
+
+            self.assertTrue(
+                np.isclose(
+                    target_note_array["onset_sec"].min() - start_time,
+                    slice_note_array["onset_sec"].min(),
+                )
             )
-        )
+            self.assertTrue(
+                np.isclose(
+                    target_note_array["onset_sec"].max() - start_time,
+                    slice_note_array["onset_sec"].max(),
+                )
+            )
+
+            nidx = slice_note_array["id"]
+            nidx.sort()
+
+            if reindex_notes:
+                tidx = np.array([f"n{idx}" for idx in range(len(nidx))])
+            else:
+                tidx = target_note_array["id"]
+
+            tidx.sort()
+            self.assertTrue(np.all(nidx == tidx))
+
+        for cno in (True, False):
+            for rin in (True, False):
+                test_arrays(cno, rin)
 
 
 class TestGenericUtils(unittest.TestCase):
     def test_interp1d(self):
         """
         Test `interp1d`
         """
@@ -557,7 +596,50 @@
             axis=0,
             kind="previous",
             bounds_error=False,
             fill_value="extrapolate",
         )
 
         self.assertTrue(np.all(sinterp(x) == pinterp(x)))
+
+class TestTokenizer(unittest.TestCase):
+    def test_tokenize1(self):
+        """ Test the partitura tokenizer"""
+        tokenizer = miditok.MIDILike()
+        # produce tokens from the score with partitura
+        pt_score = partitura.load_score(TOKENIZER_TESTFILES[0]["score"])
+        pt_tokens = tokenize(pt_score, tokenizer)[0].tokens
+        # produce tokens from the manually created MIDI file
+        mtok_midi = miditoolkit.MidiFile(TOKENIZER_TESTFILES[0]["midi"])
+        mtok_tokens = tokenizer(mtok_midi)[0].tokens
+        # filter out velocity tokens
+        pt_tokens = [tok for tok in pt_tokens if not tok.startswith("Velocity")]
+        mtok_tokens = [tok for tok in mtok_tokens if not tok.startswith("Velocity")]
+        self.assertTrue(pt_tokens == mtok_tokens)
+
+    def test_tokenize2(self):
+        """ Test the partitura tokenizer"""
+        tokenizer = miditok.REMI()
+        # produce tokens from the score with partitura
+        pt_score = partitura.load_score(TOKENIZER_TESTFILES[0]["score"])
+        pt_tokens = tokenize(pt_score, tokenizer)[0].tokens
+        # produce tokens from the manually created MIDI file
+        mtok_midi = miditoolkit.MidiFile(TOKENIZER_TESTFILES[0]["midi"])
+        mtok_tokens = tokenizer(mtok_midi)[0].tokens
+        # filter out velocity tokens
+        pt_tokens = [tok for tok in pt_tokens if not tok.startswith("Velocity")]
+        mtok_tokens = [tok for tok in mtok_tokens if not tok.startswith("Velocity")]
+        self.assertTrue(pt_tokens == mtok_tokens)
+
+    def test_tokenize1(self):
+        """ Test the partitura tokenizer"""
+        tokenizer = miditok.MIDILike()
+        # produce tokens from the score with partitura
+        pt_score = partitura.load_score(TOKENIZER_TESTFILES[0]["score"])
+        pt_tokens = tokenize(pt_score, tokenizer)[0].tokens
+        # produce tokens from the manually created MIDI file
+        mtok_midi = miditoolkit.MidiFile(TOKENIZER_TESTFILES[0]["midi"])
+        mtok_tokens = tokenizer(mtok_midi)[0].tokens
+        # filter out velocity tokens
+        pt_tokens = [tok for tok in pt_tokens if not tok.startswith("Velocity")]
+        mtok_tokens = [tok for tok in mtok_tokens if not tok.startswith("Velocity")]
+        self.assertTrue(pt_tokens == mtok_tokens)
```

### Comparing `partitura-1.2.2/tests/test_voice_estimation.py` & `partitura-1.3.0/tests/test_voice_estimation.py`

 * *Files identical despite different names*

### Comparing `partitura-1.2.2/tests/test_xml.py` & `partitura-1.3.0/tests/test_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         part1 = score.Part("My Part")
 
         # create contents
         divs = 10
         ts = score.TimeSignature(3, 4)
         page1 = score.Page(1)
         system1 = score.System(1)
-        measure1 = score.Measure(number=1)
+        measure1 = score.Measure(number=1, name='1')
         note1 = score.Note(step="A", octave=4, voice=1, staff=1)
         rest1 = score.Rest(voice=1, staff=1)
         note2 = score.Note(step="C", octave=5, alter=-1, voice=2, staff=1)
 
         # and add the contents to the part:
         part1.set_quarter_duration(0, divs)
         part1.add(ts, 0)
@@ -192,14 +192,15 @@
             part2 = load_musicxml(f)[0]
 
         # pretty print saved/loaded part:
         pstring2 = part2.pretty()
 
         # test pretty printed strings for equality
         equal = pstring1 == pstring2
+        print('equal:', equal)
 
         if not equal:
             show_diff(pstring1, pstring2)
         msg = "Exported and imported score does not yield identical pretty printed representations"
         self.assertTrue(equal, msg)
 
     def test_export_import_tuplet(self):
```

