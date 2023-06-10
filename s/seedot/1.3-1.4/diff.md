# Comparing `tmp/seedot-1.3.tar.gz` & `tmp/seedot-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedot-1.3.tar", last modified: Sat Jun 10 14:04:27 2023, max compression
+gzip compressed data, was "seedot-1.4.tar", last modified: Sat Jun 10 14:25:55 2023, max compression
```

## Comparing `seedot-1.3.tar` & `seedot-1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:04:27.787830 seedot-1.3/
--rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-1.3/LICENSE.txt
--rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-1.3/MANIFEST.in
--rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 14:04:27.788040 seedot-1.3/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)     6043 2023-06-09 16:55:58.000000 seedot-1.3/README.rst
--rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-1.3/__init__.py
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:04:27.783795 seedot-1.3/seedot/
--rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-1.3/seedot/SEEDOT_lexicon_electronic.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-1.3/seedot/SEEDOT_lexicon_finance.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-1.3/seedot/SEEDOT_lexicon_food.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-1.3/seedot/SEEDOT_lexicon_hotel.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-1.3/seedot/__init__.py
--rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-1.3/seedot/emoji_utf8_lexicon.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-10 14:02:50.000000 seedot-1.3/seedot/seedot_electronic.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-10 14:02:13.000000 seedot-1.3/seedot/seedot_finance.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-10 14:02:32.000000 seedot-1.3/seedot/seedot_food.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34313 2023-06-10 14:03:23.000000 seedot-1.3/seedot/seedot_hotel.py
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:04:27.787377 seedot-1.3/seedot.egg-info/
--rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)      495 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/SOURCES.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/dependency_links.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/requires.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/top_level.txt
--rw-rw-r--   0 Vittom     (505) staff       (20)     1563 2023-06-10 14:04:27.788660 seedot-1.3/setup.cfg
--rw-rw-rw-   0 Vittom     (505) staff       (20)     1875 2023-06-10 14:04:14.000000 seedot-1.3/setup.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:25:55.561166 seedot-1.4/
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-1.4/LICENSE.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-1.4/MANIFEST.in
+-rw-r--r--   0 Vittom     (505) staff       (20)     7079 2023-06-10 14:25:55.561325 seedot-1.4/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)     6043 2023-06-09 16:55:58.000000 seedot-1.4/README.rst
+-rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-1.4/__init__.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:25:55.559210 seedot-1.4/seedot/
+-rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-1.4/seedot/SEEDOT_lexicon_electronic.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-1.4/seedot/SEEDOT_lexicon_finance.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-1.4/seedot/SEEDOT_lexicon_food.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-1.4/seedot/SEEDOT_lexicon_hotel.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-1.4/seedot/__init__.py
+-rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-1.4/seedot/emoji_utf8_lexicon.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-10 14:02:50.000000 seedot-1.4/seedot/seedot_electronic.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-10 14:02:13.000000 seedot-1.4/seedot/seedot_finance.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-10 14:02:32.000000 seedot-1.4/seedot/seedot_food.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34313 2023-06-10 14:03:23.000000 seedot-1.4/seedot/seedot_hotel.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:25:55.560857 seedot-1.4/seedot.egg-info/
+-rw-r--r--   0 Vittom     (505) staff       (20)     7079 2023-06-10 14:25:55.000000 seedot-1.4/seedot.egg-info/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)      495 2023-06-10 14:25:55.000000 seedot-1.4/seedot.egg-info/SOURCES.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-10 14:25:55.000000 seedot-1.4/seedot.egg-info/dependency_links.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-10 14:25:55.000000 seedot-1.4/seedot.egg-info/requires.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-10 14:25:55.000000 seedot-1.4/seedot.egg-info/top_level.txt
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1359 2023-06-10 14:25:55.561885 seedot-1.4/setup.cfg
+-rw-rw-rw-   0 Vittom     (505) staff       (20)     1849 2023-06-10 14:25:35.000000 seedot-1.4/setup.py
```

### Comparing `seedot-1.3/LICENSE.txt` & `seedot-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.3/README.rst` & `seedot-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/SEEDOT_lexicon_electronic.txt` & `seedot-1.4/seedot/SEEDOT_lexicon_electronic.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/SEEDOT_lexicon_finance.txt` & `seedot-1.4/seedot/SEEDOT_lexicon_finance.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/SEEDOT_lexicon_food.txt` & `seedot-1.4/seedot/SEEDOT_lexicon_food.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/SEEDOT_lexicon_hotel.txt` & `seedot-1.4/seedot/SEEDOT_lexicon_hotel.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/emoji_utf8_lexicon.txt` & `seedot-1.4/seedot/emoji_utf8_lexicon.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/seedot_electronic.py` & `seedot-1.4/seedot/seedot_electronic.py`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/seedot_finance.py` & `seedot-1.4/seedot/seedot_finance.py`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/seedot_food.py` & `seedot-1.4/seedot/seedot_food.py`

 * *Files identical despite different names*

### Comparing `seedot-1.3/seedot/seedot_hotel.py` & `seedot-1.4/seedot/seedot_hotel.py`

 * *Files identical despite different names*

### Comparing `seedot-1.3/setup.cfg` & `seedot-1.4/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 name = seedot
 author = Seedot
 Author-email = seedotvsvader@gmail.com
 license = MIT
 license-file = LICENSE.txt
 url = https://github.com/SEEDOT1/SEEDOT
 description = This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
-long_description = This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Text Processing :: Linguistic
```

### Comparing `seedot-1.3/setup.py` & `seedot-1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,20 @@
         return f.read()
 
 setup(
   name = 'seedot',
   #packages = ['GROGU'], # this must be the same as the name above
   packages = find_packages(exclude=['tests*']), # a better way to do it than the line above -- this way no typo/transpo errors
   include_package_data=True,
-  version = '1.3',
-  description = 'This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.',
+  version = '1.4',
   author = ['Seedot'],
   author_email = 'seedotvsvader@gmail.com',
+  description = 'SEEDOT: Tool for Enhancing Sentiment Lexicon with Machine Learning',
+  long_description = read("README.rst"),
+  long_description_content_type = "text/markdown",
   license = 'MIT License: http://opensource.org/licenses/MIT',
   #url = 'https://github.com/Lucaa00/Vader_new', # use the URL to the github repo
   install_requires = ['requests'],
   keywords = ['seedot','vader', 'sentiment', 'analysis', 'opinion', 'mining', 'nlp', 'text', 'data',
               'text analysis', 'opinion analysis', 'sentiment analysis', 'text mining', 'twitter sentiment',
               'opinion mining', 'social media', 'twitter', 'social', 'media'], # arbitrary keywords
   classifiers = ['Development Status :: 4 - Beta', 'Intended Audience :: Science/Research',
```

