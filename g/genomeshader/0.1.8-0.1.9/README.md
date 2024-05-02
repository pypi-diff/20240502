# Comparing `tmp/genomeshader-0.1.8.tar.gz` & `tmp/genomeshader-0.1.9.tar.gz`

## Comparing `genomeshader-0.1.8.tar` & `genomeshader-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 genomeshader-0.1.8/Cargo.toml
--rw-r--r--   0     1001      127      424 2024-01-14 22:40:06.000000 genomeshader-0.1.8/.bumpversion.cfg
--rw-r--r--   0     1001      127     6583 2024-01-14 22:40:06.000000 genomeshader-0.1.8/.github/workflows/release.yml
--rw-r--r--   0     1001      127      140 2024-01-14 22:40:06.000000 genomeshader-0.1.8/.gitignore
--rw-r--r--   0     1001      127     1523 2024-01-14 22:40:06.000000 genomeshader-0.1.8/LICENSE
--rw-r--r--   0     1001      127     1794 2024-01-14 22:40:06.000000 genomeshader-0.1.8/README.rst
--rw-r--r--   0     1001      127       15 2024-01-14 22:40:06.000000 genomeshader-0.1.8/VERSION
--rw-r--r--   0     1001      127   102538 2024-01-14 22:40:06.000000 genomeshader-0.1.8/playground.ipynb
--rw-r--r--   0     1001      127      194 2024-01-14 22:40:06.000000 genomeshader-0.1.8/python/genomeshader/__init__.py
--rw-r--r--   0     1001      127     7987 2024-01-14 22:40:06.000000 genomeshader-0.1.8/python/genomeshader/view.py
--rw-r--r--   0     1001      127      611 2024-01-14 22:40:06.000000 genomeshader-0.1.8/requirements.txt
--rw-r--r--   0     1001      127    13404 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/alignment.rs
--rw-r--r--   0     1001      127     3780 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/app.rs
--rw-r--r--   0     1001      127     4021 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/events.rs
--rw-r--r--   0     1001      127     8118 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/layout.rs
--rw-r--r--   0     1001      127     6106 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/lib.rs
--rw-r--r--   0     1001      127     1821 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/storage.rs
--rw-r--r--   0     1001      127     1829 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/styles.rs
--rwxr-xr-x   0     1001      127     1053 2024-01-14 22:40:06.000000 genomeshader-0.1.8/src/tests/make_test_read.sh
--rw-r--r--   0     1001      127   155802 2024-01-14 22:40:13.000000 genomeshader-0.1.8/Cargo.lock
--rw-r--r--   0     1001      127      357 2024-01-14 22:40:06.000000 genomeshader-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 genomeshader-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 genomeshader-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      127      424 2024-01-15 01:20:57.000000 genomeshader-0.1.9/.bumpversion.cfg
+-rw-r--r--   0     1001      127     6583 2024-01-15 01:20:57.000000 genomeshader-0.1.9/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      140 2024-01-15 01:20:57.000000 genomeshader-0.1.9/.gitignore
+-rw-r--r--   0     1001      127     1523 2024-01-15 01:20:57.000000 genomeshader-0.1.9/LICENSE
+-rw-r--r--   0     1001      127     1794 2024-01-15 01:20:57.000000 genomeshader-0.1.9/README.rst
+-rw-r--r--   0     1001      127       15 2024-01-15 01:20:57.000000 genomeshader-0.1.9/VERSION
+-rw-r--r--   0     1001      127   102538 2024-01-15 01:20:57.000000 genomeshader-0.1.9/playground.ipynb
+-rw-r--r--   0     1001      127      194 2024-01-15 01:20:57.000000 genomeshader-0.1.9/python/genomeshader/__init__.py
+-rw-r--r--   0     1001      127     7987 2024-01-15 01:20:57.000000 genomeshader-0.1.9/python/genomeshader/view.py
+-rw-r--r--   0     1001      127      611 2024-01-15 01:20:57.000000 genomeshader-0.1.9/requirements.txt
+-rw-r--r--   0     1001      127    13404 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/alignment.rs
+-rw-r--r--   0     1001      127     3780 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/app.rs
+-rw-r--r--   0     1001      127     4021 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/events.rs
+-rw-r--r--   0     1001      127     8118 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/layout.rs
+-rw-r--r--   0     1001      127     6106 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      127     1821 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/storage.rs
+-rw-r--r--   0     1001      127     1829 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/styles.rs
+-rwxr-xr-x   0     1001      127     1053 2024-01-15 01:20:57.000000 genomeshader-0.1.9/src/tests/make_test_read.sh
+-rw-r--r--   0     1001      127   155813 2024-01-15 01:21:04.000000 genomeshader-0.1.9/Cargo.lock
+-rw-r--r--   0     1001      127      357 2024-01-15 01:20:57.000000 genomeshader-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 genomeshader-0.1.9/PKG-INFO
```

### Comparing `genomeshader-0.1.8/Cargo.toml` & `genomeshader-0.1.9/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "genomeshader"
-version = "0.1.8"
+version = "0.1.9"
 authors = ["Kiran V Garimella <kiran@broadinstitute.org>"]
 edition = "2021"
 license = "BSD 3-Clause"
 license-file = "LICENSE"
 readme = "README.rst"
 homepage = "https://github.com/broadinstitute/genomeshader"
 repository = "https://github.com/broadinstitute/genomeshader.git"
@@ -14,14 +14,15 @@
 [lib]
 name = "genomeshader"
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0"
 cloud-storage = { version = "*", features = ["sync"] }
+crossbeam-utils = "0.8.19"
 egui = "0.23.0"
 eframe = "*"
 fs_extra = "1.2"
 google-cloud-storage = "*"
 glob = "0.3"
 indicatif = { version = "*", features = ["rayon"] }
 lazy_static = "*"
