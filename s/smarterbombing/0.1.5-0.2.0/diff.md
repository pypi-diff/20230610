# Comparing `tmp/smarterbombing-0.1.5.tar.gz` & `tmp/smarterbombing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarterbombing-0.1.5.tar", max compression
+gzip compressed data, was "smarterbombing-0.2.0.tar", max compression
```

## Comparing `smarterbombing-0.1.5.tar` & `smarterbombing-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/LICENSE
--rw-r--r--   0        0        0      782 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/README.md
--rw-r--r--   0        0        0      860 2023-06-06 16:30:11.348100 smarterbombing-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/__init__.py
--rw-r--r--   0        0        0      769 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/__main__.py
--rw-r--r--   0        0        0    10637 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/analysis.py
--rw-r--r--   0        0        0     5473 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/app_live.py
--rw-r--r--   0        0        0     2979 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/app_offline.py
--rw-r--r--   0        0        0      817 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/configuration.py
--rw-r--r--   0        0        0     3648 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/log_reader.py
--rw-r--r--   0        0        0     3533 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/logs.py
--rw-r--r--   0        0        0        0 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/__init__.py
--rw-r--r--   0        0        0     1104 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui.py
--rw-r--r--   0        0        0     1837 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui_configuration.py
--rw-r--r--   0        0        0     5546 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui_live.py
--rw-r--r--   0        0        0     4199 2023-06-06 16:29:40.163005 smarterbombing-0.1.5/src/smarterbombing/webui/ui_offline_analysis.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 smarterbombing-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-10 15:17:24.112142 smarterbombing-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1321 2023-06-10 15:17:24.112142 smarterbombing-0.2.0/README.md
+-rw-r--r--   0        0        0      935 2023-06-10 15:17:56.510493 smarterbombing-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/__init__.py
+-rw-r--r--   0        0        0      769 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/aggregrator/__init__.py
+-rw-r--r--   0        0        0      712 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/aggregrator/aggregator.py
+-rw-r--r--   0        0        0     4060 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/aggregrator/damage_graph_aggregator.py
+-rw-r--r--   0        0        0     5902 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/aggregrator/site_statistics_aggregator.py
+-rw-r--r--   0        0        0     4455 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/app/squad.py
+-rw-r--r--   0        0        0     3549 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/configuration.py
+-rw-r--r--   0        0        0        0 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/logs/__init__.py
+-rw-r--r--   0        0        0     2817 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/logs/log_locator.py
+-rw-r--r--   0        0        0     1943 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/logs/log_reader.py
+-rw-r--r--   0        0        0        0 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/parsing/__init__.py
+-rw-r--r--   0        0        0     2589 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/parsing/combat_log_parser.py
+-rw-r--r--   0        0        0        0 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/webui/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/webui/html_generate_statistics.py
+-rw-r--r--   0        0        0     1180 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/webui/ui.py
+-rw-r--r--   0        0        0     4160 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/webui/ui_squad.py
+-rw-r--r--   0        0        0      511 2023-06-10 15:17:24.172145 smarterbombing-0.2.0/src/smarterbombing/webui/ui_squads.py
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 smarterbombing-0.2.0/PKG-INFO
```

### Comparing `smarterbombing-0.1.5/LICENSE` & `smarterbombing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.5/pyproject.toml` & `smarterbombing-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [tool.poetry]
 name = "smarterbombing"
