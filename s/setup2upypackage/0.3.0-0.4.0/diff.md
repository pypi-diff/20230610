# Comparing `tmp/setup2upypackage-0.3.0.tar.gz` & `tmp/setup2upypackage-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup2upypackage-0.3.0.tar", last modified: Sat May 27 14:18:28 2023, max compression
+gzip compressed data, was "setup2upypackage-0.4.0.tar", last modified: Sat Jun 10 09:26:00 2023, max compression
```

## Comparing `setup2upypackage-0.3.0.tar` & `setup2upypackage-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:18:28.342606 setup2upypackage-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-27 14:18:28.342606 setup2upypackage-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 14:18:28.342606 setup2upypackage-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:18:28.334605 setup2upypackage-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:18:28.338605 setup2upypackage-0.3.0/src/setup2upypackage/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/src/setup2upypackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/src/setup2upypackage/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/src/setup2upypackage/setup2upypackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-27 14:18:20.000000 setup2upypackage-0.3.0/src/setup2upypackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:18:28.342606 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-27 14:18:28.000000 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-27 14:18:28.000000 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 14:18:28.000000 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-27 14:18:28.000000 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-27 14:18:28.000000 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 14:18:28.000000 setup2upypackage-0.3.0/src/setup2upypackage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:18:28.342606 setup2upypackage-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/tests/test_absolute_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-27 14:18:08.000000 setup2upypackage-0.3.0/tests/test_setup2upypackage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/src/setup2upypackage/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/src/setup2upypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/src/setup2upypackage/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/src/setup2upypackage/setup2upypackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-10 09:25:53.000000 setup2upypackage-0.4.0/src/setup2upypackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/tests/test_absolute_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/tests/test_setup2upypackage.py
```

### Comparing `setup2upypackage-0.3.0/LICENSE.txt` & `setup2upypackage-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.3.0/PKG-INFO` & `setup2upypackage-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.3.0
+Version: 0.4.0
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
@@ -124,15 +124,16 @@
     --validate
 ```
 
 #### Options
 
 To not take the version or the dependencies specified in the `package.json`
 file during a validation run, use the `--ignore-version` or `--ignore-deps`
-argument.
+argument. Additionally added `boot.py` and `main.py` files in `package.json`
+can be ignored using `--ignore-boot-main` during a validation run.
 
 ### Create
 #### Create package JSON file
 
 The following command creates a `package.json` file in the same directory as
 the specified `setup.py` file. The content of the `package.json` file is
 additionally printed to stdout (`--print`) with an indentation of 4 (due to
```

### Comparing `setup2upypackage-0.3.0/README.md` & `setup2upypackage-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,16 @@
     --validate
 ```
 
 #### Options
 
 To not take the version or the dependencies specified in the `package.json`
 file during a validation run, use the `--ignore-version` or `--ignore-deps`
-argument.
+argument. Additionally added `boot.py` and `main.py` files in `package.json`
+can be ignored using `--ignore-boot-main` during a validation run.
 
 ### Create
 #### Create package JSON file
 
 The following command creates a `package.json` file in the same directory as
 the specified `setup.py` file. The content of the `package.json` file is
 additionally printed to stdout (`--print`) with an indentation of 4 (due to
```

### Comparing `setup2upypackage-0.3.0/setup.py` & `setup2upypackage-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.3.0/src/setup2upypackage/main.py` & `setup2upypackage-0.4.0/src/setup2upypackage/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,20 @@
 
     parser.add_argument('--ignore-deps',
                         dest='ignore_deps',
                         action='store_true',
                         required=False,
                         help='Exclude dependencies from check')
 
