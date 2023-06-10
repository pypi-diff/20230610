# Comparing `tmp/django-nepali-0.0.0.tar.gz` & `tmp/django-nepali-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nepali-0.0.0.tar", last modified: Mon May 15 14:56:45 2023, max compression
+gzip compressed data, was "django-nepali-0.0.1.tar", last modified: Sat Jun 10 15:58:50 2023, max compression
```

## Comparing `django-nepali-0.0.0.tar` & `django-nepali-0.0.1.tar`

### file list

```diff
@@ -1,9 +1,18 @@
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-05-15 14:56:45.267314 django-nepali-0.0.0/
--rw-r--r--   0 aj3sh      (501) staff       (20)      545 2023-05-15 14:56:45.267172 django-nepali-0.0.0/PKG-INFO
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-05-15 14:56:45.266994 django-nepali-0.0.0/django_nepali.egg-info/
--rw-r--r--   0 aj3sh      (501) staff       (20)      545 2023-05-15 14:56:45.000000 django-nepali-0.0.0/django_nepali.egg-info/PKG-INFO
--rw-r--r--   0 aj3sh      (501) staff       (20)      156 2023-05-15 14:56:45.000000 django-nepali-0.0.0/django_nepali.egg-info/SOURCES.txt
--rw-r--r--   0 aj3sh      (501) staff       (20)        1 2023-05-15 14:56:45.000000 django-nepali-0.0.0/django_nepali.egg-info/dependency_links.txt
--rw-r--r--   0 aj3sh      (501) staff       (20)        1 2023-05-15 14:56:45.000000 django-nepali-0.0.0/django_nepali.egg-info/top_level.txt
--rw-r--r--   0 aj3sh      (501) staff       (20)       38 2023-05-15 14:56:45.267355 django-nepali-0.0.0/setup.cfg
--rwxr-xr-x   0 aj3sh      (501) staff       (20)     1424 2023-05-15 14:56:28.000000 django-nepali-0.0.0/setup.py
+drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-06-10 15:58:50.573197 django-nepali-0.0.1/
+-rw-r--r--   0 aj3sh      (501) staff       (20)    35149 2023-05-22 15:23:44.000000 django-nepali-0.0.1/LICENSE
+-rw-r--r--   0 aj3sh      (501) staff       (20)     4348 2023-06-10 15:58:50.572961 django-nepali-0.0.1/PKG-INFO
+-rw-r--r--   0 aj3sh      (501) staff       (20)     3589 2023-06-10 15:53:15.000000 django-nepali-0.0.1/README.md
+drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-06-10 15:58:50.571207 django-nepali-0.0.1/django_nepali/
+-rw-r--r--   0 aj3sh      (501) staff       (20)        0 2023-06-10 15:53:15.000000 django-nepali-0.0.1/django_nepali/__init__.py
+drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-06-10 15:58:50.572587 django-nepali-0.0.1/django_nepali/templatetags/
+-rwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-06-10 15:53:15.000000 django-nepali-0.0.1/django_nepali/templatetags/__init__.py
+-rwxr-xr-x   0 aj3sh      (501) staff       (20)     4710 2023-06-10 15:53:15.000000 django-nepali-0.0.1/django_nepali/templatetags/nepalidatetime.py
+-rw-r--r--   0 aj3sh      (501) staff       (20)     1757 2023-06-10 15:53:15.000000 django-nepali-0.0.1/django_nepali/templatetags/nepalinumber.py
+drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2023-06-10 15:58:50.571990 django-nepali-0.0.1/django_nepali.egg-info/
+-rw-r--r--   0 aj3sh      (501) staff       (20)     4348 2023-06-10 15:58:50.000000 django-nepali-0.0.1/django_nepali.egg-info/PKG-INFO
+-rw-r--r--   0 aj3sh      (501) staff       (20)      363 2023-06-10 15:58:50.000000 django-nepali-0.0.1/django_nepali.egg-info/SOURCES.txt
+-rw-r--r--   0 aj3sh      (501) staff       (20)        1 2023-06-10 15:58:50.000000 django-nepali-0.0.1/django_nepali.egg-info/dependency_links.txt
+-rw-r--r--   0 aj3sh      (501) staff       (20)       21 2023-06-10 15:58:50.000000 django-nepali-0.0.1/django_nepali.egg-info/requires.txt
+-rw-r--r--   0 aj3sh      (501) staff       (20)       14 2023-06-10 15:58:50.000000 django-nepali-0.0.1/django_nepali.egg-info/top_level.txt
+-rw-r--r--   0 aj3sh      (501) staff       (20)       38 2023-06-10 15:58:50.573248 django-nepali-0.0.1/setup.cfg
+-rw-r--r--   0 aj3sh      (501) staff       (20)     1743 2023-06-10 15:58:24.000000 django-nepali-0.0.1/setup.py
```

### Comparing `django-nepali-0.0.0/setup.py` & `django-nepali-0.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,45 +14,52 @@
     twine upload dist/*
 
 """
 import os
 import sys
 import setuptools
 
-long_description = "# django-nepali"
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 
 if sys.argv[-1] == "publish":
     if os.system("pip3 freeze | grep twine"):
         print("twine not installed.\nUse `pip install twine`.\nExiting.")
         sys.exit()
     os.system("rm -rf dist")
     os.system("python3 setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
 
 
 setuptools.setup(
     name="django-nepali",
-    version="0.0.0",
+    version="0.0.1",
     author="opensource-nepal",
-    author_email="aj3sshh@gmail.com",
-    description="Django package for supporting nepali package",
+    author_email="aj3sshh@gmail.com, sugatbajracharya49@gmail.com",
+    description="A django package on top of 'nepali' a python package which supports nepali date time, time conversion, etc on django projects.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "django",
         "nepali date conversion",
         "convert date",
         "nepali date time",
         "python convert date",
         "parse nepali date time",
     ],
     url="https://github.com/opensource-nepal/django-nepali",
-    packages=setuptools.find_packages(),
-    install_requires=[],
+    packages=setuptools.find_packages(exclude=["django_nepali_example"]),
+    install_requires=[
+        'django',
+        'nepali>=1.0.0',
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU General Public License (GPL)",
+        "Environment :: Web Environment",
         "Operating System :: OS Independent",
+        "Framework :: Django",
     ],
 )
```

