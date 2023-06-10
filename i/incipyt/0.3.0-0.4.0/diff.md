# Comparing `tmp/incipyt-0.3.0.tar.gz` & `tmp/incipyt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incipyt-0.3.0.tar", last modified: Sun Apr  9 13:14:49 2023, max compression
+gzip compressed data, was "incipyt-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `incipyt-0.3.0.tar` & `incipyt-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,60 @@
--rw-r--r--   0        0        0      335 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1576 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1552 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/workflows/release-please.yml
--rw-r--r--   0        0        0     2241 2023-04-09 13:14:29.363232 incipyt-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1826 2023-04-09 13:14:29.363232 incipyt-0.3.0/.gitignore
--rw-r--r--   0        0        0     1192 2023-04-09 13:14:29.363232 incipyt-0.3.0/.gitmessage
--rw-r--r--   0        0        0      803 2023-04-09 13:14:29.363232 incipyt-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5709 2023-04-09 13:14:29.363232 incipyt-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2023-04-09 13:14:29.363232 incipyt-0.3.0/LICENSE
--rw-r--r--   0        0        0     2065 2023-04-09 13:14:29.363232 incipyt-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/__init__.py
--rw-r--r--   0        0        0     5484 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/__main__.py
--rw-r--r--   0        0        0        0 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/__init__.py
--rw-r--r--   0        0        0     2056 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/dumpers.py
--rw-r--r--   0        0        0      414 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/sanitizers.py
--rw-r--r--   0        0        0    15570 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/templates.py
--rw-r--r--   0        0        0     2900 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/_internal/utils.py
--rw-r--r--   0        0        0     4746 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/commands.py
--rw-r--r--   0        0        0    10044 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/project.py
--rw-r--r--   0        0        0      240 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/signals.py
--rw-r--r--   0        0        0       40 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/README.md
--rw-r--r--   0        0        0     9132 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/Apache-2.0.txt
--rw-r--r--   0        0        0     1268 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/BSD-2-Clause.txt
--rw-r--r--   0        0        0     1460 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/BSD-3-Clause.txt
--rw-r--r--   0        0        0    16375 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/CDDL-1.0.txt
--rw-r--r--   0        0        0       45 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/Copyright.txt
--rw-r--r--   0        0        0    14134 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/EPL-2.0.txt
--rw-r--r--   0        0        0    17669 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/GPL-2.0.txt
--rw-r--r--   0        0        0    34438 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/GPL-3.0.txt
--rw-r--r--   0        0        0    24942 2023-04-09 13:14:29.363232 incipyt-0.3.0/incipyt/templates/licenses/LGPL-2.0.txt
--rw-r--r--   0        0        0    25972 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/LGPL-2.1.txt
--rw-r--r--   0        0        0     7441 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/LGPL-3.0.txt
--rw-r--r--   0        0        0     1055 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/MIT.txt
--rw-r--r--   0        0        0    14944 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/licenses/MPL-2.0.txt
--rw-r--r--   0        0        0     1826 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/python.gitignore
--rw-r--r--   0        0        0        0 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/templates/{PROJECT_NAME}/__init__.py
--rw-r--r--   0        0        0      250 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/__init__.py
--rw-r--r--   0        0        0      673 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/base.py
--rw-r--r--   0        0        0     2646 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/git.py
--rw-r--r--   0        0        0     1703 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/license.py
--rw-r--r--   0        0        0      234 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/__init__.py
--rw-r--r--   0        0        0     4541 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/base.py
--rw-r--r--   0        0        0     1093 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/flit.py
--rw-r--r--   0        0        0     1093 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/hatch.py
--rw-r--r--   0        0        0     1083 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/pdm.py
--rw-r--r--   0        0        0     1049 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/pep517/setuptools.py
--rw-r--r--   0        0        0     5031 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/poetry.py
--rw-r--r--   0        0        0      733 2023-04-09 13:14:29.367232 incipyt-0.3.0/incipyt/tools/venv.py
--rw-r--r--   0        0        0     2407 2023-04-09 13:14:29.367232 incipyt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2822 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_dumpers.py
--rw-r--r--   0        0        0     5311 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_project.py
--rw-r--r--   0        0        0     3437 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_renderers.py
--rw-r--r--   0        0        0     8212 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_templates.py
--rw-r--r--   0        0        0      411 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0      262 2023-04-09 13:14:29.367232 incipyt-0.3.0/tests/utils.py
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 incipyt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-06-10 13:12:01.902812 incipyt-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1576 2023-06-10 13:12:01.902812 incipyt-0.4.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1560 2023-06-10 13:12:01.902812 incipyt-0.4.0/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0     2258 2023-06-10 13:12:01.902812 incipyt-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1826 2023-06-10 13:12:01.902812 incipyt-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1192 2023-06-10 13:12:01.902812 incipyt-0.4.0/.gitmessage
+-rw-r--r--   0        0        0      803 2023-06-10 13:12:01.902812 incipyt-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8689 2023-06-10 13:12:01.902812 incipyt-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2023-06-10 13:12:01.902812 incipyt-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2106 2023-06-10 13:12:01.902812 incipyt-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/__init__.py
+-rw-r--r--   0        0        0     8500 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/_internal/__init__.py
+-rw-r--r--   0        0        0     2072 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/_internal/dumpers.py
+-rw-r--r--   0        0        0      414 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/_internal/sanitizers.py
+-rw-r--r--   0        0        0    13847 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/_internal/templates.py
+-rw-r--r--   0        0        0     3413 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/_internal/utils.py
+-rw-r--r--   0        0        0     4722 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/commands.py
+-rw-r--r--   0        0        0      104 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/project/__init__.py
+-rw-r--r--   0        0        0     5587 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/project/environment.py
+-rw-r--r--   0        0        0     3322 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/project/meta_variables.py
+-rw-r--r--   0        0        0     5820 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/project/structure.py
+-rw-r--r--   0        0        0      240 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/signals.py
+-rw-r--r--   0        0        0       40 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/README.md
+-rw-r--r--   0        0        0     9132 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/Apache-2.0.txt
+-rw-r--r--   0        0        0     1268 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/BSD-2-Clause.txt
+-rw-r--r--   0        0        0     1460 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/BSD-3-Clause.txt
+-rw-r--r--   0        0        0    16375 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/CDDL-1.0.txt
+-rw-r--r--   0        0        0       45 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/Copyright.txt
+-rw-r--r--   0        0        0    14134 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/EPL-2.0.txt
+-rw-r--r--   0        0        0    17669 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/GPL-2.0.txt
+-rw-r--r--   0        0        0    34438 2023-06-10 13:12:01.902812 incipyt-0.4.0/incipyt/templates/licenses/GPL-3.0.txt
+-rw-r--r--   0        0        0    24942 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/licenses/LGPL-2.0.txt
+-rw-r--r--   0        0        0    25972 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/licenses/LGPL-2.1.txt
+-rw-r--r--   0        0        0     7441 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/licenses/LGPL-3.0.txt
+-rw-r--r--   0        0        0     1055 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/licenses/MIT.txt
+-rw-r--r--   0        0        0    14944 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/licenses/MPL-2.0.txt
+-rw-r--r--   0        0        0     1826 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/python.gitignore
+-rw-r--r--   0        0        0        0 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/templates/{PROJECT_NAME}/__init__.py
+-rw-r--r--   0        0        0      250 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/base.py
+-rw-r--r--   0        0        0     2749 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/git.py
+-rw-r--r--   0        0        0     1703 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/license.py
+-rw-r--r--   0        0        0      234 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/pep517/__init__.py
+-rw-r--r--   0        0        0     4105 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/pep517/base.py
+-rw-r--r--   0        0        0     1107 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/pep517/flit.py
+-rw-r--r--   0        0        0     1107 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/pep517/hatch.py
+-rw-r--r--   0        0        0     1097 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/pep517/pdm.py
+-rw-r--r--   0        0        0     1049 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/pep517/setuptools.py
+-rw-r--r--   0        0        0     4759 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/poetry.py
+-rw-r--r--   0        0        0      835 2023-06-10 13:12:01.906813 incipyt-0.4.0/incipyt/tools/venv.py
+-rw-r--r--   0        0        0     2516 2023-06-10 13:12:01.906813 incipyt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2791 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/test_dumpers.py
+-rw-r--r--   0        0        0     4376 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/test_project.py
+-rw-r--r--   0        0        0     5294 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/test_renderers.py
+-rw-r--r--   0        0        0    11733 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/test_templates.py
+-rw-r--r--   0        0        0      411 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0      262 2023-06-10 13:12:01.906813 incipyt-0.4.0/tests/utils.py
+-rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 incipyt-0.4.0/PKG-INFO
```

### Comparing `incipyt-0.3.0/.github/workflows/pre-commit.yml` & `incipyt-0.4.0/.github/workflows/pre-commit.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     - cron: 13 2 * * 0 # weekly
 
 jobs:
   update:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v3.5.0
