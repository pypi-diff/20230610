# Comparing `tmp/typst-0.4.0.tar.gz` & `tmp/typst-0.5.0.tar.gz`

## Comparing `typst-0.4.0.tar` & `typst-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 typst-0.4.0/Cargo.toml
--rw-r--r--   0     1001      123     2901 2023-05-21 06:11:04.000000 typst-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-05-21 06:11:04.000000 typst-0.4.0/.gitignore
--rw-r--r--   0     1001      123     9723 2023-05-21 06:11:04.000000 typst-0.4.0/LICENSE
--rw-r--r--   0     1001      123      766 2023-05-21 06:11:04.000000 typst-0.4.0/README.md
--rw-r--r--   0     1001      123      421 2023-05-21 06:11:04.000000 typst-0.4.0/pyproject.toml
--rw-r--r--   0     1001      123       74 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/__init__.py
--rw-r--r--   0     1001      123      483 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/__init__.pyi
--rw-r--r--   0     1001      123   331992 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
--rw-r--r--   0     1001      123   253580 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
--rw-r--r--   0     1001      123   251932 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
--rw-r--r--   0     1001      123   340712 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono.ttf
--rw-r--r--   0     1001      123   806856 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_R.ttf
--rw-r--r--   0     1001      123   748600 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_RB.ttf
--rw-r--r--   0     1001      123   533532 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_RBI.ttf
--rw-r--r--   0     1001      123   721340 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_RI.ttf
--rw-r--r--   0     1001      123   499128 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-Bold.otf
--rw-r--r--   0     1001      123   445800 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-BoldItalic.otf
--rw-r--r--   0     1001      123   464808 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-Italic.otf
--rw-r--r--   0     1001      123   547508 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-Regular.otf
--rw-r--r--   0     1001      123  2161432 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCMMath-Book.otf
--rw-r--r--   0     1001      123  1229208 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCMMath-Regular.otf
--rw-r--r--   0     1001      123        1 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/py.typed
--rw-r--r--   0     1001      123     9419 2023-05-21 06:11:04.000000 typst-0.4.0/src/compiler.rs
--rw-r--r--   0     1001      123     3946 2023-05-21 06:11:04.000000 typst-0.4.0/src/lib.rs
--rw-r--r--   0     1001      123    47424 2023-05-21 06:11:04.000000 typst-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 typst-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      123     2989 2023-06-10 12:29:15.000000 typst-0.5.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-10 12:29:15.000000 typst-0.5.0/.gitignore
+-rw-r--r--   0     1001      123     9723 2023-06-10 12:29:15.000000 typst-0.5.0/LICENSE
+-rw-r--r--   0     1001      123      766 2023-06-10 12:29:15.000000 typst-0.5.0/README.md
+-rw-r--r--   0     1001      123      419 2023-06-10 12:29:15.000000 typst-0.5.0/pyproject.toml
+-rw-r--r--   0     1001      123       74 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/__init__.py
+-rw-r--r--   0     1001      123      483 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/__init__.pyi
+-rw-r--r--   0     1001      123   331992 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0     1001      123   253580 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
+-rw-r--r--   0     1001      123   251932 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
+-rw-r--r--   0     1001      123   340712 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0     1001      123   806856 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/LinLibertine_R.ttf
+-rw-r--r--   0     1001      123   748600 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/LinLibertine_RB.ttf
+-rw-r--r--   0     1001      123   533532 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/LinLibertine_RBI.ttf
+-rw-r--r--   0     1001      123   721340 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/LinLibertine_RI.ttf
+-rw-r--r--   0     1001      123   499128 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/NewCM10-Bold.otf
+-rw-r--r--   0     1001      123   445800 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/NewCM10-BoldItalic.otf
+-rw-r--r--   0     1001      123   464808 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/NewCM10-Italic.otf
+-rw-r--r--   0     1001      123   547508 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/NewCM10-Regular.otf
+-rw-r--r--   0     1001      123  2161432 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/NewCMMath-Book.otf
+-rw-r--r--   0     1001      123  1229208 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/fonts/NewCMMath-Regular.otf
+-rw-r--r--   0     1001      123        1 2023-06-10 12:29:15.000000 typst-0.5.0/python/typst/py.typed
+-rw-r--r--   0     1001      123    10301 2023-06-10 12:29:15.000000 typst-0.5.0/src/compiler.rs
+-rw-r--r--   0     1001      123     3946 2023-06-10 12:29:15.000000 typst-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      123    54971 2023-06-10 12:29:15.000000 typst-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.5.0/PKG-INFO
```

### Comparing `typst-0.4.0/.github/workflows/CI.yml` & `typst-0.5.0/.github/workflows/CI.yml`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         target: [x64, x86]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
           architecture: ${{ matrix.target }}
+      - uses: dtolnay/rust-toolchain@stable
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
@@ -74,14 +75,15 @@
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
+      - uses: dtolnay/rust-toolchain@stable
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
```

