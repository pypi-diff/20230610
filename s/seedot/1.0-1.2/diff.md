# Comparing `tmp/SEEDOT-1.0.tar.gz` & `tmp/seedot-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SEEDOT-1.0.tar", last modified: Fri Jun  9 17:03:37 2023, max compression
+gzip compressed data, was "seedot-1.2.tar", last modified: Sat Jun 10 13:58:41 2023, max compression
```

## Comparing `SEEDOT-1.0.tar` & `seedot-1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-09 17:03:37.433329 SEEDOT-1.0/
--rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 SEEDOT-1.0/LICENSE.txt
--rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 16:55:58.000000 SEEDOT-1.0/MANIFEST.in
--rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-09 17:03:37.433492 SEEDOT-1.0/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)     6043 2023-06-09 16:55:58.000000 SEEDOT-1.0/README.rst
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-09 17:03:37.430202 SEEDOT-1.0/SEEDOT/
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-09 16:55:58.000000 SEEDOT-1.0/SEEDOT/SEEDOT_electronic.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-09 16:56:38.000000 SEEDOT-1.0/SEEDOT/SEEDOT_finance.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-09 16:56:50.000000 SEEDOT-1.0/SEEDOT/SEEDOT_food.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34316 2023-06-09 16:57:01.000000 SEEDOT-1.0/SEEDOT/SEEDOT_hotel.py
--rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_electronic.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_finance.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_food.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_hotel.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 SEEDOT-1.0/SEEDOT/__init__.py
--rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 SEEDOT-1.0/SEEDOT/emoji_utf8_lexicon.txt
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-09 17:03:37.432506 SEEDOT-1.0/SEEDOT.egg-info/
--rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-09 17:03:37.000000 SEEDOT-1.0/SEEDOT.egg-info/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)      495 2023-06-09 17:03:37.000000 SEEDOT-1.0/SEEDOT.egg-info/SOURCES.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-09 17:03:37.000000 SEEDOT-1.0/SEEDOT.egg-info/dependency_links.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-09 17:03:37.000000 SEEDOT-1.0/SEEDOT.egg-info/requires.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-09 17:03:37.000000 SEEDOT-1.0/SEEDOT.egg-info/top_level.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 SEEDOT-1.0/__init__.py
--rw-rw-r--   0 Vittom     (505) staff       (20)     1563 2023-06-09 17:03:37.434614 SEEDOT-1.0/setup.cfg
--rw-rw-rw-   0 Vittom     (505) staff       (20)     1875 2023-06-09 17:02:45.000000 SEEDOT-1.0/setup.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 13:58:41.794471 seedot-1.2/
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-1.2/LICENSE.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-1.2/MANIFEST.in
+-rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 13:58:41.794663 seedot-1.2/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)     6043 2023-06-09 16:55:58.000000 seedot-1.2/README.rst
+-rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-1.2/__init__.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 13:58:41.791470 seedot-1.2/seedot/
+-rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-1.2/seedot/SEEDOT_lexicon_electronic.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-1.2/seedot/SEEDOT_lexicon_finance.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-1.2/seedot/SEEDOT_lexicon_food.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-1.2/seedot/SEEDOT_lexicon_hotel.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-1.2/seedot/__init__.py
+-rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-1.2/seedot/emoji_utf8_lexicon.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_electronic.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_finance.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_food.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34314 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_hotel.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 13:58:41.794090 seedot-1.2/seedot.egg-info/
+-rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)      495 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/SOURCES.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/dependency_links.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/requires.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/top_level.txt
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1563 2023-06-10 13:58:41.795494 seedot-1.2/setup.cfg
+-rw-rw-rw-   0 Vittom     (505) staff       (20)     1875 2023-06-10 13:58:12.000000 seedot-1.2/setup.py
```

### Comparing `SEEDOT-1.0/LICENSE.txt` & `seedot-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/PKG-INFO` & `seedot-1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SEEDOT
-Version: 1.0
+Name: seedot
+Version: 1.2
 Summary: This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
 Home-page: https://github.com/SEEDOT1/SEEDOT
 Author: ['Seedot']
 Author-email: seedotvsvader@gmail.com
 License: MIT License: http://opensource.org/licenses/MIT
 Keywords: seedot,vader,sentiment,analysis,opinion,mining,nlp,text,data,text analysis,opinion analysis,sentiment analysis,text mining,twitter sentiment,opinion mining,social media,twitter,social,media
 Platform: any
