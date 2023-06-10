# Comparing `tmp/netsim-tools-1.5.3.post1.tar.gz` & `tmp/netsim-tools-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim-tools-1.5.3.post1.tar", last modified: Tue May 16 06:09:07 2023, max compression
+gzip compressed data, was "netsim-tools-1.5.4.tar", last modified: Sat Jun 10 16:47:35 2023, max compression
```

## Comparing `netsim-tools-1.5.3.post1.tar` & `netsim-tools-1.5.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:09:07.576027 netsim-tools-1.5.3.post1/
--rw-r--r--   0 pipi       (501) staff       (20)      499 2023-05-16 06:09:07.575914 netsim-tools-1.5.3.post1/PKG-INFO
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:09:07.575770 netsim-tools-1.5.3.post1/netsim_tools.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)      499 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)      187 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       24 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-05-16 06:09:07.576065 netsim-tools-1.5.3.post1/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1298 2023-05-16 06:07:28.000000 netsim-tools-1.5.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:35.097739 netsim-tools-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-10 16:47:35.093739 netsim-tools-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-10 16:47:05.000000 netsim-tools-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:35.093739 netsim-tools-1.5.4/netsim_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:47:35.000000 netsim-tools-1.5.4/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:47:35.097739 netsim-tools-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-10 16:47:05.000000 netsim-tools-1.5.4/setup.py
```

### Comparing `netsim-tools-1.5.3.post1/setup.py` & `netsim-tools-1.5.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
+from pathlib import Path
 
 sys.path.append('..')
 
-version="1.5.3-post1"
+version="1.5.4"
+
+long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
   author="Ivan Pepelnjak",
   author_email="ip@ipspace.net",
   description="CLI-based Virtual Networking Lab Abstraction Layer",
+  long_description=long_description,
   install_requires=[f"networklab>={version}"],
   classifiers=[
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
   ],
   url="https://github.com/ipspace/netlab",
   python_requires='>=3.7',  # Due to e.g. 'capture_output' in subprocess.run
 )
-
-print("""
-=======================================================================
-                          WARNING WARNING WARNING
-=======================================================================
-netsim-tools has been renamed to netlab in August 2022.
-
-The Python package netsim-tools has been renamed to networklab and is
-installed as a dependency of netsim-tools every time you install or
-upgrade netsim-tools, but we won't keep that dependency active foreer.
-
-Please stop using netsim-tools package and use networklab package.
-""")
```

