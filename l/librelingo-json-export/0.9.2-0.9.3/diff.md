# Comparing `tmp/librelingo_json_export-0.9.2.tar.gz` & `tmp/librelingo_json_export-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librelingo_json_export-0.9.2.tar", max compression
+gzip compressed data, was "librelingo_json_export-0.9.3.tar", max compression
```

## Comparing `librelingo_json_export-0.9.2.tar` & `librelingo_json_export-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      542 2021-11-07 14:03:02.329040 librelingo_json_export-0.9.2/README.md
--rw-r--r--   0        0        0      172 2021-11-07 14:13:24.173259 librelingo_json_export-0.9.2/librelingo_json_export/__init__.py
--rw-r--r--   0        0        0     5735 2021-09-12 18:47:08.929519 librelingo_json_export-0.9.2/librelingo_json_export/challenge_types.py
--rw-r--r--   0        0        0     1768 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.2/librelingo_json_export/challenges.py
--rw-r--r--   0        0        0      986 2021-06-27 09:38:52.827621 librelingo_json_export-0.9.2/librelingo_json_export/cli.py
--rw-r--r--   0        0        0      605 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.2/librelingo_json_export/course.py
--rw-r--r--   0        0        0     1964 2021-11-07 13:57:31.566856 librelingo_json_export-0.9.2/librelingo_json_export/dictionary.py
--rw-r--r--   0        0        0     3413 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.2/librelingo_json_export/export.py
--rw-r--r--   0        0        0     1368 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.2/librelingo_json_export/module.py
--rw-r--r--   0        0        0      428 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.2/librelingo_json_export/skills.py
--rw-r--r--   0        0        0      860 2021-11-07 14:13:31.853312 librelingo_json_export-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1496 2021-11-07 14:16:28.177943 librelingo_json_export-0.9.2/setup.py
--rw-r--r--   0        0        0     1357 2021-11-07 14:16:28.178122 librelingo_json_export-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      950 2021-11-11 06:52:57.910271 librelingo_json_export-0.9.3/README.md
+-rw-r--r--   0        0        0      172 2021-11-11 06:58:08.044730 librelingo_json_export-0.9.3/librelingo_json_export/__init__.py
+-rw-r--r--   0        0        0     5735 2021-09-12 18:47:08.929519 librelingo_json_export-0.9.3/librelingo_json_export/challenge_types.py
+-rw-r--r--   0        0        0     1768 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.3/librelingo_json_export/challenges.py
+-rw-r--r--   0        0        0      978 2021-11-08 19:23:02.998071 librelingo_json_export-0.9.3/librelingo_json_export/cli.py
+-rw-r--r--   0        0        0      605 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.3/librelingo_json_export/course.py
+-rw-r--r--   0        0        0     1964 2021-11-08 19:11:56.486672 librelingo_json_export-0.9.3/librelingo_json_export/dictionary.py
+-rw-r--r--   0        0        0     3413 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.3/librelingo_json_export/export.py
+-rw-r--r--   0        0        0     1368 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.3/librelingo_json_export/module.py
+-rw-r--r--   0        0        0      428 2021-06-25 19:16:11.864076 librelingo_json_export-0.9.3/librelingo_json_export/skills.py
+-rw-r--r--   0        0        0      930 2021-11-11 06:57:58.034630 librelingo_json_export-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2044 2021-11-11 06:59:30.548827 librelingo_json_export-0.9.3/setup.py
+-rw-r--r--   0        0        0     1765 2021-11-11 06:59:30.549039 librelingo_json_export-0.9.3/PKG-INFO
```

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/challenge_types.py` & `librelingo_json_export-0.9.3/librelingo_json_export/challenge_types.py`

 * *Files identical despite different names*

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/challenges.py` & `librelingo_json_export-0.9.3/librelingo_json_export/challenges.py`

 * *Files identical despite different names*

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/cli.py` & `librelingo_json_export-0.9.3/librelingo_json_export/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         Path(output_path).mkdir(parents=True, exist_ok=True)
 
 
 @click.command()
 @click.argument("input_path")
 @click.argument("output_path")
 @click.option("--dry-run/--no-dry-run", default=DEFAULT_SETTINGS.dry_run)
-def _command(input_path, output_path, dry_run):
+def main(input_path, output_path, dry_run):
     """
     Convert a YAML course into JSON files to be consumed by the web app.
     """
     settings = Settings(
         dry_run=dry_run,
     )
     course = load_course(input_path)
     ensure_output_directory(output_path, settings)
     export_course(output_path, course, settings)
 
 
 if __name__ == "__main__":
-    _command()
+    main()
```

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/course.py` & `librelingo_json_export-0.9.3/librelingo_json_export/course.py`

 * *Files identical despite different names*

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/dictionary.py` & `librelingo_json_export-0.9.3/librelingo_json_export/dictionary.py`

 * *Files identical despite different names*

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/export.py` & `librelingo_json_export-0.9.3/librelingo_json_export/export.py`

 * *Files identical despite different names*

### Comparing `librelingo_json_export-0.9.2/librelingo_json_export/module.py` & `librelingo_json_export-0.9.3/librelingo_json_export/module.py`

 * *Files identical despite different names*

### Comparing `librelingo_json_export-0.9.2/pyproject.toml` & `librelingo_json_export-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "librelingo_json_export"
-version = "0.9.2"  # Do not edit before merge to 'main'
+version = "0.9.3"  # Do not edit before merge to 'main'
 description = "Export LibreLingo courses in the JSON format used by the web app"
 authors = ["Dániel Kántor <git@daniel-kantor.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
+[tool.poetry.scripts]
+export-cli = 'librelingo_json_export.cli:main'
+
 [tool.poetry.dependencies]
 python = "^3.8"
 librelingo-types = "^3.0.0"
 librelingo-utils = "^2.6.0"
 python-slugify = "^4.0.1"
 librelingo-yaml-loader = "^1.0.0"
 editdistance = "^0.6.0"
```

### Comparing `librelingo_json_export-0.9.2/setup.py` & `librelingo_json_export-0.9.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,26 +13,30 @@
  'librelingo-utils>=2.6.0,<3.0.0',
  'librelingo-yaml-loader>=1.0.0,<2.0.0',
  'python-slugify>=4.0.1,<5.0.0']
 
 extras_require = \
 {'hunspell': ['hunspell>=0.5.5,<0.6.0']}
 
