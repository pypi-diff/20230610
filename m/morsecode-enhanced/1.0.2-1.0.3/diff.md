# Comparing `tmp/morsecode_enhanced-1.0.2.tar.gz` & `tmp/morsecode_enhanced-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morsecode_enhanced-1.0.2.tar", last modified: Sat Jun 10 11:05:41 2023, max compression
+gzip compressed data, was "morsecode_enhanced-1.0.3.tar", last modified: Sat Jun 10 11:25:34 2023, max compression
```

## Comparing `morsecode_enhanced-1.0.2.tar` & `morsecode_enhanced-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 11:05:41.114910 morsecode_enhanced-1.0.2/
--rw-rw-rw-   0        0        0     1055 2023-06-10 08:21:58.000000 morsecode_enhanced-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1977 2023-06-10 11:05:41.110948 morsecode_enhanced-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2023-06-10 10:37:47.000000 morsecode_enhanced-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 11:05:41.072060 morsecode_enhanced-1.0.2/morsecode_enhanced/
--rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.2/morsecode_enhanced/__init__.py
--rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.2/morsecode_enhanced/morsecode_enhanced.py
-drwxrwxrwx   0        0        0        0 2023-06-10 11:05:41.105932 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/
--rw-rw-rw-   0        0        0     1977 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-10 11:05:40.000000 morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 11:05:41.114910 morsecode_enhanced-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-06-10 11:05:32.000000 morsecode_enhanced-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:25:34.909945 morsecode_enhanced-1.0.3/
+-rw-rw-rw-   0        0        0     1055 2023-06-10 08:21:58.000000 morsecode_enhanced-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2502 2023-06-10 11:25:34.907945 morsecode_enhanced-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2023-06-10 11:24:21.000000 morsecode_enhanced-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 11:25:34.868346 morsecode_enhanced-1.0.3/morsecode_enhanced/
+-rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.3/morsecode_enhanced/__init__.py
+-rw-rw-rw-   0        0        0    15738 2023-06-10 10:51:24.000000 morsecode_enhanced-1.0.3/morsecode_enhanced/morsecode_enhanced.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:25:34.904991 morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/
+-rw-rw-rw-   0        0        0     2502 2023-06-10 11:25:34.000000 morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-10 11:25:34.000000 morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 11:25:34.000000 morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-10 11:25:34.000000 morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 11:25:34.000000 morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 11:25:34.909945 morsecode_enhanced-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-06-10 11:24:56.000000 morsecode_enhanced-1.0.3/setup.py
```

### Comparing `morsecode_enhanced-1.0.2/LICENSE.txt` & `morsecode_enhanced-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.2/PKG-INFO` & `morsecode_enhanced-1.0.3/morsecode_enhanced.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: morsecode_enhanced
-Version: 1.0.2
+Name: morsecode-enhanced
+Version: 1.0.3
 Summary: A package for encoding and decoding Morse code.
 Home-page: https://github.com/danysrour/morsecode_enhanced
 Author: Dany Srour
 Author-email: dany.srour@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -32,42 +32,72 @@
 # Usage
 
 ## Encoding
 
 To encode text into Morse code, you can use the encode function:
 
 ```python
-from morsecode_enhanced import encode
+from morsecode_enhanced import MorseCode
+
+mc = MorseCode()
+encoded_word = mc.encode_word('Hello, World!')
+print(encodex_word)
 
-encoded_message = encode('Hello, World!')
-print(encoded_message)
 
 ```
 
 Output:
 ```text
 .... . .-.. .-.. --- --..-- / .-- --- .-. .-.. -.. -.-.--
 ```
 
 ## Decoding
 
 To decode Morse code into text, you can use the decode function:
 
 ```python
-from morsecode_enhanced import decode
+from morsecode_enhanced import MorseCode
 
-decoded_message = decode('.... . .-.. .-.. --- --..-- / .-- --- .-. .-.. -.. -.-.--')
+mc = MorseCode()
+decoded_message = mc.decode('.... . .-.. .-.. --- --..-- / .-- --- .-. .-.. -.. -.-.--')
 print(decoded_message)
 
 ```
 
 Output:
 ```text
 HELLO, WORLD!
 ```
