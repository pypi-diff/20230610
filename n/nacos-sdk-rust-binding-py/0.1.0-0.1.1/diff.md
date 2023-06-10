# Comparing `tmp/nacos_sdk_rust_binding_py-0.1.0.tar.gz` & `tmp/nacos_sdk_rust_binding_py-0.1.1.tar.gz`

## Comparing `nacos_sdk_rust_binding_py-0.1.0.tar` & `nacos_sdk_rust_binding_py-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      519 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/.gitignore
--rw-r--r--   0     1001      123    11357 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/LICENSE
--rw-r--r--   0     1001      123      896 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/README.md
--rw-r--r--   0     1001      123       10 2023-06-10 06:04:45.000000 nacos_sdk_rust_binding_py-0.1.0/dist/nacos_sdk_rust_binding_py-0.1.0.tar.gz
--rw-r--r--   0     1001      123      862 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     5677 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/src/config.rs
--rw-r--r--   0     1001      123     2131 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123    10077 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/src/naming.rs
--rw-r--r--   0     1001      123      230 2023-06-10 06:02:50.000000 nacos_sdk_rust_binding_py-0.1.0/test.sh
--rw-r--r--   0     1001      123    38648 2023-06-10 06:04:43.000000 nacos_sdk_rust_binding_py-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      519 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/LICENSE
+-rw-r--r--   0     1001      123      953 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/README.md
+-rw-r--r--   0     1001      123       10 2023-06-10 17:02:38.000000 nacos_sdk_rust_binding_py-0.1.1/dist/nacos_sdk_rust_binding_py-0.1.1.tar.gz
+-rw-r--r--   0     1001      123      947 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/examples/config.py
+-rw-r--r--   0     1001      123      612 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/examples/naming.py
+-rw-r--r--   0     1001      123      856 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     5779 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/src/config.rs
+-rw-r--r--   0     1001      123     2647 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123    10978 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/src/naming.rs
+-rw-r--r--   0     1001      123      230 2023-06-10 17:00:21.000000 nacos_sdk_rust_binding_py-0.1.1/test.sh
+-rw-r--r--   0     1001      123    38648 2023-06-10 17:02:35.000000 nacos_sdk_rust_binding_py-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1881 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.1.1/PKG-INFO
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/Cargo.toml` & `nacos_sdk_rust_binding_py-0.1.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nacos-sdk-rust-binding-py"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 license = "Apache-2.0"
 publish = false
 authors = ["CheirshCai <785427346@qq.com>"]
 readme = "README.md"
 repository = "https://github.com/opc-source/nacos-sdk-rust-binding-py.git"
 description = "nacos-sdk-rust binding for Python with PyO3."
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/.github/workflows/CI.yml` & `nacos_sdk_rust_binding_py-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.0/.gitignore` & `nacos_sdk_rust_binding_py-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.0/LICENSE` & `nacos_sdk_rust_binding_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.0/README.md` & `nacos_sdk_rust_binding_py-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 nacos-sdk-rust binding for Python with PyO3.
 
 Tip: nacos-sdk-python 仓库暂未提供 2.x gRPC 交互模式，为了能升级它，故而通过 ffi 方式调用 nacos-sdk-rust
 
 ## Installation
 
 ```bash
-pip install nacos_sdk_rust_binding_py
+pip install nacos-sdk-rust-binding-py
 ```
 
 # Usage