+entry_points = \
+{'console_scripts': ['export-cli = librelingo_json_export.cli:main']}
+
 setup_kwargs = {
     'name': 'librelingo-json-export',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Export LibreLingo courses in the JSON format used by the web app',
-    'long_description': '<a name="librelingo_json_export.export"></a>\n# librelingo\\_json\\_export.export\n\n<a name="librelingo_json_export.export.export_course"></a>\n#### export\\_course\n\n```python\nexport_course(export_path, course, settings=None)\n```\n\nWrites the course to JSON files in the specified path.\n\n### Usage example:\n\n```python\nfrom librelingo_yaml_loader import load_course\nfrom librelingo_json_export.export import export_course\n\ncourse = load_course("./courses/french-from-english")\nexport_course("./apps/web/src/courses/french-from-english", course)\n```\n\n',
+    'long_description': '<a name="librelingo_json_export.export"></a>\n# librelingo\\_json\\_export.export\n\n<a name="librelingo_json_export.export.export_course"></a>\n#### export\\_course\n\n```python\nexport_course(export_path, course, settings=None)\n```\n\nWrites the course to JSON files in the specified path.\n\n### Usage example:\n\n```python\nfrom librelingo_yaml_loader import load_course\nfrom librelingo_json_export.export import export_course\n\ncourse = load_course("./courses/french-from-english")\nexport_course("./apps/web/src/courses/french-from-english", course)\n```\n\n<a name="librelingo_json_export.cli"></a>\n# librelingo\\_json\\_export.cli\n\n<a name="librelingo_json_export.cli.main"></a>\n#### main\n\n```python\n@click.command()\n@click.argument("input_path")\n@click.argument("output_path")\n@click.option("--dry-run/--no-dry-run", default=DEFAULT_SETTINGS.dry_run)\nmain(input_path, output_path, dry_run)\n```\n\nConvert a YAML course into JSON files to be consumed by the web app.\n\n',
     'author': 'Dániel Kántor',
     'author_email': 'git@daniel-kantor.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `librelingo_json_export-0.9.2/PKG-INFO` & `librelingo_json_export-0.9.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librelingo-json-export
-Version: 0.9.2
+Version: 0.9.3
 Summary: Export LibreLingo courses in the JSON format used by the web app
 License: AGPLv3
 Author: Dániel Kántor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -37,8 +37,24 @@
 from librelingo_yaml_loader import load_course
 from librelingo_json_export.export import export_course
 
 course = load_course("./courses/french-from-english")
 export_course("./apps/web/src/courses/french-from-english", course)
 ```
 
+<a name="librelingo_json_export.cli"></a>
+# librelingo\_json\_export.cli
+
+<a name="librelingo_json_export.cli.main"></a>
+#### main
+
+```python
+@click.command()
+@click.argument("input_path")
+@click.argument("output_path")
+@click.option("--dry-run/--no-dry-run", default=DEFAULT_SETTINGS.dry_run)
+main(input_path, output_path, dry_run)
+```
+
+Convert a YAML course into JSON files to be consumed by the web app.
+
```

