# Comparing `tmp/neon_gui-1.1.3a5-py3-none-any.whl.zip` & `tmp/neon_gui-1.1.3a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11270 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1831 b- defN 23-Jun-02 18:27 neon_gui/__init__.py
--rw-r--r--  2.0 unx     2575 b- defN 23-Jun-02 18:27 neon_gui/__main__.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Jun-02 18:27 neon_gui/cli.py
--rw-r--r--  2.0 unx     3853 b- defN 23-Jun-02 18:27 neon_gui/service.py
--rw-r--r--  2.0 unx     5572 b- defN 23-Jun-02 18:27 neon_gui/utils.py
--rw-r--r--  2.0 unx     1635 b- defN 23-Jun-02 18:27 neon_gui-1.1.3a5.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1485 b- defN 23-Jun-02 18:27 neon_gui-1.1.3a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 18:27 neon_gui-1.1.3a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-02 18:27 neon_gui-1.1.3a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-02 18:27 neon_gui-1.1.3a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      877 b- defN 23-Jun-02 18:27 neon_gui-1.1.3a5.dist-info/RECORD
-11 files, 20734 bytes uncompressed, 9790 bytes compressed:  52.8%
+Zip file size: 11268 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jun-09 23:16 neon_gui/__init__.py
+-rw-r--r--  2.0 unx     2575 b- defN 23-Jun-09 23:16 neon_gui/__main__.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-Jun-09 23:16 neon_gui/cli.py
+-rw-r--r--  2.0 unx     3853 b- defN 23-Jun-09 23:16 neon_gui/service.py
+-rw-r--r--  2.0 unx     5572 b- defN 23-Jun-09 23:16 neon_gui/utils.py
+-rw-r--r--  2.0 unx     1635 b- defN 23-Jun-09 23:16 neon_gui-1.1.3a6.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1492 b- defN 23-Jun-09 23:16 neon_gui-1.1.3a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 23:16 neon_gui-1.1.3a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-09 23:16 neon_gui-1.1.3a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-09 23:16 neon_gui-1.1.3a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      877 b- defN 23-Jun-09 23:16 neon_gui-1.1.3a6.dist-info/RECORD
+11 files, 20741 bytes uncompressed, 9788 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: neon_gui/service.py
 Comment: 
 
 Filename: neon_gui/utils.py
 Comment: 
 
-Filename: neon_gui-1.1.3a5.dist-info/LICENSE.md
+Filename: neon_gui-1.1.3a6.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_gui-1.1.3a5.dist-info/METADATA
+Filename: neon_gui-1.1.3a6.dist-info/METADATA
 Comment: 
 
-Filename: neon_gui-1.1.3a5.dist-info/WHEEL
+Filename: neon_gui-1.1.3a6.dist-info/WHEEL
 Comment: 
 
-Filename: neon_gui-1.1.3a5.dist-info/entry_points.txt
+Filename: neon_gui-1.1.3a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_gui-1.1.3a5.dist-info/top_level.txt
+Filename: neon_gui-1.1.3a6.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_gui-1.1.3a5.dist-info/RECORD
+Filename: neon_gui-1.1.3a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_gui-1.1.3a5.dist-info/LICENSE.md` & `neon_gui-1.1.3a6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_gui-1.1.3a5.dist-info/METADATA` & `neon_gui-1.1.3a6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.1.3a5
+Version: 1.1.3a6
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: neon-utils[network] (>=1.5.0a11,~=1.3)
-Requires-Dist: ovos-utils (>=0.0.25,~=0.0)
+Requires-Dist: neon-utils[network] (~=1.5)
+Requires-Dist: ovos-utils (~=0.0.33)
+Requires-Dist: ovos-config (~=0.0.10)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
 Requires-Dist: tornado (~=6.0)
 Requires-Dist: ovos-bus-client (~=0.0.3)
-Requires-Dist: ovos-gui (>=0.0.3a2,~=0.0.2)
-Requires-Dist: ovos-config (~=0.0.4)
-Requires-Dist: ovos-plugin-manager (>=0.0.23a22,~=0.0.22)
+Requires-Dist: ovos-gui (!=0.0.3.post1,>=0.0.3a4,~=0.0.2)
 Provides-Extra: docker
+Requires-Dist: ovos-gui-plugin-shell-companion ; extra == 'docker'
 
 # Neon GUI
 GUI Module for Neon Core. This module extracts the GUI components from the 
 [Mycroft Mark 2 Skill](https://github.com/MycroftAI/skill-mark-2) and the `enclosure` module
 from [mycroft-core](https://github.com/MycroftAI/mycroft-core/tree/dev/mycroft/enclosure). 
 
 ## Neon Enhancements
```

## Comparing `neon_gui-1.1.3a5.dist-info/RECORD` & `neon_gui-1.1.3a6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 neon_gui/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 neon_gui/__main__.py,sha256=OsHSVwu4IAIvO5LQmbxnn7_HIMWYkvw43Hsmcr-WBsY,2575
 neon_gui/cli.py,sha256=TnBQ6WXsXXMvffL6FHQ_qeopVX8SqBkkRTxuOi6SBD4,2708
 neon_gui/service.py,sha256=yiLfj5jSiB9hU_rcV7ANMFW_3blhg6h-7iDgW1En0UU,3853
 neon_gui/utils.py,sha256=I-9bDQRY7dD_3d-65KGCHtdPExroatiRpwvpYpfk8BM,5572
-neon_gui-1.1.3a5.dist-info/LICENSE.md,sha256=KxXbLh0XZkaLbNrj5ksC1Hl04EeiMbY-I0pGhKTPBRc,1635
-neon_gui-1.1.3a5.dist-info/METADATA,sha256=7LJ5IDVASoxVGv476vWogXPczbEjLZcaGxKIPuBYk2M,1485
-neon_gui-1.1.3a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_gui-1.1.3a5.dist-info/entry_points.txt,sha256=LzdAhBDD2vSyzkqLJCPDVTEQ_mXNSvQ69skbicVlqII,97
-neon_gui-1.1.3a5.dist-info/top_level.txt,sha256=TYzHMKJMmDxoVOZENwOOqnXQZpcaWbmngtOUOXgDDpY,9
-neon_gui-1.1.3a5.dist-info/RECORD,,
+neon_gui-1.1.3a6.dist-info/LICENSE.md,sha256=KxXbLh0XZkaLbNrj5ksC1Hl04EeiMbY-I0pGhKTPBRc,1635
+neon_gui-1.1.3a6.dist-info/METADATA,sha256=gCiq_F3aiM_qck-bLfaYryMVp4TX0gth28oexqifRfE,1492
+neon_gui-1.1.3a6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_gui-1.1.3a6.dist-info/entry_points.txt,sha256=LzdAhBDD2vSyzkqLJCPDVTEQ_mXNSvQ69skbicVlqII,97
+neon_gui-1.1.3a6.dist-info/top_level.txt,sha256=TYzHMKJMmDxoVOZENwOOqnXQZpcaWbmngtOUOXgDDpY,9
+neon_gui-1.1.3a6.dist-info/RECORD,,
```