+- see https://pypi.org/project/nacos-sdk-rust-binding-py
 - TODO
 
 ## Development
 
 Setup virtualenv:
 
 ```shell
@@ -45,15 +46,15 @@
 behave tests
 ```
 
 Build API docs:
 
 ```shell
 maturin develop -E docs
-pdoc nacos_sdk_rust_binding_py
+pdoc nacos-sdk-rust-binding-py
 ```
 
 # License
 [Apache License Version 2.0](LICENSE)
 
 # Acknowledgement
 - binding for Python with [PyO3](https://github.com/PyO3/pyo3.git)
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/pyproject.toml` & `nacos_sdk_rust_binding_py-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 readme = "README.md"
 
 [project.optional-dependencies]
 docs = ["pdoc"]
 test = ["behave"]
 
 [project.urls]
-Documentation = "https://github.com/opc-source/nacos-sdk-rust-binding-node.git"
-Homepage = "https://github.com/opc-source/nacos-sdk-rust-binding-node.git"
-Repository = "https://github.com/opc-source/nacos-sdk-rust-binding-node.git"
+Documentation = "https://github.com/opc-source/nacos-sdk-rust-binding-py.git"
+Homepage = "https://github.com/opc-source/nacos-sdk-rust-binding-py.git"
+Repository = "https://github.com/opc-source/nacos-sdk-rust-binding-py.git"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/src/config.rs` & `nacos_sdk_rust_binding_py-0.1.1/src/config.rs`

 * *Files 2% similar despite different names*

```diff
@@ -132,24 +132,30 @@
         Ok(())
     }
 }
 
 #[pyclass]
 pub struct NacosConfigResponse {
     /// Namespace/Tenant
+    #[pyo3(get)]
     pub namespace: String,
     /// DataId
+    #[pyo3(get)]
     pub data_id: String,
     /// Group
+    #[pyo3(get)]
     pub group: String,
     /// Content
+    #[pyo3(get)]
     pub content: String,
     /// Content's Type; e.g. json,properties,xml,html,text,yaml
+    #[pyo3(get)]
     pub content_type: String,
     /// Content's md5
+    #[pyo3(get)]
     pub md5: String,
 }
 
 /*
 pub struct NacosConfigChangeListener {
     func: Arc<PyFunction>,
 }
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/src/lib.rs` & `nacos_sdk_rust_binding_py-0.1.1/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -52,23 +52,48 @@
     &LOG_GUARD
 }
 
 #[pyclass]
 #[derive(Clone)]
 pub struct ClientOptions {
     /// Server Addr, e.g. address:port[,address:port],...]
+    #[pyo3(set, get)]
     pub server_addr: String,
     /// Namespace/Tenant
+    #[pyo3(set, get)]
     pub namespace: String,
     /// AppName
+    #[pyo3(set, get)]
     pub app_name: Option<String>,
     /// Username for Auth
+    #[pyo3(set, get)]
     pub username: Option<String>,
     /// Password for Auth
+    #[pyo3(set, get)]
     pub password: Option<String>,
 }
 
+#[pymethods]
+impl ClientOptions {
+    #[new]
+    pub fn new(
+        server_addr: String,
+        namespace: String,
+        app_name: Option<String>,
+        username: Option<String>,
+        password: Option<String>,
+    ) -> PyResult<ClientOptions> {
+        Ok(Self {
+            server_addr,
+            namespace,
+            app_name,
+            username,
+            password,
+        })
+    }
+}
+
 mod config;
 pub use config::*;
 
 mod naming;
 pub use naming::*;
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/src/naming.rs` & `nacos_sdk_rust_binding_py-0.1.1/src/naming.rs`

 * *Files 6% similar despite different names*

```diff
@@ -248,35 +248,75 @@
 }
 */
 
 #[pyclass]
 #[derive(Clone)]
 pub struct NacosServiceInstance {
     /// Instance Id
+    #[pyo3(set, get)]
     pub instance_id: Option<String>,
     /// Ip
+    #[pyo3(set, get)]
     pub ip: String,
     /// Port
+    #[pyo3(set, get)]
     pub port: i32,
     /// Weight, default 1.0
+    #[pyo3(set, get)]
     pub weight: Option<f64>,
     /// Healthy or not, default true
+    #[pyo3(set, get)]
     pub healthy: Option<bool>,
     /// Enabled ot not, default true
+    #[pyo3(set, get)]
     pub enabled: Option<bool>,
     /// Ephemeral or not, default true
+    #[pyo3(set, get)]
     pub ephemeral: Option<bool>,
     /// Cluster Name, default 'DEFAULT'
+    #[pyo3(set, get)]
     pub cluster_name: Option<String>,
     /// Service Name
+    #[pyo3(set, get)]
     pub service_name: Option<String>,
     /// Metadata, default '{}'
+    #[pyo3(set, get)]
     pub metadata: Option<std::collections::HashMap<String, String>>,
 }
 
