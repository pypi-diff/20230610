# Comparing `tmp/pipen_runinfo-0.0.0.tar.gz` & `tmp/pipen_runinfo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_runinfo-0.0.0.tar", max compression
+gzip compressed data, was "pipen_runinfo-0.1.0.tar", max compression
```

## Comparing `pipen_runinfo-0.0.0.tar` & `pipen_runinfo-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2336 2023-06-09 22:24:46.232044 pipen_runinfo-0.0.0/README.md
--rw-r--r--   0        0        0     6073 2023-06-09 22:24:46.232044 pipen_runinfo-0.0.0/pipen_runinfo.py
--rw-r--r--   0        0        0     1057 2023-06-09 22:24:46.236044 pipen_runinfo-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 pipen_runinfo-0.0.0/setup.py
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 pipen_runinfo-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2755 2023-06-10 06:31:57.015234 pipen_runinfo-0.1.0/README.md
+-rw-r--r--   0        0        0     6586 2023-06-10 06:31:57.015234 pipen_runinfo-0.1.0/pipen_runinfo.py
+-rw-r--r--   0        0        0     1057 2023-06-10 06:31:57.015234 pipen_runinfo-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.0/setup.py
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.0/PKG-INFO
```

### Comparing `pipen_runinfo-0.0.0/README.md` & `pipen_runinfo-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,87 @@
 # pipen-runinfo
 
 Generate running information for jobs in [pipen][1] pipelines.
 
+Including session info (packages and versions), time, and device info.
+
 ## Install
 
 ```bash
 pip install -U pipen-runinfo
 ```
 
 ## Enable/Disable the plugin
 
 The plugin is registered via entrypoints. It's by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.
 
 ## Plugin options
 
-- `runinfo_lang`: The name of the language to run the job script.
+- `runinfo_lang`: The name of the language to run the job script for session info.
     Default is `None`, which means it will be inferred from the `proc.lang`
     This should be a process-level option, unless you only have one single
     process in your pipeline.
-- `runinfo_path`: Whether to include paths for the modules in the running information.
+- `runinfo_path`: Whether to include paths for the modules in the session information.
     Default is `True`.
     This option could be either specified in the process-level or the pipeline-level.
     Only works for `python`.
-- `runinfo_submod`: Whether to include submodules in the running information.
+- `runinfo_submod`: Whether to include submodules in the session information.
     Default is `False`.
     This option could be either specified in the process-level or the pipeline-level.
     Only works for `python`.
 
-## Supported languages
+## Supported languages for session info
 
 `python`, `R`, `bash`, and `fish`.
 
 ## Usage
 
-The plugin will generate a `job.runinfo` file in the job directory of the pipeline, which contains the running information of the job.
+The plugin will generate 3 files in the job directory of the pipeline.
+
+### `job.runinfo.session`
 
-### Python
+The session information of the job, including the interpreter, packages and their versions.
+
+#### Python
 
 Generates a TSV file with the following columns:
 
 - `Name`: The name of the module, or python itself
 - `__version__`: The version fetched by `module.__version__` or `module.version`
 - `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`
 - `Path`: The path of the module (only if `runinfo_path` is `True`)
 
-### R
+#### R
 
 Generates a text file `sessionInfo()` output.
 
-### Bash
+#### Bash
 
 Generates a TSV file with the following columns:
 
 - `SHELL`: The value of `$SHELL`
 - `BASH_VERSION`: The value of `$BASH_VERSION`
 - `BASH_ARGV0`: The value of `$BASH_ARGV0`
 - `BASH_SOURCE`: The value of `$BASH_SOURCE`
 - `proc-exe`: The real path of the executable from `/proc/<pid>/exe`
 - `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`
 
-### Fish
+#### Fish
 
 Generates a TSV file with the following columns:
 
 - `SHELL`: The value of `$SHELL`
 - `FISH_VERSION`: The value of `$FISH_VERSION`
 - `proc-exe`: The real path of the executable from `/proc/<pid>/exe`
 - `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`
 
