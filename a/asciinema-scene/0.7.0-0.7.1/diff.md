# Comparing `tmp/asciinema_scene-0.7.0.tar.gz` & `tmp/asciinema_scene-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciinema_scene-0.7.0.tar", max compression
+gzip compressed data, was "asciinema_scene-0.7.1.tar", max compression
```

## Comparing `asciinema_scene-0.7.0.tar` & `asciinema_scene-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-05-28 08:56:04.271598 asciinema_scene-0.7.0/LICENSE
--rw-r--r--   0        0        0    14025 2023-06-03 14:11:51.106725 asciinema_scene-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-05-27 11:46:28.615482 asciinema_scene-0.7.0/asciinema_scene/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 19:33:44.981797 asciinema_scene-0.7.0/asciinema_scene/scenelib/__init__.py
--rw-r--r--   0        0        0       75 2023-06-03 13:04:22.243864 asciinema_scene-0.7.0/asciinema_scene/scenelib/constants.py
--rw-r--r--   0        0        0     2437 2023-06-03 13:04:22.243994 asciinema_scene-0.7.0/asciinema_scene/scenelib/frame.py
--rw-r--r--   0        0        0     9953 2023-06-03 13:04:22.244155 asciinema_scene-0.7.0/asciinema_scene/scenelib/scene.py
--rw-r--r--   0        0        0     4991 2023-06-03 13:04:22.244308 asciinema_scene-0.7.0/asciinema_scene/scenelib/scene_content.py
--rw-r--r--   0        0        0     8511 2023-06-03 13:04:22.244461 asciinema_scene-0.7.0/asciinema_scene/sciine.py
--rw-r--r--   0        0        0     2105 2023-06-03 14:06:34.479951 asciinema_scene-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    14939 1970-01-01 00:00:00.000000 asciinema_scene-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-10 12:44:09.777665 asciinema_scene-0.7.1/LICENSE
+-rw-r--r--   0        0        0    14186 2023-06-10 12:44:09.777901 asciinema_scene-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 12:44:09.777955 asciinema_scene-0.7.1/asciinema_scene/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 12:44:09.778030 asciinema_scene-0.7.1/asciinema_scene/scenelib/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-10 12:44:09.778265 asciinema_scene-0.7.1/asciinema_scene/scenelib/constants.py
+-rw-r--r--   0        0        0     2437 2023-06-10 12:44:09.778386 asciinema_scene-0.7.1/asciinema_scene/scenelib/frame.py
+-rw-r--r--   0        0        0     9949 2023-06-10 12:44:09.778773 asciinema_scene-0.7.1/asciinema_scene/scenelib/scene.py
+-rw-r--r--   0        0        0     5062 2023-06-10 12:44:09.779034 asciinema_scene-0.7.1/asciinema_scene/scenelib/scene_content.py
+-rw-r--r--   0        0        0      375 2023-06-10 12:44:09.779251 asciinema_scene-0.7.1/asciinema_scene/scenelib/utils.py
+-rw-r--r--   0        0        0     9365 2023-06-10 12:44:09.779469 asciinema_scene-0.7.1/asciinema_scene/sciine.py
+-rw-r--r--   0        0        0     2163 2023-06-10 12:44:09.780605 asciinema_scene-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    15100 1970-01-01 00:00:00.000000 asciinema_scene-0.7.1/PKG-INFO
```

### Comparing `asciinema_scene-0.7.0/LICENSE` & `asciinema_scene-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asciinema_scene-0.7.0/README.md` & `asciinema_scene-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # asciinema-scene
 
 [![Release](https://img.shields.io/github/v/release/jdum/asciinema-scene)](https://img.shields.io/github/v/release/jdum/asciinema-scene)
 [![Build status](https://img.shields.io/github/actions/workflow/status/jdum/asciinema-scene/main.yml?branch=main)](https://github.com/jdum/asciinema-scene/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/jdum/asciinema-scene/branch/main/graph/badge.svg)](https://codecov.io/gh/jdum/asciinema-scene)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/jdum/asciinema-scene)](https://img.shields.io/github/commit-activity/m/jdum/asciinema-scene)
 [![License](https://img.shields.io/github/license/jdum/asciinema-scene)](https://img.shields.io/github/license/jdum/asciinema-scene)
 
 `asciinema-scene` provides the `sciine` command line toolkit for editing screen casts produced by [asciinema](https://asciinema.org/).
 
 `sciine` takes as input the content of a screencast, apply a unitary transformation and returns the transformed content.
```

### Comparing `asciinema_scene-0.7.0/asciinema_scene/scenelib/frame.py` & `asciinema_scene-0.7.1/asciinema_scene/scenelib/frame.py`

 * *Files identical despite different names*

### Comparing `asciinema_scene-0.7.0/asciinema_scene/scenelib/scene.py` & `asciinema_scene-0.7.1/asciinema_scene/scenelib/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from .frame import Frame
 from .scene_content import SceneContent
 
 
 class Scene(SceneContent):
     @classmethod
     def parse(cls, input_file: str | Path | None = None) -> Scene:
-        scformat = SceneContent.parse(input_file)
+        content = SceneContent.parse(input_file)
         scene = Scene()
-        scene.input_file = scformat.input_file
-        scene.header = scformat.header
-        scene.frames = scformat.frames
+        scene.input_file = content.input_file
+        scene.header = content.header
+        scene.frames = content.frames
         return scene
 
     def _split_parts(
         self,
         tcode_start: int,
         tcode_end: int,
     ) -> tuple[int, int]:
```

### Comparing `asciinema_scene-0.7.0/asciinema_scene/scenelib/scene_content.py` & `asciinema_scene-0.7.1/asciinema_scene/scenelib/scene_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from datetime import datetime, timezone
 from pathlib import Path
 from time import time
 from typing import Any
 from zipfile import ZipFile
 
 from .frame import Frame
+from .utils import detect_stdin_timeout
 
 
 class SceneContent:
     def __init__(self) -> None:
         self.input_file: str = "string"
         self.header: dict[str, Any] = {}
         self.frames: list[Frame] = []
@@ -62,14 +63,15 @@
             scene.parse_content(path.read_text(encoding="utf8"))
         return scene
 
     @classmethod
     def parse(cls, input_file: str | Path | None = None) -> SceneContent:
         if input_file:
             return cls.from_file(input_file)
+        detect_stdin_timeout()
         scene = SceneContent()
         scene.input_file = "sys.stdin"
         scene.parse_content("\n".join(list(sys.stdin)))
         return scene
 
     def duplicate(self) -> SceneContent:
         duplicate = SceneContent()
```

### Comparing `asciinema_scene-0.7.0/asciinema_scene/sciine.py` & `asciinema_scene-0.7.1/asciinema_scene/sciine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import importlib.metadata
+from collections.abc import Callable
+from functools import wraps
 from pprint import pformat
+from typing import Any
 
 import click
 
 from .scenelib.scene import Scene
+from .scenelib.utils import SceneStdinError
 
 __version__ = importlib.metadata.version("asciinema_scene")
 
 input_option = click.option(
     "--input",
     "-i",
     "input_file",
@@ -38,37 +42,54 @@
     "-a",
     is_flag=True,
     default=False,
     help="Adjust durations of frames at precise cut values.",
 )
 
 
+def stdin_timeout_handler(function: Callable) -> Callable:
+    @wraps(function)
+    def wrapped(*args: list[Any], **kwargs: dict[str, Any]) -> Any:
+        try:
+            function(*args, **kwargs)
+        except SceneStdinError:
+            print("Timeout while waiting for STDIN input.\n")
+            ctx = click.get_current_context()
+            click.echo(ctx.get_help())
+            ctx.exit()
+
+    return wrapped
+
+
 @click.group(invoke_without_command=True, no_args_is_help=True)
 @click.version_option(version=__version__)
 def cli() -> None:
     pass
 
 
 @cli.command("status")
+@stdin_timeout_handler
 @input_option
 def info_cmd(input_file: str | None) -> None:
     """Print informations about the content (duration, ...)."""
     scene = Scene.parse(input_file)
     print(scene.info)
 
 
 @cli.command("header")
+@stdin_timeout_handler
 @input_option
 def header_cmd(input_file: str | None) -> None:
     """Print the header field of the content."""
     scene = Scene.parse(input_file)
     print(pformat(scene.header))
 
 
 @cli.command("show")
+@stdin_timeout_handler
 @start_option
 @end_option
 @click.option(
     "--lines",
     "-l",
     type=int,
     help="Number of lines to show.",
@@ -111,14 +132,15 @@
         max_lines=lines,
         precise=precise,
         as_str=as_str,
     )
 
 
 @cli.command("cut")
+@stdin_timeout_handler
 @start_option
 @end_option
 @adjust_option
 @input_option
 @output_option
 def cut_cmd(
     start: float | None,
@@ -134,14 +156,15 @@
     """
     scene = Scene.parse(input_file)
     scene.cut_frames(start=start, end=end, adjust=adjust)
     scene.dump(output_file)
 
 
 @cli.command("copy")
+@stdin_timeout_handler
 @start_option
 @end_option
 @input_option
 @output_option
 def copy_cmd(
     start: float | None,
     end: float | None,
@@ -152,14 +175,15 @@
     """Copy content between START and END timecodes."""
     scene = Scene.parse(input_file)
     scene.copy(start=start, end=end, adjust=adjust)
     scene.dump(output_file)
 
 
 @cli.command("speed")
+@stdin_timeout_handler
 @click.argument("speed", required=True, type=float)
 @start_option
 @end_option
 @input_option
 @output_option
 def speed_cmd(
     speed: float,
@@ -177,14 +201,15 @@
     """
     scene = Scene.parse(input_file)
     scene.speed(speed, start=start, end=end)
     scene.dump(output_file)
 
 
 @cli.command("maximum")
+@stdin_timeout_handler
 @click.argument("duration", required=True, type=float)
 @start_option
 @end_option
 @input_option
 @output_option
 def maximum_cmd(
     duration: float,
@@ -202,14 +227,15 @@
     """
     scene = Scene.parse(input_file)
     scene.maximum(duration, start=start, end=end)
     scene.dump(output_file)
 
 
 @cli.command("minimum")
+@stdin_timeout_handler
 @click.argument("duration", required=True, type=float)
 @start_option
 @end_option
 @input_option
 @output_option
 def minimum_cmd(
     duration: float,
@@ -227,14 +253,15 @@
     """
     scene = Scene.parse(input_file)
     scene.minimum(duration, start=start, end=end)
     scene.dump(output_file)
 
 
 @cli.command("quantize")
+@stdin_timeout_handler
 @click.argument("range_min", required=True, type=float)
 @click.argument("range_max", required=True, type=float)
 @click.argument("duration", required=True, type=float)
 @start_option
 @end_option
 @input_option
 @output_option
@@ -256,14 +283,15 @@
     """
     scene = Scene.parse(input_file)
     scene.quantize(range_min, range_max, duration, start=start, end=end)
     scene.dump(output_file)
 
 
 @cli.command("insert")
+@stdin_timeout_handler
 @click.argument("timecode", required=True, type=float)
 @click.argument("duration", required=True, type=float)
 @click.argument("text", required=True, type=str)
 @click.argument("etype", required=False, type=str)
 @input_option
 @output_option
 def insert_cmd(
@@ -283,14 +311,15 @@
     if not etype:
         etype = "o"
     scene.insert(timecode, duration, text, etype)
     scene.dump(output_file)
 
 
 @cli.command("delete")
+@stdin_timeout_handler
 @click.argument("timecode", required=True, type=float)
 @input_option
 @output_option
 def delete_cmd(
     timecode: float,
     input_file: str | None,
     output_file: str | None,
@@ -298,14 +327,15 @@
     """Delete the frame with timecode >= TIMECODE."""
     scene = Scene.parse(input_file)
     scene.delete(timecode)
     scene.dump(output_file)
 
 
 @cli.command("replace")
+@stdin_timeout_handler
 @click.argument("timecode", required=True, type=float)
 @click.argument("text", required=True, type=str)
 @input_option
 @output_option
 def replace_cmd(
     timecode: float,
     text: str,
@@ -315,14 +345,15 @@
     """Replace the text of frame with timecode >= TIMECODE by TEXT."""
     scene = Scene.parse(input_file)
     scene.replace(timecode, text)
     scene.dump(output_file)
 
 
 @cli.command("include")
+@stdin_timeout_handler
 @click.argument("timecode", required=True, type=float)
 @click.argument("include_file", type=click.Path(exists=True), required=True)
 @input_option
 @output_option
 def include_cmd(
     timecode: float,
     include_file: str,
```

### Comparing `asciinema_scene-0.7.0/pyproject.toml` & `asciinema_scene-0.7.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asciinema_scene"
-version = "0.7.0"
+version = "0.7.1"
 description = "Toolbox to edit asciinema screencasts (sciine)."
 authors = ["Jerome Dumonteil <jerome.dumonteil@gmail.com>"]
 repository = "https://github.com/jdum/asciinema-scene"
 documentation = "https://jdum.github.io/asciinema-scene/"
 readme = "README.md"
 license = "MIT"
 classifiers = [
@@ -91,14 +91,16 @@
 ignore = [
     # LineTooLong
     "E501",
     # DoNotAssignLambda
     "E731",
     #Use specific rule codes when ignoring type issues
     "PGH003",
+    #check for execution of untrusted input
+    # "S603",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
 
 [tool.coverage.report]
 skip_empty = true
```

### Comparing `asciinema_scene-0.7.0/PKG-INFO` & `asciinema_scene-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asciinema-scene
-Version: 0.7.0
+Version: 0.7.1
 Summary: Toolbox to edit asciinema screencasts (sciine).
 Home-page: https://github.com/jdum/asciinema-scene
 License: MIT
 Author: Jerome Dumonteil
 Author-email: jerome.dumonteil@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 
 # asciinema-scene
 
 [![Release](https://img.shields.io/github/v/release/jdum/asciinema-scene)](https://img.shields.io/github/v/release/jdum/asciinema-scene)
 [![Build status](https://img.shields.io/github/actions/workflow/status/jdum/asciinema-scene/main.yml?branch=main)](https://github.com/jdum/asciinema-scene/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/jdum/asciinema-scene/branch/main/graph/badge.svg)](https://codecov.io/gh/jdum/asciinema-scene)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/jdum/asciinema-scene)](https://img.shields.io/github/commit-activity/m/jdum/asciinema-scene)
 [![License](https://img.shields.io/github/license/jdum/asciinema-scene)](https://img.shields.io/github/license/jdum/asciinema-scene)
 
 `asciinema-scene` provides the `sciine` command line toolkit for editing screen casts produced by [asciinema](https://asciinema.org/).
 
 `sciine` takes as input the content of a screencast, apply a unitary transformation and returns the transformed content.
```

