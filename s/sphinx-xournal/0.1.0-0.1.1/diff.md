# Comparing `tmp/sphinx_xournal-0.1.0.tar.gz` & `tmp/sphinx_xournal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_xournal-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_xournal-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_xournal-0.1.0.tar` & `sphinx_xournal-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      268 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/.editorconfig
--rw-r--r--   0        0        0       62 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/.gitignore
--rw-r--r--   0        0        0     2244 2023-06-09 19:39:40.610842 sphinx_xournal-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      178 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/AUTHORS.rst
--rw-r--r--   0        0        0      156 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/HISTORY.rst
--rw-r--r--   0        0        0     7642 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/LICENSE
--rw-r--r--   0        0        0      167 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/README.rst
--rw-r--r--   0        0        0     1222 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/docs/templates/pyproject.toml
--rw-r--r--   0        0        0     1052 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      283 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/requirements.txt
--rw-r--r--   0        0        0      241 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/__init__.py
--rw-r--r--   0        0        0     3774 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/convert.py
--rw-r--r--   0        0        0     1713 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/directives.py
--rw-r--r--   0        0        0      945 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/exceptions.py
--rw-r--r--   0        0        0     1453 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/main.py
--rw-r--r--   0        0        0        0 2023-06-09 19:50:18.135236 sphinx_xournal-0.1.0/sphinx_xournal/xournal.css
--rw-r--r--   0        0        0     3320 2023-06-09 14:52:42.777621 sphinx_xournal-0.1.0/tasks.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 sphinx_xournal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/.editorconfig
+-rw-r--r--   0        0        0       62 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2336 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      178 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/AUTHORS.rst
+-rw-r--r--   0        0        0      306 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/HISTORY.rst
+-rw-r--r--   0        0        0     7642 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/LICENSE
+-rw-r--r--   0        0        0      167 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/README.rst
+-rw-r--r--   0        0        0     1222 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/docs/templates/pyproject.toml
+-rw-r--r--   0        0        0     1052 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      241 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/sphinx_xournal/__init__.py
+-rw-r--r--   0        0        0     4045 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/sphinx_xournal/convert.py
+-rw-r--r--   0        0        0     1713 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.1/sphinx_xournal/directives.py
+-rw-r--r--   0        0        0      825 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/sphinx_xournal/exceptions.py
+-rw-r--r--   0        0        0     1453 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.1/sphinx_xournal/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 00:29:20.406053 sphinx_xournal-0.1.1/sphinx_xournal/xournal.css
+-rw-r--r--   0        0        0     3320 2023-06-09 14:52:42.777621 sphinx_xournal-0.1.1/tasks.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 sphinx_xournal-0.1.1/PKG-INFO
```

### Comparing `sphinx_xournal-0.1.0/.gitlab-ci.yml` & `sphinx_xournal-0.1.1/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,16 @@
       allow_failure: true
 
 deploy-docs:
   image: python:3.11
   stage: release
   before_script:
     - export DISPLAY=:0
