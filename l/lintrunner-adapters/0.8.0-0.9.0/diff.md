# Comparing `tmp/lintrunner_adapters-0.8.0.tar.gz` & `tmp/lintrunner_adapters-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lintrunner_adapters-0.8.0.tar", max compression
+gzip compressed data, was "lintrunner_adapters-0.9.0.tar", max compression
```

## Comparing `lintrunner_adapters-0.8.0.tar` & `lintrunner_adapters-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     4389 2023-04-26 14:39:00.168660 lintrunner_adapters-0.8.0/LICENSE
--rw-r--r--   0        0        0     1984 2023-04-26 14:39:00.168660 lintrunner_adapters-0.8.0/README.md
--rw-r--r--   0        0        0      711 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/__init__.py
--rw-r--r--   0        0        0     1752 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/__main__.py
--rw-r--r--   0        0        0     3546 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/_common/lintrunner_common.py
--rw-r--r--   0        0        0     4097 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py
--rw-r--r--   0        0        0     5321 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_isort_linter.py
--rw-r--r--   0        0        0     4790 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_linter.py
--rw-r--r--   0        0        0     6348 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clangformat_linter.py
--rw-r--r--   0        0        0     7641 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clippy_linter.py
--rw-r--r--   0        0        0     3453 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/cmake_linter.py
--rw-r--r--   0        0        0     4374 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/django_upgrade_linter.py
--rw-r--r--   0        0        0     3140 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py
--rw-r--r--   0        0        0     1776 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/exec_linter.py
--rw-r--r--   0        0        0    10327 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/flake8_linter.py
--rw-r--r--   0        0        0     7062 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/grep_linter.py
--rw-r--r--   0        0        0     4269 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/isort_linter.py
--rw-r--r--   0        0        0     5933 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/mypy_linter.py
--rw-r--r--   0        0        0     4593 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/newlines_linter.py
--rw-r--r--   0        0        0     3369 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pip_init.py
--rw-r--r--   0        0        0     6048 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pylint_linter.py
--rw-r--r--   0        0        0     4532 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pyupgrade_linter.py
--rw-r--r--   0        0        0     4722 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/refurb_linter.py
--rw-r--r--   0        0        0     4144 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_fix_linter.py
--rw-r--r--   0        0        0     9672 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_linter.py
--rw-r--r--   0        0        0     7223 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/rustfmt_linter.py
--rw-r--r--   0        0        0     2305 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/shellcheck_linter.py
--rw-r--r--   0        0        0     3122 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ufmt_linter.py
--rw-r--r--   0        0        0     4060 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif.py
--rw-r--r--   0        0        0     6820 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif_test.py
--rw-r--r--   0        0        0     2413 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 lintrunner_adapters-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4389 2023-06-10 16:24:48.294050 lintrunner_adapters-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1984 2023-06-10 16:24:48.294050 lintrunner_adapters-0.9.0/README.md
+-rw-r--r--   0        0        0      711 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/__init__.py
+-rw-r--r--   0        0        0     1752 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/__main__.py
+-rw-r--r--   0        0        0     3546 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/_common/lintrunner_common.py
+-rw-r--r--   0        0        0     4097 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py
+-rw-r--r--   0        0        0     5321 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/black_isort_linter.py
+-rw-r--r--   0        0        0     4790 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/black_linter.py
+-rw-r--r--   0        0        0     6348 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/clangformat_linter.py
+-rw-r--r--   0        0        0     7641 2023-06-10 16:24:48.298050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/clippy_linter.py
+-rw-r--r--   0        0        0     3453 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/cmake_linter.py
+-rw-r--r--   0        0        0     4374 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/django_upgrade_linter.py
+-rw-r--r--   0        0        0     3140 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py
+-rw-r--r--   0        0        0     1776 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/exec_linter.py
+-rw-r--r--   0        0        0    10327 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/flake8_linter.py
+-rw-r--r--   0        0        0     7062 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/grep_linter.py
+-rw-r--r--   0        0        0     4269 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/isort_linter.py
+-rw-r--r--   0        0        0     5933 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/mypy_linter.py
+-rw-r--r--   0        0        0     4593 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/newlines_linter.py
+-rw-r--r--   0        0        0     3369 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/pip_init.py
+-rw-r--r--   0        0        0     6048 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/pylint_linter.py
+-rw-r--r--   0        0        0     4532 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/pyupgrade_linter.py
+-rw-r--r--   0        0        0     4722 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/refurb_linter.py
+-rw-r--r--   0        0        0     4144 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/ruff_fix_linter.py
+-rw-r--r--   0        0        0     9672 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/ruff_linter.py
+-rw-r--r--   0        0        0     7223 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/rustfmt_linter.py
+-rw-r--r--   0        0        0     2305 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/shellcheck_linter.py
+-rw-r--r--   0        0        0     3974 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/toml_sort_linter.py
+-rw-r--r--   0        0        0     3122 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/ufmt_linter.py
+-rw-r--r--   0        0        0     4060 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/tools/convert_to_sarif.py
+-rw-r--r--   0        0        0     6820 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/lintrunner_adapters/tools/convert_to_sarif_test.py
+-rw-r--r--   0        0        0     2494 2023-06-10 16:24:48.302050 lintrunner_adapters-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 lintrunner_adapters-0.9.0/PKG-INFO
```

### Comparing `lintrunner_adapters-0.8.0/LICENSE` & `lintrunner_adapters-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/README.md` & `lintrunner_adapters-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/__init__.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/__main__.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/__main__.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/_common/lintrunner_common.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/_common/lintrunner_common.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_isort_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/black_isort_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/black_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clangformat_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/clangformat_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clippy_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/clippy_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/cmake_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/cmake_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/django_upgrade_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/django_upgrade_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/exec_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/exec_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/flake8_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/flake8_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/grep_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/grep_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/isort_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/isort_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/mypy_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/mypy_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/newlines_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/newlines_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pip_init.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/pip_init.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pylint_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/pylint_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pyupgrade_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/pyupgrade_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/refurb_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/refurb_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_fix_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/ruff_fix_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/ruff_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/rustfmt_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/rustfmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/shellcheck_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/shellcheck_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ufmt_linter.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/adapters/ufmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/tools/convert_to_sarif.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif_test.py` & `lintrunner_adapters-0.9.0/lintrunner_adapters/tools/convert_to_sarif_test.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.8.0/pyproject.toml` & `lintrunner_adapters-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,51 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+strict = true
+show_error_codes = true
+show_column_numbers = true
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "lintrunner_adapters.adapters.*"
+warn_unused_ignores = false
+
 [tool.poetry]
 name = "lintrunner-adapters"
