# Comparing `tmp/VelesResearch-0.0.3.tar.gz` & `tmp/velesresearch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VelesResearch-0.0.3.tar", last modified: Fri Jun  9 19:45:15 2023, max compression
+gzip compressed data, was "velesresearch-0.0.4.tar", max compression
```

## Comparing `VelesResearch-0.0.3.tar` & `velesresearch-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,9 @@
-drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 19:45:15.112753 VelesResearch-0.0.3/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      351 2023-06-09 19:45:15.112753 VelesResearch-0.0.3/PKG-INFO
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1261 2023-06-09 15:14:07.000000 VelesResearch-0.0.3/README.md
-drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 19:45:15.112753 VelesResearch-0.0.3/VelesResearch/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      101 2023-06-09 19:41:07.000000 VelesResearch-0.0.3/VelesResearch/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1355 2023-06-09 17:35:19.000000 VelesResearch-0.0.3/VelesResearch/options.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1656 2023-06-09 18:41:19.000000 VelesResearch-0.0.3/VelesResearch/question_types.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     4456 2023-06-09 18:41:06.000000 VelesResearch-0.0.3/VelesResearch/structure.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1377 2023-06-09 18:43:57.000000 VelesResearch-0.0.3/VelesResearch/survey_tools.py
-drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 19:45:15.112753 VelesResearch-0.0.3/VelesResearch.egg-info/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      351 2023-06-09 19:45:15.000000 VelesResearch-0.0.3/VelesResearch.egg-info/PKG-INFO
--rw-r--r--   0 jakub     (1000) jakub     (1000)      306 2023-06-09 19:45:15.000000 VelesResearch-0.0.3/VelesResearch.egg-info/SOURCES.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)        1 2023-06-09 19:45:15.000000 VelesResearch-0.0.3/VelesResearch.egg-info/dependency_links.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)       14 2023-06-09 19:45:15.000000 VelesResearch-0.0.3/VelesResearch.egg-info/top_level.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)       38 2023-06-09 19:45:15.112753 VelesResearch-0.0.3/setup.cfg
--rw-r--r--   0 jakub     (1000) jakub     (1000)      568 2023-06-09 19:41:25.000000 VelesResearch-0.0.3/setup.py
+-rw-r--r--   0        0        0    35149 2023-06-09 21:53:20.015152 velesresearch-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1261 2023-06-09 15:14:07.859737 velesresearch-0.0.4/README.md
+-rw-r--r--   0        0        0      102 2023-06-09 22:03:56.416947 velesresearch-0.0.4/VelesResearch/__init__.py
+-rw-r--r--   0        0        0     1544 2023-06-09 22:03:56.606946 velesresearch-0.0.4/VelesResearch/options.py
+-rw-r--r--   0        0        0     1915 2023-06-09 22:03:56.593613 velesresearch-0.0.4/VelesResearch/question_types.py
+-rw-r--r--   0        0        0     4472 2023-06-09 22:03:56.636946 velesresearch-0.0.4/VelesResearch/structure.py
+-rw-r--r--   0        0        0     1660 2023-06-09 22:03:56.610279 velesresearch-0.0.4/VelesResearch/survey_tools.py
+-rw-r--r--   0        0        0      399 2023-06-09 21:43:01.250069 velesresearch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 velesresearch-0.0.4/PKG-INFO
```

### Comparing `VelesResearch-0.0.3/README.md` & `velesresearch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `VelesResearch-0.0.3/VelesResearch/structure.py` & `velesresearch-0.0.4/VelesResearch/structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,93 +2,111 @@
 
 from typing import Union, List, Optional
 from json import JSONEncoder
 from numpy import concatenate, array
 from question_types import Question
 from options import *
 
+
 @typechecked
 class Page:
-    def __init__(self, label: str, *questions: Union[Question, List[Question]], title: Optional[str]=None, description: Optional[str]=None, options: Optional[PageOptions]=None):
+    def __init__(
+        self,
+        label: str,
+        *questions: Union[Question, List[Question]],
+        title: Optional[str] = None,
+        description: Optional[str] = None,
+        options: Optional[PageOptions] = None
+    ):
         self.label = label
         self.questions = list(concatenate([questions]).flat)
         self.title = title
         self.description = description
         self.options = options
 
+
 @typechecked
 class Survey:
-    def __init__(self, *pages: Union[Page, List[Page]], title: Optional[str]=None, description: Optional[str]=None, options: Optional[SurveyOptions]=None):
+    def __init__(
+        self,
+        *pages: Union[Page, List[Page]],
+        title: Optional[str] = None,
+        description: Optional[str] = None,
+        options: Optional[SurveyOptions] = None
+    ):
         self.pages = list(concatenate([pages]).flat)
         self.title = title
         self.description = description
         self.options = options
-    
+
     def json(self):
         from json import dumps
+
         return dumps(obj=self, cls=SurveyEncoder, indent=2)
-    
+
     def create(self):
         from json import dumps
+
         json = dumps(obj=self, cls=SurveyEncoder, indent=2)
         f = open("survey.json", "w")
         f.write(json)
         f.close()
 
+
 class SurveyEncoder(JSONEncoder):
     "Create SurveyJS-compliant json from Question object"
 
     def default(self, o):
         if isinstance(o, Survey):
             json = {
                 "title": o.title,
                 "description": o.description,
-                "pages": [self.default(p) for p in o.pages]
+                "pages": [self.default(p) for p in o.pages],
             }
-            
+
             if o.options:
                 opts = o.options.__dict__
                 if opts["language"] != "en":
                     json["locale"] = opts["language"]
                 if opts["url_on_complete"]:
                     json["navigateToUrl"] = opts["url_on_complete"]
-            
+
         elif isinstance(o, Page):
             json = {
                 "name": o.label,
                 "elements": [self.default(q) for q in o.questions],
             }
-            
+
             if o.title:
                 json["title"] = o.title
             if o.description:
                 json["description"] = o.description
             if o.options:
                 opts = o.options.__dict__
                 if opts["read_only"]:
                     json["readOnly"] = True
                 if opts["time_limit"]:
                     json["maxTimeToFinish"] = opts["time_limit"]
                 if not opts["visible"]:
                     json["visible"] = False
-       
+
         else:
             # SurveyJS types dictionary
             surveyjs_types = {"radio": "radiogroup", "checkbox": "checkbox"}
-            
+
             json = {
                 "name": o.label,
                 "type": surveyjs_types[o.question_type],
                 "title": o.question_text,
-                "choices": list(concatenate([o.answers]).flat)
+                "choices": list(concatenate([o.answers]).flat),
             }
-            
+
             if o.description:
                 json["description"] = o.description
-                
+
             if o.options:
                 opts = o.options.__dict__
                 if not opts["visible"]:
                     json["visible"] = False
                 if opts["required"]:
                     json["isRequired"] = True
                 if opts["answers_order"] != "none":
@@ -109,9 +127,9 @@
                         json["otherPlaceHolder"] = opts["other_placeholder"]
                 if opts["none"]:
                     json["showNoneItem"] = True
                     if opts["none_text"]:
                         json["noneText"] = opts["none_text"]
                 if opts["clear_button"]:
                     json["showClearButton"] = True
-            
+
         return json
```

