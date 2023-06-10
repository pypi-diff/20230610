# Comparing `tmp/untypedscript-utsc-1.0.1.tar.gz` & `tmp/untypedscript-utsc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untypedscript-utsc-1.0.1.tar", last modified: Fri Jun  9 20:38:11 2023, max compression
+gzip compressed data, was "untypedscript-utsc-1.0.2.tar", last modified: Sat Jun 10 00:07:25 2023, max compression
```

## Comparing `untypedscript-utsc-1.0.1.tar` & `untypedscript-utsc-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.239304 untypedscript-utsc-1.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       49 2023-06-09 20:08:40.000000 untypedscript-utsc-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6644 2023-06-09 20:38:11.237799 untypedscript-utsc-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-1.0.1/README.md
--rw-rw-rw-   0        0        0      648 2023-06-09 20:37:51.000000 untypedscript-utsc-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 20:38:11.240313 untypedscript-utsc-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.110283 untypedscript-utsc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.145777 untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/
--rw-rw-rw-   0        0        0     6644 2023-06-09 20:38:11.000000 untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-06-09 20:38:11.000000 untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:38:11.000000 untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-09 20:38:11.000000 untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 20:38:11.000000 untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.107264 untypedscript-utsc-1.0.1/src/uts-lib/
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.155751 untypedscript-utsc-1.0.1/src/uts-lib/typed/
--rw-rw-rw-   0        0        0     2521 2023-06-04 21:46:35.000000 untypedscript-utsc-1.0.1/src/uts-lib/typed/io.uts
--rw-rw-rw-   0        0        0      215 2023-05-01 19:54:36.000000 untypedscript-utsc-1.0.1/src/uts-lib/typed/typed-value.uts
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.171754 untypedscript-utsc-1.0.1/src/uts-lib/utils/
--rw-rw-rw-   0        0        0      457 2023-04-26 20:34:59.000000 untypedscript-utsc-1.0.1/src/uts-lib/utils/math.uts
--rw-rw-rw-   0        0        0     2225 2023-06-04 21:32:06.000000 untypedscript-utsc-1.0.1/src/uts-lib/utils/obj.uts
--rw-rw-rw-   0        0        0      183 2023-04-10 00:56:50.000000 untypedscript-utsc-1.0.1/src/uts-lib/utils/uts-array.uts
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.187002 untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/
--rw-rw-rw-   0        0        0      812 2023-04-27 12:38:42.000000 untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/async.uts
--rw-rw-rw-   0        0        0     1629 2023-06-09 00:35:56.000000 untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/heapfuncs-nouse.uts
--rw-rw-rw-   0        0        0     2318 2023-06-09 00:39:22.000000 untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/libheapfunc.o
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.190535 untypedscript-utsc-1.0.1/src/uts-lib/uts/
--rw-rw-rw-   0        0        0       74 2023-06-04 16:59:55.000000 untypedscript-utsc-1.0.1/src/uts-lib/uts/info.uts
-drwxrwxrwx   0        0        0        0 2023-06-09 20:38:11.233045 untypedscript-utsc-1.0.1/src/utsc/
--rw-rw-rw-   0        0        0     9314 2023-06-09 20:37:16.000000 untypedscript-utsc-1.0.1/src/utsc/__init__.py
--rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-1.0.1/src/utsc/ast_cleaner.py
--rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-1.0.1/src/utsc/ast_preprocessor.py
--rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-1.0.1/src/utsc/code_lowerer.py
--rw-rw-rw-   0        0        0    36176 2023-06-09 20:31:27.000000 untypedscript-utsc-1.0.1/src/utsc/compiler.py
--rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-1.0.1/src/utsc/optimizer.py
--rw-rw-rw-   0        0        0     7829 2023-06-09 18:44:10.000000 untypedscript-utsc-1.0.1/src/utsc/sequential_lexer.py
--rw-rw-rw-   0        0        0     4817 2023-06-09 19:19:00.000000 untypedscript-utsc-1.0.1/src/utsc/utils.py
--rw-rw-rw-   0        0        0    39560 2023-06-09 18:44:01.000000 untypedscript-utsc-1.0.1/src/utsc/uts_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.175654 untypedscript-utsc-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       49 2023-06-09 20:08:40.000000 untypedscript-utsc-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6644 2023-06-10 00:07:25.173651 untypedscript-utsc-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-1.0.2/README.md
+-rw-rw-rw-   0        0        0      648 2023-06-10 00:07:12.000000 untypedscript-utsc-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 00:07:25.175654 untypedscript-utsc-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.052555 untypedscript-utsc-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.081062 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/
+-rw-rw-rw-   0        0        0     6644 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.051547 untypedscript-utsc-1.0.2/src/uts-lib/
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.087050 untypedscript-utsc-1.0.2/src/uts-lib/typed/
+-rw-rw-rw-   0        0        0     2521 2023-06-04 21:46:35.000000 untypedscript-utsc-1.0.2/src/uts-lib/typed/io.uts
+-rw-rw-rw-   0        0        0      215 2023-05-01 19:54:36.000000 untypedscript-utsc-1.0.2/src/uts-lib/typed/typed-value.uts
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.094617 untypedscript-utsc-1.0.2/src/uts-lib/utils/
+-rw-rw-rw-   0        0        0      457 2023-04-26 20:34:59.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/math.uts
+-rw-rw-rw-   0        0        0     2225 2023-06-04 21:32:06.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/obj.uts
+-rw-rw-rw-   0        0        0      183 2023-04-10 00:56:50.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/uts-array.uts
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.115335 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/
+-rw-rw-rw-   0        0        0      812 2023-04-27 12:38:42.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/async.uts
+-rw-rw-rw-   0        0        0     1629 2023-06-09 00:35:56.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/heapfuncs-nouse.uts
+-rw-rw-rw-   0        0        0     2318 2023-06-09 00:39:22.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/libheapfunc.o
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.132085 untypedscript-utsc-1.0.2/src/uts-lib/uts/
+-rw-rw-rw-   0        0        0       74 2023-06-04 16:59:55.000000 untypedscript-utsc-1.0.2/src/uts-lib/uts/info.uts
+drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.169647 untypedscript-utsc-1.0.2/src/utsc/
+-rw-rw-rw-   0        0        0     9297 2023-06-09 20:40:43.000000 untypedscript-utsc-1.0.2/src/utsc/__init__.py
+-rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-1.0.2/src/utsc/ast_cleaner.py
+-rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-1.0.2/src/utsc/ast_preprocessor.py
+-rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-1.0.2/src/utsc/code_lowerer.py
+-rw-rw-rw-   0        0        0    36382 2023-06-10 00:00:01.000000 untypedscript-utsc-1.0.2/src/utsc/compiler.py
+-rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-1.0.2/src/utsc/optimizer.py
+-rw-rw-rw-   0        0        0     7847 2023-06-10 00:03:58.000000 untypedscript-utsc-1.0.2/src/utsc/sequential_lexer.py
+-rw-rw-rw-   0        0        0     4876 2023-06-09 23:46:49.000000 untypedscript-utsc-1.0.2/src/utsc/utils.py
+-rw-rw-rw-   0        0        0    39976 2023-06-10 00:02:48.000000 untypedscript-utsc-1.0.2/src/utsc/uts_parser.py
```

### Comparing `untypedscript-utsc-1.0.1/LICENSE` & `untypedscript-utsc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/PKG-INFO` & `untypedscript-utsc-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 1.0.1
+Version: 1.0.2
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `untypedscript-utsc-1.0.1/README.md` & `untypedscript-utsc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/pyproject.toml` & `untypedscript-utsc-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "untypedscript-utsc"
-version = "1.0.1"
+version = "1.0.2"
 description = "UntypedScript original implementation compiler"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = []
 keywords = []
 dependencies = []
```

