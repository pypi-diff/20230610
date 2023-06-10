# Comparing `tmp/comai-0.0.9.tar.gz` & `tmp/comai-0.1.0.tar.gz`

## Comparing `comai-0.0.9.tar` & `comai-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.0.9/.github/workflows/release.yml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 comai-0.0.9/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/__main__.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/cli.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 comai-0.0.9/src/comai/config.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 comai-0.0.9/tests/test_comai.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 comai-0.0.9/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.0.9/LICENSE
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 comai-0.0.9/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 comai-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    44480 2020-02-02 00:00:00.000000 comai-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0  4135795 2020-02-02 00:00:00.000000 comai-0.1.0/demo.gif
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 comai-0.1.0/logo.svg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 comai-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/__main__.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/animations.py
+-rwxr-xr-x   0        0        0     2073 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/cli.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/config.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/context.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/history.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/menu.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/translation.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 comai-0.1.0/tests/test_comai.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 comai-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 comai-0.1.0/README.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 comai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    46765 2020-02-02 00:00:00.000000 comai-0.1.0/PKG-INFO
```

### Comparing `comai-0.0.9/.github/workflows/release.yml` & `comai-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `comai-0.0.9/src/comai/config.py` & `comai-0.1.0/src/comai/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,55 @@
-import configparser
 import os
-import appdirs
+import configparser
+import typer
+import tempfile
+from typing import List
 from cryptography.fernet import Fernet
 
-app_name = "comai"
-app_author = "ricopinazo"
-config_dir = appdirs.user_config_dir(app_name, app_author)
-config_path = os.path.join(config_dir, "config.ini")
+CONTEXT_SIZE = 20
+APP_NAME = "comai"
+config_dir = typer.get_app_dir(APP_NAME, force_posix=True)
+key_path = os.path.join(config_dir, "config.ini")
+temp_dir = tempfile.gettempdir()
+session_id = os.getenv("TERM_SESSION_ID")
+log_path = None
+try:
+    log_path = os.path.join(temp_dir, session_id)
+except Exception:
+    pass
 
-encryption_key = b'QUMSqTJ5nape3p8joqkgHFCzyJdyQtqzHk6dCuGl9Nw='
+encryption_key = b"QUMSqTJ5nape3p8joqkgHFCzyJdyQtqzHk6dCuGl9Nw="
 cipher_suite = Fernet(encryption_key)
 
+
 def save_api_key(api_key):
     encrypted_key = cipher_suite.encrypt(api_key.encode())
     config = configparser.ConfigParser()
     config["DEFAULT"] = {"api_key": encrypted_key.decode()}
 
-    os.makedirs(config_dir, mode=0o700,  exist_ok=True)
+    os.makedirs(config_dir, mode=0o700, exist_ok=True)
+
     def opener(path, flags):
         return os.open(path, flags, 0o600)
-    with open(config_path, "w", opener=opener) as configfile:
+
+    with open(key_path, "w", opener=opener) as configfile:
         config.write(configfile)
 
+
 def load_api_key():
     try:
         config = configparser.ConfigParser()
-        config.read(config_path)
+        config.read(key_path)
         encrypted_key = config["DEFAULT"]["api_key"].encode()
         decrypted_key = cipher_suite.decrypt(encrypted_key)
         return decrypted_key.decode()
     except Exception:
         return None
 
+
 def delete_api_key():
-    if os.path.isfile(config_path):
-        os.remove(config_path)
-    if os.path.isdir(config_dir):
-        os.rmdir(config_dir)
+    if os.path.isfile(key_path):
+        os.remove(key_path)
+
+
+def get_history_path() -> os.PathLike:
+    return log_path
```