+        uses: actions/checkout@v3.5.2
       - name: Set up Python
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.1
         with:
           cache: pip
           cache-dependency-path: pyproject.toml
           check-latest: true
           python-version: 3.11
       - name: Install deps
         env:
@@ -34,15 +34,15 @@
         with:
           key: ${{ hashFiles('.pre-commit-config.yaml') }}
           path: ~/.cache/pre-commit
       - name: Update pre-commit cache if needed
         if: ${{ ! steps.cache-pre-commit.outputs.cache-hit }}
         run: pre-commit install-hooks
       - name: Open dependabot-like PR
-        uses: peter-evans/create-pull-request@v5.0.0
+        uses: peter-evans/create-pull-request@v5.0.1
         with:
           author: "GitHub <noreply@github.com>"
           base: ${{ github.ref_name }}
           branch: dependabot/pre-commit/${{ github.ref_name }}
           committer: "GitHub <noreply@github.com>"
           commit-message: "chore(dev): bump pre-commit hooks"
           labels: |
```

### Comparing `incipyt-0.3.0/.github/workflows/release-please.yml` & `incipyt-0.4.0/.github/workflows/release-please.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,26 +9,26 @@
     branches: [main]
 
 jobs:
   release-please:
     name: Release Please
     runs-on: ubuntu-latest
     steps:
-      - uses: GoogleCloudPlatform/release-please-action@v3.7.6
+      - uses: GoogleCloudPlatform/release-please-action@v3.7.9
         id: release
         with:
-          token: ${{ secrets.GITHUB_TOKEN }}
+          bump-minor-pre-major: true
+          bump-patch-for-minor-pre-major: true
           release-type: python
-          default-branch: main
       - name: Checkout
         if: ${{ steps.release.outputs.release_created }}
-        uses: actions/checkout@v3.5.0
+        uses: actions/checkout@v3.5.2
       - name: Set up Python
         if: ${{ steps.release.outputs.release_created }}
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.1
         with:
           cache: pip
           cache-dependency-path: pyproject.toml
           check-latest: true
           python-version: 3.11
       - name: Cache python env
         if: ${{ steps.release.outputs.release_created }}
```

### Comparing `incipyt-0.3.0/.github/workflows/test.yml` & `incipyt-0.4.0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,17 @@
   lint:
     name: Pre-commit (include linter)
     runs-on: ubuntu-latest
     if: github.event.pull_request.draft == false
 
     steps:
     - name: Checkout
-      uses: actions/checkout@v3.5.0
+      uses: actions/checkout@v3.5.2
     - name: Set up Python
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.1
       with:
         cache: pip
         cache-dependency-path: pyproject.toml
         check-latest: true
         python-version: 3.11
     - name: Install deps
       env:
@@ -45,36 +45,37 @@
 
   test:
     name: Tests
     needs: lint
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
       fail-fast: false
     runs-on: ${{ matrix.os }}
     env:
       _OS: ${{ matrix.os }}
       _PY: ${{ matrix.python-version }}
 
     steps:
     - name: Checkout
-      uses: actions/checkout@v3.5.0
+      uses: actions/checkout@v3.5.2
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.1
       with:
         cache: pip
         cache-dependency-path: pyproject.toml
         check-latest: true
         python-version: ${{ matrix.python-version }}
     - name: Install deps
       env:
         PIP_UPGRADE: True
         PIP_UPGRADE_STRATEGY: eager
       run: python -m pip install -e ".[test]"
     - name: Run tests with pytest
       run: pytest -v --cov=incipyt --cov-report=xml
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3.1.1
+      uses: codecov/codecov-action@v3.1.4
       with:
         fail_ci_if_error: true
         env_vars: _OS,_PY