-version = "0.1.5"
+version = "0.2.0"
 description = "A tool which reads combat logs from Eve Online and displays statistics."
 repository = "https://github.com/agelito/eve-smarterbombing"
 authors = ["Axel Wettervik <axel.wettervik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^2.0.2"
-parse = "^1.19.0"
 tabulate = "^0.9.0"
 gradio = "^3.33.1"
 matplotlib = "^3.7.1"
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.34.3"
+pyment = "^0.3.3"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+pylint = "^2.17.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
```

### Comparing `smarterbombing-0.1.5/src/smarterbombing/__main__.py` & `smarterbombing-0.2.0/src/smarterbombing/__main__.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.1.5/src/smarterbombing/logs.py` & `smarterbombing-0.2.0/src/smarterbombing/logs/log_locator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-"""Functions for finding and filtering log files"""
+"""Functions to help locate Eve Online log files"""
 from datetime import datetime
 from os import listdir
 from os.path import isfile, join
 from pathlib import Path
 import pandas as pd
-from parse import parse
+
+def _join_paths(filename: str, directory: str):
+    return join(directory, filename)
+
+def _date_string(date: datetime):
+    return date.date().strftime('%Y-%m-%d')
 
 def _map_log_file(filename: str):
-    """Retrieve structured data about log file based on the file name"""
     [name, _] = filename.split('.')
     parts =  name.split('_', 3)
 
     if len(parts) == 3:
-        (date, time, account) = parts
+        (date, time, character_id) = parts
     elif len(parts) == 2:
-        (date, time, account) = parts + [None]
+        (date, time, character_id) = parts + [None]
 
     date_time = f'{date} {time}'
     created_at = datetime.strptime(date_time, '%Y%m%d %H%M%S')
 
     return {
         'filename': filename,
-        'account': account,
+        'character_id': character_id,
         'created_at': created_at
     }
 
-def _find_log_files(eve_logs_directory):
-    """Find all log files in provided directory"""
-    files = [f for f in listdir(eve_logs_directory) if isfile(join(eve_logs_directory, f))]
-    files = list(map(_map_log_file, files))
+def _log_files(directory: str):
+    files = [f for f in listdir(directory) if isfile(join(directory, f))]
+    files = map(_map_log_file, files)
 
     return pd.DataFrame(files)
 
 LOG_HEADER_SIG = '------------------------------------------------------------'
 LOG_HEADER_TITLE = 'Gamelog'
 
 def _read_log_character_name(log_file_path):
@@ -43,75 +46,57 @@
             return None
 
         title = log_file.readline().strip()
         if LOG_HEADER_TITLE not in title:
             return None
 
         character_line = log_file.readline().strip()
-        character_name = parse('Listener: {}', character_line)
-        if character_name is None:
-            return None
-
-    return character_name[0]
+        character_name = character_line[10:]
 
-def _create_log_result(directory, log):
-    log_path = join(directory, log['filename'])
-    character_name = _read_log_character_name(log_path)
+    return character_name
 
-    return {
-        'path': log_path,
-        'character_id': log['account'],
-        'character_name': character_name,
-        'created_at': log['created_at'],
-    }
+def get_all_log_dates(directory: str) -> list:
+    """
+    Get a list of all log dates.
 
-def find_most_recent_character_logs(directory):
-    """Find the most recent log file for each account"""
-    log_files = _find_log_files(directory)
+    :param directory: which directory to search for log files
 
-    log_files.dropna(inplace=True)
-    log_files.sort_values(by='created_at', inplace=True, ascending=False)
+    :returns: list of unique log file dates
 
-    unique_accounts = log_files['account'].unique()
+    """
 
-    result = []
+    result = _log_files(directory)
 
-    for account in unique_accounts:
-        account_logs = log_files.loc[log_files['account'] == account]
-        if account_logs.count == 0:
-            continue
+    dates = result['created_at'].apply(_date_string)
+    dates = sorted(dates.unique(), reverse=True)
 
-        first_log = account_logs.iloc[0]
+    return dates
 
-        result.append(_create_log_result(directory, first_log))
+def get_latest_log_files(directory: str) -> list:
+    """
+    Get all latest log files.
 
-    return result
+    :param directory: which directory to search for log files
 
-def find_character_logs_at_date(directory, date):
-    """Find all log files at date"""
-    log_files = _find_log_files(directory)
-    log_files.dropna(inplace=True)
+    :returns: list of log files dict[path, filename, character_id, character, created_at]
 
-    log_files['date'] = log_files['created_at'].apply(_date_string)
+    """
+    result = _log_files(directory)
 
-    logs_at_date = log_files['date'].isin([date])
-    filtered_logs = log_files[logs_at_date]
+    result['path'] = result['filename'].apply(_join_paths, args=(directory, ))
 
-    return list(
-        filtered_logs.apply(lambda log: _create_log_result(directory, log), axis=1)
-    )
+    result = result.sort_values(by='created_at', ascending=False)
+    result = result.groupby('character_id', dropna=True).first()
+    result['character'] = result['path'].apply(_read_log_character_name)
 
-def _date_string(date: datetime):
-    return date.date().strftime('%Y-%m-%d')
+    return result.to_dict('records')
 
-def find_all_dates(directory):
-    """Find all available log file dates"""
-    log_files = _find_log_files(directory)
-    log_files.dropna(inplace=True)
+def default_log_directory():
+    """
+    Get the default Eve Online logs directory.
 
-    return list(log_files['created_at'].apply(_date_string).unique())
+    :returns: absolute path to logs directory
 
-def default_log_directory():
-    """Retrieve the default Eve log directory"""
+    """
     user_directory = join(Path.home(), 'Documents\\EVE\\logs\\Gamelogs')
 
     return user_directory
```

