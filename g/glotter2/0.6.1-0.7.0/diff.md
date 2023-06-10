# Comparing `tmp/glotter2-0.6.1.tar.gz` & `tmp/glotter2-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glotter2-0.6.1.tar", max compression
+gzip compressed data, was "glotter2-0.7.0.tar", max compression
```

## Comparing `glotter2-0.6.1.tar` & `glotter2-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1105 2023-02-25 14:19:23.663270 glotter2-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     2820 2023-05-06 11:22:09.635606 glotter2-0.6.1/README.md
--rw-r--r--   0        0        0      191 2023-04-01 17:41:06.994287 glotter2-0.6.1/glotter/__init__.py
--rw-r--r--   0        0        0     3271 2023-03-02 01:12:21.951067 glotter2-0.6.1/glotter/__main__.py
--rw-r--r--   0        0        0    12978 2023-03-28 18:23:01.742869 glotter2-0.6.1/glotter/auto_gen_test.py
--rw-r--r--   0        0        0     3781 2023-03-02 02:24:54.569331 glotter2-0.6.1/glotter/containerfactory.py
--rw-r--r--   0        0        0      680 2023-02-26 16:00:40.206266 glotter2-0.6.1/glotter/decorators.py
--rw-r--r--   0        0        0      959 2023-03-02 00:31:52.361647 glotter2-0.6.1/glotter/download.py
--rw-r--r--   0        0        0     4753 2023-03-18 14:28:46.995459 glotter2-0.6.1/glotter/project.py
--rw-r--r--   0        0        0     3087 2023-02-26 19:19:43.729458 glotter2-0.6.1/glotter/report.py
--rw-r--r--   0        0        0      728 2023-03-01 00:45:45.072395 glotter2-0.6.1/glotter/run.py
--rw-r--r--   0        0        0     7758 2023-03-18 19:56:57.285778 glotter2-0.6.1/glotter/settings.py
--rw-r--r--   0        0        0      327 2023-03-14 17:43:43.187564 glotter2-0.6.1/glotter/singleton.py
--rw-r--r--   0        0        0     6263 2023-03-17 22:38:08.039572 glotter2-0.6.1/glotter/source.py
--rw-r--r--   0        0        0     1933 2023-03-17 22:36:01.438407 glotter2-0.6.1/glotter/test.py
--rw-r--r--   0        0        0     5027 2023-04-01 18:00:31.534775 glotter2-0.6.1/glotter/test_doc_generator.py
--rw-r--r--   0        0        0     2161 2023-03-17 22:20:40.522430 glotter2-0.6.1/glotter/test_generator.py
--rw-r--r--   0        0        0     5490 2023-02-25 19:40:59.629278 glotter2-0.6.1/glotter/testinfo.py
--rw-r--r--   0        0        0      853 2023-03-17 22:34:49.362111 glotter2-0.6.1/glotter/utils.py
--rw-r--r--   0        0        0     1590 2023-05-06 11:24:16.524057 glotter2-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 glotter2-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-02-25 14:19:23.663270 glotter2-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3061 2023-06-10 21:19:18.566829 glotter2-0.7.0/README.md
+-rw-r--r--   0        0        0      191 2023-04-01 17:41:06.994287 glotter2-0.7.0/glotter/__init__.py
+-rw-r--r--   0        0        0     4258 2023-06-10 17:29:20.213170 glotter2-0.7.0/glotter/__main__.py
+-rw-r--r--   0        0        0    12978 2023-03-28 18:23:01.742869 glotter2-0.7.0/glotter/auto_gen_test.py
+-rw-r--r--   0        0        0     2334 2023-06-10 21:13:27.448366 glotter2-0.7.0/glotter/batch.py
+-rw-r--r--   0        0        0     4297 2023-06-10 00:48:10.057388 glotter2-0.7.0/glotter/containerfactory.py
+-rw-r--r--   0        0        0      680 2023-02-26 16:00:40.206266 glotter2-0.7.0/glotter/decorators.py
+-rw-r--r--   0        0        0     1340 2023-06-10 19:43:20.404026 glotter2-0.7.0/glotter/download.py
+-rw-r--r--   0        0        0     4753 2023-03-18 14:28:46.995459 glotter2-0.7.0/glotter/project.py
+-rw-r--r--   0        0        0     3087 2023-02-26 19:19:43.729458 glotter2-0.7.0/glotter/report.py
+-rw-r--r--   0        0        0      762 2023-06-08 23:13:27.025405 glotter2-0.7.0/glotter/run.py
+-rw-r--r--   0        0        0     7758 2023-03-18 19:56:57.285778 glotter2-0.7.0/glotter/settings.py
+-rw-r--r--   0        0        0      327 2023-03-14 17:43:43.187564 glotter2-0.7.0/glotter/singleton.py
+-rw-r--r--   0        0        0     6648 2023-06-10 00:21:29.981543 glotter2-0.7.0/glotter/source.py
+-rw-r--r--   0        0        0     1933 2023-03-17 22:36:01.438407 glotter2-0.7.0/glotter/test.py
+-rw-r--r--   0        0        0     5027 2023-04-01 18:00:31.534775 glotter2-0.7.0/glotter/test_doc_generator.py
+-rw-r--r--   0        0        0     2195 2023-06-08 23:02:04.303251 glotter2-0.7.0/glotter/test_generator.py
+-rw-r--r--   0        0        0     5490 2023-02-25 19:40:59.629278 glotter2-0.7.0/glotter/testinfo.py
+-rw-r--r--   0        0        0      853 2023-03-17 22:34:49.362111 glotter2-0.7.0/glotter/utils.py
+-rw-r--r--   0        0        0     1595 2023-06-10 21:22:22.371463 glotter2-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4309 1970-01-01 00:00:00.000000 glotter2-0.7.0/PKG-INFO
```

### Comparing `glotter2-0.6.1/LICENSE.txt` & `glotter2-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/README.md` & `glotter2-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
 If you'd like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).
 
 ## Changelog
 
 ### Glotter2 releases
 