+        version: v0.4.1
```

### Comparing `incipyt-0.3.0/.gitignore` & `incipyt-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/.gitmessage` & `incipyt-0.4.0/.gitmessage`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/.pre-commit-config.yaml` & `incipyt-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/CHANGELOG.md` & `incipyt-0.4.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,45 @@
 # Changelog
 
+## [0.4.0](https://github.com/NotANameServer/incipyt/compare/v0.3.0...v0.4.0) (2023-06-10)
+
+
+### ⚠ BREAKING CHANGES
+
+* bump python to 3.8
+
+### Features
+
+* config file ([83b36a2](https://github.com/NotANameServer/incipyt/commit/83b36a2416c2786d5734e2c1fa306e6c97265559))
+* metadata system ([14e761f](https://github.com/NotANameServer/incipyt/commit/14e761f6a5de8dc2710daf0947abec8dcedaee14))
+* **metadata:** implement a declarative metadata system for environment variables ([868e85a](https://github.com/NotANameServer/incipyt/commit/868e85af19ce6136a14f57b13894e7f2002e851f))
+* **metadata:** metadata field do_not_prompt to bypass prompting ([619c9b7](https://github.com/NotANameServer/incipyt/commit/619c9b776977471f24f9c52b247bf931bc679dea))
+* **metadata:** metadata field required and purging mechanism for template ([f7261ca](https://github.com/NotANameServer/incipyt/commit/f7261ca7a1b37dc1830870ffb3acd32fd7497d57))
+* **metadata:** stage control on metadata setter ([9b9b097](https://github.com/NotANameServer/incipyt/commit/9b9b097bfd18d099292caeff2db3364da0e900d7))
+* split project.py in multiple files ([03cf0e2](https://github.com/NotANameServer/incipyt/commit/03cf0e2d09997659ca9be28ccc34d6656260b577))
+* use project.environ to store additional options ([f8e8a6a](https://github.com/NotANameServer/incipyt/commit/f8e8a6a7e68f7a356a55b04b0202b3a3a91e6587))
+
+
+### Bug Fixes
+
+* **build:** add min_version for dependency slots ([e972377](https://github.com/NotANameServer/incipyt/commit/e972377aebcd661e9ac2f7dab6bcda92cd54e2ce))
+* **build:** add required metadata for mandatory fields for poetry builder ([b34cce2](https://github.com/NotANameServer/incipyt/commit/b34cce20a1c289440d061873b42960d2bbde6aa5))
+* **build:** remove unused **kwargs in __init__ and explicit check_build parameter ([1b91c65](https://github.com/NotANameServer/incipyt/commit/1b91c659e1470d83e0e9d46c3622447c6b3a3256))
+* bumps toml to tomli_w for dumpers.Toml ([9fe71ce](https://github.com/NotANameServer/incipyt/commit/9fe71cebf310703f92520f5ed619e232aa735fc2))
+* **main:** don't drop args[0] when importing ([665b5a4](https://github.com/NotANameServer/incipyt/commit/665b5a463ebeebd27d97e82cf7ca27cf568d6209))
+* **README:** mix tabs and spaces ([9c153c9](https://github.com/NotANameServer/incipyt/commit/9c153c987c885e6c4c4386e6f64f3c9166fbcb79))
+* replace |= operator by update function for UserDict based class ([7aa6ab7](https://github.com/NotANameServer/incipyt/commit/7aa6ab70fedee3e5120d2aefd95bf36d2f5cd0da))
+* use a list instead of a set when parsing string patterns ([e688458](https://github.com/NotANameServer/incipyt/commit/e68845872b21afc69485054372abd5adeb3921ec))
+* **venv:** use an hidden option as virtual env folder name ([5cbfd3f](https://github.com/NotANameServer/incipyt/commit/5cbfd3f00084b73d8e36b34b48e53aa31e33e3c2))
+
+
+### Miscellaneous Chores
+
+* bump python to 3.8 ([2120661](https://github.com/NotANameServer/incipyt/commit/21206618a1c319e3a08706c52c7c60e0134946a8))
+
 ## [0.3.0](https://github.com/NotANameServer/incipyt/compare/v0.2.0...v0.3.0) (2023-04-09)
 
 
 ### Features
 
 * **build:** flit supports ([3eccc8d](https://github.com/NotANameServer/incipyt/commit/3eccc8d976af066285a6892ed2abb384544e8988))
 * **build:** hatch support ([c44647f](https://github.com/NotANameServer/incipyt/commit/c44647f5727cbdadba667563fd86f97f7c6537e9))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `incipyt-0.3.0/LICENSE` & `incipyt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/README.md` & `incipyt-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	├── setup.cfg
 	└── setup.py
 
 incipyt provides a rich command line interface so you can choose various build
 systems, version control system, virtual environments, documentation software,
 linters, formatters, etc.
 
-	$ python -m incipyt --help
+    $ python -m incipyt --help
 
 ## Contribute
 
 incipyt is released under the MIT license and is open to contributions
 
 The complete setup instruction are found on the [dev-instructions]. Below is
 the minimum to get started:
@@ -54,14 +54,15 @@
     $ cd incipyt
     $ git config commit.template .gitmessage
     $ python -m venv --upgrade-deps .env
     $ source .env/bin/activate
     $ python -m pip install --upgrade flit
     $ python -m flit install --pth-file --deps develop
     $ python -m pytest -vv tests
+    $ pre-commit & pre-commit install
 
 [PyPA/packaging-projects]: https://packaging.python.org/tutorials/packaging-projects/
 [pyproject.toml]: https://www.python.org/dev/peps/pep-0518/
 [setuptools]: https://pypi.org/project/setuptools/
 [git]: https://git-scm.com/
 [sphinx]: https://www.sphinx-doc.org/en/master/
 [dev-instructions]: https://github.com/NotANameServer/incipyt/wiki/Developper-instructions
```

### Comparing `incipyt-0.3.0/incipyt/_internal/dumpers.py` & `incipyt-0.4.0/incipyt/_internal/dumpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import os
 import pathlib
 from abc import ABC, abstractmethod
 