-    - apt-get update && apt-get -y install wget curl xvfb nano libgtk-3-0 libnotify4 libnss3 libxss1 libxtst6 xdg-utils libatspi2.0-0 libappindicator3-1 libsecret-1-0 libgbm1 desktop-file-utils libasound2 xournallpp && rm -rf /var/lib/apt/lists/*
+    - add-apt-repository ppa:apandada1/xournalpp-stable && apt-get update && apt-get install xournalpp
+    - apt-get update && apt-get -y install wget curl xvfb nano libgtk-3-0 libnotify4 libnss3 libxss1 libxtst6 xdg-utils libatspi2.0-0 libappindicator3-1 libsecret-1-0 libgbm1 desktop-file-utils libasound2 && rm -rf /var/lib/apt/lists/*
     - wget https://github.com/jgraph/drawio-desktop/releases/download/v$DRAWIO_VERSION/drawio-amd64-$DRAWIO_VERSION.deb
     - dpkg -i drawio-amd64-$DRAWIO_VERSION.deb
     - rm drawio-amd64-$DRAWIO_VERSION.deb
     - python -V
     - echo "${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi"
   script:
     - export DISPLAY=:0
```

### Comparing `sphinx_xournal-0.1.0/LICENSE` & `sphinx_xournal-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.0/docs/templates/pyproject.toml` & `sphinx_xournal-0.1.1/docs/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.0/pyproject.toml` & `sphinx_xournal-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.0/sphinx_xournal/convert.py` & `sphinx_xournal-0.1.1/sphinx_xournal/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 
     def is_available(self) -> bool:
         """Check if we can use this converter."""
         return True
 
     def guess_mimetypes(self, node: nodes.image) -> List[str]:
         """Should always be application/gzip unless a wrong file got passed in."""
-        return ["application/gzip"]
+        # Add compatibility with sphinxcontrib-drawio
+        if "drawio" in node.get("classes"):
+            return []
+        if node.get("format") == "xopp":
+            return ["application/gzip"]
+        return []
 
     def handle(self, node: nodes.image) -> None:
         """Find out if we can convert the file and do so."""
         candidates = node.get("candidates", {})
         from_type, to_type = self.get_conversion_rule(node)
         source_path = candidates.get(from_type, candidates["*"])
         absolute_source_path = Path(self.app.srcdir) / source_path
@@ -46,15 +51,18 @@
     def is_cached(file_path: Path, input_abspath: Path) -> bool:
         """Check if we can reuse the cached image."""
         return file_path.exists() and file_path.stat().st_mtime > input_abspath.stat().st_mtime
 
     @staticmethod
     def hash_image(input_abspath: Path, builder: Builder, options: dict) -> str:
         """Return the unique hash of the image and its properties."""
-        input_relpath = input_abspath.relative_to(builder.srcdir)
+        try:
+            input_relpath = input_abspath.relative_to(builder.srcdir)
+        except ValueError:
+            input_relpath = input_abspath.relative_to(builder.outdir)
         page = str(options.get("page", 0))
         unique_values = (str(input_relpath), page)
         hash_key = "\n".join(unique_values)
         sha_key = sha1(hash_key.encode()).hexdigest()
         return sha_key
 
     def generate(self, input_abspath: Path, options: dict, out_filename: str) -> Path:
@@ -67,16 +75,16 @@
             return output_image_file_path
         binary_path = builder.config.xournal_binary_path
         xournal_args = [binary_path, "--create-img", str(output_image_file_path), str(input_abspath)]
         new_env = os.environ.copy()
         try:
             value = subprocess.run(xournal_args, stderr=PIPE, stdout=PIPE, check=True, env=new_env)
         except OSError as exc:
-            raise XournalCallError(binary_path, xournal_args, exc)
+            raise XournalCallError(xournal_args, exc)
         except subprocess.CalledProcessError as exc:
-            raise XournalCallError(binary_path, xournal_args, exc.returncode, exc.stderr, exc.stdout)
+            raise XournalCallError(xournal_args, exc.returncode, exc.stderr, exc.stdout)
         return output_image_file_path
 
     @property
     def imagedir(self) -> str:
         """"""
         return str(Path(self.app.doctreedir) / Path("xournal"))
```

### Comparing `sphinx_xournal-0.1.0/sphinx_xournal/directives.py` & `sphinx_xournal-0.1.1/sphinx_xournal/directives.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.0/sphinx_xournal/main.py` & `sphinx_xournal-0.1.1/sphinx_xournal/main.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.0/tasks.py` & `sphinx_xournal-0.1.1/tasks.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.0/PKG-INFO` & `sphinx_xournal-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-xournal
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sphinx extension to generate images from xournal files.
 Keywords: sphinx,xournal,notes
 Author-email: Arkadiusz Michał Ryś <Arkadiusz.Michal.Rys@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python :: 3
```