+
+# More Functionalities
+
+```python
+from morsecode_enhanced import MorseCode
+
+mc = MorseCode()
+encoded_word = mc.encode_word('Hello')
+print(encoded_word)
+
+decoded_word = mc.decode_word('.-..')
+print(decoded_word)
+
+random_morse = mc.generate_random_morse(10)
+
+is_valid_morse = mc.is_valid_morse_code(encoded_word)
+
+analyzed = mc.analyze_frequency('.-..')
+
+visualised = mc.visualize_morse_code('.-..')
+
+duration = mc.calculate_duration('.-..')
+
+
+
+```
+
 # Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on [GitHub](https://github.com/danysrour/MorseCode).
 
 # License
 
 This project is licensed under the [MIT License](https://github.com/danysrour/morsecodeplus.git)
```

### Comparing `morsecode_enhanced-1.0.2/morsecode_enhanced/__init__.py` & `morsecode_enhanced-1.0.3/morsecode_enhanced/__init__.py`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.2/morsecode_enhanced/morsecode_enhanced.py` & `morsecode_enhanced-1.0.3/morsecode_enhanced/morsecode_enhanced.py`

 * *Files identical despite different names*

### Comparing `morsecode_enhanced-1.0.2/morsecode_enhanced.egg-info/PKG-INFO` & `morsecode_enhanced-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: morsecode-enhanced
-Version: 1.0.2
+Name: morsecode_enhanced
+Version: 1.0.3
 Summary: A package for encoding and decoding Morse code.
 Home-page: https://github.com/danysrour/morsecode_enhanced
 Author: Dany Srour
 Author-email: dany.srour@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -32,42 +32,72 @@
 # Usage
 
 ## Encoding
 
 To encode text into Morse code, you can use the encode function:
 
 ```python
-from morsecode_enhanced import encode
+from morsecode_enhanced import MorseCode
+
+mc = MorseCode()
+encoded_word = mc.encode_word('Hello, World!')
+print(encodex_word)
 
-encoded_message = encode('Hello, World!')
-print(encoded_message)
 
 ```
 
 Output:
 ```text
 .... . .-.. .-.. --- --..-- / .-- --- .-. .-.. -.. -.-.--
 ```
 
 ## Decoding
 
 To decode Morse code into text, you can use the decode function:
 
 ```python
-from morsecode_enhanced import decode
+from morsecode_enhanced import MorseCode
 
-decoded_message = decode('.... . .-.. .-.. --- --..-- / .-- --- .-. .-.. -.. -.-.--')
+mc = MorseCode()
+decoded_message = mc.decode('.... . .-.. .-.. --- --..-- / .-- --- .-. .-.. -.. -.-.--')
 print(decoded_message)
 
 ```
 
 Output:
 ```text
 HELLO, WORLD!
 ```
+
+# More Functionalities
+
+```python
+from morsecode_enhanced import MorseCode
+
+mc = MorseCode()
+encoded_word = mc.encode_word('Hello')
+print(encoded_word)
+
+decoded_word = mc.decode_word('.-..')
+print(decoded_word)
+
+random_morse = mc.generate_random_morse(10)
+
+is_valid_morse = mc.is_valid_morse_code(encoded_word)
+
+analyzed = mc.analyze_frequency('.-..')
+
+visualised = mc.visualize_morse_code('.-..')
+
+duration = mc.calculate_duration('.-..')
+
+
+
+```
+
 # Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on [GitHub](https://github.com/danysrour/MorseCode).
 
 # License
 
 This project is licensed under the [MIT License](https://github.com/danysrour/morsecodeplus.git)
```

### Comparing `morsecode_enhanced-1.0.2/setup.py` & `morsecode_enhanced-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='morsecode_enhanced',
-    version='1.0.2',
+    version='1.0.3',
     author='Dany Srour',
     author_email='dany.srour@gmail.com',
     description='A package for encoding and decoding Morse code.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/danysrour/morsecode_enhanced',
     packages=['morsecode_enhanced'],
```

