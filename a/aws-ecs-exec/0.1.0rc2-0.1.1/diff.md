# Comparing `tmp/aws_ecs_exec-0.1.0rc2.tar.gz` & `tmp/aws_ecs_exec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ecs_exec-0.1.0rc2.tar", max compression
+gzip compressed data, was "aws_ecs_exec-0.1.1.tar", max compression
```

## Comparing `aws_ecs_exec-0.1.0rc2.tar` & `aws_ecs_exec-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      709 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/README.md
--rw-r--r--   0        0        0       20 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/__init__.py
--rwxr-xr-x   0        0        0     7259 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/cli.py
--rwxr-xr-x   0        0        0     3168 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/colors.py
--rwxr-xr-x   0        0        0      288 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/exceptions.py
--rwxr-xr-x   0        0        0     2429 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/utils.py
--rwxr-xr-x   0        0        0     3077 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/aws_ecs_exec/widgets.py
--rw-r--r--   0        0        0      885 2023-06-10 07:35:12.898194 aws_ecs_exec-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 aws_ecs_exec-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/README.md
+-rw-r--r--   0        0        0       20 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/aws_ecs_exec/__init__.py
+-rwxr-xr-x   0        0        0     7548 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/aws_ecs_exec/cli.py
+-rwxr-xr-x   0        0        0     3168 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/aws_ecs_exec/colors.py
+-rwxr-xr-x   0        0        0      288 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/aws_ecs_exec/exceptions.py
+-rwxr-xr-x   0        0        0     2429 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/aws_ecs_exec/utils.py
+-rwxr-xr-x   0        0        0     3077 2023-06-10 08:01:43.029535 aws_ecs_exec-0.1.1/aws_ecs_exec/widgets.py
+-rw-r--r--   0        0        0      881 2023-06-10 08:01:43.033535 aws_ecs_exec-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 aws_ecs_exec-0.1.1/PKG-INFO
```

### Comparing `aws_ecs_exec-0.1.0rc2/README.md` & `aws_ecs_exec-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/cli.py` & `aws_ecs_exec-0.1.1/aws_ecs_exec/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functions for executing command in AWS ECS Tasks."""
 import argparse
 import logging
 import os
 import shlex
 from functools import partial
+from importlib.metadata import version
 from typing import Callable
 
 import boto3
 from botocore.exceptions import ProfileNotFound
 
 from aws_ecs_exec import exceptions, utils
 from aws_ecs_exec.colors import colored, get_colored_logger
@@ -92,14 +93,19 @@
     parser.add_argument(
         "-v",
         "--verbose",
         help="Log debug statements (default: False)",
         action="store_true",
         default=False,
     )
+    parser.add_argument(
+        "--version",
+        help="Print the current version of aws-ecs-exec and exit",
+        action="store_true",
+    )
     return parser.parse_args()
 
 
 def execute_command(
     *,
     aws_profile: str,
     cluster: str,
@@ -139,14 +145,18 @@
 
 # pylint: disable-next=too-many-return-statements
 def entrypoint():
     """Execute a command in an AWS ECS Task."""
     try:
         args = get_args()
 
+        if args.version:
+            print("Version:", version("aws-ecs-exec"))
+            return 0
+
         if args.verbose:
             logger.setLevel(logging.DEBUG)
 
         if args.colors is not None:
             if args.colors:
                 os.environ.pop("NO_COLOR", None)
             else:
```

### Comparing `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/colors.py` & `aws_ecs_exec-0.1.1/aws_ecs_exec/colors.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/utils.py` & `aws_ecs_exec-0.1.1/aws_ecs_exec/utils.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc2/aws_ecs_exec/widgets.py` & `aws_ecs_exec-0.1.1/aws_ecs_exec/widgets.py`

 * *Files identical despite different names*

### Comparing `aws_ecs_exec-0.1.0rc2/pyproject.toml` & `aws_ecs_exec-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-ecs-exec"
-version = "0.1.0rc2"
+version = "0.1.1"
 description = "A cli tool to conveniently execute commands in AWS ECS Tasks"
 authors = ["Nat Gordon <nat@nattyg93.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_ecs_exec"}]
 
 [tool.poetry.dependencies]
@@ -25,15 +25,14 @@
 [tool.poetry.scripts]
 ecs-exec = "aws_ecs_exec.cli:entrypoint"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-
 [tool.isort]
 profile = "black"
 
 [tool.pylint."messages control"]
 enable = "useless-suppression"
 fail-on = "useless-suppression"
```

### Comparing `aws_ecs_exec-0.1.0rc2/PKG-INFO` & `aws_ecs_exec-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ecs-exec
-Version: 0.1.0rc2
+Version: 0.1.1
 Summary: A cli tool to conveniently execute commands in AWS ECS Tasks
 License: MIT
 Author: Nat Gordon
 Author-email: nat@nattyg93.com.au
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

