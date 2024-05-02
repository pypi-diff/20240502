# Comparing `tmp/pyreqwest_impersonate-0.3.2.tar.gz` & `tmp/pyreqwest_impersonate-0.4.0.tar.gz`

## Comparing `pyreqwest_impersonate-0.3.2.tar` & `pyreqwest_impersonate-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.2/Cargo.toml
--rw-r--r--   0     1001      127     4854 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/.gitignore
--rw-r--r--   0     1001      127     7808 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/README.md
--rw-r--r--   0     1001      127      273 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/1_threads.csv
--rw-r--r--   0     1001      127      273 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/4_threads.csv
--rw-r--r--   0     1001      127      343 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/README.md
--rw-r--r--   0     1001      127     3299 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/benchmark.py
--rw-r--r--   0     1001      127       83 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/requirements.txt
--rw-r--r--   0     1001      127      799 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/server.py
--rw-r--r--   0     1001      127    23737 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/src/lib.rs
--rw-r--r--   0     1001      127     3033 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/src/response.rs
--rw-r--r--   0     1001      127     3830 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/tests/test_client.py
--rw-r--r--   0     1001      127     5370 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/tests/test_defs.py
--rw-r--r--   0     1001      127    41944 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      127     6070 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      766 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/.gitignore
+-rw-r--r--   0     1001      127     7404 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/README.md
+-rw-r--r--   0     1001      127      343 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/benchmark/README.md
+-rw-r--r--   0     1001      127     3484 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3188 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/benchmark/generate_image.py
+-rw-r--r--   0     1001      127       94 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      990 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/benchmark/server.py
+-rw-r--r--   0     1001      127    26340 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/src/response.rs
+-rw-r--r--   0     1001      127     3830 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/tests/test_client.py
+-rw-r--r--   0     1001      127     5370 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/tests/test_defs.py
+-rw-r--r--   0     1001      127    42920 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-05-02 00:09:01.000000 pyreqwest_impersonate-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8473 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.0/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.3.2/Cargo.toml` & `pyreqwest_impersonate-0.4.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.3.2"
+version = "0.4.0"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pyreqwest_impersonate"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21", features = ["extension-module", "abi3-py38"] }
 reqwest-impersonate = { version = "0.11", default-features = false, features = [
     "cookies",
-    "blocking",
     "boring-tls",
     "impersonate",
     "json",
     "multipart",  # to send a multipart/form-data body
     "socks",
     "gzip",
     "brotli",
     "deflate",
 ] }
 encoding_rs = "0.8"
 pythonize = "0.21"
 serde_json = "1"
+tokio = { version = "1", features = ["fs", "rt-multi-thread"] }
+rayon = "1"
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
 opt-level = 3
 panic = "abort"
 strip = "symbols"
```

### Comparing `pyreqwest_impersonate-0.3.2/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.4.0/.github/workflows/CI.yml`

 * *Files 20% similar despite different names*

```diff
@@ -129,22 +129,22 @@
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.platform.target }}
           path: dist
-      #- name: pytest
-      #  if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
-      #  shell: bash
-      #  run: |
-      #    set -e
-      #    pip install pyreqwest_impersonate --no-index --find-links dist --force-reinstall
-      #    pip install pytest
-      #    pytest
+      - name: pytest
+        if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
+        shell: bash
+        run: |
+          set -e
+          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pytest
+          pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Build sdist
         uses: PyO3/maturin-action@v1
