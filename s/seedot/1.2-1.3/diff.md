# Comparing `tmp/seedot-1.2.tar.gz` & `tmp/seedot-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedot-1.2.tar", last modified: Sat Jun 10 13:58:41 2023, max compression
+gzip compressed data, was "seedot-1.3.tar", last modified: Sat Jun 10 14:04:27 2023, max compression
```

## Comparing `seedot-1.2.tar` & `seedot-1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 13:58:41.794471 seedot-1.2/
--rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-1.2/LICENSE.txt
--rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-1.2/MANIFEST.in
--rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 13:58:41.794663 seedot-1.2/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)     6043 2023-06-09 16:55:58.000000 seedot-1.2/README.rst
--rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-1.2/__init__.py
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 13:58:41.791470 seedot-1.2/seedot/
--rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-1.2/seedot/SEEDOT_lexicon_electronic.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-1.2/seedot/SEEDOT_lexicon_finance.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-1.2/seedot/SEEDOT_lexicon_food.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-1.2/seedot/SEEDOT_lexicon_hotel.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-1.2/seedot/__init__.py
--rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-1.2/seedot/emoji_utf8_lexicon.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_electronic.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_finance.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_food.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34314 2023-06-09 17:22:08.000000 seedot-1.2/seedot/seedot_hotel.py
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 13:58:41.794090 seedot-1.2/seedot.egg-info/
--rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)      495 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/SOURCES.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/dependency_links.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/requires.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-10 13:58:41.000000 seedot-1.2/seedot.egg-info/top_level.txt
--rw-rw-r--   0 Vittom     (505) staff       (20)     1563 2023-06-10 13:58:41.795494 seedot-1.2/setup.cfg
--rw-rw-rw-   0 Vittom     (505) staff       (20)     1875 2023-06-10 13:58:12.000000 seedot-1.2/setup.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:04:27.787830 seedot-1.3/
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-1.3/LICENSE.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-1.3/MANIFEST.in
+-rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 14:04:27.788040 seedot-1.3/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)     6043 2023-06-09 16:55:58.000000 seedot-1.3/README.rst
+-rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-1.3/__init__.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:04:27.783795 seedot-1.3/seedot/
+-rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-1.3/seedot/SEEDOT_lexicon_electronic.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-1.3/seedot/SEEDOT_lexicon_finance.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-1.3/seedot/SEEDOT_lexicon_food.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-1.3/seedot/SEEDOT_lexicon_hotel.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-1.3/seedot/__init__.py
+-rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-1.3/seedot/emoji_utf8_lexicon.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-10 14:02:50.000000 seedot-1.3/seedot/seedot_electronic.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-10 14:02:13.000000 seedot-1.3/seedot/seedot_finance.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-10 14:02:32.000000 seedot-1.3/seedot/seedot_food.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    34313 2023-06-10 14:03:23.000000 seedot-1.3/seedot/seedot_hotel.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 14:04:27.787377 seedot-1.3/seedot.egg-info/
+-rw-r--r--   0 Vittom     (505) staff       (20)     1299 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)      495 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/SOURCES.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/dependency_links.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/requires.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-10 14:04:27.000000 seedot-1.3/seedot.egg-info/top_level.txt
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1563 2023-06-10 14:04:27.788660 seedot-1.3/setup.cfg
+-rw-rw-rw-   0 Vittom     (505) staff       (20)     1875 2023-06-10 14:04:14.000000 seedot-1.3/setup.py
```

### Comparing `seedot-1.2/LICENSE.txt` & `seedot-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.2/PKG-INFO` & `seedot-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedot
-Version: 1.2
+Version: 1.3
 Summary: This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
 Home-page: https://github.com/SEEDOT1/SEEDOT
 Author: ['Seedot']
 Author-email: seedotvsvader@gmail.com
 License: MIT License: http://opensource.org/licenses/MIT
 Keywords: seedot,vader,sentiment,analysis,opinion,mining,nlp,text,data,text analysis,opinion analysis,sentiment analysis,text mining,twitter sentiment,opinion mining,social media,twitter,social,media
 Platform: any