+    parser.add_argument('--ignore-boot-main',
+                        dest='ignore_boot_main',
+                        action='store_true',
+                        required=False,
+                        help='Boot and main files from check')
+
     parser.add_argument('--print',
                         dest='print_result',
                         required=False,
                         action='store_true',
                         help='Print parsed setup.py as JSON to stdout')
 
     parser.add_argument('--pretty',
@@ -151,27 +157,29 @@
     package_changelog_file = args.package_changelog_file
     do_validate = args.do_validate
     dump_to_file = args.dump_to_file
     print_result = args.print_result
     pretty_output = args.pretty_output
     ignore_version = args.ignore_version
     ignore_deps = args.ignore_deps
+    ignore_boot_main = args.ignore_boot_main
 
     setup_2_upy_package = Setup2uPyPackage(
         setup_file=setup_file,
         package_file=package_file,
         package_changelog_file=package_changelog_file,
         logger=logger)
 
     package_data = setup_2_upy_package.package_data
 
     if do_validate:
         validation_result = setup_2_upy_package.validate(
             ignore_version=ignore_version,
-            ignore_deps=ignore_deps)
+            ignore_deps=ignore_deps,
+            ignore_boot_main=ignore_boot_main)
 
         if validation_result is False:
             diff = setup_2_upy_package.validation_diff
 
             if pretty_output:
                 stdout.write(json.dumps(diff, indent=4))
             else:
```

### Comparing `setup2upypackage-0.3.0/src/setup2upypackage/setup2upypackage.py` & `setup2upypackage-0.4.0/src/setup2upypackage/setup2upypackage.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import json
 import logging
 import sys
 from distutils.core import run_setup
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from changelog2version.extract_version import ExtractVersion
 from deepdiff import DeepDiff
 from mock import Mock
 
 
 class Setup2uPyPackageError(Exception):
@@ -304,43 +304,77 @@
         else:
             raise Setup2uPyPackageError("No package.json data specified")
 
         return existing_data
 
     def validate(self,
                  ignore_version: bool = False,
-                 ignore_deps: bool = False) -> bool:
+                 ignore_deps: bool = False,
+                 ignore_boot_main: bool = False) -> bool:
         """
         Validate existing package.json with setup.py based data
 
-        :param      ignore_version:  Indicates if the version is ignored
-        :type       ignore_version:  bool
-        :param      ignore_deps:     Indicates if the dependencies are ignored
-        :type       ignore_deps:     bool
+        :param      ignore_version:     Flag to ignore the version
+        :type       ignore_version:     bool
+        :param      ignore_deps:        Flag to ignore the dependencies
+        :type       ignore_deps:        bool
+        :param      ignore_boot_main:   Flag to ignore the main and boot files
+        :type       ignore_boot_main:   bool
 
         :returns:   Result of validation, True on success, False otherwise
         :rtype:     bool
         """
         # list of URL entries might be sorted differently
         package_json_data = dict(self.package_json_data)
         package_data = dict(self.package_data)
 
         if ignore_version:
-            package_json_data.pop("version")
-            package_data.pop("version")
+            package_json_data.pop("version", None)
+            package_data.pop("version", None)
 
         if ignore_deps:
-            package_json_data.pop("deps")
-            package_data.pop("deps")
+            package_json_data.pop("deps", None)
+            package_data.pop("deps", None)
+
+        if ignore_boot_main:
+            package_json_data["urls"] = self._exclude_package_files(
+                package_files=package_json_data.get("urls")
+            )
+
+            package_data["urls"] = self._exclude_package_files(
+                package_files=package_data.get("urls")
+            )
 
         package_json_data.get("urls", []).sort()
         package_data.get("urls", []).sort()
 
         return package_json_data == package_data
 
