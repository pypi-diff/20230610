# Comparing `tmp/granny-pliers-0.0.6.tar.gz` & `tmp/granny-pliers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granny-pliers-0.0.6.tar", last modified: Fri Jun  9 10:11:08 2023, max compression
+gzip compressed data, was "granny-pliers-0.0.7.tar", last modified: Fri Jun  9 20:57:17 2023, max compression
```

## Comparing `granny-pliers-0.0.6.tar` & `granny-pliers-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.301534 granny-pliers-0.0.6/
--rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.6/LICENSE
--rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-09 10:11:08.300895 granny-pliers-0.0.6/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)       15 2023-06-03 15:16:58.000000 granny-pliers-0.0.6/README.md
--rw-r--r--   0 pd         (501) staff       (20)     1915 2023-06-09 10:10:16.000000 granny-pliers-0.0.6/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-09 10:11:08.301680 granny-pliers-0.0.6/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.283725 granny-pliers-0.0.6/src/
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.286502 granny-pliers-0.0.6/src/granny_pliers/
--rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-09 10:10:16.000000 granny-pliers-0.0.6/src/granny_pliers/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.292093 granny-pliers-0.0.6/src/granny_pliers/config/
--rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/config/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2438 2023-06-04 16:08:02.000000 granny-pliers-0.0.6/src/granny_pliers/config/abstract_config.py
--rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.6/src/granny_pliers/config/autowired_config.py
--rw-r--r--   0 pd         (501) staff       (20)     5994 2023-06-03 23:39:30.000000 granny-pliers-0.0.6/src/granny_pliers/config/logger_config.py
--rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.6/src/granny_pliers/config/project_environment.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.294200 granny-pliers-0.0.6/src/granny_pliers/logger/
--rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/logger/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.6/src/granny_pliers/logger/abstract_logger.py
--rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.6/src/granny_pliers/logger/log_processors.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.296988 granny-pliers-0.0.6/src/granny_pliers/orm/
--rw-r--r--   0 pd         (501) staff       (20)      852 2023-06-09 10:10:16.000000 granny-pliers-0.0.6/src/granny_pliers/orm/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5456 2023-06-09 10:10:16.000000 granny-pliers-0.0.6/src/granny_pliers/orm/abstract_http_client.py
--rw-r--r--   0 pd         (501) staff       (20)     1328 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/orm/abstract_model.py
--rw-r--r--   0 pd         (501) staff       (20)     7530 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/orm/abstract_repository.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.298882 granny-pliers-0.0.6/src/granny_pliers/testing/
--rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/testing/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1982 2023-06-04 16:08:02.000000 granny-pliers-0.0.6/src/granny_pliers/testing/abstract_test_case.py
--rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-04 16:08:02.000000 granny-pliers-0.0.6/src/granny_pliers/testing/async_abstract_test_case.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.300008 granny-pliers-0.0.6/src/granny_pliers/worker/
--rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/worker/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.6/src/granny_pliers/worker/abstract_worker.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 10:11:08.288795 granny-pliers-0.0.6/src/granny_pliers.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-09 10:11:08.000000 granny-pliers-0.0.6/src/granny_pliers.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      992 2023-06-09 10:11:08.000000 granny-pliers-0.0.6/src/granny_pliers.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-09 10:11:08.000000 granny-pliers-0.0.6/src/granny_pliers.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      235 2023-06-09 10:11:08.000000 granny-pliers-0.0.6/src/granny_pliers.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-09 10:11:08.000000 granny-pliers-0.0.6/src/granny_pliers.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.144766 granny-pliers-0.0.7/
+-rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.7/LICENSE
+-rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-09 20:57:17.144346 granny-pliers-0.0.7/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)       15 2023-06-03 15:16:58.000000 granny-pliers-0.0.7/README.md
+-rw-r--r--   0 pd         (501) staff       (20)     1915 2023-06-09 20:56:08.000000 granny-pliers-0.0.7/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-09 20:57:17.144856 granny-pliers-0.0.7/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.132666 granny-pliers-0.0.7/src/
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.135069 granny-pliers-0.0.7/src/granny_pliers/
+-rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-09 20:56:14.000000 granny-pliers-0.0.7/src/granny_pliers/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.138889 granny-pliers-0.0.7/src/granny_pliers/config/
+-rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/config/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     3186 2023-06-09 20:55:51.000000 granny-pliers-0.0.7/src/granny_pliers/config/abstract_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.7/src/granny_pliers/config/autowired_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     5994 2023-06-03 23:39:30.000000 granny-pliers-0.0.7/src/granny_pliers/config/logger_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.7/src/granny_pliers/config/project_environment.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.139910 granny-pliers-0.0.7/src/granny_pliers/logger/
+-rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/logger/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.7/src/granny_pliers/logger/abstract_logger.py
+-rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.7/src/granny_pliers/logger/log_processors.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.141703 granny-pliers-0.0.7/src/granny_pliers/orm/
+-rw-r--r--   0 pd         (501) staff       (20)      852 2023-06-09 10:10:16.000000 granny-pliers-0.0.7/src/granny_pliers/orm/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5456 2023-06-09 10:10:16.000000 granny-pliers-0.0.7/src/granny_pliers/orm/abstract_http_client.py
+-rw-r--r--   0 pd         (501) staff       (20)     1328 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/orm/abstract_model.py
+-rw-r--r--   0 pd         (501) staff       (20)     7530 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/orm/abstract_repository.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.143152 granny-pliers-0.0.7/src/granny_pliers/testing/
+-rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/testing/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1982 2023-06-04 16:08:02.000000 granny-pliers-0.0.7/src/granny_pliers/testing/abstract_test_case.py
+-rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-04 16:08:02.000000 granny-pliers-0.0.7/src/granny_pliers/testing/async_abstract_test_case.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.143838 granny-pliers-0.0.7/src/granny_pliers/worker/
+-rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/worker/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.7/src/granny_pliers/worker/abstract_worker.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-09 20:57:17.137106 granny-pliers-0.0.7/src/granny_pliers.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-09 20:57:17.000000 granny-pliers-0.0.7/src/granny_pliers.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      992 2023-06-09 20:57:17.000000 granny-pliers-0.0.7/src/granny_pliers.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-09 20:57:17.000000 granny-pliers-0.0.7/src/granny_pliers.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      235 2023-06-09 20:57:17.000000 granny-pliers-0.0.7/src/granny_pliers.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-09 20:57:17.000000 granny-pliers-0.0.7/src/granny_pliers.egg-info/top_level.txt
```

### Comparing `granny-pliers-0.0.6/LICENSE` & `granny-pliers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/PKG-INFO` & `granny-pliers-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.6/pyproject.toml` & `granny-pliers-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "granny-pliers"
-version = "0.0.6"
+version = "0.0.7"
 
 authors = [
     { name = "Dmytro Stepanenko", email = "dmitrijstepanenko@gmail.com" },
 ]
 
 license = { file = "LICENSE" }