+### `job.runinfo.time`
+
+The time spent on the job, and more, generated by `time -v` command.
+
+### `job.runinfo.device`
+
+The device information of the job, generated by `lshw` command.
+Note that only processor, memory, display and storage are included.
+
 
 [1]: https://github.com/pwwang/pipen
```

### Comparing `pipen_runinfo-0.0.0/pipen_runinfo.py` & `pipen_runinfo-0.1.0/pipen_runinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 from typing import TYPE_CHECKING, List
 from pathlib import Path
 
 from pipen import plugin
+from pipen.job import Job
 
 if TYPE_CHECKING:
     from pipen import Proc, Pipen
 
+__version__ = "0.1.0"
 
-__version__ = "0.0.0"
+# Monkey-path Job.CMD_WRAPPER_TEMPLATE to time the script
+Job.CMD_WRAPPER_TEMPLATE = Job.CMD_WRAPPER_TEMPLATE.replace(
+    "{job.strcmd}",
+    "/usr/bin/time -o {job.metadir}/job.runinfo.time -v {job.strcmd}",
+).replace(
+    "{postscript}",
+    "{postscript}\n\n"
+    "lshw -quiet -notime -sanitize -short -class processor -class memory "
+    "-class display -class storage 2>/dev/null "
+    "> {job.metadir}/job.runinfo.device"
+)
 
 
 SESSION_INFO_PYTHON = r"""
 def _session_info(show_path: bool, include_submodule: bool):
     try:
         from importlib import metadata as importlib_metadata
     except ImportError:
         import importlib_metadata
 
     import sys
-    runinfo_file = "{{job.metadir}}/job.runinfo"
+    runinfo_file = "{{job.metadir}}/job.runinfo.session"
 
     lines = ["# Generated by pipen_runinfo v%(version)s\n", "# Lang: python\n"]
     if show_path:
         lines.append("Name\t__version__\timportlib.metadata\tPath\n")
         lines.append(f"python\t{sys.version}\t-\t{sys.executable}\n")
     else:
         lines.append("Name\t__version__\timportlib.metadata\n")
@@ -60,31 +72,31 @@
 SESSION_INFO_R = r"""
 writeLines(
     c(
         "# Generated by pipen_runinfo v%(version)s",
         "# Lang: R",
         capture.output(sessionInfo())
     ),
-    "{{job.metadir}}/job.runinfo"
+    "{{job.metadir}}/job.runinfo.session"
 )
 """ % {"version": __version__}
 
 SESSION_INFO_FISH = r"""
-set -l runinfo_file "{{job.metadir}}/job.runinfo"
+set -l runinfo_file "{{job.metadir}}/job.runinfo.session"
 echo "# Generated by pipen_runinfo v%(version)s" > $runinfo_file
 echo "# Lang: fish" >> $runinfo_file
 echo -e "SHELL\t$SHELL" >> $runinfo_file
 echo -e "FISH_VERSION\t$FISH_VERSION" >> $runinfo_file
 set -l exe (readlink /proc/(echo %%self)/exe)
 echo -e "proc-exe\t$exe" >> $runinfo_file
 echo -e "proc-exe-verion\t$($exe --version)" 2>/dev/null >> $runinfo_file
 """ % {"version": __version__}
 
 SESSION_INFO_BASH = r"""
-runinfo_file="{{job.metadir}}/job.runinfo"
+runinfo_file="{{job.metadir}}/job.runinfo.session"
 echo "# Generated by pipen_runinfo v%(version)s" > $runinfo_file
 echo "# Lang: bash" >> $runinfo_file
 echo -e "SHELL\t$SHELL" >> $runinfo_file
 echo -e "BASH_VERSION\t$BASH_VERSION" >> $runinfo_file
 echo -e "BASH_ARGV0\t$BASH_ARGV0" >> $runinfo_file
 echo -e "BASH_SOURCE\t$BASH_SOURCE" >> $runinfo_file
 exe=$(readlink /proc/$$/exe)
