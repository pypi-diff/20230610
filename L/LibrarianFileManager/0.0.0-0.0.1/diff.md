# Comparing `tmp/LibrarianFileManager-0.0.0.tar.gz` & `tmp/LibrarianFileManager-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibrarianFileManager-0.0.0.tar", last modified: Wed Jun  7 18:24:59 2023, max compression
+gzip compressed data, was "LibrarianFileManager-0.0.1.tar", last modified: Fri Jun  9 22:12:25 2023, max compression
```

## Comparing `LibrarianFileManager-0.0.0.tar` & `LibrarianFileManager-0.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-07 18:24:59.713327 LibrarianFileManager-0.0.0/
--rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-30 20:04:30.000000 LibrarianFileManager-0.0.0/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)      715 2023-06-07 18:24:59.713716 LibrarianFileManager-0.0.0/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-30 20:04:24.000000 LibrarianFileManager-0.0.0/README.md
--rw-r--r--   0 sam        (501) staff       (20)      992 2023-06-07 18:23:28.000000 LibrarianFileManager-0.0.0/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)      307 2023-06-07 18:24:59.715512 LibrarianFileManager-0.0.0/setup.cfg
--rw-r--r--   0 sam        (501) staff       (20)      708 2023-06-07 16:08:05.000000 LibrarianFileManager-0.0.0/setup.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-07 18:24:59.697522 LibrarianFileManager-0.0.0/src/
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-07 18:24:59.702389 LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)      715 2023-06-07 18:24:59.000000 LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      633 2023-06-07 18:24:59.000000 LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2023-06-07 18:24:59.000000 LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)      102 2023-06-07 18:24:59.000000 LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)       10 2023-06-07 18:24:59.000000 LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/top_level.txt
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-07 18:24:59.704805 LibrarianFileManager-0.0.0/src/librarian/
--rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-30 20:06:21.000000 LibrarianFileManager-0.0.0/src/librarian/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     2649 2023-05-31 23:32:54.000000 LibrarianFileManager-0.0.0/src/librarian/actor.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-07 18:24:59.708709 LibrarianFileManager-0.0.0/src/librarian/actors/
--rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-31 22:54:31.000000 LibrarianFileManager-0.0.0/src/librarian/actors/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)    12249 2023-06-07 18:03:19.000000 LibrarianFileManager-0.0.0/src/librarian/actors/plotter.py
--rw-r--r--   0 sam        (501) staff       (20)     3334 2023-06-06 22:13:42.000000 LibrarianFileManager-0.0.0/src/librarian/actors/reader.py
--rw-r--r--   0 sam        (501) staff       (20)     3953 2023-06-07 17:24:17.000000 LibrarianFileManager-0.0.0/src/librarian/actors/writer.py
--rw-r--r--   0 sam        (501) staff       (20)    19045 2023-06-07 18:03:01.000000 LibrarianFileManager-0.0.0/src/librarian/catalog.py
--rw-r--r--   0 sam        (501) staff       (20)     6563 2023-06-07 05:35:56.000000 LibrarianFileManager-0.0.0/src/librarian/librarian.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-07 18:24:59.712381 LibrarianFileManager-0.0.0/src/librarian/plotters/
--rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-31 22:54:37.000000 LibrarianFileManager-0.0.0/src/librarian/plotters/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)      647 2023-06-06 23:33:01.000000 LibrarianFileManager-0.0.0/src/librarian/plotters/errorbarplotter.py
--rw-r--r--   0 sam        (501) staff       (20)      874 2023-06-07 17:56:36.000000 LibrarianFileManager-0.0.0/src/librarian/plotters/histplotter.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-09 22:12:25.112319 LibrarianFileManager-0.0.1/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-30 20:04:30.000000 LibrarianFileManager-0.0.1/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     1176 2023-06-09 22:12:25.112569 LibrarianFileManager-0.0.1/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      460 2023-06-07 18:42:09.000000 LibrarianFileManager-0.0.1/README.md
+-rw-r--r--   0 sam        (501) staff       (20)      992 2023-06-09 22:10:54.000000 LibrarianFileManager-0.0.1/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)      307 2023-06-09 22:12:25.113634 LibrarianFileManager-0.0.1/setup.cfg
+-rw-r--r--   0 sam        (501) staff       (20)      708 2023-06-07 16:08:05.000000 LibrarianFileManager-0.0.1/setup.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-09 22:12:25.096156 LibrarianFileManager-0.0.1/src/
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-09 22:12:25.102011 LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     1176 2023-06-09 22:12:25.000000 LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      633 2023-06-09 22:12:25.000000 LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2023-06-09 22:12:25.000000 LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)      102 2023-06-09 22:12:25.000000 LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)       10 2023-06-09 22:12:25.000000 LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/top_level.txt
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-09 22:12:25.105273 LibrarianFileManager-0.0.1/src/librarian/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-30 20:06:21.000000 LibrarianFileManager-0.0.1/src/librarian/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     2779 2023-06-09 17:34:15.000000 LibrarianFileManager-0.0.1/src/librarian/actor.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-09 22:12:25.109041 LibrarianFileManager-0.0.1/src/librarian/actors/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-31 22:54:31.000000 LibrarianFileManager-0.0.1/src/librarian/actors/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)    12444 2023-06-09 17:35:41.000000 LibrarianFileManager-0.0.1/src/librarian/actors/plotter.py
+-rw-r--r--   0 sam        (501) staff       (20)     3619 2023-06-09 17:36:51.000000 LibrarianFileManager-0.0.1/src/librarian/actors/reader.py
+-rw-r--r--   0 sam        (501) staff       (20)     4783 2023-06-09 17:37:34.000000 LibrarianFileManager-0.0.1/src/librarian/actors/writer.py
+-rw-r--r--   0 sam        (501) staff       (20)    29958 2023-06-09 21:53:45.000000 LibrarianFileManager-0.0.1/src/librarian/catalog.py
+-rw-r--r--   0 sam        (501) staff       (20)     7379 2023-06-09 21:21:57.000000 LibrarianFileManager-0.0.1/src/librarian/librarian.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-06-09 22:12:25.111590 LibrarianFileManager-0.0.1/src/librarian/plotters/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2023-05-31 22:54:37.000000 LibrarianFileManager-0.0.1/src/librarian/plotters/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)      791 2023-06-09 17:39:35.000000 LibrarianFileManager-0.0.1/src/librarian/plotters/errorbarplotter.py
+-rw-r--r--   0 sam        (501) staff       (20)     1009 2023-06-09 17:40:02.000000 LibrarianFileManager-0.0.1/src/librarian/plotters/histplotter.py
```

### Comparing `LibrarianFileManager-0.0.0/PKG-INFO` & `LibrarianFileManager-0.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 Metadata-Version: 2.1
 Name: LibrarianFileManager