+    def _exclude_package_files(
+            self,
+            package_files: List[Tuple[str, str]],
+            excludes: List[str] = [
+                "boot.py", "main.py"
+            ]) -> List[Tuple[str, str]]:
+        """
+        Exclude elements of a list if the first element matches an exclude str
+
+        :param      package_files:  The package files
+        :type       package_files:  List[Tuple[str, str]]
+        :param      excludes:       The list of excludes
+        :type       excludes:       List[str]
+
+        :returns:   List without elements matching the exclude list
+        :rtype:     List[Tuple[str, str]]
+        """
+        return [
+            ele for ele in package_files
+            if not any(i in ele[0] for i in excludes)
+        ]
+
     @property
     def validation_diff(self) -> DeepDiff:
         """
         Get difference of package.json and setup.py
 
         :returns:   The deep difference.
         :rtype:     DeepDiff
```

### Comparing `setup2upypackage-0.3.0/src/setup2upypackage.egg-info/PKG-INFO` & `setup2upypackage-0.4.0/src/setup2upypackage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.3.0
+Version: 0.4.0
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
@@ -124,15 +124,16 @@
     --validate
 ```
 
 #### Options
 
 To not take the version or the dependencies specified in the `package.json`
 file during a validation run, use the `--ignore-version` or `--ignore-deps`
-argument.
+argument. Additionally added `boot.py` and `main.py` files in `package.json`
+can be ignored using `--ignore-boot-main` during a validation run.
 
 ### Create
 #### Create package JSON file
 
 The following command creates a `package.json` file in the same directory as
 the specified `setup.py` file. The content of the `package.json` file is
 additionally printed to stdout (`--print`) with an indentation of 4 (due to
```

### Comparing `setup2upypackage-0.3.0/src/setup2upypackage.egg-info/SOURCES.txt` & `setup2upypackage-0.4.0/src/setup2upypackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.3.0/tests/test_absolute_truth.py` & `setup2upypackage-0.4.0/tests/test_absolute_truth.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.3.0/tests/test_setup2upypackage.py` & `setup2upypackage-0.4.0/tests/test_setup2upypackage.py`

 * *Files 8% similar despite different names*

```diff
@@ -351,14 +351,76 @@
             patched.return_value = diff_deps_package_json_data
             is_valid = s2pp.validate(ignore_deps=True)
             if is_valid:
                 self.assertTrue(is_valid)
             else:
                 self.test_logger.warning(s2pp.validation_diff)
 
+        # check for main and/or boot entries
+        diff_urls_package_json_data = dict(s2pp.package_json_data)
+        diff_urls_package_json_data.get("urls").append([
+            "boot.py",
+            "github:brainelectronics/micropython-package-validation/boot.py"
+        ])
+        diff_urls_package_json_data.get("urls").append([
+            "asdf/main.py",
+            "github:brainelectronics/micropython-package-validation/main.py"
+        ])
+        self.assertNotEqual(
+            diff_urls_package_json_data["urls"],
+            s2pp.package_json_data
+        )
+        self.assertTrue(
+            all(isinstance(ele, list)
+                for ele in diff_urls_package_json_data.get("urls"))
+        )
+
+        with patch('setup2upypackage.setup2upypackage.Setup2uPyPackage.package_json_data', new_callable=PropertyMock) as patched:     # noqa: E501
+            patched.return_value = diff_urls_package_json_data
+            is_valid = s2pp.validate(ignore_boot_main=True)
+            if is_valid:
+                self.assertTrue(is_valid)
+            else:
+                self.test_logger.warning(s2pp.validation_diff)
+
+    def test__exclude_package_files(self) -> None:
+        """Test excluding package files from list of package files"""
+        package = [
+            [
+                "main.py",
+                "github:brainelectronics/micropython-package-validation/main.py"    # noqa: E501
+            ],
+            [
+                "other_dir/bar.py",
+                "github:brainelectronics/micropython-package-validation/other_dir/bar.py"   # noqa: E501
+            ],
+            [
+                "some/foo.py",
+                "github:brainelectronics/micropython-package-validation/some/foo.py"   # noqa: E501
+            ],
+        ]
+
+        result = self.s2pp._exclude_package_files(package_files=package)
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 2)
+        for ele in result:
+            self.assertEqual(len(ele), 2)
+        self.assertEqual(result, package[1:])
+
+        # use non default exclude list
+        result = self.s2pp._exclude_package_files(
+            package_files=package,
+            excludes=["some/foo.py"]
+        )
+        self.assertIsInstance(result, list)
+        self.assertEqual(len(result), 2)
+        for ele in result:
+            self.assertEqual(len(ele), 2)
+        self.assertEqual(result, package[:-1])
+
     @unittest.skip("Not yet implemented")
     def test_validation_diff(self) -> None:
         """Test validation difference property"""
         pass
 
     @params(
         ("asdf.json", False),   # path, pretty
```