### Comparing `typst-0.4.0/.gitignore` & `typst-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/LICENSE` & `typst-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/README.md` & `typst-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/DejaVuSansMono-Bold.ttf` & `typst-0.5.0/python/typst/fonts/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf` & `typst-0.5.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf` & `typst-0.5.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/DejaVuSansMono.ttf` & `typst-0.5.0/python/typst/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/LinLibertine_R.ttf` & `typst-0.5.0/python/typst/fonts/LinLibertine_R.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/LinLibertine_RB.ttf` & `typst-0.5.0/python/typst/fonts/LinLibertine_RB.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/LinLibertine_RBI.ttf` & `typst-0.5.0/python/typst/fonts/LinLibertine_RBI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/LinLibertine_RI.ttf` & `typst-0.5.0/python/typst/fonts/LinLibertine_RI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/NewCM10-Bold.otf` & `typst-0.5.0/python/typst/fonts/NewCM10-Bold.otf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/NewCM10-BoldItalic.otf` & `typst-0.5.0/python/typst/fonts/NewCM10-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/NewCM10-Italic.otf` & `typst-0.5.0/python/typst/fonts/NewCM10-Italic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/NewCM10-Regular.otf` & `typst-0.5.0/python/typst/fonts/NewCM10-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/NewCMMath-Book.otf` & `typst-0.5.0/python/typst/fonts/NewCMMath-Book.otf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/python/typst/fonts/NewCMMath-Regular.otf` & `typst-0.5.0/python/typst/fonts/NewCMMath-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/src/compiler.rs` & `typst-0.5.0/src/compiler.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-use std::cell::{RefCell, RefMut};
+use std::cell::{Cell, OnceCell, RefCell, RefMut};
 use std::collections::HashMap;
 use std::fs::{self, File};
 use std::hash::Hash;
 use std::path::{Path, PathBuf};
 
+use chrono::Datelike;
 use comemo::Prehashed;
 use elsa::FrozenVec;
 use memmap2::Mmap;
-use once_cell::unsync::OnceCell;
 use same_file::Handle;
 use siphasher::sip128::{Hasher128, SipHasher13};
 use typst::diag::{FileError, FileResult, StrResult};
-use typst::eval::Library;
+use typst::eval::{Datetime, Library};
 use typst::font::{Font, FontBook, FontInfo};
 use typst::syntax::{Source, SourceId};
 use typst::util::{Buffer, PathExt};
 use typst::World;
 use walkdir::WalkDir;
 
 /// A world that provides access to the operating system.
@@ -23,14 +23,15 @@
     root: PathBuf,
     library: Prehashed<Library>,
     book: Prehashed<FontBook>,
     fonts: Vec<FontSlot>,
     hashes: RefCell<HashMap<PathBuf, FileResult<PathHash>>>,
     paths: RefCell<HashMap<PathHash, PathSlot>>,
     sources: FrozenVec<Box<Source>>,
