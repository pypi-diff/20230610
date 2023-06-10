# Comparing `tmp/irvy-1.0.1.tar.gz` & `tmp/irvy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irvy-1.0.1.tar", last modified: Sat Jun 10 20:25:57 2023, max compression
+gzip compressed data, was "irvy-1.0.2.tar", last modified: Sat Jun 10 20:32:58 2023, max compression
```

## Comparing `irvy-1.0.1.tar` & `irvy-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:57.551653 irvy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-10 20:25:57.551653 irvy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-10 20:25:45.000000 irvy-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:57.551653 irvy-1.0.1/irvy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:57.551653 irvy-1.0.1/irvy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/generators/PlaywrightGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/generators/SeleniumGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/irvy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:57.551653 irvy-1.0.1/irvy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:45.000000 irvy-1.0.1/irvy/utils/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:25:57.551653 irvy-1.0.1/irvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-10 20:25:57.000000 irvy-1.0.1/irvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 20:25:57.000000 irvy-1.0.1/irvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:25:57.000000 irvy-1.0.1/irvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-10 20:25:57.000000 irvy-1.0.1/irvy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 20:25:57.000000 irvy-1.0.1/irvy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:25:57.551653 irvy-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 20:25:45.000000 irvy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-10 20:32:58.028215 irvy-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-10 20:32:48.000000 irvy-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/generators/PlaywrightGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/generators/SeleniumGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/irvy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/utils/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:32:58.032214 irvy-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 20:32:48.000000 irvy-1.0.2/setup.py
```

### Comparing `irvy-1.0.1/PKG-INFO` & `irvy-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-Metadata-Version: 2.1
-Name: irvy
-Version: 1.0.1
-Summary: A brief description of your project
-Description-Content-Type: text/markdown
-
 # Irvy
 
-Irvy is a command-line tool to setup projects for Selenium and Playwright in different languages.
+Irvy simplifies the setup process for test automation using Selenium or Playwright across multiple programming languages. It serves as a valuable tool for both novice automation engineers and seasoned professionals, facilitating a seamless transition between programming languages such as Java, C#, or JavaScript by providing comparable building blocks.
 
 In an ever-evolving technological landscape, the demand for efficient and versatile test automation tools has never been greater. Irvy, a command-line interface tool, steps up to this challenge by streamlining the setup process for test automation across a broad spectrum of programming languages. Whether you are a novice entering the world of automation engineering or a seasoned veteran, Irvy’s ability to provide comparable building blocks facilitates an effortless transition between different programming languages such as Java, C#, or JavaScript.
 
 Harnessing the capabilities of popular automation tools like Selenium and Playwright, Irvy empowers users to initiate projects in their language of choice with a simple, interactive command-line interface. This process alleviates the potential complexities associated with the setup phase, allowing users to focus their attention on the development of high-quality, robust automation scripts.
 
 In addition, Irvy fosters an environment of continuous learning and skill diversification. For seasoned professionals who have primarily worked in a single programming language, Irvy offers a comfortable, straightforward entry point to explore and adopt different languages. This not only widens their skillset but also broadens their perspective on the different strategies and approaches to test automation.
```

### Comparing `irvy-1.0.1/README.md` & `irvy-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+Metadata-Version: 2.1
+Name: irvy
+Version: 1.0.2
+Summary: A brief description of your project
+Description-Content-Type: text/markdown
+
 # Irvy
 
-Irvy is a command-line tool to setup projects for Selenium and Playwright in different languages.
+Irvy simplifies the setup process for test automation using Selenium or Playwright across multiple programming languages. It serves as a valuable tool for both novice automation engineers and seasoned professionals, facilitating a seamless transition between programming languages such as Java, C#, or JavaScript by providing comparable building blocks.
 
 In an ever-evolving technological landscape, the demand for efficient and versatile test automation tools has never been greater. Irvy, a command-line interface tool, steps up to this challenge by streamlining the setup process for test automation across a broad spectrum of programming languages. Whether you are a novice entering the world of automation engineering or a seasoned veteran, Irvy’s ability to provide comparable building blocks facilitates an effortless transition between different programming languages such as Java, C#, or JavaScript.
 
 Harnessing the capabilities of popular automation tools like Selenium and Playwright, Irvy empowers users to initiate projects in their language of choice with a simple, interactive command-line interface. This process alleviates the potential complexities associated with the setup phase, allowing users to focus their attention on the development of high-quality, robust automation scripts.
 
 In addition, Irvy fosters an environment of continuous learning and skill diversification. For seasoned professionals who have primarily worked in a single programming language, Irvy offers a comfortable, straightforward entry point to explore and adopt different languages. This not only widens their skillset but also broadens their perspective on the different strategies and approaches to test automation.
```

### Comparing `irvy-1.0.1/irvy/generators/PlaywrightGenerator.py` & `irvy-1.0.2/irvy/generators/PlaywrightGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.1/irvy/generators/SeleniumGenerator.py` & `irvy-1.0.2/irvy/generators/SeleniumGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.1/irvy/irvy.py` & `irvy-1.0.2/irvy/irvy.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.1/irvy.egg-info/PKG-INFO` & `irvy-1.0.2/irvy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: irvy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A brief description of your project
 Description-Content-Type: text/markdown
 
 # Irvy
 
-Irvy is a command-line tool to setup projects for Selenium and Playwright in different languages.
+Irvy simplifies the setup process for test automation using Selenium or Playwright across multiple programming languages. It serves as a valuable tool for both novice automation engineers and seasoned professionals, facilitating a seamless transition between programming languages such as Java, C#, or JavaScript by providing comparable building blocks.
 
 In an ever-evolving technological landscape, the demand for efficient and versatile test automation tools has never been greater. Irvy, a command-line interface tool, steps up to this challenge by streamlining the setup process for test automation across a broad spectrum of programming languages. Whether you are a novice entering the world of automation engineering or a seasoned veteran, Irvy’s ability to provide comparable building blocks facilitates an effortless transition between different programming languages such as Java, C#, or JavaScript.
 
 Harnessing the capabilities of popular automation tools like Selenium and Playwright, Irvy empowers users to initiate projects in their language of choice with a simple, interactive command-line interface. This process alleviates the potential complexities associated with the setup phase, allowing users to focus their attention on the development of high-quality, robust automation scripts.
 
 In addition, Irvy fosters an environment of continuous learning and skill diversification. For seasoned professionals who have primarily worked in a single programming language, Irvy offers a comfortable, straightforward entry point to explore and adopt different languages. This not only widens their skillset but also broadens their perspective on the different strategies and approaches to test automation.
```

### Comparing `irvy-1.0.1/setup.py` & `irvy-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Open the README file.
 with open(file="README.md", mode="r") as readme_handle:
     long_description = readme_handle.read()
 
 setup(
     name='irvy',
-    version='1.0.1',
+    version='1.0.2',
     description='A brief description of your project',  # add this
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # this should automatically find your packages
     include_package_data=True,
     install_requires=[
         # list of dependencies
```

