# Comparing `tmp/hilbert_prop_logic-0.1.0.tar.gz` & `tmp/hilbert_prop_logic-0.1.1.tar.gz`

## Comparing `hilbert_prop_logic-0.1.0.tar` & `hilbert_prop_logic-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 hilbert_prop_logic-0.1.0/Cargo.toml
--rw-r--r--   0      502       20      380 2023-06-09 20:06:53.000000 hilbert_prop_logic-0.1.0/pyproject.toml
--rw-r--r--   0      502       20    44086 2023-06-09 20:06:50.000000 hilbert_prop_logic-0.1.0/src/lib.rs
--rw-r--r--   0      502       20     8804 2023-06-09 20:06:55.000000 hilbert_prop_logic-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 hilbert_prop_logic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 hilbert_prop_logic-0.1.1/Cargo.toml
+-rw-r--r--   0      502       20      379 2023-06-10 00:59:12.000000 hilbert_prop_logic-0.1.1/pyproject.toml
+-rw-r--r--   0      502       20    44031 2023-06-10 17:07:48.000000 hilbert_prop_logic-0.1.1/src/lib.rs
+-rw-r--r--   0      502       20     8804 2023-06-10 17:41:10.000000 hilbert_prop_logic-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 hilbert_prop_logic-0.1.1/PKG-INFO
```

### Comparing `hilbert_prop_logic-0.1.0/src/lib.rs` & `hilbert_prop_logic-0.1.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,40 +4,16 @@
 use std::collections::{HashSet, HashMap};
 use std::hash::Hash;
 use rand::prelude::*;
 use rand::rngs::StdRng;
 
 static NUM_ATOMS: usize = 26;
 static ATOMS: [char; 26] = [
-    'A',
-    'B',
-    'C',
-    'D',
-    'E',
-    'F',
-    'G',
-    'H',
-    'I',
-    'J',
-    'K',
-    'L',
-    'M',
-    'N',
-    'O',
-    'P',
-    'Q',
-    'R',
-    'S',
-    'T',
-    'U',
-    'V',
-    'W',
-    'X',
-    'Y',
-    'Z'
+    'A','B','C','D','E','F','G','H','I','J','K','L','M',
+    'N','O','P','Q','R','S','T','U','V','W','X','Y','Z'
 ];
 
 // static ID: fn(PropFormula) -> PropFormula = |f: PropFormula| f;
 
 #[derive(Debug, Clone)]
 pub enum SymbolParseError {
     InvalidChar(char),
@@ -52,14 +28,15 @@
         }
     }
 }
 
 impl std::error::Error for SymbolParseError {}
 
 
+
 #[derive(Debug)]
 pub enum ValidationError {
     Binary(BinaryOp),
     Unary(UnaryOp),
     Atom(char),
     Parentheses,
     EmptyFormula,
@@ -747,14 +724,15 @@
 
 /// A Python-facing interface for PropFormula.
 #[pymethods]
 impl PropFormula {
     /// Python initializer. Either initialize a random from a passed in set or an atom from
     /// passed in str atom: ONLY THE FIRST CHARACTER of atom will be used!
     #[new]
+    #[pyo3(signature = (random=false, atom=None, atoms=None))]
     pub fn new_atom(random: bool, atom: Option<&str>, atoms: Option<HashSet<char>>) -> PyResult<Self> {
         if random {
             if let Some(set) = atoms {
                 if let Some(c) = set.iter().choose(&mut thread_rng()) {
                     Ok(PropFormula::new(*c))
                 } else {Err(PyValueError::new_err("set of atoms must be non-empty!"))}
             } else {
@@ -1078,8 +1056,8 @@
 
 
 /// A Python logic module implemented in Rust.
 #[pymodule]
 fn hilbert_prop_logic(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<PropFormula>()?;
     Ok(())
-}
+}
```

### Comparing `hilbert_prop_logic-0.1.0/Cargo.lock` & `hilbert_prop_logic-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hilbert_prop_logic"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "rand",
 ]
 
 [[package]]
 name = "indoc"
```

