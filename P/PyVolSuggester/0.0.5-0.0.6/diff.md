# Comparing `tmp/pyvolsuggester-0.0.5.tar.gz` & `tmp/pyvolsuggester-0.0.6.tar.gz`

## Comparing `pyvolsuggester-0.0.5.tar` & `pyvolsuggester-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,5 @@
--rw-r--r--   0        0        0   348044 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/1.png
--rw-r--r--   0        0        0    98739 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/10.png
--rw-r--r--   0        0        0   360267 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/11.png
--rw-r--r--   0        0        0    96844 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/12.png
--rw-r--r--   0        0        0   213069 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/13.png
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/14.png
--rw-r--r--   0        0        0   147275 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/2.png
--rw-r--r--   0        0        0    70013 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/3.png
--rw-r--r--   0        0        0    22104 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/4.png
--rw-r--r--   0        0        0    17706 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/5.png
--rw-r--r--   0        0        0   101783 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/6.png
--rw-r--r--   0        0        0   944565 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/7.png
--rw-r--r--   0        0        0   573913 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/8.png
--rw-r--r--   0        0        0   105460 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/Images/9.png
--rw-r--r--   0        0        0    16169 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/src/PyVolSuggester/Suggester.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/src/PyVolSuggester/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/License.txt
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/README.md
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.6/License.txt
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.6/README.md
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.6/PKG-INFO
```

### Comparing `pyvolsuggester-0.0.5/License.txt` & `pyvolsuggester-0.0.6/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.5/pyproject.toml` & `pyvolsuggester-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.5"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "0.0.6"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
```

