# Comparing `tmp/aichat-cli-0.4.4.tar.gz` & `tmp/aichat-cli-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aichat-cli-0.4.4.tar", last modified: Mon Jun  5 19:43:20 2023, max compression
+gzip compressed data, was "aichat-cli-0.4.5.tar", last modified: Sat Jun 10 20:01:59 2023, max compression
```

## Comparing `aichat-cli-0.4.4.tar` & `aichat-cli-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 19:43:20.358472 aichat-cli-0.4.4/
--rw-rw-rw-   0        0        0    35823 2023-05-15 15:29:09.000000 aichat-cli-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     4353 2023-06-05 19:43:20.357471 aichat-cli-0.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 19:43:20.356472 aichat-cli-0.4.4/aichat_cli.egg-info/
--rw-rw-rw-   0        0        0     4353 2023-06-05 19:43:20.000000 aichat-cli-0.4.4/aichat_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-05 19:43:20.000000 aichat-cli-0.4.4/aichat_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 19:43:20.000000 aichat-cli-0.4.4/aichat_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-06-05 19:43:20.000000 aichat-cli-0.4.4/aichat_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 19:43:20.000000 aichat-cli-0.4.4/aichat_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 19:43:20.358472 aichat-cli-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-06-05 19:42:59.000000 aichat-cli-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:01:59.004407 aichat-cli-0.4.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     4378 2023-06-10 20:01:59.004407 aichat-cli-0.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 20:01:59.002282 aichat-cli-0.4.5/aichat_cli.egg-info/
+-rw-rw-rw-   0        0        0     4378 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 20:01:59.005405 aichat-cli-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-06-10 19:48:02.000000 aichat-cli-0.4.5/setup.py
```

### Comparing `aichat-cli-0.4.4/LICENSE` & `aichat-cli-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aichat-cli-0.4.4/PKG-INFO` & `aichat-cli-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.4
+Version: 0.4.5
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ai Chat CLI v3.0
+# Ai Chat CLI
 
 [![Did i find a bad token today ?](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml/badge.svg)](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml)
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
@@ -62,30 +62,30 @@
 
 Chromium: Devtools > Application > Cookies > poe.com
 
 Firefox: Devtools > Storage > Cookies
 
 Safari: Devtools > Storage > Cookies
 
-then save the token by creating `poe_token.txt` in `/tokens`
+then save the token by creating `poe_token.txt` in `/aichat/tokens`
 
 ---
 
 ### Bard token
 
 Log into [Bard](https://bard.google.com/) on any web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `__Secure-1PSID` cookie in the following menus:
 (tip : copy the cookie name to the filter box)
 
 Chromium: Devtools > Application > Cookies > bard.google.com
 
 Firefox: Devtools > Storage > Cookies
 
 Safari: Devtools > Storage > Cookies
 
-then save the token by creating `bard_token.txt` in `/tokens`
+then save the token by creating `bard_token.txt` in `/aichat/tokens`
 > :warning: **Warning:** Be careful using Bard tokens; they are Google account tokens.
 
 ---
 
 ### Bing token
 
 Not required.
@@ -108,15 +108,15 @@
 
 If you don't provide any command-line arguments, the app will prompt you to choose a bot and enter a message interactively.
 
 Once the conversation starts, you can continue the interaction by typing your messages or selecting options from the menu. The menu options include changing the bot or exporting the conversation to a .txt file.
 
 ## Notes📌
 
-- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` script provided.
+- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` in `/token_gen` script provided.
 
 - The CLI app also supports the use of premium tokens , so you can be able to use GPT4.
 
 - The conversation history is stored within the app and is not persistent between sessions.
 
 Feel free to customize and enhance the GPT CLI app according to your needs. Happy **chatting**!
```

### Comparing `aichat-cli-0.4.4/aichat_cli.egg-info/PKG-INFO` & `aichat-cli-0.4.5/aichat_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.4
+Version: 0.4.5
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ai Chat CLI v3.0
+# Ai Chat CLI
 
 [![Did i find a bad token today ?](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml/badge.svg)](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml)
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
@@ -62,30 +62,30 @@
 
 Chromium: Devtools > Application > Cookies > poe.com
 
 Firefox: Devtools > Storage > Cookies
 
 Safari: Devtools > Storage > Cookies
 
-then save the token by creating `poe_token.txt` in `/tokens`
+then save the token by creating `poe_token.txt` in `/aichat/tokens`
 
 ---
 
 ### Bard token
 
 Log into [Bard](https://bard.google.com/) on any web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `__Secure-1PSID` cookie in the following menus:
 (tip : copy the cookie name to the filter box)
 
 Chromium: Devtools > Application > Cookies > bard.google.com
 
 Firefox: Devtools > Storage > Cookies
 
 Safari: Devtools > Storage > Cookies
 
-then save the token by creating `bard_token.txt` in `/tokens`
+then save the token by creating `bard_token.txt` in `/aichat/tokens`
 > :warning: **Warning:** Be careful using Bard tokens; they are Google account tokens.
 
 ---
 
 ### Bing token
 
 Not required.
@@ -108,15 +108,15 @@
 
 If you don't provide any command-line arguments, the app will prompt you to choose a bot and enter a message interactively.
 
 Once the conversation starts, you can continue the interaction by typing your messages or selecting options from the menu. The menu options include changing the bot or exporting the conversation to a .txt file.
 
 ## Notes📌
 
-- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` script provided.
+- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` in `/token_gen` script provided.
 
 - The CLI app also supports the use of premium tokens , so you can be able to use GPT4.
 
 - The conversation history is stored within the app and is not persistent between sessions.
 
 Feel free to customize and enhance the GPT CLI app according to your needs. Happy **chatting**!
```

### Comparing `aichat-cli-0.4.4/setup.py` & `aichat-cli-0.4.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import setuptools
 from pathlib import Path
 
-# note: build this package with the following command:
-# pip wheel --no-deps -w dist .
-
+# note: build this package with the following commands: #TODO: automate this
+'''
+python setup.py sdist bdist_wheel
+twine check dist/*
+twine upload dist/*
+'''
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 setuptools.setup(
     name="aichat-cli",
-    version="0.4.4",
+    version="0.4.5",
     author="TheLime1",
     license="GPLv3",
     description="A CLI app that allows you to have interactive conversations with different AI bots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent"
     ],
     python_requires=">=3.7",
     packages=setuptools.find_packages(),
-    install_requires=[
-        'argparse',
-        'poe-api==0.4.4',
-        'selenium',
-        'pyperclip==1.8.2',
-        'prompt_toolkit',
-        'bardapi==0.1.11',
-        'EdgeGPT==0.8.0'
-    ],
+    install_requires=requirements,
     url="https://github.com/TheLime1/aichat-cli"
 )
```