```

### Comparing `seedot-1.2/README.rst` & `seedot-1.3/README.rst`

 * *Files identical despite different names*

### Comparing `seedot-1.2/seedot/SEEDOT_lexicon_electronic.txt` & `seedot-1.3/seedot/SEEDOT_lexicon_electronic.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.2/seedot/SEEDOT_lexicon_finance.txt` & `seedot-1.3/seedot/SEEDOT_lexicon_finance.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.2/seedot/SEEDOT_lexicon_food.txt` & `seedot-1.3/seedot/SEEDOT_lexicon_food.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.2/seedot/SEEDOT_lexicon_hotel.txt` & `seedot-1.3/seedot/SEEDOT_lexicon_hotel.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.2/seedot/emoji_utf8_lexicon.txt` & `seedot-1.3/seedot/emoji_utf8_lexicon.txt`

 * *Files identical despite different names*

### Comparing `seedot-1.2/seedot/seedot_electronic.py` & `seedot-1.3/seedot/seedot_electronic.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 text_no_emoji += description
                 prev_space = False
             else:
                 text_no_emoji += chr
                 prev_space = chr == ' '
         text = text_no_emoji.strip()
 
-        sentitext = Electronic_ST(text)
+        sentitext = electronic_ST(text)
 
         sentiments = []
         words_and_emoticons = sentitext.words_and_emoticons
         for i, item in enumerate(words_and_emoticons):
             valence = 0
             # check for SEEDOT_lexicon words that may be used as modifiers or negations
             if item.lower() in BOOSTER_DICT:
```

### Comparing `seedot-1.2/seedot/seedot_finance.py` & `seedot-1.3/seedot/seedot_finance.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 text_no_emoji += description
                 prev_space = False
             else:
                 text_no_emoji += chr
                 prev_space = chr == ' '
         text = text_no_emoji.strip()
 
-        sentitext = Finance_ST(text)
+        sentitext = finance_ST(text)
 
         sentiments = []
         words_and_emoticons = sentitext.words_and_emoticons
         for i, item in enumerate(words_and_emoticons):
             valence = 0
             # check for SEEDOT_lexicon words that may be used as modifiers or negations
             if item.lower() in BOOSTER_DICT:
```

### Comparing `seedot-1.2/seedot/seedot_food.py` & `seedot-1.3/seedot/seedot_food.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 text_no_emoji += description
                 prev_space = False
             else:
                 text_no_emoji += chr
                 prev_space = chr == ' '
         text = text_no_emoji.strip()
 
-        sentitext = Food_ST(text)
+        sentitext = food_ST(text)
 
         sentiments = []
         words_and_emoticons = sentitext.words_and_emoticons
         for i, item in enumerate(words_and_emoticons):
             valence = 0
             # check for SEEDOT_lexicon words that may be used as modifiers or negations
             if item.lower() in BOOSTER_DICT:
```

### Comparing `seedot-1.2/seedot/seedot_hotel.py` & `seedot-1.3/seedot/seedot_hotel.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 text_no_emoji += description
                 prev_space = False
             else:
                 text_no_emoji += chr
                 prev_space = chr == ' '
         text = text_no_emoji.strip()
 
-        sentitext = Disney_ST(text)
+        sentitext = hotel_ST(text)
 
         sentiments = []
         words_and_emoticons = sentitext.words_and_emoticons
         for i, item in enumerate(words_and_emoticons):
             valence = 0
             # check for SEEDOT_lexicon words that may be used as modifiers or negations
             if item.lower() in BOOSTER_DICT:
```

### Comparing `seedot-1.2/seedot.egg-info/PKG-INFO` & `seedot-1.3/seedot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedot
-Version: 1.2
+Version: 1.3
 Summary: This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
 Home-page: https://github.com/SEEDOT1/SEEDOT
 Author: ['Seedot']
 Author-email: seedotvsvader@gmail.com
 License: MIT License: http://opensource.org/licenses/MIT
 Keywords: seedot,vader,sentiment,analysis,opinion,mining,nlp,text,data,text analysis,opinion analysis,sentiment analysis,text mining,twitter sentiment,opinion mining,social media,twitter,social,media
 Platform: any
```

### Comparing `seedot-1.2/setup.cfg` & `seedot-1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `seedot-1.2/setup.py` & `seedot-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         return f.read()
 
 setup(
   name = 'seedot',
   #packages = ['GROGU'], # this must be the same as the name above
   packages = find_packages(exclude=['tests*']), # a better way to do it than the line above -- this way no typo/transpo errors
   include_package_data=True,
-  version = '1.2',
+  version = '1.3',
   description = 'This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.',
   author = ['Seedot'],
   author_email = 'seedotvsvader@gmail.com',
   license = 'MIT License: http://opensource.org/licenses/MIT',
   #url = 'https://github.com/Lucaa00/Vader_new', # use the URL to the github repo
   install_requires = ['requests'],
   keywords = ['seedot','vader', 'sentiment', 'analysis', 'opinion', 'mining', 'nlp', 'text', 'data',
```

