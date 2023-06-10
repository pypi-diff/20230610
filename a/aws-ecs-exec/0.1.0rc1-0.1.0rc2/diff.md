# Comparing `tmp/aws_ecs_exec-0.1.0rc1.tar.gz` & `tmp/aws_ecs_exec-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ecs_exec-0.1.0rc1.tar", max compression
+gzip compressed data, was "aws_ecs_exec-0.1.0rc2.tar", max compression
```

## Comparing `aws_ecs_exec-0.1.0rc1.tar` & `aws_ecs_exec-0.1.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      709 2023-06-10 04:28:44.816531 aws_ecs_exec-0.1.0rc1/README.md
--rw-r--r--   0        0        0       20 2023-06-10 04:28:35.358806 aws_ecs_exec-0.1.0rc1/aws_ecs_exec/__init__.py
--rwxr-xr-x   0        0        0     7259 2023-06-10 05:16:39.764665 aws_ecs_exec-0.1.0rc1/aws_ecs_exec/cli.py
--rwxr-xr-x   0        0        0     3168 2023-06-10 05:00:56.721699 aws_ecs_exec-0.1.0rc1/aws_ecs_exec/colors.py
--rwxr-xr-x   0        0        0      288 2023-06-10 04:28:44.816804 aws_ecs_exec-0.1.0rc1/aws_ecs_exec/exceptions.py
--rwxr-xr-x   0        0        0     2429 2023-06-10 04:51:29.403098 aws_ecs_exec-0.1.0rc1/aws_ecs_exec/utils.py
--rwxr-xr-x   0        0        0     3077 2023-06-10 04:51:29.403428 aws_ecs_exec-0.1.0rc1/aws_ecs_exec/widgets.py
--rw-r--r--   0        0        0      885 2023-06-10 05:26:42.654223 aws_ecs_exec-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 aws_ecs_exec-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/README.md
+-rw-r--r--   0        0        0       20 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/__init__.py
+-rwxr-xr-x   0        0        0     7259 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/cli.py
+-rwxr-xr-x   0        0        0     3168 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/colors.py
+-rwxr-xr-x   0        0        0      288 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/exceptions.py
+-rwxr-xr-x   0        0        0     2429 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/utils.py
+-rwxr-xr-x   0        0        0     3077 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/widgets.py
+-rw-r--r--   0        0        0      885 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 aws_ecs_exec-0.1.0rc2/PKG-INFO
```

### Comparing `aws_ecs_exec-0.1.0rc1/README.md` & `aws_ecs_exec-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc1/aws_ecs_exec/cli.py` & `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/cli.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc1/aws_ecs_exec/colors.py` & `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/colors.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc1/aws_ecs_exec/utils.py` & `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/utils.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc1/aws_ecs_exec/widgets.py` & `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/widgets.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc1/pyproject.toml` & `aws_ecs_exec-0.1.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-ecs-exec"
-version = "0.1.0rc1"
+version = "0.1.0rc2"
 description = "A cli tool to conveniently execute commands in AWS ECS Tasks"
 authors = ["Nat Gordon <nat@nattyg93.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_ecs_exec"}]
 
 [tool.poetry.dependencies]
```

### Comparing `aws_ecs_exec-0.1.0rc1/PKG-INFO` & `aws_ecs_exec-0.1.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-exec
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: A cli tool to conveniently execute commands in AWS ECS Tasks
 License: MIT
 Author: Nat Gordon
 Author-email: nat@nattyg93.com.au
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

