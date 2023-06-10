# Comparing `tmp/asp_chef_cli-0.1.3.tar.gz` & `tmp/asp_chef_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_chef_cli-0.1.3.tar", max compression
+gzip compressed data, was "asp_chef_cli-0.1.4.tar", max compression
```

## Comparing `asp_chef_cli-0.1.3.tar` & `asp_chef_cli-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0     2864 2023-06-09 21:10:23.234341 asp_chef_cli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_cli-0.1.3/asp_chef_cli/__init__.py
--rw-r--r--   0        0        0      102 2023-06-09 20:54:07.739786 asp_chef_cli-0.1.3/asp_chef_cli/__main__.py
--rwxr-xr-x   0        0        0     4155 2023-06-09 21:07:32.879890 asp_chef_cli-0.1.3/asp_chef_cli/cli.py
--rw-r--r--   0        0        0      399 2023-06-09 21:10:52.010140 asp_chef_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.3/setup.py
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_cli-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2991 2023-06-10 05:18:18.990369 asp_chef_cli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_cli-0.1.4/asp_chef_cli/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-09 20:54:07.739786 asp_chef_cli-0.1.4/asp_chef_cli/__main__.py
+-rwxr-xr-x   0        0        0     4155 2023-06-09 21:07:32.879890 asp_chef_cli-0.1.4/asp_chef_cli/cli.py
+-rw-r--r--   0        0        0      399 2023-06-10 05:18:45.986104 asp_chef_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.4/setup.py
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.4/PKG-INFO
```

### Comparing `asp_chef_cli-0.1.3/LICENSE` & `asp_chef_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_chef_cli-0.1.3/README.md` & `asp_chef_cli-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 The suggested way is via pip:
 ```bash
 $ pip install asp-chef-cli
 $ playwright install
 ```
 
-Docker is another option (for headless mode):
+Docker is another option (headed mode needs extra parameters):
 ```bash
-$ docker run malvi/asp-chef-headless
+$ docker run malvi/asp-chef-cli
+$ docker run docker run --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" malvi/asp-chef-cli
 ```
 
 
 
 
 ## Usage
 
 Run with one of the following commands:
 ```bash
-$ docker run malvi/asp-chef-headless --help
 $ python -m asp_chef_cli --help
+$ docker run malvi/asp-chef-cli --help
 ```
 
 Add the recipe (an ASP Chef sharable URL) with the option `--url` (quote the URL as it contains characters like # that breaks bash and other terminals).
 The headless mode can be activated with the flag `--headless` (always active in the docker image).
 Possibly change the default browser used by playwright with the option `--browser`.
 Finally, give a command to execute:
 * `run` simply runs the recipe as it is;
```

### Comparing `asp_chef_cli-0.1.3/asp_chef_cli/cli.py` & `asp_chef_cli-0.1.4/asp_chef_cli/cli.py`

 * *Files identical despite different names*

### Comparing `asp_chef_cli-0.1.3/setup.py` & `asp_chef_cli-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['dumbo-utils>=0.1.9,<0.2.0',
  'pytest-playwright>=0.3.3,<0.4.0',
  'rich>=13.4.1,<14.0.0',
  'typer>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'asp-chef-cli',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A simple CLI to run ASP Chef recipes',
-    'long_description': '# ASP Chef CLI\n\nA simple CLI to run ASP Chef, in headed or headless mode.\n\n\n## Install\n\nThe suggested way is via pip:\n```bash\n$ pip install asp-chef-cli\n$ playwright install\n```\n\nDocker is another option (for headless mode):\n```bash\n$ docker run malvi/asp-chef-headless\n```\n\n\n\n\n## Usage\n\nRun with one of the following commands:\n```bash\n$ docker run malvi/asp-chef-headless --help\n$ python -m asp_chef_cli --help\n```\n\nAdd the recipe (an ASP Chef sharable URL) with the option `--url` (quote the URL as it contains characters like # that breaks bash and other terminals).\nThe headless mode can be activated with the flag `--headless` (always active in the docker image).\nPossibly change the default browser used by playwright with the option `--browser`.\nFinally, give a command to execute:\n* `run` simply runs the recipe as it is;\n* `run-with` runs the recipe with the input replaced by the one specified either with the option `--input` or via the prompt.\n\nThe flag `--help` can be specified after a command to get a list of arguments for that command.\n\n\n## Examples\n\nLet us consider [this simple recipe](https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21) with no input and guessing the atom `world`.\nThe recipe can be run headless by giving the following command:\n```bash\n$ python -m asp_chef_cli --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run\nEMPTY MODEL\n§\nworld.\n```\n\nIt is possible to specify a different input as follows:\n```bash\n$ python -m asp_chef_headless --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run-with --input "hello."\nhello.\n§\nhello.\nworld.\n```',
+    'long_description': '# ASP Chef CLI\n\nA simple CLI to run ASP Chef, in headed or headless mode.\n\n\n## Install\n\nThe suggested way is via pip:\n```bash\n$ pip install asp-chef-cli\n$ playwright install\n```\n\nDocker is another option (headed mode needs extra parameters):\n```bash\n$ docker run malvi/asp-chef-cli\n$ docker run docker run --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" malvi/asp-chef-cli\n```\n\n\n\n\n## Usage\n\nRun with one of the following commands:\n```bash\n$ python -m asp_chef_cli --help\n$ docker run malvi/asp-chef-cli --help\n```\n\nAdd the recipe (an ASP Chef sharable URL) with the option `--url` (quote the URL as it contains characters like # that breaks bash and other terminals).\nThe headless mode can be activated with the flag `--headless` (always active in the docker image).\nPossibly change the default browser used by playwright with the option `--browser`.\nFinally, give a command to execute:\n* `run` simply runs the recipe as it is;\n* `run-with` runs the recipe with the input replaced by the one specified either with the option `--input` or via the prompt.\n\nThe flag `--help` can be specified after a command to get a list of arguments for that command.\n\n\n## Examples\n\nLet us consider [this simple recipe](https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21) with no input and guessing the atom `world`.\nThe recipe can be run headless by giving the following command:\n```bash\n$ python -m asp_chef_cli --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run\nEMPTY MODEL\n§\nworld.\n```\n\nIt is possible to specify a different input as follows:\n```bash\n$ python -m asp_chef_headless --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run-with --input "hello."\nhello.\n§\nhello.\nworld.\n```',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `asp_chef_cli-0.1.3/PKG-INFO` & `asp_chef_cli-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp-chef-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple CLI to run ASP Chef recipes
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,28 +23,29 @@
 
 The suggested way is via pip:
 ```bash
 $ pip install asp-chef-cli
 $ playwright install
 ```
 
-Docker is another option (for headless mode):
+Docker is another option (headed mode needs extra parameters):
 ```bash
-$ docker run malvi/asp-chef-headless
+$ docker run malvi/asp-chef-cli
+$ docker run docker run --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" malvi/asp-chef-cli
 ```
 
 
 
 
 ## Usage
 
 Run with one of the following commands:
 ```bash
-$ docker run malvi/asp-chef-headless --help
 $ python -m asp_chef_cli --help
+$ docker run malvi/asp-chef-cli --help
 ```
 
 Add the recipe (an ASP Chef sharable URL) with the option `--url` (quote the URL as it contains characters like # that breaks bash and other terminals).
 The headless mode can be activated with the flag `--headless` (always active in the docker image).
 Possibly change the default browser used by playwright with the option `--browser`.
 Finally, give a command to execute:
 * `run` simply runs the recipe as it is;
```