+* 0.7.0: work-in-progress
+  * Add `try/finally` to auto-generated project fixture to make sure docker
+    container is cleaned up
+  * Add `try/finally` to `run` command to make sure docker container is
+    cleaned up
+  * Add `batch` command
 * 0.6.1:
   * Update `docker` dependency to 6.1.0 to support `urllib3` 2.x
 * 0.6.0:
   * Add test documentation generation
 * 0.5.0:
   * Add test generation
   * Add `pydantic` dependency
```

### Comparing `glotter2-0.6.1/glotter/__main__.py` & `glotter2-0.7.0/glotter/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import sys
 import argparse
 
 from glotter.run import run
 from glotter.test import test
 from glotter.download import download
 from glotter.report import report
+from glotter.batch import batch
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="glotter",
         usage="""usage: glotter [-h] COMMAND
 
 Commands:
   run         Run sources or group of sources. Use `glotter run --help` for more information.
   test        Run tests for sources or a group of sources. Use `glotter test --help` for more information.
   download    Download all the docker images required to run the tests
   report      Output a report of discovered sources for configured projects and languages
+  batch       Download docker images, run tests, and optionally remove images for each batch
 """,
     )
     parser.add_argument(
         "command",
         type=str,
         help="Subcommand to run",
-        choices=["run", "test", "download", "report"],
+        choices=["run", "test", "download", "report", "batch"],
     )
     args = parser.parse_args(sys.argv[1:2])
     commands = {
         "download": parse_download,
         "run": parse_run,
         "test": parse_test,
         "report": parse_report,
+        "batch": parse_batch,
     }
     commands[args.command]()
 
 
 def parse_download():
     parser = argparse.ArgumentParser(
         prog="glotter",
@@ -109,9 +112,34 @@
         type=str,
         help="output the report as a csv at REPORT_PATH instead of to stdout",
     )
     args = parser.parse_args(sys.argv[2:])
     report(args)
 
 
