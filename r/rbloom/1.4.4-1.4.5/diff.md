# Comparing `tmp/rbloom-1.4.4.tar.gz` & `tmp/rbloom-1.4.5.tar.gz`

## Comparing `rbloom-1.4.4.tar` & `rbloom-1.4.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 rbloom-1.4.4/Cargo.toml
--rw-r--r--   0     1001      123     1665 2023-02-16 18:55:35.000000 rbloom-1.4.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      699 2023-02-16 18:55:35.000000 rbloom-1.4.4/.gitignore
--rw-r--r--   0     1001      123     1069 2023-02-16 18:55:35.000000 rbloom-1.4.4/LICENSE
--rw-r--r--   0     1001      123    11468 2023-02-16 18:55:35.000000 rbloom-1.4.4/README.md
--rw-r--r--   0     1001      123      533 2023-02-16 18:55:35.000000 rbloom-1.4.4/pyproject.toml
--rw-r--r--   0     1001      123     2843 2023-02-16 18:55:35.000000 rbloom-1.4.4/rbloom.pyi
--rwxr-xr-x   0     1001      123      984 2023-02-16 18:56:05.000000 rbloom-1.4.4/run-maturin-action.sh
--rw-r--r--   0     1001      123    17688 2023-02-16 18:55:35.000000 rbloom-1.4.4/src/lib.rs
--rwxr-xr-x   0     1001      123     2681 2023-02-16 18:55:35.000000 rbloom-1.4.4/tests/api_test.py
--rw-r--r--   0        0        0     7650 2023-02-16 18:57:45.000000 rbloom-1.4.4/Cargo.lock
--rw-r--r--   0        0        0    11962 1970-01-01 00:00:00.000000 rbloom-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 rbloom-1.4.5/Cargo.toml
+-rw-r--r--   0     1001      123     1665 2023-06-10 08:09:20.000000 rbloom-1.4.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      699 2023-06-10 08:09:20.000000 rbloom-1.4.5/.gitignore
+-rw-r--r--   0     1001      123     1103 2023-06-10 08:09:20.000000 rbloom-1.4.5/LICENSE
+-rw-r--r--   0     1001      123    10890 2023-06-10 08:09:20.000000 rbloom-1.4.5/README.md
+-rw-r--r--   0     1001      123      536 2023-06-10 08:09:20.000000 rbloom-1.4.5/pyproject.toml
+-rw-r--r--   0     1001      123     2896 2023-06-10 08:09:20.000000 rbloom-1.4.5/rbloom.pyi
+-rwxr-xr-x   0     1001      123     1058 2023-06-10 08:10:22.000000 rbloom-1.4.5/run-maturin-action.sh
+-rw-r--r--   0     1001      123    17789 2023-06-10 08:09:20.000000 rbloom-1.4.5/src/lib.rs
+-rwxr-xr-x   0     1001      123     2681 2023-06-10 08:09:20.000000 rbloom-1.4.5/tests/api_test.py
+-rw-r--r--   0        0        0     7419 2023-06-10 08:10:51.000000 rbloom-1.4.5/Cargo.lock
+-rw-r--r--   0        0        0    11387 1970-01-01 00:00:00.000000 rbloom-1.4.5/PKG-INFO
```

### Comparing `rbloom-1.4.4/.github/workflows/CI.yml` & `rbloom-1.4.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rbloom-1.4.4/.gitignore` & `rbloom-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rbloom-1.4.4/LICENSE` & `rbloom-1.4.5/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Kenan Hanke
+Copyright (c) 2023 Zachary Dremann
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rbloom-1.4.4/README.md` & `rbloom-1.4.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # rBloom
 
 [![PyPI](https://img.shields.io/pypi/v/rbloom)](https://pypi.org/project/rbloom/)
-![build](https://img.shields.io/github/actions/workflow/status/kenbyte/rbloom/CI.yml)
-![license](https://img.shields.io/github/license/kenbyte/rbloom)
+![build](https://img.shields.io/github/actions/workflow/status/KenanHanke/rbloom/CI.yml)
+![license](https://img.shields.io/github/license/KenanHanke/rbloom)
 
 A fast, simple and lightweight
 [Bloom filter](https://en.wikipedia.org/wiki/Bloom_filter) library for
-Python, implemented in Rust. It's designed to be as pythonic as
-possible, mimicking the built-in `set` type where it can, and works with
-any hashable object. While it's a new
-kid on the block (this project was started in 2023), it's also currently
-the fastest kid on the block by a long shot (see the section
+Python, implemented in Rust. It's designed to be as pythonic as possible,
+mimicking the built-in `set` type where it can, and works with any
+hashable object. While it's a new library (this project was started in
+2023), it's currently the fastest option for Python by
+a long shot (see the section
 [Benchmarks](#benchmarks)). Releases are published on
 [PyPI](https://pypi.org/project/rbloom/).
 
 ## Quickstart
 
 This library defines only one class, which can be used as follows:
 
@@ -27,25 +27,22 @@
 >>> "world" in bf
 False
 >>> bf.update(["hello", "world"])  # "hello" and "world" now in bf
 >>> other_bf = Bloom(200, 0.01)
 
 ### add some items to other_bf
 
->>> third_bf = bf | other_bf  # third_bf now contains all items in
-                              # bf and other_bf
+>>> third_bf = bf | other_bf    # third_bf now contains all items in
+                                # bf and other_bf
 >>> third_bf = bf.copy()
-... third_bf.update(other_bf)  # same as above
->>> bf.issubset(third_bf)  # bf <= third_bf also works
+... third_bf.update(other_bf)   # same as above
+>>> bf.issubset(third_bf)    # bf <= third_bf also works
 True
 ```
 
-Unlike BF's in real life, you can have as many of these as you want,
-and they all work well together!
-
 For the full API, see the section [Documentation](#documentation).
 
 ## Installation
 
 On almost all platforms, simply run:
 
 ```sh
@@ -79,27 +76,22 @@
 - **Lightweight:** `rbloom` has no dependencies of its own.
 - **Maintainable:** This library is very concise, and it's written
   in idiomatic Rust. Even if I were to stop maintaining `rbloom` (which I
   don't intend to), it would be trivially easy for you to fork it and keep
   it working for you.
 
 I started `rbloom` because I was looking for a simple Bloom filter
-dependency for a project, but the pure Python implementations were too
-slow. The only fast alternative I could find, `pybloomfiltermmap3` (written
-in C), showed undefined behavior on recent versions of Python (see below),
-so I made `rbloom` instead. It ended up being twice as fast and has grown to
-encompass a more complete API (e.g. with set comparisons like `issubset`).
-Do note that while `rbloom` only supports reading and writing its Bloom filter
-files in one sweep, `pybloomfiltermmap3` supports modifying them in-place with
-mmap. This is of limited utility in most cases due to the random-access-heavy
-nature of Bloom filters, which causes the entire file to be in memory after
-only a few operations in spite of mmap, but does more elegantly utilize the
-disk cache on most operating systems. As a rule of thumb, if you need filters
-larger than your system memory (one gigabyte stores around a billion items
-depending on the false positive rate), you should use `pybloomfiltermmap3`.
+dependency for a project, and the only sufficiently fast option
+(`pybloomfiltermmap3`) was segfaulting on recent Python versions. `rbloom`
+ended up being twice as fast and has grown to encompass a more complete
+API (e.g. with set comparisons like `issubset`). Do note that it doesn't
+use mmapped files, however. This shouldn't be an issue in most cases, as
+the random access heavy nature of a Bloom filter negates the benefits of
+mmap after very few operations, but it is something to keep in mind for
+edge cases.
 
 ## Benchmarks
 
 I implemented the following simple benchmark in the respective API of
 each library:
 
 ```python
@@ -110,21 +102,21 @@
 
 for i in range(10_000_000):
     assert i + 0.5 in bf
 ```
 
 This resulted in the following runtimes:
 
-| Library                                                            | Time     | Notes                                 |
-| ------------------------------------------------------------------ | -------- | ------------------------------------- |
-| [rBloom](https://pypi.org/project/rbloom/)                         | 5.956s   | works out-of-the-box                  |
-| [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) | 11.280s  | surprisingly hard to get working [1]  |
-| [pybloom3](https://pypi.org/project/pybloom3/)                     | 75.871s  | works out-of-the-box                  |
-| [Flor](https://pypi.org/project/Flor/)                             | 128.837s | doesn't work on arbitrary objects [2] |
-| [bloom-filter2](https://pypi.org/project/bloom-filter2/)           | 325.044s | doesn't work on arbitrary objects [2] |
+| Library                                                            | Time      | Notes                                 |
+| ------------------------------------------------------------------ | --------- | ------------------------------------- |
+| [rBloom](https://pypi.org/project/rbloom/)                         | 5.956 s   | works out-of-the-box                  |
+| [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) | 11.280 s  | surprisingly hard to get working [1]  |
+| [pybloom3](https://pypi.org/project/pybloom3/)                     | 75.871 s  | works out-of-the-box                  |
+| [Flor](https://pypi.org/project/Flor/)                             | 128.837 s | doesn't work on arbitrary objects [2] |
+| [bloom-filter2](https://pypi.org/project/bloom-filter2/)           | 325.044 s | doesn't work on arbitrary objects [2] |
 
 [1] It refused to install on Python 3.11 and kept segfaulting on 3.10 (on Linux
 as of January 2023), so I installed 3.7 on my machine for this benchmark.  
 [2] I tested both converting to bytes and pickling, and chose the faster time.
 
 The benchmark was run on a 2019 Dell XPS 15 7590 with an Intel Core
 i5-9300H. It was run 5 times for each library, and the average time was
@@ -198,15 +190,15 @@
     def copy(self) -> Bloom                       # duplicate self
 ```
 
 To prevent death and destruction, the bitwise set operations only work on
 filters where all parameters are equal (including the hash functions being
 the exact same object). Because this is a Bloom filter, the `__contains__`
 and `approx_items` methods are probabilistic, as are all the methods that
-compare two filters (such as `__le__` and `__issubset__`).
+compare two filters (such as `__le__` and `issubset`).
 
 ## Cryptographic security
 
 Python's built-in hash function is designed to be fast, not maximally
 collision-resistant, so if your program depends on the false positive rate
 being perfectly correct, you may want to supply your own hash function.
 This is especially the case when working with very large filters (more
@@ -220,22 +212,23 @@
 from hashlib import sha256
 from pickle import dumps
 
 def hash_func(obj):
     h = sha256(dumps(obj)).digest()
     return int.from_bytes(h[:16], "big") - 2**127
 
-bf = Bloom(100_000_000, 0.01, hash_func=hash_func)
+bf = Bloom(100_000_000, 0.01, hash_func)
 ```
 
 When you throw away Python's built-in hash function and start hashing
 serialized representations of objects, however, you open up a breach into
 the scary realm of the unpythonic:
 
-- Numbers like `2`, `2.0` and `2 + 0j` will suddenly no longer be equal.
+- Numbers like `1`, `1.0`, `1 + 0j` and `True` will suddenly no longer
+  be equal.
 - Instances of classes with custom hashing logic (e.g. to stop
   caches inside instances from affecting their hashes) will suddenly
   display undefined behavior.
 - Objects that can't be serialized simply won't be hashable at all.
 
 Making you supply your own hash function in this case is a deliberate
 design decision intended to show you what you're doing and prevent
@@ -260,15 +253,15 @@
 
 bf.save("bf.bloom")
 
 loaded_bf = Bloom.load("bf.bloom", some_hash_func)
 assert loaded_bf == bf
 ```
 
-The size of the file is `bf.size_in_bits // 8 + 8` bytes.
+The size of the file is `bf.size_in_bits / 8 + 8` bytes.
 
 ---
 
 **Statement of attribution:** Bloom filters were originally proposed in
 [(Bloom, 1970)](https://doi.org/10.1145/362686.362692). Furthermore, this
 implementation makes use of a constant recommended by
 [(L'Ecuyer, 1999)](https://doi.org/10.1090/S0025-5718-99-00996-5) for
```

### Comparing `rbloom-1.4.4/pyproject.toml` & `rbloom-1.4.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,11 +10,11 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 
 [project.urls]
-"Source Code" = "https://github.com/kenbyte/rbloom"
+"Source Code" = "https://github.com/KenanHanke/rbloom"
 
 [tool.maturin]
 sdist-include = ["LICENSE", "README.md"]
```

### Comparing `rbloom-1.4.4/rbloom.pyi` & `rbloom-1.4.5/rbloom.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, Callable, Iterable, Union
+from typing import Any, Callable, Iterable, Union, final
 
 
+@final
 class Bloom:
 
     # expected_items:  max number of items to be added to the filter
     # false_positive_rate:  max false positive rate of the filter
     # hash_func:  optional argument, see section "Cryptographic security"
     def __init__(self, expected_items: int, false_positive_rate: float,
                  hash_func=__builtins__.hash) -> None: ...
@@ -19,26 +20,26 @@
 
     # estimated number of items in the filter
     @property
     def approx_items(self) -> float: ...
 
     # load from file, see section "Persistence"
     @classmethod
-    def load(cls, filepath: str, hash_func) -> Bloom: ...
+    def load(cls, filepath: str, hash_func: Callable[[Any], int]) -> Bloom: ...
 
     # save to file, see section "Persistence"
     def save(self, filepath: str) -> None: ...
 
     #####################################################################
     #                    ALL SUBSEQUENT METHODS ARE                     #
     #              EQUIVALENT TO THE CORRESPONDING METHODS              #
     #                     OF THE BUILT-IN SET TYPE                      #
     #####################################################################
 
-    def add(self, obj: Any) -> None: ...
+    def add(self, obj: Any, /) -> None: ...
 
     def __contains__(self, obj: Any) -> bool: ...
 
     def __bool__(self) -> bool: ...                   # False if empty
 
     def __repr__(self) -> str: ...                    # basic info
 
@@ -63,17 +64,17 @@
     def intersection_update(self, *others: Union[Iterable, Bloom]) -> None: ...
 
     # these implement <, >, <=, >=, ==, !=
     def __lt__(self, other: Bloom) -> bool: ...
     def __gt__(self, other: Bloom) -> bool: ...
     def __le__(self, other: Bloom) -> bool: ...
     def __ge__(self, other: Bloom) -> bool: ...
-    def __eq__(self, other: Bloom) -> bool: ...
-    def __ne__(self, other: Bloom) -> bool: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __ne__(self, other: object) -> bool: ...
 
-    def issubset(self, other: Bloom) -> bool: ...      # self <= other
+    def issubset(self, other: Bloom, /) -> bool: ...      # self <= other
 
-    def issuperset(self, other: Bloom) -> bool: ...    # self >= other
+    def issuperset(self, other: Bloom, /) -> bool: ...    # self >= other
 
-    def clear(self) -> None: ...                       # remove all items
+    def clear(self) -> None: ...                          # remove all items
 
-    def copy(self) -> Bloom: ...                       # duplicate self
+    def copy(self) -> Bloom: ...                          # duplicate self
```

### Comparing `rbloom-1.4.4/run-maturin-action.sh` & `rbloom-1.4.5/run-maturin-action.sh`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 set -e
 echo "::group::Install Rust"
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain stable
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set stable
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
-export PATH="$PATH:/opt/python/cp36-cp36m/bin:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin"
+export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.14.13/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v0.14.17/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
+python3 -m pip install cffi || true
 echo "::endgroup::"
 echo "::group::Install Rust target"
-if [[ ! -d $(rustc --print target-libdir --target i686-unknown-linux-gnu) ]]; then rustup target add i686-unknown-linux-gnu; fi
+if [[ ! -d $(rustc --print target-libdir --target aarch64-unknown-linux-gnu) ]]; then rustup target add aarch64-unknown-linux-gnu; fi
 echo "::endgroup::"
-maturin build --target i686-unknown-linux-gnu --release --sdist -o dist --find-interpreter
+maturin build --target aarch64-unknown-linux-gnu --release --sdist -o dist --find-interpreter
```

### Comparing `rbloom-1.4.4/src/lib.rs` & `rbloom-1.4.5/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use bitline::BitLine;
-use pyo3::exceptions::PyValueError;
+use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::types::PyType;
 use pyo3::{basic::CompareOp, prelude::*, types::PyTuple};
 use std::fs::File;
 use std::io::{Read, Write};
+use std::mem;
 
-#[pyclass]
+#[pyclass(module = "rbloom")]
 #[derive(Clone)]
 struct Bloom {
     filter: BitLine,
     k: u64, // Number of hash functions (implemented via a LCG that uses
     // the original hash as a seed)
     hash_func: Option<PyObject>,
 }
@@ -21,26 +22,24 @@
         expected_items: u64,
         false_positive_rate: f64,
         hash_func: Option<&PyAny>,
     ) -> PyResult<Self> {
         // Check the inputs
         if let Some(hash_func) = hash_func {
             if !hash_func.is_callable() {
-                return Err(pyo3::exceptions::PyTypeError::new_err(
-                    "hash_func must be callable",
-                ));
+                return Err(PyTypeError::new_err("hash_func must be callable"));
             }
         }
         if false_positive_rate <= 0.0 || false_positive_rate >= 1.0 {
-            return Err(pyo3::exceptions::PyValueError::new_err(
+            return Err(PyValueError::new_err(
                 "false_positive_rate must be between 0 and 1",
             ));
         }
         if expected_items == 0 {
-            return Err(pyo3::exceptions::PyValueError::new_err(
+            return Err(PyValueError::new_err(
                 "expected_items must be greater than 0",
             ));
         }
 
         // Calculate the parameters for the filter
         let size_in_bits =
             -1.0 * (expected_items as f64) * false_positive_rate.ln() / 2.0f64.ln().powi(2);
@@ -57,27 +56,30 @@
         Ok(Bloom {
             filter: BitLine::new(size_in_bits as u64)?,
             k: k as u64,
             hash_func,
         })
     }
 
+    /// Number of buckets in the filter
     #[getter]
     fn size_in_bits(&self) -> u64 {
         self.filter.len()
     }
 
+    /// Retrieve the hash_func given to __init__
     #[getter]
     fn hash_func<'a>(&'a self, py: Python<'a>) -> PyResult<&'a PyAny> {
         match self.hash_func.as_ref() {
             Some(hash_func) => Ok(hash_func.as_ref(py)),
             None => get_builtin_hash_func(py),
         }
     }
 
+    /// Estimated number of items in the filter
     #[getter]
     fn approx_items(&self) -> f64 {
         let len = self.filter.len() as f64;
         let bits_set = self.filter.sum() as f64;
         (len / (self.k as f64) * (1.0 - (bits_set) / len).ln()).abs()
     }
 
@@ -205,20 +207,18 @@
                 }
                 self.__iand__(temp)?;
             }
         }
         Ok(())
     }
 
-    #[pyo3(signature = ())]
     fn clear(&mut self) {
         self.filter.clear();
     }
 
-    #[pyo3(signature = ())]
     fn copy(&self) -> Bloom {
         self.clone()
     }
 
     fn __repr__(&self) -> String {
         // Use a format that makes it clear that the object
         // cannot be reconstructed from the repr
@@ -244,45 +244,45 @@
             CompareOp::Gt => other.filter.is_strict_subset(&self.filter),
         })
     }
 
     #[classattr]
     const __hash__: Option<PyObject> = None;
 
+    /// Load from a file, see "Persistence" section in the README
     #[classmethod]
     fn load(_cls: &PyType, filepath: &str, hash_func: &PyAny) -> PyResult<Bloom> {
         // check that the hash_func is callable
         if !hash_func.is_callable() {
-            return Err(pyo3::exceptions::PyTypeError::new_err(
-                "hash_func must be callable",
-            ));
+            return Err(PyTypeError::new_err("hash_func must be callable"));
         }
         // check that the hash_func isn't the built-in hash function
         if hash_func.is(get_builtin_hash_func(hash_func.py())?) {
             return Err(PyValueError::new_err(
                 "Cannot load a bloom filter that uses the built-in hash function",
             ));
         }
         let hash_func = Some(hash_func.to_object(hash_func.py()));
 
         let mut file = File::open(filepath)?;
 
-        let mut k_bytes = [0; 8];
+        let mut k_bytes = [0; mem::size_of::<u64>()];
         file.read_exact(&mut k_bytes)?;
         let k = u64::from_le_bytes(k_bytes);
 
         let filter = BitLine::load(&mut file)?;
 
         Ok(Bloom {
             filter,
             k,
             hash_func,
         })
     }
 
+    /// Save to a file, see "Persistence" section in the README
     fn save(&self, filepath: &str) -> PyResult<()> {
         if self.hash_func.is_none() {
             return Err(PyValueError::new_err(
                 "Cannot save a bloom filter that uses the built-in hash function",
             ));
         }
         let mut file = File::create(filepath)?;
@@ -538,30 +538,30 @@
         }
         None => Ok(o.hash()? as i128),
     }
 }
 
 fn check_compatible(a: &Bloom, b: &Bloom) -> PyResult<()> {
     if a.k != b.k || a.filter.len() != b.filter.len() {
-        return Err(pyo3::exceptions::PyValueError::new_err(
+        return Err(PyValueError::new_err(
             "size and max false positive rate must be the same for both filters",
         ));
     }
 
     // now only the hash function can be different
     let same_hash_fn = match (&a.hash_func, &b.hash_func) {
         (Some(lhs), Some(rhs)) => lhs.is(rhs),
         (&None, &None) => true,
         _ => false,
     };
 
     if same_hash_fn {
         Ok(())
     } else {
-        Err(pyo3::exceptions::PyValueError::new_err(
+        Err(PyValueError::new_err(
             "Bloom filters must have the same hash function",
         ))
     }
 }
 
 fn get_builtin_hash_func(py: Python<'_>) -> PyResult<&'_ PyAny> {
     let builtins = PyModule::import(py, "builtins")?;
```

### Comparing `rbloom-1.4.4/tests/api_test.py` & `rbloom-1.4.5/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `rbloom-1.4.4/Cargo.lock` & `rbloom-1.4.5/Cargo.lock`

 * *Files 24% similar despite different names*

```diff
@@ -24,156 +24,156 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rbloom"
-version = "1.4.4"
+version = "1.4.5"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
@@ -184,99 +184,90 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `rbloom-1.4.4/PKG-INFO` & `rbloom-1.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: rbloom
-Version: 1.4.4
+Version: 1.4.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Highly optimized Bloom filter that mimics the Python set API, written in Rust
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/kenbyte/rbloom
+Project-URL: Source Code, https://github.com/KenanHanke/rbloom
 
 # rBloom
 
 [![PyPI](https://img.shields.io/pypi/v/rbloom)](https://pypi.org/project/rbloom/)
-![build](https://img.shields.io/github/actions/workflow/status/kenbyte/rbloom/CI.yml)
-![license](https://img.shields.io/github/license/kenbyte/rbloom)
+![build](https://img.shields.io/github/actions/workflow/status/KenanHanke/rbloom/CI.yml)
+![license](https://img.shields.io/github/license/KenanHanke/rbloom)
 
 A fast, simple and lightweight
 [Bloom filter](https://en.wikipedia.org/wiki/Bloom_filter) library for
-Python, implemented in Rust. It's designed to be as pythonic as
-possible, mimicking the built-in `set` type where it can, and works with
-any hashable object. While it's a new
-kid on the block (this project was started in 2023), it's also currently
-the fastest kid on the block by a long shot (see the section
+Python, implemented in Rust. It's designed to be as pythonic as possible,
+mimicking the built-in `set` type where it can, and works with any
+hashable object. While it's a new library (this project was started in
+2023), it's currently the fastest option for Python by
+a long shot (see the section
 [Benchmarks](#benchmarks)). Releases are published on
 [PyPI](https://pypi.org/project/rbloom/).
 
 ## Quickstart
 
 This library defines only one class, which can be used as follows:
 
@@ -39,25 +39,22 @@
 >>> "world" in bf
 False
 >>> bf.update(["hello", "world"])  # "hello" and "world" now in bf
 >>> other_bf = Bloom(200, 0.01)
 
 ### add some items to other_bf
 
->>> third_bf = bf | other_bf  # third_bf now contains all items in
-                              # bf and other_bf
+>>> third_bf = bf | other_bf    # third_bf now contains all items in
+                                # bf and other_bf
 >>> third_bf = bf.copy()
-... third_bf.update(other_bf)  # same as above
->>> bf.issubset(third_bf)  # bf <= third_bf also works
+... third_bf.update(other_bf)   # same as above
+>>> bf.issubset(third_bf)    # bf <= third_bf also works
 True
 ```
 
-Unlike BF's in real life, you can have as many of these as you want,
-and they all work well together!
-
 For the full API, see the section [Documentation](#documentation).
 
 ## Installation
 
 On almost all platforms, simply run:
 
 ```sh
@@ -91,27 +88,22 @@
 - **Lightweight:** `rbloom` has no dependencies of its own.
 - **Maintainable:** This library is very concise, and it's written
   in idiomatic Rust. Even if I were to stop maintaining `rbloom` (which I
   don't intend to), it would be trivially easy for you to fork it and keep
   it working for you.
 
 I started `rbloom` because I was looking for a simple Bloom filter
-dependency for a project, but the pure Python implementations were too
-slow. The only fast alternative I could find, `pybloomfiltermmap3` (written
-in C), showed undefined behavior on recent versions of Python (see below),
-so I made `rbloom` instead. It ended up being twice as fast and has grown to
-encompass a more complete API (e.g. with set comparisons like `issubset`).
-Do note that while `rbloom` only supports reading and writing its Bloom filter
-files in one sweep, `pybloomfiltermmap3` supports modifying them in-place with
-mmap. This is of limited utility in most cases due to the random-access-heavy
-nature of Bloom filters, which causes the entire file to be in memory after
-only a few operations in spite of mmap, but does more elegantly utilize the
-disk cache on most operating systems. As a rule of thumb, if you need filters
-larger than your system memory (one gigabyte stores around a billion items
-depending on the false positive rate), you should use `pybloomfiltermmap3`.
+dependency for a project, and the only sufficiently fast option
+(`pybloomfiltermmap3`) was segfaulting on recent Python versions. `rbloom`
+ended up being twice as fast and has grown to encompass a more complete
+API (e.g. with set comparisons like `issubset`). Do note that it doesn't
+use mmapped files, however. This shouldn't be an issue in most cases, as
+the random access heavy nature of a Bloom filter negates the benefits of
+mmap after very few operations, but it is something to keep in mind for
+edge cases.
 
 ## Benchmarks
 
 I implemented the following simple benchmark in the respective API of
 each library:
 
 ```python
@@ -122,21 +114,21 @@
 
 for i in range(10_000_000):
     assert i + 0.5 in bf
 ```
 
 This resulted in the following runtimes:
 
-| Library                                                            | Time     | Notes                                 |
-| ------------------------------------------------------------------ | -------- | ------------------------------------- |
-| [rBloom](https://pypi.org/project/rbloom/)                         | 5.956s   | works out-of-the-box                  |
-| [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) | 11.280s  | surprisingly hard to get working [1]  |
-| [pybloom3](https://pypi.org/project/pybloom3/)                     | 75.871s  | works out-of-the-box                  |
-| [Flor](https://pypi.org/project/Flor/)                             | 128.837s | doesn't work on arbitrary objects [2] |
-| [bloom-filter2](https://pypi.org/project/bloom-filter2/)           | 325.044s | doesn't work on arbitrary objects [2] |
+| Library                                                            | Time      | Notes                                 |
+| ------------------------------------------------------------------ | --------- | ------------------------------------- |
+| [rBloom](https://pypi.org/project/rbloom/)                         | 5.956 s   | works out-of-the-box                  |
+| [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) | 11.280 s  | surprisingly hard to get working [1]  |
+| [pybloom3](https://pypi.org/project/pybloom3/)                     | 75.871 s  | works out-of-the-box                  |
+| [Flor](https://pypi.org/project/Flor/)                             | 128.837 s | doesn't work on arbitrary objects [2] |
+| [bloom-filter2](https://pypi.org/project/bloom-filter2/)           | 325.044 s | doesn't work on arbitrary objects [2] |
 
 [1] It refused to install on Python 3.11 and kept segfaulting on 3.10 (on Linux
 as of January 2023), so I installed 3.7 on my machine for this benchmark.  
 [2] I tested both converting to bytes and pickling, and chose the faster time.
 
 The benchmark was run on a 2019 Dell XPS 15 7590 with an Intel Core
 i5-9300H. It was run 5 times for each library, and the average time was
@@ -210,15 +202,15 @@
     def copy(self) -> Bloom                       # duplicate self
 ```
 
 To prevent death and destruction, the bitwise set operations only work on
 filters where all parameters are equal (including the hash functions being
 the exact same object). Because this is a Bloom filter, the `__contains__`
 and `approx_items` methods are probabilistic, as are all the methods that
-compare two filters (such as `__le__` and `__issubset__`).
+compare two filters (such as `__le__` and `issubset`).
 
 ## Cryptographic security
 
 Python's built-in hash function is designed to be fast, not maximally
 collision-resistant, so if your program depends on the false positive rate
 being perfectly correct, you may want to supply your own hash function.
 This is especially the case when working with very large filters (more
@@ -232,22 +224,23 @@
 from hashlib import sha256
 from pickle import dumps
 
 def hash_func(obj):
     h = sha256(dumps(obj)).digest()
     return int.from_bytes(h[:16], "big") - 2**127
 
-bf = Bloom(100_000_000, 0.01, hash_func=hash_func)
+bf = Bloom(100_000_000, 0.01, hash_func)
 ```
 
 When you throw away Python's built-in hash function and start hashing
 serialized representations of objects, however, you open up a breach into
 the scary realm of the unpythonic:
 
-- Numbers like `2`, `2.0` and `2 + 0j` will suddenly no longer be equal.
+- Numbers like `1`, `1.0`, `1 + 0j` and `True` will suddenly no longer
+  be equal.
 - Instances of classes with custom hashing logic (e.g. to stop
   caches inside instances from affecting their hashes) will suddenly
   display undefined behavior.
 - Objects that can't be serialized simply won't be hashable at all.
 
 Making you supply your own hash function in this case is a deliberate
 design decision intended to show you what you're doing and prevent
@@ -272,15 +265,15 @@
 
 bf.save("bf.bloom")
 
 loaded_bf = Bloom.load("bf.bloom", some_hash_func)
 assert loaded_bf == bf
 ```
 
-The size of the file is `bf.size_in_bits // 8 + 8` bytes.
+The size of the file is `bf.size_in_bits / 8 + 8` bytes.
 
 ---
 
 **Statement of attribution:** Bloom filters were originally proposed in
 [(Bloom, 1970)](https://doi.org/10.1145/362686.362692). Furthermore, this
 implementation makes use of a constant recommended by
 [(L'Ecuyer, 1999)](https://doi.org/10.1090/S0025-5718-99-00996-5) for
```

