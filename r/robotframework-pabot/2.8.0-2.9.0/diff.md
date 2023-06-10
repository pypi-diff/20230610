# Comparing `tmp/robotframework-pabot-2.8.0.tar.gz` & `tmp/robotframework-pabot-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-pabot-2.8.0.tar", last modified: Tue Nov  1 08:12:22 2022, max compression
+gzip compressed data, was "robotframework-pabot-2.9.0.tar", last modified: Fri Dec 30 09:55:28 2022, max compression
```

## Comparing `robotframework-pabot-2.8.0.tar` & `robotframework-pabot-2.9.0.tar`

### file list

```diff
@@ -1,32 +1,109 @@
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-11-01 08:12:22.446729 robotframework-pabot-2.8.0/
--rw-r--r--   0 mkorpela   (501) staff       (20)    11357 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/LICENSE.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       20 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/MANIFEST.in
--rw-r--r--   0 mkorpela   (501) staff       (20)      903 2022-11-01 08:12:22.446589 robotframework-pabot-2.8.0/PKG-INFO
--rw-r--r--   0 mkorpela   (501) staff       (20)    10781 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/README.md
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-11-01 08:12:22.444764 robotframework-pabot-2.8.0/pabot/
--rw-r--r--   0 mkorpela   (501) staff       (20)     2217 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/SharedLibrary.py
--rw-r--r--   0 mkorpela   (501) staff       (20)       71 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/__init__.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     6689 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/arguments.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      231 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/clientwrapper.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      195 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/coordinatorwrapper.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     7817 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/execution_items.py
--rwxr-xr-x   0 mkorpela   (501) staff       (20)    65135 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/pabot.py
--rw-r--r--   0 mkorpela   (501) staff       (20)    22042 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/pabotlib.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-11-01 08:12:22.445489 robotframework-pabot-2.8.0/pabot/py3/
--rw-r--r--   0 mkorpela   (501) staff       (20)        0 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/py3/__init__.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     1434 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/py3/client.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     2313 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/py3/coordinator.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     2558 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/py3/messages.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     1612 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/py3/worker.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     8870 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/result_merger.py
--rw-r--r--   0 mkorpela   (501) staff       (20)    22272 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/robotremoteserver.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      185 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/pabot/workerwrapper.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-11-01 08:12:22.446387 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/
--rw-r--r--   0 mkorpela   (501) staff       (20)      903 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/PKG-INFO
--rw-r--r--   0 mkorpela   (501) staff       (20)      659 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/SOURCES.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)        1 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/dependency_links.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       44 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/entry_points.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       68 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/requires.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)        6 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/robotframework_pabot.egg-info/top_level.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       38 2022-11-01 08:12:22.446781 robotframework-pabot-2.8.0/setup.cfg
--rw-r--r--   0 mkorpela   (501) staff       (20)     1399 2022-11-01 08:12:22.000000 robotframework-pabot-2.8.0/setup.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.503217 robotframework-pabot-2.9.0/
+-rw-r--r--   0 mkorpela   (501) staff       (20)       38 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/.gitattributes
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.484258 robotframework-pabot-2.9.0/.github/
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.490057 robotframework-pabot-2.9.0/.github/workflows/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      546 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 mkorpela   (501) staff       (20)      123 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/.gitignore
+-rw-r--r--   0 mkorpela   (501) staff       (20)    11357 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/LICENSE.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)       20 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/MANIFEST.in
+-rw-r--r--   0 mkorpela   (501) staff       (20)      903 2022-12-30 09:55:28.502977 robotframework-pabot-2.9.0/PKG-INFO
+-rw-r--r--   0 mkorpela   (501) staff       (20)   131811 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/PabotLib.html
+-rw-r--r--   0 mkorpela   (501) staff       (20)    10781 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/README.md
+-rw-r--r--   0 mkorpela   (501) staff       (20)    12570 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/README_ru.md
+-rw-r--r--   0 mkorpela   (501) staff       (20)     7070 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/README_zh.md
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1195 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/TRICKS.md
+-rwxr-xr-x   0 mkorpela   (501) staff       (20)       35 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/devpy2.sh
+-rwxr-xr-x   0 mkorpela   (501) staff       (20)       35 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/devpy3.sh
+-rw-r--r--   0 mkorpela   (501) staff       (20)       94 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/mypy.ini
+-rw-r--r--   0 mkorpela   (501) staff       (20)       98 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/mypy.py2.ini
+-rw-r--r--   0 mkorpela   (501) staff       (20)       94 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/mypy.py3.ini
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.492265 robotframework-pabot-2.9.0/pabot/
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2217 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/SharedLibrary.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)       71 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/__init__.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     6689 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/arguments.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      231 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/clientwrapper.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      195 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/coordinatorwrapper.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     7936 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/execution_items.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    65552 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/pabot.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    22042 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/pabotlib.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.493124 robotframework-pabot-2.9.0/pabot/py3/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/py3/__init__.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1434 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/py3/client.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2313 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/py3/coordinator.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2558 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/py3/messages.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1612 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/py3/worker.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     8870 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/result_merger.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    22272 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/robotremoteserver.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      185 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot/workerwrapper.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    10575 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot.png
+-rw-r--r--   0 mkorpela   (501) staff       (20)     3849 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabot.svg
+-rw-r--r--   0 mkorpela   (501) staff       (20)      343 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/pabotprofiler.py
+-rwxr-xr-x   0 mkorpela   (501) staff       (20)      147 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/release.sh
+-rw-r--r--   0 mkorpela   (501) staff       (20)      224 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/requirements.txt
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.494194 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      903 2022-12-30 09:55:28.000000 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/PKG-INFO
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2900 2022-12-30 09:55:28.000000 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/SOURCES.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)        1 2022-12-30 09:55:28.000000 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/dependency_links.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)       43 2022-12-30 09:55:28.000000 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/entry_points.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)       68 2022-12-30 09:55:28.000000 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/requires.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)        6 2022-12-30 09:55:28.000000 robotframework-pabot-2.9.0/robotframework_pabot.egg-info/top_level.txt
+-rwxr-xr-x   0 mkorpela   (501) staff       (20)      223 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/run_tests.sh
+-rw-r--r--   0 mkorpela   (501) staff       (20)       38 2022-12-30 09:55:28.503280 robotframework-pabot-2.9.0/setup.cfg
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1430 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/setup.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.497970 robotframework-pabot-2.9.0/tests/
+-rw-r--r--   0 mkorpela   (501) staff       (20)       14 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/arguments.arg
+-rw-r--r--   0 mkorpela   (501) staff       (20)       26 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/failingarg.txt
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.498914 robotframework-pabot-2.9.0/tests/fixtures/
+-rw-r--r--   0 mkorpela   (501) staff       (20)       59 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/ingored.tmp
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1096 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/suite_one.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)      652 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/suite_second.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)       53 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/suite_special.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1695 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/suite_with_valueset_tags.robot
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.499490 robotframework-pabot-2.9.0/tests/fixtures/test_copy_artifacts/
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1261 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/test_copy_artifacts/keywords.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)      434 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/test_copy_artifacts/suite_1.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)      434 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/fixtures/test_copy_artifacts/suite_2.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)      197 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/mylib.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     6485 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/output.xml
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.500411 robotframework-pabot-2.9.0/tests/outputs/
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1895 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/first.xml
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.485099 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.485158 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.485522 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.500798 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/fake_screenshot_root.png
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.501192 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/other_artifacts/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/other_artifacts/another_artifact.bar
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/other_artifacts/some_artifact.foo
+-rw-r--r--   0 mkorpela   (501) staff       (20)    11143 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/output.xml
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.501566 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/screenshots/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/screenshots/fake_screenshot_subfolder_1.png
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/0/screenshots/fake_screenshot_subfolder_2.png
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.501930 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/fake_screenshot_root.png
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.502301 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/other_artifacts/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/other_artifacts/another_artifact.bar
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/other_artifacts/some_artifact.foo
+-rw-r--r--   0 mkorpela   (501) staff       (20)    11144 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/output.xml
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-12-30 09:55:28.502675 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/screenshots/
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/screenshots/fake_screenshot_subfolder_1.png
+-rw-r--r--   0 mkorpela   (501) staff       (20)        4 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/outputs_with_artifacts/out_dir/pabot_results/1/screenshots/fake_screenshot_subfolder_2.png
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1900 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/second.xml
+-rw-r--r--   0 mkorpela   (501) staff       (20)     4068 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/tests.xml
+-rw-r--r--   0 mkorpela   (501) staff       (20)     4078 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/tests2.xml
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1897 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/outputs/third.xml
+-rw-r--r--   0 mkorpela   (501) staff       (20)       26 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/passingarg.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)      144 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/recursion.robot
+-rw-r--r--   0 mkorpela   (501) staff       (20)      235 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/resourcefile.dat
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2045 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_arguments_output.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     4369 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_depends.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1367 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_functional.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     6862 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_ordering.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    48520 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_pabot.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    11338 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_pabotlib.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1806 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_pabotsuitenames_io.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2118 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_resultmerger.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1225 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_stacktrace.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2353 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/test_testlevelsplit_output_task_order.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      283 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tests/valueset.dat
+-rw-r--r--   0 mkorpela   (501) staff       (20)      265 2022-12-30 09:55:27.000000 robotframework-pabot-2.9.0/tox.ini
```

### Comparing `robotframework-pabot-2.8.0/LICENSE.txt` & `robotframework-pabot-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/PKG-INFO` & `robotframework-pabot-2.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: robotframework-pabot
-Version: 2.8.0
+Version: 2.9.0
 Summary: Parallel test runner for Robot Framework
 Home-page: https://pabot.org