```

### Comparing `granny-pliers-0.0.6/src/granny_pliers/__init__.py` & `granny-pliers-0.0.7/src/granny_pliers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Granny Pliers is a Python library that contains a collection of useful
 and helpful tools, designed to simplify developers' lives."""
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __author__ = "Dmytro Stepanenko"
 __copyright__ = "Copyright 2022, Dmytro Stepanenko, Granny Pliers"
 __credits__ = ["Dmytro Stepanenko"]
 __license__ = "Apache License Version 2.0"
 __email__ = "dmitrijstepanenko@gmail.com"
```

### Comparing `granny-pliers-0.0.6/src/granny_pliers/config/__init__.py` & `granny-pliers-0.0.7/src/granny_pliers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/config/autowired_config.py` & `granny-pliers-0.0.7/src/granny_pliers/config/autowired_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/config/logger_config.py` & `granny-pliers-0.0.7/src/granny_pliers/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/config/project_environment.py` & `granny-pliers-0.0.7/src/granny_pliers/config/project_environment.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/logger/__init__.py` & `granny-pliers-0.0.7/src/granny_pliers/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/logger/abstract_logger.py` & `granny-pliers-0.0.7/src/granny_pliers/logger/abstract_logger.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/logger/log_processors.py` & `granny-pliers-0.0.7/src/granny_pliers/logger/log_processors.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/orm/__init__.py` & `granny-pliers-0.0.7/src/granny_pliers/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/orm/abstract_http_client.py` & `granny-pliers-0.0.7/src/granny_pliers/orm/abstract_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/orm/abstract_model.py` & `granny-pliers-0.0.7/src/granny_pliers/orm/abstract_model.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/orm/abstract_repository.py` & `granny-pliers-0.0.7/src/granny_pliers/orm/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/testing/__init__.py` & `granny-pliers-0.0.7/src/granny_pliers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/testing/abstract_test_case.py` & `granny-pliers-0.0.7/src/granny_pliers/testing/abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/testing/async_abstract_test_case.py` & `granny-pliers-0.0.7/src/granny_pliers/testing/async_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/worker/__init__.py` & `granny-pliers-0.0.7/src/granny_pliers/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers/worker/abstract_worker.py` & `granny-pliers-0.0.7/src/granny_pliers/worker/abstract_worker.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.6/src/granny_pliers.egg-info/PKG-INFO` & `granny-pliers-0.0.7/src/granny_pliers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.6/src/granny_pliers.egg-info/SOURCES.txt` & `granny-pliers-0.0.7/src/granny_pliers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