### Comparing `comai-0.0.9/LICENSE` & `comai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comai-0.0.9/pyproject.toml` & `comai-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,27 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Operating System :: MacOS",
     "Operating System :: Unix",
 ]
 dependencies = [
+  "typer==0.9.0",
   "openai==0.27.5",
-  "appdirs==1.4.4",
   "cryptography==40.0.2",
   "termcolor==2.3.0",
-  "getch==1.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/ricopinazo/comai"
 repository = "https://github.com/ricopinazo/comai"
 issues = "https://github.com/ricopinazo/comai/issues"
 
 [project.scripts]
-comai = "comai.cli:main"
+comai = "comai.cli:app"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "hatchling",
     "python-dotenv"
 ]
```

### Comparing `comai-0.0.9/PKG-INFO` & `comai-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comai
-Version: 0.0.9
+Version: 0.1.0
 Summary: AI powered console assistant
 Project-URL: homepage, https://github.com/ricopinazo/comai
 Project-URL: repository, https://github.com/ricopinazo/comai
 Project-URL: issues, https://github.com/ricopinazo/comai/issues
 Author-email: Pedro Rico <ricopinazo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -683,89 +683,143 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: appdirs==1.4.4
 Requires-Dist: cryptography==40.0.2
-Requires-Dist: getch==1.0
 Requires-Dist: openai==0.27.5
 Requires-Dist: termcolor==2.3.0
+Requires-Dist: typer==0.9.0
 Provides-Extra: test
 Requires-Dist: hatchling; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: python-dotenv; extra == 'test'
 Description-Content-Type: text/markdown
 