@@ -93,15 +105,15 @@
 """ % {"version": __version__}
 
 
 def _get_lang(langpath: str | List[str]):
     if isinstance(langpath, list):
         langpath = langpath[0]
 
-    stem = Path(langpath).stem
+    stem = Path(langpath).stem if langpath else "bash"
     # Might be python3, python3.7, python3.7m, etc.
     if stem.startswith("python"):
         return "python"
 
     if (
         stem in ("Rscript", "R")
         or stem.startswith("Rscript")
```

### Comparing `pipen_runinfo-0.0.0/pyproject.toml` & `pipen_runinfo-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-runinfo"
-version = "0.0.0"
+version = "0.1.0"
 description = "Generate running information for jobs in pipen pipelines"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pipen_runinfo-0.0.0/setup.py` & `pipen_runinfo-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ['pipen>=0.10.1,<0.11.0']
 
 entry_points = \
 {'pipen': ['runinfo = pipen_runinfo:PipenRuninfoPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-runinfo',
-    'version': '0.0.0',
+    'version': '0.1.0',
     'description': 'Generate running information for jobs in pipen pipelines',
-    'long_description': '# pipen-runinfo\n\nGenerate running information for jobs in [pipen][1] pipelines.\n\n## Install\n\n```bash\npip install -U pipen-runinfo\n```\n\n## Enable/Disable the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.\n\n## Plugin options\n\n- `runinfo_lang`: The name of the language to run the job script.\n    Default is `None`, which means it will be inferred from the `proc.lang`\n    This should be a process-level option, unless you only have one single\n    process in your pipeline.\n- `runinfo_path`: Whether to include paths for the modules in the running information.\n    Default is `True`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n- `runinfo_submod`: Whether to include submodules in the running information.\n    Default is `False`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n\n## Supported languages\n\n`python`, `R`, `bash`, and `fish`.\n\n## Usage\n\nThe plugin will generate a `job.runinfo` file in the job directory of the pipeline, which contains the running information of the job.\n\n### Python\n\nGenerates a TSV file with the following columns:\n\n- `Name`: The name of the module, or python itself\n- `__version__`: The version fetched by `module.__version__` or `module.version`\n- `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`\n- `Path`: The path of the module (only if `runinfo_path` is `True`)\n\n### R\n\nGenerates a text file `sessionInfo()` output.\n\n### Bash\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `BASH_VERSION`: The value of `$BASH_VERSION`\n- `BASH_ARGV0`: The value of `$BASH_ARGV0`\n- `BASH_SOURCE`: The value of `$BASH_SOURCE`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n### Fish\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `FISH_VERSION`: The value of `$FISH_VERSION`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-runinfo\n\nGenerate running information for jobs in [pipen][1] pipelines.\n\nIncluding session info (packages and versions), time, and device info.\n\n## Install\n\n```bash\npip install -U pipen-runinfo\n```\n\n## Enable/Disable the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.\n\n## Plugin options\n\n- `runinfo_lang`: The name of the language to run the job script for session info.\n    Default is `None`, which means it will be inferred from the `proc.lang`\n    This should be a process-level option, unless you only have one single\n    process in your pipeline.\n- `runinfo_path`: Whether to include paths for the modules in the session information.\n    Default is `True`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n- `runinfo_submod`: Whether to include submodules in the session information.\n    Default is `False`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n\n## Supported languages for session info\n\n`python`, `R`, `bash`, and `fish`.\n\n## Usage\n\nThe plugin will generate 3 files in the job directory of the pipeline.\n\n### `job.runinfo.session`\n\nThe session information of the job, including the interpreter, packages and their versions.\n\n#### Python\n\nGenerates a TSV file with the following columns:\n\n- `Name`: The name of the module, or python itself\n- `__version__`: The version fetched by `module.__version__` or `module.version`\n- `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`\n- `Path`: The path of the module (only if `runinfo_path` is `True`)\n\n#### R\n\nGenerates a text file `sessionInfo()` output.\n\n#### Bash\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `BASH_VERSION`: The value of `$BASH_VERSION`\n- `BASH_ARGV0`: The value of `$BASH_ARGV0`\n- `BASH_SOURCE`: The value of `$BASH_SOURCE`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n#### Fish\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `FISH_VERSION`: The value of `$FISH_VERSION`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n### `job.runinfo.time`\n\nThe time spent on the job, and more, generated by `time -v` command.\n\n### `job.runinfo.device`\n\nThe device information of the job, generated by `lshw` command.\nNote that only processor, memory, display and storage are included.\n\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `pipen_runinfo-0.0.0/PKG-INFO` & `pipen_runinfo-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-runinfo
-Version: 0.0.0
+Version: 0.1.0
 Summary: Generate running information for jobs in pipen pipelines
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,76 +15,91 @@
 Requires-Dist: pipen (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # pipen-runinfo
 
 Generate running information for jobs in [pipen][1] pipelines.
 
+Including session info (packages and versions), time, and device info.
+
 ## Install
 
 ```bash
 pip install -U pipen-runinfo
 ```
 
 ## Enable/Disable the plugin
 
 The plugin is registered via entrypoints. It's by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.
 
 ## Plugin options
 
-- `runinfo_lang`: The name of the language to run the job script.
+- `runinfo_lang`: The name of the language to run the job script for session info.
     Default is `None`, which means it will be inferred from the `proc.lang`
     This should be a process-level option, unless you only have one single
     process in your pipeline.
-- `runinfo_path`: Whether to include paths for the modules in the running information.
+- `runinfo_path`: Whether to include paths for the modules in the session information.
     Default is `True`.
     This option could be either specified in the process-level or the pipeline-level.
     Only works for `python`.
-- `runinfo_submod`: Whether to include submodules in the running information.
+- `runinfo_submod`: Whether to include submodules in the session information.
     Default is `False`.
     This option could be either specified in the process-level or the pipeline-level.
     Only works for `python`.
 
-## Supported languages
+## Supported languages for session info
 
 `python`, `R`, `bash`, and `fish`.
 
 ## Usage
 
-The plugin will generate a `job.runinfo` file in the job directory of the pipeline, which contains the running information of the job.
+The plugin will generate 3 files in the job directory of the pipeline.
+
+### `job.runinfo.session`
 
-### Python
+The session information of the job, including the interpreter, packages and their versions.
+
+#### Python
 
 Generates a TSV file with the following columns:
 
 - `Name`: The name of the module, or python itself
 - `__version__`: The version fetched by `module.__version__` or `module.version`
 - `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`
 - `Path`: The path of the module (only if `runinfo_path` is `True`)
 
-### R
+#### R
 
 Generates a text file `sessionInfo()` output.
 
-### Bash
+#### Bash
 
 Generates a TSV file with the following columns:
 
 - `SHELL`: The value of `$SHELL`
 - `BASH_VERSION`: The value of `$BASH_VERSION`
 - `BASH_ARGV0`: The value of `$BASH_ARGV0`
 - `BASH_SOURCE`: The value of `$BASH_SOURCE`
 - `proc-exe`: The real path of the executable from `/proc/<pid>/exe`
 - `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`
 
-### Fish
+#### Fish
 
 Generates a TSV file with the following columns:
 
 - `SHELL`: The value of `$SHELL`
 - `FISH_VERSION`: The value of `$FISH_VERSION`
 - `proc-exe`: The real path of the executable from `/proc/<pid>/exe`
 - `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`
 
+### `job.runinfo.time`
+
+The time spent on the job, and more, generated by `time -v` command.
+
+### `job.runinfo.device`
+
+The device information of the job, generated by `lshw` command.
+Note that only processor, memory, display and storage are included.
+
 
 [1]: https://github.com/pwwang/pipen
```

