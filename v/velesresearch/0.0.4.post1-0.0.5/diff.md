# Comparing `tmp/velesresearch-0.0.4.post1.tar.gz` & `tmp/velesresearch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velesresearch-0.0.4.post1.tar", max compression
+gzip compressed data, was "velesresearch-0.0.5.tar", max compression
```

## Comparing `velesresearch-0.0.4.post1.tar` & `velesresearch-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-09 21:53:20.015152 velesresearch-0.0.4.post1/LICENSE
--rw-r--r--   0        0        0     1261 2023-06-09 15:14:07.859737 velesresearch-0.0.4.post1/README.md
--rw-r--r--   0        0        0      102 2023-06-09 22:03:56.416947 velesresearch-0.0.4.post1/VelesResearch/__init__.py
--rw-r--r--   0        0        0     1544 2023-06-09 22:03:56.606946 velesresearch-0.0.4.post1/VelesResearch/options.py
--rw-r--r--   0        0        0     1915 2023-06-09 22:03:56.593613 velesresearch-0.0.4.post1/VelesResearch/question_types.py
--rw-r--r--   0        0        0     4472 2023-06-09 22:03:56.636946 velesresearch-0.0.4.post1/VelesResearch/structure.py
--rw-r--r--   0        0        0     1660 2023-06-09 22:03:56.610279 velesresearch-0.0.4.post1/VelesResearch/survey_tools.py
--rw-r--r--   0        0        0      501 2023-06-09 22:31:59.878380 velesresearch-0.0.4.post1/pyproject.toml
--rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 velesresearch-0.0.4.post1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 21:53:20.015152 velesresearch-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1440 2023-06-09 22:37:47.070331 velesresearch-0.0.5/README.md
+-rw-r--r--   0        0        0      513 2023-06-10 16:06:02.782537 velesresearch-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 15:09:23.525306 velesresearch-0.0.5/velesresearch/__init__.py
+-rw-r--r--   0        0        0     1589 2023-06-10 14:38:02.740277 velesresearch-0.0.5/velesresearch/options.py
+-rw-r--r--   0        0        0     5370 2023-06-10 15:51:22.477305 velesresearch-0.0.5/velesresearch/structure.py
+-rw-r--r--   0        0        0     1891 2023-06-10 15:54:23.053614 velesresearch-0.0.5/velesresearch/survey_tools.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 velesresearch-0.0.5/PKG-INFO
```

### Comparing `velesresearch-0.0.4.post1/LICENSE` & `velesresearch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4.post1/VelesResearch/options.py` & `velesresearch-0.0.5/velesresearch/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typeguard import typechecked
+"Options objects definitions"
 
-from typing import Optional
 
-
-@typechecked
 class QuestionOptions:
+    "Options for Question object"
+
     def __init__(
         self,
         required: bool = False,
         answers_order: str = "none",
-        inherit_answers: Optional[str] = None,
+        inherit_answers: str | None = None,
         comment: bool = False,
         comment_text: str = "Other",
         comment_placeholder: str = "",
         visible: bool = True,
         other: bool = False,
         other_text: str = "Other",
         other_placeholder: str = "",
@@ -33,22 +32,26 @@
         self.other_placeholder = other_placeholder
         self.none = none
         self.none_text = none_text
         self.clear_button = clear_button
 
 
 class PageOptions:
+    "Options for Page object"
+
     def __init__(
         self,
         read_only: bool = False,
-        time_limit: Optional[int] = None,
+        time_limit: int | None = None,
         visible: bool = True,
     ):
         self.read_only = read_only
         self.time_limit = time_limit
         self.visible = visible
 
 
 class SurveyOptions:
-    def __init__(self, language: str = "en", url_on_complete: Optional[str] = None):
+    "Optrions for Survey object"
+
+    def __init__(self, language: str = "en", url_on_complete: str | None = None):
         self.language = language
         self.url_on_complete = url_on_complete
```

### Comparing `velesresearch-0.0.4.post1/VelesResearch/question_types.py` & `velesresearch-0.0.5/velesresearch/survey_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,70 @@
-"Classes for different types of questions"
+"Functions and wrappers for creating survey structure"
+from collections.abc import Sequence
+from .structure import Question, Page, Survey
+from .options import QuestionOptions, PageOptions, SurveyOptions
 
-from typeguard import typechecked
 
-from typing import Optional, List, Union, Sequence
-from json import dumps
-from options import QuestionOptions
-
-
-@typechecked
-class Question:
-    "General question class"
-
-    def __init__(
-        self,
-        label: str,
-        question_type: str,
-        question_text: str,
-        *answers: Union[str, Sequence[str]],
-        options: Optional[QuestionOptions] = None,
-        description: Optional[str] = None,
-    ):
-        self.label = label
-        self.question_type = question_type
-        self.question_text = question_text
-        self.answers = answers
-        self.options = options
-        self.description = description
-
-    def __str__(self):
-        answers = "  - " + "\n  - ".join(self.answers)
-        return f"{self.label}:\n{self.question_text} ({self.question_type})\n{answers}"
-
-    def __repr__(self):
-        return f"Question({self.label})"
-
-    def json(self):
-        "Converts question to SurveyJS-compliant json"
-        from structure import SurveyEncoder
-
-        return dumps(self, cls=SurveyEncoder, indent=4)
-
-
-def radio(
-    self,
+def question(
     label: str,
+    question_type: str,
     question_text: str,
-    *answers: Union[str, List[str]],
-    options: Optional[QuestionOptions] = None,
-    description: Optional[str] = None,
-):
-    "Single choice question"
+    *answers: str | Sequence[str],
+    options: QuestionOptions | None = None,
+    description: str | None = None,
+) -> Question:
+    "Wrapper around Question class"
     return Question(
         label,
-        "radio",
-        options,
+        question_type,
         question_text,
         answers,
         options=options,
         description=description,
     )
 
 
-def radio(
-    self,
+def questionnaire(
     label: str,
-    question_text: str,
-    *answers: Union[str, List[str]],
-    options: Optional[QuestionOptions] = None,
-    description: Optional[str] = None,
-):
-    "Single choice question"
-    return Question(
-        label,
-        "checkbox",
-        options,
-        question_text,
-        answers,
-        options=options,
-        description=description,
-    )
+    items: Sequence[str] | str,
+    answers: Sequence[str] | str,
+    question_type: str = "radio",
+    options: QuestionOptions = None,
+    description: str = None,
+) -> list[Question]:
+    "Convert whole questionnaire to Question objects list"
+    q_list = []
+    for i in enumerate(items):
+        q_list.append(
+            Question(
+                f"{label}_{i[0] + 1}",
+                question_type,
+                i[1],
+                answers,
+                options=options,
+                description=description,
+            )
+        )
+    return q_list
+
+
+def page(
+    label: str,
+    *questions: Question | Sequence[Question],
+    title: str | None = None,
+    description: str | None = None,
+    options: PageOptions | None = None,
+) -> Page:
+    "Wrapper around Page class"
+    return Page(label, questions, title=title, description=description, options=options)
+
+
+def survey(
+    *pages: Page | Sequence[Page],
+    title: str | None = None,
+    description: str | None = None,
+    options: SurveyOptions | None = None,
+) -> Survey:
+    "Create Survey object from pages, create json file"
+    survey_obj = Survey(pages, title=title, description=description, options=options)
+    survey_obj.create()
+    return survey_obj
```

### Comparing `velesresearch-0.0.4.post1/VelesResearch/structure.py` & `velesresearch-0.0.5/velesresearch/structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,88 @@
-from typeguard import typechecked
+"Structural elements of the survey"
+from collections.abc import Sequence
+from json import JSONEncoder, dumps
+import numpy as np
+from .options import QuestionOptions, PageOptions, SurveyOptions
 
-from typing import Union, List, Optional
-from json import JSONEncoder
-from numpy import concatenate, array
-from question_types import Question
-from options import *
+
+class Question:
+    "General question class"
+
+    def __init__(
+        self,
+        label: str,
+        question_type: str,
+        question_text: str,
+        *answers: str | Sequence[str],
+        options: QuestionOptions | None = None,
+        description: str | None = None,
+    ):
+        self.label = label
+        self.question_type = question_type
+        self.question_text = question_text
+        self.answers = list(np.concatenate([answers]).flat)
+        self.options = options
+        self.description = description
+
+    def __str__(self):
+        answers = "  - " + "\n  - ".join(self.answers)
+        return (
+            f"{self.label}:\n  {self.question_text} ({self.question_type})\n{answers}"
+        )
+
+    def __repr__(self):
+        return f"Question({self.label})"
 
 
-@typechecked
 class Page:
+    "General page class"
+
     def __init__(
         self,
         label: str,
-        *questions: Union[Question, List[Question]],
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        options: Optional[PageOptions] = None
+        *questions: Question | Sequence[Question],
+        title: str | None = None,
+        description: str | None = None,
+        options: PageOptions | None = None,
     ):
         self.label = label
-        self.questions = list(concatenate([questions]).flat)
+        self.questions = list(np.concatenate([questions]).flat)
         self.title = title
         self.description = description
         self.options = options
 
+    def __str__(self):
+        page = f"Page {self.label}:\n"
+        for i in enumerate(self.questions):
+            page += f"  {i[0] + 1}. {i[1].label}\n"
+        return page
+
 
-@typechecked
 class Survey:
+    "General survey class"
+
     def __init__(
         self,
-        *pages: Union[Page, List[Page]],
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        options: Optional[SurveyOptions] = None
+        *pages: Page | Sequence[Page],
+        title: str | None = None,
+        description: str | None = None,
+        options: SurveyOptions | None = None,
     ):
-        self.pages = list(concatenate([pages]).flat)
+        self.pages = list(np.concatenate([pages]).flat)
         self.title = title
         self.description = description
         self.options = options
 
-    def json(self):
-        from json import dumps
-
-        return dumps(obj=self, cls=SurveyEncoder, indent=2)
-
     def create(self):
-        from json import dumps
-
+        "Saves survey to survey.json file"
         json = dumps(obj=self, cls=SurveyEncoder, indent=2)
-        f = open("survey.json", "w")
-        f.write(json)
-        f.close()
+        survey_file = open("survey.json", "w", encoding="utf-8")
+        survey_file.write(json)
+        survey_file.close()
 
 
 class SurveyEncoder(JSONEncoder):
     "Create SurveyJS-compliant json from Question object"
 
     def default(self, o):
         if isinstance(o, Survey):
@@ -93,15 +122,15 @@
             # SurveyJS types dictionary
             surveyjs_types = {"radio": "radiogroup", "checkbox": "checkbox"}
 
             json = {
                 "name": o.label,
                 "type": surveyjs_types[o.question_type],
                 "title": o.question_text,
-                "choices": list(concatenate([o.answers]).flat),
+                "choices": o.answers,
             }
 
             if o.description:
                 json["description"] = o.description
 
             if o.options:
                 opts = o.options.__dict__
```

### Comparing `velesresearch-0.0.4.post1/PKG-INFO` & `velesresearch-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 Metadata-Version: 2.1
 Name: velesresearch
-Version: 0.0.4.post1
+Version: 0.0.5
 Summary: Veles is a free and open source python survey tool for researchers.
 License: GPL-3.0-or-later
 Author: Jakub Jędrusiak
 Author-email: kuba23031999@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="./figs/Veles-logo-white.svg">
     <source media="(prefers-color-scheme: light)" srcset="./figs/Veles-logo.svg">
     <img alt="Veles logo, text Veles with Veles' rune instead of V." src="Veles-logo.svg" width=60%>
   </picture>
 </p>
 <br>
 
+<!-- badges: start -->
+
+![PyPI](https://img.shields.io/pypi/v/velesresearch)
+![GitHub](https://img.shields.io/github/license/jakub-jedrusiak/VelesResearch)
+
+<!-- badges: end -->
+
 Veles is a free and open source python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
 
 Veles is in pre-alpha development, but the goal features are:
 
 -   Free and open source.
 
 -   Text-based, so automatable and easily modifiable.
```

