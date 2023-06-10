# Comparing `tmp/pyaikit-1.0.3.tar.gz` & `tmp/pyaikit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyaikit-1.0.3.tar", last modified: Sat Jun 10 13:42:07 2023, max compression
+gzip compressed data, was "dist\pyaikit-1.0.4.tar", last modified: Sat Jun 10 13:46:49 2023, max compression
```

## Comparing `pyaikit-1.0.3.tar` & `pyaikit-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/
--rw-rw-rw-   0        0        0     5720 2023-06-10 13:42:07.000000 pyaikit-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4977 2023-06-10 12:49:12.000000 pyaikit-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:20:37.000000 pyaikit-1.0.3/pyaikit/__init__.py
--rw-rw-rw-   0        0        0      750 2023-06-04 08:19:53.000000 pyaikit-1.0.3/pyaikit/authentication.py
--rw-rw-rw-   0        0        0     1155 2023-06-10 11:55:09.000000 pyaikit-1.0.3/pyaikit/example.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/sentiment_analysis/
--rw-rw-rw-   0        0        0     6743 2023-06-05 17:19:55.000000 pyaikit-1.0.3/pyaikit/sentiment_analysis/sentiment_analyzer.py
--rw-rw-rw-   0        0        0     1177 2023-06-10 13:42:00.000000 pyaikit-1.0.3/pyaikit/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/text_generation/
--rw-rw-rw-   0        0        0     1574 2023-06-10 10:03:48.000000 pyaikit-1.0.3/pyaikit/text_generation/text_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/text_summerization/
--rw-rw-rw-   0        0        0     4761 2023-06-07 04:21:23.000000 pyaikit-1.0.3/pyaikit/text_summerization/text_summerizer.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit/translation/
--rw-rw-rw-   0        0        0     1546 2023-06-10 09:50:21.000000 pyaikit-1.0.3/pyaikit/translation/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/
--rw-rw-rw-   0        0        0     5720 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0      106 2023-06-10 13:42:07.000000 pyaikit-1.0.3/pyaikit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 13:42:07.000000 pyaikit-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-06-10 13:41:57.000000 pyaikit-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/
+-rw-rw-rw-   0        0        0     5412 2023-06-10 13:46:49.000000 pyaikit-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4669 2023-06-10 13:45:53.000000 pyaikit-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:20:37.000000 pyaikit-1.0.4/pyaikit/__init__.py
+-rw-rw-rw-   0        0        0      750 2023-06-04 08:19:53.000000 pyaikit-1.0.4/pyaikit/authentication.py
+-rw-rw-rw-   0        0        0     1155 2023-06-10 11:55:09.000000 pyaikit-1.0.4/pyaikit/example.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit/sentiment_analysis/
+-rw-rw-rw-   0        0        0     6743 2023-06-05 17:19:55.000000 pyaikit-1.0.4/pyaikit/sentiment_analysis/sentiment_analyzer.py
+-rw-rw-rw-   0        0        0     1177 2023-06-10 13:45:11.000000 pyaikit-1.0.4/pyaikit/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit/text_generation/
+-rw-rw-rw-   0        0        0     1574 2023-06-10 10:03:48.000000 pyaikit-1.0.4/pyaikit/text_generation/text_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit/text_summerization/
+-rw-rw-rw-   0        0        0     4761 2023-06-07 04:21:23.000000 pyaikit-1.0.4/pyaikit/text_summerization/text_summerizer.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit/translation/
+-rw-rw-rw-   0        0        0     1546 2023-06-10 09:50:21.000000 pyaikit-1.0.4/pyaikit/translation/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit.egg-info/
+-rw-rw-rw-   0        0        0     5412 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      106 2023-06-10 13:46:49.000000 pyaikit-1.0.4/pyaikit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:46:49.000000 pyaikit-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-06-10 13:46:45.000000 pyaikit-1.0.4/setup.py
```

### Comparing `pyaikit-1.0.3/PKG-INFO` & `pyaikit-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaikit
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyAIKit is a user-friendly Python package that simplifies the integration and usage of OpenAIs powerful ChatGPT API for natural language processing tasks
 Home-page: https://github.com/somenath24/pyaikit
 Author: Somenath Sit
 Author-email: somenath.bhu.2010@gmail.com
 Project-URL: GitHub, https://github.com/somenath24/pyaikit
 Project-URL: Changelog, https://github.com/Somenath24/pyaikit/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: MIT License