-version = "0.8.0"
+version = "0.9.0"
 description = "Adapters and tools for lintrunner"
 authors = ["Justin Chu <justinchu@microsoft.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/justinchuby/lintrunner-adapters"
 keywords = ["lintrunner", "lint", "cli", "sarif", "linting", "ci", "linter", "flake8", "clippy", "ruff", "rustfmt", "github-code-scanning"]
 classifiers = [
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Quality Assurance",
 ]
-packages = [{ include = "lintrunner_adapters" }]
+packages = [{include = "lintrunner_adapters"}]
 include = ["LICENSE"]
 
-[tool.poetry.scripts]
-lintrunner_adapters = 'lintrunner_adapters.__main__:cli'
-
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
 lintrunner = "^0.10.0"
 pytest = "^7.2.0"
 types-pyyaml = "^6.0.12.2"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-addopts = "--doctest-modules"
-
-[tool.mypy]
-strict = true
-show_error_codes = true
-show_column_numbers = true
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "lintrunner_adapters.adapters.*"
-warn_unused_ignores = false
-
-[tool.isort]
-profile = "black"
+[tool.poetry.scripts]
+lintrunner_adapters = 'lintrunner_adapters.__main__:cli'
 
 [tool.pylint.messages_control]
 disable = [
     "duplicate-code",
     "fixme",
     "format",
     "import-error",
@@ -70,14 +67,17 @@
     "subprocess-run-check",
     "too-many-return-statements",
     "unnecessary-pass",
     "unused-argument",
     "unused-import",
 ]
 
+[tool.pytest.ini_options]
+addopts = "--doctest-modules"
+
 [tool.refurb]
 python_version = "3.7"
 disable = ["FURB101", "FURB150"] # disable suggestions using pathlib
 
 [tool.ruff]
 target-version = "py37"
 ignore-init-module-imports = true
@@ -112,7 +112,11 @@
     "D415",
     "E501",
 ]
 line-length = 120
 
 [tool.ruff.pydocstyle]
 convention = "google"
+
+[tool.tomlsort]
+spaces_indent_inline_array = 4
+trailing_comma_inline_array = true
```

### Comparing `lintrunner_adapters-0.8.0/PKG-INFO` & `lintrunner_adapters-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintrunner-adapters
-Version: 0.8.0
+Version: 0.9.0
 Summary: Adapters and tools for lintrunner
 Home-page: https://github.com/justinchuby/lintrunner-adapters
 License: MIT
 Keywords: lintrunner,lint,cli,sarif,linting,ci,linter,flake8,clippy,ruff,rustfmt,github-code-scanning
 Author: Justin Chu
 Author-email: justinchu@microsoft.com
 Requires-Python: >=3.7,<4.0
```