@@ -29,14 +30,15 @@
 nannou_egui = { git = "https://github.com/tychedelia/nannou.git" }
 openssl = { version = "0.10", features = ["vendored"] }
 polars = { version = "*", features = ["performant", "parquet", "dtype-categorical", "fmt", "rows"] }
 pollster = "0.3"
 pyo3 = { version = "*", features = ["abi3-py37", "extension-module"] }
 pyo3-polars = "*"
 pyo3-asyncio = { version = "*", features = ["attributes", "async-std-runtime", "tokio-runtime"] }
+memoffset = "0.9.0"
 ndarray = { version = "0.15.6", features = ["rayon"] }
 rand = "*"
 rayon = "*"
 regex = "*"
 rust-htslib = { version = "*", features = ["gcs"] }
 sprs = "0.11.1"
 sys-info = "0.9.1"
```

### Comparing `genomeshader-0.1.8/.github/workflows/release.yml` & `genomeshader-0.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/LICENSE` & `genomeshader-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/README.rst` & `genomeshader-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/playground.ipynb` & `genomeshader-0.1.9/playground.ipynb`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/python/genomeshader/view.py` & `genomeshader-0.1.9/python/genomeshader/view.py`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/requirements.txt` & `genomeshader-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/alignment.rs` & `genomeshader-0.1.9/src/alignment.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/app.rs` & `genomeshader-0.1.9/src/app.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/events.rs` & `genomeshader-0.1.9/src/events.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/layout.rs` & `genomeshader-0.1.9/src/layout.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/lib.rs` & `genomeshader-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/storage.rs` & `genomeshader-0.1.9/src/storage.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/styles.rs` & `genomeshader-0.1.9/src/styles.rs`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/src/tests/make_test_read.sh` & `genomeshader-0.1.9/src/tests/make_test_read.sh`

 * *Files identical despite different names*

### Comparing `genomeshader-0.1.8/Cargo.lock` & `genomeshader-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
 checksum = "62565bb4402e926b29953c785397c6dc0391b7b446e45008b0049eb43cec6f5d"
 dependencies = [
  "async-channel 1.9.0",
  "async-global-executor",
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-process",
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-lite 1.13.0",
  "gloo-timers",
  "kv-log-macro",
  "log",
@@ -975,15 +975,15 @@
 
 [[package]]
 name = "concurrent-queue"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
 dependencies = [
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
 ]
 
 [[package]]
 name = "console"
 version = "0.15.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
@@ -1062,15 +1062,15 @@
 [[package]]
 name = "crossbeam-channel"
 version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82a9b73a36529d9c47029b9fb3a6f0ea3cc916a261195352ba19e770fc1748b2"
 dependencies = [
  "cfg-if 1.0.0",
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20ff29ded3204c5106278a81a38f4b482636ed4fa1e6cfbeef193291beb29ed"
@@ -1084,15 +1084,15 @@
 name = "crossbeam-deque"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fca89a0e215bab21874660c67903c5f143333cab1da83d041c7ded6053774751"
 dependencies = [
  "cfg-if 1.0.0",
  "crossbeam-epoch 0.9.17",
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "058ed274caafc1f60c4997b5fc07bf7dc7cca454af7c6e81edffe5f33f70dace"
@@ -1110,25 +1110,25 @@
 name = "crossbeam-epoch"
 version = "0.9.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e3681d554572a651dda4186cd47240627c3d0114d45a95f6ad27f2f22e7548d"
 dependencies = [
  "autocfg",
  "cfg-if 1.0.0",
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
 ]
 
 [[package]]
 name = "crossbeam-queue"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adc6598521bb5a83d491e8c1fe51db7296019d2ca3cb93cc6c2a20369a4d78a2"
 dependencies = [
  "cfg-if 1.0.0",
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3c7c73a2d1e9fc0886a08b93e98eb643461230d5f1925e4036204d5f2e261a8"
@@ -1136,20 +1136,17 @@
  "autocfg",
  "cfg-if 0.1.10",
  "lazy_static",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.18"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3a430a770ebd84726f584a90ee7f020d28db52c6d02138900f22341f866d39c"
-dependencies = [
- "cfg-if 1.0.0",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "crossterm"
 version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f476fe445d41c9e991fd07515a6f463074b782242ccf4a5b7b1d1012e70824df"
 dependencies = [
@@ -1827,26 +1824,28 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "genomeshader"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "anyhow",
  "async-std",
  "cloud-storage",
+ "crossbeam-utils 0.8.19",
  "eframe",
  "egui",
  "fs_extra",
  "glob",
  "google-cloud-storage",
  "indicatif",
  "lazy_static",
+ "memoffset 0.9.0",
  "nannou",
  "nannou_egui",
  "ndarray",
  "openssl",
  "polars",
  "pollster",
  "pyo3",
@@ -4318,15 +4317,15 @@
 [[package]]
 name = "rayon-core"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ce3fb6ad83f861aac485e76e1985cd109d9a3713802152be56c3b1f0e0658ed"
 dependencies = [
  "crossbeam-deque 0.8.4",
- "crossbeam-utils 0.8.18",
+ "crossbeam-utils 0.8.19",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
```

### Comparing `genomeshader-0.1.8/PKG-INFO` & `genomeshader-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomeshader
-Version: 0.1.8
+Version: 0.1.9
 Requires-Dist: polars
 Requires-Dist: holoviews
 Requires-Dist: datashader
 License-File: LICENSE
 Summary: Fast visualization of genomic data
 Home-Page: https://github.com/broadinstitute/genomeshader
 Author: Kiran V Garimella <kiran@broadinstitute.org>
```