+def parse_batch():
+    parser = argparse.ArgumentParser(
+        prog="glotter",
+        description="Download images, run tests, and optionally remove image in batches"
+        "project, or a single source. Only one option may be specified.",
+    )
+    parser.add_argument(
+        "num_batches", metavar="NUM_BATCHES", type=int, help="number of batches"
+    )
+    _add_parallel_arg(
+        parser,
+        "Download images, run tests, and optionally remove images in parallel for each batch",
+    )
+    parser.add_argument(
+        "--batch", type=int, metavar="BATCH", help="batch number (1 to NUM_BATCHES)"
+    )
+    parser.add_argument(
+        "--remove",
+        action="store_true",
+        help="remove docker images are each batch is finished",
+    )
+    args = parser.parse_args(sys.argv[2:])
+    batch(args)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `glotter2-0.6.1/glotter/auto_gen_test.py` & `glotter2-0.7.0/glotter/auto_gen_test.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/containerfactory.py` & `glotter2-0.7.0/glotter/containerfactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,14 +95,29 @@
             name=f"{container_info.image}:{str(container_info.tag)}"
         )
         if len(images) == 1:
             return images[0]
 
         return None
 
+    def remove_image(self, container_info):
+        """
+        Remove a docker image
+
+        :param container_info: metadata about the image to remove
+        """
+
+        image_name = f"{container_info.image}:{str(container_info.tag)}"
+        images = self._client.images.list(
+            name=f"{container_info.image}:{str(container_info.tag)}"
+        )
+        if len(images) == 1:
+            print(f"Removing {image_name}", flush=True)
+            self._client.images.remove(image=image_name, force=True)
+
     def cleanup(self, source):
         """
         Cleanup docker container and temporary folder. Also remove both from their
         respective dictionaries
 
         :param source: source for determining what to cleanup
         """
```

### Comparing `glotter2-0.6.1/glotter/decorators.py` & `glotter2-0.7.0/glotter/decorators.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/download.py` & `glotter2-0.7.0/glotter/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,35 @@
 from glotter.settings import Settings
 from glotter.containerfactory import ContainerFactory
 
 
 def download(args):
     sources_by_type = filter_sources(args, get_sources(Settings().source_root))
     containers = {
-        source.test_info.container_info.image: source.test_info.container_info
+        f"{source.test_info.container_info.image}:{str(source.test_info.container_info.tag)}": source.test_info.container_info
         for sources in sources_by_type.values()
         for source in sources
     }
-
     if args.parallel:
         with ThreadPoolExecutor(max_workers=4) as executor:
             executor.map(
                 lambda source: _download_image_from_source(source, True),
                 containers.values(),
             )
     else:
         for container_info in containers:
             _download_image_from_source(container_info)
 
+    return containers
+
 
 def _download_image_from_source(container_info, parallel=False):
     ContainerFactory().get_image(container_info, parallel=parallel)
+
+
+def remove_images(containers, parallel):
+    if parallel:
+        with ThreadPoolExecutor(max_workers=4) as executor:
+            executor.map(ContainerFactory().remove_image, containers.values())
+    else:
+        for container_info in containers:
+            ContainerFactory().remove_image(container_info)
```

### Comparing `glotter2-0.6.1/glotter/project.py` & `glotter2-0.7.0/glotter/project.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/report.py` & `glotter2-0.7.0/glotter/report.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/run.py` & `glotter2-0.7.0/glotter/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,10 +15,12 @@
         return ""
     return input(f'input parameters for "{project_type}": ')
 
 
 def _build_and_run(source, params):
     print()
     print(f'Running "{source.name}{source.extension}"...')
-    source.build()
-    print(source.run(params))
-    source.cleanup()
+    try:
+        source.build()
+        print(source.run(params))
+    finally:
+        source.cleanup()
```

### Comparing `glotter2-0.6.1/glotter/settings.py` & `glotter2-0.7.0/glotter/settings.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/source.py` & `glotter2-0.7.0/glotter/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,29 +166,39 @@
 
     if not filtered_sources_by_type:
         errors = []
         if args.project:
             errors.append(f'project "{args.project}"')
 
         if args.language:
-            errors.append(f'language "{args.language}"')
+            if isinstance(args.language, set):
+                errors.append(
+                    "languages "
+                    + ", ".join(f'"{language}"' for language in sorted(args.language))
+                )
+            else:
+                errors.append(f'language "{args.language}"')
 
         if args.source:
             errors.append(f'source "{args.source}"')
 
         if errors:
             error_msg = ", ".join(errors)
             error_and_exit(
                 f"No valid sources found for the following combination: {error_msg}"
             )
 
     return filtered_sources_by_type
 
 
 def _matches_source(args, source):
-    if args.language and source.language.lower() != args.language.lower():
-        return False
+    if args.language:
+        if isinstance(args.language, set):
+            if source.language.lower() not in args.language:
+                return False
+        elif source.language.lower() != args.language.lower():
+            return False
 
     return (
         not args.source
         or f"{source.name}{source.extension}".lower() == args.source.lower()
     )
```

### Comparing `glotter2-0.6.1/glotter/test.py` & `glotter2-0.7.0/glotter/test.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/test_doc_generator.py` & `glotter2-0.7.0/glotter/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/test_generator.py` & `glotter2-0.7.0/glotter/test_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,17 +56,19 @@
         return test_code
 
     def _get_project_fixture(self):
         return f"""\
 PROJECT_NAME="{self.project_name}"
 @project_fixture(PROJECT_NAME)
 def {self.long_project_name}(request):
-    request.param.build()
-    yield request.param
-    request.param.cleanup()
+    try:
+        request.param.build()
+        yield request.param
+    finally:
+        request.param.cleanup()
 """
 
     def write_tests(self, test_code):
         os.makedirs(AUTO_GEN_TEST_PATH, exist_ok=True)
         with open(
             os.path.join(AUTO_GEN_TEST_PATH, f"test_{self.long_project_name}.py"),
             "w",
```

### Comparing `glotter2-0.6.1/glotter/testinfo.py` & `glotter2-0.7.0/glotter/testinfo.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/glotter/utils.py` & `glotter2-0.7.0/glotter/utils.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.1/pyproject.toml` & `glotter2-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "glotter2"
 packages = [{include="glotter"}]
-version = "0.6.1"
+version = "0.7.0"
 description = "An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter"
 authors = ["auroq", "rzuckerm"]
 readme = "README.md"
 license = "LICENSE.txt"
 homepage = "https://github.com/rzuckerm/glotter2"
 documentation = "https://rzuckerm.github.io/glotter2"
 classifiers = [
@@ -55,10 +55,10 @@
     "too-few-public-methods",
     "no-else-return",
     "too-many-arguments"
 ]
 
 [tool.pylint.basic]
 good-names = [
-    "e", "f", "k", "v",
+    "e", "f", "k", "v", "n",
     "hyphen", "underscore", "camel", "pascal", "lower", "upper", "two_letter_limit"
 ]
```

### Comparing `glotter2-0.6.1/PKG-INFO` & `glotter2-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glotter2
-Version: 0.6.1
+Version: 0.7.0
 Summary: An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter
 Home-page: https://github.com/rzuckerm/glotter2
 License: LICENSE.txt
 Author: auroq
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -50,14 +50,20 @@
 
 If you'd like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).
 
 ## Changelog
 
 ### Glotter2 releases
 
+* 0.7.0: work-in-progress
+  * Add `try/finally` to auto-generated project fixture to make sure docker
+    container is cleaned up
+  * Add `try/finally` to `run` command to make sure docker container is
+    cleaned up
+  * Add `batch` command
 * 0.6.1:
   * Update `docker` dependency to 6.1.0 to support `urllib3` 2.x
 * 0.6.0:
   * Add test documentation generation
 * 0.5.0:
   * Add test generation
   * Add `pydantic` dependency
```