@@ -110,14 +110,10 @@
         This expansion would enable users to combine the power of ChatGPT with other state-of-the-art models, such as image recognition or speech processing models. This integration would enhance the package's versatility and enable the development of more comprehensive AI solutions.</p>
 <h2>License</h2>
 
 <p>PyAIKit is distributed under the <a href="https://github.com/somenath24/pyaikit/blob/main/LICENSE">MIT License</a>. See the <code>LICENSE</code> file for more information.
 </p>
 <p>
 This package is using OpenAI API, no connection with openai organization
+</p>
 <hr>
 
-<p>We hope that PyAIKit simplifies your integration with OpenAI's API and empowers you to leverage the potential of artificial intelligence in your Python projects. If you have any questions or need support, please don't hesitate to reach out to me at somenath.bhu.2010@gmail.com.</p>
-
-<p>Happy coding!</p>
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyaikit Version: 1.0.3 Summary: PyAIKit is a user-
+Metadata-Version: 2.1 Name: pyaikit Version: 1.0.4 Summary: PyAIKit is a user-
 friendly Python package that simplifies the integration and usage of OpenAIs
 powerful ChatGPT API for natural language processing tasks Home-page: https://
 github.com/somenath24/pyaikit Author: Somenath Sit Author-email:
 somenath.bhu.2010@gmail.com Project-URL: GitHub, https://github.com/somenath24/
 pyaikit Project-URL: Changelog, https://github.com/Somenath24/pyaikit/blob/
 main/CHANGELOG.md Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -78,12 +78,7 @@
 package's versatility and enable the development of more comprehensive AI
 solutions.
 ***** License *****
 PyAIKit is distributed under the MIT_License. See the LICENSE file for more
 information.
 This package is using OpenAI API, no connection with openai organization
 ===============================================================================
-We hope that PyAIKit simplifies your integration with OpenAI's API and empowers
-you to leverage the potential of artificial intelligence in your Python
-projects. If you have any questions or need support, please don't hesitate to
-reach out to me at somenath.bhu.2010@gmail.com.
-Happy coding!
```

### Comparing `pyaikit-1.0.3/README.md` & `pyaikit-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,10 @@
         This expansion would enable users to combine the power of ChatGPT with other state-of-the-art models, such as image recognition or speech processing models. This integration would enhance the package's versatility and enable the development of more comprehensive AI solutions.</p>
 <h2>License</h2>
 
 <p>PyAIKit is distributed under the <a href="https://github.com/somenath24/pyaikit/blob/main/LICENSE">MIT License</a>. See the <code>LICENSE</code> file for more information.
 </p>
 <p>
 This package is using OpenAI API, no connection with openai organization
+</p>
 <hr>
 
-<p>We hope that PyAIKit simplifies your integration with OpenAI's API and empowers you to leverage the potential of artificial intelligence in your Python projects. If you have any questions or need support, please don't hesitate to reach out to me at somenath.bhu.2010@gmail.com.</p>
-
-<p>Happy coding!</p>
-
-
```

#### html2text {}

```diff
@@ -68,12 +68,7 @@
 package's versatility and enable the development of more comprehensive AI
 solutions.
 ***** License *****
 PyAIKit is distributed under the MIT_License. See the LICENSE file for more
 information.
 This package is using OpenAI API, no connection with openai organization
 ===============================================================================
-We hope that PyAIKit simplifies your integration with OpenAI's API and empowers
-you to leverage the potential of artificial intelligence in your Python
-projects. If you have any questions or need support, please don't hesitate to
-reach out to me at somenath.bhu.2010@gmail.com.
-Happy coding!
```

### Comparing `pyaikit-1.0.3/pyaikit/authentication.py` & `pyaikit-1.0.4/pyaikit/authentication.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/pyaikit/example.py` & `pyaikit-1.0.4/pyaikit/example.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/pyaikit/sentiment_analysis/sentiment_analyzer.py` & `pyaikit-1.0.4/pyaikit/sentiment_analysis/sentiment_analyzer.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/pyaikit/setup.py` & `pyaikit-1.0.4/pyaikit/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pyaikit',
-    version='1.0.3',
+    version='1.0.4',
     author='Somenath Sit',
     author_email='somenath.bhu.2010@gmail.com',
     description='PyAIKit is a user-friendly Python package that simplifies the integration and usage of OpenAIs powerful ChatGPT API for natural language processing tasks',
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/somenath24/pyaikit',
     packages=['pyaikit','pyaikit/sentiment_analysis','pyaikit/text_summerization','pyaikit/translation','pyaikit/text_generation'],