-import toml
+import tomli_w
 
 from incipyt._internal import templates, utils
 
 
 class BaseDumper(ABC):
     def __init__(self, path, sanitizer=None):
         self._path = pathlib.Path(path)
@@ -72,9 +72,9 @@
     def dump_in(self, config):
         with self.open() as file:
             file.write(self._sep.join(config) + self._sep)
 
 
 class Toml(BaseDumper):
     def dump_in(self, config):
-        with self.open() as file:
-            toml.dump(config, file)
+        with self.open(mode="wb+") as file:
+            tomli_w.dump(config, file)
```

### Comparing `incipyt-0.3.0/incipyt/_internal/templates.py` & `incipyt-0.4.0/incipyt/_internal/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Incipyt mainly uses two kinds of templates: bare template strings that behave
 like builtin Python string formatting. It also provides special wrappers to
 allow easier templating of collections data structures, such as dict-like
 template objects.
 """
 
-import contextlib
 import logging
 from abc import ABCMeta, abstractmethod
 from collections import abc
 from pathlib import Path
 from string import Formatter
 
 import click
@@ -31,89 +30,56 @@
 class StringTemplate(Formattable):
     """This class acts like a wrapper around a format string.
 
     When an instance is called, it renders the underlying format string using
     environ values and overrides.
     """
 
-    def __init__(
-        self, format_string, confirmed=False, sanitizer=None, value_error=True, **kwargs
-    ):
-        r"""This class acts like a wrapper around a format string.
+    def __init__(self, format_string, sanitizer=None):
+        """This class acts like a wrapper around a format string.
 
         When an instance is called, it renders the underlying format string
         using environ values and overrides.
 
         :param format_string: A format string whose keyword argument will be substituted.
         :type format_string: :class:`str`
-        :param confirmed: Confirmed status for new variables from keyword args.
-        :type confirmed: :class:`bool`, optionnal
         :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
         :type sanitizer: :class:`function` or `None`, optionnal
-        :param value_error: Empty values generate errors.
-        :type value_error: :class:`bool`
-        :param \**kwargs: Variables overrides that will be used for rendering and pushed to the environ.
-            Automatically wrapped in :class:`incipyt._internal.utils.EnvValue` if needed.
-        :type \**kwargs: :class:`str`, optionnal
         """
-        self._confirmed = confirmed
         self._sanitizer = sanitizer
-        self._value_error = value_error
         self._format_string = format_string
-        self._kwargs = kwargs
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.format() == other
-        return utils.attrs_eq(
-            self, other, "_format_string", "_confirmed", "_sanitizer", "_value_error", "_kwargs"
-        )
+        return utils.attrs_eq(self, other, "_format_string", "_sanitizer")
 
     def __lt__(self, other):
         if isinstance(other, str):
             return self.format() < other
         return self.format() < other.format()
 
     def __gt__(self, other):
         if isinstance(other, str):
             return self.format() > other
         return self.format() > other.format()
 
     def __hash__(self):
-        return utils.attrs_hash(
-            self, "_format_string", "_confirmed", "_sanitizer", "_value_error", **self._kwargs
-        )
+        return utils.attrs_hash(self, "_format_string", "_sanitizer")
 
     def format(self):  # noqa: A003
         """Format the underlying format string using variables from the environ.
 
         :return: The formatted string.
         :rtype: :class:`str`
         """
-        return FormatterEnviron(sanitizer=self._sanitizer, value_error=self._value_error).format(
-            self._format_string,
-            **{
-                key: (
-                    value
-                    if isinstance(value, utils.EnvValue)
-                    else utils.EnvValue(value, confirmed=self._confirmed)
-                )
-                for key, value in self._kwargs.items()
-            },
-        )
+        return FormatterEnviron(sanitizer=self._sanitizer).format(self._format_string)
 
     def __repr__(self):
-        return utils.make_repr(
-            self,
-            format_string=self._format_string,
-            confirmed=self._confirmed,
-            sanitizer=self._sanitizer,
-            value_error=self._value_error,
-            kwargs=self._kwargs,
-        )
+        return utils.make_repr(self, format_string=self._format_string, sanitizer=self._sanitizer)
 
     @classmethod
     def wrap(cls, value):
         return value if isinstance(value, Formattable) else cls(value)
 
     @classmethod
     def from_file(cls, filename):
@@ -395,40 +361,36 @@
 
 class FormatterEnviron(abc.Mapping):
     """Class wrapping an environ and providing an interface to render templates.
 
     It can be used to render template strings.
     """
 
-    def __init__(self, sanitizer=None, value_error=True):
+    def __init__(self, sanitizer=None):
         """Class wrapping an environ and providing an interface to render templates.
 
         :param sanitizer: An optionnal callable to sanitize the values given (key, value) pairs.
         :type sanitizer: :class:`function` or `None`, optionnal
         :param environ: Consider empty string value as an error.
         :type environ: :class:`bool`, optional
         """
         self.data = project.environ
         self._keys = set()
         self._sanitizer = sanitizer
-        self._value_error = value_error
 
     def __contains__(self, key):
         if key not in self.data:
             self.data.__getitem__(key)
 
         return True
 
     def __getitem__(self, key):
         # Call to inner dict __getitem__ will create missing keys
         value = self.data[key]
-        if self._value_error and not value:
-            raise ValueError
-
-        return self._sanitizer(key, value) if self._sanitizer else value
+        return self._sanitizer(key, value) if value is not None and self._sanitizer else value
 
     def __iter__(self):
         return iter(self._keys)
 
     def __len__(self):
         return len(self._keys)
 
@@ -437,32 +399,25 @@
 
     def values(self):
         return (self[key] for key in self)
 
     def items(self):
         return zip(self.keys(), self.values())
 
-    def format(self, format_string, **kwargs):  # noqa: A003
-        r"""Render a format string.
+    def format(self, format_string):  # noqa: A003
+        """Render a format string.
 
         Variables will be request from the underlying environ, and undefined
-        variables will be created. If `self._value_error` is `True` and an
-        empty variable will cause the whole render result to be `None`.
+        variables will be created.
 
         Additional variables can be specified using keyword arguments. They
         will be added to the environ, hence they will override environ values.
 
         :param template: A format string whose keyword argument will be substituted.
         :type template: :class:`str`
