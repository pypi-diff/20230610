# Comparing `tmp/python_code_outline-0.1.6.tar.gz` & `tmp/python_code_outline-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_code_outline-0.1.6.tar", max compression
+gzip compressed data, was "python_code_outline-0.1.7.tar", max compression
```

## Comparing `python_code_outline-0.1.6.tar` & `python_code_outline-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.6/LICENSE
--rw-r--r--   0        0        0     5875 2023-06-08 08:08:25.199602 python_code_outline-0.1.6/README.md
--rw-r--r--   0        0        0      581 2023-06-08 08:38:41.587386 python_code_outline-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      155 2023-06-05 06:37:21.617890 python_code_outline-0.1.6/python_code_outline/__init__.py
--rw-r--r--   0        0        0     5505 2023-06-08 08:35:39.928287 python_code_outline-0.1.6/python_code_outline/python_report_generator.py
--rw-r--r--   0        0        0     6498 1970-01-01 00:00:00.000000 python_code_outline-0.1.6/setup.py
--rw-r--r--   0        0        0     6162 1970-01-01 00:00:00.000000 python_code_outline-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5862 2023-06-08 08:42:20.090459 python_code_outline-0.1.7/README.md
+-rw-r--r--   0        0        0      581 2023-06-10 07:50:28.984205 python_code_outline-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-06-10 07:46:56.328447 python_code_outline-0.1.7/python_code_outline/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:50:00.560611 python_code_outline-0.1.7/python_code_outline/py.typed
+-rw-r--r--   0        0        0     5505 2023-06-08 08:35:39.928287 python_code_outline-0.1.7/python_code_outline/python_report_generator.py
+-rw-r--r--   0        0        0     6149 1970-01-01 00:00:00.000000 python_code_outline-0.1.7/PKG-INFO
```

### Comparing `python_code_outline-0.1.6/LICENSE` & `python_code_outline-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_code_outline-0.1.6/README.md` & `python_code_outline-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage as a pip module
 
 After installing the package via pip, you can import and use the functionality in your own code as well. For example:
 
 ```python
 """ Generate a report of the python code outline of a folder. """
-from python_code_outline import python_report_generator
+from python_code_outline import get_report
 
 # Define the root folder
 ROOT_FOLDER = "/path/to/folder"
 
 # Specify the report and ignore file paths (optional)
 REPORT_FILE_PATH = "custom_report.txt"
 IGNORE_FILE_PATH = "/path/to/folder/.gitignore"
```

### Comparing `python_code_outline-0.1.6/python_code_outline/python_report_generator.py` & `python_code_outline-0.1.7/python_code_outline/python_report_generator.py`

 * *Files identical despite different names*

### Comparing `python_code_outline-0.1.6/setup.py` & `python_code_outline-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,165 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-code-outline
+Version: 0.1.7
+Summary: Takes a folder path and outputs a text outline of the code, supports ignore files.
+Author: Sean Dearnaley
+Author-email: SeanDearnaley@outlook.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['python_code_outline']
+# Python Code Structure Report Generator
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)
 