### Comparing `untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/PKG-INFO` & `untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 1.0.1
+Version: 1.0.2
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `untypedscript-utsc-1.0.1/src/untypedscript_utsc.egg-info/SOURCES.txt` & `untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/uts-lib/typed/io.uts` & `untypedscript-utsc-1.0.2/src/uts-lib/typed/io.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/uts-lib/utils/obj.uts` & `untypedscript-utsc-1.0.2/src/uts-lib/utils/obj.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/async.uts` & `untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/async.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/heapfuncs-nouse.uts` & `untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/heapfuncs-nouse.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/uts-lib/utils/win32/libheapfunc.o` & `untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/libheapfunc.o`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/utsc/__init__.py` & `untypedscript-utsc-1.0.2/src/utsc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 	argparser.add_argument("-s", "--suppresswarnings", help="suppress all warnings", action="store_true", default=False)
 	argparser.add_argument("filename", nargs='?', default='', type=str, help='Source file')
 	argparser.add_argument("-f", "--fmt", type=str, default="win32", help="format to compile to")
 	argparser.add_argument("-O", "--optimization", type=int, default=0, help="Optimization level to apply. Can be 0 (default), 1, or 2")
 	argparser.add_argument("-m", "--module", action="store_true", help="Compile this file without linking object files")
 	outgroup = argparser.add_mutually_exclusive_group()
 	outgroup.add_argument("-o", "--out", type=str, help="output filename")