@@ -167,7 +167,40 @@
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --non-interactive --skip-existing wheels-*/*
+
+  benchmark:
+    permissions:
+      contents: write
+    runs-on: ubuntu-latest
+    if: "startsWith(github.ref, 'refs/tags/')"
+    needs: [release]
+    steps:
+      - uses: actions/checkout@v4
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
+      - name: Install dependencies
+        run: |
+          sleep 30  # Wait for the package to be available on PyPI
+          python -m pip install --upgrade pip
+          pip install -r benchmark/requirements.txt
+      - name: Start Uvicorn server
+        run: |
+          uvicorn benchmark.server:app --host 0.0.0.0 --port 8000 &
+          sleep 10
+      - name: Run benchmark
+        run: python benchmark/benchmark.py
+      - name: Generate image and commit
+        run: |
+          python benchmark/generate_image.py
+          git config --global user.name 'GitHub Actions'
+          git config --global user.email 'actions@github.com'
+          git add \*.jpg
+          git commit -m "Update generated image" || echo "No changes to commit"
+          git pull origin benchmark --allow-unrelated-histories || echo "No changes to pull"
+          git push https://${{ secrets.PUSH_TOKEN }}@github.com/${{ github.repository }}
```

### Comparing `pyreqwest_impersonate-0.3.2/.gitignore` & `pyreqwest_impersonate-0.4.0/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -66,7 +66,11 @@
 .idea/
 
 # VSCode
 .vscode/
 
 # Pyenv
 .python-version
+
+# Ignore csv and jpg files in benchmark folder
+benchmark/*.csv
+benchmark/*.jpg
```

### Comparing `pyreqwest_impersonate-0.3.2/README.md` & `pyreqwest_impersonate-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/pyreqwest-impersonate)](https://github.com/deedy5/pyreqwest-impersonate/releases) [![](https://badge.fury.io/py/pyreqwest_impersonate.svg)](https://pypi.org/project/pyreqwest_impersonate) [![Downloads](https://static.pepy.tech/badge/pyreqwest_impersonate/week)](https://pepy.tech/project/pyreqwest_impersonate) [![CI](https://github.com/deedy5/pyreqwest-impersonate/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/deedy5/pyreqwest-impersonate/actions/workflows/CI.yml)
 # Pyreqwest_impersonate
 
 The fastest python HTTP client that can impersonate web browsers by mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints.</br>
-Binding to the Rust `reqwest_impersonate` library.</br>
-🏁 Check the [benchmark](https://github.com/deedy5/pyreqwest_impersonate/tree/main/benchmark) for more details.
-
+Binding to the Rust [reqwest_impersonate](https://github.com/gngpp/reqwest-impersonate) library.</br>
 
 Provides precompiled wheels:
 - [x] Linux:  `amd64`, `aarch64`, `armv7`.
 - [x] Windows: `amd64`.
 - [x] MacOS:  `amd64`, `aarch64`.
 
 ## Table of Contents
@@ -23,19 +21,21 @@
 ## Installation
 
 ```python
 pip install -U pyreqwest_impersonate
 ```
 
 ## Key Features
-- `Impersonate`: The `Client` offers an `impersonate` option, enabling it to mimic web browsers by replicating their headers and `TLS/JA3/JA4/HTTP2` fingerprints. This feature is crucial for avoiding detection as a bot and potential blocking by websites.
-- `Thread-safe`: The `Client` is designed to be thread-safe, allowing it to be safely used in multithreaded environments.
-- `High Performance`: The attributes of the `Response` object are executed in Rust, which is known for its high performance. This ensures that operations like accessing headers, decoding text, or parsing JSON are very fast.
-- `Lazy Execution`: All attributes of the `Response` object are executed lazily. This means that the actual computation or data retrieval happens only when you access the attribute, not when the `Response` object is created.
-- `Automatic Character Encoding Detection`: The `Response` object intelligently detects the character encoding of the response body from the "Content-Type" header. If the encoding is not specified, it defaults to "UTF-8".
+- Impersonate: The Client offers an `impersonate` option, enabling it to mimic web browsers by replicating their headers and TLS/JA3/JA4/HTTP2 fingerprints.
+- Thread-safe: The Client is designed to be thread-safe, allowing it to be safely used in multithreaded environments.
+- Automatic Character Encoding Detection: The encoding is taken from the "Content-Type" header, but if not specified, "UTF-8".
+- Small Size: The compiled library is about 5.8MB in size.
+- High Performance: The library is designed for a large number of threads, uses all processors, and releases the GIL. All operations like accessing headers, decoding text, or parsing JSON are executed in Rust.
+
+![](https://github.com/deedy5/pyreqwest_impersonate/blob/benchmark/benchmark.jpg?raw=true)
 
 ## Usage
 ### I. Client
 
 HTTP client that can impersonate web browsers.
 ```python
 class Client:
@@ -68,30 +68,30 @@
     """
 ```
 
 #### Client Methods
 
 The `Client` class provides a set of methods for making HTTP requests: `get`, `head`, `options`, `delete`, `post`, `put`, `patch`, each of which internally utilizes the `request()` method for execution. The parameters for these methods closely resemble those in `httpx`.
 ```python
-def get(url, *, params=None, headers=None, auth=None, auth_bearer=None, timeout=None):
+def get(url, params=None, headers=None, auth=None, auth_bearer=None, timeout=None):
     """Performs a GET request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password 
             for basic authentication. Default is None.
         auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
         timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 
     """
 ```
 ```python
-def post(url, *, params=None, headers=None, content=None, data=None, files=None, auth=None, auth_bearer=None, timeout=None):
+def post(url, params=None, headers=None, content=None, data=None, files=None, auth=None, auth_bearer=None, timeout=None):
     """Performs a POST request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         content (Optional[bytes]): The content to send in the request body as bytes. Default is None.
@@ -126,14 +126,14 @@
 print(resp.json())
 print(resp.status_code)
 print(resp.text)
 print(resp.url)
 
 # You can also use convenience functions that use a default Client instance under the hood:
 # pri.get() | pri.head() | pri.options() | pri.delete() | pri.post | pri.patch | pri.put
-resp = pri.get("https://httpbin.org/anything") # Default Client does not impersonate a browser
-resp = pri.Client(impersonate="chrome_123").get("https://httpbin.org/anything")  
+# These functions can accept the `impersonate` parameter:
+resp = pri.get("https://httpbin.org/anything", impersonate="chrome_123")  
 ```
 ### II. AsyncClient
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyreqwest_impersonate-0.3.2/benchmark/benchmark.py` & `pyreqwest_impersonate-0.4.0/benchmark/benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,63 +28,64 @@
         s.get(url).text
 
 
 PACKAGES = add_package_version(PACKAGES)
 
 # one thread
 requests_number = 2000
-for response_size in ["5k", "50k"]:
+for response_size in ["5k", "50k", "200k"]:
     url = f"http://127.0.0.1:8000/{response_size}"
     print(f"\nOne worker, {response_size=}, {requests_number=}")
     for name, session_class in PACKAGES:
         start = time.perf_counter()
         cpu_start = time.process_time()
         session_get_test(session_class, requests_number)
-        dur = round(time.perf_counter() - start, 3)
-        cpu_dur = round(time.process_time() - cpu_start, 3)
+        dur = round(time.perf_counter() - start, 2)
+        cpu_dur = round(time.process_time() - cpu_start, 2)
         results.append(
             {
                 "name": name,
                 "threads": 1,
                 "size": response_size,
                 "time": dur,
                 "cpu_time": cpu_dur,
             }
         )
         print(f"    name: {name:<30} time: {dur} cpu_time: {cpu_dur}")
 
 
 # multiple threads
-requests_number = 500
-threads_number = 4
-for response_size in ["5k", "50k"]:
-    url = f"http://127.0.0.1:8000/{response_size}"
-    print(f"\n{threads_number} workers, {response_size=}, {requests_number=}")
-    for name, session_class in PACKAGES:
-        start = time.perf_counter()
-        cpu_start = time.process_time()
-        with ThreadPoolExecutor(threads_number) as executor:
-            futures = [
-                executor.submit(session_get_test, session_class, requests_number)
-                for _ in range(threads_number)
-            ]
-            for f in as_completed(futures):
-                f.result()
-        dur = round(time.perf_counter() - start, 3)
-        cpu_dur = round(time.process_time() - cpu_start, 3)
-        results.append(
-            {
-                "name": name,
-                "threads": threads_number,
-                "size": response_size,
-                "time": dur,
-                "cpu_time": cpu_dur,
-            }
-        )
-        print(f"    name: {name:<30} time: {dur} cpu_time: {cpu_dur}")
+requests_number = 2000
+threads_numbers = [5, 32]
+for threads_number in threads_numbers:
+    for response_size in ["5k", "50k", "200k"]:
+        url = f"http://127.0.0.1:8000/{response_size}"
+        print(f"\n{threads_number} workers, {response_size=}, {requests_number=}")
+        for name, session_class in PACKAGES:
+            start = time.perf_counter()
+            cpu_start = time.process_time()
+            with ThreadPoolExecutor(threads_number) as executor:
+                futures = [
+                    executor.submit(session_get_test, session_class, int(requests_number / threads_number))
+                    for _ in range(threads_number)
+                ]
+                for f in as_completed(futures):
+                    f.result()
+            dur = round(time.perf_counter() - start, 2)
+            cpu_dur = round(time.process_time() - cpu_start, 2)
+            results.append(
+                {
+                    "name": name,
+                    "threads": threads_number,
+                    "size": response_size,
+                    "time": dur,
+                    "cpu_time": cpu_dur,
+                }
+            )
+            print(f"    name: {name:<30} time: {dur} cpu_time: {cpu_dur}")
 
 
 df = pd.DataFrame(results)
 pivot_df = df.pivot_table(
     index=["name", "threads"],
     columns="size",
     values=["time", "cpu_time"],
```

### Comparing `pyreqwest_impersonate-0.3.2/benchmark/server.py` & `pyreqwest_impersonate-0.4.0/benchmark/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,27 @@
 
 random_5k = base64.b64encode(os.urandom(5 * 1024)).decode('utf-8')
 random_5k = gzip.compress(random_5k.encode('utf-8'))
 
 random_50k = base64.b64encode(os.urandom(50 * 1024)).decode('utf-8')
 random_50k = gzip.compress(random_50k.encode('utf-8'))
 
+random_200k = base64.b64encode(os.urandom(200 * 1024)).decode('utf-8')
+random_200k = gzip.compress(random_200k.encode('utf-8'))
+
 
 def gzip_response(gzipped_content):
     headers = {
         'Content-Encoding': 'gzip',
         'Content-Length': str(len(gzipped_content)),
     }
     return Response(gzipped_content, headers=headers)
 
 app = Starlette(
     routes=[
         Route("/5k", lambda r: gzip_response(random_5k)),
         Route("/50k", lambda r: gzip_response(random_50k)),
+        Route("/200k", lambda r: gzip_response(random_200k)),
     ],
 )
 
 # Run server: uvicorn server:app
```

### Comparing `pyreqwest_impersonate-0.3.2/src/lib.rs` & `pyreqwest_impersonate-0.4.0/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,47 @@
 use std::collections::HashMap;
 use std::str::FromStr;
+use std::sync::{mpsc, Arc, OnceLock};
 use std::time::Duration;
 
 use pyo3::exceptions;
 use pyo3::prelude::*;
-use pyo3::types::PyBytes;
-use pyo3::types::{PyDict, PyString};
-use reqwest_impersonate::blocking::multipart;
+use pyo3::types::{PyBytes, PyDict, PyString};
+use rayon::{ThreadPool, ThreadPoolBuilder};
 use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
+use reqwest_impersonate::multipart;
 use reqwest_impersonate::redirect::Policy;
 use reqwest_impersonate::Method;
+use tokio::runtime::{self, Runtime};
 
 mod response;
 use response::Response;
 
+// Rayon global thread pool
+fn cpu_pool() -> &'static ThreadPool {
+    static CPU_POOL: OnceLock<ThreadPool> = OnceLock::new();
+    CPU_POOL.get_or_init(|| ThreadPoolBuilder::new().num_threads(32).build().unwrap())
+}
+
+// Tokio global multi-thread runtime
+fn runtime() -> &'static Runtime {
+    static RUNTIME: OnceLock<Runtime> = OnceLock::new();
+    RUNTIME.get_or_init(|| {
+        runtime::Builder::new_multi_thread()
+            .enable_all()
+            .build()
+            .unwrap()
+    })
+}
+
 #[pyclass]
 /// HTTP client that can impersonate web browsers.
-struct Client {
-    client: reqwest_impersonate::blocking::Client,
+pub struct Client {
+    client: Arc<reqwest_impersonate::Client>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     params: Option<HashMap<String, String>>,
 }
 
 #[pymethods]
 impl Client {
@@ -90,18 +109,18 @@
     ) -> PyResult<Self> {
         if auth.is_some() && auth_bearer.is_some() {
             return Err(PyErr::new::<exceptions::PyValueError, _>(
                 "Cannot provide both auth and auth_bearer",
             ));
         }
 
-        let mut client_builder = reqwest_impersonate::blocking::Client::builder()
+        // Client builder
+        let mut client_builder = reqwest_impersonate::Client::builder()
             .enable_ech_grease(true)
-            .permute_extensions(true)
-            .timeout(timeout.map(Duration::from_secs_f64));
+            .permute_extensions(true);
 
         // Headers
         if let Some(headers) = headers {
             let mut headers_new = HeaderMap::new();
             for (key, value) in headers {
                 headers_new.insert(
                     HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
@@ -128,14 +147,19 @@
         // Proxy
         if let Some(proxy_url) = proxy {
             let proxy = reqwest_impersonate::Proxy::all(proxy_url)
                 .map_err(|_| PyErr::new::<exceptions::PyValueError, _>("Invalid proxy URL"))?;
             client_builder = client_builder.proxy(proxy);
         }
 
+        // Timeout
+        if let Some(seconds) = timeout {
+            client_builder = client_builder.timeout(Duration::from_secs_f64(seconds));
+        }
+
         // Impersonate
         if let Some(impersonation_type) = impersonate {
             let impersonation = Impersonate::from_str(impersonation_type).map_err(|_| {
                 PyErr::new::<exceptions::PyValueError, _>("Invalid impersonate param")
             })?;
             client_builder = client_builder.impersonate(impersonation);
         }
@@ -162,17 +186,18 @@
                 ));
             }
             (Some(true), _) => client_builder = client_builder.http1_only(),
             (_, Some(true)) => client_builder = client_builder.http2_prior_knowledge(),
             _ => (),
         }
 
-        let client = client_builder
-            .build()
-            .map_err(|_| PyErr::new::<exceptions::PyValueError, _>("Failed to build client"))?;
+        let client =
+            Arc::new(client_builder.build().map_err(|_| {
+                PyErr::new::<exceptions::PyValueError, _>("Failed to build client")
+            })?);
 
         Ok(Client {
             client,
             auth,
             auth_bearer,
             params,
         })
@@ -211,123 +236,123 @@
         content: Option<Vec<u8>>,
         data: Option<HashMap<String, String>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
-        // Check if method is POST || PUT || PATCH
-        let is_post_put_patch = method == "POST" || method == "PUT" || method == "PATCH";
-
-        // Method
-        let method = match method {
-            "GET" => Ok(Method::GET),
-            "POST" => Ok(Method::POST),
-            "HEAD" => Ok(Method::HEAD),
-            "OPTIONS" => Ok(Method::OPTIONS),
-            "PUT" => Ok(Method::PUT),
-            "PATCH" => Ok(Method::PATCH),
-            "DELETE" => Ok(Method::DELETE),
-            &_ => Err(PyErr::new::<exceptions::PyException, _>(
-                "Unrecognized HTTP method",
-            )),
-        };
-        let method = method?;
-
-        // Create request builder
-        let mut request_builder = self.client.request(method, url);
-
-        // Params (use the provided `params` if available; otherwise, fall back to `self.params`)
-        let params_to_use = params.or(self.params.clone()).unwrap_or_default();
-        if !params_to_use.is_empty() {
-            request_builder = request_builder.query(&params_to_use);
-        }
-
-        // Headers
-        if let Some(headers) = headers {
-            let mut headers_new = HeaderMap::new();
-            for (key, value) in headers {
-                headers_new.insert(
-                    HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
-                        PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
-                    })?,
-                    HeaderValue::from_str(&value).map_err(|_| {
-                        PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
-                    })?,
-                );
+        let client = Arc::clone(&self.client);
+        let method = method.to_owned();
+        let url = url.to_owned();
+        let auth = auth.or(self.auth.clone());
+        let auth_bearer = auth_bearer.or(self.auth_bearer.clone());
+        let params = params.or(self.params.clone());
+
+        let future = async move {
+            // Check if method is POST || PUT || PATCH
+            let is_post_put_patch = method == "POST" || method == "PUT" || method == "PATCH";
+
+            // Method
+            let method = match method.as_str() {
+                "GET" => Ok(Method::GET),
+                "POST" => Ok(Method::POST),
+                "HEAD" => Ok(Method::HEAD),
+                "OPTIONS" => Ok(Method::OPTIONS),
+                "PUT" => Ok(Method::PUT),
+                "PATCH" => Ok(Method::PATCH),
+                "DELETE" => Ok(Method::DELETE),
+                &_ => Err(PyErr::new::<exceptions::PyException, _>(
+                    "Unrecognized HTTP method",
+                )),
+            }?;
+
+            // Create request builder
+            let mut request_builder = client.request(method, url);
+
+            // Params
+            if let Some(params) = params {
+                request_builder = request_builder.query(&params);
+            }
+
+            // Headers
+            if let Some(headers) = headers {
+                let mut headers_new = HeaderMap::new();
+                for (key, value) in headers {
+                    headers_new.insert(
+                        HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
+                            PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
+                        })?,
+                        HeaderValue::from_str(&value).map_err(|_| {
+                            PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
+                        })?,
+                    );
+                }
+                request_builder = request_builder.headers(headers_new);
             }
-            request_builder = request_builder.headers(headers_new);
-        }
 
-        // Only if method POST || PUT || PATCH
-        if is_post_put_patch {
-            // Content
-            if let Some(content) = content {
-                request_builder = request_builder.body(content);
-            }
-            // Data
-            if let Some(data) = data {
-                request_builder = request_builder.form(&data);
-            }
-            // Files
-            if let Some(files) = files {
-                let mut form = multipart::Form::new();
-                for (field, path) in files {
-                    form = form.file(field, path)?;
+            // Only if method POST || PUT || PATCH
+            if is_post_put_patch {
+                // Content
+                if let Some(content) = content {
+                    request_builder = request_builder.body(content);
+                }
+                // Data
+                if let Some(data) = data {
+                    request_builder = request_builder.form(&data);
+                }
+                // Files
+                if let Some(files) = files {
+                    let mut form = multipart::Form::new();
+                    for (field, path) in files {
+                        let file_content = tokio::fs::read(&path).await.map_err(|e| {
+                            PyErr::new::<exceptions::PyException, _>(format!(
+                                "Error reading file {}: {}",
+                                path, e
+                            ))
+                        })?;
+                        let part = multipart::Part::bytes(file_content);
+                        form = form.part(field, part);
+                    }
+                    request_builder = request_builder.multipart(form);
                 }
-                request_builder = request_builder.multipart(form);
             }
-        }
 
-        // Auth
-        match (auth, auth_bearer, &self.auth, &self.auth_bearer) {
-            (Some((username, password)), None, _, _) => {
-                request_builder = request_builder.basic_auth(username, password.as_deref());
-            }
-            (None, Some(token), _, _) => {
-                request_builder = request_builder.bearer_auth(token);
-            }
-            (None, None, Some((username, password)), None) => {
-                request_builder = request_builder.basic_auth(username, password.as_deref());
-            }
-            (None, None, None, Some(token)) => {
-                request_builder = request_builder.bearer_auth(token);
-            }
-            (Some(_), Some(_), None, None) | (None, None, Some(_), Some(_)) => {
-                return Err(PyErr::new::<exceptions::PyValueError, _>(
-                    "Cannot provide both auth and auth_bearer",
-                ));
+            // Auth
+            match (auth, auth_bearer) {
+                (Some((username, password)), None) => {
+                    request_builder = request_builder.basic_auth(username, password.as_deref());
+                }
+                (None, Some(token)) => {
+                    request_builder = request_builder.bearer_auth(token);
+                }
+                (Some(_), Some(_)) => {
+                    return Err(PyErr::new::<exceptions::PyValueError, _>(
+                        "Cannot provide both auth and auth_bearer",
+                    ));
+                }
+                _ => {} // No authentication provided
             }
-            _ => {} // No authentication provided
-        }
 
-        // Timeout
-        if let Some(seconds) = timeout {
-            request_builder = request_builder.timeout(Duration::from_secs_f64(seconds));
-        }
+            // Timeout
+            if let Some(seconds) = timeout {
+                request_builder = request_builder.timeout(Duration::from_secs_f64(seconds));
+            }
 
-        // Send request | release GIL
-        let resp = py.allow_threads(|| {
-            request_builder.send().map_err(|e| {
+            // Send the request and await the response
+            let resp = request_builder.send().await.map_err(|e| {
                 PyErr::new::<exceptions::PyException, _>(format!("Error in request: {}", e))
-            })
-        })?;
-
-        // Response items
-        let cookies_dict = PyDict::new_bound(py);
-        for cookie in resp.cookies() {
-            let key = cookie.name().to_string();
-            let value = cookie.value().to_string();
-            cookies_dict.set_item(key, value)?;
-        }
-        let cookies = cookies_dict.unbind();
+            })?;
 
-        // Encoding from "Content-Type" header or "UTF-8"
-        let encoding = {
-            let encoding_str = resp
+            // Response items
+            let cookies: HashMap<String, String> = resp
+                .cookies()
+                .map(|cookie| (cookie.name().to_string(), cookie.value().to_string()))
+                .collect();
+            // Encoding from "Content-Type" header or "UTF-8"
+            let encoding = resp
                 .headers()
                 .get("Content-Type")
                 .and_then(|ct| ct.to_str().ok())
                 .and_then(|ct| {
                     ct.split(';').find_map(|param| {
                         let mut kv = param.splitn(2, '=');
                         let key = kv.next()?.trim();
@@ -336,33 +361,62 @@
                             Some(value.to_string())
                         } else {
                             None
                         }
                     })
                 })
                 .unwrap_or("UTF-8".to_string());
-            PyString::new_bound(py, &encoding_str).unbind()
+            let headers: HashMap<String, String> = resp
+                .headers()
+                .iter()
+                .map(|(k, v)| (k.as_str().to_string(), v.to_str().unwrap_or("").to_string()))
+                .collect();
+            let status_code = resp.status().as_u16();
+            let url = resp.url().to_string();
+            let buf = resp.bytes().await.map_err(|e| {
+                PyErr::new::<exceptions::PyException, _>(format!(
+                    "Error reading response bytes: {}",
+                    e
+                ))
+            })?;
+            Ok((buf, cookies, encoding, headers, status_code, url))
         };
 
+        // Execute an async future in Python, releasing the GIL for concurrency.
+        // Uses Rayon's global thread pool and Tokio global runtime to block on the future.
+        let (tx, rx) = mpsc::sync_channel(1);
+        py.allow_threads(|| {
+            cpu_pool().install(|| {
+                let result = runtime().block_on(future);
+                _ = tx.send(result);
+            });
+        });
+        let result = rx.recv().map_err(|e| {
+            PyErr::new::<exceptions::PyException, _>(format!("Error executing future: {}", e))
+        })?;
+        let (f_buf, f_cookies, f_encoding, f_headers, f_status_code, f_url) = match result {
+            Ok(value) => value,
+            Err(e) => return Err(e),
+        };
+
+        // Response items
+        let cookies_dict = PyDict::new_bound(py);
+        for (key, value) in f_cookies {
+            cookies_dict.set_item(key, value)?;
+        }
+        let cookies = cookies_dict.unbind();
+        let encoding = PyString::new_bound(py, f_encoding.as_str()).unbind();
         let headers_dict = PyDict::new_bound(py);
-        for (key, value) in resp.headers().iter() {
-            let key_str = key.as_str();
-            let value_str = value.to_str().unwrap_or("");
-            headers_dict.set_item(key_str, value_str)?;
+        for (key, value) in f_headers {
+            headers_dict.set_item(key, value)?;
         }
         let headers = headers_dict.unbind();
-
-        let status_code = resp.status().as_u16().into_py(py);
-
-        let url = PyString::new_bound(py, resp.url().as_ref()).into();
-
-        let buf = resp.bytes().map_err(|e| {
-            PyErr::new::<exceptions::PyException, _>(format!("Error reading response bytes: {}", e))
-        })?;
-        let content = PyBytes::new_bound(py, &buf).unbind();
+        let status_code = f_status_code.into_py(py);
+        let url = PyString::new_bound(py, &f_url).unbind();
+        let content = PyBytes::new_bound(py, &f_buf).unbind();
 
         Ok(Response {
             content,
             cookies,
             encoding,
             headers,
             status_code,
@@ -556,65 +610,69 @@
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.get(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn head(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.head(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn options(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.options(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn delete(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.delete(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn post(
     py: Python,
@@ -623,17 +681,18 @@
     headers: Option<HashMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<HashMap<String, String>>,
     files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.post(
         py,
         url,
         params,
         headers,
         content,
@@ -653,17 +712,18 @@
     headers: Option<HashMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<HashMap<String, String>>,
     files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.put(
         py,
         url,
         params,
         headers,
         content,
@@ -683,17 +743,18 @@
     headers: Option<HashMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<HashMap<String, String>>,
     files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
+    impersonate: Option<&str>,
 ) -> PyResult<Response> {
     let client = Client::new(
-        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+        None, None, None, None, None, None, None, None, impersonate, None, None, None, None, None,
     )?;
     client.patch(
         py,
         url,
         params,
         headers,
         content,
```

### Comparing `pyreqwest_impersonate-0.3.2/src/response.rs` & `pyreqwest_impersonate-0.4.0/src/response.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     #[pyo3(get)]
     pub encoding: Py<PyString>,
     #[pyo3(get)]
     pub headers: Py<PyDict>,
     #[pyo3(get)]
     pub status_code: Py<PyAny>,
     #[pyo3(get)]
-    pub url: Py<PyAny>,
+    pub url: Py<PyString>,
 }
 
 #[pymethods]
 impl Response {
     #[getter]
     fn text(&mut self, py: Python) -> PyResult<String> {
         // Access the string data as bytes
```

### Comparing `pyreqwest_impersonate-0.3.2/tests/test_client.py` & `pyreqwest_impersonate-0.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.2/tests/test_defs.py` & `pyreqwest_impersonate-0.4.0/tests/test_defs.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.2/Cargo.lock` & `pyreqwest_impersonate-0.4.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -197,17 +197,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
@@ -290,14 +290,39 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
@@ -387,20 +412,14 @@
 [[package]]
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
-name = "futures-io"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
-
-[[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
@@ -411,20 +430,17 @@
 [[package]]
 name = "futures-util"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-core",
- "futures-io",
  "futures-task",
- "memchr",
  "pin-project-lite",
  "pin-utils",
- "slab",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
@@ -909,21 +925,23 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.3.2"
+version = "0.4.0"
 dependencies = [
  "encoding_rs",
  "pyo3",
  "pythonize",
+ "rayon",
  "reqwest-impersonate",
  "serde_json",
+ "tokio",
 ]
 
 [[package]]
 name = "pythonize"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d0664248812c38cc55a4ed07f88e4df516ce82604b93b1ffdc041aa77a6cb3c"
@@ -938,14 +956,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rayon"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags 2.5.0",
 ]
@@ -977,17 +1015,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest-impersonate"
-version = "0.11.72"
+version = "0.11.75"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b725314a794f526bac22292a10e2bf581cbea5ebd527fa3032e2cfd829068be"
+checksum = "78ba0d953bf10f7aa5d454bc8d9136efd94c3cfb4d6db4f02323b54957f7310f"
 dependencies = [
  "async-compression",
  "base64",
  "boring-imp",
  "boring-sys-imp",
  "bytes",
  "cookie",
@@ -1047,26 +1085,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
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
```

### Comparing `pyreqwest_impersonate-0.3.2/pyproject.toml` & `pyreqwest_impersonate-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.2/PKG-INFO` & `pyreqwest_impersonate-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.3.2
+Version: 0.4.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -22,17 +22,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/pyreqwest-impersonate)](https://github.com/deedy5/pyreqwest-impersonate/releases) [![](https://badge.fury.io/py/pyreqwest_impersonate.svg)](https://pypi.org/project/pyreqwest_impersonate) [![Downloads](https://static.pepy.tech/badge/pyreqwest_impersonate/week)](https://pepy.tech/project/pyreqwest_impersonate) [![CI](https://github.com/deedy5/pyreqwest-impersonate/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/deedy5/pyreqwest-impersonate/actions/workflows/CI.yml)
 # Pyreqwest_impersonate
 
 The fastest python HTTP client that can impersonate web browsers by mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints.</br>
-Binding to the Rust `reqwest_impersonate` library.</br>
-🏁 Check the [benchmark](https://github.com/deedy5/pyreqwest_impersonate/tree/main/benchmark) for more details.
-
+Binding to the Rust [reqwest_impersonate](https://github.com/gngpp/reqwest-impersonate) library.</br>
 
 Provides precompiled wheels:
 - [x] Linux:  `amd64`, `aarch64`, `armv7`.
 - [x] Windows: `amd64`.
 - [x] MacOS:  `amd64`, `aarch64`.
 
 ## Table of Contents
@@ -47,19 +45,21 @@
 ## Installation
 
 ```python
 pip install -U pyreqwest_impersonate
 ```
 
 ## Key Features
-- `Impersonate`: The `Client` offers an `impersonate` option, enabling it to mimic web browsers by replicating their headers and `TLS/JA3/JA4/HTTP2` fingerprints. This feature is crucial for avoiding detection as a bot and potential blocking by websites.
-- `Thread-safe`: The `Client` is designed to be thread-safe, allowing it to be safely used in multithreaded environments.
-- `High Performance`: The attributes of the `Response` object are executed in Rust, which is known for its high performance. This ensures that operations like accessing headers, decoding text, or parsing JSON are very fast.
-- `Lazy Execution`: All attributes of the `Response` object are executed lazily. This means that the actual computation or data retrieval happens only when you access the attribute, not when the `Response` object is created.
-- `Automatic Character Encoding Detection`: The `Response` object intelligently detects the character encoding of the response body from the "Content-Type" header. If the encoding is not specified, it defaults to "UTF-8".
+- Impersonate: The Client offers an `impersonate` option, enabling it to mimic web browsers by replicating their headers and TLS/JA3/JA4/HTTP2 fingerprints.
+- Thread-safe: The Client is designed to be thread-safe, allowing it to be safely used in multithreaded environments.
+- Automatic Character Encoding Detection: The encoding is taken from the "Content-Type" header, but if not specified, "UTF-8".
+- Small Size: The compiled library is about 5.8MB in size.
+- High Performance: The library is designed for a large number of threads, uses all processors, and releases the GIL. All operations like accessing headers, decoding text, or parsing JSON are executed in Rust.
+
+![](https://github.com/deedy5/pyreqwest_impersonate/blob/benchmark/benchmark.jpg?raw=true)
 
 ## Usage
 ### I. Client
 
 HTTP client that can impersonate web browsers.
 ```python
 class Client:
@@ -92,30 +92,30 @@
     """
 ```
 
 #### Client Methods
 
 The `Client` class provides a set of methods for making HTTP requests: `get`, `head`, `options`, `delete`, `post`, `put`, `patch`, each of which internally utilizes the `request()` method for execution. The parameters for these methods closely resemble those in `httpx`.
 ```python
-def get(url, *, params=None, headers=None, auth=None, auth_bearer=None, timeout=None):
+def get(url, params=None, headers=None, auth=None, auth_bearer=None, timeout=None):
     """Performs a GET request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password 
             for basic authentication. Default is None.
         auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
         timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 
     """
 ```
 ```python
-def post(url, *, params=None, headers=None, content=None, data=None, files=None, auth=None, auth_bearer=None, timeout=None):
+def post(url, params=None, headers=None, content=None, data=None, files=None, auth=None, auth_bearer=None, timeout=None):
     """Performs a POST request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         content (Optional[bytes]): The content to send in the request body as bytes. Default is None.
@@ -150,15 +150,15 @@
 print(resp.json())
 print(resp.status_code)
 print(resp.text)
 print(resp.url)
 
 # You can also use convenience functions that use a default Client instance under the hood:
 # pri.get() | pri.head() | pri.options() | pri.delete() | pri.post | pri.patch | pri.put
-resp = pri.get("https://httpbin.org/anything") # Default Client does not impersonate a browser
-resp = pri.Client(impersonate="chrome_123").get("https://httpbin.org/anything")  
+# These functions can accept the `impersonate` parameter:
+resp = pri.get("https://httpbin.org/anything", impersonate="chrome_123")  
 ```
 ### II. AsyncClient
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