+    today: Cell<Option<Datetime>>,
     main: SourceId,
 }
 
 /// Holds details about the location of a font and lazily the font itself.
 struct FontSlot {
     path: PathBuf,
     index: u32,
@@ -58,22 +59,28 @@
     }
 
     fn resolve(&self, path: &Path) -> FileResult<SourceId> {
         self.slot(path)?
             .source
             .get_or_init(|| {
                 let buf = read(path)?;
-                let text = String::from_utf8(buf)?;
+                let text = if buf.starts_with(b"\xef\xbb\xbf") {
+                    // remove UTF-8 BOM
+                    std::str::from_utf8(&buf[3..])?.to_owned()
+                } else {
+                    // Assume UTF-8
+                    String::from_utf8(buf)?
+                };
                 Ok(self.insert(path, text))
             })
             .clone()
     }
 
     fn source(&self, id: SourceId) -> &Source {
-        &self.sources[id.into_u16() as usize]
+        &self.sources[id.as_u16() as usize]
     }
 
     fn book(&self) -> &Prehashed<FontBook> {
         &self.book
     }
 
     fn font(&self, id: usize) -> Option<Font> {
@@ -88,14 +95,31 @@
 
     fn file(&self, path: &Path) -> FileResult<Buffer> {
         self.slot(path)?
             .buffer
             .get_or_init(|| read(path).map(Buffer::from))
             .clone()
     }
+
+    fn today(&self, offset: Option<i64>) -> Option<Datetime> {
+        if self.today.get().is_none() {
+            let datetime = match offset {
+                None => chrono::Local::now().naive_local(),
+                Some(o) => (chrono::Utc::now() + chrono::Duration::hours(o)).naive_utc(),
+            };
+
+            self.today.set(Some(Datetime::from_ymd(
+                datetime.year(),
+                datetime.month().try_into().ok()?,
+                datetime.day().try_into().ok()?,
+            )?))
+        }
+
+        self.today.get()
+    }
 }
 
 impl SystemWorld {
     pub fn new(root: PathBuf, font_paths: &[PathBuf], font_files: &[PathBuf]) -> Self {
         let mut searcher = FontSearcher::new();
         searcher.search_system();
 
@@ -110,14 +134,15 @@
             root,
             library: Prehashed::new(typst_library::build()),
             book: Prehashed::new(searcher.book),
             fonts: searcher.fonts,
             hashes: RefCell::default(),
             paths: RefCell::default(),
             sources: FrozenVec::new(),
+            today: Cell::new(None),
             main: SourceId::detached(),
         }
     }
 
     fn slot(&self, path: &Path) -> FileResult<RefMut<PathSlot>> {
         let mut hashes = self.hashes.borrow_mut();
         let hash = match hashes.get(path).cloned() {
```

### Comparing `typst-0.4.0/src/lib.rs` & `typst-0.5.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typst-0.4.0/Cargo.lock` & `typst-0.5.0/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,37 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
@@ -39,17 +54,17 @@
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "biblatex"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc9fd60378277e44cd400ec5f35e768ce0d5a63d8d18ac7b1a9231196251dae5"
 dependencies = [
@@ -97,14 +112,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "bumpalo"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "byteorder"
@@ -140,23 +161,31 @@
 name = "chinese-variant"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aeea139b89efab957972956e5d3e4efb66a6c261f726abf6911040cc8ef700f7"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
- "num-integer",
+ "android-tzdata",
+ "iana-time-zone",
  "num-traits",
+ "winapi",
 ]
 
 [[package]]
+name = "cobs"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67ba02a97a2bd10f4b59b25c7973101c79642302776489e030cd13cdab09ed15"
+
+[[package]]
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "comemo"
@@ -176,27 +205,33 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "core-foundation-sys"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+
+[[package]]
 name = "crc32fast"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "csv"
-version = "1.2.1"
+version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b015497079b9a9d69c02ad25de6c0a6edef051ea6360a327d0bd05802ef64ad"
+checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
 dependencies = [
  "csv-core",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -229,26 +264,26 @@
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
  "option-ext",
  "redox_users",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "ecow"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5c5051925c54d9a42c8652313b5358a7432eed209466b443ed5220431243a14"
@@ -268,15 +303,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4f76552f53cefc9a7f64987c3701b99d982f7690606fd67de1d09712fbf52f1"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "fancy-regex"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d6b8560a05112eb52f04b00e5d3790c0dd75d9d980eb8a122fb23b92a623ccf"
@@ -326,26 +361,26 @@
  "memmap2 0.5.10",
  "slotmap",
  "ttf-parser",
 ]
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -394,18 +429,153 @@
 [[package]]
 name = "hypher"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0cf92443ef10ecfc1b8b4b65a93e31d983f020a355699d83874b12a7c797ac3"
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.57"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "icu_collections"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef8302d8dfd6044d3ddb3f807a5ef3d7bbca9a574959c6d6e4dc39aa7012d0d5"
+dependencies = [
+ "displaydoc",
+ "serde",
+ "yoke",
+ "zerofrom",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_locid"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3003f85dccfc0e238ff567693248c59153a46f4e6125ba4020b973cef4d1d335"
+dependencies = [
+ "displaydoc",
+ "litemap",
+ "tinystr",
+ "writeable",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_properties"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ce0e1aa26851f16c9e04412a5911c86b7f8768dac8f8d4c5f1c568a7e5d7a434"
+dependencies = [
+ "displaydoc",
+ "icu_collections",
+ "icu_provider",
+ "serde",
+ "tinystr",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_provider"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8dc312a7b6148f7dfe098047ae2494d12d4034f48ade58d4f353000db376e305"
+dependencies = [
+ "displaydoc",
+ "icu_locid",
+ "icu_provider_macros",
+ "postcard",
+ "serde",
+ "stable_deref_trait",
+ "writeable",
+ "yoke",
+ "zerofrom",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_provider_adapters"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4ae1e2bd0c41728b77e7c46e9afdec5e2127d1eedacc684724667d50c126bd3"
+dependencies = [
+ "icu_locid",
+ "icu_provider",
+ "tinystr",
+ "yoke",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_provider_blob"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd364c9a01f791a4bc04a74cf2a1d01d9f6926a40fd5ae1c28004e1e70d8338b"
+dependencies = [
+ "icu_provider",
+ "postcard",
+ "serde",
+ "writeable",
+ "yoke",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_provider_macros"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd8b728b9421e93eff1d9f8681101b78fa745e0748c95c655c83f337044a7e10"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "icu_segmenter"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3300a7b6bf187be98a57264ad094f11f2e062c2e8263132af010ff522ee5495"
+dependencies = [
+ "displaydoc",
+ "icu_collections",
+ "icu_locid",
+ "icu_provider",
+ "num-traits",
+ "serde",
+ "utf8_iter",
+ "zerovec",
+]
+
+[[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "if_chain"
@@ -469,14 +639,23 @@
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
 
 [[package]]
+name = "js-sys"
+version = "0.3.63"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "kurbo"
 version = "0.9.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd85a5776cd9500c2e2059c8c76c3b01528566b7fcbaf8098b55a33fc298849b"
 dependencies = [
  "arrayvec",
 ]
@@ -485,17 +664,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+
+[[package]]
+name = "libm"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
@@ -506,31 +691,34 @@
 checksum = "9c5e9ef2d2ad6fe67a59ace27c203c8d3a71d195532ee82e3bbe0d5f9a9ca541"
 dependencies = [
  "rand",
  "rand_chacha",
 ]
 
 [[package]]
+name = "litemap"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a04a5b2b6f54acba899926491d0a6c59d98012938ca2ab5befb281c034e8f94"
+
+[[package]]
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
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -541,26 +729,26 @@
 checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memmap2"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0aa1b505aeecb0adb017db2b6a79a17a38e64f882a201f05e9de8a982cd6096"
+checksum = "6d28bba84adfe6646737845bc5ebbfa2c08424eb1c37e94a1fd2a82adb56a872"
 dependencies = [
  "libc",
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
 name = "miniz_oxide"
 version = "0.7.1"
@@ -606,27 +794,28 @@
 [[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "numerals"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e25be21376a772d15f97ae789845340a9651d3c4246ff5ebb6a2b35f9c37bd31"
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
@@ -638,23 +827,23 @@
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
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
@@ -668,17 +857,17 @@
  "bitflags 1.3.2",
  "itoa",
  "ryu",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "phf"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
 dependencies = [
@@ -725,24 +914,34 @@
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "postcard"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cfa512cd0d087cc9f99ad30a1bf64795b67871edbead083ffc3a4dfafa59aa00"
+dependencies = [
+ "cobs",
+ "serde",
+]
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -750,77 +949,77 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
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
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -858,46 +1057,55 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags 1.3.2",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.1",
+ "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "resvg"
 version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "142e83d8ae8c8c639f304698a5567b229ba65caba867bf4387bbc0ae158827cf"
 dependencies = [
@@ -981,30 +1189,30 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -1088,17 +1296,17 @@
  "libc",
  "psm",
  "winapi",
 ]
 
 [[package]]
 name = "strict-num"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9df65f20698aeed245efdde3628a6b559ea1239bbb871af1b6e3b58c413b2bd1"
+checksum = "6637bab7722d379c8b41ba849228d680cc12d0a45ba1fa2b48f2a30577a06731"
 dependencies = [
  "float-cmp",
 ]
 
 [[package]]
 name = "strum"
 version = "0.24.1"
@@ -1157,24 +1365,36 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "synstructure"
+version = "0.12.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "unicode-xid",
+]
+
+[[package]]
 name = "syntect"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6c454c27d9d7d9a84c7803aaa3c50cd088d2906fe3c6e42da3209aa623576a8"
 dependencies = [
  "bincode",
  "bitflags 1.3.2",
@@ -1210,15 +1430,42 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "time"
+version = "0.3.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+dependencies = [
+ "itoa",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+dependencies = [
+ "time-core",
 ]
 
 [[package]]
 name = "tiny-skia"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce2986c82f77818c7b9144c70818fdde98db15308e329ae2f7204d767808fd3c"
@@ -1246,14 +1493,16 @@
 [[package]]
 name = "tinystr"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ac3f5b6856e931e15e07b478e98c8045239829a65f9156d4fa7e7788197a5ef"
 dependencies = [
  "displaydoc",
+ "serde",
+ "zerovec",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1286,17 +1535,17 @@
 checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.9"
+version = "0.19.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d964908cec0d030b812013af25a0e57fddfadb1e066ecc6681d86253129d4f"
+checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
@@ -1317,15 +1566,15 @@
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -1343,16 +1592,16 @@
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typst"
-version = "0.4.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.4.0#f692a5efc62bf95f57d123895b7dce55d2eb9741"
+version = "0.5.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.5.0#3a8b9cce471934031ba57c5972d194ac1d7d2a6c"
 dependencies = [
  "bitflags 2.3.1",
  "bytemuck",
  "comemo",
  "ecow",
  "flate2",
  "fontdb",
@@ -1369,14 +1618,15 @@
  "roxmltree",
  "rustybuzz",
  "serde",
  "siphasher",
  "stacker",
  "subsetter",
  "svg2pdf",
+ "time",
  "tiny-skia",
  "tracing",
  "ttf-parser",
  "typst-macros",
  "unicode-general-category",
  "unicode-ident",
  "unicode-math-class",
@@ -1384,66 +1634,71 @@
  "unscanny",
  "usvg",
  "xmp-writer",
 ]
 
 [[package]]
 name = "typst-library"
-version = "0.4.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.4.0#f692a5efc62bf95f57d123895b7dce55d2eb9741"
+version = "0.5.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.5.0#3a8b9cce471934031ba57c5972d194ac1d7d2a6c"
 dependencies = [
  "az",
  "chinese-number",
  "comemo",
  "csv",
  "ecow",
  "hayagriva",
  "hypher",
+ "icu_properties",
+ "icu_provider",
+ "icu_provider_adapters",
+ "icu_provider_blob",
+ "icu_segmenter",
  "kurbo",
  "lipsum",
  "log",
  "once_cell",
  "roxmltree",
  "rustybuzz",
  "serde_json",
  "serde_yaml",
  "smallvec",
  "syntect",
+ "time",
  "toml",
  "tracing",
  "ttf-parser",
  "typed-arena",
  "typst",
  "unicode-bidi",
  "unicode-math-class",
  "unicode-script",
  "unicode-segmentation",
- "xi-unicode",
 ]
 
 [[package]]
 name = "typst-macros"
-version = "0.4.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.4.0#f692a5efc62bf95f57d123895b7dce55d2eb9741"
+version = "0.5.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.5.0#3a8b9cce471934031ba57c5972d194ac1d7d2a6c"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "typst-py"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
+ "chrono",
  "comemo",
  "dirs",
  "elsa",
- "memmap2 0.6.1",
- "once_cell",
+ "memmap2 0.6.2",
  "pyo3",
  "same-file",
  "siphasher",
  "typst",
  "typst-library",
  "walkdir",
 ]
@@ -1488,17 +1743,17 @@
 name = "unicode-general-category"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2281c8c1d221438e373249e065ca4989c4c36952c211ff21a0ee91c44a3869e7"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-math-class"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d246cf599d5fae3c8d56e04b20eb519adb89a8af8d0b0fbcded369aa3647d65"
 
@@ -1526,30 +1781,36 @@
 [[package]]
 name = "unicode-vo"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1d386ff53b415b7fe27b50bb44679e2cc4660272694b7b6f3326d8480823a94"
 
 [[package]]
+name = "unicode-xid"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "unscanny"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9df2af067a7953e9c3831320f35c1cc0600c30d44d9f7a12b01db1cd88d6b47"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
@@ -1609,14 +1870,20 @@
  "kurbo",
  "rctree",
  "strict-num",
  "svgtypes",
 ]
 
 [[package]]
+name = "utf8_iter"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "64a8922555b9500e3d865caed19330172cd67cbf82203f1a3311d8c305cc9f33"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
@@ -1631,14 +1898,68 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+
+[[package]]
 name = "weezl"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
 
 [[package]]
 name = "winapi"
@@ -1668,159 +1989,102 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
+name = "windows"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "xi-unicode"
-version = "0.3.0"
+name = "writeable"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a67300977d3dc3f8034dae89778f502b6ba20b269527b3223ba59c0cf393bb8a"
+checksum = "60e49e42bdb1d5dc76f4cd78102f8f0714d32edfa3efb82286eb0f0b1fc0da0f"
 
 [[package]]
 name = "xmlparser"
 version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
 
@@ -1840,7 +2104,76 @@
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
+
+[[package]]
+name = "yoke"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1848075a23a28f9773498ee9a0f2cf58fcbad4f8c0ccf84a210ab33c6ae495de"
+dependencies = [
+ "serde",
+ "stable_deref_trait",
+ "yoke-derive",
+ "zerofrom",
+]
+
+[[package]]
+name = "yoke-derive"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af46c169923ed7516eef0aa32b56d2651b229f57458ebe46b49ddd6efef5b7a2"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "synstructure",
+]
+
+[[package]]
+name = "zerofrom"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df54d76c3251de27615dfcce21e636c172dafb2549cd7fd93e21c66f6ca6bea2"
+dependencies = [
+ "zerofrom-derive",
+]
+
+[[package]]
+name = "zerofrom-derive"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4eae7c1f7d4b8eafce526bc0771449ddc2f250881ae31c50d22c032b5a1c499"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "synstructure",
+]
+
+[[package]]
+name = "zerovec"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "198f54134cd865f437820aa3b43d0ad518af4e68ee161b444cdd15d8e567c8ea"
+dependencies = [
+ "serde",
+ "yoke",
+ "zerofrom",
+ "zerovec-derive",
+]
+
+[[package]]
+name = "zerovec-derive"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "486558732d5dde10d0f8cb2936507c1bb21bc539d924c949baf5f36a58e51bac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "synstructure",
+]
```

### Comparing `typst-0.4.0/PKG-INFO` & `typst-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python binding to typst
 License: Apache-2.0
 Requires-Python: >=3.7
```

