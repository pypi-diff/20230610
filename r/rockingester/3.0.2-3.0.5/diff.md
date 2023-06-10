# Comparing `tmp/rockingester-3.0.2.tar.gz` & `tmp/rockingester-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-3.0.2.tar", last modified: Tue Jun  6 12:09:05 2023, max compression
+gzip compressed data, was "rockingester-3.0.5.tar", last modified: Sat Jun 10 10:58:01 2023, max compression
```

## Comparing `rockingester-3.0.2.tar` & `rockingester-3.0.5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:05.001597 rockingester-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.989596 rockingester-3.0.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.989596 rockingester-3.0.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-06 12:08:55.000000 rockingester-3.0.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-06 12:08:55.000000 rockingester-3.0.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-06 12:08:55.000000 rockingester-3.0.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.985596 rockingester-3.0.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-06 12:08:55.000000 rockingester-3.0.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 12:08:55.000000 rockingester-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-06 12:08:55.000000 rockingester-3.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 12:08:55.000000 rockingester-3.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 12:08:55.000000 rockingester-3.0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 12:08:55.000000 rockingester-3.0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 12:08:55.000000 rockingester-3.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 12:08:55.000000 rockingester-3.0.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 12:08:55.000000 rockingester-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-06 12:09:05.001597 rockingester-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-06 12:08:55.000000 rockingester-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-06 12:08:55.000000 rockingester-3.0.2/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.989596 rockingester-3.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.993596 rockingester-3.0.2/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 12:08:55.000000 rockingester-3.0.2/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-06 12:08:55.000000 rockingester-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:09:05.001597 rockingester-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.989596 rockingester-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:04.997596 rockingester-3.0.2/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:05.001597 rockingester-3.0.2/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 12:09:04.000000 rockingester-3.0.2/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:05.001597 rockingester-3.0.2/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/collectors/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/ftrix_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/plate_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-06 12:08:55.000000 rockingester-3.0.2/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:05.001597 rockingester-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:09:05.001597 rockingester-3.0.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/configurations/direct_sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/configurations/service_mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/configurations/service_sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/test_ftrix_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/test_plate_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-06 12:08:55.000000 rockingester-3.0.2/tests/test_platewait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.775267 rockingester-3.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-10 10:57:53.000000 rockingester-3.0.5/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-10 10:57:53.000000 rockingester-3.0.5/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-10 10:57:53.000000 rockingester-3.0.5/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.763267 rockingester-3.0.5/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-10 10:57:53.000000 rockingester-3.0.5/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-10 10:57:53.000000 rockingester-3.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-10 10:57:53.000000 rockingester-3.0.5/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-10 10:57:53.000000 rockingester-3.0.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-10 10:57:53.000000 rockingester-3.0.5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-10 10:57:53.000000 rockingester-3.0.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-10 10:57:53.000000 rockingester-3.0.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-10 10:57:53.000000 rockingester-3.0.5/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 10:57:53.000000 rockingester-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-10 10:58:01.775267 rockingester-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-10 10:57:53.000000 rockingester-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-10 10:57:53.000000 rockingester-3.0.5/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.763267 rockingester-3.0.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.767267 rockingester-3.0.5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 10:57:53.000000 rockingester-3.0.5/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-10 10:57:53.000000 rockingester-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 10:58:01.775267 rockingester-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.763267 rockingester-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.771267 rockingester-3.0.5/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.775267 rockingester-3.0.5/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.775267 rockingester-3.0.5/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 10:58:01.000000 rockingester-3.0.5/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.775267 rockingester-3.0.5/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/collectors/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/ftrix_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/plate_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-10 10:57:53.000000 rockingester-3.0.5/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.775267 rockingester-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:58:01.775267 rockingester-3.0.5/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/configurations/direct_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/configurations/service_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/configurations/service_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/test_ftrix_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/test_plate_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-10 10:57:53.000000 rockingester-3.0.5/tests/test_platewait.py
```

### Comparing `rockingester-3.0.2/.dae-devops/Makefile` & `rockingester-3.0.5/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/conventions.rst` & `rockingester-3.0.5/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/developing.rst` & `rockingester-3.0.5/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/devops.rst` & `rockingester-3.0.5/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/docs_structure.rst` & `rockingester-3.0.5/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/documenting.rst` & `rockingester-3.0.5/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/installing.rst` & `rockingester-3.0.5/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/docs/testing.rst` & `rockingester-3.0.5/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.dae-devops/project.yaml` & `rockingester-3.0.5/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.devcontainer/Dockerfile` & `rockingester-3.0.5/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.devcontainer/devcontainer.json` & `rockingester-3.0.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/CONTRIBUTING.rst` & `rockingester-3.0.5/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/actions/install_requirements/action.yml` & `rockingester-3.0.5/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/dependabot.yml` & `rockingester-3.0.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/pages/make_switcher.py` & `rockingester-3.0.5/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/workflows/code.yml` & `rockingester-3.0.5/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/workflows/docs.yml` & `rockingester-3.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/workflows/docs_clean.yml` & `rockingester-3.0.5/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.github/workflows/linkcheck.yml` & `rockingester-3.0.5/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.gitignore` & `rockingester-3.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.gitlab-ci.yml` & `rockingester-3.0.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/.vscode/launch.json` & `rockingester-3.0.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/LICENSE` & `rockingester-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/PKG-INFO` & `rockingester-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 3.0.2
+Version: 3.0.5
 Summary: Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-3.0.2/configurations/development.yaml` & `rockingester-3.0.5/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/docs/conf.py` & `rockingester-3.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/docs/images/dls-favicon.ico` & `rockingester-3.0.5/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/docs/images/dls-logo.svg` & `rockingester-3.0.5/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/pyproject.toml` & `rockingester-3.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester.egg-info/PKG-INFO` & `rockingester-3.0.5/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 3.0.2