+#[pymethods]
+impl NacosServiceInstance {
+    #[new]
+    pub fn new(
+        ip: String,
+        port: i32,
+        weight: Option<f64>,
+        healthy: Option<bool>,
+        enabled: Option<bool>,
+        ephemeral: Option<bool>,
+        cluster_name: Option<String>,
+        service_name: Option<String>,
+        metadata: Option<std::collections::HashMap<String, String>>,
+    ) -> PyResult<NacosServiceInstance> {
+        Ok(Self {
+            instance_id: None,
+            ip,
+            port,
+            weight,
+            healthy,
+            enabled,
+            ephemeral,
+            cluster_name,
+            service_name,
+            metadata,
+        })
+    }
+}
+
+
 fn transfer_ffi_instance_to_rust(
     ffi_instance: &NacosServiceInstance,
 ) -> nacos_sdk::api::naming::ServiceInstance {
     nacos_sdk::api::naming::ServiceInstance {
         instance_id: ffi_instance.instance_id.clone(),
         ip: ffi_instance.ip.clone(),
         port: ffi_instance.port,
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/Cargo.lock` & `nacos_sdk_rust_binding_py-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
  "tower",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "nacos-sdk-rust-binding-py"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "lazy_static",
  "nacos-sdk",
  "pyo3",
  "tracing-appender",
  "tracing-subscriber",
 ]
```

### Comparing `nacos_sdk_rust_binding_py-0.1.0/PKG-INFO` & `nacos_sdk_rust_binding_py-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacos-sdk-rust-binding-py
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc ; extra == 'docs'
 Requires-Dist: behave ; extra == 'test'
 Provides-Extra: docs
 Provides-Extra: test
@@ -12,30 +12,31 @@
 Summary: nacos-sdk-rust binding for Python.
 Keywords: nacos,ffi,pyo3,binding,python
 Author: CheirshCai <785427346@qq.com>
 Author-email: CheirshCai <785427346@qq.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://github.com/opc-source/nacos-sdk-rust-binding-node.git
-Project-URL: Homepage, https://github.com/opc-source/nacos-sdk-rust-binding-node.git
-Project-URL: Repository, https://github.com/opc-source/nacos-sdk-rust-binding-node.git
+Project-URL: Documentation, https://github.com/opc-source/nacos-sdk-rust-binding-py.git
+Project-URL: Homepage, https://github.com/opc-source/nacos-sdk-rust-binding-py.git
+Project-URL: Repository, https://github.com/opc-source/nacos-sdk-rust-binding-py.git
 
 # nacos-sdk-rust-binding-py
 nacos-sdk-rust binding for Python with PyO3.
 
 Tip: nacos-sdk-python 仓库暂未提供 2.x gRPC 交互模式，为了能升级它，故而通过 ffi 方式调用 nacos-sdk-rust
 
 ## Installation
 
 ```bash
-pip install nacos_sdk_rust_binding_py
+pip install nacos-sdk-rust-binding-py
 ```
 
 # Usage
+- see https://pypi.org/project/nacos-sdk-rust-binding-py
 - TODO
 
 ## Development
 
 Setup virtualenv:
 
 ```shell
@@ -67,15 +68,15 @@
 behave tests
 ```
 
 Build API docs:
 
 ```shell
 maturin develop -E docs
-pdoc nacos_sdk_rust_binding_py
+pdoc nacos-sdk-rust-binding-py
 ```
 
 # License
 [Apache License Version 2.0](LICENSE)
 
 # Acknowledgement
 - binding for Python with [PyO3](https://github.com/PyO3/pyo3.git)
```