-# Comai - The AI powered terminal assistant
+<div align="center">
+  <img src="https://raw.githubusercontent.com/ricopinazo/comai/main/logo.svg" alt="demo" width="200"/>
+  
+  **The AI powered terminal assistant**
+  
+  [![Tests](https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg)](https://github.com/ricopinazo/comai/actions/workflows/tests.yml)
+  [![Latest release](https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases)](https://github.com/ricopinazo/comai/releases)
+  [![PyPI](https://img.shields.io/pypi/v/comai)](https://pypi.org/project/comai/)
+  [![Issues](https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen)](https://github.com/ricopinazo/comai/issues)
+  [![License GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
+  [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+</div>
 
-<p align="left">
-<a href="https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg">
-<img alt="Test and Build" src="https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg" />
-</a>
-<a href="https://github.com/ricopinazo/comai/releases">
-<img alt="Latest Release" src="https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases" />
-</a>
-<a href="https://pypi.org/project/comai/">
-<img alt="PyPI" src="https://img.shields.io/pypi/v/comai">
-</a>
-<a href="https://github.com/ricopinazo/comai/issues">
-<img alt="Issues" src="https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen" />
-</a>
-</p>
+## What is comai? 🎯
 
 `comai` is an open source terminal assistant powered by OpenAI API that enables you to interact with your command line interface using natural language instructions. It simplifies your workflow by converting natural language queries into executable commands. No more memorizing complex syntax. Just chat with `comai` using plain English!
 
+<div align="left">
+<img src="https://raw.githubusercontent.com/ricopinazo/comai/main/demo.gif" alt="demo" width="350"/>
+</div>
+
 ## Installation 🚀
 
-Getting `comai` up and running is a breeze. Simply use `pip` to install the latest tested version:
+Getting `comai` up and running is a breeze. You can simply use [`pip`](https://pip.pypa.io/en/stable/) to install the latest version:
 
 ```shell
 pip install comai
 ```
 
+However, if you usually work with python environments, it is recommended to use [`pipx`](https://pypa.github.io/pipx/) instead:
+
+```shell
+pipx install comai
+```
+
 The first time you run it, it'll ask you for an OpenAI API key. You can create a developer account [here](https://platform.openai.com/overview). Once in your account, go to `API Keys` section and `Create new secret key`. We recommend setting a usage limit under `Billing`/`Usage limits`.
 
+> **_NOTE:_** `comai` uses the environment variable `TERM_SESSION_ID` to maintain context between calls so you don't need to repeat yourself giving instructions to it. You can check if it is available in your default terminal checking the output of `echo $TERM_SESSION_ID`, which should return some type of UUID. If the output is empty, you can simply add the following to your `.zshrc`/`.bashrc` file:
+> ```shell
+> export TERM_SESSION_ID=$(uuidgen)
+> ```
+
 ## Usage Examples 🎉
 
 Using `comai` is straightforward. Simply invoke the `comai` command followed by your natural language instruction. `comai` will provide you with the corresponding executable command, which you can execute by pressing Enter or ignore by pressing any other key.
 
 Let's dive into some exciting examples of how you can harness the power of `comai`:
 
-1. Unleash your creativity with an ASCII art cow:
+1. Manage your system like a pro:
 ```shell
-$ comai print a cow saying Moo!
-💡≫ echo "Moo!" | cowsay
+$ comai print my private ip address
+❯ ifconfig | grep "inet " | grep -v 127.0.0.1 | awk '{print $2}'
+192.168.0.2
+
+$ comai and my public one
+❯ curl ifconfig.me
+92.234.58.146
 ```
 
-2. Update the main branch and merge it into the current branch:
+2. Master the intricacies of `git`:
 ```shell
-$ comai update the main branch and merge it into the current
-💡≫ git checkout main; git pull; git checkout -; git merge main
-```
+$ comai squash the last 3 commits into a single commit
+❯ git rebase -i HEAD~3
 
+$ comai show me all the branches having commit c4c0d2d in common
+❯ git branch --contains c4c0d2d
+  chat-api
+  configparser
+* main
+```
 
 3. Check the weather forecast for your location:
 ```shell
 $ comai show me the weather forecast
-💡≫ curl wttr.in
+❯ curl wttr.in
 ```
 
-3. Find the annoying process using the port 8000:
+4. Find the annoying process using the port 8080:
 ```shell
-$ comai show me the process using port 8000
-💡≫ lsof -i :8000
+$ comai show me the process using the port 8080
+❯ lsof -i :8080
+COMMAND   PID      USER   FD   TYPE            DEVICE SIZE/OFF NODE NAME
+node    36350 pedrorico   18u  IPv4 0xe0d28ea918e376b      0t0  TCP *:http-alt (LISTEN)
+
+$ comai show me only the PID
+❯ lsof -t -i :8080
+36350
+
+$ comai kill it
+❯ kill $(lsof -t -i :8080)
 ```
 
-4. Discover your future with a fortune cookie quote:
+5. Swiftly get rid of all your docker containers:
 ```shell
-$ comai give me a fortune cookie quote
-💡≫ fortune cookie
+$ comai stop and remove all running docker containers
+❯ docker stop $(docker ps -aq) && docker rm $(docker ps -aq)
 ```
 
 These are just a few examples of how `comai` can help you harness the power of the command line and provide you with useful and entertaining commands. Feel free to explore and experiment with the commands generated by `comai` to discover more exciting possibilities!
 
+## Contributions welcome! 🤝
+
+If you're interested in joining the development of new features for `comai`, here's all you need to get started:
+
+1. Clone the [repository](https://github.com/ricopinazo/comai) and navigate to the root folder.
+2. Install the package in editable mode by running `pip install -e .`.
+3. Run the tests using `pytest`. Make sure you have the `OPENAI_API_KEY` environment variable set up with your OpenAI API key. Alternatively, you can create a file named `.env` and define the variable there.
+
+
+This project utilizes black for code formatting. To ensure your changes adhere to this format, simply follow these steps:
+
+```shell
+pip install black
+black .
+```
+
+For users of VS Code, you can configure the following options after installing `black`:
+
+```json
+"editor.formatOnSave": true,
+"python.formatting.provider": "black"
+```
+
 ## License 📜
 
 Comai is licensed under the GPLv3. You can find the full text of the license in the [LICENSE](./LICENSE) file.
```