-	outgroup.add_argument("-e", "--executable", help="run assemble.ps1 and produce an executable using NASM and MinGW", action="store_true")
+	outgroup.add_argument("-e", "--executable", help="produce an executable using NASM and MinGW/gcc", action="store_true")
 	outgroup.add_argument("-r", "--run", help="Run the uts program and exit", action="store_true")
 	
 	args = argparser.parse_args()
 	
 	warnings = not args.suppresswarnings
 	executable = args.executable
 	runfile = args.run
```

### Comparing `untypedscript-utsc-1.0.1/src/utsc/ast_cleaner.py` & `untypedscript-utsc-1.0.2/src/utsc/ast_cleaner.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/utsc/ast_preprocessor.py` & `untypedscript-utsc-1.0.2/src/utsc/ast_preprocessor.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/utsc/code_lowerer.py` & `untypedscript-utsc-1.0.2/src/utsc/code_lowerer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/utsc/compiler.py` & `untypedscript-utsc-1.0.2/src/utsc/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,19 @@
 
 		self.symbols.declare(name, _type, 4, f"_{name}")
 		self.symbols.assign(name, value, index)
 
 		if value.get("Anonymous Function") is not None:
 			value = value["Anonymous Function"]
 
+			if value["type"] != "normal":
+				code = get_code(self.source, value["index"])
+
+				warn(f"UTSC 314: tried to create {value['type']} function in global scope, defaulting to normal function", code)
+
 			func_compiler = FunctionCompiler(
 				value["parameters"],
 				value["body"],
 				self.source,
 				self
 			)
```

### Comparing `untypedscript-utsc-1.0.1/src/utsc/optimizer.py` & `untypedscript-utsc-1.0.2/src/utsc/optimizer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.1/src/utsc/sequential_lexer.py` & `untypedscript-utsc-1.0.2/src/utsc/sequential_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,20 +297,22 @@
 				try: char = self.code[self.i]
 				except IndexError:
 					return "line"
 
 			return "line"
 		
 		if char == '*':
+			start = self.i
+
 			while 1:
 				self.i+=1
 
 				try: char = self.code[self.i]
 				except IndexError:
-					code = get_code(self.code, self.i-2)
+					code = get_code(self.code, start)
 
 					throw("UTSC 102: Block comment was not closed - terminating tokenization", code)
 					raise SigTermTokenization()
 				
 				if (char == '*') and (self.i+1 < self.num_chars) and (self.code[self.i+1] == '/'):
 					self.i+=1
 					return "block"
```

### Comparing `untypedscript-utsc-1.0.1/src/utsc/utils.py` & `untypedscript-utsc-1.0.2/src/utsc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,33 +37,32 @@
 			code+="\t"
 		else:
 			code+=" "
 
 		if i == idx:
 			break
 
-	linenolen = len(lineno)+1
+	linenolen = len(lineno)-1
 	code+=(" "*linenolen)+"^^^\n"
 	return code
 
-def strgetline(string: str, index: int):
+def strgetline(string: str, target_index: int):
 	current_idx = 0
+
 	for i, line in enumerate(string.splitlines()):
-		for j in range(0, len(line)-1):
-			if current_idx == index:
-				return [line, j, i+1]
-			current_idx+=1
+		for j in range(len(line)):
+			if current_idx == target_index: return [line, j, i+1]
 
-		current_idx+=1
+			current_idx+=1
 
+		if current_idx == target_index: return [line, len(line)-1, i+1]
 