+Download-URL: https://pypi.python.org/pypi/robotframework-pabot
 Author: Mikko Korpela
 Author-email: mikko.korpela@gmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/robotframework-pabot
 Project-URL: Source, https://github.com/mkorpela/pabot
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `robotframework-pabot-2.8.0/README.md` & `robotframework-pabot-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/SharedLibrary.py` & `robotframework-pabot-2.9.0/pabot/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/arguments.py` & `robotframework-pabot-2.9.0/pabot/arguments.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/execution_items.py` & `robotframework-pabot-2.9.0/pabot/execution_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,23 +102,33 @@
 
     depends = None  # type: str
     depends_keyword = "#DEPENDS"
 
     def set_name_and_depends(self, name):
         line_name = name.encode("utf-8") if PY2 and is_unicode(name) else name
         depends_begin_index = line_name.find(self.depends_keyword)
-        self.name = line_name if depends_begin_index == -1 else line_name[0:depends_begin_index].strip()
-        self.depends = line_name[depends_begin_index+len(self.depends_keyword):].strip() if depends_begin_index != -1 \
+        self.name = (
+            line_name
+            if depends_begin_index == -1
+            else line_name[0:depends_begin_index].strip()
+        )
+        self.depends = (
+            line_name[depends_begin_index + len(self.depends_keyword) :].strip()
+            if depends_begin_index != -1
             else None
+        )
 
     def line(self):
         # type: () -> str
         line_without_depends = "--" + self.type + " " + self.name
-        return line_without_depends + " " + self.depends_keyword + " " + self.depends if self.depends \
+        return (
+            line_without_depends + " " + self.depends_keyword + " " + self.depends
+            if self.depends
             else line_without_depends
+        )
 
 
 class SuiteItem(RunnableItem):
 
     type = "suite"
 
     def __init__(self, name, tests=None, suites=None, dynamictests=None):
```