-Version: 0.0.0
+Version: 0.0.1
 Summary: A librarian for managing your files: General purpose file management tools for initializing, keeping track of, and interacting with file structures e.g. for cataloging data, plotting of figures, etc.).
 Home-page: https://github.com/samcaf/LibrarianFileManager
 Author: Samuel Alipour-fard
 Author-email: Samuel Alipour-fard <samuelaf@mit.edu>
 Project-URL: Homepage, https://github.com/samcaf/LibrarianFileManager
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# LibrarianFileManager (LFM)
+
+A Librarian for managing your files. General purpose file management tools for initializing, keeping track of, and interacting with file structures e.g. for cataloging data, plotting of figures, etc.).
+
+Also located at
+https://pypi.org/project/LibrarianFileManager/0.0.0/
+
+
+## Setup
+Set up LFM with pip via
+```
+pip install LibrarianFileManager
+```
+
+## Usage
+For now, take a look at the example folder `test_librarian/` for usage.
```

### Comparing `LibrarianFileManager-0.0.0/pyproject.toml` & `LibrarianFileManager-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LibrarianFileManager"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Samuel Alipour-fard", email="samuelaf@mit.edu" },
 ]
 description = "A librarian for managing your files: General purpose file management tools for initializing, keeping track of, and interacting with file structures e.g. for cataloging data, plotting of figures, etc.)."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LibrarianFileManager-0.0.0/setup.py` & `LibrarianFileManager-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/PKG-INFO` & `LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 Metadata-Version: 2.1
 Name: LibrarianFileManager