-        :param \**kwargs: Additional variables that will override environ variables.
-        :type \**kwargs: :class:`str`, optionnal
         :return: The rendered template or `None` if a context variable is empty.
         :rtype: :class:`str` or `None`
         """
 
-        self._keys = {item[1] for item in Formatter().parse(format_string) if item[1]}
-        for key in self:
-            if key in kwargs:
-                self.data[key] = kwargs[key]
-
-        with contextlib.suppress(ValueError):
-            return format_string.format(**self)
+        self._keys = [item[1] for item in Formatter().parse(format_string) if item[1]]
+        formatted_string = format_string.format(**self)
+        return formatted_string if None not in self.values() else None
```

### Comparing `incipyt-0.3.0/incipyt/_internal/utils.py` & `incipyt-0.4.0/incipyt/_internal/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,8 @@
 import collections.abc
-import dataclasses
-from typing import Any
-
-
-@dataclasses.dataclass
-class EnvValue:
-    value: Any
-    update: bool = False
-    confirmed: bool = False
 
 
 def attrs_eq(a, b, *args):
     r"""Compare two objects according to their attributes.
 
     :param a: First object to compare.
     :param b: Second object to compare.
@@ -57,14 +48,34 @@
     from_attributes = [f"{a}={getattr(obj, a)}" for a in args]
     from_kwargs = [f"{k}={v}" for k, v in kwargs.items()]
     params = ", ".join(from_attributes + from_kwargs)
 
     return f"""{type(obj).__name__}({params})"""
 
 
+def strtobool(val):
+    """Convert a string representation of truth to true (1) or false (0).
+
+    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+    'val' is anything else.
+
+    Source: https://github.com/python/cpython/blob/v3.11.3/Lib/distutils/util.py#L308-L321
+    """
+    if isinstance(val, (bool, int)):
+        return bool(val)
+    val = val.lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    elif val in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    else:
+        raise ValueError("invalid truth value %r" % (val,))
+
+
 def unfold_dict(config):
     unfolded_config = {}
 
     for key_section, value_section in config.items():
         if isinstance(value_section, collections.abc.Mapping):
             if key_section not in unfolded_config:
                 unfolded_config[key_section] = {}
```

### Comparing `incipyt-0.3.0/incipyt/commands.py` & `incipyt-0.4.0/incipyt/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 import os
 import subprocess
 
 from incipyt import project
 from incipyt._internal.templates import Formattable
-from incipyt._internal.utils import EnvValue
 
 logger = logging.getLogger(__name__)
 
 
 def run(args, check=True, **kwargs):
     r"""Run a command after substitution using the environ.
 
@@ -36,15 +35,16 @@
     """Set PYTHON_CMD environment variable.
 
     :param python_path: List of the command elements.
     :type python_path: :class:`pathlib.Path`
     """
     if not python_path.is_absolute():
         raise AssertionError(f"{python_path} is not absolute.")
-    project.environ["PYTHON_CMD"] = EnvValue(os.fspath(python_path), update=True)
+    del project.environ["PYTHON_CMD"]
+    project.environ.inject("PYTHON_CMD", os.fspath(python_path))
 
 
 def python_m(args, **kwargs):
     r"""Run a python module after substitution using the environ.
 
     :param args: List of the command elements, excluding `python -m`.
     :type args: :class:`list`
```

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/Apache-2.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/BSD-2-Clause.txt` & `incipyt-0.4.0/incipyt/templates/licenses/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/BSD-3-Clause.txt` & `incipyt-0.4.0/incipyt/templates/licenses/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/CDDL-1.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/CDDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/EPL-2.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/EPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/GPL-2.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/GPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/GPL-3.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/GPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/LGPL-2.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/LGPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/LGPL-2.1.txt` & `incipyt-0.4.0/incipyt/templates/licenses/LGPL-2.1.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/LGPL-3.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/MIT.txt` & `incipyt-0.4.0/incipyt/templates/licenses/MIT.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/licenses/MPL-2.0.txt` & `incipyt-0.4.0/incipyt/templates/licenses/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/templates/python.gitignore` & `incipyt-0.4.0/incipyt/templates/python.gitignore`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/tools/base.py` & `incipyt-0.4.0/incipyt/tools/base.py`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/tools/git.py` & `incipyt-0.4.0/incipyt/tools/git.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,16 +45,20 @@
 
         Also push {AUTHOR_NAME} and {AUTHOR_EMAIL} using `git config user.*`.
 
         :param workon: Work-on folder.
         :type workon: :class:`pathlib.Path`
         """
         git(["init", os.fspath(workon)])
-        project.environ.setdefault("AUTHOR_EMAIL", git_get_config("user.email", workon=workon))
-        project.environ.setdefault("AUTHOR_NAME", git_get_config("user.name", workon=workon))
+        git_name = git_get_config("user.name", workon=workon)
+        if git_name:
+            project.environ.suggest("AUTHOR_NAME", git_name)
+        git_email = git_get_config("user.email", workon=workon)
+        if git_email:
+            project.environ.suggest("AUTHOR_EMAIL", git_email)
 
     def post(self, workon):
         """Check config name+email and then run `git add --all`.
 
         :param workon: Work-on folder.
         :type workon: :class:`pathlib.Path`
         """
```

### Comparing `incipyt-0.3.0/incipyt/tools/license.py` & `incipyt-0.4.0/incipyt/tools/license.py`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/tools/pep517/base.py` & `incipyt-0.4.0/incipyt/tools/pep517/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import os
-import sys
 
 from incipyt import commands, project, signals, tools
 from incipyt._internal import sanitizers, templates
 from incipyt._internal.dumpers import Toml
 
-# as of may 2022, the latest stable release of most bsd/linux
-# distributions ship a python whoose verion is at least 3.9
-LINUX_MIN_PYTHON_VERSION = (3, 9)
-
 
 class BuildSystem(tools.Tool):
     """Scripts to add generic PEP 517 build system to :class:`incipyt.project._Structure`."""
 