```

### Comparing `SEEDOT-1.0/README.rst` & `seedot-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_electronic.py` & `seedot-1.2/seedot/seedot_electronic.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             if valence > 0:
                 scalar += C_INCR
             else:
                 scalar -= C_INCR
     return scalar
 
 
-class Electronic_ST(object):
+class electronic_ST(object):
     """
     Identify sentiment-relevant string-level properties of input text.
     """
 
     def __init__(self, text):
         if not isinstance(text, str):
             text = str(text).encode('utf-8')
@@ -175,15 +175,15 @@
         Leaves contractions and most emoticons
             Does not preserve punc-plus-letter emoticons (e.g. :D)
         """
         wes = self.text.split()
         stripped = list(map(self._strip_punc_if_word, wes))
         return stripped
 
-class Electronic_SIA(object):
+class electronic_SIA(object):
     """
     Give a sentiment intensity score to sentences.
     """
 
     def __init__(self, lexicon_file="SEEDOT_lexicon_electronic.txt", emoji_lexicon="emoji_utf8_lexicon.txt"):
         _this_module_file_path_ = os.path.abspath(getsourcefile(lambda: 0))
         lexicon_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), lexicon_file)
```

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_finance.py` & `seedot-1.2/seedot/seedot_finance.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             if valence > 0:
                 scalar += C_INCR
             else:
                 scalar -= C_INCR
     return scalar
 
 
-class Finance_ST(object):
+class finance_ST(object):
     """
     Identify sentiment-relevant string-level properties of input text.
     """
 
     def __init__(self, text):
         if not isinstance(text, str):
             text = str(text).encode('utf-8')
@@ -175,15 +175,15 @@
         Leaves contractions and most emoticons
             Does not preserve punc-plus-letter emoticons (e.g. :D)
         """
         wes = self.text.split()
         stripped = list(map(self._strip_punc_if_word, wes))
         return stripped
 
-class Finance_SIA(object):
+class finance_SIA(object):
     """
     Give a sentiment intensity score to sentences.
     """
 
     def __init__(self, lexicon_file="SEEDOT_lexicon_finance.txt", emoji_lexicon="emoji_utf8_lexicon.txt"):
         _this_module_file_path_ = os.path.abspath(getsourcefile(lambda: 0))
         lexicon_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), lexicon_file)
```

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_food.py` & `seedot-1.2/seedot/seedot_food.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             if valence > 0:
                 scalar += C_INCR
             else:
                 scalar -= C_INCR
     return scalar
 
 
-class Food_ST(object):
+class food_ST(object):
     """
     Identify sentiment-relevant string-level properties of input text.
     """
 
     def __init__(self, text):
         if not isinstance(text, str):
             text = str(text).encode('utf-8')
@@ -175,15 +175,15 @@
         Leaves contractions and most emoticons
             Does not preserve punc-plus-letter emoticons (e.g. :D)
         """
         wes = self.text.split()
         stripped = list(map(self._strip_punc_if_word, wes))
         return stripped
 
-class Food_SIA(object):
+class food_SIA(object):
     """
     Give a sentiment intensity score to sentences. 
     """
 
     def __init__(self, lexicon_file="SEEDOT_lexicon_food.txt", emoji_lexicon="emoji_utf8_lexicon.txt"):
         _this_module_file_path_ = os.path.abspath(getsourcefile(lambda: 0))
         lexicon_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), lexicon_file)
```

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_hotel.py` & `seedot-1.2/seedot/seedot_hotel.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             if valence > 0:
                 scalar += C_INCR
             else:
                 scalar -= C_INCR
     return scalar
 
 
