# Comparing `tmp/odb-plotter-0.5.3.tar.gz` & `tmp/odb-plotter-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.5.3.tar", last modified: Fri Jun  2 17:24:04 2023, max compression
+gzip compressed data, was "odb-plotter-0.5.4.tar", last modified: Sat Jun 10 00:10:04 2023, max compression
```

## Comparing `odb-plotter-0.5.3.tar` & `odb-plotter-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.5.3/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3535 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1610 2023-06-02 17:23:51.000000 odb-plotter-0.5.3/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1194 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.415136 odb-plotter-0.5.3/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3535 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      144 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-02 17:23:51.000000 odb-plotter-0.5.3/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.3/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24794 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.3/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.3/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)     3964 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/npz_to_hdf.py
--rw-r--r--   0 clark     (1000) clark     (1000)    17386 2023-06-02 17:23:51.000000 odb-plotter-0.5.3/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4832 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-05-25 14:12:43.000000 odb-plotter-0.5.3/src/odbp/py2_scripts/extract.py
--rw-r--r--   0 clark     (1000) clark     (1000)     7194 2023-06-01 00:43:21.000000 odb-plotter-0.5.3/src/odbp/py2_scripts/odb_to_npz.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2354 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/read_hdf5.py
--rw-r--r--   0 clark     (1000) clark     (1000)    28791 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     1925 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/util.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.5.4/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3587 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     1662 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1194 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3587 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      144 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.4/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24794 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.4/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.4/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)     3964 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/npz_to_hdf.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    17751 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-06-09 23:40:46.000000 odb-plotter-0.5.4/src/odbp/py2_scripts/extract.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     7226 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/py2_scripts/odb_to_npz.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2382 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/read_hdf5.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    28791 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     1925 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/util.py
```

### Comparing `odb-plotter-0.5.3/LICENSE` & `odb-plotter-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/PKG-INFO` & `odb-plotter-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -62,14 +62,15 @@
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
+    * 0.5.4: Parametrize number of cpus for testing
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.3/README.md` & `odb-plotter-0.5.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
+    * 0.5.4: Parametrize number of cpus for testing
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.3/pyproject.toml` & `odb-plotter-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.5.4/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -62,14 +62,15 @@
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
+    * 0.5.4: Parametrize number of cpus for testing
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.3/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.5.4/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odbp/cli.py` & `odb-plotter-0.5.4/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odbp/data/config.toml` & `odb-plotter-0.5.4/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odbp/npz_to_hdf.py` & `odb-plotter-0.5.4/src/odbp/npz_to_hdf.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odbp/odb.py` & `odb-plotter-0.5.4/src/odbp/odb.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 class Odb():
     """
     Stores Data from a .hdf5, implements extractor methods to transfer from .odb to .hdf5
     Implements abilities to resize the dimenisons or timeframe of the data
     """
 
+    # TODO user settings sub-section, overload getattr
     __slots__ = (
         "_odb_handler",
         "_odb",
         "_x_low",
         "_x_high",
         "_y_low",
         "_y_high",
@@ -51,14 +52,15 @@
         "_hdf_source_dir",
         "_abaqus_executable",
         "_odb_to_npz_script_path",
         "_odb_to_npz_conversion_pickle_path",
         "_npz_result_path",
         "_nodesets",
         "_frames",
+        "_cpus",
         )
 
     def __init__(self) -> None:
         """
         Type Hints and hard-coded parameters. See the @staticmethod
         "constructors" of this class in order to learn about initialization
         """
@@ -103,14 +105,16 @@
         )
 
         self._npz_result_path: pathlib.Path = pathlib.Path(
             pathlib.Path.cwd(),
             "npz_path.pickle"
         )
 
+        self._cpus = multiprocessing.cpu_count()
+
         # TODO
         """self._parts: NullableStrList
         self._nodes: dict[str, list[int]]"""
 
 
     # def __new__(self) -> None:
     #     raise Exception("Do not instantiate OdbViewer instances this way."
@@ -469,14 +473,25 @@
 
 
     @nodesets.setter
     def nodesets(self, value: "List[int]") -> None:
         self._nodesets = value
 
 
+    @property
+    def cpus(self) -> int:
+        return self._cpus
+
+
+    @cpus.setter
+    def cpus(self, value: int) -> None:
+        assert value > 0
+        self._cpus = value
+
+
     """def set_parts(self, parts: "list[str]") -> None:
         if not isinstance(parts, list):
             new_list: list[str] = [parts]
             self.parts = new_list
 
         else:
             self.parts = parts
@@ -553,15 +568,16 @@
             odb_path: pathlib.Path
             ) -> None:
 
         odb_to_npz_pickle_input_dict: Dict[
             str, Union[List[str], List[int], None]
             ] = {
                 "nodesets": self._nodesets,
-                "frames": self._frames
+                "frames": self._frames,
+                "cpus": self.cpus
             }
         pickle_file: TextIO
         with open(
             self._odb_to_npz_conversion_pickle_path, "wb") as pickle_file:
             pickle.dump(odb_to_npz_pickle_input_dict, pickle_file, protocol=2)
 
         odb_convert_args: List[Union[pathlib.Path, str]]  = [
@@ -592,15 +608,15 @@
 
         if not hasattr(self, "hdf_path"):
             raise AttributeError("hdf_path attribute must be set before "
                     "calling load_hdf method.")
 
         try:
             # Only case where this should be set, bypass the setter
-            self._odb = self._odb_handler.load_hdf(self.hdf_path)
+            self._odb = self._odb_handler.load_hdf(self.hdf_path, self.cpus)
             self._odb_handler = OdbUnloader()
 
         except AttributeError:
             raise AttributeError("load_hdf can only be used once in a row, "
                     "before a .hdf5 file is loaded. Call unload_hdf on this "
                     "OdbViewer before calling load_hdf.")
 
@@ -619,16 +635,16 @@
 
 
     # TODO generator method for time steps. Overload __iter__?
 
 
 class OdbLoader:
 
-    def load_hdf(self, hdf_path: pathlib.Path) -> DataFrameType:
-        return get_odb_data(hdf_path)
+    def load_hdf(self, hdf_path: pathlib.Path, cpus: int) -> DataFrameType:
+        return get_odb_data(hdf_path, cpus)
 
 
 class OdbUnloader:
 
     @abstractmethod
     def unload_hdf(self) -> None:
         ...
```

### Comparing `odb-plotter-0.5.3/src/odbp/odb_visualizer.py` & `odb-plotter-0.5.4/src/odbp/odb_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             Tuple[
                 float,
                 str
                 ]
             ] = [(time, label) for time in times]
         results: List[pv.Plotter] = list()
         pool: MultiprocessingPoolType
-        with multiprocessing.Pool() as pool:
+        with multiprocessing.Pool(processes=self.cpus) as pool:
             results: list[pv.Plotter] = pool.starmap(
                 self.plot_3d_single,
                 plotting_args
                 )"""
 
         return results