-    def __init__(self, check_build=False, **kwargs):
-        self.check_build = check_build
+    def __init__(self):
         signals.build_dependency.connect(self._slot_dependency)
         signals.classifier.connect(self._slot_classifier)
         signals.project_url.connect(self._slot_url)
 
     def add_to_structure(self):
         """Add PEP 517 core structure to `project.structure`.
 
@@ -52,68 +46,61 @@
         value is appended to the current one(s), the user will be asked to
         choose when commiting.
         """
         pyproject = project.structure.get_config_dict(Toml("pyproject.toml"))
 
         pyproject["project"] = {
             "authors": [{"name": "{AUTHOR_NAME}", "email": "{AUTHOR_EMAIL}"}],
-            "description": templates.StringTemplate(
-                "{SUMMARY_DESCRIPTION}",
-                SUMMARY_DESCRIPTION="\t",
-            ),
+            "description": "{SUMMARY_DESCRIPTION}",
             "license": {"file": "LICENSE"},
             "maintainers": [{"name": "{AUTHOR_NAME}", "email": "{AUTHOR_EMAIL}"}],
             "name": templates.StringTemplate(
                 "{PROJECT_NAME}",
                 sanitizer=sanitizers.project,
             ),
             "readme": "README.md",
             "requires-python": templates.StringTemplate(
-                ">={AUDIENCE_PYTHON_VERSION}",
-                sanitizer=sanitizers.version,
-                AUDIENCE_PYTHON_VERSION="{0[0]}.{0[1]}".format(
-                    min(sys.version_info, LINUX_MIN_PYTHON_VERSION)
-                ),
+                ">={AUDIENCE_PYTHON_VERSION}", sanitizer=sanitizers.version
             ),
             "version": templates.StringTemplate(
-                "{PACKAGE_VERSION}",
-                sanitizer=sanitizers.version,
-                PACKAGE_VERSION="0.0.0",
+                "{PACKAGE_VERSION}", sanitizer=sanitizers.version
             ),
         }
 
         project.structure.use_template("{PROJECT_NAME}/__init__.py", sanitizer=sanitizers.package)
         project.structure.use_template("README.md")
 
-        signals.build_dependency.emit(dep_name="build>=0.2.0")
+        signals.build_dependency.emit(dep_name="build", min_version="0.2.0")
 
         signals.classifier.emit(classifier="Programming Language :: Python :: 3 :: Only")
 
         signals.vcs_ignore.emit(pattern="dist/")
         signals.vcs_ignore.emit(pattern="*.egg-info")
 
     def _slot_classifier(self, classifier, **kwargs):
         pyproject = project.structure.get_config_dict(Toml("pyproject.toml"))
         if ("project", "classifiers") not in pyproject:
             pyproject["project", "classifiers"] = []
         pyproject["project", "classifiers"].append(classifier)
 
-    def _slot_dependency(self, dep_name, **kwargs):
+    def _slot_dependency(self, dep_name, min_version=None, **kwargs):
         pyproject = project.structure.get_config_dict(Toml("pyproject.toml"))
         if ("project", "optional-dependencies", "dev") not in pyproject:
             pyproject["project", "optional-dependencies", "dev"] = []
-        pyproject["project", "optional-dependencies", "dev"].append(dep_name)
+        pyproject["project", "optional-dependencies", "dev"].append(
+            dep_name if min_version is None else f"{dep_name}>={min_version}"
+        )
 
     def _slot_url(self, url_kind, url_value, **kwargs):
         project.structure.get_config_dict(Toml("pyproject.toml"))["project", "urls"] = {
             url_kind: url_value
         }
 
     def post(self, workon):
         """Editable install and build for test.
 
         :param workon: Work-on folder.
         :type workon: :class:`pathlib.Path`
         """
         commands.pip_install(["--editable", f"{workon}[dev]"])
-        if self.check_build:
+        if project.environ["CHECK_BUILD"]:
             commands.build([os.fspath(workon)])
```

### Comparing `incipyt-0.3.0/incipyt/tools/pep517/flit.py` & `incipyt-0.4.0/incipyt/tools/pep517/flit.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             raise RuntimeError("Build system already registered.")
 
         pyproject["build-system"] = {
             "build-backend": "flit_core.buildapi",
             "requires": ["flit_core>=3.4.0"],
         }
 
-        signals.build_dependency.emit(dep_name="flit>=3.4.0")
+        signals.build_dependency.emit(dep_name="flit", min_version="3.4.0")
```

### Comparing `incipyt-0.3.0/incipyt/tools/pep517/hatch.py` & `incipyt-0.4.0/incipyt/tools/pep517/hatch.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             raise RuntimeError("Build system already registered.")
 
         pyproject["build-system"] = {
             "build-backend": "hatchling.build",
             "requires": ["hatchling>=1.3.0"],
         }
 
-        signals.build_dependency.emit(dep_name="hatch>=1.2.0")
+        signals.build_dependency.emit(dep_name="hatch", min_version="1.2.0")
```

### Comparing `incipyt-0.3.0/incipyt/tools/pep517/pdm.py` & `incipyt-0.4.0/incipyt/tools/pep517/pdm.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             raise RuntimeError("Build system already registered.")
 
         pyproject["build-system"] = {
             "build-backend": "pdm.pep517.api",
             "requires": ["pdm-pep517>=1.0.0"],
         }
 
-        signals.build_dependency.emit(dep_name="pdm>=2.0.0")
+        signals.build_dependency.emit(dep_name="pdm", min_version="2.0.0")
```

### Comparing `incipyt-0.3.0/incipyt/tools/pep517/setuptools.py` & `incipyt-0.4.0/incipyt/tools/pep517/setuptools.py`

 * *Files identical despite different names*

### Comparing `incipyt-0.3.0/incipyt/tools/poetry.py` & `incipyt-0.4.0/incipyt/tools/poetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
-import sys
 
 from incipyt import commands, project, signals, tools
 from incipyt._internal import sanitizers, templates
 from incipyt._internal.dumpers import Toml
-from incipyt.tools.pep517.base import LINUX_MIN_PYTHON_VERSION
 
 
 class Poetry(tools.Tool):
     """Scripts to add Poetry to :class:`incipyt.project._Structure`."""
 
-    def __init__(self, check_build=False, **kwargs):
-        self.check_build = check_build
+    def __init__(self):
         signals.build_dependency.connect(self._slot_dependency)
         signals.classifier.connect(self._slot_classifier)
         signals.project_url.connect(self._slot_url)
 