-setup_kwargs = {
-    'name': 'python-code-outline',
-    'version': '0.1.6',
-    'description': 'Takes a folder path and outputs a text outline of the code, supports ignore files.',
-    'long_description': '# Python Code Structure Report Generator\n\n[![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)\n\n![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)\n\nThis Python script generates a text-based report of the code structure for all Python files in a given folder. It\'s useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.\n\n[Example Report](example_report.txt?raw=true)\n\n## Usage\n\nTo use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.\n\n```bash\npython python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore\n```\n\nIf the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.\n\n```bash\npython python_report_generator.py /path/to/folder\n```\n\n## Usage as a pip module\n\nAfter installing the package via pip, you can import and use the functionality in your own code as well. For example:\n\n```python\n""" Generate a report of the python code outline of a folder. """\nfrom python_code_outline import python_report_generator\n\n# Define the root folder\nROOT_FOLDER = "/path/to/folder"\n\n# Specify the report and ignore file paths (optional)\nREPORT_FILE_PATH = "custom_report.txt"\nIGNORE_FILE_PATH = "/path/to/folder/.gitignore"\n\n# Generate the report\nREPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)\n\n# Write the report to a file\nwith open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:\n    file.write(REPORT)\n\nprint(f"Report generated successfully to {REPORT_FILE_PATH}.")\n```\n\nPlease replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.\n\n## Output\n\nThe script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.\n\n## Optional Parameters\n\n- `--report_file_path`: The name of the report file. Defaults to `report.txt` if not provided.\n- `--ignore_file_path`: The path to the ignore file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.\n\n## Requirements\n\nThis script requires Python 3.x to run.\n\n## Installation\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency management. To install the dependencies, first install Poetry by following the [official installation guide](https://python-poetry.org/docs/#installation), and then run the following command in the project directory:\n\n```bash\npoetry install\n```\n\nThis will create a virtual environment and install the required dependencies.\n\nYou can install this module using pip:\n\n```bash\npip install python-code-outline\n```\n\nor with poetry\n\n```bash\npoetry add python-code-outline\n```\n\nThis command will download the package from PyPI and install it in your current Python environment.\n\n## Running Tests\n\nThis project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:\n\n```bash\npoetry shell\n```\n\nThen, run the tests using the following command:\n\n```bash\npytest\n```\n\n## Checking Test Coverage\n\nThis project uses the `coverage` package to generate test coverage reports. Here\'s how to use it:\n\n1. First, you need to install the `coverage` package if it\'s not already installed.\n\n```bash\npip install coverage\n```\n\nor\n\n```bash\npoetry add coverage\n```\n\nIf you\'re using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.\n\n2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you\'re using `pytest` for testing, you can use the following command:\n\n```bash\ncoverage run -m pytest\n```\n\nThis command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.\n\n3. Once you\'ve collected coverage data, you can generate a report by running:\n\n```bash\ncoverage report\n```\n\nThis will print a coverage report to the terminal, showing the code coverage for each module in your project.\n\n4. If you want a more detailed view, you can generate an HTML report using:\n\n```bash\ncoverage html\n```\n\nThis will generate an `htmlcov` directory in your project directory. Inside this directory, you\'ll find an `index.html` file. You can open this file in a web browser to view a detailed coverage report that shows which lines of each file were covered by the tests.\n\n5. If you\'re finished checking coverage and want to clear the collected data, you can use the command:\n\n```bash\ncoverage erase\n```\n\nThis will delete the `.coverage` data file, clearing the collected coverage data.\n\nRemember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn\'t necessarily mean your testing is perfect. It\'s important to write meaningful tests and not just strive for high coverage percentages.',
-    'author': 'Sean Dearnaley',
-    'author_email': 'SeanDearnaley@outlook.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
+![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)
 
+This Python script generates a text-based report of the code structure for all Python files in a given folder. It's useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.
 
-setup(**setup_kwargs)
+[Example Report](example_report.txt?raw=true)
+
+## Usage
+
+To use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
+
+```bash
+python python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore
+```
+
+If the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.
+
+```bash
+python python_report_generator.py /path/to/folder
+```
+
+## Usage as a pip module
+
+After installing the package via pip, you can import and use the functionality in your own code as well. For example:
+
+```python
+""" Generate a report of the python code outline of a folder. """
+from python_code_outline import get_report
+
+# Define the root folder
+ROOT_FOLDER = "/path/to/folder"
+
+# Specify the report and ignore file paths (optional)
+REPORT_FILE_PATH = "custom_report.txt"
+IGNORE_FILE_PATH = "/path/to/folder/.gitignore"
+
+# Generate the report
+REPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)
+
+# Write the report to a file
+with open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:
+    file.write(REPORT)
+
+print(f"Report generated successfully to {REPORT_FILE_PATH}.")
+```
+
+Please replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.
+
+## Output
+
+The script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.
+
+## Optional Parameters
+
+- `--report_file_path`: The name of the report file. Defaults to `report.txt` if not provided.
+- `--ignore_file_path`: The path to the ignore file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
+
+## Requirements
+
+This script requires Python 3.x to run.
+
+## Installation
+
+This project uses [Poetry](https://python-poetry.org/) for dependency management. To install the dependencies, first install Poetry by following the [official installation guide](https://python-poetry.org/docs/#installation), and then run the following command in the project directory:
+
+```bash
+poetry install
+```
+
+This will create a virtual environment and install the required dependencies.
+
+You can install this module using pip:
+
+```bash
+pip install python-code-outline
+```
+
+or with poetry
+
+```bash
+poetry add python-code-outline
+```
+
+This command will download the package from PyPI and install it in your current Python environment.
+
+## Running Tests
+
+This project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:
+
+```bash
+poetry shell
+```
+
+Then, run the tests using the following command:
+
+```bash
+pytest
+```
+
+## Checking Test Coverage
+
+This project uses the `coverage` package to generate test coverage reports. Here's how to use it:
+
+1. First, you need to install the `coverage` package if it's not already installed.
+
+```bash
+pip install coverage
+```
+
+or
+
+```bash
+poetry add coverage
+```
+
+If you're using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.
+
+2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
+
+```bash
+coverage run -m pytest
+```
+
+This command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.
+
+3. Once you've collected coverage data, you can generate a report by running:
+
+```bash
+coverage report
+```
+
+This will print a coverage report to the terminal, showing the code coverage for each module in your project.
+
+4. If you want a more detailed view, you can generate an HTML report using:
+
+```bash
+coverage html
+```
+
+This will generate an `htmlcov` directory in your project directory. Inside this directory, you'll find an `index.html` file. You can open this file in a web browser to view a detailed coverage report that shows which lines of each file were covered by the tests.
+
+5. If you're finished checking coverage and want to clear the collected data, you can use the command:
+
+```bash
+coverage erase
+```
+
+This will delete the `.coverage` data file, clearing the collected coverage data.
+
+Remember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn't necessarily mean your testing is perfect. It's important to write meaningful tests and not just strive for high coverage percentages.
```

