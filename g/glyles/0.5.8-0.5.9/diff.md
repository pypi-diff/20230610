# Comparing `tmp/glyles-0.5.8.tar.gz` & `tmp/glyles-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyles-0.5.8.tar", max compression
+gzip compressed data, was "glyles-0.5.9.tar", max compression
```

## Comparing `glyles-0.5.8.tar` & `glyles-0.5.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       94 2023-01-26 19:41:15.194122 glyles-0.5.8/glyles/__init__.py
--rw-r--r--   0        0        0     1893 2023-01-27 10:31:36.232845 glyles-0.5.8/glyles/__main__.py
--rw-r--r--   0        0        0     7921 2023-01-26 20:07:17.810800 glyles-0.5.8/glyles/converter.py
--rw-r--r--   0        0        0        0 2022-11-30 20:47:41.081113 glyles-0.5.8/glyles/glycans/__init__.py
--rw-r--r--   0        0        0        0 2022-11-30 20:47:41.081113 glyles-0.5.8/glyles/glycans/factory/__init__.py
--rw-r--r--   0        0        0     8413 2023-01-26 20:07:41.484261 glyles-0.5.8/glyles/glycans/factory/factory.py
--rw-r--r--   0        0        0    22814 2023-01-26 20:07:41.278730 glyles-0.5.8/glyles/glycans/factory/factory_f.py
--rw-r--r--   0        0        0    13292 2023-01-26 20:07:40.949333 glyles-0.5.8/glyles/glycans/factory/factory_o.py
--rw-r--r--   0        0        0    30663 2023-01-26 20:07:40.982639 glyles-0.5.8/glyles/glycans/factory/factory_p.py
--rw-r--r--   0        0        0        0 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/glycans/mono/__init__.py
--rw-r--r--   0        0        0     8118 2023-01-26 20:07:41.015621 glyles-0.5.8/glyles/glycans/mono/enum_c.py
--rw-r--r--   0        0        0    18487 2023-01-26 20:07:40.829881 glyles-0.5.8/glyles/glycans/mono/monomer.py
--rw-r--r--   0        0        0    29671 2023-01-26 20:07:41.529664 glyles-0.5.8/glyles/glycans/mono/reactor.py
--rw-r--r--   0        0        0     6588 2023-01-26 20:07:41.076913 glyles-0.5.8/glyles/glycans/mono/reactor_basic.py
--rw-r--r--   0        0        0        0 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/glycans/poly/__init__.py
--rw-r--r--   0        0        0    20088 2023-01-26 20:07:41.151373 glyles-0.5.8/glyles/glycans/poly/glycan.py
--rw-r--r--   0        0        0     5455 2023-01-26 20:07:41.449614 glyles-0.5.8/glyles/glycans/poly/merger.py
--rw-r--r--   0        0        0    31999 2023-01-03 10:06:24.945465 glyles-0.5.8/glyles/glycans/poly/viz.py
--rw-r--r--   0        0        0     7222 2023-01-26 20:07:41.043792 glyles-0.5.8/glyles/glycans/poly/walker.py
--rw-r--r--   0        0        0    20089 2023-01-03 10:06:24.946799 glyles-0.5.8/glyles/glycans/utils.py
--rw-r--r--   0        0        0        0 2022-11-30 20:47:41.096735 glyles-0.5.8/glyles/grammar/__init__.py
--rw-r--r--   0        0        0     2797 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/grammar/Glycan.g4
--rw-r--r--   0        0        0     7153 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/grammar/Glycan.interp
--rw-r--r--   0        0        0      183 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/grammar/Glycan.tokens
--rw-r--r--   0        0        0    27181 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/grammar/GlycanLexer.interp
--rw-r--r--   0        0        0    30774 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/grammar/GlycanLexer.py
--rw-r--r--   0        0        0      183 2022-11-30 21:30:50.116925 glyles-0.5.8/glyles/grammar/GlycanLexer.tokens
--rw-r--r--   0        0        0     1420 2022-11-30 20:47:41.096735 glyles-0.5.8/glyles/grammar/GlycanListener.py
--rw-r--r--   0        0        0    30702 2022-11-30 21:30:50.132719 glyles-0.5.8/glyles/grammar/GlycanParser.py
--rw-r--r--   0        0        0     1090 2022-11-30 20:47:41.050455 glyles-0.5.8/LICENSE
--rw-r--r--   0        0        0      878 2023-01-27 10:35:06.977850 glyles-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3869 2023-01-26 20:07:41.198420 glyles-0.5.8/README.md
--rw-r--r--   0        0        0     4924 2023-01-27 10:35:18.174029 glyles-0.5.8/setup.py
--rw-r--r--   0        0        0     4689 2023-01-27 10:35:18.174029 glyles-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-01-26 19:41:15.194122 glyles-0.5.9/glyles/__init__.py
+-rw-r--r--   0        0        0     1579 2023-01-27 11:51:08.211182 glyles-0.5.9/glyles/__main__.py
+-rw-r--r--   0        0        0     7921 2023-01-26 20:07:17.810800 glyles-0.5.9/glyles/converter.py
+-rw-r--r--   0        0        0        0 2022-11-30 20:47:41.081113 glyles-0.5.9/glyles/glycans/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-30 20:47:41.081113 glyles-0.5.9/glyles/glycans/factory/__init__.py
+-rw-r--r--   0        0        0     8413 2023-01-26 20:07:41.484261 glyles-0.5.9/glyles/glycans/factory/factory.py
+-rw-r--r--   0        0        0    22814 2023-01-26 20:07:41.278730 glyles-0.5.9/glyles/glycans/factory/factory_f.py
+-rw-r--r--   0        0        0    13292 2023-01-26 20:07:40.949333 glyles-0.5.9/glyles/glycans/factory/factory_o.py
+-rw-r--r--   0        0        0    30663 2023-01-26 20:07:40.982639 glyles-0.5.9/glyles/glycans/factory/factory_p.py
+-rw-r--r--   0        0        0        0 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/glycans/mono/__init__.py
+-rw-r--r--   0        0        0     8118 2023-01-26 20:07:41.015621 glyles-0.5.9/glyles/glycans/mono/enum_c.py
+-rw-r--r--   0        0        0    18487 2023-01-26 20:07:40.829881 glyles-0.5.9/glyles/glycans/mono/monomer.py
+-rw-r--r--   0        0        0    29671 2023-01-26 20:07:41.529664 glyles-0.5.9/glyles/glycans/mono/reactor.py
+-rw-r--r--   0        0        0     6588 2023-01-26 20:07:41.076913 glyles-0.5.9/glyles/glycans/mono/reactor_basic.py
+-rw-r--r--   0        0        0        0 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/glycans/poly/__init__.py
+-rw-r--r--   0        0        0    20088 2023-01-26 20:07:41.151373 glyles-0.5.9/glyles/glycans/poly/glycan.py
+-rw-r--r--   0        0        0     5455 2023-01-26 20:07:41.449614 glyles-0.5.9/glyles/glycans/poly/merger.py
+-rw-r--r--   0        0        0    31999 2023-01-03 10:06:24.945465 glyles-0.5.9/glyles/glycans/poly/viz.py
+-rw-r--r--   0        0        0     7222 2023-01-26 20:07:41.043792 glyles-0.5.9/glyles/glycans/poly/walker.py
+-rw-r--r--   0        0        0    20089 2023-01-03 10:06:24.946799 glyles-0.5.9/glyles/glycans/utils.py
+-rw-r--r--   0        0        0        0 2022-11-30 20:47:41.096735 glyles-0.5.9/glyles/grammar/__init__.py
+-rw-r--r--   0        0        0     2797 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/grammar/Glycan.g4
+-rw-r--r--   0        0        0     7153 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/grammar/Glycan.interp
+-rw-r--r--   0        0        0      183 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/grammar/Glycan.tokens
+-rw-r--r--   0        0        0    27181 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/grammar/GlycanLexer.interp
+-rw-r--r--   0        0        0    30774 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/grammar/GlycanLexer.py
+-rw-r--r--   0        0        0      183 2022-11-30 21:30:50.116925 glyles-0.5.9/glyles/grammar/GlycanLexer.tokens
+-rw-r--r--   0        0        0     1420 2022-11-30 20:47:41.096735 glyles-0.5.9/glyles/grammar/GlycanListener.py
+-rw-r--r--   0        0        0    30702 2022-11-30 21:30:50.132719 glyles-0.5.9/glyles/grammar/GlycanParser.py
+-rw-r--r--   0        0        0     1090 2022-11-30 20:47:41.050455 glyles-0.5.9/LICENSE
+-rw-r--r--   0        0        0      878 2023-01-27 11:39:11.013203 glyles-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3869 2023-01-26 20:07:41.198420 glyles-0.5.9/README.md
+-rw-r--r--   0        0        0     4924 2023-01-27 11:51:14.875304 glyles-0.5.9/setup.py
+-rw-r--r--   0        0        0     4689 2023-01-27 11:51:14.875304 glyles-0.5.9/PKG-INFO
```

### Comparing `glyles-0.5.8/glyles/__main__.py` & `glyles-0.5.9/glyles/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import os
 import sys
 import argparse
