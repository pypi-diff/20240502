# Comparing `tmp/servicing-0.0.8.tar.gz` & `tmp/servicing-0.0.9.tar.gz`

## Comparing `servicing-0.0.8.tar` & `servicing-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 servicing-0.0.8/Cargo.toml
--rw-r--r--   0     1001      127     3958 2024-05-01 16:09:52.000000 servicing-0.0.8/.github/workflows/cicd.yml
--rw-r--r--   0     1001      127      686 2024-05-01 16:09:52.000000 servicing-0.0.8/.gitignore
--rw-r--r--   0     1001      127      165 2024-05-01 16:09:52.000000 servicing-0.0.8/.vimspector.json
--rw-r--r--   0     1001      127      693 2024-05-01 16:09:52.000000 servicing-0.0.8/README.md
--rw-r--r--   0     1001      127      271 2024-05-01 16:09:52.000000 servicing-0.0.8/build.rs
--rw-r--r--   0     1001      127     3432 2024-05-01 16:09:52.000000 servicing-0.0.8/servicing.pyi
--rw-r--r--   0     1001      127    18688 2024-05-01 16:09:52.000000 servicing-0.0.8/src/dispatcher/mod.rs
--rw-r--r--   0     1001      127     1455 2024-05-01 16:09:52.000000 servicing-0.0.8/src/error/mod.rs
--rw-r--r--   0     1001      127     5892 2024-05-01 16:09:52.000000 servicing-0.0.8/src/helper/mod.rs
--rw-r--r--   0     1001      127      637 2024-05-01 16:09:52.000000 servicing-0.0.8/src/lib.rs
--rw-r--r--   0     1001      127     4284 2024-05-01 16:09:52.000000 servicing-0.0.8/src/models/mod.rs
--rw-r--r--   0     1001      127      302 2024-05-01 16:09:52.000000 servicing-0.0.8/template/service.yaml
--rw-r--r--   0     1001      127    43004 2024-05-01 16:09:52.000000 servicing-0.0.8/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-05-01 16:09:52.000000 servicing-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 servicing-0.0.9/Cargo.toml
+-rw-r--r--   0     1001      127     3958 2024-05-02 03:24:14.000000 servicing-0.0.9/.github/workflows/cicd.yml
+-rw-r--r--   0     1001      127      686 2024-05-02 03:24:14.000000 servicing-0.0.9/.gitignore
+-rw-r--r--   0     1001      127      165 2024-05-02 03:24:14.000000 servicing-0.0.9/.vimspector.json
+-rw-r--r--   0     1001      127      693 2024-05-02 03:24:14.000000 servicing-0.0.9/README.md
+-rw-r--r--   0     1001      127      271 2024-05-02 03:24:14.000000 servicing-0.0.9/build.rs
+-rw-r--r--   0     1001      127     3432 2024-05-02 03:24:14.000000 servicing-0.0.9/servicing.pyi
+-rw-r--r--   0     1001      127    18688 2024-05-02 03:24:14.000000 servicing-0.0.9/src/dispatcher/mod.rs
+-rw-r--r--   0     1001      127     1455 2024-05-02 03:24:14.000000 servicing-0.0.9/src/error/mod.rs
+-rw-r--r--   0     1001      127     5892 2024-05-02 03:24:14.000000 servicing-0.0.9/src/helper/mod.rs
+-rw-r--r--   0     1001      127      637 2024-05-02 03:24:14.000000 servicing-0.0.9/src/lib.rs
+-rw-r--r--   0     1001      127     4977 2024-05-02 03:24:14.000000 servicing-0.0.9/src/models/mod.rs
+-rw-r--r--   0     1001      127      302 2024-05-02 03:24:14.000000 servicing-0.0.9/template/service.yaml
+-rw-r--r--   0     1001      127    43004 2024-05-02 03:24:14.000000 servicing-0.0.9/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-05-02 03:24:14.000000 servicing-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.9/PKG-INFO
```

### Comparing `servicing-0.0.8/Cargo.toml` & `servicing-0.0.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "servicing"
-version = "0.0.8"
+version = "0.0.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "servicing"
 crate-type = ["cdylib"]
```

### Comparing `servicing-0.0.8/.github/workflows/cicd.yml` & `servicing-0.0.9/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/.gitignore` & `servicing-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/README.md` & `servicing-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/servicing.pyi` & `servicing-0.0.9/servicing.pyi`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/src/dispatcher/mod.rs` & `servicing-0.0.9/src/dispatcher/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/src/error/mod.rs` & `servicing-0.0.9/src/error/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/src/helper/mod.rs` & `servicing-0.0.9/src/helper/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/src/lib.rs` & `servicing-0.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.8/src/models/mod.rs` & `servicing-0.0.9/src/models/mod.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use pyo3::{pyclass, pymethods};
-use serde::{Deserialize, Serialize};
+use serde::{ser::SerializeStruct, Deserialize, Serialize};
 
 #[pyclass]
 #[derive(Clone, Serialize, Deserialize, Debug)]
 pub struct UserProvidedConfig {
     pub port: Option<u16>,
     pub replicas: Option<u16>,
     pub cloud: Option<String>,
@@ -98,25 +98,44 @@
 
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Service {
     pub readiness_probe: String,
     pub replicas: u16,
 }
 
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Deserialize, Debug)]
 pub struct Resources {
     pub ports: u16,
     pub cloud: String,
     pub cpus: String,
     pub memory: String,
     pub disk_size: u16,
-    #[serde(skip_serializing_if = "Option::is_none")]
     pub accelerators: Option<String>,
 }
 
+impl Serialize for Resources {
+    fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
+    where
+        S: serde::ser::Serializer,
+    {
+        let should_serialize = self.accelerators.is_some() || !serializer.is_human_readable();
+
+        let mut stats = serializer.serialize_struct("Resources", 6)?;
+        stats.serialize_field("ports", &self.ports)?;
+        stats.serialize_field("cloud", &self.cloud)?;
+        stats.serialize_field("cpus", &self.cpus)?;
+        stats.serialize_field("memory", &self.memory)?;
+        stats.serialize_field("disk_size", &self.disk_size)?;
+        if should_serialize {
+            stats.serialize_field("accelerators", &self.accelerators)?;
+        }
+        stats.end()
+    }
+}
+
 impl Default for Configuration {
     fn default() -> Self {
         Configuration {
             service: Service {
                 readiness_probe: "/health".to_string(),
                 replicas: 2,
             },
```

### Comparing `servicing-0.0.8/Cargo.lock` & `servicing-0.0.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1065,26 +1065,26 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1121,15 +1121,15 @@
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "servicing"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "base64",
  "bincode",
  "dirs",
  "env_logger",
  "futures",
  "log",
```

### Comparing `servicing-0.0.8/PKG-INFO` & `servicing-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: servicing
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
```