```

### Comparing `pyaikit-1.0.3/pyaikit/text_generation/text_generator.py` & `pyaikit-1.0.4/pyaikit/text_generation/text_generator.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/pyaikit/text_summerization/text_summerizer.py` & `pyaikit-1.0.4/pyaikit/text_summerization/text_summerizer.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/pyaikit/translation/translator.py` & `pyaikit-1.0.4/pyaikit/translation/translator.py`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/pyaikit.egg-info/PKG-INFO` & `pyaikit-1.0.4/pyaikit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaikit
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyAIKit is a user-friendly Python package that simplifies the integration and usage of OpenAIs powerful ChatGPT API for natural language processing tasks
 Home-page: https://github.com/somenath24/pyaikit
 Author: Somenath Sit
 Author-email: somenath.bhu.2010@gmail.com
 Project-URL: GitHub, https://github.com/somenath24/pyaikit
 Project-URL: Changelog, https://github.com/Somenath24/pyaikit/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: MIT License
@@ -110,14 +110,10 @@
         This expansion would enable users to combine the power of ChatGPT with other state-of-the-art models, such as image recognition or speech processing models. This integration would enhance the package's versatility and enable the development of more comprehensive AI solutions.</p>
 <h2>License</h2>
 
 <p>PyAIKit is distributed under the <a href="https://github.com/somenath24/pyaikit/blob/main/LICENSE">MIT License</a>. See the <code>LICENSE</code> file for more information.
 </p>
 <p>
 This package is using OpenAI API, no connection with openai organization
+</p>
 <hr>
 
-<p>We hope that PyAIKit simplifies your integration with OpenAI's API and empowers you to leverage the potential of artificial intelligence in your Python projects. If you have any questions or need support, please don't hesitate to reach out to me at somenath.bhu.2010@gmail.com.</p>
-
-<p>Happy coding!</p>
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyaikit Version: 1.0.3 Summary: PyAIKit is a user-
+Metadata-Version: 2.1 Name: pyaikit Version: 1.0.4 Summary: PyAIKit is a user-
 friendly Python package that simplifies the integration and usage of OpenAIs
 powerful ChatGPT API for natural language processing tasks Home-page: https://
 github.com/somenath24/pyaikit Author: Somenath Sit Author-email:
 somenath.bhu.2010@gmail.com Project-URL: GitHub, https://github.com/somenath24/
 pyaikit Project-URL: Changelog, https://github.com/Somenath24/pyaikit/blob/
 main/CHANGELOG.md Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -78,12 +78,7 @@
 package's versatility and enable the development of more comprehensive AI
 solutions.
 ***** License *****
 PyAIKit is distributed under the MIT_License. See the LICENSE file for more
 information.
 This package is using OpenAI API, no connection with openai organization
 ===============================================================================
-We hope that PyAIKit simplifies your integration with OpenAI's API and empowers
-you to leverage the potential of artificial intelligence in your Python
-projects. If you have any questions or need support, please don't hesitate to
-reach out to me at somenath.bhu.2010@gmail.com.
-Happy coding!
```

### Comparing `pyaikit-1.0.3/pyaikit.egg-info/SOURCES.txt` & `pyaikit-1.0.4/pyaikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaikit-1.0.3/setup.py` & `pyaikit-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pyaikit',
-    version='1.0.3',
+    version='1.0.4',
     author='Somenath Sit',
     author_email='somenath.bhu.2010@gmail.com',
     description='PyAIKit is a user-friendly Python package that simplifies the integration and usage of OpenAIs powerful ChatGPT API for natural language processing tasks',
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/somenath24/pyaikit',
     packages=['pyaikit','pyaikit/sentiment_analysis','pyaikit/text_summerization','pyaikit/translation','pyaikit/text_generation'],
```