-		if current_idx == index:
-			return [line, j+1, i+1]
+		current_idx+=1
 
-	return ["", 0, 0]
+	return ["<<<untypedscript: could not locate code>>>", 0, 0]
 #
 
 
 #Error throwing functions
 def throw(message, code=""):
 	global errors
 	global thrown
```

### Comparing `untypedscript-utsc-1.0.1/src/utsc/uts_parser.py` & `untypedscript-utsc-1.0.2/src/utsc/uts_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 		self.value = value
 
 	def __repr__(self):
 		return f'{{ "String Literal": {dumps(self.value)}  }}'
 
 class BinOpNode(Node):
 	def __init__(self, left: Node, op: str, right: Node):
-		self.left = left
+		self.left = left if left else "null"
 		self.value = op
-		self.right = right
+		self.right = right if right else "null"
 
 	def __repr__(self):
 		return f'{{ "Binary Operation {self.value}" : [{self.left}, {self.right}] }}'
 
 class UnaryOpNode(Node):
 	def __init__(self, op: str, node: Node):
 		self.op = op
@@ -168,32 +168,33 @@
 		return '{ "Unimplemented Node" : null }'
 
 class AnonymousFunctionNode(Node):
 	NORMAL = "normal"
 	LOCALLY_EXPOSED = "localonly"
 	HEAP_ALLOCATED = "heapalloced"
 
-	def __init__(self, params: dict[str, str], body: dict, flag: str=NORMAL):
+	def __init__(self, params: dict[str, str], body: dict, idx: int, flag: str=NORMAL):
 		self.params = dumps(params)
 		
 		try:
 			if tuple(body.values())[-1].get("Return Statement") is None:
 				body["Expression_CompilerAddedDefaultReturn"] = loads(str(FunctionReturnStatement(None)))
 		except IndexError: body["Expression_CompilerAddedDefaultReturn"] = loads(str(FunctionReturnStatement(None)))
 # this is an empty func
 
 		self.body = dumps(body)
 		self.flag = flag
+		self.idx = idx
 	
 	def __repr__(self):
 		if self.flag == AnonymousFunctionNode.HEAP_ALLOCATED:
 			# obviously change these later and take platform into account when using these win32 functions (use mmap instead)
-			return f'{{ "Verify-Imported0": ["HeapFuncAlloc", "heap-allocated functions"], "Verify-Imported1": ["HeapFuncProtect", "heap-allocated functions"], "Verify-Imported1": ["HeapFuncFree", "heap-allocated functions"], "Verify-Imported2": ["memcpy", "heap-allocated functions"], "Anonymous Function" : {{ "parameters" : {self.params}, "body" : {self.body}, "type": "{self.flag}" }} }}'
+			return f'{{ "Verify-Imported0": ["HeapFuncAlloc", "heap-allocated functions"], "Verify-Imported1": ["HeapFuncProtect", "heap-allocated functions"], "Verify-Imported1": ["HeapFuncFree", "heap-allocated functions"], "Verify-Imported2": ["memcpy", "heap-allocated functions"], "Anonymous Function" : {{ "parameters" : {self.params}, "body" : {self.body}, "type": "{self.flag}", "index": {self.idx} }} }}'
 		
-		return f'{{"Anonymous Function" : {{ "parameters" : {self.params}, "body" : {self.body}, "type": "{self.flag}" }} }}'
+		return f'{{"Anonymous Function" : {{ "parameters" : {self.params}, "body" : {self.body}, "type": "{self.flag}", "index": {self.idx} }} }}'
 
 class NamespaceDeclarationNode(Node):
 	def __init__(self, name: str, body: dict):
 		self.body = dumps(body)
 		self.name = name
 	
 	def __repr__(self):
@@ -555,14 +556,20 @@
 			op = self.current.value
 			self.advance()
 
 			if self.in_paren: self.skip_newlines()
 
 			right = func_b()
 			
+			if right is None: # must be a newline, backtrack one to get the right line
+				code = get_code(self.code, self.current.idx-1)
+
+				throw("UTSC 203: Expected expression, got <newline>", code)
+
+			
 			left = BinOpNode(left, op, right)		
 		
 		return left
 
 	def fallback_paren_expr(self, fallback_idx: int): # Function to call if arrow function parsing fails
 		self.in_paren.append(None)
 