+Version: 3.0.5
 Summary: Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-3.0.2/src/rockingester.egg-info/SOURCES.txt` & `rockingester-3.0.5/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_api/collectors/aiohttp.py` & `rockingester-3.0.5/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_api/collectors/collectors.py` & `rockingester-3.0.5/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_api/collectors/context.py` & `rockingester-3.0.5/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_api/exceptions.py` & `rockingester-3.0.5/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_api/thing.py` & `rockingester-3.0.5/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_api/things.py` & `rockingester-3.0.5/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_cli/main.py` & `rockingester-3.0.5/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_cli/subcommands/base.py` & `rockingester-3.0.5/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_cli/subcommands/service.py` & `rockingester-3.0.5/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_cli/version.py` & `rockingester-3.0.5/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/__main__.py` & `rockingester-3.0.5/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-3.0.5/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/collectors/base.py` & `rockingester-3.0.5/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/collectors/collectors.py` & `rockingester-3.0.5/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/collectors/context.py` & `rockingester-3.0.5/src/rockingester_lib/collectors/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,24 +58,28 @@
 
         # Not running as a service?
         elif self.context_specification.get("start_as") == "direct":
             # We need to activate the tick() task.
             await self.server.activate()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self, type, value, traceback) -> None:
+    async def aexit(self, type=None, value=None, traceback=None):
         """
         Asyncio context exit.
 
         Stop service if one was started and releases any client resources.
         """
+        logger.debug(f"[DISSHU] {thing_type} aexit")
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
-                # Put in request to shutdown the server.
-                await self.server.client_shutdown()
+                # The server associated with this context is running?
+                if await self.is_process_alive():
+                    logger.debug(f"[DISSHU] {thing_type} calling client_shutdown")
+                    # Put in request to shutdown the server.
+                    await self.server.client_shutdown()
 
             if self.context_specification.get("start_as") == "coro":
                 await self.server.direct_shutdown()
 
             if self.context_specification.get("start_as") == "direct":
                 await self.server.deactivate()
