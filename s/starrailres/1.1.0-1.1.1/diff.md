# Comparing `tmp/starrailres-1.1.0.tar.gz` & `tmp/starrailres-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailres-1.1.0.tar", max compression
+gzip compressed data, was "starrailres-1.1.1.tar", max compression
```

## Comparing `starrailres-1.1.0.tar` & `starrailres-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.0/LICENSE
--rw-r--r--   0        0        0      499 2023-06-09 09:36:07.597528 starrailres-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.0/README.md
--rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.1.0/starrailres/__init__.py
--rw-r--r--   0        0        0    29302 2023-06-09 09:19:54.028504 starrailres-1.1.0/starrailres/index.py
--rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.0/starrailres/models/avatars.py
--rw-r--r--   0        0        0     1723 2023-05-29 05:55:48.065843 starrailres-1.1.0/starrailres/models/characters.py
--rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.0/starrailres/models/common.py
--rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.0/starrailres/models/descriptions.py
--rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.0/starrailres/models/elements.py
--rw-r--r--   0        0        0     2774 2023-06-09 09:28:24.494447 starrailres-1.1.0/starrailres/models/info.py
--rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.0/starrailres/models/items.py
--rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.0/starrailres/models/light_cones.py
--rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.0/starrailres/models/paths.py
--rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.0/starrailres/models/properties.py
--rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.0/starrailres/models/relics.py
--rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.1.0/starrailres/utils.py
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.1/LICENSE
+-rw-r--r--   0        0        0      499 2023-06-10 11:48:43.124281 starrailres-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.1.1/starrailres/__init__.py
+-rw-r--r--   0        0        0    29597 2023-06-10 10:47:50.002358 starrailres-1.1.1/starrailres/index.py
+-rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.1/starrailres/models/avatars.py
+-rw-r--r--   0        0        0     1738 2023-06-10 10:42:25.990067 starrailres-1.1.1/starrailres/models/characters.py
+-rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.1/starrailres/models/common.py
+-rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.1/starrailres/models/descriptions.py
+-rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.1/starrailres/models/elements.py
+-rw-r--r--   0        0        0     2895 2023-06-10 10:47:49.809032 starrailres-1.1.1/starrailres/models/info.py
+-rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.1/starrailres/models/items.py
+-rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.1/starrailres/models/light_cones.py
+-rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.1/starrailres/models/paths.py
+-rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.1/starrailres/models/properties.py
+-rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.1/starrailres/models/relics.py
+-rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.1.1/starrailres/utils.py
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.1/PKG-INFO
```

### Comparing `starrailres-1.1.0/LICENSE` & `starrailres-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.0/README.md` & `starrailres-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.0/starrailres/index.py` & `starrailres-1.1.1/starrailres/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     LightConeInfo,
     PathInfo,
     PropertyInfo,
     RelicBasicInfo,
     RelicInfo,
     RelicSetInfo,
     SkillInfo,
+    SkillTreeInfo,
     SubAffixInfo,
 )
 from .models.light_cones import (
     LightConeIndex,
     LightConePromotionIndex,
     LightConeRankIndex,
 )
@@ -159,14 +160,22 @@
                         ),
                         self.get_character_skill_upgrade_from_skill_tree(
                             basic.id, basic.skill_tree_levels
                         ),
                     ]
                 ),
             ),
+            skill_trees=[
+                SkillTreeInfo(
+                    id=i.id,
+                    level=i.level,
+                    icon=self.character_skill_trees[i.id].icon,
+                )
+                for i in basic.skill_tree_levels
+            ],
             light_cone=None,
             relics=[],
             relic_sets=[],
             attributes=self.get_character_attribute_from_promotion(
                 basic.id, basic.promotion, basic.level
             ),
             additions=[],
```

### Comparing `starrailres-1.1.0/starrailres/models/characters.py` & `starrailres-1.1.1/starrailres/models/characters.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 class CharacterSkillTreeType(Struct):
     id: str
     max_level: int
     anchor: str
     pre_points: List[str]
     level_up_skills: List[Quantity]
     levels: List[SkillTreeLevelType]
+    icon: str
 
 
 class CharacterPromotionType(Struct):
     id: str
     values: List[Dict[str, Promotion]]
     materials: List[List[Quantity]]
```

### Comparing `starrailres-1.1.0/starrailres/models/info.py` & `starrailres-1.1.1/starrailres/models/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     effect: str
     effect_text: str
     simple_desc: str
     desc: str
     icon: str
 
 
+class SkillTreeInfo(Struct):
+    id: str
+    level: int
+    icon: str
+
+
 class PropertyInfo(Struct):
     type: str
     field: str
     name: str
     icon: str
     value: float
     display: str
@@ -137,13 +143,14 @@
     icon: str
     preview: str
     portrait: str
     rank_icons: List[str] = []
     path: Optional[PathInfo] = None
     element: Optional[ElementInfo] = None
     skills: List[SkillInfo] = []
+    skill_trees: List[SkillTreeInfo] = []
     light_cone: Optional[LightConeInfo] = None
     relics: List[RelicInfo] = []
     relic_sets: List[RelicSetInfo] = []
     attributes: List[AttributeInfo] = []
     additions: List[AttributeInfo] = []
     properties: List[PropertyInfo] = []
```

### Comparing `starrailres-1.1.0/starrailres/models/light_cones.py` & `starrailres-1.1.1/starrailres/models/light_cones.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.0/starrailres/models/relics.py` & `starrailres-1.1.1/starrailres/models/relics.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.0/PKG-INFO` & `starrailres-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailres
-Version: 1.1.0
+Version: 1.1.1
 Summary: StarRailRes index package.
 Home-page: https://github.com/Mar-7th/StarRailRes-Python
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