+import pkg_resources
 
-# SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-# sys.path.append(os.path.dirname(SCRIPT_DIR))
 
 from glyles import convert
 
 
 def main():
-    input_string_flag = False
-    input_list_flag = False
-    input_path_flag = False
-
     parser = argparse.ArgumentParser(
         prog="glyles",
         description="A tool to convert IUPAC representation of Glycans into SMILES representation"
     )
     parser.add_argument(
         '-i',
         '--input',
@@ -34,43 +29,32 @@
     )
     parser.add_argument(
         '--override',
         required=False,
         action="store_true",
         help="Override output file"
     )
-    # parser.add_argument("-h", "--help", action="help")
-    # parser.add_argument("-v", "--version", action="version")
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version=f"%(prog)s {pkg_resources.get_distribution('glyles').version}"
+    )
     args = parser.parse_args()
-
-    input = args.input
-    output = args.output
-
-    if len(input) == 1:
-        input = input[0]
-
-    if os.path.isfile(input):
-        input_path_flag = True
-    else:
-        if type(input) == list:
-            input_list_flag = True
-
-        elif type(input) == str:
-            input_string_flag = True
-
-    if os.path.isfile(output):
+    if os.path.isfile(args.output):
         if not args.override:
             print("Given output exist, please pick another name or use --override")
             sys.exit()
 