### Comparing `robotframework-pabot-2.8.0/pabot/pabot.py` & `robotframework-pabot-2.9.0/pabot/pabot.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  partly based on work by Nokia Solutions and Networks Oyj
 """A parallel executor for Robot Framework test cases.
-Version 2.8.0
+Version 2.9.0
 
 Supports all Robot Framework command line options and also following
 options (these must be before normal RF options):
 
 --verbose
   more output
 
@@ -315,14 +315,15 @@
         stdout,
         verbose,
         show_stdout_on_failure,
     )
     if is_ignored and os.path.isdir(outs_dir):
         shutil.rmtree(outs_dir)
 
+
 def _result_to_stdout(
     elapsed,
     is_ignored,
     item_name,
     my_index,
     pool_id,
     process,
@@ -776,15 +777,14 @@
 
 
 if PY2:
 
     def _open_pabotsuitenames(mode):
         return open(".pabotsuitenames", mode)
 
-
 else:
 
     def _open_pabotsuitenames(mode):
         return open(".pabotsuitenames", mode, encoding="utf-8")
 
 
 def solve_shard_suites(suite_names, pabot_args):
@@ -892,29 +892,31 @@
 ):  # type: (Optional[Hashes], Hashes, Dict[str, str], str, List[str], Dict[str, str], List[ExecutionItem]) -> List[ExecutionItem]
     assert all(isinstance(s, ExecutionItem) for s in lines)
     if (
         (file_h is None or file_h.suitesfrom != h.suitesfrom)
         and "suitesfrom" in pabot_args
         and os.path.isfile(pabot_args["suitesfrom"])
     ):
-        suites = _suites_from_file(file_h, h, pabot_args, outs_dir, datasources, options, lines)
+        suites = _suites_from_file(
+            file_h, h, pabot_args, outs_dir, datasources, options, lines
+        )
     else:
-        suites = _suites_from_wrong_or_empty_file(pabot_args, outs_dir, datasources, options, lines)
+        suites = _suites_from_wrong_or_empty_file(
+            pabot_args, outs_dir, datasources, options, lines
+        )
     if suites:
         store_suite_names(h, suites)
     assert all(isinstance(s, ExecutionItem) for s in suites)
     return suites
 
 
 def _suites_from_file(file_h, h, pabot_args, outs_dir, datasources, options, lines):
     suites = _suites_from_outputxml(pabot_args["suitesfrom"])
     if file_h is None or file_h.dirs != h.dirs:
-        all_suites = generate_suite_names_with_builder(
-            outs_dir, datasources, options
-        )
+        all_suites = generate_suite_names_with_builder(outs_dir, datasources, options)
     else:
         all_suites = [suite for suite in lines if suite]
     return _preserve_order(all_suites, suites)
 
 
 def _suites_from_wrong_or_empty_file(pabot_args, outs_dir, datasources, options, lines):
     suites = _levelsplit(
@@ -1776,20 +1778,18 @@
             else:
                 names.append(item.execution_item.name)
     index = 0
     for items in all_items:
         for item in items:
             if isinstance(item.execution_item, SuiteItems):
                 for suite in item.execution_item.suites:
-                    item.last_level = _find_ending_level(
-                        suite.name, names[index + 1:]
-                    )
+                    item.last_level = _find_ending_level(suite.name, names[index + 1 :])
             else:
                 item.last_level = _find_ending_level(
-                    item.execution_item.name, names[index + 1:]
+                    item.execution_item.name, names[index + 1 :]
                 )
             index += 1
 
 
 def _initialize_queue_index():
     global _PABOTLIBURI
     plib = Remote(_PABOTLIBURI)
@@ -1837,48 +1837,52 @@
         _NUMBER_OF_ITEMS_TO_BE_EXECUTED += len(items)
         for item in items:
             _NOT_COMPLETED_INDEXES.append(item.index)
     return items
 
 
 def main(args=None):
+    return sys.exit(main_program(args))
+
+
+def main_program(args):
     global _PABOTLIBPROCESS
     args = args or sys.argv[1:]
     if len(args) == 0:
         print(
             "[ "
             + _wrap_with(Color.RED, "ERROR")
             + " ]: Expected at least 1 argument, got 0."
         )
         print("Try --help for usage information.")
-        sys.exit(252)
+        return 252
     start_time = time.time()
     start_time_string = _now()
     # NOTE: timeout option
     try:
         _start_message_writer()
         options, datasources, pabot_args, opts_for_run = parse_args(args)
         if pabot_args["help"]:
             print(__doc__)
-            sys.exit(0)
+            return 0
         if len(datasources) == 0:
             print("[ " + _wrap_with(Color.RED, "ERROR") + " ]: No datasources given.")
             print("Try --help for usage information.")
-            sys.exit(252)
+            return 252
         _PABOTLIBPROCESS = _start_remote_library(pabot_args)
         if _pabotlib_in_use():
             _initialize_queue_index()
         outs_dir = _output_dir(options)
         suite_groups = _group_suites(outs_dir, datasources, options, pabot_args)
         if pabot_args["verbose"]:
             _write("Suite names resolved in %s seconds" % str(time.time() - start_time))
         if not suite_groups or suite_groups == [[]]:
             _write("No tests to execute")
             if not options.get("runemptysuite", False):
-                sys.exit(252)
+                return 252
         execution_items = _create_execution_items(
             suite_groups, datasources, outs_dir, options, opts_for_run, pabot_args
         )
         while execution_items:
             items = execution_items.pop(0)
             _parallel_execute(
                 items,
@@ -1891,42 +1895,48 @@
         result_code = _report_results(
             outs_dir,
             pabot_args,
             options,
             start_time_string,
             _get_suite_root_name(suite_groups),
         )
-        sys.exit(result_code if not _ABNORMAL_EXIT_HAPPENED else 252)
+        return result_code if not _ABNORMAL_EXIT_HAPPENED else 252
     except Information as i:
         print(__doc__)
         print(i.message)
     except DataError as err:
         print(err.message)
-        sys.exit(252)
+        return 252
     except Exception:
         _write("[ERROR] EXCEPTION RAISED DURING PABOT EXECUTION", Color.RED)
         _write(
             "[ERROR] PLEASE CONSIDER REPORTING THIS ISSUE TO https://github.com/mkorpela/pabot/issues",
             Color.RED,
         )
+        _write("Pabot: 2.9.0")
+        _write("Python: %s" % sys.version)
+        _write("Robot Framework: %s" % ROBOT_VERSION)
         raise
     finally:
         if _PABOTLIBPROCESS:
             _stop_remote_library(_PABOTLIBPROCESS)
         _print_elapsed(start_time, time.time())
         _stop_message_writer()
 
 
 def _group_suites(outs_dir, datasources, options, pabot_args):
     suite_names = solve_suite_names(outs_dir, datasources, options, pabot_args)
     _verify_depends(suite_names)
     shard_suites = solve_shard_suites(suite_names, pabot_args)
     ordered_suites = _preserve_order(shard_suites, pabot_args.get("ordering"))
-    grouped_suites = _chunked_suite_names(ordered_suites, pabot_args["processes"]) if pabot_args["chunk"] \
+    grouped_suites = (
+        _chunked_suite_names(ordered_suites, pabot_args["processes"])
+        if pabot_args["chunk"]
         else _group_by_wait(_group_by_groups(ordered_suites))
+    )
     grouped_by_depend = _all_grouped_suites_by_depend(grouped_suites)
     return grouped_by_depend
 
 
 def _chunked_suite_names(suite_names, processes):
     q, r = divmod(len(suite_names), processes)
     result = []
@@ -1940,42 +1950,63 @@
         for item in chunk:
             grouped.add(item)
         result.append(grouped)
     return [result]
 
 
 def _verify_depends(suite_names):
-    runnable_suites = list(filter(lambda suite: isinstance(suite, RunnableItem), suite_names))
+    runnable_suites = list(
+        filter(lambda suite: isinstance(suite, RunnableItem), suite_names)
+    )
     suites_with_depends = list(filter(lambda suite: suite.depends, runnable_suites))
     suites_with_found_dependencies = list(
-        filter(lambda suite: any(runnable_suite.name == suite.depends for runnable_suite in runnable_suites),
-               suites_with_depends))
+        filter(
+            lambda suite: any(
+                runnable_suite.name == suite.depends
+                for runnable_suite in runnable_suites
+            ),
+            suites_with_depends,
+        )
+    )
     if suites_with_depends != suites_with_found_dependencies:
         raise Exception("There are unmet dependencies using #DEPENDS")
-    suites_with_circular_dependencies = list(filter(lambda suite: suite.depends == suite.name, suites_with_depends))
+    suites_with_circular_dependencies = list(
+        filter(lambda suite: suite.depends == suite.name, suites_with_depends)
+    )
     if suites_with_circular_dependencies:
         raise Exception("There are suites with circular dependencies using #DEPENDS")
-    grouped_suites = list(filter(lambda suite: isinstance(suite, GroupItem), suite_names))
+    grouped_suites = list(
+        filter(lambda suite: isinstance(suite, GroupItem), suite_names)
+    )
     if grouped_suites and suites_with_depends:
         raise Exception("#DEPENDS and grouped suites are incompatible")
 
 
 def _group_by_depend(suite_names):
     group_items = list(filter(lambda suite: isinstance(suite, GroupItem), suite_names))
-    runnable_suites = list(filter(lambda suite: isinstance(suite, RunnableItem), suite_names))
+    runnable_suites = list(
+        filter(lambda suite: isinstance(suite, RunnableItem), suite_names)
+    )
     if group_items or not runnable_suites:
         return [suite_names]
     independent_tests = list(filter(lambda suite: not suite.depends, runnable_suites))
     dependency_tree = [independent_tests]
     while True:
         dependent_tests = list(filter(lambda suite: suite.depends, runnable_suites))
-        dependent_on_last_stage = list(filter(
-            lambda suite: any(test_in_tier_before.name == suite.depends for test_in_tier_before in dependency_tree[-1]),
-            dependent_tests))
-        if not dependent_on_last_stage: break
+        dependent_on_last_stage = list(
+            filter(
+                lambda suite: any(
+                    test_in_tier_before.name == suite.depends
+                    for test_in_tier_before in dependency_tree[-1]
+                ),
+                dependent_tests,
+            )
+        )
+        if not dependent_on_last_stage:
+            break
         dependency_tree += [dependent_on_last_stage]
     flattened_dependency_tree = sum(dependency_tree, [])
     if len(flattened_dependency_tree) != len(runnable_suites):
         raise Exception("There are circular or unmet dependencies using #DEPENDS")
     return dependency_tree
```

### Comparing `robotframework-pabot-2.8.0/pabot/pabotlib.py` & `robotframework-pabot-2.9.0/pabot/pabotlib.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/py3/client.py` & `robotframework-pabot-2.9.0/pabot/py3/client.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/py3/coordinator.py` & `robotframework-pabot-2.9.0/pabot/py3/coordinator.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/py3/messages.py` & `robotframework-pabot-2.9.0/pabot/py3/messages.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/py3/worker.py` & `robotframework-pabot-2.9.0/pabot/py3/worker.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/result_merger.py` & `robotframework-pabot-2.9.0/pabot/result_merger.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/pabot/robotremoteserver.py` & `robotframework-pabot-2.9.0/pabot/robotremoteserver.py`

 * *Files identical despite different names*

### Comparing `robotframework-pabot-2.8.0/robotframework_pabot.egg-info/PKG-INFO` & `robotframework-pabot-2.9.0/robotframework_pabot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: robotframework-pabot
-Version: 2.8.0
+Version: 2.9.0
 Summary: Parallel test runner for Robot Framework
 Home-page: https://pabot.org
+Download-URL: https://pypi.python.org/pypi/robotframework-pabot
 Author: Mikko Korpela
 Author-email: mikko.korpela@gmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/robotframework-pabot
 Project-URL: Source, https://github.com/mkorpela/pabot
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `robotframework-pabot-2.8.0/setup.py` & `robotframework-pabot-2.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 name = "Mikko Korpela"
 # I might be just a little bit too much afraid of those bots..
 address = name.lower().replace(" ", ".") + chr(64) + "gmail.com"
 
 setup(
     name="robotframework-pabot",
-    version="2.8.0",
+    version="2.9.0",
     description="Parallel test runner for Robot Framework",
     long_description="A parallel executor for Robot Framework tests."
     " With Pabot you can split one execution into multiple and save test execution time.",
     author=name,
     author_email=address,
     url="https://pabot.org",
     project_urls={
@@ -28,11 +28,15 @@
         "Topic :: Software Development :: Testing",
         "License :: OSI Approved :: Apache Software License",
         "Development Status :: 5 - Production/Stable",
         "Framework :: Robot Framework",
     ],
     entry_points={"console_scripts": ["pabot=pabot.pabot:main"]},
     license="Apache License, Version 2.0",
-    install_requires=["robotframework>=3.2", "robotframework-stacktrace>=0.4.1", "natsort>=8.2.0"],
+    install_requires=[
+        "robotframework>=3.2",
+        "robotframework-stacktrace>=0.4.1",
+        "natsort>=8.2.0",
+    ],
     python_requires=">=3.6",
     include_package_data=True,
 )
```