```

### Comparing `odb-plotter-0.5.3/src/odbp/py2_scripts/extract.py` & `odb-plotter-0.5.4/src/odbp/py2_scripts/extract.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odbp/py2_scripts/odb_to_npz.py` & `odb-plotter-0.5.4/src/odbp/py2_scripts/odb_to_npz.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,25 +48,26 @@
         pickle_file.close()
 
     # Now we can remove the file
     os.remove(pickle_path)
 
     nodesets = data_to_extract["nodesets"]
     frames = data_to_extract["frames"]
+    num_cpus = data_to_extract["cpus"]
 
-    result_name = convert_odb_to_npz(odb_path, nodesets, frames)
+    result_name = convert_odb_to_npz(odb_path, nodesets, frames, num_cpus)
     result_file = open(result_path, "wb")
     try:
         pickle.dump(result_name, result_file)
     finally:
         result_file.close()
 
 
 
-def convert_odb_to_npz(odb_path, nodesets, frames):
+def convert_odb_to_npz(odb_path, nodesets, frames, num_cpus):
     """
     Based on the 4 lists given, convert the .odb data to .npz files
     odb_path: str path to the .odb file
     nodes: list[int] which nodes to convert (default to all)
     parts: list[str] which parts to convert (default to no specific part)
     nodesets: list[str] which nodesets to convert (default to the first
     nodeset)
@@ -111,20 +112,20 @@
 
     odb.close()
 
     for nodeset in nodesets:
         for step_key, base_time in base_times:
             coord_file = os.path.join(parent_dir, "node_coords.npz")
             read_nodeset_coords(odb_path, nodeset, coord_file, step_key)
-            read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset)
+            read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset, num_cpus)
 
     return parent_dir
 
 
-def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset):
+def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset, num_cpus):
     odb = openOdb(odb_path, readOnly=True)
     steps = odb.steps
 
     curr_step_dir = os.path.join(temps_dir, step_key)
     if not os.path.exists(curr_step_dir):
         os.mkdir(curr_step_dir)
 
@@ -139,15 +140,14 @@
     manager = multiprocessing.Manager()
     frame_times = manager.list()
     #frame_times = list()
     if len(steps[step_key].frames) > 0:
         idx_list = [i for i in range(len(steps[step_key].frames))]
         idx_list_len = len(idx_list)
         idx_list_max = idx_list[-1]
-        num_cpus = multiprocessing.cpu_count()
         # TODO: what if the length isn't divisible by the number of processors (is it now?)
         final_idx_list = [idx_list[i: i + int(idx_list_len / num_cpus)] for i in range(0, idx_list_len, max(int(idx_list_len / num_cpus), 1))]
         odb.close()
 
         temp_procs = list()
         for idx_list in final_idx_list:
             p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, frames, step_key, curr_step_dir, frame_times, base_time, nodeset))
```

### Comparing `odb-plotter-0.5.3/src/odbp/read_hdf5.py` & `odb-plotter-0.5.4/src/odbp/read_hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import pandas as pd
 from typing import Tuple, List
 from .util import NDArrayType, DataFrameType, H5PYGroupType, H5PYFileType, MultiprocessingPoolType
 
 
 def get_odb_data(
     hdf_path: pathlib.Path
+    cpus: int
     ) -> DataFrameType:
     """
     get_node_coords(hdf_path: pathlib.Path) -> DataFrameType
     return a data frame with nodes by integer index and floating point
     3-dimensional coordinates.
     """
 
@@ -39,15 +40,15 @@
                         (hdf_path, step, frame_name)
                         for frame_name
                         in hdf_file["nodes"][step].keys() 
                         ]
 
                 results: List[DataFrameType]
                 pool: MultiprocessingPoolType
-                with multiprocessing.Pool() as pool:
+                with multiprocessing.Pool(processes=cpus) as pool:
                     results = pool.starmap(get_frame_data, args_list)
 
                 return pd.concat(results)
 
     except (FileNotFoundError, OSError):
         raise Exception("Error accessing .hdf5 file")
```

### Comparing `odb-plotter-0.5.3/src/odbp/state.py` & `odb-plotter-0.5.4/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.3/src/odbp/util.py` & `odb-plotter-0.5.4/src/odbp/util.py`

 * *Files identical despite different names*