+        project.variables["AUTHOR_NAME"].required = True
+        project.variables["AUTHOR_EMAIL"].required = True
+
     def add_to_structure(self):
         """Add poetry configuration to `project.structure`.
 
         :file:`pyptoject.toml`
 
         .. code-block::
 
@@ -41,19 +41,17 @@
             name = "{PROJECT_NAME}"
             readme = "README.md"
             version = "{PACKAGE_VERSION}"
 
             [tool.poetry.dependencies]
             python = ">={PYTHON_VERSION}"
 
-            [tool.poetry.extras]
-            dev = [
-                "build",
-                "poetry",
-            ]
+            [tool.poetry.dev-dependencies]
+            build = ">=0.2.0"
+            poetry = "*"
 
         If this configuration cannot be populate like that, an error is raised.
 
         Here key-value association is appended, if a key already exists the
         value is appended to the current one(s), the user will be asked to
         choose when commiting.
 
@@ -67,62 +65,53 @@
         pyproject["build-system"] = {
             "build-backend": "poetry.core.masonry.api",
             "requires": ["poetry_core"],
         }
 
         pyproject["tool", "poetry"] = {
             "authors": ["{AUTHOR_NAME} <{AUTHOR_EMAIL}>"],
-            "description": templates.StringTemplate(
-                "{SUMMARY_DESCRIPTION}",
-                SUMMARY_DESCRIPTION="\t",
-            ),
+            "description": "{SUMMARY_DESCRIPTION}",
             "license": "{LICENSE}",
             "maintainers": ["{AUTHOR_NAME} <{AUTHOR_EMAIL}>"],
             "name": templates.StringTemplate(
                 "{PROJECT_NAME}",
                 sanitizer=sanitizers.project,
             ),
             "readme": "README.md",
             "version": templates.StringTemplate(
-                "{PACKAGE_VERSION}",
-                sanitizer=sanitizers.version,
-                PACKAGE_VERSION="0.0.0",
+                "{PACKAGE_VERSION}", sanitizer=sanitizers.version
             ),
         }
 
         pyproject["tool", "poetry", "dependencies"] = {
             "python": templates.StringTemplate(
-                ">={AUDIENCE_PYTHON_VERSION}",
-                sanitizer=sanitizers.version,
-                AUDIENCE_PYTHON_VERSION="{0[0]}.{0[1]}".format(
-                    min(sys.version_info, LINUX_MIN_PYTHON_VERSION)
-                ),
-            ),
+                ">={AUDIENCE_PYTHON_VERSION}", sanitizer=sanitizers.version
+            )
         }
 
         project.structure.use_template("{PROJECT_NAME}/__init__.py", sanitizer=sanitizers.package)
         project.structure.use_template("README.md")
 
-        signals.build_dependency.emit(dep_name="build")
+        signals.build_dependency.emit(dep_name="build", min_version="0.2.0")
         signals.build_dependency.emit(dep_name="poetry")
 
         signals.classifier.emit(classifier="Programming Language :: Python :: 3 :: Only")
 
         signals.vcs_ignore.emit(pattern="dist")
 
     def _slot_classifier(self, classifier, **kwargs):
         pyproject = project.structure.get_config_dict(Toml("pyproject.toml"))
         if ("tool", "poetry", "classifiers") not in pyproject:
             pyproject["tool", "poetry", "classifiers"] = []
         pyproject["tool", "poetry", "classifiers"].append(classifier)
 
-    def _slot_dependency(self, dep_name, **kwargs):
+    def _slot_dependency(self, dep_name, min_version=None, **kwargs):
         project.structure.get_config_dict(Toml("pyproject.toml"))[
             "tool", "poetry", "dev-dependencies"
-        ] = {dep_name: "*"}
+        ] = {dep_name: "*" if min_version is None else f">={min_version}"}
 
     def _slot_url(self, url_kind, url_value, **kwargs):
         project.structure.get_config_dict(Toml("pyproject.toml"))["tool", "poetry"] = {
             url_kind: url_value
         }
 
     def post(self, workon):
@@ -136,10 +125,10 @@
             ["poetry", "env", "use", project.environ["PYTHON_CMD"]],
             cwd=os.fspath(workon),
         )
         commands.python_m(
             ["poetry", "install"],
             cwd=os.fspath(workon),
         )
-        if self.check_build:
+        if project.environ["CHECK_BUILD"]:
             commands.pip_install(["build"])
             commands.build([os.fspath(workon)])
```

### Comparing `incipyt-0.3.0/incipyt/tools/venv.py` & `incipyt-0.4.0/incipyt/tools/venv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 
 from incipyt import commands, signals, tools
+from incipyt._internal.templates import FormatterEnviron
 
 
 class Venv(tools.Tool):
     """Scripts to add virtualenv to :class:`incipyt.project._Structure`."""
 
     def add_to_structure(self):
         """Add venv configuration to `project.structure`, do nothing."""
-        signals.vcs_ignore.emit(pattern=".env/")
+        signals.vcs_ignore.emit(pattern="{VENV_FOLDER}/")
 
     def pre(self, workon):
         """Run `python -m venv .env`.
 
         :param workon: Work-on folder.
         :type workon: :class:`pathlib.Path`
         """
-        env_path = workon / ".env"
+        env_path = workon / FormatterEnviron().format("{VENV_FOLDER}")
         commands.venv([os.fspath(env_path)])
         commands.setenv_python_cmd(
             env_path.resolve() / ("Scripts" if os.name == "nt" else "bin") / "python"
         )
         commands.pip_install(["pip>=21.3.0"])
```

### Comparing `incipyt-0.3.0/pyproject.toml` & `incipyt-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -13,43 +13,44 @@
 ]
 description = "incipyt is a command-line tool that bootstraps a python project."
 maintainers = [
   {name = "Not at Name", email = "julien@drlazor.be"},
 ]
 name = "incipyt"
 readme = "README.md"
-requires-python = ">=3.7, <4.0"
-version = "0.3.0"
+requires-python = ">=3.8, <4.0"
+version = "0.4.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development",
 ]
 dependencies = [
   "click",
   "signalslot",
-  "toml",
+  "tomli_w",
+  "tomli; python_version<'3.11'"
 ]
 
 [project.optional-dependencies]
 dev = [
-  "flit==3.8.0",
-  "pre-commit==3.2.2",
+  "flit==3.9.0",
+  "pre-commit==3.3.2",
 ]
 doc = [
   "m2r2==0.3.2",
   "sphinxcontrib-apidoc==0.3.0",
-  "sphinx_rtd_theme==1.2.0",
+  "sphinx_rtd_theme==1.2.1",
 ]
 test = [
-  "pytest-cov==4.0.0",
+  "pytest-cov==4.1.0",
   "pytest-subprocess==1.5.0",
 ]
 
 [project.scripts]
 incipyt = "incipyt.__main__:main"
 
 [tool.black]
@@ -62,14 +63,15 @@
 format = "github"
 ignore = [
   "B024", "B027", # Disable rules about missing abstract decorators
   "D100", "D104", "D105", "D107", "D203", "D211", "D213",
   # Ease rules for pydocstyle (module/package/magic method/empty lines)
   "E501", "W505", # Disable rules about line-too-long, black does that
   "FBT002", #Disable "Boolean default value in function definition" rule
+  "PLC1901",  # Disable "(value == '') can be simplified to (not value)"
 ]
 select = [
   "B", "C4", "D", "E", "ERA", "F", "G", "I", "PIE", "PLC", "Q", "RUF", "SIM", "W",
   "A", "BLE", "FBT", "ISC", "N", "PLW", "PTH", "S", "YTT",
 ]
 show-fixes = true
 show-source = true
```

### Comparing `incipyt-0.3.0/tests/test_dumpers.py` & `incipyt-0.4.0/tests/test_dumpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from pytest import fixture, mark, raises
 
 from incipyt import project
+from incipyt.__main__ import feed_environ
 from incipyt._internal.dumpers import CfgIni, TextFile, Toml
 
 
 @fixture
 def reset_environ():
-    project.environ.clear()
+    feed_environ()
 
 
 @mark.parametrize("dumper", (CfgIni, Toml, TextFile))
 def test_format_path(dumper, reset_environ, tmp_path):
     dmp = dumper("{first}/{second}.ext")
-    project.environ["first"] = project.EnvValue("folder", confirmed=True)
-    project.environ["second"] = project.EnvValue("file", confirmed=True)
+    project.environ["first"] = "folder"
+    project.environ["second"] = "file"
     dmp.commit(tmp_path)
     assert dmp.format_path() == tmp_path / "folder" / "file.ext"
 
 
 @mark.parametrize("dumper", (CfgIni, Toml, TextFile))
 def test_mkdir(dumper, reset_environ, tmp_path):
     dmp = dumper("folder/file")
@@ -64,22 +65,22 @@
                     "fourth": {"one": {"two": "2"}},
                     "fifth": [{"one": "1.1", "two": "1.2"}, {"one": "2.1", "two": "2.2"}],
                 }
             },
             (
                 "[section]\n"
                 'first = "1"\n'
-                'third = [ "one", "two",]\n'
-                "[[section.fifth]]\n"
-                'one = "1.1"\n'
-                'two = "1.2"\n'
-                "\n"
-                "[[section.fifth]]\n"
-                'one = "2.1"\n'
-                'two = "2.2"\n'
+                "third = [\n"
+                '    "one",\n'
+                '    "two",\n'
+                "]\n"
+                "fifth = [\n"
+                '    { one = "1.1", two = "1.2" },\n'
+                '    { one = "2.1", two = "2.2" },\n'
+                "]\n"
                 "\n"
                 "[section.second]\n"
                 'one = "1"\n'
                 'two = "2"\n'
                 "\n"
                 "[section.fourth.one]\n"
                 'two = "2"\n'
```

### Comparing `incipyt-0.3.0/PKG-INFO` & `incipyt-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: incipyt
-Version: 0.3.0
+Version: 0.4.0
 Summary: incipyt is a command-line tool that bootstraps a python project.
 Author-email: Not at Name <julien@drlazor.be>
 Maintainer-email: Not at Name <julien@drlazor.be>
-Requires-Python: >=3.7, <4.0
+Requires-Python: >=3.8, <4.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Requires-Dist: click
 Requires-Dist: signalslot
-Requires-Dist: toml
-Requires-Dist: flit==3.8.0 ; extra == "dev"
-Requires-Dist: pre-commit==3.2.2 ; extra == "dev"
+Requires-Dist: tomli_w
+Requires-Dist: tomli; python_version<'3.11'
+Requires-Dist: flit==3.9.0 ; extra == "dev"
+Requires-Dist: pre-commit==3.3.2 ; extra == "dev"
 Requires-Dist: m2r2==0.3.2 ; extra == "doc"
 Requires-Dist: sphinxcontrib-apidoc==0.3.0 ; extra == "doc"
-Requires-Dist: sphinx_rtd_theme==1.2.0 ; extra == "doc"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
+Requires-Dist: sphinx_rtd_theme==1.2.1 ; extra == "doc"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "test"
 Requires-Dist: pytest-subprocess==1.5.0 ; extra == "test"
 Project-URL: documentation, https://github.com/NotANameServer/incipyt/wiki
 Project-URL: homepage, https://pypi.org/incipyt
 Project-URL: repository, https://github.com/NotANameServer/incipyt
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
@@ -69,15 +70,15 @@
 	├── setup.cfg
 	└── setup.py
 
 incipyt provides a rich command line interface so you can choose various build
 systems, version control system, virtual environments, documentation software,
 linters, formatters, etc.
 
-	$ python -m incipyt --help
+    $ python -m incipyt --help
 
 ## Contribute
 
 incipyt is released under the MIT license and is open to contributions
 
 The complete setup instruction are found on the [dev-instructions]. Below is
 the minimum to get started:
@@ -86,14 +87,15 @@
     $ cd incipyt
     $ git config commit.template .gitmessage
     $ python -m venv --upgrade-deps .env
     $ source .env/bin/activate
     $ python -m pip install --upgrade flit
     $ python -m flit install --pth-file --deps develop
     $ python -m pytest -vv tests
+    $ pre-commit & pre-commit install
 
 [PyPA/packaging-projects]: https://packaging.python.org/tutorials/packaging-projects/
 [pyproject.toml]: https://www.python.org/dev/peps/pep-0518/
 [setuptools]: https://pypi.org/project/setuptools/
 [git]: https://git-scm.com/
 [sphinx]: https://www.sphinx-doc.org/en/master/
 [dev-instructions]: https://github.com/NotANameServer/incipyt/wiki/Developper-instructions
```