-Version: 0.0.0
+Version: 0.0.1
 Summary: A librarian for managing your files: General purpose file management tools for initializing, keeping track of, and interacting with file structures e.g. for cataloging data, plotting of figures, etc.).
 Home-page: https://github.com/samcaf/LibrarianFileManager
 Author: Samuel Alipour-fard
 Author-email: Samuel Alipour-fard <samuelaf@mit.edu>
 Project-URL: Homepage, https://github.com/samcaf/LibrarianFileManager
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# LibrarianFileManager (LFM)
+
+A Librarian for managing your files. General purpose file management tools for initializing, keeping track of, and interacting with file structures e.g. for cataloging data, plotting of figures, etc.).
+
+Also located at
+https://pypi.org/project/LibrarianFileManager/0.0.0/
+
+
+## Setup
+Set up LFM with pip via
+```
+pip install LibrarianFileManager
+```
+
+## Usage
+For now, take a look at the example folder `test_librarian/` for usage.
```

### Comparing `LibrarianFileManager-0.0.0/src/LibrarianFileManager.egg-info/SOURCES.txt` & `LibrarianFileManager-0.0.1/src/LibrarianFileManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LibrarianFileManager-0.0.0/src/librarian/actor.py` & `LibrarianFileManager-0.0.1/src/librarian/actor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""This module defines the Actor class, which is a
+base class with methods for performing actions on
+files within a catalog.
+"""
+
 class Actor:
     """The Actor class serves as a base class for specific subclasses
     or implementations like "Plotters," "Loggers," "Converters," and
     others. It takes a catalog object as a parameter during initialization,
     allowing the actor to interact with the catalog and the files within the
     library.
```

### Comparing `LibrarianFileManager-0.0.0/src/librarian/actors/plotter.py` & `LibrarianFileManager-0.0.1/src/librarian/actors/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""This module contains the Plotter class, which is a base
+class with methods for creating figures and for plotting data
+from single or multiple files within a catalog, or between catalogs.
+"""
+
 import warnings
 from datetime import date
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from cycler import cycler
```

### Comparing `LibrarianFileManager-0.0.0/src/librarian/actors/reader.py` & `LibrarianFileManager-0.0.1/src/librarian/actors/reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""This module defines the Reader class, which is a class
+used to read data from files within catalogs.
+
+It can also be used as a base class for other classes which
+are designed to read data from files and then _process_ that data
+in some way. An example is the Plotter subclass.
+"""
+
 import os
 
 # File storage
 import dill as pickle
 import numpy as np
 
 # The Reader acts on files:
```

### Comparing `LibrarianFileManager-0.0.0/src/librarian/librarian.py` & `LibrarianFileManager-0.0.1/src/librarian/librarian.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+"""This module defines the Librarian class, which
+is used to create a file structure associated with a
+project and to manage the project's data at a coarse
+grained level.
+
+The Librarian class can be given a set of folders,
+which will be used to store catalogs for different types
+of information for the project.
+"""
+
 from pathlib import Path
 import dill as pickle
 
 from librarian.catalog import Catalog
 from librarian.catalog import ask_to_overwrite
 
 # TODO:
@@ -30,47 +40,55 @@
     by providing a key-value pair.
 
     The get_project_metadata method returns the project metadata dictionary.
     """
     def __init__(self, location: str,
                  project_metadata: str = '',
                  catalog_folders: dict = None,
-                 catalog_metadata: dict = None):
+                 catalog_metadata: dict = None,
+                 catalog_parameters: dict = None):
         # Project information
         self.location = Path(location)
         self.project_metadata = project_metadata
 
         # ---------------------------------
         # Catalog information
         # ---------------------------------
         # Folder locations as a dict of the form {name: dir}
         self.catalog_folders = catalog_folders
 
         # Catalog .yaml locations as a dict of the form {name: yaml}
         self.catalog_yamls = {cat_name: Path(cat_location) / f"{cat_name}.yaml"
-                          for cat_name, cat_location in catalog_folders.items()}
+                              for cat_name, cat_location
+                              in catalog_folders.items()}
+
+        # Parameters describing the data in each catalog
+        self.catalog_parameters = {cat_name: None
+                                   for cat_name in catalog_folders}
+        if catalog_parameters is not None:
+            self.catalog_parameters.update(catalog_parameters)
 
         # Catalog metadata as a dict of the form {name: metadata}
-        if catalog_metadata is not None:
-            assert catalog_metadata.keys() == catalog_folders.keys(), \
-                "Catalog structure and metadata keys must match."
-            self.catalog_metadata = catalog_metadata
-        else:
-            self.catalog_metadata = {}
+        self.catalog_metadata = {cat_name: {}
+                                 for cat_name in catalog_folders}
+        self.catalog_metadata.update(catalog_metadata)
 
         # Making the project location if it doesn't exist
         self.location.mkdir(parents=True, exist_ok=True)
 
 
     def create_stacks(self, save=False):
         """Creates folders and files for each catalog in the library."""
         # Create catalogs/dirs with headers
         for catalog_name, catalog_dir in self.catalog_folders.items():
+            metadata = self.catalog_metadata[catalog_name]
+            parameters = self.catalog_parameters[catalog_name]
             self.add_catalog(catalog_name, catalog_dir,
-                     metadata=self.catalog_metadata[catalog_name])
+                             metadata=metadata,
+                             parameters=parameters)
 
         # Create README.md
         self.write_readme()
 
         # pickle librarian object to location
         if save:
             self.save()
@@ -100,50 +118,53 @@
         """
         string = f"# Librarian for `{self.location.name}`\n\n"
         if self.project_metadata:
             string += "## Project Metadata\n\n"
             for key, value in self.project_metadata.items():
                 string += f"- {key}: {value}\n"
         if self.catalog_folders:
-            string += "\n## Catalog Data\n\n"
+            string += "\n## Catalog Data\n"
             for catalog_name, folder in self.catalog_folders.items():
+                string += "\n"
                 string += f"### {catalog_name}\n"
                 string += f"\t- Location: `{folder}`\n"
-                metadata = self.catalog_metadata.get(catalog_name, {})
+                metadata = self.catalog_metadata[catalog_name]
                 for key, value in metadata.items():
                     string += f"\t- {key}: {value}\n"
-                string += "\n"
         return string
 
 
     def write_readme(self):
         """Writes a README.md in self.location using
         project and catalog metadata.
         """
         readme_path = self.location / 'README.md'
         with open(readme_path, 'w', encoding='utf-8') as file:
             file.write(str(self))
 
 
     def add_catalog(self, catalog_name, catalog_dir,
-                    metadata=None, default_behavior='skip'):
+                    metadata=None,
+                    parameters=None,
+                    default_behavior='skip'):
         """Adds a catalog to the library."""
         # Check existence of catalog .yaml file and
         # run by user if default_behavior is None
         catalog_dir = Path(catalog_dir)
         catalog_path = catalog_dir / f"{catalog_name}.yaml"
         if catalog_path.exists():
             print("Catalog with the given name in the "
                   "given location exists!")
             if not ask_to_overwrite(catalog_path, default_behavior):
                 return
 
         # Attempting to initialize the catalog
         # (this creates a folder and .yaml for the catalog)
-        catalog = Catalog(catalog_name, catalog_dir, **metadata)
+        catalog = Catalog(catalog_name, catalog_dir,
+                          parameters=parameters, **metadata)
         catalog.save()
 
         # Add catalog to catalog_folders
         self.catalog_folders[catalog_name] = catalog_dir
         self.catalog_yamls[catalog_name] = catalog_path
         if metadata is not None:
             self.catalog_metadata[catalog_name] = metadata
```

### Comparing `LibrarianFileManager-0.0.0/src/librarian/plotters/histplotter.py` & `LibrarianFileManager-0.0.1/src/librarian/plotters/histplotter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""This module contains the HistPlotter class,
+which is a subclass of the Plotter class designed
+to produce histograms from data.
+"""
+
 import matplotlib.pyplot as plt
 
 from librarian.actors.plotter import Plotter
 
 
 class HistPlotter(Plotter):
     """Plotter class for plotting histograms."""
```