-class Disney_ST(object):
+class hotel_ST(object):
     """
     Identify sentiment-relevant string-level properties of input text.
     """
 
     def __init__(self, text):
         if not isinstance(text, str):
             text = str(text).encode('utf-8')
@@ -175,15 +175,15 @@
         Leaves contractions and most emoticons
             Does not preserve punc-plus-letter emoticons (e.g. :D)
         """
         wes = self.text.split()
         stripped = list(map(self._strip_punc_if_word, wes))
         return stripped
 
-class Disney_SIA(object):
+class hotel_SIA(object):
     """
     Give a sentiment intensity score to sentences.
     """
 
     def __init__(self, lexicon_file="SEEDOT_lexicon_hotel.txt", emoji_lexicon="emoji_utf8_lexicon.txt"):
         _this_module_file_path_ = os.path.abspath(getsourcefile(lambda: 0))
         lexicon_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), lexicon_file)
```

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_electronic.txt` & `seedot-1.2/seedot/SEEDOT_lexicon_electronic.txt`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_finance.txt` & `seedot-1.2/seedot/SEEDOT_lexicon_finance.txt`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_food.txt` & `seedot-1.2/seedot/SEEDOT_lexicon_food.txt`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/SEEDOT/SEEDOT_lexicon_hotel.txt` & `seedot-1.2/seedot/SEEDOT_lexicon_hotel.txt`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/SEEDOT/emoji_utf8_lexicon.txt` & `seedot-1.2/seedot/emoji_utf8_lexicon.txt`

 * *Files identical despite different names*

### Comparing `SEEDOT-1.0/SEEDOT.egg-info/PKG-INFO` & `seedot-1.2/seedot.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SEEDOT
-Version: 1.0
+Name: seedot
+Version: 1.2
 Summary: This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
 Home-page: https://github.com/SEEDOT1/SEEDOT
 Author: ['Seedot']
 Author-email: seedotvsvader@gmail.com
 License: MIT License: http://opensource.org/licenses/MIT
 Keywords: seedot,vader,sentiment,analysis,opinion,mining,nlp,text,data,text analysis,opinion analysis,sentiment analysis,text mining,twitter sentiment,opinion mining,social media,twitter,social,media
 Platform: any
```

### Comparing `SEEDOT-1.0/setup.cfg` & `seedot-1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = SEEDOT
+name = seedot
 author = Seedot
 Author-email = seedotvsvader@gmail.com
 license = MIT
 license-file = LICENSE.txt
 url = https://github.com/SEEDOT1/SEEDOT
 description = This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
 long_description = This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
```

### Comparing `SEEDOT-1.0/setup.py` & `seedot-1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     Build an absolute path from *parts* and and return the contents of the
     resulting file.  Assume UTF-8 encoding.
     """
     with codecs.open(os.path.join(HERE, *parts), "rb", "utf-8") as f:
         return f.read()
 
 setup(
-  name = 'SEEDOT',
+  name = 'seedot',
   #packages = ['GROGU'], # this must be the same as the name above
   packages = find_packages(exclude=['tests*']), # a better way to do it than the line above -- this way no typo/transpo errors
   include_package_data=True,
-  version = '1.0',
+  version = '1.2',
   description = 'This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.',
   author = ['Seedot'],
   author_email = 'seedotvsvader@gmail.com',
   license = 'MIT License: http://opensource.org/licenses/MIT',
   #url = 'https://github.com/Lucaa00/Vader_new', # use the URL to the github repo
   install_requires = ['requests'],
   keywords = ['seedot','vader', 'sentiment', 'analysis', 'opinion', 'mining', 'nlp', 'text', 'data',
```

