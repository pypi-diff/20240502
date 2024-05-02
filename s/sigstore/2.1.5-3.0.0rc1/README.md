# Comparing `tmp/sigstore-2.1.5.tar.gz` & `tmp/sigstore-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-2.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore-3.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore-2.1.5.tar` & `sigstore-3.0.0rc1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0    11358 2024-04-08 14:27:08.179680 sigstore-2.1.5/LICENSE
--rw-r--r--   0        0        0    20630 2024-04-08 14:27:08.179680 sigstore-2.1.5/README.md
--rw-r--r--   0        0        0     3948 2024-04-08 14:27:08.179680 sigstore-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      955 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/__init__.py
--rw-r--r--   0        0        0      726 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/__main__.py
--rw-r--r--   0        0        0    35844 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_cli.py
--rw-r--r--   0        0        0      738 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/__init__.py
--rw-r--r--   0        0        0      774 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/ctfe.py
--rw-r--r--   0        0        0      883 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/fulcio/__init__.py
--rw-r--r--   0        0        0    12112 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/fulcio/client.py
--rw-r--r--   0        0        0     3891 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/keyring.py
--rw-r--r--   0        0        0     4544 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/merkle.py
--rw-r--r--   0        0        0      653 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    15958 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/oidc/oauth.py
--rw-r--r--   0        0        0      748 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/rekor/__init__.py
--rw-r--r--   0        0        0     7235 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/rekor/checkpoint.py
--rw-r--r--   0        0        0     8026 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/rekor/client.py
--rw-r--r--   0        0        0     9884 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/sct.py
--rw-r--r--   0        0        0     1729 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/set.py
--rw-r--r--   0        0        0     9403 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/tuf.py
--rw-r--r--   0        0        0     1247 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/__init__.py
--rw-r--r--   0        0        0     6388 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/prod/root.json
--rw-r--r--   0        0        0     4567 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/prod/trusted_root.json
--rw-r--r--   0        0        0     1876 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/staging/root.json
--rw-r--r--   0        0        0     4521 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/staging/trusted_root.json
--rw-r--r--   0        0        0    10225 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_utils.py
--rw-r--r--   0        0        0     3247 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/errors.py
--rw-r--r--   0        0        0    15939 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/oidc.py
--rw-r--r--   0        0        0    13258 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/sign.py
--rw-r--r--   0        0        0     5519 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/transparency.py
--rw-r--r--   0        0        0     1932 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/__init__.py
--rw-r--r--   0        0        0    18223 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/models.py
--rw-r--r--   0        0        0     9824 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/policy.py
--rw-r--r--   0        0        0    11484 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/verifier.py
--rw-r--r--   0        0        0    22802 1970-01-01 00:00:00.000000 sigstore-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    18625 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/README.md
+-rw-r--r--   0        0        0     3969 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      958 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/__main__.py
+-rw-r--r--   0        0        0    31481 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_cli.py
+-rw-r--r--   0        0        0      738 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/fulcio/__init__.py
+-rw-r--r--   0        0        0    11999 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/fulcio/client.py
+-rw-r--r--   0        0        0     4414 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/merkle.py
+-rw-r--r--   0        0        0      653 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    15962 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/oidc/oauth.py
+-rw-r--r--   0        0        0     1634 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/rekor/__init__.py
+-rw-r--r--   0        0        0     7293 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/rekor/checkpoint.py
+-rw-r--r--   0        0        0     8028 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/rekor/client.py
+-rw-r--r--   0        0        0     8688 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/sct.py
+-rw-r--r--   0        0        0    10909 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/trustroot.py
+-rw-r--r--   0        0        0     5819 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_internal/tuf.py
+-rw-r--r--   0        0        0     1247 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/__init__.py
+-rw-r--r--   0        0        0     6388 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/prod/root.json
+-rw-r--r--   0        0        0     4567 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/prod/trusted_root.json
+-rw-r--r--   0        0        0     1871 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/staging/root.json
+-rw-r--r--   0        0        0     7256 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_store/staging/trusted_root.json
+-rw-r--r--   0        0        0    11933 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/_utils.py
+-rw-r--r--   0        0        0     7723 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/dsse.py
+-rw-r--r--   0        0        0     3391 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/errors.py
+-rw-r--r--   0        0        0     1779 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/hashes.py
+-rw-r--r--   0        0        0    18257 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/models.py
+-rw-r--r--   0        0        0    15939 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/oidc.py
+-rw-r--r--   0        0        0    11866 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/sign.py
+-rw-r--r--   0        0        0     1280 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/verify/__init__.py
+-rw-r--r--   0        0        0     8755 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/verify/policy.py
+-rw-r--r--   0        0        0    13885 2024-05-02 15:20:59.736195 sigstore-3.0.0rc1/sigstore/verify/verifier.py
+-rw-r--r--   0        0        0    20876 1970-01-01 00:00:00.000000 sigstore-3.0.0rc1/PKG-INFO
```

### Comparing `sigstore-2.1.5/LICENSE` & `sigstore-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/README.md` & `sigstore-3.0.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,62 @@
+Metadata-Version: 2.1
+Name: sigstore
+Version: 3.0.0rc1
+Summary: A tool for signing Python package distributions
+Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Security
+Classifier: Topic :: Security :: Cryptography
+Requires-Dist: cryptography >= 42
+Requires-Dist: id >= 1.1.0
+Requires-Dist: importlib_resources ~= 5.7; python_version < '3.11'
+Requires-Dist: pydantic >= 2,< 3
+Requires-Dist: pyjwt >= 2.1
+Requires-Dist: pyOpenSSL >= 23.0.0
+Requires-Dist: requests
+Requires-Dist: rich ~= 13.0
+Requires-Dist: rfc8785 ~= 0.1.2
+Requires-Dist: sigstore-protobuf-specs ~= 0.3.1
+Requires-Dist: sigstore-rekor-types == 0.0.13
+Requires-Dist: tuf ~= 4.0
+Requires-Dist: platformdirs ~= 4.2
+Requires-Dist: build ; extra == "dev"
+Requires-Dist: bump >= 1.3.2 ; extra == "dev"
+Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
+Requires-Dist: pdoc ; extra == "doc"
+Requires-Dist: bandit ; extra == "lint"
+Requires-Dist: setuptools ; extra == "lint"
+Requires-Dist: interrogate ; extra == "lint"
+Requires-Dist: mypy ~= 1.1 ; extra == "lint"
+Requires-Dist: ruff < 0.4.3 ; extra == "lint"
+Requires-Dist: types-requests ; extra == "lint"
+Requires-Dist: types-pyOpenSSL ; extra == "lint"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pretend ; extra == "test"
+Requires-Dist: coverage[toml] ; extra == "test"
+Project-URL: Documentation, https://sigstore.github.io/sigstore-python/
+Project-URL: Homepage, https://pypi.org/project/sigstore/
+Project-URL: Issues, https://github.com/sigstore/sigstore-python/issues
+Project-URL: Source, https://github.com/sigstore/sigstore-python
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: lint
+Provides-Extra: test
+
 sigstore-python
 ===============
 
 <!--- @begin-badges@ --->
 ![CI](https://github.com/sigstore/sigstore-python/workflows/CI/badge.svg)
 [![PyPI version](https://badge.fury.io/py/sigstore.svg)](https://pypi.org/project/sigstore)
 [![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/sigstore/sigstore-python/badge)](https://securityscorecards.dev/viewer/?uri=github.com/sigstore/sigstore-python)
@@ -92,66 +147,61 @@
 python -m sigstore --help
 ```
 
 Top-level:
 
 <!-- @begin-sigstore-help@ -->
 ```
-usage: sigstore [-h] [-v] [-V] [--staging] [--rekor-url URL]
-                [--rekor-root-pubkey FILE]
-                COMMAND ...
+usage: sigstore [-h] [-v] [-V] [--staging] [--rekor-url URL] COMMAND ...
 
 a tool for signing and verifying Python package distributions
 
 positional arguments:
-  COMMAND               the operation to perform
-    sign                sign one or more inputs
-    verify              verify one or more inputs
-    get-identity-token  retrieve and return a Sigstore-compatible OpenID
-                        Connect token
+  COMMAND             the operation to perform
+    sign              sign one or more inputs
+    verify            verify one or more inputs
+    get-identity-token
+                      retrieve and return a Sigstore-compatible OpenID Connect
+                      token
 
 optional arguments:
-  -h, --help            show this help message and exit
-  -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
-  -V, --version         show program's version number and exit
+  -h, --help          show this help message and exit
+  -v, --verbose       run with additional debug logging; supply multiple times
+                      to increase verbosity (default: 0)
+  -V, --version       show program's version number and exit
 
 Sigstore instance options:
-  --staging             Use sigstore's staging instances, instead of the
-                        default production instances (default: False)
-  --rekor-url URL       The Rekor instance to use (conflicts with --staging)
-                        (default: https://rekor.sigstore.dev)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging) (default: None)
+  --staging           Use sigstore's staging instances, instead of the default
+                      production instances (default: False)
+  --rekor-url URL     The Rekor instance to use (conflicts with --staging)
+                      (default: https://rekor.sigstore.dev)
 ```
 <!-- @end-sigstore-help@ -->
 
 
 ### Signing
 
 <!-- @begin-sigstore-sign-help@ -->
 ```
 usage: sigstore sign [-h] [-v] [--identity-token TOKEN] [--oidc-client-id ID]
                      [--oidc-client-secret SECRET]
                      [--oidc-disable-ambient-providers] [--oidc-issuer URL]
                      [--oauth-force-oob] [--no-default-files]
                      [--signature FILE] [--certificate FILE] [--bundle FILE]
                      [--output-directory DIR] [--overwrite] [--staging]
-                     [--rekor-url URL] [--rekor-root-pubkey FILE]
-                     [--fulcio-url URL] [--ctfe FILE]
+                     [--rekor-url URL] [--fulcio-url URL]
                      FILE [FILE ...]
 
 positional arguments:
   FILE                  The file to sign
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
+                        times to increase verbosity (default: 0)
 
 OpenID Connect options:
   --identity-token TOKEN
                         the OIDC identity token to use (default: None)
   --oidc-client-id ID   The custom OpenID Connect client ID to use during
                         OAuth2 (default: sigstore)
   --oidc-client-secret SECRET
@@ -189,23 +239,16 @@
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
                         in a future release. (default: False)
   --rekor-url URL       The Rekor instance to use (conflicts with --staging).
                         This option will be deprecated in favor of the global
                         `--rekor-url` option in a future release. (default:
                         None)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging). This option will be
-                        deprecated in favor of the global `--rekor-root-
-                        pubkey` option in a future release. (default: None)
   --fulcio-url URL      The Fulcio instance to use (conflicts with --staging)
                         (default: https://fulcio.sigstore.dev)
-  --ctfe FILE           A PEM-encoded public key for the CT log (conflicts
-                        with --staging) (default: None)
 ```
 <!-- @end-sigstore-sign-help@ -->
 
 ### Verifying
 
 #### Generic identities
 
@@ -216,22 +259,21 @@
 
 <!-- @begin-sigstore-verify-identity-help@ -->
 ```
 usage: sigstore verify identity [-h] [-v] [--certificate FILE]
                                 [--signature FILE] [--bundle FILE]
                                 --cert-identity IDENTITY [--offline]
                                 --cert-oidc-issuer URL [--staging]
-                                [--rekor-url URL] [--rekor-root-pubkey FILE]
-                                [--certificate-chain FILE]
+                                [--rekor-url URL]
                                 FILE [FILE ...]
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
+                        times to increase verbosity (default: 0)
 
 Verification inputs:
   --certificate FILE, --cert FILE
                         The PEM-encoded certificate to verify against; not
                         used with multiple inputs (default: None)
   --signature FILE      The signature to verify against; not used with
                         multiple inputs (default: None)
@@ -254,23 +296,14 @@
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
                         in a future release. (default: False)
   --rekor-url URL       The Rekor instance to use (conflicts with --staging).
                         This option will be deprecated in favor of the global
                         `--rekor-url` option in a future release. (default:
                         None)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging). This option will be
-                        deprecated in favor of the global `--rekor-root-
-                        pubkey` option in a future release. (default: None)
-  --certificate-chain FILE
-                        Path to a list of CA certificates in PEM format which
-                        will be needed when building the certificate chain for
-                        the Fulcio signing certificate (default: None)
 ```
 <!-- @end-sigstore-verify-identity-help@ -->
 
 #### Signatures from GitHub Actions
 
 If your signatures are coming from GitHub Actions (e.g., a workflow
 that uses its [ambient credentials](#signing-with-ambient-credentials)),
@@ -280,22 +313,21 @@
 <!-- @begin-sigstore-verify-github-help@ -->
 ```
 usage: sigstore verify github [-h] [-v] [--certificate FILE]
                               [--signature FILE] [--bundle FILE]
                               --cert-identity IDENTITY [--offline]
                               [--trigger EVENT] [--sha SHA] [--name NAME]
                               [--repository REPO] [--ref REF] [--staging]
-                              [--rekor-url URL] [--rekor-root-pubkey FILE]
-                              [--certificate-chain FILE]
+                              [--rekor-url URL]
                               FILE [FILE ...]
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
+                        times to increase verbosity (default: 0)
 
 Verification inputs:
   --certificate FILE, --cert FILE
                         The PEM-encoded certificate to verify against; not
                         used with multiple inputs (default: None)
   --signature FILE      The signature to verify against; not used with
                         multiple inputs (default: None)
@@ -325,23 +357,14 @@
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
                         in a future release. (default: False)
   --rekor-url URL       The Rekor instance to use (conflicts with --staging).
                         This option will be deprecated in favor of the global
                         `--rekor-url` option in a future release. (default:
                         None)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging). This option will be
-                        deprecated in favor of the global `--rekor-root-
-                        pubkey` option in a future release. (default: None)
-  --certificate-chain FILE
-                        Path to a list of CA certificates in PEM format which
-                        will be needed when building the certificate chain for
-                        the Fulcio signing certificate (default: None)
 ```
 <!-- @end-sigstore-verify-github-help@ -->
 
 ## Example uses
 
 `sigstore` supports a wide variety of workflows and usages. Some common ones are
 provided below.
@@ -468,7 +491,8 @@
 process](https://github.com/sigstore/.github/blob/main/SECURITY.md).
 
 ### SLSA Provenance
 This project emits a SLSA provenance on its release! This enables you to verify the integrity
 of the downloaded artifacts and ensured that the binary's code really comes from this source code.
 
 To do so, please follow the instructions [here](https://github.com/slsa-framework/slsa-github-generator#verification-of-provenance).
+
```

### Comparing `sigstore-2.1.5/pyproject.toml` & `sigstore-3.0.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,28 +21,28 @@
   "Programming Language :: Python :: 3.11",
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Security",
   "Topic :: Security :: Cryptography",
 ]
 dependencies = [
-  "appdirs ~= 1.4",
-  "cryptography >= 39",
+  "cryptography >= 42",
   "id >= 1.1.0",
   "importlib_resources ~= 5.7; python_version < '3.11'",
   "pydantic >= 2,< 3",
   "pyjwt >= 2.1",
   "pyOpenSSL >= 23.0.0",
   "requests",
   "rich ~= 13.0",
-  "securesystemslib < 0.32.0",
-  "sigstore-protobuf-specs >= 0.2.2, < 0.4",
+  "rfc8785 ~= 0.1.2",
+  "sigstore-protobuf-specs ~= 0.3.1",
   # NOTE(ww): Under active development, so strictly pinned.
-  "sigstore-rekor-types == 0.0.11",
-  "tuf >= 2.1,< 4.0",
+  "sigstore-rekor-types == 0.0.13",
+  "tuf ~= 4.0",
+  "platformdirs ~= 4.2",
 ]
 requires-python = ">=3.8"
 
 [project.scripts]
 sigstore = "sigstore._cli:main"
 
 [project.urls]
@@ -51,23 +51,24 @@
 Source = "https://github.com/sigstore/sigstore-python"
 Documentation = "https://sigstore.github.io/sigstore-python/"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "pretend", "coverage[toml]"]
 lint = [
   "bandit",
+  # HACK(ww): interrogate needs setuptools to provide `pkg_resources` on Python 3.12+;
+  # remove this when https://github.com/econchick/interrogate/issues/164 is resolved.
+  "setuptools",
   "interrogate",
   "mypy ~= 1.1",
   # NOTE(ww): ruff is under active development, so we pin conservatively here
   # and let Dependabot periodically perform this update.
-  "ruff < 0.1.8",
+  "ruff < 0.4.3",
   "types-requests",
-  # TODO(ww): Re-enable once dependency on types-cryptography is dropped.
-  # See: https://github.com/python/typeshed/issues/8699
-  # "types-pyOpenSSL",
+  "types-pyOpenSSL",
 ]
 doc = ["pdoc"]
 dev = ["build", "bump >= 1.3.2", "sigstore[doc,test,lint]"]
 
 [tool.coverage.run]
 # branch coverage in addition to statement coverage.
 branch = true
@@ -115,14 +116,13 @@
 warn_unused_configs = true
 warn_unused_ignores = true
 plugins = ["pydantic.mypy"]
 
 [tool.bandit]
 exclude_dirs = ["./test"]
 
-[tool.ruff]
+[tool.ruff.lint]
 # Never enforce `E501` (line length violations).
 ignore = ["E501"]
 # TODO: Enable "UP" here once Pydantic allows us to:
 # See: https://github.com/pydantic/pydantic/issues/4146
 select = ["E", "F", "I", "W"]
-target-version = "py38"
```

### Comparing `sigstore-2.1.5/sigstore/__init__.py` & `sigstore-3.0.0rc1/sigstore/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 Otherwise, here are some quick starting points:
 
 * `sigstore.verify`: verifying of Sigstore signatures,
   including flexible policy control
 * `sigstore.sign`: creation of Sigstore signatures
 """
 
-__version__ = "2.1.5"
+__version__ = "3.0.0rc1"
```

### Comparing `sigstore-2.1.5/sigstore/__main__.py` & `sigstore-3.0.0rc1/sigstore/__main__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/sigstore/_cli.py` & `sigstore-3.0.0rc1/sigstore/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,63 +16,57 @@
 
 import argparse
 import base64
 import logging
 import os
 import sys
 from pathlib import Path
-from textwrap import dedent
-from typing import NoReturn, Optional, TextIO, Union, cast
+from typing import NoReturn, Optional, TextIO, Union
 
-from cryptography.x509 import load_pem_x509_certificates
+from cryptography.hazmat.primitives.serialization import Encoding
+from cryptography.x509 import load_pem_x509_certificate
 from rich.logging import RichHandler
-from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import Bundle
 
 from sigstore import __version__
-from sigstore._internal.ctfe import CTKeyring
 from sigstore._internal.fulcio.client import (
     DEFAULT_FULCIO_URL,
     ExpiredCertificate,
     FulcioClient,
 )
-from sigstore._internal.keyring import Keyring
+from sigstore._internal.rekor import _hashedrekord_from_parts
 from sigstore._internal.rekor.client import (
     DEFAULT_REKOR_URL,
     RekorClient,
-    RekorKeyring,
 )
-from sigstore._internal.tuf import TrustUpdater
-from sigstore._utils import PEMCert
-from sigstore.errors import Error
+from sigstore._internal.trustroot import KeyringPurpose, TrustedRoot
+from sigstore._utils import sha256_digest
+from sigstore.errors import Error, VerificationError
+from sigstore.hashes import Hashed
+from sigstore.models import Bundle
 from sigstore.oidc import (
     DEFAULT_OAUTH_ISSUER_URL,
     STAGING_OAUTH_ISSUER_URL,
     ExpiredIdentity,
     IdentityToken,
     Issuer,
     detect_credential,
 )
 from sigstore.sign import SigningContext
-from sigstore.transparency import LogEntry
 from sigstore.verify import (
-    CertificateVerificationFailure,
-    LogEntryMissing,
-    VerificationMaterials,
     Verifier,
     policy,
 )
-from sigstore.verify.models import VerificationFailure
 
 logging.basicConfig(format="%(message)s", datefmt="[%X]", handlers=[RichHandler()])
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 # NOTE: We configure the top package logger, rather than the root logger,
 # to avoid overly verbose logging in third-party code by default.
-package_logger = logging.getLogger("sigstore")
-package_logger.setLevel(os.environ.get("SIGSTORE_LOGLEVEL", "INFO").upper())
+_package_logger = logging.getLogger("sigstore")
+_package_logger.setLevel(os.environ.get("SIGSTORE_LOGLEVEL", "INFO").upper())
 
 
 def _die(args: argparse.Namespace, message: str) -> NoReturn:
     """
     An `argparse` helper that fixes up the type hints on our use of
     `ArgumentParser.error`.
     """
@@ -124,26 +118,14 @@
         default=None,
         help=(
             "The Rekor instance to use (conflicts with --staging). "
             "This option will be deprecated in favor of the global `--rekor-url` option "
             "in a future release."
         ),
     )
-    group.add_argument(
-        "--rekor-root-pubkey",
-        dest="__deprecated_rekor_root_pubkey",
-        metavar="FILE",
-        type=argparse.FileType("rb"),
-        default=None,
-        help=(
-            "A PEM-encoded root public key for Rekor itself (conflicts with --staging). "
-            "This option will be deprecated in favor of the global `--rekor-root-pubkey` option "
-            "in a future release."
-        ),
-    )
 
 
 def _add_shared_verify_input_options(group: argparse._ArgumentGroup) -> None:
     """
     Common input options, shared between all `sigstore verify` subcommands.
     """
     group.add_argument(
@@ -238,15 +220,15 @@
 def _parser() -> argparse.ArgumentParser:
     # Arguments in parent_parser can be used for both commands and subcommands
     parent_parser = argparse.ArgumentParser(add_help=False)
     parent_parser.add_argument(
         "-v",
         "--verbose",
         action="count",
-        default=argparse.SUPPRESS,
+        default=0,
         help="run with additional debug logging; supply multiple times to increase verbosity",
     )
 
     parser = argparse.ArgumentParser(
         prog="sigstore",
         description="a tool for signing and verifying Python package distributions",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -266,21 +248,14 @@
     global_instance_options.add_argument(
         "--rekor-url",
         metavar="URL",
         type=str,
         default=os.getenv("SIGSTORE_REKOR_URL", DEFAULT_REKOR_URL),
         help="The Rekor instance to use (conflicts with --staging)",
     )
-    global_instance_options.add_argument(
-        "--rekor-root-pubkey",
-        metavar="FILE",
-        type=argparse.FileType("rb"),
-        help="A PEM-encoded root public key for Rekor itself (conflicts with --staging)",
-        default=os.getenv("SIGSTORE_REKOR_ROOT_PUBKEY"),
-    )
 
     subcommands = parser.add_subparsers(
         required=True,
         dest="subcommand",
         metavar="COMMAND",
         help="the operation to perform",
     )
@@ -362,22 +337,14 @@
     instance_options.add_argument(
         "--fulcio-url",
         metavar="URL",
         type=str,
         default=os.getenv("SIGSTORE_FULCIO_URL", DEFAULT_FULCIO_URL),
         help="The Fulcio instance to use (conflicts with --staging)",
     )
-    instance_options.add_argument(
-        "--ctfe",
-        dest="ctfe_pem",
-        metavar="FILE",
-        type=argparse.FileType("rb"),
-        help="A PEM-encoded public key for the CT log (conflicts with --staging)",
-        default=os.getenv("SIGSTORE_CTFE"),
-    )
 
     sign.add_argument(
         "files",
         metavar="FILE",
         type=Path,
         nargs="+",
         help="The file to sign",
@@ -416,23 +383,14 @@
         default=os.getenv("SIGSTORE_CERT_OIDC_ISSUER"),
         help="The OIDC issuer URL to check for in the certificate's OIDC issuer extension",
         required=True,
     )
 
     instance_options = verify_identity.add_argument_group("Sigstore instance options")
     _add_shared_instance_options(instance_options)
-    instance_options.add_argument(
-        "--certificate-chain",
-        metavar="FILE",
-        type=argparse.FileType("rb"),
-        help=(
-            "Path to a list of CA certificates in PEM format which will be needed when building "
-            "the certificate chain for the Fulcio signing certificate"
-        ),
-    )
 
     # `sigstore verify github`
     verify_github = verify_subcommand.add_parser(
         "github",
         help="verify against GitHub Actions-specific claims",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=[parent_parser],
@@ -482,23 +440,14 @@
         type=str,
         default=os.getenv("SIGSTORE_VERIFY_GITHUB_WORKFLOW_REF"),
         help="The `git` ref that the workflow was invoked with",
     )
 
     instance_options = verify_github.add_argument_group("Sigstore instance options")
     _add_shared_instance_options(instance_options)
-    instance_options.add_argument(
-        "--certificate-chain",
-        metavar="FILE",
-        type=argparse.FileType("rb"),
-        help=(
-            "Path to a list of CA certificates in PEM format which will be needed when building "
-            "the certificate chain for the Fulcio signing certificate"
-        ),
-    )
 
     # `sigstore get-identity-token`
     get_identity_token = subcommands.add_parser(
         "get-identity-token",
         help="retrieve and return a Sigstore-compatible OpenID Connect token",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=[parent_parser],
@@ -509,44 +458,36 @@
 
 
 def main() -> None:
     parser = _parser()
     args = parser.parse_args()
 
     # Configure logging upfront, so that we don't miss anything.
-    verbose = args.verbose if hasattr(args, "verbose") else 0
-    if verbose >= 1:
-        package_logger.setLevel("DEBUG")
-    if verbose >= 2:
+    if args.verbose >= 1:
+        _package_logger.setLevel("DEBUG")
+    if args.verbose >= 2:
         logging.getLogger().setLevel("DEBUG")
 
-    logger.debug(f"parsed arguments {args}")
+    _logger.debug(f"parsed arguments {args}")
 
     # A few instance flags (like `--staging` and `--rekor-url`) are supported at both the
     # top-level `sigstore` level and the subcommand level (e.g. `sigstore verify --staging`),
     # but the former is preferred.
     if getattr(args, "__deprecated_staging", False):
-        logger.warning(
+        _logger.warning(
             "`--staging` should be used as a global option, rather than a subcommand option. "
             "Passing `--staging` as a subcommand option will be deprecated in a future release."
         )
         args.staging = args.__deprecated_staging
     if getattr(args, "__deprecated_rekor_url", None):
-        logger.warning(
+        _logger.warning(
             "`--rekor-url` should be used as a global option, rather than a subcommand option. "
             "Passing `--rekor-url` as a subcommand option will be deprecated in a future release."
         )
         args.rekor_url = args.__deprecated_rekor_url
-    if getattr(args, "__deprecated_rekor_root_pubkey", None):
-        logger.warning(
-            "`--rekor-root-pubkey` should be used as a global option, rather than a "
-            "subcommand option. Passing `--rekor-root-pubkey` as a subcommand option will be "
-            "deprecated in a future release."
-        )
-        args.rekor_root_pubkey = args.__deprecated_rekor_root_pubkey
 
     # Stuff the parser back into our namespace, so that we can use it for
     # error handling later.
     args._parser = parser
 
     try:
         if args.subcommand == "sign":
@@ -562,15 +503,15 @@
                 print(identity)
             else:
                 _die(args, "No identity token supplied or detected!")
 
         else:
             _die(args, f"Unknown subcommand: {args.subcommand}")
     except Error as e:
-        e.print_and_exit(verbose >= 1)
+        e.log_and_exit(_logger, args.verbose >= 1)
 
 
 def _sign(args: argparse.Namespace) -> None:
     has_sig = bool(args.signature)
     has_crt = bool(args.certificate)
     has_bundle = bool(args.bundle)
 
@@ -597,15 +538,15 @@
 
     # Fail if either `--signature` or `--certificate` is specified, but not both.
     if has_sig ^ has_crt:
         _die(args, "Error: --signature and --certificate must be used together.")
 
     # Build up the map of inputs -> outputs ahead of any signing operations,
     # so that we can fail early if overwriting without `--overwrite`.
-    output_map = {}
+    output_map: dict[Path, dict[str, Path | None]] = {}
     for file in args.files:
         if not file.is_file():
             _die(args, f"Input must be a file: {file}")
 
         sig, cert, bundle = (
             args.signature,
             args.certificate,
@@ -640,37 +581,27 @@
             "cert": cert,
             "sig": sig,
             "bundle": bundle,
         }
 
     # Select the signing context to use.
     if args.staging:
-        logger.debug("sign: staging instances requested")
+        _logger.debug("sign: staging instances requested")
         signing_ctx = SigningContext.staging()
         args.oidc_issuer = STAGING_OAUTH_ISSUER_URL
     elif args.fulcio_url == DEFAULT_FULCIO_URL and args.rekor_url == DEFAULT_REKOR_URL:
         signing_ctx = SigningContext.production()
     else:
-        # Assume "production" keys if none are given as arguments
-        updater = TrustUpdater.production()
-        if args.ctfe_pem is not None:
-            ctfe_keys = [args.ctfe_pem.read()]
-        else:
-            ctfe_keys = updater.get_ctfe_keys()
-        if args.rekor_root_pubkey is not None:
-            rekor_keys = [args.rekor_root_pubkey.read()]
-        else:
-            rekor_keys = updater.get_rekor_keys()
-
-        ct_keyring = CTKeyring(Keyring(ctfe_keys))
-        rekor_keyring = RekorKeyring(Keyring(rekor_keys))
+        # Assume "production" trust root if no keys are given as arguments
+        trusted_root = TrustedRoot.production(purpose=KeyringPurpose.SIGN)
 
         signing_ctx = SigningContext(
             fulcio=FulcioClient(args.fulcio_url),
-            rekor=RekorClient(args.rekor_url, rekor_keyring, ct_keyring),
+            rekor=RekorClient(args.rekor_url),
+            trusted_root=trusted_root,
         )
 
     # The order of precedence for identities is as follows:
     #
     # 1) Explicitly supplied identity token
     # 2) Ambient credential detected in the environment, unless disabled
     # 3) Interactive OAuth flow
@@ -681,63 +612,71 @@
         identity = _get_identity(args)
 
     if not identity:
         _die(args, "No identity token supplied or detected!")
 
     with signing_ctx.signer(identity) as signer:
         for file, outputs in output_map.items():
-            logger.debug(f"signing for {file.name}")
-            with file.open(mode="rb", buffering=0) as io:
-                try:
-                    result = signer.sign(input_=io)
-                except ExpiredIdentity as exp_identity:
-                    print("Signature failed: identity token has expired")
-                    raise exp_identity
-
-                except ExpiredCertificate as exp_certificate:
-                    print("Signature failed: Fulcio signing certificate has expired")
-                    raise exp_certificate
+            _logger.debug(f"signing for {file.name}")
+            with file.open(mode="rb") as io:
+                # The input can be indefinitely large, so we perform a streaming
+                # digest and sign the prehash rather than buffering it fully.
+                digest = sha256_digest(io)
+            try:
+                result = signer.sign_artifact(input_=digest)
+            except ExpiredIdentity as exp_identity:
+                print("Signature failed: identity token has expired")
+                raise exp_identity
+
+            except ExpiredCertificate as exp_certificate:
+                print("Signature failed: Fulcio signing certificate has expired")
+                raise exp_certificate
 
             print("Using ephemeral certificate:")
-            print(result.cert_pem)
+            cert = result.signing_certificate
+            cert_pem = cert.public_bytes(Encoding.PEM).decode()
+            print(cert_pem)
 
             print(
                 f"Transparency log entry created at index: {result.log_entry.log_index}"
             )
 
             sig_output: TextIO
             if outputs["sig"] is not None:
                 sig_output = outputs["sig"].open("w")
             else:
                 sig_output = sys.stdout
 
-            print(result.b64_signature, file=sig_output)
+            signature = base64.b64encode(
+                result._inner.message_signature.signature
+            ).decode()
+            print(signature, file=sig_output)
             if outputs["sig"] is not None:
                 print(f"Signature written to {outputs['sig']}")
 
             if outputs["cert"] is not None:
                 with outputs["cert"].open(mode="w") as io:
-                    print(result.cert_pem, file=io)
+                    print(cert_pem, file=io)
                 print(f"Certificate written to {outputs['cert']}")
 
             if outputs["bundle"] is not None:
                 with outputs["bundle"].open(mode="w") as io:
-                    print(result.to_bundle().to_json(), file=io)
+                    print(result.to_json(), file=io)
                 print(f"Sigstore bundle written to {outputs['bundle']}")
 
 
 def _collect_verification_state(
     args: argparse.Namespace,
-) -> tuple[Verifier, list[tuple[Path, VerificationMaterials]]]:
+) -> tuple[Verifier, list[tuple[Path, Hashed, Bundle]]]:
     """
     Performs CLI functionality common across all `sigstore verify` subcommands.
 
-    Returns a tuple of the active verifier instance and a list of `(file, materials)`
-    tuples, where `file` is the path to the file being verified (for display
-    purposes) and `materials` is the `VerificationMaterials` to verify with.
+    Returns a tuple of the active verifier instance and a list of `(path, hashed, bundle)`
+    tuples, where `path` is the filename for display purposes, `hashed` is the
+    pre-hashed input to the file being verified and `bundle` is the `Bundle` to verify with.
     """
 
     # Fail if --certificate, --signature, or --bundle is specified and we
     # have more than one input.
     if (args.certificate or args.signature or args.bundle) and len(args.files) > 1:
         _die(
             args,
@@ -745,14 +684,18 @@
             "with a single input file",
         )
 
     # Fail if `--certificate` or `--signature` is used with `--bundle`.
     if args.bundle and (args.certificate or args.signature):
         _die(args, "--bundle cannot be used with --certificate or --signature")
 
+    # Fail if `--certificate` or `--signature` is used with `--offline`.
+    if args.offline and (args.certificate or args.signature):
+        _die(args, "--offline cannot be used with --certificate or --signature")
+
     # The converse of `sign`: we build up an expected input map and check
     # that we have everything so that we can fail early.
     input_map = {}
     for file in args.files:
         if not file.is_file():
             _die(args, f"Input must be a file: {file}")
 
@@ -769,15 +712,15 @@
             # NOTE(ww): If the user hasn't specified a bundle via `--bundle` and
             # `{input}.sigstore.json` doesn't exist, then we try `{input}.sigstore`
             # for backwards compatibility.
             legacy_default_bundle = file.parent / f"{file.name}.sigstore"
             bundle = file.parent / f"{file.name}.sigstore.json"
 
             if not bundle.is_file() and legacy_default_bundle.is_file():
-                logger.warning(
+                _logger.warning(
                     f"{file}: {legacy_default_bundle} should be named {bundle}. "
                     "Support for discovering 'bare' .sigstore inputs will be deprecated in "
                     "a future release."
                 )
                 bundle = legacy_default_bundle
             elif bundle.is_file() and legacy_default_bundle.is_file():
                 # Don't allow the user to implicitly verify `{input}.sigstore.json` if
@@ -804,163 +747,85 @@
             input_map[file] = {"bundle": bundle}
 
         if missing:
             _die(
                 args,
                 f"Missing verification materials for {(file)}: {', '.join(missing)}",
             )
-
     if args.staging:
-        logger.debug("verify: staging instances requested")
+        _logger.debug("verify: staging instances requested")
         verifier = Verifier.staging()
     elif args.rekor_url == DEFAULT_REKOR_URL:
         verifier = Verifier.production()
     else:
-        if not args.certificate_chain:
-            _die(args, "Custom Rekor URL used without specifying --certificate-chain")
-
-        try:
-            certificate_chain = load_pem_x509_certificates(
-                args.certificate_chain.read()
-            )
-        except ValueError as error:
-            _die(args, f"Invalid certificate chain: {error}")
-
-        if args.rekor_root_pubkey is not None:
-            rekor_keys = [args.rekor_root_pubkey.read()]
-        else:
-            updater = TrustUpdater.production()
-            rekor_keys = updater.get_rekor_keys()
-
+        trusted_root = TrustedRoot.production(purpose=KeyringPurpose.VERIFY)
         verifier = Verifier(
             rekor=RekorClient(
                 url=args.rekor_url,
-                rekor_keyring=RekorKeyring(Keyring(rekor_keys)),
-                # We don't use the CT keyring in verification so we can supply an empty keyring
-                ct_keyring=CTKeyring(Keyring()),
             ),
-            fulcio_certificate_chain=certificate_chain,
+            trusted_root=trusted_root,
         )
 
     all_materials = []
     for file, inputs in input_map.items():
-        cert_pem: str
-        signature: bytes
-        entry: LogEntry | None = None
+        with file.open(mode="rb") as io:
+            hashed = sha256_digest(io)
+
         if "bundle" in inputs:
             # Load the bundle
-            logger.debug(f"Using bundle from: {inputs['bundle']}")
+            _logger.debug(f"Using bundle from: {inputs['bundle']}")
 
             bundle_bytes = inputs["bundle"].read_bytes()
-            bundle = Bundle().from_json(bundle_bytes)
-
-            with file.open(mode="rb", buffering=0) as io:
-                materials = VerificationMaterials.from_bundle(
-                    input_=io, bundle=bundle, offline=args.offline
-                )
+            bundle = Bundle.from_json(bundle_bytes)
         else:
             # Load the signing certificate
-            logger.debug(f"Using certificate from: {inputs['cert']}")
-            cert_pem = inputs["cert"].read_text()
+            _logger.debug(f"Using certificate from: {inputs['cert']}")
+            cert = load_pem_x509_certificate(inputs["cert"].read_bytes())
 
             # Load the signature
-            logger.debug(f"Using signature from: {inputs['sig']}")
+            _logger.debug(f"Using signature from: {inputs['sig']}")
             b64_signature = inputs["sig"].read_text()
             signature = base64.b64decode(b64_signature)
 
-            with file.open(mode="rb", buffering=0) as io:
-                materials = VerificationMaterials(
-                    input_=io,
-                    cert_pem=PEMCert(cert_pem),
-                    signature=signature,
-                    rekor_entry=entry,
-                    offline=args.offline,
-                )
-
-        logger.debug(f"Verifying contents from: {file}")
-
-        with file.open(mode="rb", buffering=0) as io:
-            all_materials.append((file, materials))
-
-    return (verifier, all_materials)
-
-
-class VerificationError(Error):
-    """Raised when the verifier returns a `VerificationFailure` result."""
-
-    def __init__(self, result: VerificationFailure):
-        self.message = f"Verification failed: {result.reason}"
-        self.result = result
-
-    def diagnostics(self) -> str:
-        message = f"Failure reason: {self.result.reason}\n"
-
-        if isinstance(self.result, CertificateVerificationFailure):
-            message += dedent(
-                f"""
-                The given certificate could not be verified against the
-                root of trust.
-
-                This may be a result of connecting to the wrong Fulcio instance
-                (for example, staging instead of production, or vice versa).
-
-                Additional context:
-
-                {self.result.exception}
-                """
+            # When using "detached" materials, we *must* retrieve the log
+            # entry from the online log.
+            # TODO: This should be abstracted somewhere much better.
+            log_entry = verifier._rekor.log.entries.retrieve.post(
+                _hashedrekord_from_parts(cert, signature, hashed)
             )
-        elif isinstance(self.result, LogEntryMissing):
-            message += dedent(
-                f"""
-                These signing artifacts could not be matched to a entry
-                in the configured transparency log.
+            if log_entry is None:
+                _die(args, f"No matching log entry for {file}'s verification materials")
+            bundle = Bundle.from_parts(cert, signature, log_entry)
 
-                This may be a result of connecting to the wrong Rekor instance
-                (for example, staging instead of production, or vice versa).
+        _logger.debug(f"Verifying contents from: {file}")
 
-                Additional context:
+        all_materials.append((file, hashed, bundle))
 
-                Signature: {self.result.signature}
-
-                Artifact hash: {self.result.artifact_hash}
-                """
-            )
-        else:
-            message += dedent(
-                f"""
-                A verification error occurred.
-
-                Additional context:
-
-                {self.result}
-                """
-            )
-
-        return message
+    return (verifier, all_materials)
 
 
 def _verify_identity(args: argparse.Namespace) -> None:
-    verifier, files_with_materials = _collect_verification_state(args)
+    verifier, materials = _collect_verification_state(args)
 
-    for file, materials in files_with_materials:
+    for file, hashed, bundle in materials:
         policy_ = policy.Identity(
             identity=args.cert_identity,
             issuer=args.cert_oidc_issuer,
         )
 
-        result = verifier.verify(
-            materials=materials,
-            policy=policy_,
-        )
-
-        if result:
+        try:
+            verifier.verify_artifact(
+                input_=hashed,
+                bundle=bundle,
+                policy=policy_,
+            )
             print(f"OK: {file}")
-        else:
-            print(f"FAIL: {file}")
-            raise VerificationError(cast(VerificationFailure, result))
+        except VerificationError as exc:
+            _logger.error(f"FAIL: {file}")
+            exc.log_and_exit(_logger, args.verbose >= 1)
 
 
 def _verify_github(args: argparse.Namespace) -> None:
     # Every GitHub verification begins with an identity policy,
     # for which we know the issuer URL ahead of time.
     # We then add more policies, as configured by the user's passed-in options.
     inner_policies: list[policy.VerificationPolicy] = [
@@ -979,23 +844,22 @@
     if args.workflow_repository:
         inner_policies.append(policy.GitHubWorkflowRepository(args.workflow_repository))
     if args.workflow_ref:
         inner_policies.append(policy.GitHubWorkflowRef(args.workflow_ref))
 
     policy_ = policy.AllOf(inner_policies)
 
-    verifier, files_with_materials = _collect_verification_state(args)
-    for file, materials in files_with_materials:
-        result = verifier.verify(materials=materials, policy=policy_)
-
-        if result:
+    verifier, materials = _collect_verification_state(args)
+    for file, hashed, bundle in materials:
+        try:
+            verifier.verify_artifact(input_=hashed, bundle=bundle, policy=policy_)
             print(f"OK: {file}")
-        else:
-            print(f"FAIL: {file}")
-            raise VerificationError(cast(VerificationFailure, result))
+        except VerificationError as exc:
+            _logger.error(f"FAIL: {file}")
+            exc.log_and_exit(_logger, args.verbose >= 1)
 
 
 def _get_identity(args: argparse.Namespace) -> Optional[IdentityToken]:
     token = None
     if not args.oidc_disable_ambient_providers:
         token = detect_credential()
```

### Comparing `sigstore-2.1.5/sigstore/_internal/__init__.py` & `sigstore-3.0.0rc1/sigstore/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/sigstore/_internal/ctfe.py` & `sigstore-3.0.0rc1/sigstore/_internal/oidc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Functionality for interacting with CT ("CTFE") signing keys.
+Internal OIDC and OAuth functionality for sigstore-python.
 """
-
-from typing import NewType
-
-from sigstore._internal.keyring import Keyring
-
-CTKeyring = NewType("CTKeyring", Keyring)
```

### Comparing `sigstore-2.1.5/sigstore/_internal/fulcio/__init__.py` & `sigstore-3.0.0rc1/sigstore/_internal/fulcio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 APIs for interacting with Fulcio.
 """
 
-
 from .client import (
     DetachedFulcioSCT,
     ExpiredCertificate,
     FulcioCertificateSigningResponse,
     FulcioClient,
 )
```

### Comparing `sigstore-2.1.5/sigstore/_internal/fulcio/client.py` & `sigstore-3.0.0rc1/sigstore/_internal/fulcio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,29 +30,32 @@
 from urllib.parse import urljoin
 
 import requests
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.x509 import (
     Certificate,
     CertificateSigningRequest,
-    PrecertificateSignedCertificateTimestamps,
     load_pem_x509_certificate,
 )
 from cryptography.x509.certificate_transparency import (
     LogEntryType,
     SignatureAlgorithm,
     SignedCertificateTimestamp,
     Version,
 )
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 
+from sigstore._internal.sct import (
+    UnexpectedSctCountException,
+    _get_precertificate_signed_certificate_timestamps,
+)
 from sigstore._utils import B64Str
 from sigstore.oidc import IdentityToken
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 DEFAULT_FULCIO_URL = "https://fulcio.sigstore.dev"
 STAGING_FULCIO_URL = "https://fulcio.sigstage.dev"
 SIGNING_CERT_ENDPOINT = "/api/v2/signingCert"
 TRUST_BUNDLE_ENDPOINT = "/api/v2/trustBundle"
 
 
@@ -262,24 +265,21 @@
             raise FulcioClientError(
                 f"Certificate chain is too short: {len(certificates)} < 2"
             )
         cert = load_pem_x509_certificate(certificates[0].encode())
         chain = [load_pem_x509_certificate(c.encode()) for c in certificates[1:]]
 
         if sct_embedded:
-            # Try to retrieve the embedded SCTs within the cert.
-            precert_scts_extension = cert.extensions.get_extension_for_class(
-                PrecertificateSignedCertificateTimestamps
-            ).value
+            try:
+                # The SignedCertificateTimestamp should be acessed by the index 0
+                sct = _get_precertificate_signed_certificate_timestamps(cert)[0]
+
+            except UnexpectedSctCountException as ex:
+                raise FulcioClientError(ex)
 
-            if len(precert_scts_extension) != 1:
-                raise FulcioClientError(
-                    f"Unexpected embedded SCT count in response: {len(precert_scts_extension)} != 1"
-                )
-            sct = precert_scts_extension[0]
         else:
             # If we don't have any embedded SCTs, then we might be dealing
             # with a Fulcio instance that provides detached SCTs.
 
             # The detached SCT is a base64-encoded payload, which in turn
             # is a JSON representation of the SignedCertificateTimestamp
             # in RFC 6962 (subsec. 3.2).
@@ -331,15 +331,15 @@
 
 
 class FulcioClient:
     """The internal Fulcio client"""
 
     def __init__(self, url: str = DEFAULT_FULCIO_URL) -> None:
         """Initialize the client"""
-        logger.debug(f"Fulcio client using URL: {url}")
+        _logger.debug(f"Fulcio client using URL: {url}")
         self.url = url
         self.session = requests.Session()
 
     def __del__(self) -> None:
         """
         Destroys the underlying network session.
         """
```

### Comparing `sigstore-2.1.5/sigstore/_internal/merkle.py` & `sigstore-3.0.0rc1/sigstore/_internal/merkle.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,29 +17,27 @@
 
 This code is based off Google's Trillian Merkle Tree implementation which Cosign uses to validate
 Rekor entries.
 
 The data format for the Merkle tree nodes is described in IETF's RFC 6962.
 """
 
+from __future__ import annotations
+
 import base64
 import hashlib
 import struct
+import typing
 from typing import List, Tuple
 
 from sigstore._utils import HexStr
-from sigstore.transparency import LogEntry
-
-
-class InvalidInclusionProofError(Exception):
-    """
-    Raised if the Merkle inclusion proof fails.
-    """
+from sigstore.errors import VerificationError
 
-    pass
+if typing.TYPE_CHECKING:
+    from sigstore.models import LogEntry
 
 
 _LEAF_HASH_PREFIX = 0
 _NODE_HASH_PREFIX = 1
 
 
 def _decomp_inclusion_proof(index: int, size: int) -> Tuple[int, int]:
@@ -95,26 +93,24 @@
     data = struct.pack(pattern, _LEAF_HASH_PREFIX, leaf)
     return hashlib.sha256(data).digest()
 
 
 def verify_merkle_inclusion(entry: LogEntry) -> None:
     """Verify the Merkle Inclusion Proof for a given Rekor entry."""
     inclusion_proof = entry.inclusion_proof
-    if inclusion_proof is None:
-        raise InvalidInclusionProofError("Rekor entry has no inclusion proof")
 
     # Figure out which subset of hashes corresponds to the inner and border nodes.
     inner, border = _decomp_inclusion_proof(
         inclusion_proof.log_index, inclusion_proof.tree_size
     )
 
     # Check against the number of hashes.
     if len(inclusion_proof.hashes) != (inner + border):
-        raise InvalidInclusionProofError(
-            f"Inclusion proof has wrong size: expected {inner + border}, got "
+        raise VerificationError(
+            f"inclusion proof has wrong size: expected {inner + border}, got "
             f"{len(inclusion_proof.hashes)}"
         )
 
     # The new entry's hash isn't included in the inclusion proof so we should calculate this
     # ourselves.
     leaf_hash: bytes = _hash_leaf(base64.b64decode(entry.body))
 
@@ -125,11 +121,11 @@
     )
 
     calc_hash: HexStr = HexStr(
         _chain_border_right(intermediate_result, inclusion_proof.hashes[inner:]).hex()
     )
 
     if calc_hash != inclusion_proof.root_hash:
-        raise InvalidInclusionProofError(
-            f"Inclusion proof contains invalid root hash: expected {inclusion_proof}, calculated "
+        raise VerificationError(
+            f"inclusion proof contains invalid root hash: expected {inclusion_proof}, calculated "
             f"{calc_hash}"
         )
```

### Comparing `sigstore-2.1.5/sigstore/_internal/oidc/oauth.py` & `sigstore-3.0.0rc1/sigstore/_internal/oidc/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from typing import Any, Dict, List, Optional, cast
 
 from id import IdentityError
 
 from sigstore._utils import B64Str
 from sigstore.oidc import Issuer
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 # This HTML is copied from the Go Sigstore library and was originally authored by Julien Vermette:
 #   https://github.com/sigstore/sigstore/blob/main/pkg/oauth/interactive.go
 AUTH_SUCCESS_HTML = """
 <html>
   <head>
@@ -124,21 +124,21 @@
 
 
 class _OAuthRedirectHandler(http.server.BaseHTTPRequestHandler):
     def log_message(self, _format: str, *_args: Any) -> None:
         pass
 
     def do_GET(self) -> None:
-        logger.debug(f"GET: {self.path} with {dict(self.headers)}")
+        _logger.debug(f"GET: {self.path} with {dict(self.headers)}")
         server = cast(_OAuthRedirectServer, self.server)
 
         # If the auth response has already been populated, the main thread will be stopping this
         # thread and accessing the auth response shortly so we should stop servicing any requests.
         if server.auth_response is not None:
-            logger.debug(f"{self.path} unavailable (teardown)")
+            _logger.debug(f"{self.path} unavailable (teardown)")
             self.send_response(404)
             return None
 
         r = urllib.parse.urlsplit(self.path)
 
         # We only understand two kinds of requests:
         # 1. The response from a successful OAuth redirect
@@ -245,12 +245,12 @@
         )
 
     @property
     def auth_endpoint(self) -> str:
         return self.oauth_session.auth_endpoint(self.redirect_uri)
 
     def enable_oob(self) -> None:
-        logger.debug("enabling out-of-band OAuth flow")
+        _logger.debug("enabling out-of-band OAuth flow")
         self._is_out_of_band = True
 
     def is_oob(self) -> bool:
         return self._is_out_of_band
```

### Comparing `sigstore-2.1.5/sigstore/_internal/rekor/checkpoint.py` & `sigstore-3.0.0rc1/sigstore/_internal/rekor/checkpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,23 +17,26 @@
 """
 
 from __future__ import annotations
 
 import base64
 import re
 import struct
+import typing
 from dataclasses import dataclass
 from typing import List
 
 from pydantic import BaseModel, Field, StrictStr
 
-from sigstore._internal.keyring import KeyringSignatureError
-from sigstore._internal.rekor.client import RekorClient
+from sigstore._internal.trustroot import RekorKeyring
 from sigstore._utils import KeyID
-from sigstore.transparency import LogEntry
+from sigstore.errors import VerificationError
+
+if typing.TYPE_CHECKING:
+    from sigstore.models import LogEntry
 
 
 @dataclass(frozen=True)
 class RekorSignature:
     """
     Represents a `RekorSignature` containing:
 
@@ -43,18 +46,14 @@
     """
 
     name: str
     sig_hash: bytes
     signature: bytes
 
 
-class CheckpointError(Exception):
-    """Raised during LogCheckpoint parsing or verification."""
-
-
 class LogCheckpoint(BaseModel):
     """
     Represents a Rekor `LogCheckpoint` containing:
 
     - an origin, e.g. "rekor.sigstage.dev - 8050909264565447525"
     - the size of the log,
     - the hash of the log,
@@ -72,19 +71,19 @@
     def from_text(cls, text: str) -> LogCheckpoint:
         """
         Serialize from the text header ("note") of a SignedNote.
         """
 
         lines = text.strip().split("\n")
         if len(lines) < 3:
-            raise CheckpointError("Malformed LogCheckpoint: too few items in header!")
+            raise VerificationError("malformed LogCheckpoint: too few items in header")
 
         origin = lines[0]
         if len(origin) == 0:
-            raise CheckpointError("Malformed LogCheckpoint: empty origin!")
+            raise VerificationError("malformed LogCheckpoint: empty origin")
 
         log_size = int(lines[1])
         root_hash = base64.b64decode(lines[2]).hex()
 
         return LogCheckpoint(
             origin=origin,
             log_size=log_size,
@@ -126,64 +125,69 @@
 
         This is derived from Rekor's `UnmarshalText`:
         <https://github.com/sigstore/rekor/blob/4b1fa6661cc6dfbc844b4c6ed9b1f44e7c5ae1c0/pkg/util/signed_note.go#L141>
         """
 
         separator: str = "\n\n"
         if text.count(separator) != 1:
-            raise CheckpointError(
-                "Note must contain one blank line, deliniating the text from the signature block"
+            raise VerificationError(
+                "note must contain one blank line, deliniating the text from the signature block"
             )
         split = text.index(separator)
 
         header: str = text[: split + 1]
         data: str = text[split + len(separator) :]
 
         if len(data) == 0:
-            raise CheckpointError(
-                "Malformed Note: must contain at least one signature!"
+            raise VerificationError(
+                "malformed Note: must contain at least one signature"
             )
         if data[-1] != "\n":
-            raise CheckpointError("Malformed Note: data section must end with newline!")
+            raise VerificationError(
+                "malformed Note: data section must end with newline"
+            )
 
         sig_parser = re.compile(r"\u2014 (\S+) (\S+)\n")
         signatures: list[RekorSignature] = []
         for name, signature in re.findall(sig_parser, data):
             signature_bytes: bytes = base64.b64decode(signature)
             if len(signature_bytes) < 5:
-                raise CheckpointError(
-                    "Malformed Note: signature contains too few bytes"
+                raise VerificationError(
+                    "malformed Note: signature contains too few bytes"
                 )
 
             signature = RekorSignature(
                 name=name,
                 sig_hash=struct.unpack(">4s", signature_bytes[0:4])[0],
                 signature=base64.b64encode(signature_bytes[4:]),
             )
             signatures.append(signature)
 
         return cls(note=header, signatures=signatures)
 
-    def verify(self, client: RekorClient, key_id: KeyID) -> None:
+    def verify(self, rekor_keyring: RekorKeyring, key_id: KeyID) -> None:
         """
-        Verify the `SignedNote` with using the given RekorClient by verifying each contained signature.
+        Verify the `SignedNote` using the given RekorKeyring by verifying
+        each contained signature.
         """
 
         note = str.encode(self.note)
 
         for sig in self.signatures:
             if sig.sig_hash != key_id[:4]:
-                raise CheckpointError("sig_hash hint does not match expected key_id")
+                raise VerificationError(
+                    "checkpoint: sig_hash hint does not match expected key_id"
+                )
 
             try:
-                client._rekor_keyring.verify(
+                rekor_keyring.verify(
                     key_id=key_id, signature=base64.b64decode(sig.signature), data=note
                 )
-            except KeyringSignatureError as sig_err:
-                raise CheckpointError("invalid signature") from sig_err
+            except VerificationError as sig_err:
+                raise VerificationError(f"checkpoint: invalid signature: {sig_err}")
 
 
 @dataclass(frozen=True)
 class SignedCheckpoint:
     """
     Represents a *signed* `Checkpoint`: a `LogCheckpoint` and its corresponding `SignedNote`.
     """
@@ -198,30 +202,32 @@
         """
 
         signed_note = SignedNote.from_text(text)
         checkpoint = LogCheckpoint.from_text(signed_note.note)
         return cls(signed_note=signed_note, checkpoint=checkpoint)
 
 
-def verify_checkpoint(client: RekorClient, entry: LogEntry) -> None:
+def verify_checkpoint(rekor_keyring: RekorKeyring, entry: LogEntry) -> None:
     """
     Verify the inclusion proof's checkpoint.
     """
 
     inclusion_proof = entry.inclusion_proof
     if inclusion_proof is None:
-        raise CheckpointError("Rekor entry has no inclusion proof")
+        raise VerificationError("Rekor entry has no inclusion proof")
 
     # verification occurs in two stages:
     # 1) verify the signature on the checkpoint
     # 2) verify the root hash in the checkpoint matches the root hash from the inclusion proof.
     signed_checkpoint = SignedCheckpoint.from_text(inclusion_proof.checkpoint)
-    signed_checkpoint.signed_note.verify(client, KeyID(bytes.fromhex(entry.log_id)))
+    signed_checkpoint.signed_note.verify(
+        rekor_keyring, KeyID(bytes.fromhex(entry.log_id))
+    )
 
     checkpoint_hash = signed_checkpoint.checkpoint.log_hash
     root_hash = inclusion_proof.root_hash
 
     if checkpoint_hash != root_hash:
-        raise CheckpointError(
+        raise VerificationError(
             "Inclusion proof contains invalid root hash signature: ",
             f"expected {str(checkpoint_hash)} got {str(root_hash)}",
         )
```

### Comparing `sigstore-2.1.5/sigstore/_internal/rekor/client.py` & `sigstore-3.0.0rc1/sigstore/_internal/rekor/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,37 +14,32 @@
 
 """
 Client implementation for interacting with Rekor.
 """
 
 from __future__ import annotations
 
+import json
 import logging
 from abc import ABC
 from dataclasses import dataclass
-from typing import Any, Dict, NewType, Optional
+from typing import Any, Dict, Optional
 from urllib.parse import urljoin
 
+import rekor_types
 import requests
-import sigstore_rekor_types
 
-from sigstore._internal.ctfe import CTKeyring
-from sigstore._internal.keyring import Keyring
-from sigstore._internal.tuf import TrustUpdater
-from sigstore.transparency import LogEntry
+from sigstore.models import LogEntry
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 DEFAULT_REKOR_URL = "https://rekor.sigstore.dev"
 STAGING_REKOR_URL = "https://rekor.sigstage.dev"
 
 
-RekorKeyring = NewType("RekorKeyring", Keyring)
-
-
 @dataclass(frozen=True)
 class RekorLogInfo:
     """
     Represents information about the Rekor log.
     """
 
     root_hash: str
@@ -68,15 +63,28 @@
 
 
 class RekorClientError(Exception):
     """
     A generic error in the Rekor client.
     """
 
-    pass
+    def __init__(self, http_error: requests.HTTPError):
+        """
+        Create a new `RekorClientError` from the given `requests.HTTPError`.
+        """
+        if http_error.response is not None:
+            try:
+                error = rekor_types.Error.model_validate_json(http_error.response.text)
+                super().__init__(f"{error.code}: {error.message}")
+            except Exception:
+                super().__init__(
+                    f"Rekor returned an unknown error with HTTP {http_error.response.status_code}"
+                )
+        else:
+            super().__init__(f"Unexpected Rekor error: {http_error}")
 
 
 class _Endpoint(ABC):
     def __init__(self, url: str, session: requests.Session) -> None:
         self.url = url
         self.session = session
 
@@ -90,15 +98,15 @@
         """
         Returns information about the Rekor instance's log.
         """
         resp: requests.Response = self.session.get(self.url)
         try:
             resp.raise_for_status()
         except requests.HTTPError as http_error:
-            raise RekorClientError from http_error
+            raise RekorClientError(http_error)
         return RekorLogInfo.from_response(resp.json())
 
     @property
     def entries(self) -> RekorEntries:
         """
         Returns a `RekorEntries` capable of accessing detailed information
         about individual log entries.
@@ -116,46 +124,49 @@
     ) -> LogEntry:
         """
         Retrieve a specific log entry, either by UUID or by log index.
 
         Either `uuid` or `log_index` must be present, but not both.
         """
         if not (bool(uuid) ^ bool(log_index)):
-            raise RekorClientError("uuid or log_index required, but not both")
+            raise ValueError("uuid or log_index required, but not both")
 
         resp: requests.Response
 
         if uuid is not None:
             resp = self.session.get(urljoin(self.url, uuid))
         else:
             resp = self.session.get(self.url, params={"logIndex": log_index})
 
         try:
             resp.raise_for_status()
         except requests.HTTPError as http_error:
-            raise RekorClientError from http_error
+            raise RekorClientError(http_error)
         return LogEntry._from_response(resp.json())
 
     def post(
         self,
-        proposed_entry: sigstore_rekor_types.Hashedrekord,
+        proposed_entry: rekor_types.Hashedrekord | rekor_types.Dsse,
     ) -> LogEntry:
         """
         Submit a new entry for inclusion in the Rekor log.
         """
 
-        resp: requests.Response = self.session.post(
-            self.url, json=proposed_entry.model_dump(mode="json", by_alias=True)
-        )
+        payload = proposed_entry.model_dump(mode="json", by_alias=True)
+        _logger.debug(f"proposed: {json.dumps(payload)}")
+
+        resp: requests.Response = self.session.post(self.url, json=payload)
         try:
             resp.raise_for_status()
         except requests.HTTPError as http_error:
-            raise RekorClientError from http_error
+            raise RekorClientError(http_error)
 
-        return LogEntry._from_response(resp.json())
+        integrated_entry = resp.json()
+        _logger.debug(f"integrated: {integrated_entry}")
+        return LogEntry._from_response(integrated_entry)
 
     @property
     def retrieve(self) -> RekorEntriesRetrieve:
         """
         Returns a `RekorEntriesRetrieve` capable of retrieving entries.
         """
         return RekorEntriesRetrieve(
@@ -166,15 +177,15 @@
 class RekorEntriesRetrieve(_Endpoint):
     """
     Represents the entry retrieval endpoints on a Rekor instance.
     """
 
     def post(
         self,
-        expected_entry: sigstore_rekor_types.Hashedrekord,
+        expected_entry: rekor_types.Hashedrekord | rekor_types.Dsse,
     ) -> Optional[LogEntry]:
         """
         Retrieves an extant Rekor entry, identified by its artifact signature,
         artifact hash, and signing certificate.
 
         Returns None if Rekor has no entry corresponding to the signing
         materials.
@@ -183,15 +194,15 @@
 
         resp: requests.Response = self.session.post(self.url, json=data)
         try:
             resp.raise_for_status()
         except requests.HTTPError as http_error:
             if http_error.response and http_error.response.status_code == 404:
                 return None
-            raise RekorClientError(resp.text) from http_error
+            raise RekorClientError(http_error)
 
         results = resp.json()
 
         # The response is a list of `{uuid: LogEntry}` objects.
         # We select the oldest entry for our actual return value,
         # since a malicious actor could conceivably spam the log with
         # newer duplicate entries.
@@ -206,66 +217,49 @@
 
         return oldest_entry
 
 
 class RekorClient:
     """The internal Rekor client"""
 
-    def __init__(
-        self, url: str, rekor_keyring: RekorKeyring, ct_keyring: CTKeyring
-    ) -> None:
+    def __init__(self, url: str) -> None:
         """
         Create a new `RekorClient` from the given URL.
         """
         self.url = urljoin(url, "api/v1/")
         self.session = requests.Session()
         self.session.headers.update(
             {"Content-Type": "application/json", "Accept": "application/json"}
         )
 
-        self._ct_keyring = ct_keyring
-        self._rekor_keyring = rekor_keyring
-
     def __del__(self) -> None:
         """
         Terminates the underlying network session.
         """
         self.session.close()
 
     @classmethod
-    def production(cls, updater: TrustUpdater) -> RekorClient:
+    def production(cls) -> RekorClient:
         """
         Returns a `RekorClient` populated with the default Rekor production instance.
 
-        updater must be a `TrustUpdater` for the production TUF repository.
+        trust_root must be a `TrustedRoot` for the production TUF repository.
         """
-        rekor_keys = updater.get_rekor_keys()
-        ctfe_keys = updater.get_ctfe_keys()
-
         return cls(
             DEFAULT_REKOR_URL,
-            RekorKeyring(Keyring(rekor_keys)),
-            CTKeyring(Keyring(ctfe_keys)),
         )
 
     @classmethod
-    def staging(cls, updater: TrustUpdater) -> RekorClient:
+    def staging(cls) -> RekorClient:
         """
         Returns a `RekorClient` populated with the default Rekor staging instance.
 
-        updater must be a `TrustUpdater` for the staging TUF repository.
+        trust_root must be a `TrustedRoot` for the staging TUF repository.
         """
-        rekor_keys = updater.get_rekor_keys()
-        ctfe_keys = updater.get_ctfe_keys()
-
-        return cls(
-            STAGING_REKOR_URL,
-            RekorKeyring(Keyring(rekor_keys)),
-            CTKeyring(Keyring(ctfe_keys)),
-        )
+        return cls(STAGING_REKOR_URL)
 
     @property
     def log(self) -> RekorLog:
         """
         Returns a `RekorLog` adapter for making requests to a Rekor log.
         """
         return RekorLog(urljoin(self.url, "log/"), session=self.session)
```

### Comparing `sigstore-2.1.5/sigstore/_internal/sct.py` & `sigstore-3.0.0rc1/sigstore/_internal/sct.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,78 +15,78 @@
 """
 Utilities for verifying signed certificate timestamps.
 """
 
 import logging
 import struct
 from datetime import timezone
-from textwrap import dedent
 from typing import List, Optional
 
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
-from cryptography.x509 import Certificate, ExtendedKeyUsage, ExtensionNotFound
+from cryptography.x509 import (
+    Certificate,
+    ExtendedKeyUsage,
+    ExtensionNotFound,
+    PrecertificateSignedCertificateTimestamps,
+)
 from cryptography.x509.certificate_transparency import (
     LogEntryType,
     SignedCertificateTimestamp,
 )
 from cryptography.x509.oid import ExtendedKeyUsageOID
 
-from sigstore._internal.ctfe import CTKeyring
-from sigstore._internal.keyring import (
-    KeyringError,
-    KeyringLookupError,
-    KeyringSignatureError,
-)
+from sigstore._internal.trustroot import CTKeyring
 from sigstore._utils import (
     DERCert,
-    InvalidCertError,
     KeyID,
     cert_is_ca,
     key_id,
 )
-from sigstore.errors import Error
+from sigstore.errors import VerificationError
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 def _pack_signed_entry(
     sct: SignedCertificateTimestamp, cert: Certificate, issuer_key_id: Optional[bytes]
 ) -> bytes:
     fields = []
     if sct.entry_type == LogEntryType.X509_CERTIFICATE:
         # When dealing with a "normal" certificate, our signed entry looks like this:
         #
         # [0]: opaque ASN.1Cert<1..2^24-1>
         pack_format = "!BBB{cert_der_len}s"
         cert_der = DERCert(cert.public_bytes(encoding=serialization.Encoding.DER))
     elif sct.entry_type == LogEntryType.PRE_CERTIFICATE:
         if not issuer_key_id or len(issuer_key_id) != 32:
-            raise InvalidSCTError("API misuse: issuer key ID missing")
+            raise VerificationError("API misuse: issuer key ID missing")
 
         # When dealing with a precertificate, our signed entry looks like this:
         #
         # [0]: issuer_key_id[32]
         # [1]: opaque TBSCertificate<1..2^24-1>
         pack_format = "!32sBBB{cert_der_len}s"
 
         # Precertificates must have their SCT list extension filtered out.
         cert_der = DERCert(cert.tbs_precertificate_bytes)
         fields.append(issuer_key_id)
     else:
-        raise InvalidSCTError(f"unknown SCT log entry type: {sct.entry_type!r}")
+        raise VerificationError(f"unknown SCT log entry type: {sct.entry_type!r}")
 
     # The `opaque` length is a u24, which isn't directly supported by `struct`.
     # So we have to decompose it into 3 bytes.
     unused, len1, len2, len3 = struct.unpack(
         "!4B",
         struct.pack("!I", len(cert_der)),
     )
     if unused:
-        raise InvalidSCTError(f"Unexpectedly large certificate length: {len(cert_der)}")
+        raise VerificationError(
+            f"Unexpectedly large certificate length: {len(cert_der)}"
+        )
 
     pack_format = pack_format.format(cert_der_len=len(cert_der))
     fields.extend((len1, len2, len3, cert_der))
 
     return struct.pack(pack_format, *fields)
 
 
@@ -102,15 +102,15 @@
 
     The format of the digitaly signed data is described in IETF's RFC 6962.
     """
 
     # No extensions are currently specified, so we treat the presence
     # of any extension bytes as suspicious.
     if len(sct.extension_bytes) != 0:
-        raise InvalidSCTError("Unexpected trailing extension bytes")
+        raise VerificationError("Unexpected trailing extension bytes")
 
     # This constructs the "core" `signed_entry` field, which is either
     # the public bytes of the cert *or* the TBSPrecertificate (with some
     # filtering), depending on whether our SCT is for a precertificate.
     signed_entry = _pack_signed_entry(sct, cert, issuer_key_id)
 
     # Assemble a format string with the certificate length baked in and then pack the digitally
@@ -145,93 +145,50 @@
 def _get_issuer_cert(chain: List[Certificate]) -> Certificate:
     issuer = chain[0]
     if _is_preissuer(issuer):
         issuer = chain[1]
     return issuer
 
 
-def _cert_is_ca(cert: Certificate) -> bool:
-    logger.debug(f"Found {cert.subject} as issuer, verifying if it is a ca")
-    try:
-        cert_is_ca(cert)
-    except InvalidCertError as e:
-        logger.debug(f"Invalid {cert.subject}: failed to validate as a CA: {e}")
-        return False
-    return True
-
-
-class InvalidSCTError(Error):
-    """
-    Raised during SCT verification if an SCT is invalid in some way.
+class UnexpectedSctCountException(Exception):
     """
-
-    def diagnostics(self) -> str:
-        """Returns diagnostics for the error."""
-
-        ctx = f"\nContext: {self.__context__}" if self.__context__ else ""
-        return dedent(
-            f"""
-            SCT verification failed.
-
-            Additional context:
-
-            Message: {str(self)}
-            """
-            + ctx
-        )
-
-
-class InvalidSCTKeyError(InvalidSCTError):
-    """
-    Raised during SCT verification if the SCT can't be validated against the given keyring.
-
-    We specialize this error case, since it usually indicates one of
-    two conditions: either the current sigstore client is out-of-date,
-    or that the SCT is well-formed but invalid for the current configuration
-    (indicating that the user has asked for the wrong instance).
+    Number of percerts scts is wrong
     """
 
-    def diagnostics(self) -> str:
-        """Returns diagnostics for the error."""
-        return dedent(
-            f"""
-                Invalid key ID in SCT: not found in current keyring.
+    pass
 
-                This may be a result of an outdated `sigstore` installation.
 
-                Consider upgrading with:
-
-                    python -m pip install --upgrade sigstore
-
-                Additional context:
-
-                {self.__cause__}
-                """
+def _get_precertificate_signed_certificate_timestamps(
+    certificate: Certificate,
+) -> PrecertificateSignedCertificateTimestamps:
+    # Try to retrieve the embedded SCTs within the cert.
+    try:
+        precert_scts_extension = certificate.extensions.get_extension_for_class(
+            PrecertificateSignedCertificateTimestamps
+        ).value
+    except ExtensionNotFound:
+        raise ValueError(
+            "No PrecertificateSignedCertificateTimestamps found for the certificate"
         )
 
+    if len(precert_scts_extension) != 1:
+        raise UnexpectedSctCountException(
+            f"Unexpected embedded SCT count in response: {len(precert_scts_extension)} != 1"
+        )
+    return precert_scts_extension
 
-class SCTSignatureError(InvalidSCTError):
-    """
-    Raised during SCT verification if the signature of the SCT is invalid.
-    """
-
-    def diagnostics(self) -> str:
-        """Returns diagnostics for the error."""
-        return dedent(
-            f"""
-            Invalid signature on SCT.
-
-            If validating a certificate, the certificate associated with this
-            SCT should not be trusted.
-
-            Additional context:
 
-            {self.__cause__}
-            """
-        )
+def _cert_is_ca(cert: Certificate) -> bool:
+    _logger.debug(f"Found {cert.subject} as issuer, verifying if it is a ca")
+    try:
+        cert_is_ca(cert)
+    except VerificationError as e:
+        _logger.debug(f"Invalid {cert.subject}: failed to validate as a CA: {e}")
+        return False
+    return True
 
 
 def verify_sct(
     sct: SignedCertificateTimestamp,
     cert: Certificate,
     chain: List[Certificate],
     ct_keyring: CTKeyring,
@@ -251,41 +208,37 @@
         # find its issuer in the chain and calculate a hash over
         # its public key information, as part of the "binding" proof
         # that ties the issuer to the final certificate.
         issuer_cert = _get_issuer_cert(chain)
         issuer_pubkey = issuer_cert.public_key()
 
         if not _cert_is_ca(issuer_cert):
-            raise InvalidSCTError(
-                f"Invalid issuer pubkey basicConstraint (not a CA): {issuer_pubkey}"
+            raise VerificationError(
+                f"SCT verify: Invalid issuer pubkey basicConstraint (not a CA): {issuer_pubkey}"
             )
 
         if not isinstance(issuer_pubkey, (rsa.RSAPublicKey, ec.EllipticCurvePublicKey)):
-            raise InvalidSCTError(
-                f"invalid issuer pubkey format (not ECDSA or RSA): {issuer_pubkey}"
+            raise VerificationError(
+                f"SCT verify: invalid issuer pubkey format (not ECDSA or RSA): {issuer_pubkey}"
             )
 
         issuer_key_id = key_id(issuer_pubkey)
 
     digitally_signed = _pack_digitally_signed(sct, cert, issuer_key_id)
 
     if not isinstance(sct.signature_hash_algorithm, hashes.SHA256):
-        raise InvalidSCTError(
+        raise VerificationError(
             "Found unexpected hash algorithm in SCT: only SHA256 is supported "
             f"(expected {hashes.SHA256}, got {sct.signature_hash_algorithm})"
         )
 
     try:
-        logger.debug(f"attempting to verify SCT with key ID {sct.log_id.hex()}")
+        _logger.debug(f"attempting to verify SCT with key ID {sct.log_id.hex()}")
         # NOTE(ww): In terms of the DER structure, the SCT's `LogID` contains a
         # singular `opaque key_id[32]`. Cryptography's APIs don't bother
         # to expose this trivial single member, so we use the `log_id`
         # attribute directly.
         ct_keyring.verify(
             key_id=KeyID(sct.log_id), signature=sct.signature, data=digitally_signed
         )
-    except KeyringLookupError as exc:
-        raise InvalidSCTKeyError from exc
-    except KeyringSignatureError as exc:
-        raise SCTSignatureError from exc
-    except KeyringError as exc:
-        raise InvalidSCTError from exc
+    except VerificationError as exc:
+        raise VerificationError(f"SCT verify failed: {exc}")
```

### Comparing `sigstore-2.1.5/sigstore/_store/__init__.py` & `sigstore-3.0.0rc1/sigstore/_store/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/sigstore/_store/prod/root.json` & `sigstore-3.0.0rc1/sigstore/_store/prod/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/sigstore/_store/prod/trusted_root.json` & `sigstore-3.0.0rc1/sigstore/_store/prod/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/sigstore/_store/staging/root.json` & `sigstore-3.0.0rc1/sigstore/_store/staging/root.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9017857142857143%*

 * *Differences: {"'signatures'": "{0: {'sig': "*

 * *                 "'3044022006fe8fff51d18753aeff141f81a962b8ac33f49831bbbec1334b2733ea96890002206e6f343c9c7b98a2ebd1f0b51aa5286ed3a4d48e271c77d88ea77499231bff5c'}}",*

 * * "'signed'": "{'version': 4, 'expires': '2029-03-05T22:50:21Z'}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "signatures": [
         {
             "keyid": "c8e09a68b5821b75462ae0df52151c81deb7f1838246dc1da8c34cc91ec12bda",
-            "sig": "304602210085927cdb96e1d9d0876bfc26b6ceea7421a54f959e30b9af3e12d31f6c750543022100dde611b58a1f2b9fb26c43767138c68f4422cdeb898c8b63f3f0193791030d12"
+            "sig": "3044022006fe8fff51d18753aeff141f81a962b8ac33f49831bbbec1334b2733ea96890002206e6f343c9c7b98a2ebd1f0b51aa5286ed3a4d48e271c77d88ea77499231bff5c"
         }
     ],
     "signed": {
         "_type": "root",
         "consistent_snapshot": true,
-        "expires": "2024-09-29T16:47:17Z",
+        "expires": "2029-03-05T22:50:21Z",
         "keys": {
             "314ae73abd3012fc73bfcc3783e31d03852716597642b891d6a33155c4baf600": {
                 "keyid_hash_algorithms": [
                     "sha256",
                     "sha512"
                 ],
                 "keytype": "ecdsa-sha2-nistp256",
@@ -56,10 +56,10 @@
                 "keyids": [
                     "314ae73abd3012fc73bfcc3783e31d03852716597642b891d6a33155c4baf600"
                 ],
                 "threshold": 1
             }
         },
         "spec_version": "1.0",
-        "version": 1
+        "version": 4
     }
 }
```

### Comparing `sigstore-2.1.5/sigstore/_utils.py` & `sigstore-3.0.0rc1/sigstore/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,31 +17,41 @@
 """
 
 from __future__ import annotations
 
 import base64
 import hashlib
 import sys
-from typing import IO, NewType, Union
+from enum import Enum
+from typing import IO, NewType, Type, Union
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
-from cryptography.x509 import Certificate, ExtensionNotFound, Version
+from cryptography.x509 import (
+    Certificate,
+    ExtensionNotFound,
+    Version,
+    load_der_x509_certificate,
+)
 from cryptography.x509.oid import ExtendedKeyUsageOID, ExtensionOID
+from sigstore_protobuf_specs.dev.sigstore.common.v1 import HashAlgorithm
 
-from sigstore.errors import Error
+from sigstore import hashes as sigstore_hashes
+from sigstore.errors import VerificationError
 
 if sys.version_info < (3, 11):
     import importlib_resources as resources
 else:
     from importlib import resources
 
 
 PublicKey = Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey]
 
+PublicKeyTypes = Union[Type[rsa.RSAPublicKey], Type[ec.EllipticCurvePublicKey]]
+
 HexStr = NewType("HexStr", str)
 """
 A newtype for `str` objects that contain hexadecimal strings (e.g. `ffabcd00ff`).
 """
 B64Str = NewType("B64Str", str)
 """
 A newtype for `str` objects that contain base64 encoded strings.
@@ -56,95 +66,131 @@
 """
 KeyID = NewType("KeyID", bytes)
 """
 A newtype for `bytes` objects that contain a key id.
 """
 
 
-class InvalidKeyError(Error):
-    """
-    Raised when loading a key fails.
-    """
-
-    pass
-
-
-class InvalidCertError(Error):
+class BundleType(str, Enum):
     """
-    Raised when loading or evaluating a certificate fails.
+    Known Sigstore bundle media types.
     """
 
+    BUNDLE_0_1 = "application/vnd.dev.sigstore.bundle+json;version=0.1"
+    BUNDLE_0_2 = "application/vnd.dev.sigstore.bundle+json;version=0.2"
+    BUNDLE_0_3_ALT = "application/vnd.dev.sigstore.bundle+json;version=0.3"
+    BUNDLE_0_3 = "application/vnd.dev.sigstore.bundle.v0.3+json"
 
-class UnexpectedKeyFormatError(InvalidKeyError):
-    """
-    Raised when loading a key produces a key of an unexpected type.
-    """
+    def __str__(self) -> str:
+        """Returns the variant's string value."""
+        return self.value
 
-    pass
 
-
-def load_pem_public_key(key_pem: bytes) -> PublicKey:
+def load_pem_public_key(
+    key_pem: bytes,
+    *,
+    types: tuple[PublicKeyTypes, ...] = (rsa.RSAPublicKey, ec.EllipticCurvePublicKey),
+) -> PublicKey:
     """
     A specialization of `cryptography`'s `serialization.load_pem_public_key`
-    with a uniform exception type (`InvalidKeyError`) and additional restrictions
-    on key validity (only RSA and ECDSA keys are valid).
+    with a uniform exception type (`VerificationError`) and filtering on valid key types
+    for Sigstore purposes.
     """
 
     try:
         key = serialization.load_pem_public_key(key_pem)
     except Exception as exc:
-        raise InvalidKeyError("could not load PEM-formatted public key") from exc
+        raise VerificationError("could not load PEM-formatted public key") from exc
 
-    if not isinstance(key, (rsa.RSAPublicKey, ec.EllipticCurvePublicKey)):
-        raise UnexpectedKeyFormatError(f"invalid key format (not ECDSA or RSA): {key}")
+    if not isinstance(key, types):
+        raise VerificationError(f"invalid key format: not one of {types}")
 
-    return key
+    return key  # type: ignore[return-value]
 
 
-def load_der_public_key(key_der: bytes) -> PublicKey:
+def load_der_public_key(
+    key_der: bytes,
+    *,
+    types: tuple[PublicKeyTypes, ...] = (rsa.RSAPublicKey, ec.EllipticCurvePublicKey),
+) -> PublicKey:
     """
     The `load_pem_public_key` specialization, but DER.
     """
 
     try:
         key = serialization.load_der_public_key(key_der)
     except Exception as exc:
-        raise InvalidKeyError("could not load DER-formatted public key") from exc
+        raise VerificationError("could not load DER-formatted public key") from exc
 
-    if not isinstance(key, (rsa.RSAPublicKey, ec.EllipticCurvePublicKey)):
-        raise UnexpectedKeyFormatError(f"invalid key format (not ECDSA or RSA): {key}")
+    if not isinstance(key, types):
+        raise VerificationError(f"invalid key format: not one of {types}")
 
-    return key
+    return key  # type: ignore[return-value]
 
 
 def base64_encode_pem_cert(cert: Certificate) -> B64Str:
     """
     Returns a string containing a base64-encoded PEM-encoded X.509 certificate.
     """
 
     return B64Str(
         base64.b64encode(cert.public_bytes(serialization.Encoding.PEM)).decode()
     )
 
 
+def cert_der_to_pem(der: bytes) -> str:
+    """
+    Converts a DER-encoded X.509 certificate into its PEM encoding.
+
+    Returns a string containing a PEM-encoded X.509 certificate.
+    """
+
+    # NOTE: Technically we don't have to round-trip like this, since
+    # the DER-to-PEM transformation is entirely mechanical.
+    cert = load_der_x509_certificate(der)
+    return cert.public_bytes(serialization.Encoding.PEM).decode()
+
+
 def key_id(key: PublicKey) -> KeyID:
     """
     Returns an RFC 6962-style "key ID" for the given public key.
 
     See: <https://www.rfc-editor.org/rfc/rfc6962#section-3.2>
     """
     public_bytes = key.public_bytes(
         encoding=serialization.Encoding.DER,
         format=serialization.PublicFormat.SubjectPublicKeyInfo,
     )
 
     return KeyID(hashlib.sha256(public_bytes).digest())
 
 
-def sha256_streaming(io: IO[bytes]) -> bytes:
+def sha256_digest(
+    input_: bytes | IO[bytes] | sigstore_hashes.Hashed,
+) -> sigstore_hashes.Hashed:
+    """
+    Compute the SHA256 digest of an input stream or buffer or,
+    if given a `Hashed`, return it directly.
+    """
+    if isinstance(input_, sigstore_hashes.Hashed):
+        return input_
+
+    # If the input is already buffered into memory, there's no point in
+    # going back through an I/O abstraction.
+    if isinstance(input_, bytes):
+        return sigstore_hashes.Hashed(
+            digest=hashlib.sha256(input_).digest(), algorithm=HashAlgorithm.SHA2_256
+        )
+
+    return sigstore_hashes.Hashed(
+        digest=_sha256_streaming(input_), algorithm=HashAlgorithm.SHA2_256
+    )
+
+
+def _sha256_streaming(io: IO[bytes]) -> bytes:
     """
     Compute the SHA256 of a stream.
 
     This function does its own internal buffering, so an unbuffered stream
     should be supplied for optimal performance.
     """
 
@@ -195,15 +241,15 @@
     leaf upholds Sigstore's invariants.
     """
 
     # Only v3 certificates should appear in the context of Sigstore;
     # earlier versions of X.509 lack extensions and have ambiguous CA
     # behavior.
     if cert.version != Version.v3:
-        raise InvalidCertError(f"invalid X.509 version: {cert.version}")
+        raise VerificationError(f"invalid X.509 version: {cert.version}")
 
     # Valid CA certificates must have the following set:
     #
     #  * `BasicKeyUsage.keyCertSign`
     #  * `BasicConstraints.ca`
     #
     # Any other combination of states is inconsistent and invalid, meaning
@@ -212,40 +258,40 @@
     try:
         basic_constraints = cert.extensions.get_extension_for_oid(
             ExtensionOID.BASIC_CONSTRAINTS
         )
 
         # BasicConstraints must be marked as critical, per RFC 5280 4.2.1.9.
         if not basic_constraints.critical:
-            raise InvalidCertError(
+            raise VerificationError(
                 "invalid X.509 certificate: non-critical BasicConstraints in CA"
             )
 
         ca = basic_constraints.value.ca  # type: ignore
     except ExtensionNotFound:
         # No BasicConstrains means that this can't possibly be a CA.
         return False
 
     key_cert_sign = False
     try:
         key_usage = cert.extensions.get_extension_for_oid(ExtensionOID.KEY_USAGE)
         key_cert_sign = key_usage.value.key_cert_sign  # type: ignore
     except ExtensionNotFound:
-        raise InvalidCertError("invalid X.509 certificate: missing KeyUsage")
+        raise VerificationError("invalid X.509 certificate: missing KeyUsage")
 
     # If both states are set, this is a CA.
     if ca and key_cert_sign:
         return True
 
     if not (ca or key_cert_sign):
         return False
 
     # Anything else is an invalid state that should never occur.
-    raise InvalidCertError(
-        f"invalid certificate states: KeyUsage.keyCertSign={key_cert_sign}"
+    raise VerificationError(
+        f"invalid X.509 certificate states: KeyUsage.keyCertSign={key_cert_sign}"
         f", BasicConstraints.ca={ca}"
     )
 
 
 def cert_is_root_ca(cert: Certificate) -> bool:
     """
     Returns `True` if and only if the given `Certificate` indicates
@@ -258,15 +304,15 @@
     # NOTE(ww): This function is obnoxiously long to make the different
     # states explicit.
 
     # Only v3 certificates should appear in the context of Sigstore;
     # earlier versions of X.509 lack extensions and have ambiguous CA
     # behavior.
     if cert.version != Version.v3:
-        raise InvalidCertError(f"invalid X.509 version: {cert.version}")
+        raise VerificationError(f"invalid X.509 version: {cert.version}")
 
     # Non-CAs can't possibly be root CAs.
     if not cert_is_ca(cert):
         return False
 
     # A certificate that is its own issuer and signer is considered a root CA.
     try:
@@ -289,32 +335,32 @@
     the trustworthiness of the given certificate.
     """
 
     # Only v3 certificates should appear in the context of Sigstore;
     # earlier versions of X.509 lack extensions and have ambiguous CA
     # behavior.
     if cert.version != Version.v3:
-        raise InvalidCertError(f"invalid X.509 version: {cert.version}")
+        raise VerificationError(f"invalid X.509 version: {cert.version}")
 
     # CAs are not leaves.
     if cert_is_ca(cert):
         return False
 
     key_usage = cert.extensions.get_extension_for_oid(ExtensionOID.KEY_USAGE)
     digital_signature = key_usage.value.digital_signature  # type: ignore
 
     if not digital_signature:
-        raise InvalidCertError(
+        raise VerificationError(
             "invalid certificate for Sigstore purposes: missing digital signature usage"
         )
 
     # Finally, we check to make sure the leaf has an `ExtendedKeyUsages`
     # extension that includes a codesigning entitlement. Sigstore should
     # never issue a leaf that doesn't have this extended usage.
     try:
         extended_key_usage = cert.extensions.get_extension_for_oid(
             ExtensionOID.EXTENDED_KEY_USAGE
         )
 
         return ExtendedKeyUsageOID.CODE_SIGNING in extended_key_usage.value  # type: ignore
     except ExtensionNotFound:
-        raise InvalidCertError("invalid X.509 certificate: missing ExtendedKeyUsage")
+        raise VerificationError("invalid X.509 certificate: missing ExtendedKeyUsage")
```

### Comparing `sigstore-2.1.5/sigstore/errors.py` & `sigstore-3.0.0rc1/sigstore/errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,35 +13,36 @@
 # limitations under the License.
 
 """
 Exceptions.
 """
 
 import sys
+from logging import Logger
 from typing import Any, Mapping
 
 
 class Error(Exception):
     """Base sigstore exception type. Defines helpers for diagnostics."""
 
     def diagnostics(self) -> str:
         """Returns human-friendly error information."""
 
-        return """An issue occurred."""
+        return str(self)
 
-    def print_and_exit(self, raise_error: bool = False) -> None:
+    def log_and_exit(self, logger: Logger, raise_error: bool = False) -> None:
         """Prints all relevant error information to stderr and exits."""
 
         remind_verbose = (
             "Raising original exception:"
             if raise_error
             else "For detailed error information, run sigstore with the `--verbose` flag."
         )
 
-        print(f"{self.diagnostics()}\n{remind_verbose}", file=sys.stderr)
+        logger.error(f"{self.diagnostics()}\n{remind_verbose}")
 
         if raise_error:
             # don't want "during handling another exception"
             self.__suppress_context__ = True
             raise self
 
         sys.exit(1)
@@ -113,7 +114,13 @@
 
     def diagnostics(self) -> str:
         """Returns diagnostics for the error."""
         return """\
         Unable to establish root of trust.
 
         This error may occur when the resources embedded in this distribution of sigstore-python are out of date."""
+
+
+class VerificationError(Error):
+    """
+    Raised whenever any phase or subcomponent of Sigstore verification fails.
+    """
```

### Comparing `sigstore-2.1.5/sigstore/oidc.py` & `sigstore-3.0.0rc1/sigstore/oidc.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.5/sigstore/sign.py` & `sigstore-3.0.0rc1/sigstore/verify/verifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,389 +9,332 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-API for signing artifacts.
-
-Example:
-
-```python
-from pathlib import Path
-
-from sigstore.sign import SigningContext
-from sigstore.oidc import Issuer
-
-issuer = Issuer.production()
-identity = issuer.identity_token()
-
-# The artifact to sign
-artifact = Path("foo.txt")
-
-with artifact.open("rb") as file:
-    signing_ctx = SigningContext.production()
-    with signing_ctx.signer(identity, cache=True) as signer:
-        result = signer.sign(file)
-        print(result)
-```
+Verification API machinery.
 """
 
 from __future__ import annotations
 
 import base64
 import logging
-from contextlib import contextmanager
 from datetime import datetime, timezone
-from typing import IO, Iterator, Optional
+from typing import List, cast
 
-import cryptography.x509 as x509
-import sigstore_rekor_types
-from cryptography.hazmat.primitives import hashes, serialization
+import rekor_types
+from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives.asymmetric import ec
-from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
-from cryptography.x509.oid import NameOID
-from pydantic import BaseModel
-from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import (
-    Bundle,
-    VerificationMaterial,
-)
-from sigstore_protobuf_specs.dev.sigstore.common.v1 import (
-    HashAlgorithm,
-    HashOutput,
-    LogId,
-    MessageSignature,
-    X509Certificate,
-    X509CertificateChain,
-)
-from sigstore_protobuf_specs.dev.sigstore.rekor.v1 import (
-    Checkpoint,
-    InclusionPromise,
-    InclusionProof,
-    KindVersion,
-    TransparencyLogEntry,
+from cryptography.x509 import ExtendedKeyUsage, KeyUsage
+from cryptography.x509.oid import ExtendedKeyUsageOID
+from OpenSSL.crypto import (
+    X509,
+    X509Store,
+    X509StoreContext,
+    X509StoreContextError,
+    X509StoreFlags,
 )
+from pydantic import ValidationError
 
-from sigstore._internal.fulcio import (
-    ExpiredCertificate,
-    FulcioCertificateSigningResponse,
-    FulcioClient,
-)
+from sigstore import dsse
+from sigstore._internal.rekor import _hashedrekord_from_parts
 from sigstore._internal.rekor.client import RekorClient
-from sigstore._internal.sct import verify_sct
-from sigstore._internal.tuf import TrustUpdater
-from sigstore._utils import B64Str, HexStr, PEMCert, sha256_streaming
-from sigstore.oidc import ExpiredIdentity, IdentityToken
-from sigstore.transparency import LogEntry
-
-logger = logging.getLogger(__name__)
-
-
-class Signer:
-    """
-    The primary API for signing operations.
-    """
-
-    def __init__(
-        self,
-        identity_token: IdentityToken,
-        signing_ctx: SigningContext,
-        cache: bool = True,
-    ) -> None:
-        """
-        Create a new `Signer`.
-
-        `identity_token` is the identity token used to request a signing certificate
-        from Fulcio.
-
-        `signing_ctx` is a `SigningContext` that keeps information about the signing
-        configuration.
-
-        `cache` determines whether the signing certificate and ephemeral private key
-        should be reused (until the certificate expires) to sign different artifacts.
-        Default is `True`.
-        """
-        self._identity_token = identity_token
-        self._signing_ctx: SigningContext = signing_ctx
-        self.__cached_private_key: Optional[ec.EllipticCurvePrivateKey] = None
-        self.__cached_signing_certificate: Optional[
-            FulcioCertificateSigningResponse
-        ] = None
-        if cache:
-            logger.debug("Generating ephemeral keys...")
-            self.__cached_private_key = ec.generate_private_key(ec.SECP256R1())
-            logger.debug("Requesting ephemeral certificate...")
-            self.__cached_signing_certificate = self._signing_cert(self._private_key)
-
-    @property
-    def _private_key(self) -> ec.EllipticCurvePrivateKey:
-        """Get or generate a signing key."""
-        if self.__cached_private_key is None:
-            logger.debug("no cached key; generating ephemeral key")
-            return ec.generate_private_key(ec.SECP256R1())
-        return self.__cached_private_key
-
-    def _signing_cert(
-        self,
-        private_key: ec.EllipticCurvePrivateKey,
-    ) -> FulcioCertificateSigningResponse:
-        """Get or request a signing certificate from Fulcio."""
-        # If it exists, verify if the current certificate is expired
-        if self.__cached_signing_certificate:
-            not_valid_after = self.__cached_signing_certificate.cert.not_valid_after
-            not_valid_after_tzutc = not_valid_after.replace(tzinfo=timezone.utc)
-            if datetime.now(timezone.utc) > not_valid_after_tzutc:
-                raise ExpiredCertificate
-            return self.__cached_signing_certificate
-
-        else:
-            logger.debug("Retrieving signed certificate...")
-
-            # Build an X.509 Certificiate Signing Request
-            builder = (
-                x509.CertificateSigningRequestBuilder()
-                .subject_name(
-                    x509.Name(
-                        [
-                            x509.NameAttribute(
-                                NameOID.EMAIL_ADDRESS, self._identity_token._identity
-                            ),
-                        ]
-                    )
-                )
-                .add_extension(
-                    x509.BasicConstraints(ca=False, path_length=None),
-                    critical=True,
-                )
-            )
-            certificate_request = builder.sign(private_key, hashes.SHA256())
-
-            certificate_response = self._signing_ctx._fulcio.signing_cert.post(
-                certificate_request, self._identity_token
-            )
-
-            return certificate_response
-
-    def sign(
-        self,
-        input_: IO[bytes],
-    ) -> SigningResult:
-        """Public API for signing blobs"""
-        input_digest = sha256_streaming(input_)
-        private_key = self._private_key
-
-        if not self._identity_token.in_validity_period():
-            raise ExpiredIdentity
-
-        try:
-            certificate_response = self._signing_cert(private_key)
-        except ExpiredCertificate as e:
-            raise e
-
-        # TODO(alex): Retrieve the public key via TUF
-        #
-        # Verify the SCT
-        sct = certificate_response.sct  # noqa
-        cert = certificate_response.cert  # noqa
-        chain = certificate_response.chain
-
-        verify_sct(sct, cert, chain, self._signing_ctx._rekor._ct_keyring)
-
-        logger.debug("Successfully verified SCT...")
-
-        # Sign artifact
-        artifact_signature = private_key.sign(
-            input_digest, ec.ECDSA(Prehashed(hashes.SHA256()))
-        )
-        b64_artifact_signature = B64Str(base64.b64encode(artifact_signature).decode())
-
-        # Prepare inputs
-        b64_cert = base64.b64encode(
-            cert.public_bytes(encoding=serialization.Encoding.PEM)
-        )
-
-        # Create the transparency log entry
-        proposed_entry = sigstore_rekor_types.Hashedrekord(
-            kind="hashedrekord",
-            api_version="0.0.1",
-            spec=sigstore_rekor_types.HashedrekordV001Schema(
-                signature=sigstore_rekor_types.Signature1(
-                    content=b64_artifact_signature,
-                    public_key=sigstore_rekor_types.PublicKey1(
-                        content=b64_cert.decode()
-                    ),
-                ),
-                data=sigstore_rekor_types.Data(
-                    hash=sigstore_rekor_types.Hash(
-                        algorithm=sigstore_rekor_types.Algorithm.SHA256,
-                        value=input_digest.hex(),
-                    )
-                ),
-            ),
-        )
-        entry = self._signing_ctx._rekor.log.entries.post(proposed_entry)
-
-        logger.debug(f"Transparency log entry created with index: {entry.log_index}")
+from sigstore._internal.sct import (
+    _get_precertificate_signed_certificate_timestamps,
+    verify_sct,
+)
+from sigstore._internal.trustroot import KeyringPurpose, TrustedRoot
+from sigstore._utils import base64_encode_pem_cert, sha256_digest
+from sigstore.errors import VerificationError
+from sigstore.hashes import Hashed
+from sigstore.models import Bundle
+from sigstore.verify.policy import VerificationPolicy
 
-        return SigningResult(
-            input_digest=HexStr(input_digest.hex()),
-            cert_pem=PEMCert(
-                cert.public_bytes(encoding=serialization.Encoding.PEM).decode()
-            ),
-            b64_signature=B64Str(b64_artifact_signature),
-            log_entry=entry,
-        )
+_logger = logging.getLogger(__name__)
 
 
-class SigningContext:
+class Verifier:
     """
-    Keep a context between signing operations.
+    The primary API for verification operations.
     """
 
-    def __init__(
-        self,
-        *,
-        fulcio: FulcioClient,
-        rekor: RekorClient,
-    ):
+    def __init__(self, *, rekor: RekorClient, trusted_root: TrustedRoot):
         """
-        Create a new `SigningContext`.
-
-        `fulcio` is a `FulcioClient` capable of connecting to a Fulcio instance
-        and returning signing certificates.
+        Create a new `Verifier`.
 
         `rekor` is a `RekorClient` capable of connecting to a Rekor instance
-        and creating transparency log entries.
+        containing logs for the file(s) being verified.
+
+        `fulcio_certificate_chain` is a list of PEM-encoded X.509 certificates,
+        establishing the trust chain for the signing certificate and signature.
         """
-        self._fulcio = fulcio
         self._rekor = rekor
+        self._fulcio_certificate_chain: List[X509] = [
+            X509.from_cryptography(parent_cert)
+            for parent_cert in trusted_root.get_fulcio_certs()
+        ]
+        self._trusted_root = trusted_root
 
     @classmethod
-    def production(cls) -> SigningContext:
+    def production(cls) -> Verifier:
         """
-        Return a `SigningContext` instance configured against Sigstore's production-level services.
+        Return a `Verifier` instance configured against Sigstore's production-level services.
         """
-        updater = TrustUpdater.production()
-        rekor = RekorClient.production(updater)
+        trusted_root = TrustedRoot.production(purpose=KeyringPurpose.VERIFY)
         return cls(
-            fulcio=FulcioClient.production(),
-            rekor=rekor,
+            rekor=RekorClient.production(),
+            trusted_root=trusted_root,
         )
 
     @classmethod
-    def staging(cls) -> SigningContext:
+    def staging(cls) -> Verifier:
         """
-        Return a `SignerContext` instance configured against Sigstore's staging-level services.
+        Return a `Verifier` instance configured against Sigstore's staging-level services.
         """
-        updater = TrustUpdater.staging()
-        rekor = RekorClient.staging(updater)
+        trusted_root = TrustedRoot.staging(purpose=KeyringPurpose.VERIFY)
         return cls(
-            fulcio=FulcioClient.staging(),
-            rekor=rekor,
+            rekor=RekorClient.staging(),
+            trusted_root=trusted_root,
         )
 
-    @contextmanager
-    def signer(
-        self, identity_token: IdentityToken, *, cache: bool = True
-    ) -> Iterator[Signer]:
+    def _verify_common_signing_cert(
+        self, bundle: Bundle, policy: VerificationPolicy
+    ) -> None:
         """
-        A context manager for signing operations.
-
-        `identity_token` is the identity token passed to the `Signer` instance
-        and used to request a signing certificate from Fulcio.
+        Performs the signing certificate verification steps that are shared between
+        `verify_dsse` and `verify_artifact`.
 
-        `cache` determines whether the signing certificate and ephemeral private key
-        generated by the `Signer` instance should be reused (until the certificate expires)
-        to sign different artifacts.
-        Default is `True`.
+        Raises `VerificationError` on all failures.
         """
-        yield Signer(identity_token, self, cache)
 
+        # In order to verify an artifact, we need to achieve the following:
+        #
+        # 1. Verify that the signing certificate chains to the root of trust
+        #    and is valid at the time of signing.
+        # 2. Verify the signing certificate's SCT.
+        # 3. Verify that the signing certificate conforms to the Sigstore
+        #    X.509 profile as well as the passed-in `VerificationPolicy`.
+        # 4. Verify the inclusion proof and signed checkpoint for the log
+        #    entry.
+        # 5. Verify the inclusion promise for the log entry, if present.
+        # 6. Verify the timely insertion of the log entry against the validity
+        #    period for the signing certificate.
+        # 7. Verify the signature and input against the signing certificate's
+        #    public key.
+        # 8. Verify the transparency log entry's consistency against the other
+        #    materials, to prevent variants of CVE-2022-36056.
+        #
+        # This method performs steps (1) through (6) above. Its caller
+        # MUST perform steps (7) and (8) separately, since they vary based on
+        # the kind of verification being performed (i.e. hashedrekord, DSSE, etc.)
+
+        cert = bundle.signing_certificate
+
+        # NOTE: The `X509Store` object currently cannot have its time reset once the `set_time`
+        # method been called on it. To get around this, we construct a new one for every `verify`
+        # call.
+        store = X509Store()
+        # NOTE: By explicitly setting the flags here, we ensure that OpenSSL's
+        # PARTIAL_CHAIN default does not change on us. Enabling PARTIAL_CHAIN
+        # would be strictly more conformant of OpenSSL, but we currently
+        # *want* the "long" chain behavior of performing path validation
+        # down to a self-signed root.
+        store.set_flags(X509StoreFlags.X509_STRICT)
+        for parent_cert_ossl in self._fulcio_certificate_chain:
+            store.add_cert(parent_cert_ossl)
+
+        # (1): verify that the signing certificate is signed by the root
+        #      certificate and that the signing certificate was valid at the
+        #      time of signing.
+        sign_date = cert.not_valid_before_utc
+        cert_ossl = X509.from_cryptography(cert)
 
-class SigningResult(BaseModel):
-    """
-    Represents the artifacts of a signing operation.
-    """
+        store.set_time(sign_date)
+        store_ctx = X509StoreContext(store, cert_ossl)
+        try:
+            # get_verified_chain returns the full chain including the end-entity certificate
+            # and chain should contain only CA certificates
+            chain = store_ctx.get_verified_chain()[1:]
+        except X509StoreContextError as e:
+            raise VerificationError(f"failed to build chain: {e}")
 
-    input_digest: HexStr
-    """
-    The hex-encoded SHA256 digest of the input that was signed for.
-    """
+        # (2): verify the signing certificate's SCT.
+        sct = _get_precertificate_signed_certificate_timestamps(cert)[0]
+        try:
+            verify_sct(
+                sct,
+                cert,
+                [parent_cert.to_cryptography() for parent_cert in chain],
+                self._trusted_root.ct_keyring(),
+            )
+        except VerificationError as e:
+            raise VerificationError(f"failed to verify SCT on signing certificate: {e}")
 
-    cert_pem: PEMCert
-    """
-    The PEM-encoded public half of the certificate used for signing.
-    """
+        # (3): verify the signing certificate against the Sigstore
+        #      X.509 profile and verify against the given `VerificationPolicy`.
+        usage_ext = cert.extensions.get_extension_for_class(KeyUsage)
+        if not usage_ext.value.digital_signature:
+            raise VerificationError("Key usage is not of type `digital signature`")
+
+        extended_usage_ext = cert.extensions.get_extension_for_class(ExtendedKeyUsage)
+        if ExtendedKeyUsageOID.CODE_SIGNING not in extended_usage_ext.value:
+            raise VerificationError("Extended usage does not contain `code signing`")
+
+        policy.verify(cert)
+
+        _logger.debug("Successfully verified signing certificate validity...")
+
+        # (4): verify the inclusion proof and signed checkpoint for the
+        #      log entry.
+        # (5): verify the inclusion promise for the log entry, if present.
+        entry = bundle.log_entry
+        try:
+            entry._verify(self._trusted_root.rekor_keyring())
+        except VerificationError as exc:
+            raise VerificationError(f"invalid log entry: {exc}")
+
+        # (6): verify that log entry was integrated circa the signing certificate's
+        #      validity period.
+        integrated_time = datetime.fromtimestamp(entry.integrated_time, tz=timezone.utc)
+        if not (
+            bundle.signing_certificate.not_valid_before_utc
+            <= integrated_time
+            <= bundle.signing_certificate.not_valid_after_utc
+        ):
+            raise VerificationError(
+                "invalid signing cert: expired at time of Rekor entry"
+            )
 
-    b64_signature: B64Str
-    """
-    The base64-encoded signature.
-    """
+    def verify_dsse(
+        self, bundle: Bundle, policy: VerificationPolicy
+    ) -> tuple[str, bytes]:
+        """
+        Verifies an bundle's DSSE envelope, returning the encapsulated payload
+        and its content type.
+
+        This method is only for DSSE-enveloped payloads. To verify
+        an arbitrary input against a bundle, use the `verify_artifact`
+        method.
+
+        `bundle` is the Sigstore `Bundle` to both verify and verify against.
+
+        `policy` is the `VerificationPolicy` to verify against.
+
+        Returns a tuple of `(type, payload)`, where `type` is the payload's
+        type as encoded in the DSSE envelope and `payload` is the raw `bytes`
+        of the payload. No validation of either `type` or `payload` is
+        performed; users of this API **must** assert that `type` is known
+        to them before proceeding to handle `payload` in an application-dependent
+        manner.
+        """
+
+        # (1) through (6) are performed by `_verify_common_signing_cert`.
+        self._verify_common_signing_cert(bundle, policy)
+
+        # (7): verify the bundle's signature and DSSE envelope against the
+        #      signing certificate's public key.
+        envelope = bundle._dsse_envelope
+        if envelope is None:
+            raise VerificationError(
+                "cannot perform DSSE verification on a bundle without a DSSE envelope"
+            )
 
-    log_entry: LogEntry
-    """
-    A record of the Rekor log entry for the signing operation.
-    """
+        signing_key = bundle.signing_certificate.public_key()
+        signing_key = cast(ec.EllipticCurvePublicKey, signing_key)
+        dsse._verify(signing_key, envelope)
+
+        # (8): verify the consistency of the log entry's body against
+        #      the other bundle materials.
+        # NOTE: This is very slightly weaker than the consistency check
+        # for hashedrekord entries, due to how inclusion is recorded for DSSE:
+        # the included entry for DSSE includes an envelope hash that we
+        # *cannot* verify, since the envelope is uncanonicalized JSON.
+        # Instead, we manually pick apart the entry body below and verify
+        # the parts we can (namely the payload hash and signature list).
+        entry = bundle.log_entry
+        try:
+            entry_body = rekor_types.Dsse.model_validate_json(
+                base64.b64decode(entry.body)
+            )
+        except ValidationError as exc:
+            raise VerificationError(f"invalid DSSE log entry: {exc}")
+
+        payload_hash = sha256_digest(envelope._inner.payload).digest.hex()
+        if (
+            entry_body.spec.root.payload_hash.algorithm  # type: ignore[union-attr]
+            != rekor_types.dsse.Algorithm.SHA256
+        ):
+            raise VerificationError("expected SHA256 payload hash in DSSE log entry")
+        if payload_hash != entry_body.spec.root.payload_hash.value:  # type: ignore[union-attr]
+            raise VerificationError("log entry payload hash does not match bundle")
+
+        # NOTE: Like `dsse._verify`: multiple signatures would be frivolous here,
+        # but we handle them just in case the signer has somehow produced multiple
+        # signatures for their envelope with the same signing key.
+        signatures = [
+            rekor_types.dsse.Signature(
+                signature=base64.b64encode(signature.sig).decode(),
+                verifier=base64_encode_pem_cert(bundle.signing_certificate),
+            )
+            for signature in envelope._inner.signatures
+        ]
+        if signatures != entry_body.spec.root.signatures:
+            raise VerificationError("log entry signatures do not match bundle")
 
-    def to_bundle(self) -> Bundle:
+        return (envelope._inner.payload_type, envelope._inner.payload)
+
+    def verify_artifact(
+        self,
+        input_: bytes | Hashed,
+        bundle: Bundle,
+        policy: VerificationPolicy,
+    ) -> None:
         """
-        Creates a Sigstore bundle (as defined by Sigstore's protobuf specs)
-        from this `SigningResult`.
+        Public API for verifying.
+
+        `input_` is the input to verify, either as a buffer of contents or as
+        a prehashed `Hashed` object.
+
+        `bundle` is the Sigstore `Bundle` to verify against.
+
+        `policy` is the `VerificationPolicy` to verify against.
+
+        On failure, this method raises `VerificationError`.
         """
 
-        # NOTE: We explicitly only include the leaf certificate in the bundle's "chain"
-        # here: the specs explicitly forbid the inclusion of the root certificate,
-        # and discourage inclusion of any intermediates (since they're in the root of
-        # trust already).
-        cert = x509.load_pem_x509_certificate(self.cert_pem.encode())
-        cert_der = cert.public_bytes(encoding=serialization.Encoding.DER)
-        chain = X509CertificateChain(certificates=[X509Certificate(raw_bytes=cert_der)])
-
-        inclusion_proof: InclusionProof | None = None
-        if self.log_entry.inclusion_proof is not None:
-            inclusion_proof = InclusionProof(
-                log_index=self.log_entry.inclusion_proof.log_index,
-                root_hash=bytes.fromhex(self.log_entry.inclusion_proof.root_hash),
-                tree_size=self.log_entry.inclusion_proof.tree_size,
-                hashes=[
-                    bytes.fromhex(h) for h in self.log_entry.inclusion_proof.hashes
-                ],
-                checkpoint=Checkpoint(
-                    envelope=self.log_entry.inclusion_proof.checkpoint
-                ),
-            )
+        # (1) through (6) are performed by `_verify_common_signing_cert`.
+        self._verify_common_signing_cert(bundle, policy)
 
-        tlog_entry = TransparencyLogEntry(
-            log_index=self.log_entry.log_index,
-            log_id=LogId(key_id=bytes.fromhex(self.log_entry.log_id)),
-            kind_version=KindVersion(kind="hashedrekord", version="0.0.1"),
-            integrated_time=self.log_entry.integrated_time,
-            inclusion_promise=InclusionPromise(
-                signed_entry_timestamp=base64.b64decode(
-                    self.log_entry.inclusion_promise
-                )
+        hashed_input = sha256_digest(input_)
+
+        # (7): verify that the signature was signed by the public key in the signing certificate.
+        try:
+            signing_key = bundle.signing_certificate.public_key()
+            signing_key = cast(ec.EllipticCurvePublicKey, signing_key)
+            signing_key.verify(
+                bundle._inner.message_signature.signature,
+                hashed_input.digest,
+                ec.ECDSA(hashed_input._as_prehashed()),
             )
-            if self.log_entry.inclusion_promise
-            else None,
-            inclusion_proof=inclusion_proof,
-            canonicalized_body=base64.b64decode(self.log_entry.body),
-        )
+        except InvalidSignature:
+            raise VerificationError("Signature is invalid for input")
 
-        material = VerificationMaterial(
-            x509_certificate_chain=chain,
-            tlog_entries=[tlog_entry],
-        )
+        _logger.debug("Successfully verified signature...")
 
-        bundle = Bundle(
-            media_type="application/vnd.dev.sigstore.bundle+json;version=0.2",
-            verification_material=material,
-            message_signature=MessageSignature(
-                message_digest=HashOutput(
-                    algorithm=HashAlgorithm.SHA2_256,
-                    digest=bytes.fromhex(self.input_digest),
-                ),
-                signature=base64.b64decode(self.b64_signature),
-            ),
+        # (8): verify the consistency of the log entry's body against
+        #      the other bundle materials (and input being verified).
+        entry = bundle.log_entry
+
+        expected_body = _hashedrekord_from_parts(
+            bundle.signing_certificate,
+            bundle._inner.message_signature.signature,
+            hashed_input,
         )
-
-        return bundle
+        actual_body = rekor_types.Hashedrekord.model_validate_json(
+            base64.b64decode(entry.body)
+        )
+        if expected_body != actual_body:
+            raise VerificationError(
+                "transparency log entry is inconsistent with other materials"
+            )
```

### Comparing `sigstore-2.1.5/sigstore/verify/models.py` & `sigstore-3.0.0rc1/sigstore/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,513 +9,531 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Common (base) models for the verification APIs.
+Common models shared between signing and verification.
 """
 
 from __future__ import annotations
 
 import base64
-import json
 import logging
-from dataclasses import dataclass
+import typing
 from textwrap import dedent
-from typing import IO
+from typing import Any, List, Optional
 
-import sigstore_rekor_types
+import rfc8785
 from cryptography.hazmat.primitives.serialization import Encoding
 from cryptography.x509 import (
     Certificate,
     load_der_x509_certificate,
-    load_pem_x509_certificate,
 )
-from pydantic import BaseModel
-from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import (
-    Bundle,
-    VerificationMaterial,
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    StrictInt,
+    StrictStr,
+    TypeAdapter,
+    ValidationInfo,
+    field_validator,
 )
-from sigstore_protobuf_specs.dev.sigstore.common.v1 import (
-    HashAlgorithm,
-    HashOutput,
-    LogId,
-    MessageSignature,
-    PublicKeyIdentifier,
-    X509Certificate,
-    X509CertificateChain,
+from pydantic.dataclasses import dataclass
+from rekor_types import Dsse, Hashedrekord, ProposedEntry
+from sigstore_protobuf_specs.dev.sigstore.bundle import v1 as bundle_v1
+from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import (
+    Bundle as _Bundle,
 )
+from sigstore_protobuf_specs.dev.sigstore.common import v1 as common_v1
+from sigstore_protobuf_specs.dev.sigstore.rekor import v1 as rekor_v1
 from sigstore_protobuf_specs.dev.sigstore.rekor.v1 import (
-    Checkpoint,
-    InclusionPromise,
     InclusionProof,
-    KindVersion,
-    TransparencyLogEntry,
 )
 
-from sigstore._internal.rekor import RekorClient
+from sigstore import dsse
+from sigstore._internal.merkle import verify_merkle_inclusion
+from sigstore._internal.rekor.checkpoint import verify_checkpoint
 from sigstore._utils import (
     B64Str,
-    PEMCert,
-    base64_encode_pem_cert,
+    BundleType,
+    KeyID,
     cert_is_leaf,
     cert_is_root_ca,
-    sha256_streaming,
 )
-from sigstore.errors import Error
-from sigstore.transparency import LogEntry, LogInclusionProof
+from sigstore.errors import Error, VerificationError
 
-logger = logging.getLogger(__name__)
+if typing.TYPE_CHECKING:
+    from sigstore._internal.trustroot import RekorKeyring
 
-_BUNDLE_0_1 = "application/vnd.dev.sigstore.bundle+json;version=0.1"
-_BUNDLE_0_2 = "application/vnd.dev.sigstore.bundle+json;version=0.2"
-_KNOWN_BUNDLE_TYPES = {
-    _BUNDLE_0_1,
-    _BUNDLE_0_2,
-}
 
+_logger = logging.getLogger(__name__)
 
-class VerificationResult(BaseModel):
-    """
-    Represents the result of a verification operation.
-
-    Results are boolish, and failures contain a reason (and potentially
-    some additional context).
-    """
 
-    success: bool
+class LogInclusionProof(BaseModel):
     """
-    Represents the status of this result.
+    Represents an inclusion proof for a transparency log entry.
     """
 
-    def __bool__(self) -> bool:
-        """
-        Returns a boolean representation of this result.
+    model_config = ConfigDict(populate_by_name=True)
 
-        `VerificationSuccess` is always `True`, and `VerificationFailure`
-        is always `False`.
-        """
-        return self.success
+    checkpoint: StrictStr = Field(..., alias="checkpoint")
+    hashes: List[StrictStr] = Field(..., alias="hashes")
+    log_index: StrictInt = Field(..., alias="logIndex")
+    root_hash: StrictStr = Field(..., alias="rootHash")
+    tree_size: StrictInt = Field(..., alias="treeSize")
 
+    @field_validator("log_index")
+    def _log_index_positive(cls, v: int) -> int:
+        if v < 0:
+            raise ValueError(f"Inclusion proof has invalid log index: {v} < 0")
+        return v
 
-class VerificationSuccess(VerificationResult):
-    """
-    The verification completed successfully,
+    @field_validator("tree_size")
+    def _tree_size_positive(cls, v: int) -> int:
+        if v < 0:
+            raise ValueError(f"Inclusion proof has invalid tree size: {v} < 0")
+        return v
+
+    @field_validator("tree_size")
+    def _log_index_within_tree_size(
+        cls, v: int, info: ValidationInfo, **kwargs: Any
+    ) -> int:
+        if "log_index" in info.data and v <= info.data["log_index"]:
+            raise ValueError(
+                "Inclusion proof has log index greater than or equal to tree size: "
+                f"{v} <= {info.data['log_index']}"
+            )
+        return v
+
+
+@dataclass(frozen=True)
+class LogEntry:
     """
+    Represents a transparency log entry.
 
-    success: bool = True
+    Log entries are retrieved from the transparency log after signing or verification events,
+    or loaded from "Sigstore" bundles provided by the user.
+
+    This representation allows for either a missing inclusion promise or a missing
+    inclusion proof, but not both: attempting to construct a `LogEntry` without
+    at least one will fail.
     """
-    See `VerificationResult.success`.
+
+    uuid: Optional[str]
     """
+    This entry's unique ID in the log instance it was retrieved from.
 
+    For sharded log deployments, IDs are unique per-shard.
 
-class VerificationFailure(VerificationResult):
+    Not present for `LogEntry` instances loaded from Sigstore bundles.
     """
-    The verification failed, due to `reason`.
+
+    body: B64Str
+    """
+    The base64-encoded body of the transparency log entry.
     """
 
-    success: bool = False
+    integrated_time: int
     """
-    See `VerificationResult.success`.
+    The UNIX time at which this entry was integrated into the transparency log.
     """
 
-    reason: str
+    log_id: str
     """
-    A human-readable explanation or description of the verification failure.
+    The log's ID (as the SHA256 hash of the DER-encoded public key for the log
+    at the time of entry inclusion).
     """
 
+    log_index: int
+    """
+    The index of this entry within the log.
+    """
 
-class InvalidMaterials(Error):
+    inclusion_proof: LogInclusionProof
     """
-    Raised when the associated `VerificationMaterials` are invalid in some way.
+    An inclusion proof for this log entry.
     """
 
-    def diagnostics(self) -> str:
-        """Returns diagnostics for the error."""
+    inclusion_promise: Optional[B64Str]
+    """
+    An inclusion promise for this log entry, if present.
 
-        return dedent(
-            f"""\
-        An issue occurred while parsing the verification materials.
+    Internally, this is a base64-encoded Signed Entry Timestamp (SET) for this
+    log entry.
+    """
 
-        The provided verification materials are malformed and may have been
-        modified maliciously.
+    @classmethod
+    def _from_response(cls, dict_: dict[str, Any]) -> LogEntry:
+        """
+        Create a new `LogEntry` from the given API response.
+        """
 
-        Additional context:
+        # Assumes we only get one entry back
+        entries = list(dict_.items())
+        if len(entries) != 1:
+            raise ValueError("Received multiple entries in response")
+
+        uuid, entry = entries[0]
+        return LogEntry(
+            uuid=uuid,
+            body=entry["body"],
+            integrated_time=entry["integratedTime"],
+            log_id=entry["logID"],
+            log_index=entry["logIndex"],
+            inclusion_proof=LogInclusionProof.model_validate(
+                entry["verification"]["inclusionProof"]
+            ),
+            inclusion_promise=entry["verification"]["signedEntryTimestamp"],
+        )
 
-        {self}
+    @classmethod
+    def _from_dict_rekor(cls, dict_: dict[str, Any]) -> LogEntry:
         """
+        Create a new `LogEntry` from the given Rekor TransparencyLogEntry.
+        """
+        tlog_entry = rekor_v1.TransparencyLogEntry()
+        tlog_entry.from_dict(dict_)
+
+        inclusion_proof: InclusionProof | None = tlog_entry.inclusion_proof
+        # This check is required by us as the client, not the
+        # protobuf-specs themselves.
+        if inclusion_proof is None or inclusion_proof.checkpoint.envelope is None:
+            raise InvalidBundle("entry must contain inclusion proof")
+
+        parsed_inclusion_proof = LogInclusionProof(
+            checkpoint=inclusion_proof.checkpoint.envelope,
+            hashes=[h.hex() for h in inclusion_proof.hashes],
+            log_index=inclusion_proof.log_index,
+            root_hash=inclusion_proof.root_hash.hex(),
+            tree_size=inclusion_proof.tree_size,
         )
 
+        return LogEntry(
+            uuid=None,
+            body=B64Str(base64.b64encode(tlog_entry.canonicalized_body).decode()),
+            integrated_time=tlog_entry.integrated_time,
+            log_id=tlog_entry.log_id.key_id.hex(),
+            log_index=tlog_entry.log_index,
+            inclusion_proof=parsed_inclusion_proof,
+            inclusion_promise=B64Str(
+                base64.b64encode(
+                    tlog_entry.inclusion_promise.signed_entry_timestamp
+                ).decode()
+            ),
+        )
 
-class RekorEntryMissing(Exception):
-    """
-    Raised if `VerificationMaterials.rekor_entry()` fails to find an entry
-    in the Rekor log.
+    def _to_dict_rekor(self) -> dict[str, Any]:
+        inclusion_promise: rekor_v1.InclusionPromise | None = None
+        if self.inclusion_promise:
+            inclusion_promise = rekor_v1.InclusionPromise(
+                signed_entry_timestamp=base64.b64decode(self.inclusion_promise)
+            )
 
-    This is an internal exception; users should not see it.
-    """
+        inclusion_proof = rekor_v1.InclusionProof(
+            log_index=self.inclusion_proof.log_index,
+            root_hash=bytes.fromhex(self.inclusion_proof.root_hash),
+            tree_size=self.inclusion_proof.tree_size,
+            hashes=[bytes.fromhex(hash_) for hash_ in self.inclusion_proof.hashes],
+            checkpoint=rekor_v1.Checkpoint(envelope=self.inclusion_proof.checkpoint),
+        )
 
-    pass
+        tlog_entry = rekor_v1.TransparencyLogEntry(
+            log_index=self.log_index,
+            log_id=common_v1.LogId(key_id=bytes.fromhex(self.log_id)),
+            integrated_time=self.integrated_time,
+            inclusion_promise=inclusion_promise,
+            inclusion_proof=inclusion_proof,
+            canonicalized_body=base64.b64decode(self.body),
+        )
 
+        # Fill in the appropriate kind
+        body_entry = TypeAdapter(ProposedEntry).validate_json(
+            tlog_entry.canonicalized_body
+        )
+        if not isinstance(body_entry, (Hashedrekord, Dsse)):
+            raise InvalidBundle("log entry is not of expected type")
 
-class InvalidRekorEntry(InvalidMaterials):
-    """
-    Raised if the effective Rekor entry in `VerificationMaterials.rekor_entry()`
-    does not match the other materials in `VerificationMaterials`.
+        tlog_entry.kind_version = rekor_v1.KindVersion(
+            kind=body_entry.kind, version=body_entry.api_version
+        )
 
-    This can only happen in two scenarios:
+        tlog_entry_dict: dict[str, Any] = tlog_entry.to_dict()
+        return tlog_entry_dict
 
-    * A user has supplied the wrong offline entry, potentially maliciously;
-    * The Rekor log responded with the wrong entry, suggesting a server error.
-    """
+    def encode_canonical(self) -> bytes:
+        """
+        Returns a canonicalized JSON (RFC 8785) representation of the transparency log entry.
 
-    pass
+        This encoded representation is suitable for verification against
+        the Signed Entry Timestamp.
+        """
+        payload: dict[str, int | str] = {
+            "body": self.body,
+            "integratedTime": self.integrated_time,
+            "logID": self.log_id,
+            "logIndex": self.log_index,
+        }
 
+        return rfc8785.dumps(payload)
 
-@dataclass(init=False)
-class VerificationMaterials:
-    """
-    Represents the materials needed to perform a Sigstore verification.
-    """
+    def _verify_set(self, keyring: RekorKeyring) -> None:
+        """
+        Verify the inclusion promise (Signed Entry Timestamp) for a given transparency log
+        `entry` using the given `keyring`.
 
-    input_digest: bytes
-    """
-    The SHA256 hash of the verification input, as raw bytes.
-    """
+        Fails if the given log entry does not contain an inclusion promise.
+        """
 
-    certificate: Certificate
-    """
-    The certificate that attests to and contains the public signing key.
-    """
+        if self.inclusion_promise is None:
+            raise VerificationError("SET: invalid inclusion promise: missing")
 
-    signature: bytes
-    """
-    The raw signature.
-    """
+        signed_entry_ts = base64.b64decode(self.inclusion_promise)
 
-    _offline: bool
-    """
-    Whether to do offline Rekor entry verification.
+        try:
+            keyring.verify(
+                key_id=KeyID(bytes.fromhex(self.log_id)),
+                signature=signed_entry_ts,
+                data=self.encode_canonical(),
+            )
+        except VerificationError as exc:
+            raise VerificationError(f"SET: invalid inclusion promise: {exc}")
 
-    NOTE: This is intentionally not a public field, since it's slightly
-    mismatched against the other members of `VerificationMaterials` -- it's
-    more of an option than a piece of verification material.
-    """
+    def _verify(self, keyring: RekorKeyring) -> None:
+        """
+        Verifies this log entry.
 
-    _rekor_entry: LogEntry | None
-    """
-    An optional Rekor entry.
+        This method performs steps (5), (6), and optionally (7) in
+        the top-level verify API:
+
+        * Verifies the consistency of the entry with the given bundle;
+        * Verifies the Merkle inclusion proof and its signed checkpoint;
+        * Verifies the inclusion promise, if present.
+        """
 
-    If a Rekor entry is supplied **and** `offline` is set to `True`,
-    verification will be done against this entry rather than the against the
-    online transparency log. If not provided **or** `offline` is `False` (the
-    default), then the online transparency log will be used.
+        verify_merkle_inclusion(self)
+        verify_checkpoint(keyring, self)
 
-    NOTE: This is **intentionally not a public field**. The `rekor_entry()`
-    method should be used to access a Rekor log entry for these materials,
-    as it performs the online lookup if an offline entry is not provided
-    and, **critically**, validates that the entry's contents match the other
-    signing materials. Without this check an adversary could present a
-    **valid but unrelated** Rekor entry during verification, similar
-    to CVE-2022-36056 in cosign.
+        _logger.debug(f"successfully verified inclusion proof: index={self.log_index}")
+
+        if self.inclusion_promise:
+            self._verify_set(keyring)
+            _logger.debug(
+                f"successfully verified inclusion promise: index={self.log_index}"
+            )
 
-    TODO: Support multiple entries here, with verification contingent on
-    all being valid.
+
+class InvalidBundle(Error):
+    """
+    Raised when the associated `Bundle` is invalid in some way.
     """
 
-    def __init__(
-        self,
-        *,
-        input_: IO[bytes],
-        cert_pem: PEMCert,
-        signature: bytes,
-        offline: bool = False,
-        rekor_entry: LogEntry | None,
-    ):
-        """
-        Create a new `VerificationMaterials` from the given materials.
+    def diagnostics(self) -> str:
+        """Returns diagnostics for the error."""
 
-        `offline` controls the behavior of any subsequent verification over
-        these materials: if `True`, the supplied Rekor entry (which must
-        be supplied) will be verified via its Signed Entry Timestamp, but
-        its proof of inclusion will not be checked. This is a slightly weaker
-        verification mode, as it demonstrates that an entry has been signed by
-        the log but not necessarily included in it.
+        return dedent(
+            f"""\
+        An issue occurred while parsing the Sigstore bundle.
 
-        Effect: `input_` is consumed as part of construction.
+        The provided bundle is malformed and may have been modified maliciously.
+
+        Additional context:
+
+        {self}
         """
+        )
 
-        self.input_digest = sha256_streaming(input_)
-        self.certificate = load_pem_x509_certificate(cert_pem.encode())
-        self.signature = signature
 
-        # Invariant: requesting offline verification means that a Rekor entry
-        # *must* be provided.
-        if offline and not rekor_entry:
-            raise InvalidMaterials("offline verification requires a Rekor entry")
+class Bundle:
+    """
+    Represents a Sigstore bundle.
+    """
 
-        self._offline = offline
-        self._rekor_entry = rekor_entry
+    def __init__(self, inner: _Bundle) -> None:
+        """
+        Creates a new bundle. This is not a public API; use
+        `from_json` instead.
 
-    @classmethod
-    def from_bundle(
-        cls, *, input_: IO[bytes], bundle: Bundle, offline: bool = False
-    ) -> VerificationMaterials:
+        @private
         """
-        Create a new `VerificationMaterials` from the given Sigstore bundle.
+        self._inner = inner
+        self._verify_bundle()
 
-        Effect: `input_` is consumed as part of construction.
+    def _verify_bundle(self) -> None:
         """
-        if bundle.media_type not in _KNOWN_BUNDLE_TYPES:
-            raise InvalidMaterials(f"unsupported bundle format: {bundle.media_type}")
+        Performs various feats of heroism to ensure the bundle is well-formed
+        and upholds invariants, including:
 
-        certs = bundle.verification_material.x509_certificate_chain.certificates
+        * The "leaf" (signing) certificate is present;
+        * There is a inclusion proof present, even if the Bundle's version
+           predates a mandatory inclusion proof.
+        """
 
-        if len(certs) == 0:
-            raise InvalidMaterials("expected non-empty certificate chain in bundle")
+        # The bundle must have a recognized media type.
+        try:
+            media_type = BundleType(self._inner.media_type)
+        except ValueError:
+            raise InvalidBundle(f"unsupported bundle format: {self._inner.media_type}")
 
-        # Per client policy in protobuf-specs: the first entry in the chain
-        # MUST be a leaf certificate, and the rest of the chain MUST NOT
-        # include a root CA or any intermediate CAs that appear in an
-        # independent root of trust.
-        #
-        # We expect some old bundles to violate the rules around root
-        # and intermediate CAs, so we issue warnings and not hard errors
-        # in those cases.
-        leaf_cert, *chain_certs = [
-            load_der_x509_certificate(cert.raw_bytes) for cert in certs
-        ]
-        if not cert_is_leaf(leaf_cert):
-            raise InvalidMaterials(
-                "bundle contains an invalid leaf or non-leaf certificate in the leaf position"
+        # Extract the signing certificate.
+        if media_type in (BundleType.BUNDLE_0_3, BundleType.BUNDLE_0_3_ALT):
+            # For "v3" bundles, the signing certificate is the only one present.
+            leaf_cert = load_der_x509_certificate(
+                self._inner.verification_material.certificate.raw_bytes
+            )
+        else:
+            # In older bundles, there is an entire pool (misleadingly called
+            # a chain) of certificates, the first of which is the signing
+            # certificate.
+            certs = (
+                self._inner.verification_material.x509_certificate_chain.certificates
             )
 
-        for chain_cert in chain_certs:
-            # TODO: We should also retrieve the root of trust here and
-            # cross-check against it.
-            if cert_is_root_ca(chain_cert):
-                logger.warning(
-                    "this bundle contains a root CA, making it subject to misuse"
+            if len(certs) == 0:
+                raise InvalidBundle("expected non-empty certificate chain in bundle")
+
+            # Per client policy in protobuf-specs: the first entry in the chain
+            # MUST be a leaf certificate, and the rest of the chain MUST NOT
+            # include a root CA or any intermediate CAs that appear in an
+            # independent root of trust.
+            #
+            # We expect some old bundles to violate the rules around root
+            # and intermediate CAs, so we issue warnings and not hard errors
+            # in those cases.
+            leaf_cert, *chain_certs = [
+                load_der_x509_certificate(cert.raw_bytes) for cert in certs
+            ]
+            if not cert_is_leaf(leaf_cert):
+                raise InvalidBundle(
+                    "bundle contains an invalid leaf or non-leaf certificate in the leaf position"
                 )
 
-        signature = bundle.message_signature.signature
+            for chain_cert in chain_certs:
+                # TODO: We should also retrieve the root of trust here and
+                # cross-check against it.
+                if cert_is_root_ca(chain_cert):
+                    _logger.warning(
+                        "this bundle contains a root CA, making it subject to misuse"
+                    )
+
+        self._signing_certificate = leaf_cert
 
-        tlog_entries = bundle.verification_material.tlog_entries
+        # Extract the log entry. For the time being, we expect
+        # bundles to only contain a single log entry.
+        tlog_entries = self._inner.verification_material.tlog_entries
         if len(tlog_entries) != 1:
-            raise InvalidMaterials(
-                f"expected exactly one log entry, got {len(tlog_entries)}"
-            )
+            raise InvalidBundle("expected exactly one log entry in bundle")
         tlog_entry = tlog_entries[0]
 
         # Handling of inclusion promises and proofs varies between bundle
         # format versions:
         #
         # * For 0.1, an inclusion promise is required; the client
         #   MUST verify the inclusion promise.
         #   The inclusion proof is NOT required. If provided, it might NOT
         #   contain a checkpoint; in this case, we ignore it (since it's
         #   useless without one).
         #
-        # * For 0.2, an inclusion proof is required; the client MUST
+        # * For 0.2+, an inclusion proof is required; the client MUST
         #   verify the inclusion proof. The inclusion prof MUST contain
         #   a checkpoint.
         #   The inclusion promise is NOT required; if present, the client
         #   SHOULD verify it.
-
-        inclusion_promise: InclusionPromise | None = tlog_entry.inclusion_promise
-        inclusion_proof: InclusionProof | None = tlog_entry.inclusion_proof
-        if bundle.media_type == _BUNDLE_0_1:
-            if not inclusion_promise:
-                raise InvalidMaterials("bundle must contain an inclusion promise")
-            if inclusion_proof and not inclusion_proof.checkpoint.envelope:
-                logger.debug(
+        #
+        # Before all of this, we require that the inclusion proof be present
+        # (when constructing the LogEntry).
+        log_entry = LogEntry._from_dict_rekor(tlog_entry.to_dict())
+
+        if media_type == BundleType.BUNDLE_0_1:
+            if not log_entry.inclusion_promise:
+                raise InvalidBundle("bundle must contain an inclusion promise")
+            if not log_entry.inclusion_proof.checkpoint:
+                _logger.debug(
                     "0.1 bundle contains inclusion proof without checkpoint; ignoring"
                 )
-        elif bundle.media_type == _BUNDLE_0_2:
-            if not inclusion_proof:
-                raise InvalidMaterials("bundle must contain an inclusion proof")
-            if not inclusion_proof.checkpoint.envelope:
-                raise InvalidMaterials("expected checkpoint in inclusion proof")
-
-        parsed_inclusion_proof: InclusionProof | None = None
-        if (
-            inclusion_proof is not None
-            and inclusion_proof.checkpoint.envelope is not None
-        ):
-            parsed_inclusion_proof = LogInclusionProof(
-                checkpoint=inclusion_proof.checkpoint.envelope,
-                hashes=[h.hex() for h in inclusion_proof.hashes],
-                log_index=inclusion_proof.log_index,
-                root_hash=inclusion_proof.root_hash.hex(),
-                tree_size=inclusion_proof.tree_size,
-            )
+        else:
+            if not log_entry.inclusion_proof.checkpoint:
+                raise InvalidBundle("expected checkpoint in inclusion proof")
 
-        entry = LogEntry(
-            uuid=None,
-            body=B64Str(base64.b64encode(tlog_entry.canonicalized_body).decode()),
-            integrated_time=tlog_entry.integrated_time,
-            log_id=tlog_entry.log_id.key_id.hex(),
-            log_index=tlog_entry.log_index,
-            inclusion_proof=parsed_inclusion_proof,
-            inclusion_promise=B64Str(
-                base64.b64encode(
-                    tlog_entry.inclusion_promise.signed_entry_timestamp
-                ).decode()
-            ),
-        )
+        self._log_entry = log_entry
 
-        return cls(
-            input_=input_,
-            cert_pem=PEMCert(leaf_cert.public_bytes(Encoding.PEM).decode()),
-            signature=signature,
-            offline=offline,
-            rekor_entry=entry,
-        )
+    @property
+    def signing_certificate(self) -> Certificate:
+        """Returns the bundle's contained signing (i.e. leaf) certificate."""
+        return self._signing_certificate
 
     @property
-    def has_rekor_entry(self) -> bool:
+    def log_entry(self) -> LogEntry:
         """
-        Returns whether or not these `VerificationMaterials` contain a Rekor
-        entry.
+        Returns the bundle's log entry, containing an inclusion proof
+        (with checkpoint) and an inclusion promise (if the latter is present).
+        """
+        return self._log_entry
 
-        If false, `VerificationMaterials.rekor_entry()` performs an online lookup.
+    @property
+    def _dsse_envelope(self) -> dsse.Envelope | None:
         """
-        return self._rekor_entry is not None
+        Returns the DSSE envelope within this Bundle as a `dsse.Envelope`.
 
-    def rekor_entry(self, client: RekorClient) -> LogEntry:
+        @private
         """
-        Returns a `LogEntry` for the current signing materials.
+        if self._inner.dsse_envelope:
+            return dsse.Envelope(self._inner.dsse_envelope)
+        return None
+
+    @classmethod
+    def from_json(cls, raw: bytes | str) -> Bundle:
         """
+        Deserialize the given Sigstore bundle.
+        """
+        inner = _Bundle().from_json(raw)
+        return cls(inner)
 
-        offline = self._offline
-        has_inclusion_promise = (
-            self.has_rekor_entry and self._rekor_entry.inclusion_promise is not None  # type: ignore
-        )
-        has_inclusion_proof = (
-            self.has_rekor_entry
-            and self._rekor_entry.inclusion_proof is not None  # type: ignore
-            and self._rekor_entry.inclusion_proof.checkpoint  # type: ignore
-        )
+    def to_json(self) -> str:
+        """
+        Return a JSON encoding of this bundle.
+        """
+        # TODO: Unclear why mypy doesn't like this.
+        return self._inner.to_json()  # type: ignore[no-any-return]
 
-        logger.debug(
-            f"has_inclusion_proof={has_inclusion_proof} "
-            f"has_inclusion_promise={has_inclusion_promise}"
+    @classmethod
+    def from_parts(cls, cert: Certificate, sig: bytes, log_entry: LogEntry) -> Bundle:
+        """
+        Construct a Sigstore bundle (of `hashedrekord` type) from its
+        constituent parts.
+        """
+
+        return cls._from_parts(
+            cert, common_v1.MessageSignature(signature=sig), log_entry
         )
 
-        # This "expected" entry is used both to retrieve the Rekor entry
-        # (if we don't have one) *and* to cross-check whatever response
-        # we receive. See below.
-        expected_entry = sigstore_rekor_types.Hashedrekord(
-            kind="hashedrekord",
-            api_version="0.0.1",
-            spec=sigstore_rekor_types.HashedrekordV001Schema(
-                signature=sigstore_rekor_types.Signature1(
-                    content=base64.b64encode(self.signature).decode(),
-                    public_key=sigstore_rekor_types.PublicKey1(
-                        content=base64_encode_pem_cert(self.certificate)
-                    ),
-                ),
-                data=sigstore_rekor_types.Data(
-                    hash=sigstore_rekor_types.Hash(
-                        algorithm=sigstore_rekor_types.Algorithm.SHA256,
-                        value=self.input_digest.hex(),
-                    ),
-                ),
+    @classmethod
+    def _from_parts(
+        cls,
+        cert: Certificate,
+        content: common_v1.MessageSignature | dsse.Envelope,
+        log_entry: LogEntry,
+    ) -> Bundle:
+        """
+        @private
+        """
+
+        inner = _Bundle(
+            media_type=BundleType.BUNDLE_0_3.value,
+            verification_material=bundle_v1.VerificationMaterial(
+                certificate=common_v1.X509Certificate(cert.public_bytes(Encoding.DER)),
             ),
         )
 
-        entry: LogEntry | None = None
-        if offline:
-            logger.debug("offline mode; using offline log entry")
-            # In offline mode, we require either an inclusion proof or an
-            # inclusion promise. Every `LogEntry` has at least one as a
-            # construction invariant, so no additional check is required here.
-            entry = self._rekor_entry
+        # Fill in the appropriate variants.
+        if isinstance(content, common_v1.MessageSignature):
+            inner.message_signature = content
         else:
-            # In online mode, we require an inclusion proof. If our supplied log
-            # entry doesn't have one, then we perform a lookup.
-            if not has_inclusion_proof:
-                logger.debug("retrieving transparency log entry")
-                entry = client.log.entries.retrieve.post(expected_entry)
-            else:
-                entry = self._rekor_entry
-
-        # No matter what we do above, we must end up with a Rekor entry.
-        if entry is None:
-            raise RekorEntryMissing
-
-        logger.debug("Rekor entry: ensuring contents match signing materials")
-
-        # To catch a potentially dishonest or compromised Rekor instance, we compare
-        # the expected entry (generated above) with the JSON structure returned
-        # by Rekor. If the two don't match, then we have an invalid entry
-        # and can't proceed.
-        actual_body = json.loads(base64.b64decode(entry.body))
-        if actual_body != expected_entry.model_dump(mode="json", by_alias=True):
-            raise InvalidRekorEntry
-
-        return entry
-
-    def to_bundle(self) -> Bundle:
-        """Converts VerificationMaterials into a Bundle. Requires that
-        the VerificationMaterials have a Rekor entry loaded. This is
-        the reverse operation of VerificationMaterials.from_bundle()
-        """
-        if not self.has_rekor_entry:
-            raise InvalidMaterials(
-                "Must have Rekor entry before converting to a Bundle"
-            )
-        rekor_entry: LogEntry = self._rekor_entry  # type: ignore[assignment]
+            inner.dsse_envelope = content._inner
 
-        inclusion_proof: InclusionProof | None = None
-        if rekor_entry.inclusion_proof is not None:
-            inclusion_proof = InclusionProof(
-                log_index=rekor_entry.inclusion_proof.log_index,
-                root_hash=bytes.fromhex(rekor_entry.inclusion_proof.root_hash),
-                tree_size=rekor_entry.inclusion_proof.tree_size,
-                hashes=[
-                    bytes.fromhex(hash_hex)
-                    for hash_hex in rekor_entry.inclusion_proof.hashes
-                ],
-                checkpoint=Checkpoint(envelope=rekor_entry.inclusion_proof.checkpoint),
-            )
-
-        inclusion_promise: InclusionPromise | None = None
-        if rekor_entry.inclusion_promise:
-            inclusion_promise = InclusionPromise(
-                signed_entry_timestamp=base64.b64decode(rekor_entry.inclusion_promise)
-            )
+        tlog_entry = rekor_v1.TransparencyLogEntry()
+        tlog_entry.from_dict(log_entry._to_dict_rekor())
+        inner.verification_material.tlog_entries = [tlog_entry]
 
-        bundle = Bundle(
-            media_type="application/vnd.dev.sigstore.bundle+json;version=0.2",
-            verification_material=VerificationMaterial(
-                public_key=PublicKeyIdentifier(),
-                x509_certificate_chain=X509CertificateChain(
-                    certificates=[
-                        X509Certificate(
-                            raw_bytes=self.certificate.public_bytes(Encoding.DER)
-                        )
-                    ]
-                ),
-                tlog_entries=[
-                    TransparencyLogEntry(
-                        log_index=rekor_entry.log_index,
-                        log_id=LogId(key_id=bytes.fromhex(rekor_entry.log_id)),
-                        kind_version=KindVersion(kind="hashedrekord", version="0.0.1"),
-                        integrated_time=rekor_entry.integrated_time,
-                        inclusion_promise=inclusion_promise,
-                        inclusion_proof=inclusion_proof,
-                        canonicalized_body=base64.b64decode(rekor_entry.body),
-                    )
-                ],
-            ),
-            message_signature=MessageSignature(
-                message_digest=HashOutput(
-                    algorithm=HashAlgorithm.SHA2_256,
-                    digest=self.input_digest,
-                ),
-                signature=self.signature,
-            ),
-        )
-        return bundle
+        return cls(inner)
```

### Comparing `sigstore-2.1.5/sigstore/verify/policy.py` & `sigstore-3.0.0rc1/sigstore/verify/policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,39 +17,29 @@
 passed into an individual verification step are verified.
 """
 
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from typing import cast
-
-try:
-    from typing import Protocol
-except ImportError:  # pragma: no cover
-    # TODO(ww): Remove when our minimum Python is 3.8.
-    from typing_extensions import Protocol  # type: ignore[assignment]
+from typing import Protocol
 
 from cryptography.x509 import (
     Certificate,
     ExtensionNotFound,
     ObjectIdentifier,
     OtherName,
     RFC822Name,
     SubjectAlternativeName,
     UniformResourceIdentifier,
 )
 
-from sigstore.verify.models import (
-    VerificationFailure,
-    VerificationResult,
-    VerificationSuccess,
-)
+from sigstore.errors import VerificationError
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 # From: https://github.com/sigstore/fulcio/blob/main/docs/oid-info.md
 _OIDC_ISSUER_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.1")
 _OIDC_GITHUB_WORKFLOW_TRIGGER_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.2")
 _OIDC_GITHUB_WORKFLOW_SHA_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.3")
 _OIDC_GITHUB_WORKFLOW_NAME_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.4")
 _OIDC_GITHUB_WORKFLOW_REPOSITORY_OID = ObjectIdentifier("1.3.6.1.4.1.57264.1.5")
@@ -71,41 +61,41 @@
     def __init__(self, value: str) -> None:
         """
         Creates the new policy, with `value` as the expected value during
         verification.
         """
         self._value = value
 
-    def verify(self, cert: Certificate) -> VerificationResult:
+    def verify(self, cert: Certificate) -> None:
         """
         Verify this policy against `cert`.
+
+        Raises `VerificationError` on failure.
         """
         try:
             ext = cert.extensions.get_extension_for_oid(self.oid).value
         except ExtensionNotFound:
-            return VerificationFailure(
-                reason=(
+            raise VerificationError(
+                (
                     f"Certificate does not contain {self.__class__.__name__} "
                     f"({self.oid.dotted_string}) extension"
                 )
             )
 
         # NOTE(ww): mypy is confused by the `Extension[ExtensionType]` returned
         # by `get_extension_for_oid` above.
         ext_value = ext.value.decode()  # type: ignore[attr-defined]
         if ext_value != self._value:
-            return VerificationFailure(
-                reason=(
+            raise VerificationError(
+                (
                     f"Certificate's {self.__class__.__name__} does not match "
                     f"(got {ext_value}, expected {self._value})"
                 )
             )
 
-        return VerificationSuccess()
-
 
 class OIDCIssuer(_SingleX509ExtPolicy):
     """
     Verifies the certificate's OIDC issuer, identified by
     an X.509v3 extension tagged with `1.3.6.1.4.1.57264.1.1`.
     """
 
@@ -160,17 +150,18 @@
 class VerificationPolicy(Protocol):
     """
     A protocol type describing the interface that all verification policies
     conform to.
     """
 
     @abstractmethod
-    def verify(self, cert: Certificate) -> VerificationResult:
+    def verify(self, cert: Certificate) -> None:
         """
-        Verify the given `cert` against this policy, returning a `VerificationResult`.
+        Verify the given `cert` against this policy, raising `VerificationError`
+        on failure.
         """
         raise NotImplementedError  # pragma: no cover
 
 
 class AnyOf:
     """
     The "any of" policy, corresponding to a logical OR between child policies.
@@ -180,25 +171,30 @@
 
     def __init__(self, children: list[VerificationPolicy]):
         """
         Create a new `AnyOf`, with the given child policies.
         """
         self._children = children
 
-    def verify(self, cert: Certificate) -> VerificationResult:
+    def verify(self, cert: Certificate) -> None:
         """
         Verify `cert` against the policy.
+
+        Raises `VerificationError` on failure.
         """
-        verified = any(child.verify(cert) for child in self._children)
-        if verified:
-            return VerificationSuccess()
-        else:
-            return VerificationFailure(
-                reason=f"0 of {len(self._children)} policies succeeded"
-            )
+
+        for child in self._children:
+            try:
+                child.verify(cert)
+            except VerificationError:
+                pass
+            else:
+                return
+
+        raise VerificationError(f"0 of {len(self._children)} policies succeeded")
 
 
 class AllOf:
     """
     The "all of" policy, corresponding to a logical AND between child
     policies.
 
@@ -208,61 +204,49 @@
     def __init__(self, children: list[VerificationPolicy]):
         """
         Create a new `AllOf`, with the given child policies.
         """
 
         self._children = children
 
-    def verify(self, cert: Certificate) -> VerificationResult:
+    def verify(self, cert: Certificate) -> None:
         """
         Verify `cert` against the policy.
         """
 
         # Without this, we'd consider empty lists of child policies trivially valid.
         # This is almost certainly not what the user wants and is a potential
         # source of API misuse, so we explicitly disallow it.
         if len(self._children) < 1:
-            return VerificationFailure(reason="no child policies to verify")
+            raise VerificationError("no child policies to verify")
 
-        # NOTE(ww): We need the cast here because MyPy can't tell that
-        # `VerificationResult.__bool__` is invariant with
-        # `VerificationSuccess | VerificationFailure`.
-        results = [child.verify(cert) for child in self._children]
-        failures = [
-            cast(VerificationFailure, result).reason for result in results if not result
-        ]
-        if len(failures) > 0:
-            inner_reasons = ", ".join(failures)
-            return VerificationFailure(
-                reason=f"{len(failures)} of {len(self._children)} policies failed: {inner_reasons}"
-            )
-        return VerificationSuccess()
+        for child in self._children:
+            child.verify(cert)
 
 
 class UnsafeNoOp:
     """
     The "no-op" policy, corresponding to a no-op "verification".
 
     **This policy is fundamentally insecure. You cannot use it safely.
     It must not be used to verify any sort of certificate identity, because
     it cannot do so. Using this policy is equivalent to reducing the
     verification proof down to an integrity check against a completely
     untrusted and potentially attacker-created signature. It must only
     be used for testing purposes.**
     """
 
-    def verify(self, cert: Certificate) -> VerificationResult:
+    def verify(self, cert: Certificate) -> None:
         """
         Verify `cert` against the policy.
         """
 
-        logger.warning(
+        _logger.warning(
             "unsafe (no-op) verification policy used! no verification performed!"
         )
-        return VerificationSuccess()
 
 
 class Identity:
     """
     Verifies the certificate's "identity", corresponding to the X.509v3 SAN.
     Identities are verified modulo an OIDC issuer, so the issuer's URI
     is also required.
@@ -274,22 +258,20 @@
         """
         Create a new `Identity`, with the given expected identity and issuer values.
         """
 
         self._identity = identity
         self._issuer = OIDCIssuer(issuer)
 
-    def verify(self, cert: Certificate) -> VerificationResult:
+    def verify(self, cert: Certificate) -> None:
         """
         Verify `cert` against the policy.
         """
 
-        issuer_verified: VerificationResult = self._issuer.verify(cert)
-        if not issuer_verified:
-            return issuer_verified
+        self._issuer.verify(cert)
 
         # Build a set of all valid identities.
         san_ext = cert.extensions.get_extension_for_class(SubjectAlternativeName).value
         all_sans = set(san_ext.get_values_for_type(RFC822Name))
         all_sans.update(san_ext.get_values_for_type(UniformResourceIdentifier))
         all_sans.update(
             [
@@ -297,12 +279,10 @@
                 for on in san_ext.get_values_for_type(OtherName)
                 if on.type_id == _OTHERNAME_OID
             ]
         )
 
         verified = self._identity in all_sans
         if not verified:
-            return VerificationFailure(
-                reason=f"Certificate's SANs do not match {self._identity}; actual SANs: {all_sans}"
+            raise VerificationError(
+                f"Certificate's SANs do not match {self._identity}; actual SANs: {all_sans}"
             )
-
-        return VerificationSuccess()
```

### Comparing `sigstore-2.1.5/sigstore/verify/verifier.py` & `sigstore-3.0.0rc1/sigstore/_internal/trustroot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,304 +1,326 @@
-# Copyright 2022 The Sigstore Authors
+# Copyright 2023 The Sigstore Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Verification API machinery.
+Trust root management for sigstore-python.
 """
 
 from __future__ import annotations
 
-import base64
-import datetime
-import logging
-from typing import List, cast
+from dataclasses import dataclass
+from datetime import datetime, timezone
+from enum import Enum
+from pathlib import Path
+from typing import ClassVar, Iterable, List, NewType
 
+import cryptography.hazmat.primitives.asymmetric.padding as padding
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import ec
-from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
-from cryptography.x509 import Certificate, ExtendedKeyUsage, KeyUsage
-from cryptography.x509.oid import ExtendedKeyUsageOID
-from OpenSSL.crypto import (  # type: ignore[import-untyped]
-    X509,
-    X509Store,
-    X509StoreContext,
-    X509StoreContextError,
+from cryptography.hazmat.primitives.asymmetric import ec, rsa
+from cryptography.x509 import (
+    Certificate,
+    load_der_x509_certificate,
 )
-from pydantic import ConfigDict
-
-from sigstore._internal.merkle import (
-    InvalidInclusionProofError,
-    verify_merkle_inclusion,
+from sigstore_protobuf_specs.dev.sigstore.common.v1 import PublicKey as _PublicKey
+from sigstore_protobuf_specs.dev.sigstore.common.v1 import (
+    PublicKeyDetails as _PublicKeyDetails,
 )
-from sigstore._internal.rekor.checkpoint import (
-    CheckpointError,
-    verify_checkpoint,
+from sigstore_protobuf_specs.dev.sigstore.common.v1 import TimeRange
+from sigstore_protobuf_specs.dev.sigstore.trustroot.v1 import (
+    CertificateAuthority,
+    TransparencyLogInstance,
 )
-from sigstore._internal.rekor.client import RekorClient
-from sigstore._internal.set import InvalidSETError, verify_set
-from sigstore._internal.tuf import TrustUpdater
-from sigstore._utils import B64Str, HexStr
-from sigstore.verify.models import InvalidRekorEntry as InvalidRekorEntryError
-from sigstore.verify.models import RekorEntryMissing as RekorEntryMissingError
-from sigstore.verify.models import (
-    VerificationFailure,
-    VerificationMaterials,
-    VerificationResult,
-    VerificationSuccess,
+from sigstore_protobuf_specs.dev.sigstore.trustroot.v1 import (
+    TrustedRoot as _TrustedRoot,
 )
-from sigstore.verify.policy import VerificationPolicy
 
-logger = logging.getLogger(__name__)
+from sigstore._internal.tuf import DEFAULT_TUF_URL, STAGING_TUF_URL, TrustUpdater
+from sigstore._utils import (
+    KeyID,
+    PublicKey,
+    key_id,
+    load_der_public_key,
+)
+from sigstore.errors import MetadataError, VerificationError
 
 
-class LogEntryMissing(VerificationFailure):
+def _is_timerange_valid(period: TimeRange | None, *, allow_expired: bool) -> bool:
     """
-    A specialization of `VerificationFailure` for transparency log lookup failures,
-    with additional lookup context.
+    Given a `period`, checks that the the current time is not before `start`. If
+    `allow_expired` is `False`, also checks that the current time is not after
+    `end`.
     """
+    now = datetime.now(timezone.utc)
 
-    reason: (
-        str
-    ) = "The transparency log has no entry for the given verification materials"
+    # If there was no validity period specified, the key is always valid.
+    if not period:
+        return True
 
-    signature: B64Str
-    """
-    The signature present during lookup failure, encoded with base64.
-    """
+    # Active: if the current time is before the starting period, we are not yet
+    # valid.
+    if now < period.start:
+        return False
 
-    artifact_hash: HexStr
-    """
-    The artifact hash present during lookup failure, encoded as a hex string.
-    """
+    # If we want Expired keys, the key is valid at this point. Otherwise, check
+    # that we are within range.
+    return allow_expired or (period.end is None or now <= period.end)
 
 
-class CertificateVerificationFailure(VerificationFailure):
+@dataclass(init=False)
+class Key:
     """
-    A specialization of `VerificationFailure` for certificate signature
-    verification failures, with additional exception context.
+    Represents a key in a `Keyring`.
     """
 
-    # Needed for the `exception` field above, since exceptions are
-    # not trivially serializable.
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+    hash_algorithm: hashes.HashAlgorithm
+    key: PublicKey
+    key_id: KeyID
+
+    _RSA_SHA_256_DETAILS: ClassVar[set[_PublicKeyDetails]] = {
+        _PublicKeyDetails.PKCS1_RSA_PKCS1V5,
+        _PublicKeyDetails.PKIX_RSA_PKCS1V15_2048_SHA256,
+        _PublicKeyDetails.PKIX_RSA_PKCS1V15_3072_SHA256,
+        _PublicKeyDetails.PKIX_RSA_PKCS1V15_4096_SHA256,
+    }
+
+    _EC_DETAILS_TO_HASH: ClassVar[dict[_PublicKeyDetails, hashes.HashAlgorithm]] = {
+        _PublicKeyDetails.PKIX_ECDSA_P256_SHA_256: hashes.SHA256(),
+        _PublicKeyDetails.PKIX_ECDSA_P384_SHA_384: hashes.SHA384(),
+        _PublicKeyDetails.PKIX_ECDSA_P521_SHA_512: hashes.SHA512(),
+    }
 
-    reason: str = "Failed to verify signing certificate"
-    exception: Exception
+    def __init__(self, public_key: _PublicKey) -> None:
+        """
+        Construct a key from the given Sigstore PublicKey message.
+        """
+
+        hash_algorithm: hashes.HashAlgorithm
+        if public_key.key_details in self._RSA_SHA_256_DETAILS:
+            hash_algorithm = hashes.SHA256()
+            key = load_der_public_key(public_key.raw_bytes, types=(rsa.RSAPublicKey,))
+        elif public_key.key_details in self._EC_DETAILS_TO_HASH:
+            hash_algorithm = self._EC_DETAILS_TO_HASH[public_key.key_details]
+            key = load_der_public_key(
+                public_key.raw_bytes, types=(ec.EllipticCurvePublicKey,)
+            )
+        else:
+            raise VerificationError(f"unsupported key type: {public_key.key_details}")
+
+        self.hash_algorithm = hash_algorithm
+        self.key = key
+        self.key_id = key_id(key)
+
+    def verify(self, signature: bytes, data: bytes) -> None:
+        """
+        Verifies the given `data` against `signature` using the current key.
+        """
+        if isinstance(self.key, rsa.RSAPublicKey):
+            self.key.verify(
+                signature=signature,
+                data=data,
+                # TODO: Parametrize this as well, for PSS.
+                padding=padding.PKCS1v15(),
+                algorithm=self.hash_algorithm,
+            )
+        elif isinstance(self.key, ec.EllipticCurvePublicKey):
+            self.key.verify(
+                signature=signature,
+                data=data,
+                signature_algorithm=ec.ECDSA(self.hash_algorithm),
+            )
+        else:
+            # Unreachable without API misuse.
+            raise VerificationError(f"keyring: unsupported key: {self.key}")
 
 
-class Verifier:
+class Keyring:
     """
-    The primary API for verification operations.
+    Represents a set of keys, each of which is a potentially valid verifier.
     """
 
-    def __init__(
-        self, *, rekor: RekorClient, fulcio_certificate_chain: List[Certificate]
-    ):
+    def __init__(self, public_keys: List[_PublicKey] = []):
+        """
+        Create a new `Keyring`, with `keys` as the initial set of verifying keys.
         """
-        Create a new `Verifier`.
+        self._keyring: dict[KeyID, Key] = {}
 
-        `rekor` is a `RekorClient` capable of connecting to a Rekor instance
-        containing logs for the file(s) being verified.
+        for public_key in public_keys:
+            key = Key(public_key)
+            self._keyring[key.key_id] = key
 
-        `fulcio_certificate_chain` is a list of PEM-encoded X.509 certificates,
-        establishing the trust chain for the signing certificate and signature.
+    def verify(self, *, key_id: KeyID, signature: bytes, data: bytes) -> None:
         """
-        self._rekor = rekor
+        Verify that `signature` is a valid signature for `data`, using the
+        key identified by `key_id`.
 
-        self._fulcio_certificate_chain: List[X509] = []
-        for parent_cert in fulcio_certificate_chain:
-            parent_cert_ossl = X509.from_cryptography(parent_cert)
-            self._fulcio_certificate_chain.append(parent_cert_ossl)
+        `key_id` is an unauthenticated hint; if no key matches the given key ID,
+        all keys in the keyring are tried.
 
-    @classmethod
-    def production(cls) -> Verifier:
-        """
-        Return a `Verifier` instance configured against Sigstore's production-level services.
+        Raises if the signature is invalid, i.e. is not valid for any of the
+        keys in the keyring.
         """
-        updater = TrustUpdater.production()
-        return cls(
-            rekor=RekorClient.production(updater),
-            fulcio_certificate_chain=updater.get_fulcio_certs(),
-        )
 
-    @classmethod
-    def staging(cls) -> Verifier:
-        """
-        Return a `Verifier` instance configured against Sigstore's staging-level services.
-        """
-        updater = TrustUpdater.staging()
-        return cls(
-            rekor=RekorClient.staging(updater),
-            fulcio_certificate_chain=updater.get_fulcio_certs(),
-        )
-
-    def verify(
-        self,
-        materials: VerificationMaterials,
-        policy: VerificationPolicy,
-    ) -> VerificationResult:
-        """Public API for verifying.
-
-        `materials` are the `VerificationMaterials` to verify.
-
-        `policy` is the `VerificationPolicy` to verify against.
-
-        Returns a `VerificationResult` which will be truthy or falsey depending on
-        success.
-        """
-
-        # NOTE: The `X509Store` object currently cannot have its time reset once the `set_time`
-        # method been called on it. To get around this, we construct a new one for every `verify`
-        # call.
-        store = X509Store()
-        for parent_cert_ossl in self._fulcio_certificate_chain:
-            store.add_cert(parent_cert_ossl)
-
-        # In order to verify an artifact, we need to achieve the following:
-        #
-        # 1) Verify that the signing certificate is signed by the certificate
-        #    chain and that the signing certificate was valid at the time
-        #    of signing.
-        # 2) Verify that the signing certificate belongs to the signer.
-        # 3) Verify that the artifact signature was signed by the public key in the
-        #    signing certificate.
-        # 4) Verify that the Rekor entry is consistent with the other signing
-        #    materials (preventing CVE-2022-36056)
-        # 5) Verify the inclusion proof supplied by Rekor for this artifact,
-        #    if we're doing online verification.
-        # 6) Verify the Signed Entry Timestamp (SET) supplied by Rekor for this
-        #    artifact.
-        # 7) Verify that the signing certificate was valid at the time of
-        #    signing by comparing the expiry against the integrated timestamp.
-
-        # 1) Verify that the signing certificate is signed by the root certificate and that the
-        #    signing certificate was valid at the time of signing.
-        sign_date = materials.certificate.not_valid_before
-        cert_ossl = X509.from_cryptography(materials.certificate)
-
-        store.set_time(sign_date)
-        store_ctx = X509StoreContext(store, cert_ossl)
-        try:
-            store_ctx.verify_certificate()
-        except X509StoreContextError as store_ctx_error:
-            return CertificateVerificationFailure(
-                exception=store_ctx_error,
-            )
+        key = self._keyring.get(key_id)
+        if key is not None:
+            candidates = [key]
+        else:
+            candidates = list(self._keyring.values())
 
-        # 2) Check that the signing certificate contains the proof claim as the subject
-        # Check usage is "digital signature"
-        usage_ext = materials.certificate.extensions.get_extension_for_class(KeyUsage)
-        if not usage_ext.value.digital_signature:
-            return VerificationFailure(
-                reason="Key usage is not of type `digital signature`"
-            )
+        # Try to verify each candidate key. In the happy case, this will
+        # be exactly one candidate.
+        valid = False
+        for candidate in candidates:
+            try:
+                candidate.verify(signature, data)
+                valid = True
+                break
+            except InvalidSignature:
+                pass
 
-        # Check that extended usage contains "code signing"
-        extended_usage_ext = materials.certificate.extensions.get_extension_for_class(
-            ExtendedKeyUsage
-        )
-        if ExtendedKeyUsageOID.CODE_SIGNING not in extended_usage_ext.value:
-            return VerificationFailure(
-                reason="Extended usage does not contain `code signing`"
-            )
+        if not valid:
+            raise VerificationError("keyring: invalid signature")
 
-        policy_check = policy.verify(materials.certificate)
-        if not policy_check:
-            return policy_check
-
-        logger.debug("Successfully verified signing certificate validity...")
-
-        # 3) Verify that the signature was signed by the public key in the signing certificate
-        try:
-            signing_key = materials.certificate.public_key()
-            signing_key = cast(ec.EllipticCurvePublicKey, signing_key)
-            signing_key.verify(
-                materials.signature,
-                materials.input_digest,
-                ec.ECDSA(Prehashed(hashes.SHA256())),
-            )
-        except InvalidSignature:
-            return VerificationFailure(reason="Signature is invalid for input")
 
-        logger.debug("Successfully verified signature...")
+RekorKeyring = NewType("RekorKeyring", Keyring)
+CTKeyring = NewType("CTKeyring", Keyring)
 
-        # 4) Retrieve the Rekor entry for this artifact (potentially from
-        # an offline entry), confirming its consistency with the other
-        # artifacts in the process.
-        try:
-            entry = materials.rekor_entry(self._rekor)
-        except RekorEntryMissingError:
-            return LogEntryMissing(
-                signature=B64Str(base64.b64encode(materials.signature).decode()),
-                artifact_hash=HexStr(materials.input_digest.hex()),
-            )
-        except InvalidRekorEntryError:
-            return VerificationFailure(
-                reason="Rekor entry contents do not match other signing materials"
-            )
 
-        # 5) Verify the inclusion proof supplied by Rekor for this artifact.
-        #
-        # The inclusion proof should always be present in the online case. In
-        # the offline case, if it is present, we verify it.
-        if entry.inclusion_proof and entry.inclusion_proof.checkpoint:
-            try:
-                verify_merkle_inclusion(entry)
-            except InvalidInclusionProofError as exc:
-                return VerificationFailure(
-                    reason=f"invalid Rekor inclusion proof: {exc}"
-                )
+class KeyringPurpose(str, Enum):
+    """
+    Keyring purpose typing
+    """
 
-            try:
-                verify_checkpoint(self._rekor, entry)
-            except CheckpointError as exc:
-                return VerificationFailure(reason=f"invalid Rekor root hash: {exc}")
+    SIGN = "sign"
+    VERIFY = "verify"
 
-            logger.debug(
-                f"successfully verified inclusion proof: index={entry.log_index}"
-            )
-        elif not materials._offline:
-            # Paranoia: if we weren't given an inclusion proof, then
-            # this *must* have been offline verification. If it was online
-            # then we've somehow entered an invalid state, so fail.
-            return VerificationFailure(reason="missing Rekor inclusion proof")
-        else:
-            logger.warning(
-                "inclusion proof not present in bundle: skipping due to offline verification"
-            )
+    def __str__(self) -> str:
+        """Returns the purpose string value."""
+        return self.value
 
-        # 6) Verify the Signed Entry Timestamp (SET) supplied by Rekor for this artifact
-        if entry.inclusion_promise:
-            try:
-                verify_set(self._rekor, entry)
-                logger.debug(
-                    f"successfully verified inclusion promise: index={entry.log_index}"
-                )
-            except InvalidSETError as inval_set:
-                return VerificationFailure(
-                    reason=f"invalid Rekor entry SET: {inval_set}"
-                )
-
-        # 7) Verify that the signing certificate was valid at the time of signing
-        integrated_time = datetime.datetime.utcfromtimestamp(entry.integrated_time)
-        if not (
-            materials.certificate.not_valid_before
-            <= integrated_time
-            <= materials.certificate.not_valid_after
-        ):
-            return VerificationFailure(
-                reason="invalid signing cert: expired at time of Rekor entry"
-            )
 
-        return VerificationSuccess()
+class TrustedRoot(_TrustedRoot):
+    """Complete set of trusted entities for a Sigstore client"""
+
+    purpose: KeyringPurpose
+
+    @classmethod
+    def from_file(
+        cls,
+        path: str,
+        purpose: KeyringPurpose = KeyringPurpose.VERIFY,
+    ) -> TrustedRoot:
+        """Create a new trust root from file"""
+        trusted_root: TrustedRoot = cls().from_json(Path(path).read_bytes())
+        trusted_root.purpose = purpose
+        return trusted_root
+
+    @classmethod
+    def from_tuf(
+        cls,
+        url: str,
+        offline: bool = False,
+        purpose: KeyringPurpose = KeyringPurpose.VERIFY,
+    ) -> TrustedRoot:
+        """Create a new trust root from a TUF repository.
+
+        If `offline`, will use trust root in local TUF cache. Otherwise will
+        update the trust root from remote TUF repository.
+        """
+        path = TrustUpdater(url, offline).get_trusted_root_path()
+        return cls.from_file(path, purpose)
+
+    @classmethod
+    def production(
+        cls,
+        offline: bool = False,
+        purpose: KeyringPurpose = KeyringPurpose.VERIFY,
+    ) -> TrustedRoot:
+        """Create new trust root from Sigstore production TUF repository.
+
+        If `offline`, will use trust root in local TUF cache. Otherwise will
+        update the trust root from remote TUF repository.
+        """
+        return cls.from_tuf(DEFAULT_TUF_URL, offline, purpose)
+
+    @classmethod
+    def staging(
+        cls,
+        offline: bool = False,
+        purpose: KeyringPurpose = KeyringPurpose.VERIFY,
+    ) -> TrustedRoot:
+        """Create new trust root from Sigstore staging TUF repository.
+
+        If `offline`, will use trust root in local TUF cache. Otherwise will
+        update the trust root from remote TUF repository.
+        """
+        return cls.from_tuf(STAGING_TUF_URL, offline, purpose)
+
+    @staticmethod
+    def _get_tlog_keys(
+        tlogs: list[TransparencyLogInstance], purpose: KeyringPurpose
+    ) -> Iterable[_PublicKey]:
+        """
+        Yields an iterator of public keys for transparency log instances that
+        are suitable for `purpose`.
+        """
+        allow_expired = purpose is KeyringPurpose.VERIFY
+        for tlog in tlogs:
+            if not _is_timerange_valid(
+                tlog.public_key.valid_for, allow_expired=allow_expired
+            ):
+                continue
+
+            yield tlog.public_key
+
+    @staticmethod
+    def _get_ca_keys(
+        cas: list[CertificateAuthority], *, allow_expired: bool
+    ) -> Iterable[bytes]:
+        """Return public key contents given certificate authorities."""
+
+        for ca in cas:
+            if not _is_timerange_valid(ca.valid_for, allow_expired=allow_expired):
+                continue
+            for cert in ca.cert_chain.certificates:
+                yield cert.raw_bytes
+
+    def rekor_keyring(self) -> RekorKeyring:
+        """Return keyring with keys for Rekor."""
+
+        keys: list[_PublicKey] = list(self._get_tlog_keys(self.tlogs, self.purpose))
+        if len(keys) != 1:
+            raise MetadataError("Did not find one Rekor key in trusted root")
+        return RekorKeyring(Keyring(keys))
+
+    def ct_keyring(self) -> CTKeyring:
+        """Return keyring with key for CTFE."""
+        ctfes: list[_PublicKey] = list(self._get_tlog_keys(self.ctlogs, self.purpose))
+        if not ctfes:
+            raise MetadataError("CTFE keys not found in trusted root")
+        return CTKeyring(Keyring(ctfes))
+
+    def get_fulcio_certs(self) -> list[Certificate]:
+        """Return the Fulcio certificates."""
+
+        certs: list[Certificate]
+
+        # Return expired certificates too: they are expired now but may have
+        # been active when the certificate was used to sign.
+        certs = [
+            load_der_x509_certificate(c)
+            for c in self._get_ca_keys(self.certificate_authorities, allow_expired=True)
+        ]
+        if not certs:
+            raise MetadataError("Fulcio certificates not found in trusted root")
+        return certs
```

### Comparing `sigstore-2.1.5/PKG-INFO` & `sigstore-3.0.0rc1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,7 @@
-Metadata-Version: 2.1
-Name: sigstore
-Version: 2.1.5
-Summary: A tool for signing Python package distributions
-Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Security
-Classifier: Topic :: Security :: Cryptography
-Requires-Dist: appdirs ~= 1.4
-Requires-Dist: cryptography >= 39
-Requires-Dist: id >= 1.1.0
-Requires-Dist: importlib_resources ~= 5.7; python_version < '3.11'
-Requires-Dist: pydantic >= 2,< 3
-Requires-Dist: pyjwt >= 2.1
-Requires-Dist: pyOpenSSL >= 23.0.0
-Requires-Dist: requests
-Requires-Dist: rich ~= 13.0
-Requires-Dist: securesystemslib < 0.32.0
-Requires-Dist: sigstore-protobuf-specs >= 0.2.2, < 0.4
-Requires-Dist: sigstore-rekor-types == 0.0.11
-Requires-Dist: tuf >= 2.1,< 4.0
-Requires-Dist: build ; extra == "dev"
-Requires-Dist: bump >= 1.3.2 ; extra == "dev"
-Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
-Requires-Dist: pdoc ; extra == "doc"
-Requires-Dist: bandit ; extra == "lint"
-Requires-Dist: interrogate ; extra == "lint"
-Requires-Dist: mypy ~= 1.1 ; extra == "lint"
-Requires-Dist: ruff < 0.1.8 ; extra == "lint"
-Requires-Dist: types-requests ; extra == "lint"
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: pretend ; extra == "test"
-Requires-Dist: coverage[toml] ; extra == "test"
-Project-URL: Documentation, https://sigstore.github.io/sigstore-python/
-Project-URL: Homepage, https://pypi.org/project/sigstore/
-Project-URL: Issues, https://github.com/sigstore/sigstore-python/issues
-Project-URL: Source, https://github.com/sigstore/sigstore-python
-Provides-Extra: dev
-Provides-Extra: doc
-Provides-Extra: lint
-Provides-Extra: test
-
 sigstore-python
 ===============
 
 <!--- @begin-badges@ --->
 ![CI](https://github.com/sigstore/sigstore-python/workflows/CI/badge.svg)
 [![PyPI version](https://badge.fury.io/py/sigstore.svg)](https://pypi.org/project/sigstore)
 [![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/sigstore/sigstore-python/badge)](https://securityscorecards.dev/viewer/?uri=github.com/sigstore/sigstore-python)
@@ -145,66 +92,61 @@
 python -m sigstore --help
 ```
 
 Top-level:
 
 <!-- @begin-sigstore-help@ -->
 ```
-usage: sigstore [-h] [-v] [-V] [--staging] [--rekor-url URL]
-                [--rekor-root-pubkey FILE]
-                COMMAND ...
+usage: sigstore [-h] [-v] [-V] [--staging] [--rekor-url URL] COMMAND ...
 
 a tool for signing and verifying Python package distributions
 
 positional arguments:
-  COMMAND               the operation to perform
-    sign                sign one or more inputs
-    verify              verify one or more inputs
-    get-identity-token  retrieve and return a Sigstore-compatible OpenID
-                        Connect token
+  COMMAND             the operation to perform
+    sign              sign one or more inputs
+    verify            verify one or more inputs
+    get-identity-token
+                      retrieve and return a Sigstore-compatible OpenID Connect
+                      token
 
 optional arguments:
-  -h, --help            show this help message and exit
-  -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
-  -V, --version         show program's version number and exit
+  -h, --help          show this help message and exit
+  -v, --verbose       run with additional debug logging; supply multiple times
+                      to increase verbosity (default: 0)
+  -V, --version       show program's version number and exit
 
 Sigstore instance options:
-  --staging             Use sigstore's staging instances, instead of the
-                        default production instances (default: False)
-  --rekor-url URL       The Rekor instance to use (conflicts with --staging)
-                        (default: https://rekor.sigstore.dev)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging) (default: None)
+  --staging           Use sigstore's staging instances, instead of the default
+                      production instances (default: False)
+  --rekor-url URL     The Rekor instance to use (conflicts with --staging)
+                      (default: https://rekor.sigstore.dev)
 ```
 <!-- @end-sigstore-help@ -->
 
 
 ### Signing
 
 <!-- @begin-sigstore-sign-help@ -->
 ```
 usage: sigstore sign [-h] [-v] [--identity-token TOKEN] [--oidc-client-id ID]
                      [--oidc-client-secret SECRET]
                      [--oidc-disable-ambient-providers] [--oidc-issuer URL]
                      [--oauth-force-oob] [--no-default-files]
                      [--signature FILE] [--certificate FILE] [--bundle FILE]
                      [--output-directory DIR] [--overwrite] [--staging]
-                     [--rekor-url URL] [--rekor-root-pubkey FILE]
-                     [--fulcio-url URL] [--ctfe FILE]
+                     [--rekor-url URL] [--fulcio-url URL]
                      FILE [FILE ...]
 
 positional arguments:
   FILE                  The file to sign
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
+                        times to increase verbosity (default: 0)
 
 OpenID Connect options:
   --identity-token TOKEN
                         the OIDC identity token to use (default: None)
   --oidc-client-id ID   The custom OpenID Connect client ID to use during
                         OAuth2 (default: sigstore)
   --oidc-client-secret SECRET
@@ -242,23 +184,16 @@
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
                         in a future release. (default: False)
   --rekor-url URL       The Rekor instance to use (conflicts with --staging).
                         This option will be deprecated in favor of the global
                         `--rekor-url` option in a future release. (default:
                         None)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging). This option will be
-                        deprecated in favor of the global `--rekor-root-
-                        pubkey` option in a future release. (default: None)
   --fulcio-url URL      The Fulcio instance to use (conflicts with --staging)
                         (default: https://fulcio.sigstore.dev)
-  --ctfe FILE           A PEM-encoded public key for the CT log (conflicts
-                        with --staging) (default: None)
 ```
 <!-- @end-sigstore-sign-help@ -->
 
 ### Verifying
 
 #### Generic identities
 
@@ -269,22 +204,21 @@
 
 <!-- @begin-sigstore-verify-identity-help@ -->
 ```
 usage: sigstore verify identity [-h] [-v] [--certificate FILE]
                                 [--signature FILE] [--bundle FILE]
                                 --cert-identity IDENTITY [--offline]
                                 --cert-oidc-issuer URL [--staging]
-                                [--rekor-url URL] [--rekor-root-pubkey FILE]
-                                [--certificate-chain FILE]
+                                [--rekor-url URL]
                                 FILE [FILE ...]
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
+                        times to increase verbosity (default: 0)
 
 Verification inputs:
   --certificate FILE, --cert FILE
                         The PEM-encoded certificate to verify against; not
                         used with multiple inputs (default: None)
   --signature FILE      The signature to verify against; not used with
                         multiple inputs (default: None)
@@ -307,23 +241,14 @@
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
                         in a future release. (default: False)
   --rekor-url URL       The Rekor instance to use (conflicts with --staging).
                         This option will be deprecated in favor of the global
                         `--rekor-url` option in a future release. (default:
                         None)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging). This option will be
-                        deprecated in favor of the global `--rekor-root-
-                        pubkey` option in a future release. (default: None)
-  --certificate-chain FILE
-                        Path to a list of CA certificates in PEM format which
-                        will be needed when building the certificate chain for
-                        the Fulcio signing certificate (default: None)
 ```
 <!-- @end-sigstore-verify-identity-help@ -->
 
 #### Signatures from GitHub Actions
 
 If your signatures are coming from GitHub Actions (e.g., a workflow
 that uses its [ambient credentials](#signing-with-ambient-credentials)),
@@ -333,22 +258,21 @@
 <!-- @begin-sigstore-verify-github-help@ -->
 ```
 usage: sigstore verify github [-h] [-v] [--certificate FILE]
                               [--signature FILE] [--bundle FILE]
                               --cert-identity IDENTITY [--offline]
                               [--trigger EVENT] [--sha SHA] [--name NAME]
                               [--repository REPO] [--ref REF] [--staging]
-                              [--rekor-url URL] [--rekor-root-pubkey FILE]
-                              [--certificate-chain FILE]
+                              [--rekor-url URL]
                               FILE [FILE ...]
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with additional debug logging; supply multiple
-                        times to increase verbosity
+                        times to increase verbosity (default: 0)
 
 Verification inputs:
   --certificate FILE, --cert FILE
                         The PEM-encoded certificate to verify against; not
                         used with multiple inputs (default: None)
   --signature FILE      The signature to verify against; not used with
                         multiple inputs (default: None)
@@ -378,23 +302,14 @@
                         default production instances. This option will be
                         deprecated in favor of the global `--staging` option
                         in a future release. (default: False)
   --rekor-url URL       The Rekor instance to use (conflicts with --staging).
                         This option will be deprecated in favor of the global
                         `--rekor-url` option in a future release. (default:
                         None)
-  --rekor-root-pubkey FILE
-                        A PEM-encoded root public key for Rekor itself
-                        (conflicts with --staging). This option will be
-                        deprecated in favor of the global `--rekor-root-
-                        pubkey` option in a future release. (default: None)
-  --certificate-chain FILE
-                        Path to a list of CA certificates in PEM format which
-                        will be needed when building the certificate chain for
-                        the Fulcio signing certificate (default: None)
 ```
 <!-- @end-sigstore-verify-github-help@ -->
 
 ## Example uses
 
 `sigstore` supports a wide variety of workflows and usages. Some common ones are
 provided below.
@@ -521,8 +436,7 @@
 process](https://github.com/sigstore/.github/blob/main/SECURITY.md).
 
 ### SLSA Provenance
 This project emits a SLSA provenance on its release! This enables you to verify the integrity
 of the downloaded artifacts and ensured that the binary's code really comes from this source code.
 
 To do so, please follow the instructions [here](https://github.com/slsa-framework/slsa-github-generator#verification-of-provenance).
-
```