```

### Comparing `rockingester-3.0.2/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-3.0.5/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,17 @@
 
             # TODO: Make periodic tick period to be configurable.
             await asyncio.sleep(1.0)
 
     # ----------------------------------------------------------------------------------------
     async def scrape_plates_directories(self) -> None:
         """
-        Scrape all the configured directories looking for new files.
+        Scrape all the configured directories looking in each one for new plate directories.
+
+        Normally there is only one in the configured list of these places where plates arrive.
         """
 
         # TODO: Use asyncio tasks to paralellize scraping plates directories.
         for directory in self.__plates_directories:
             try:
                 await self.scrape_plates_directory(Path(directory))
             except Exception as exception:
@@ -264,31 +266,34 @@
 
         # Get the matching plate record from the xchembku or formulatrix database.
         crystal_plate_model = await self.__plate_injector.find_or_inject_barcode(
             plate_barcode,
             self.__visits_directory,
         )
 
-        logger.debug(
-            f"[CRYERR] for plate_barcode {plate_barcode} crystal_plate_model.error is {crystal_plate_model.error}"
-        )
-
+        # The model has not been marked as being in error?
         if crystal_plate_model.error is None:
             visit_directory = get_xchem_directory(
                 self.__visits_directory, crystal_plate_model.visit
             )
 
             # Scrape the directory when all image files have arrived.
             await self.scrape_plate_directory_if_complete(
                 plate_directory,
                 crystal_plate_model,
                 visit_directory,
             )
+
+        # The model has been marked as being in error?
         else:
-            # Remember we "handled" this one.
+            logger.debug(
+                f"[ROCKDIR] for plate_barcode {plate_barcode} crystal_plate_model.error is: {crystal_plate_model.error}"
+            )
+            # Remember we "handled" this one within the current instance.
+            # Keeping this list could be obviated if we could move the files out of the plates directory after we process them.
             self.__handled_plate_names.append(plate_name)
 
     # ----------------------------------------------------------------------------------------
     async def scrape_plate_directory_if_complete(
         self,
         plate_directory: Path,
         crystal_plate_model: CrystalPlateModel,
@@ -314,15 +319,15 @@
 
         # We have already put this plate directory into the visit directory?
         # This shouldn't really happen except when someone has been fiddling with the database.
         # TODO: Have a way to rebuild rockingest after database wipe, but images have already been copied to the visit.
         if target.is_dir():
             # Presumably this is done, so no error but log it.
             logger.debug(
-                f"[ROCKDIR] plate_barcode {plate_directory.name} is apparently already copied to {target}"
+                f"[ROCKDIR] plate directory {plate_directory.name} is apparently already copied to {target}"
             )
             self.__handled_plate_names.append(plate_directory.stem)
             return
 
         # This is the first time we have scraped a directory for this plate record in the database?
         if crystal_plate_model.rockminer_collected_stem is None:
             # Update the path stem in the crystal plate record.
```

### Comparing `rockingester-3.0.2/src/rockingester_lib/exceptions.py` & `rockingester-3.0.5/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/ftrix_client.py` & `rockingester-3.0.5/src/rockingester_lib/ftrix_client.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/plate_injector.py` & `rockingester-3.0.5/src/rockingester_lib/plate_injector.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/src/rockingester_lib/version.py` & `rockingester-3.0.5/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/base.py` & `rockingester-3.0.5/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/configurations/direct_sqlite.yaml` & `rockingester-3.0.5/tests/configurations/direct_sqlite.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/configurations/service_mysql.yaml` & `rockingester-3.0.5/tests/configurations/service_mysql.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/configurations/service_sqlite.yaml` & `rockingester-3.0.5/tests/configurations/service_sqlite.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/conftest.py` & `rockingester-3.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/test_collector.py` & `rockingester-3.0.5/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/test_ftrix_client.py` & `rockingester-3.0.5/tests/test_ftrix_client.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/test_plate_injector.py` & `rockingester-3.0.5/tests/test_plate_injector.py`

 * *Files identical despite different names*

### Comparing `rockingester-3.0.2/tests/test_platewait.py` & `rockingester-3.0.5/tests/test_platewait.py`

 * *Files identical despite different names*