-    if input_string_flag:
-        convert(glycan=input, output_file=output)
-
-    elif input_list_flag:
-        convert(glycan_list=input, output_file=output)
+    if len(args.input) == 1:
+        args.input = args.input[0]
 
-    elif input_path_flag:
-        convert(glycan_file=input, output_file=output)
+    if isinstance(args.input, list):
+        convert(glycan_list=args.input, output_file=args.output)
+    elif os.path.isfile(args.input):
+        convert(glycan_file=args.input, output_file=args.output)
+    elif isinstance(args.input, str):
+        convert(glycan=args.input, output_file=args.output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `glyles-0.5.8/glyles/converter.py` & `glyles-0.5.9/glyles/converter.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/factory/factory.py` & `glyles-0.5.9/glyles/glycans/factory/factory.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/factory/factory_f.py` & `glyles-0.5.9/glyles/glycans/factory/factory_f.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/factory/factory_o.py` & `glyles-0.5.9/glyles/glycans/factory/factory_o.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/factory/factory_p.py` & `glyles-0.5.9/glyles/glycans/factory/factory_p.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/mono/enum_c.py` & `glyles-0.5.9/glyles/glycans/mono/enum_c.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/mono/monomer.py` & `glyles-0.5.9/glyles/glycans/mono/monomer.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/mono/reactor.py` & `glyles-0.5.9/glyles/glycans/mono/reactor.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/mono/reactor_basic.py` & `glyles-0.5.9/glyles/glycans/mono/reactor_basic.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/poly/glycan.py` & `glyles-0.5.9/glyles/glycans/poly/glycan.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/poly/merger.py` & `glyles-0.5.9/glyles/glycans/poly/merger.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/poly/viz.py` & `glyles-0.5.9/glyles/glycans/poly/viz.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/poly/walker.py` & `glyles-0.5.9/glyles/glycans/poly/walker.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/glycans/utils.py` & `glyles-0.5.9/glyles/glycans/utils.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/grammar/Glycan.g4` & `glyles-0.5.9/glyles/grammar/Glycan.g4`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/grammar/Glycan.interp` & `glyles-0.5.9/glyles/grammar/Glycan.interp`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/grammar/GlycanLexer.interp` & `glyles-0.5.9/glyles/grammar/GlycanLexer.interp`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/grammar/GlycanLexer.py` & `glyles-0.5.9/glyles/grammar/GlycanLexer.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/grammar/GlycanListener.py` & `glyles-0.5.9/glyles/grammar/GlycanListener.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/glyles/grammar/GlycanParser.py` & `glyles-0.5.9/glyles/grammar/GlycanParser.py`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/LICENSE` & `glyles-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/pyproject.toml` & `glyles-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glyles"
-version = "0.5.8"
+version = "0.5.9"
 repository = "https://github.com/kalininalab/GlyLES"
 readme = "README.md"
 description = "A tool to convert IUPAC representation of glycans into SMILES strings"
 authors = ["Roman Joeres <roman.joeres@helmholtz-hips.de>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent"
```

### Comparing `glyles-0.5.8/README.md` & `glyles-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `glyles-0.5.8/setup.py` & `glyles-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'rdkit-pypi>=2021.9.2,<2022.0.0']
 
 entry_points = \
 {'console_scripts': ['glyles = glyles.__main__:main']}
 
 setup_kwargs = {
     'name': 'glyles',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'A tool to convert IUPAC representation of glycans into SMILES strings',
     'long_description': '# GlyLES\n\n![testing](https://github.com/kalininalab/glyles/actions/workflows/test.yaml/badge.svg)\n![docs-image](https://readthedocs.org/projects/glyles/badge/?version=latest)\n![piwheels](https://img.shields.io/piwheels/v/glyles) \n![PyPI - Downloads](https://img.shields.io/pypi/dm/glyles) \n[![codecov](https://codecov.io/gh/kalininalab/GlyLES/branch/main/graph/badge.svg)](https://codecov.io/gh/kalininalab/glyles)\n[![DOI](https://zenodo.org/badge/431874597.svg)](https://zenodo.org/badge/latestdoi/431874597)\n\nA tool to convert IUPAC representation of Glycans into SMILES representation. This repo is still in the development \nphase; so, feel free to report any errors or issues. The code is available on \n[github](https://github.com/kalininalab/GlyLES/) and the documentation can be found on \n[ReadTheDocs](https://glyles.readthedocs.io/en/latest/index.html).\n\n## Specification and (current) Limitations\n\nThe exact specification we\'re referring to when talking about "IUPAC representations of glycan", is given in the \n"Notes" section of this [website](https://www.ncbi.nlm.nih.gov/glycans/snfg.html). But as this package is still in the \ndevelopment phase, not everything of the specification is implemented yet (especially not all side chains you can \nattach to monomers). The structure of the glycan can be represented as a tree of the monosaccharides with maximal \nbranching factor 4, i.e., each monomer in the glycan has at most 4 children.\n\n## Installation\n\nSo far, this package can only be downloaded from the python package index. So the installation with `pip` is very easy.\nJust type\n\n``````shell\npip install glyles\n``````\n\nand you\'re ready to use it as described below. Use \n\n``````shell\npip install --upgrade glyles\n``````\n\nto upgrade the glyles package to the most recent version.\n## Command Line Usage\n\n### With IUPAC input\n``````bash\n$ glyles -i Man(a1-2)Man -o ./test_output.txt\n``````\n\n### With IUPAC inputs\n``````bash\n$ glyles -i Man(a1-2)Man Fuc(a1-6)Glc -o ./test_output.txt\n``````\n\n### With file input\n``````bash\n$ glyles -i ./input_file.txt -o ./test_output.txt\n``````\n\n## Basic Usage\n\nConvert the IUPAC into a SMILES representation using the handy `convert` method\n\n``````python\nfrom glyles import convert\n\nconvert(glycan="Man(a1-2)Man", output_file="./test.txt")\n``````\n\nYou can also use the `convert_generator` method to get a generator for all SMILES:\n\n``````python\nfrom glyles import convert_generator\n\nfor smiles in convert_generator(glycan_list=["Man(a1-2)Man a", "Man(a1-2)Man b"]):\n    print(smiles)\n``````\n\nFor more examples of how to use this package, please see the notebooks in the \n[examples](https://github.com/kalininalab/GlyLES/tree/dev/examples) folder and checkout the documentation on \n[ReadTheDocs](https://glyles.readthedocs.io/en/latest/index.html).\n\n## Notation of glycans\n\nThere are multiple different notations for glycans in IUPAC. So, according to the \n[SNGF specification](https://www.ncbi.nlm.nih.gov/glycans/snfg.html), `Man(a1-4)Gal`, `Mana1-4Gal`, and `Mana4Gal` \nall describe the same disaccharide. This is also covered in this package as all three notations will be parsed into the \nsame tree of monosaccharides and result in the same SMILES string.\n\nThis is also described more detailed in a section on [ReadTheDocs]().\n\n## Poetry\n\nTo develop this package, we use the poetry package manager (see [here](https://python-poetry.org/) for detailed\ninstruction). It has basically the same functionality as conda but supports the package management better and also \nsupports distinguishing packages into those that are needed to use the package and those that are needed in the \ndevelopment of the package. To enable others to work on this repository, we also publish the exact \nspecifications of our poetry environment.\n',
     'author': 'Roman Joeres',
     'author_email': 'roman.joeres@helmholtz-hips.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kalininalab/GlyLES',
```

### Comparing `glyles-0.5.8/PKG-INFO` & `glyles-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyles
-Version: 0.5.8
+Version: 0.5.9
 Summary: A tool to convert IUPAC representation of glycans into SMILES strings
 Home-page: https://github.com/kalininalab/GlyLES
 Author: Roman Joeres
 Author-email: roman.joeres@helmholtz-hips.de
 Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

