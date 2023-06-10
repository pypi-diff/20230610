# Comparing `tmp/chachacha-0.2.3.tar.gz` & `tmp/chachacha-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chachacha-0.2.3.tar", max compression
+gzip compressed data, was "chachacha-0.2.4.tar", max compression
```

## Comparing `chachacha-0.2.3.tar` & `chachacha-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4763 2023-04-03 10:58:35.709336 chachacha-0.2.3/README.md
--rw-r--r--   0        0        0       22 2023-04-03 10:58:35.709336 chachacha-0.2.3/chachacha/__init__.py
--rw-r--r--   0        0        0     1632 2023-04-03 10:58:35.709336 chachacha-0.2.3/chachacha/configuration.py
--rw-r--r--   0        0        0        0 2023-04-03 10:58:35.709336 chachacha-0.2.3/chachacha/drivers/__init__.py
--rw-r--r--   0        0        0     1518 2023-04-03 10:58:35.709336 chachacha-0.2.3/chachacha/drivers/git_provider.py
--rw-r--r--   0        0        0     4670 2023-04-03 10:58:35.709336 chachacha-0.2.3/chachacha/drivers/kac.py
--rw-r--r--   0        0        0     4250 2023-04-03 10:58:35.709336 chachacha-0.2.3/chachacha/main.py
--rw-r--r--   0        0        0     1025 2023-04-03 10:58:35.717336 chachacha-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 chachacha-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4763 2023-06-10 11:39:23.648988 chachacha-0.2.4/README.md
+-rw-r--r--   0        0        0       22 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/__init__.py
+-rw-r--r--   0        0        0     1691 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/configuration.py
+-rw-r--r--   0        0        0        0 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/drivers/__init__.py
+-rw-r--r--   0        0        0     1629 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/drivers/git_provider.py
+-rw-r--r--   0        0        0     4670 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/drivers/kac.py
+-rw-r--r--   0        0        0     4250 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/main.py
+-rw-r--r--   0        0        0     1029 2023-06-10 11:39:23.652989 chachacha-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5894 1970-01-01 00:00:00.000000 chachacha-0.2.4/PKG-INFO
```

### Comparing `chachacha-0.2.3/README.md` & `chachacha-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.3/chachacha/configuration.py` & `chachacha-0.2.4/chachacha/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 @dataclass
 class Configuration:
     conf_map = {
         "D": "driver",
         "G": "git_provider",
         "R": "repo_name",
         "T": "tag_template",
+        "H": "host",
     }
 
     version = 2
     driver: str
     git_provider: str
     repo_name: str
     tag_template: str
+    host: str
 
     def marshal(self):
         revmap = {v: k for k, v in self.conf_map.items()}
         conf = []
         for k, v in asdict(self).items():
             if v:
                 conf.append(f"{revmap[k]}{v}")
@@ -52,13 +54,14 @@
             )
 
         configuration = {
             "driver": "",
             "git_provider": "",
             "repo_name": "",
             "tag_template": "",
+            "host": "",
         }
 
         for arg in args:
             configuration[Configuration.conf_map[arg[0]]] = arg[1:]
 
         return Configuration(**configuration)
```

### Comparing `chachacha-0.2.3/chachacha/drivers/git_provider.py` & `chachacha-0.2.4/chachacha/drivers/git_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     "GH": {
         "desc": "Github.com template",
         "compare": "https://github.com/{repo_name}/compare/{new}...{old}",
         "tag": "https://github.com/{repo_name}/releases/tag/{tag}",
     },
     "GL": {
         "desc": "Gitlab.com template",
-        "compare": "https://gitlab.com/{repo_name}/-/compare/{new}...{old}",
-        "tag": "https://gitlab.com/{repo_name}/-/tags/{tag}",
+        "compare": "https://{host}/{repo_name}/-/compare/{new}...{old}",
+        "tag": "https://{host}/{repo_name}/-/tags/{tag}",
     },
 }
 
 
 class Provider:
     def __init__(self, changelog, config):
         self.changelog = changelog
@@ -35,13 +35,16 @@
         for release in self.changelog:
             yield last if last != "HEAD" else "Unreleased", PROVIDERS[
                 self.config.git_provider
             ]["compare"].format(
                 repo_name=self.config.repo_name,
                 new=self.config.tag_template.format(t=release),
                 old=self.config.tag_template.format(t=last) if last != "HEAD" else last,
+                host=self.config.host or "gitlab.com",
             )
             last = release
 
         yield last, PROVIDERS[self.config.git_provider]["tag"].format(
-            repo_name=self.config.repo_name, tag=self.config.tag_template.format(t=last)
+            repo_name=self.config.repo_name,
+            tag=self.config.tag_template.format(t=last),
+            host=self.config.host or "gitlab.com",
         )
```

### Comparing `chachacha-0.2.3/chachacha/drivers/kac.py` & `chachacha-0.2.4/chachacha/drivers/kac.py`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.3/chachacha/main.py` & `chachacha-0.2.4/chachacha/main.py`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.3/pyproject.toml` & `chachacha-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "chachacha"
 description = "Chachacha changes changelogs"
-version = "0.2.3"
+version = "0.2.4"
 authors = ["Alessandro Ogier <alessandro.ogier@gmail.com>"]
 readme = "README.md"
 license = "BSD"
 repository = "https://github.com/aogier/chachacha"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
@@ -25,19 +25,19 @@
 keepachangelog = "^0.3.1"
 click = "^8.1.0"
 jinja2 = "^3.1.0"
 semver = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
-mypy = "^1.1"
+mypy = "^1.3"
 black = "^23"
 autoflake = "^2.0"
 pytest-cov = "^4"
 pyinstaller = "^4.1"
 pylint = "^2.5.3"
 codecov = "^2.1.12"
 
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `chachacha-0.2.3/PKG-INFO` & `chachacha-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chachacha
-Version: 0.2.3
+Version: 0.2.4
 Summary: Chachacha changes changelogs
 Home-page: https://github.com/aogier/chachacha
 License: BSD
 Author: Alessandro Ogier
 Author-email: alessandro.ogier@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,16 +15,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.0,<4.0.0)
 Requires-Dist: keepachangelog (>=0.3.1,<0.4.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/aogier/chachacha
 Description-Content-Type: text/markdown
```

