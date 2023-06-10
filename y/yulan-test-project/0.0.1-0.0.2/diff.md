# Comparing `tmp/yulan_test_project-0.0.1.tar.gz` & `tmp/yulan_test_project-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yulan_test_project-0.0.1.tar", last modified: Sat Jun 10 06:42:07 2023, max compression
+gzip compressed data, was "yulan_test_project-0.0.2.tar", last modified: Sat Jun 10 11:42:34 2023, max compression
```

## Comparing `yulan_test_project-0.0.1.tar` & `yulan_test_project-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-06-10 06:42:07.299333 yulan_test_project-0.0.1/
--rw-rw-r--   0 yulai     (1000) yulai     (1000)      179 2023-06-10 06:42:07.295333 yulan_test_project-0.0.1/PKG-INFO
--rw-rw-r--   0 yulai     (1000) yulai     (1000)        0 2023-06-08 16:14:58.000000 yulan_test_project-0.0.1/README.md
--rw-rw-r--   0 yulai     (1000) yulai     (1000)      363 2023-06-10 06:41:36.000000 yulan_test_project-0.0.1/pyproject.toml
--rw-rw-r--   0 yulai     (1000) yulai     (1000)       38 2023-06-10 06:42:07.299333 yulan_test_project-0.0.1/setup.cfg
-drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-06-10 06:42:07.291333 yulan_test_project-0.0.1/yulan_test_project/
--rw-rw-r--   0 yulai     (1000) yulai     (1000)        0 2023-06-08 16:09:17.000000 yulan_test_project-0.0.1/yulan_test_project/__init__.py
--rw-rw-r--   0 yulai     (1000) yulai     (1000)       98 2023-06-10 06:37:49.000000 yulan_test_project-0.0.1/yulan_test_project/__main__.py
--rw-rw-r--   0 yulai     (1000) yulai     (1000)       45 2023-06-10 06:37:27.000000 yulan_test_project-0.0.1/yulan_test_project/helloworld.py
-drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-06-10 06:42:07.295333 yulan_test_project-0.0.1/yulan_test_project.egg-info/
--rw-rw-r--   0 yulai     (1000) yulai     (1000)      179 2023-06-10 06:42:07.000000 yulan_test_project-0.0.1/yulan_test_project.egg-info/PKG-INFO
--rw-rw-r--   0 yulai     (1000) yulai     (1000)      373 2023-06-10 06:42:07.000000 yulan_test_project-0.0.1/yulan_test_project.egg-info/SOURCES.txt
--rw-rw-r--   0 yulai     (1000) yulai     (1000)        1 2023-06-10 06:42:07.000000 yulan_test_project-0.0.1/yulan_test_project.egg-info/dependency_links.txt
--rw-rw-r--   0 yulai     (1000) yulai     (1000)       59 2023-06-10 06:42:07.000000 yulan_test_project-0.0.1/yulan_test_project.egg-info/entry_points.txt
--rw-rw-r--   0 yulai     (1000) yulai     (1000)       16 2023-06-10 06:42:07.000000 yulan_test_project-0.0.1/yulan_test_project.egg-info/requires.txt
--rw-rw-r--   0 yulai     (1000) yulai     (1000)       19 2023-06-10 06:42:07.000000 yulan_test_project-0.0.1/yulan_test_project.egg-info/top_level.txt
+drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-06-10 11:42:34.511396 yulan_test_project-0.0.2/
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      179 2023-06-10 11:42:34.507396 yulan_test_project-0.0.2/PKG-INFO
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)        0 2023-06-08 16:14:58.000000 yulan_test_project-0.0.2/README.md
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      363 2023-06-10 11:36:50.000000 yulan_test_project-0.0.2/pyproject.toml
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       38 2023-06-10 11:42:34.511396 yulan_test_project-0.0.2/setup.cfg
+drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-06-10 11:42:34.503395 yulan_test_project-0.0.2/yulan_test_project/
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)        0 2023-06-08 16:09:17.000000 yulan_test_project-0.0.2/yulan_test_project/__init__.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       98 2023-06-10 06:37:49.000000 yulan_test_project-0.0.2/yulan_test_project/__main__.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      109 2023-06-10 11:38:01.000000 yulan_test_project-0.0.2/yulan_test_project/helloworld.py
+drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-06-10 11:42:34.507396 yulan_test_project-0.0.2/yulan_test_project.egg-info/
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      179 2023-06-10 11:42:34.000000 yulan_test_project-0.0.2/yulan_test_project.egg-info/PKG-INFO
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      373 2023-06-10 11:42:34.000000 yulan_test_project-0.0.2/yulan_test_project.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)        1 2023-06-10 11:42:34.000000 yulan_test_project-0.0.2/yulan_test_project.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       59 2023-06-10 11:42:34.000000 yulan_test_project-0.0.2/yulan_test_project.egg-info/entry_points.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       16 2023-06-10 11:42:34.000000 yulan_test_project-0.0.2/yulan_test_project.egg-info/requires.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       19 2023-06-10 11:42:34.000000 yulan_test_project-0.0.2/yulan_test_project.egg-info/top_level.txt
```

