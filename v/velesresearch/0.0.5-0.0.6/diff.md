# Comparing `tmp/velesresearch-0.0.5.tar.gz` & `tmp/velesresearch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velesresearch-0.0.5.tar", max compression
+gzip compressed data, was "velesresearch-0.0.6.tar", max compression
```

## Comparing `velesresearch-0.0.5.tar` & `velesresearch-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-09 21:53:20.015152 velesresearch-0.0.5/LICENSE
--rw-r--r--   0        0        0     1440 2023-06-09 22:37:47.070331 velesresearch-0.0.5/README.md
--rw-r--r--   0        0        0      513 2023-06-10 16:06:02.782537 velesresearch-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 15:09:23.525306 velesresearch-0.0.5/velesresearch/__init__.py
--rw-r--r--   0        0        0     1589 2023-06-10 14:38:02.740277 velesresearch-0.0.5/velesresearch/options.py
--rw-r--r--   0        0        0     5370 2023-06-10 15:51:22.477305 velesresearch-0.0.5/velesresearch/structure.py
--rw-r--r--   0        0        0     1891 2023-06-10 15:54:23.053614 velesresearch-0.0.5/velesresearch/survey_tools.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 velesresearch-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-10 19:45:41.718124 velesresearch-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1438 2023-06-10 19:45:41.718124 velesresearch-0.0.6/README.md
+-rw-r--r--   0        0        0      657 2023-06-10 19:45:41.722124 velesresearch-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/__init__.py
+-rw-r--r--   0        0        0     1589 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/options.py
+-rw-r--r--   0        0        0     6825 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/structure.py
+-rw-r--r--   0        0        0     1945 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/tools.py
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 velesresearch-0.0.6/PKG-INFO
```

### Comparing `velesresearch-0.0.5/LICENSE` & `velesresearch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.5/README.md` & `velesresearch-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="./figs/Veles-logo-white.svg">
-    <source media="(prefers-color-scheme: light)" srcset="./figs/Veles-logo.svg">
+    <source media="(prefers-color-scheme: dark)" srcset="/figs/Veles-logo-white.svg">
+    <source media="(prefers-color-scheme: light)" srcset="/figs/Veles-logo.svg">
     <img alt="Veles logo, text Veles with Veles' rune instead of V." src="Veles-logo.svg" width=60%>
   </picture>
 </p>
 <br>
 
 <!-- badges: start -->
```

### Comparing `velesresearch-0.0.5/pyproject.toml` & `velesresearch-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "velesresearch"
-version = "0.0.5"
+version = "0.0.6"
 description = "Veles is a free and open source python survey tool for researchers."
 license = "GPL-3.0-or-later"
 authors = ["Jakub Jędrusiak <kuba23031999@gmail.com>"]
 readme = "README.md"
+repository = "https://github.com/jakub-jedrusiak/VelesResearch"
+documentation = "https://jakub-jedrusiak.github.io/VelesDocs"
 packages = [{include = "velesresearch"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.24.3"
 pytest = "^7.3.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `velesresearch-0.0.5/velesresearch/options.py` & `velesresearch-0.0.6/velesresearch/options.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.5/velesresearch/survey_tools.py` & `velesresearch-0.0.6/velesresearch/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,12 +59,14 @@
 
 
 def survey(
     *pages: Page | Sequence[Page],
     title: str | None = None,
     description: str | None = None,
     options: SurveyOptions | None = None,
+    create_file: bool = True,
 ) -> Survey:
     "Create Survey object from pages, create json file"
     survey_obj = Survey(pages, title=title, description=description, options=options)
-    survey_obj.create()
+    if create_file:
+        survey_obj.create()
     return survey_obj
```

### Comparing `velesresearch-0.0.5/PKG-INFO` & `velesresearch-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: velesresearch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Veles is a free and open source python survey tool for researchers.
+Home-page: https://github.com/jakub-jedrusiak/VelesResearch
 License: GPL-3.0-or-later
 Author: Jakub Jędrusiak
 Author-email: kuba23031999@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Project-URL: Documentation, https://jakub-jedrusiak.github.io/VelesDocs
+Project-URL: Repository, https://github.com/jakub-jedrusiak/VelesResearch
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="./figs/Veles-logo-white.svg">
-    <source media="(prefers-color-scheme: light)" srcset="./figs/Veles-logo.svg">
+    <source media="(prefers-color-scheme: dark)" srcset="/figs/Veles-logo-white.svg">
+    <source media="(prefers-color-scheme: light)" srcset="/figs/Veles-logo.svg">
     <img alt="Veles logo, text Veles with Veles' rune instead of V." src="Veles-logo.svg" width=60%>
   </picture>
 </p>
 <br>
 
 <!-- badges: start -->
```

