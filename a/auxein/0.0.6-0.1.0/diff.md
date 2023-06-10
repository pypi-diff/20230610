# Comparing `tmp/Auxein-0.0.6.tar.gz` & `tmp/auxein-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Auxein-0.0.6.tar", last modified: Sun Apr 26 21:26:51 2020, max compression
+gzip compressed data, was "auxein-0.1.0.tar", max compression
```

## Comparing `Auxein-0.0.6.tar` & `auxein-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,28 @@
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      427 2020-04-26 21:26:51.000000 Auxein-0.0.6/PKG-INFO
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/parents/
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/parents/selections/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      142 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/parents/selections/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1460 2020-04-22 15:09:07.000000 Auxein-0.0.6/auxein/parents/selections/core.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)      106 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/parents/__init__.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/parents/distributions/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      134 2019-04-16 16:32:33.000000 Auxein-0.0.6/auxein/parents/distributions/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1924 2019-04-16 16:36:38.000000 Auxein-0.0.6/auxein/parents/distributions/core.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/replacements/
--rw-r--r--   0 dpalmisano   (501) staff       (20)       76 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/replacements/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1624 2020-04-22 14:19:40.000000 Auxein-0.0.6/auxein/replacements/core.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/mutations/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      140 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/mutations/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     2703 2019-04-18 12:21:33.000000 Auxein-0.0.6/auxein/mutations/core.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/recombinations/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      120 2020-04-25 21:36:27.000000 Auxein-0.0.6/auxein/recombinations/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     3180 2020-04-25 21:36:27.000000 Auxein-0.0.6/auxein/recombinations/core.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)      428 2020-04-12 09:18:46.000000 Auxein-0.0.6/auxein/__init__.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/population/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      640 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/population/genotype.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)      305 2020-04-08 18:30:55.000000 Auxein-0.0.6/auxein/population/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     5244 2020-04-22 15:09:07.000000 Auxein-0.0.6/auxein/population/core.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1488 2020-04-08 18:30:55.000000 Auxein-0.0.6/auxein/population/dna_builders.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1441 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/population/individual.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/playgrounds/
--rw-r--r--   0 dpalmisano   (501) staff       (20)       42 2019-04-16 15:26:42.000000 Auxein-0.0.6/auxein/playgrounds/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     5138 2020-04-22 15:09:07.000000 Auxein-0.0.6/auxein/playgrounds/static.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/fitness/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      672 2020-04-26 21:24:50.000000 Auxein-0.0.6/auxein/fitness/kernel_based.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     3411 2020-04-26 21:24:50.000000 Auxein-0.0.6/auxein/fitness/observation_based.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)      216 2020-04-26 21:24:50.000000 Auxein-0.0.6/auxein/fitness/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)      476 2020-04-26 21:24:50.000000 Auxein-0.0.6/auxein/fitness/core.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/auxein/fitness/utils/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      166 2020-04-22 15:09:07.000000 Auxein-0.0.6/auxein/fitness/utils/__init__.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1393 2020-04-22 15:09:07.000000 Auxein-0.0.6/auxein/fitness/utils/utils.py
--rw-r--r--   0 dpalmisano   (501) staff       (20)     1715 2020-04-22 15:09:07.000000 Auxein-0.0.6/README.md
--rw-r--r--   0 dpalmisano   (501) staff       (20)      679 2020-04-26 21:26:46.000000 Auxein-0.0.6/setup.py
-drwxr-xr-x   0 dpalmisano   (501) staff       (20)        0 2020-04-26 21:26:51.000000 Auxein-0.0.6/Auxein.egg-info/
--rw-r--r--   0 dpalmisano   (501) staff       (20)      427 2020-04-26 21:26:50.000000 Auxein-0.0.6/Auxein.egg-info/PKG-INFO
--rw-r--r--   0 dpalmisano   (501) staff       (20)      933 2020-04-26 21:26:50.000000 Auxein-0.0.6/Auxein.egg-info/SOURCES.txt
--rw-r--r--   0 dpalmisano   (501) staff       (20)       41 2020-04-26 21:26:50.000000 Auxein-0.0.6/Auxein.egg-info/requires.txt
--rw-r--r--   0 dpalmisano   (501) staff       (20)        7 2020-04-26 21:26:50.000000 Auxein-0.0.6/Auxein.egg-info/top_level.txt
--rw-r--r--   0 dpalmisano   (501) staff       (20)        1 2020-04-26 21:26:50.000000 Auxein-0.0.6/Auxein.egg-info/dependency_links.txt
--rw-r--r--   0 dpalmisano   (501) staff       (20)       38 2020-04-26 21:26:51.000000 Auxein-0.0.6/setup.cfg
+-rw-r--r--   0        0        0    11346 2023-06-10 19:35:09.851119 auxein-0.1.0/LICENSE
+-rw-r--r--   0        0        0      428 2023-06-10 19:35:09.851376 auxein-0.1.0/auxein/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-10 19:35:09.851485 auxein-0.1.0/auxein/fitness/__init__.py
+-rw-r--r--   0        0        0      476 2023-06-10 19:35:09.851565 auxein-0.1.0/auxein/fitness/core.py
+-rw-r--r--   0        0        0      672 2023-06-10 19:35:09.851633 auxein-0.1.0/auxein/fitness/kernel_based.py
+-rw-r--r--   0        0        0     3411 2023-06-10 19:35:09.851706 auxein-0.1.0/auxein/fitness/observation_based.py
+-rw-r--r--   0        0        0      166 2023-06-10 19:35:09.851807 auxein-0.1.0/auxein/fitness/utils/__init__.py
+-rw-r--r--   0        0        0     1393 2023-06-10 19:35:09.851872 auxein-0.1.0/auxein/fitness/utils/utils.py
+-rw-r--r--   0        0        0      140 2023-06-10 19:35:09.851986 auxein-0.1.0/auxein/mutations/__init__.py
+-rw-r--r--   0        0        0     2703 2023-06-10 19:35:09.852067 auxein-0.1.0/auxein/mutations/core.py
+-rw-r--r--   0        0        0      106 2023-06-10 19:35:09.852173 auxein-0.1.0/auxein/parents/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-10 19:35:09.852288 auxein-0.1.0/auxein/parents/distributions/__init__.py
+-rw-r--r--   0        0        0     1924 2023-06-10 19:35:09.852364 auxein-0.1.0/auxein/parents/distributions/core.py
+-rw-r--r--   0        0        0      142 2023-06-10 19:35:09.852473 auxein-0.1.0/auxein/parents/selections/__init__.py
+-rw-r--r--   0        0        0     1460 2023-06-10 19:35:09.852545 auxein-0.1.0/auxein/parents/selections/core.py
+-rw-r--r--   0        0        0       42 2023-06-10 19:35:09.852648 auxein-0.1.0/auxein/playgrounds/__init__.py
+-rw-r--r--   0        0        0     5138 2023-06-10 19:35:09.852721 auxein-0.1.0/auxein/playgrounds/static.py
+-rw-r--r--   0        0        0      305 2023-06-10 19:35:09.852815 auxein-0.1.0/auxein/population/__init__.py
+-rw-r--r--   0        0        0     5244 2023-06-10 19:35:09.852888 auxein-0.1.0/auxein/population/core.py
+-rw-r--r--   0        0        0     1488 2023-06-10 19:35:09.852958 auxein-0.1.0/auxein/population/dna_builders.py
+-rw-r--r--   0        0        0      640 2023-06-10 19:35:09.853027 auxein-0.1.0/auxein/population/genotype.py
+-rw-r--r--   0        0        0     1441 2023-06-10 19:35:09.853099 auxein-0.1.0/auxein/population/individual.py
+-rw-r--r--   0        0        0      120 2023-06-10 19:35:09.853193 auxein-0.1.0/auxein/recombinations/__init__.py
+-rw-r--r--   0        0        0     3180 2023-06-10 19:35:09.853265 auxein-0.1.0/auxein/recombinations/core.py
+-rw-r--r--   0        0        0       76 2023-06-10 19:35:09.853360 auxein-0.1.0/auxein/replacements/__init__.py
+-rw-r--r--   0        0        0     1624 2023-06-10 19:35:09.853448 auxein-0.1.0/auxein/replacements/core.py
+-rw-r--r--   0        0        0      472 2023-06-10 20:41:10.670390 auxein-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 auxein-0.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Auxein-0.0.6/auxein/parents/selections/core.py` & `auxein-0.1.0/auxein/parents/selections/core.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/parents/distributions/core.py` & `auxein-0.1.0/auxein/parents/distributions/core.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/replacements/core.py` & `auxein-0.1.0/auxein/replacements/core.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/mutations/core.py` & `auxein-0.1.0/auxein/mutations/core.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/recombinations/core.py` & `auxein-0.1.0/auxein/recombinations/core.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/population/genotype.py` & `auxein-0.1.0/auxein/population/genotype.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/population/core.py` & `auxein-0.1.0/auxein/population/core.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/population/dna_builders.py` & `auxein-0.1.0/auxein/population/dna_builders.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/population/individual.py` & `auxein-0.1.0/auxein/population/individual.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/playgrounds/static.py` & `auxein-0.1.0/auxein/playgrounds/static.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/fitness/kernel_based.py` & `auxein-0.1.0/auxein/fitness/kernel_based.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/fitness/observation_based.py` & `auxein-0.1.0/auxein/fitness/observation_based.py`

 * *Files identical despite different names*

### Comparing `Auxein-0.0.6/auxein/fitness/utils/utils.py` & `auxein-0.1.0/auxein/fitness/utils/utils.py`

 * *Files identical despite different names*