@@ -700,54 +707,56 @@
 	def atom(self):
 		if self.in_paren: self.skip_newlines()
 
 		current = self.current
 
 		if current.type == "IDENTIFIER":
 			self.advance()
+
+			index = self.current.idx
 			
 			if self.current.value == '=': # this needs to be in expr()
 				self.advance()
 				expr = self.comp_expr()
 				if expr is None:
 					self.decrement()
 
 					code = get_code(self.code, self.current.idx)
 					
 					throw(f"UTSC 203: Expected expression after assignment operator '=', got {fmt_type(Token(self.tokens[self.idx+1]).type)}", code)
 					
 					self.advance()
 					return UnimplementedNode()
 				else:
-					return VariableAssignmentNode(current.value, expr, self.current.idx)
+					return VariableAssignmentNode(current.value, expr, index)
 			if self.current.value in ('+', '-', '/', '*'): # += -= *= /= assignment
 				op = self.current.value
 				self.advance()
 				
 				if self.current.value == '=':
 					self.advance()
 					expr = self.comp_expr()
 					if expr is None:
 						self.decrement()
 
 						code = get_code(self.code, self.current.idx)
 						
-						throw(f"UTSC 203: Expected expression after assignment operator '{op.value}=', got {fmt_type(Token(self.tokens[self.idx+1]).type)}", code)
+						throw(f"UTSC 203: Expected expression after assignment operator '{op}=', got {fmt_type(Token(self.tokens[self.idx+1]).type)}", code)
 						
 						self.advance()
 						return UnimplementedNode()
 					else:
 						return VariableAssignmentNode( # Lowered AST for +=, -=, etc.
 							current.value,
 							BinOpNode(
 								VariableAccessNode(current),
 								op,
 								expr
 							),
-							self.current.idx
+							index
 						)
 
 				self.decrement() # back up to operator token
 
 			return VariableAccessNode(current)
 
 		if current.type in ("INTEGER", "FLOAT"):
@@ -793,14 +802,16 @@
 		if current.value == '{':
 			self.advance()
 			return self.obj_expr()
 
 		if current.value == '(':
 			self.advance()
 
+			index = self.current.idx+1 # make this past the opening arg brace
+
 			if (self.current.type in ("IDENTIFIER", "STRUCT")) or (self.current.value == ')'):
 				fallback_idx = self.current.idx
 				vartype = ""
 				parameters: dict[str, str] = {}
 
 				while self.current.value != ')':
 					vartype = "LET"
@@ -859,15 +870,15 @@
 						self.advance()
 						return UnimplementedNode()
 
 					func_body = {
 						f"Return Statement": loads(str(expr))
 					}
 
-				return AnonymousFunctionNode(parameters, func_body)
+				return AnonymousFunctionNode(parameters, func_body, index)
 
 			else:
 				return self.fallback_paren_expr(self.current.idx)
 		if current.type == "NEWLINE":
 			self.advance()
 			return None
 		
@@ -1242,14 +1253,15 @@
 				
 				throw(f"UTSC 203: Expected identifier after '{vartype.lower()}', got {fmt_type(Token(self.tokens[self.idx+1]).type)}", code)
 				
 				self.advance()
 				return UnimplementedNode()
 
 			name = self.current.value
+			index = self.current.idx
 			self.advance()
 
 			if self.current.type == "NEWLINE":
 				if vartype == "CONST":
 					self.decrement()
 
 					code = get_code(self.code, self.current.idx)
@@ -1271,15 +1283,15 @@
 					code = get_code(self.code, self.current.idx)
 					
 					throw(f"UTSC 203: Expected expression after assignment operator '=', got {fmt_type(Token(self.tokens[self.idx+1]).type)}", code)
 					
 					self.advance()
 					return UnimplementedNode()
 				else:
-					return VariableDefinitionNode(vartype, name, expr, self.current.idx)
+					return VariableDefinitionNode(vartype, name, expr, index)
 			else:
 				code = get_code(self.code, self.current.idx)
 				
 				throw(f"UTSC 203: Expected '=' or <newline>, got {fmt_type(Token(self.tokens[self.idx+1]).type)}", code)
 				
 				self.advance()
 				return UnimplementedNode()
```

