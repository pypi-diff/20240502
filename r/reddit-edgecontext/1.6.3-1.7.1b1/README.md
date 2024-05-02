# Comparing `tmp/reddit_edgecontext-1.6.3.tar.gz` & `tmp/reddit_edgecontext-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_edgecontext-1.6.3.tar", last modified: Fri Feb  3 23:32:27 2023, max compression
+gzip compressed data, was "reddit_edgecontext-1.7.1b1.tar", last modified: Thu May  2 17:18:17 2024, max compression
```

## Comparing `reddit_edgecontext-1.6.3.tar` & `reddit_edgecontext-1.7.1b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/reddit_edgecontext/
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    28317 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-03 23:32:27.795765 reddit_edgecontext-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/tests/edge_context_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:17.075254 reddit_edgecontext-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-02 17:18:17.075254 reddit_edgecontext-1.7.1b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:17.071254 reddit_edgecontext-1.7.1b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:17.071254 reddit_edgecontext-1.7.1b1/reddit_edgecontext/
+-rw-r--r--   0 runner    (1001) docker     (127)    23289 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:17.075254 reddit_edgecontext-1.7.1b1/reddit_edgecontext/thrift/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext/thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext/thrift/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27307 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext/thrift/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:17.075254 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-02 17:18:17.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-02 17:18:17.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:18:17.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 17:18:17.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 17:18:17.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:18:17.000000 reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-02 17:18:17.075254 reddit_edgecontext-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:17.075254 reddit_edgecontext-1.7.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-05-02 17:18:06.000000 reddit_edgecontext-1.7.1b1/tests/edge_context_tests.py
```

### Comparing `reddit_edgecontext-1.6.3/Makefile` & `reddit_edgecontext-1.7.1b1/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/PKG-INFO` & `reddit_edgecontext-1.7.1b1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,142 @@
 Metadata-Version: 2.1
 Name: reddit_edgecontext
-Version: 1.6.3
+Version: 1.7.1b1
 Summary: reddit edge request context baggage
 Home-page: https://github.com/reddit/edgecontext
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-edgecontext.readthedocs.io/
-Description: # edgecontext
-        
-        Python Documentation: https://reddit-edgecontext.readthedocs.io/en/latest/
-        
-        Go Documentation: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext
-        
-        Services deep within the backend often need to know information about the
-        client that originated the request, such as what user is authenticated or what
-        country they're in. Baseplate services can get this information from the edge
-        context which is automatically propagated along with calls between services.
-        
-        This library provides a Thrift specification of an edge context payload and a
-        corresponding implementation of the [`EdgeContextFactory`] interface from
-        Baseplate.py.
-        
-        [`EdgeContextFactory`]: https://baseplate.readthedocs.io/en/latest/api/baseplate/lib/edgecontext.html
-        
-        And an implementation of [`ecinterface`] from Baseplate.go.
-        
-        [`ecinterface`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface
-        
-        ## Usage
-        
-        ### Python
-        
-        Add the `EdgeContextFactory` to application startup:
-        
-        ```python
-        from baseplate import Baseplate
-        from baseplate.lib.secrets import secrets_store_from_config
-        from reddit_edgecontext import EdgeContextFactory
-        
-        
-        def make_processor(app_config):
-            secrets = secrets_store_from_config(app_config, timeout=60)
-            edgecontext_factory = EdgeContextFactory(secrets)
-        
-            # pass edgecontext_factory to your framework's integration
-            # for Thrift: baseplate.frameworks.thrift.baseplateify_processor
-            # for Pyramid: baseplate.frameworks.pyramid.BaseplateConfigurator
-        ```
-        
-        Then read fields while handling requests:
-        
-        ```python
-        def my_view(request):
-            return request.edge_context.user.id
-        ```
-        
-        See [the documentation] for all the available fields.
-        
-        [the documentation]: https://reddit-edgecontext.readthedocs.io/en/latest/
-        
-        ### Go
-        
-        Use [`edgecontext.Factory`] to create an [`ecinterface.Factory`] implementation
-        that's expected by [`baseplate.New`]:
-        
-        ```go
-        ctx, bp, err := baseplate.New(context.Background(), baseplate.NewArgs{
-          ConfigPath: configPath,
-          ServiceCfg: &cfg, // or nil if you don't have additional config to parse
-          EdgeContextFactory: edgecontext.Factory(edgecontext.Config{
-            Logger: log.ErrorWithSentryWrapper(),
-          }),
-        })
-        ```
-        
-        When using it, get the [`*EdgeRequestContext`] object out of context:
-        
-        ```go
-        if ec, ok := edgecontext.GetEdgeContext(ctx); ok {
-          user := ec.User()
-          loid, ok := user.LoID()
-          // Do something with loid
-        }
-        ```
-        
-        [`edgecontext.Factory`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#Factory
-        [`ecinterface.Factory`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface#Factory
-        [`baseplate.New`]: https://pkg.go.dev/github.com/reddit/baseplate.go#New
-        [`*EdgeRequestContext`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#EdgeRequestContext
-        
-        ## Development
-        
-        A Dockerfile is provided to get a development environment running. To use it,
-        build the base Docker image:
-        
-        ```console
-        $ docker build -t edgecontext .
-        ```
-        
-        And then fire up the environment and use the provided Makefile targets to do
-        common tasks:
-        
-        ```console
-        $ docker run -it -v $PWD:/src --user "$(id -u):$(id -g)" -w /src edgecontext
-        $ make fmt
-        ```
-        
-        The following make targets are provided:
-        
-        * `fmt`: Apply automatic formatting to the source code.
-        * `thrift`: Generate code from the Thrift IDL. Run `fmt` after doing this.
-        * `lint`: Run linters on the code.
-        * `test`: Run the test suite.
-        * `docs`: Build docs.
-            * Python output can be found in `lib/py/build/html/`.
-        
-        The generated Thrift code is committed to the Git repo, so if you change
-        `edgecontext.thrift` make sure to run `make thrift fmt` and commit those
-        changes as well.
-        
-        For Go, we do the same linting checks as Baseplate.go,
-        so please follow Baseplate.go's [Editor] guide to make sure you are doing the
-        same linting locally correctly.
-        Please also follow Baseplate.go's [Style] guide for code style.
-        
-        [Editor]: https://github.com/reddit/baseplate.go/blob/master/Editor.md
-        [Style]: https://github.com/reddit/baseplate.go/blob/master/Style.md
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: baseplate<3.0,>=1.5
+Requires-Dist: pyjwt<3.0,>=2.0.0
+Requires-Dist: thrift-unofficial<1.0,>=0.14
+Requires-Dist: cryptography>=3.0
+
+# edgecontext
+
+Python Documentation: https://reddit-edgecontext.readthedocs.io/en/latest/
+
+Go Documentation: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext
+
+Services deep within the backend often need to know information about the
+client that originated the request, such as what user is authenticated or what
+country they're in. Baseplate services can get this information from the edge
+context which is automatically propagated along with calls between services.
+
+This library provides a Thrift specification of an edge context payload and a
+corresponding implementation of the [`EdgeContextFactory`] interface from
+Baseplate.py.
+
+[`EdgeContextFactory`]: https://baseplate.readthedocs.io/en/latest/api/baseplate/lib/edgecontext.html
+
+And an implementation of [`ecinterface`] from Baseplate.go.
+
+[`ecinterface`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface
+
+## Usage
+
+### Python
+
+Add the `EdgeContextFactory` to application startup:
+
+```python
+from baseplate import Baseplate
+from baseplate.lib.secrets import secrets_store_from_config
+from reddit_edgecontext import EdgeContextFactory
+
+
+def make_processor(app_config):
+    secrets = secrets_store_from_config(app_config, timeout=60)
+    edgecontext_factory = EdgeContextFactory(secrets)
+
+    # pass edgecontext_factory to your framework's integration
+    # for Thrift: baseplate.frameworks.thrift.baseplateify_processor
+    # for Pyramid: baseplate.frameworks.pyramid.BaseplateConfigurator
+```
+
+Then read fields while handling requests:
+
+```python
+def my_view(request):
+    return request.edge_context.user.id
+```
+
+See [the documentation] for all the available fields.
+
+[the documentation]: https://reddit-edgecontext.readthedocs.io/en/latest/
+
+### Go
+
+Use [`edgecontext.Factory`] to create an [`ecinterface.Factory`] implementation
+that's expected by [`baseplate.New`]:
+
+```go
+ctx, bp, err := baseplate.New(context.Background(), baseplate.NewArgs{
+  ConfigPath: configPath,
+  ServiceCfg: &cfg, // or nil if you don't have additional config to parse
+  EdgeContextFactory: edgecontext.Factory(edgecontext.Config{
+    Logger: log.ErrorWithSentryWrapper(),
+  }),
+})
+```
+
+When using it, get the [`*EdgeRequestContext`] object out of context:
+
+```go
+if ec, ok := edgecontext.GetEdgeContext(ctx); ok {
+  user := ec.User()
+  loid, ok := user.LoID()
+  // Do something with loid
+}
+```
+
+[`edgecontext.Factory`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#Factory
+[`ecinterface.Factory`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface#Factory
+[`baseplate.New`]: https://pkg.go.dev/github.com/reddit/baseplate.go#New
+[`*EdgeRequestContext`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#EdgeRequestContext
+
+## Development
+
+A Dockerfile is provided to get a development environment running. To use it,
+build the base Docker image:
+
+```console
+$ docker build -t edgecontext .
+```
+
+And then fire up the environment and use the provided Makefile targets to do
+common tasks:
+
+```console
+$ docker run -it -v $PWD:/src --user "$(id -u):$(id -g)" -w /src edgecontext
+$ make fmt
+```
+
+The following make targets are provided:
+
+* `fmt`: Apply automatic formatting to the source code.
+* `thrift`: Generate code from the Thrift IDL. Run `fmt` after doing this.
+* `lint`: Run linters on the code.
+* `test`: Run the test suite.
+* `docs`: Build docs.
+    * Python output can be found in `lib/py/build/html/`.
+
+The generated Thrift code is committed to the Git repo, so if you change
+`edgecontext.thrift` make sure to run `make thrift fmt` and commit those
+changes as well.
+
+For Go, we do the same linting checks as Baseplate.go,
+so please follow Baseplate.go's [Editor] guide to make sure you are doing the
+same linting locally correctly.
+Please also follow Baseplate.go's [Style] guide for code style.
+
+[Editor]: https://github.com/reddit/baseplate.go/blob/master/Editor.md
+[Style]: https://github.com/reddit/baseplate.go/blob/master/Style.md
```

### Comparing `reddit_edgecontext-1.6.3/docs/conf.py` & `reddit_edgecontext-1.7.1b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/docs/index.rst` & `reddit_edgecontext-1.7.1b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/reddit_edgecontext/__init__.py` & `reddit_edgecontext-1.7.1b1/reddit_edgecontext/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,26 @@
     def loid(self) -> Optional[str]:
         raise NotImplementedError
 
     @property
     def loid_created_ms(self) -> Optional[int]:
         raise NotImplementedError
 
+    @property
+    def on_behalf_of_id(self) -> Optional[str]:
+        raise NotImplementedError
+
+    @property
+    def on_behalf_of_roles(self) -> Optional[Set[str]]:
+        raise NotImplementedError
+
+    @property
+    def requests_elevated_access(self) -> Optional[bool]:
+        raise NotImplementedError
+
 
 class ValidatedAuthenticationToken(AuthenticationToken):
     def __init__(self, payload: Dict[str, Any]):
         self.payload = payload
 
     @property
     def subject(self) -> Optional[str]:
@@ -146,14 +158,26 @@
     def loid(self) -> Optional[str]:
         return (self.payload.get("loid") or {}).get("id")
 
     @property
     def loid_created_ms(self) -> Optional[int]:
         return (self.payload.get("loid") or {}).get("created_ms")
 
+    @property
+    def on_behalf_of_id(self) -> Optional[str]:
+        return (self.payload.get("obo") or {}).get("aid")
+
+    @property
+    def on_behalf_of_roles(self) -> Optional[Set[str]]:
+        return (self.payload.get("obo") or {}).get("roles")
+
+    @property
+    def requests_elevated_access(self) -> Optional[bool]:
+        return self.payload.get("sea")
+
 
 class InvalidAuthenticationToken(AuthenticationToken):
     @property
     def subject(self) -> Optional[str]:
         raise NoAuthenticationError
 
     @cached_property
@@ -176,14 +200,26 @@
     def loid(self) -> Optional[str]:
         raise NoAuthenticationError
 
     @property
     def loid_created_ms(self) -> Optional[int]:
         raise NoAuthenticationError
 
+    @property
+    def on_behalf_of_id(self) -> Optional[str]:
+        raise NoAuthenticationError
+
+    @property
+    def on_behalf_of_roles(self) -> Optional[Set[str]]:
+        raise NoAuthenticationError
+
+    @property
+    def requests_elevated_access(self) -> Optional[bool]:
+        raise NoAuthenticationError
+
 
 class Session(NamedTuple):
     """Wrapper for the session values in the EdgeContext."""
 
     id: str
     """The ID of the session this request is part of."""
 
@@ -380,31 +416,54 @@
 
 class Service(NamedTuple):
     """Wrapper for the Service values in AuthenticationToken."""
 
     authentication_token: AuthenticationToken
     """The authentication token for this request."""
 
+    def is_service(self) -> bool:
+        subject = self.authentication_token.subject
+        if subject is None or subject == "":
+            return False
+        return subject.startswith("service/")
+
     @property
     def name(self) -> str:
         """Return the authenticated service name.
 
         :type: name string or None if context authentication is invalid
         :raises: :py:class:`NoAuthenticationError` if there was no
             authentication token, it was invalid, or the subject is not a
             service.
 
         """
         subject = self.authentication_token.subject
-        if not (subject and subject.startswith("service/")):
+        if subject is None or subject == "":
             raise NoAuthenticationError
-
         name = subject[len("service/") :]
         return name
 
+    @property
+    def on_behalf_of_id(self) -> Optional[str]:
+        if not self.is_service():
+            raise NoAuthenticationError
+        return self.authentication_token.on_behalf_of_id
+
+    @property
+    def on_behalf_of_roles(self) -> Optional[Set[str]]:
+        if not self.is_service():
+            raise NoAuthenticationError
+        return self.authentication_token.on_behalf_of_roles
+
+    @property
+    def requests_elevated_access(self) -> Optional[bool]:
+        if not self.is_service():
+            raise NoAuthenticationError
+        return self.authentication_token.requests_elevated_access
+
 
 class EdgeContext:
     """Contextual information about the initial request to an edge service.
 
     Once the :py:class:`~reddit_edgecontext.EdgeContextFactory` is set up, an
     instance of this object will be available at ``request.edge_context``.
 
@@ -476,17 +535,15 @@
     def request_id(self) -> RequestId:
         """:py:class:`~reddit_edgecontext.RequestId` object for the current context."""
         return RequestId(readable_id=self._t_request.request_id.readable_id)
 
     @cached_property
     def locale(self) -> Locale:
         """:py:class:`~reddit_edgecontext.Locale` object for the current context."""
-        return Locale(
-            locale_code=self._t_request.locale.locale_code,
-        )
+        return Locale(locale_code=self._t_request.locale.locale_code)
 
     @cached_property
     def _t_request(self) -> TRequest:
         _t_request = TRequest()
         _t_request.loid = TLoid()
         _t_request.session = TSession()
         _t_request.device = TDevice()
```

### Comparing `reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/ttypes.py` & `reddit_edgecontext-1.7.1b1/reddit_edgecontext/thrift/ttypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,17 @@
      - id: The ID of the LoID cookie.
 
      - created_ms: The time when the LoID cookie was created in epoch milliseconds.
 
 
     """
 
-    __slots__ = (
-        "id",
-        "created_ms",
-    )
+    __slots__ = ("id", "created_ms")
 
-    def __init__(
-        self,
-        id=None,
-        created_ms=None,
-    ):
+    def __init__(self, id=None, created_ms=None):
         self.id = id
         self.created_ms = created_ms
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
@@ -133,18 +126,15 @@
      - id: The ID of the Session tracker cookie.
 
 
     """
 
     __slots__ = ("id",)
 
-    def __init__(
-        self,
-        id=None,
-    ):
+    def __init__(self, id=None):
         self.id = id
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
             and self.thrift_spec is not None
@@ -217,18 +207,15 @@
      - id: The ID of the device.
 
 
     """
 
     __slots__ = ("id",)
 
-    def __init__(
-        self,
-        id=None,
-    ):
+    def __init__(self, id=None):
         self.id = id
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
             and self.thrift_spec is not None
@@ -302,18 +289,15 @@
      - name: The name of the origin service.
 
 
     """
 
     __slots__ = ("name",)
 
-    def __init__(
-        self,
-        name=None,
-    ):
+    def __init__(self, name=None):
         self.name = name
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
             and self.thrift_spec is not None
@@ -385,18 +369,15 @@
     Attributes:
      - country_code: The country code of the requesting client based on geographic location.
 
     """
 
     __slots__ = ("country_code",)
 
-    def __init__(
-        self,
-        country_code=None,
-    ):
+    def __init__(self, country_code=None):
         self.country_code = country_code
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
             and self.thrift_spec is not None
@@ -469,18 +450,15 @@
     Attributes:
      - readable_id: The id of this Edge Request, in the most human-readable format.
 
     """
 
     __slots__ = ("readable_id",)
 
-    def __init__(
-        self,
-        readable_id=None,
-    ):
+    def __init__(self, readable_id=None):
         self.readable_id = readable_id
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
             and self.thrift_spec is not None
@@ -556,18 +534,15 @@
     Preferably in BCP-47 format ({lang} or {lang}-{region}),
     but underscore separated locales also valid ({lang}_{region})
 
     """
 
     __slots__ = ("locale_code",)
 
-    def __init__(
-        self,
-        locale_code=None,
-    ):
+    def __init__(self, locale_code=None):
         self.locale_code = locale_code
 
     def read(self, iprot):
         if (
             iprot._fast_decode is not None
             and isinstance(iprot.trans, TTransport.CReadableTransport)
             and self.thrift_spec is not None
@@ -814,150 +789,36 @@
     def __ne__(self, other):
         return not (self == other)
 
 
 all_structs.append(Loid)
 Loid.thrift_spec = (
     None,  # 0
-    (
-        1,
-        TType.STRING,
-        "id",
-        "UTF8",
-        None,
-    ),  # 1
-    (
-        2,
-        TType.I64,
-        "created_ms",
-        None,
-        None,
-    ),  # 2
+    (1, TType.STRING, "id", "UTF8", None),  # 1
+    (2, TType.I64, "created_ms", None, None),  # 2
 )
 all_structs.append(Session)
-Session.thrift_spec = (
-    None,  # 0
-    (
-        1,
-        TType.STRING,
-        "id",
-        "UTF8",
-        None,
-    ),  # 1
-)
+Session.thrift_spec = (None, (1, TType.STRING, "id", "UTF8", None))  # 0  # 1
 all_structs.append(Device)
-Device.thrift_spec = (
-    None,  # 0
-    (
-        1,
-        TType.STRING,
-        "id",
-        "UTF8",
-        None,
-    ),  # 1
-)
+Device.thrift_spec = (None, (1, TType.STRING, "id", "UTF8", None))  # 0  # 1
 all_structs.append(OriginService)
-OriginService.thrift_spec = (
-    None,  # 0
-    (
-        1,
-        TType.STRING,
-        "name",
-        "UTF8",
-        None,
-    ),  # 1
-)
+OriginService.thrift_spec = (None, (1, TType.STRING, "name", "UTF8", None))  # 0  # 1
 all_structs.append(Geolocation)
-Geolocation.thrift_spec = (
-    None,  # 0
-    (
-        1,
-        TType.STRING,
-        "country_code",
-        "UTF8",
-        None,
-    ),  # 1
-)
+Geolocation.thrift_spec = (None, (1, TType.STRING, "country_code", "UTF8", None))  # 0  # 1
 all_structs.append(RequestId)
-RequestId.thrift_spec = (
-    None,  # 0
-    (
-        1,
-        TType.STRING,
-        "readable_id",
-        "UTF8",
-        None,
-    ),  # 1
-)
+RequestId.thrift_spec = (None, (1, TType.STRING, "readable_id", "UTF8", None))  # 0  # 1
 all_structs.append(Locale)
-Locale.thrift_spec = (
-    None,  # 0
-    (
-        1,
-        TType.STRING,
-        "locale_code",
-        "UTF8",
-        None,
-    ),  # 1
-)
+Locale.thrift_spec = (None, (1, TType.STRING, "locale_code", "UTF8", None))  # 0  # 1
 all_structs.append(Request)
 Request.thrift_spec = (
     None,  # 0
-    (
-        1,
-        TType.STRUCT,
-        "loid",
-        [Loid, None],
-        None,
-    ),  # 1
-    (
-        2,
-        TType.STRUCT,
-        "session",
-        [Session, None],
-        None,
-    ),  # 2
-    (
-        3,
-        TType.STRING,
-        "authentication_token",
-        "UTF8",
-        None,
-    ),  # 3
-    (
-        4,
-        TType.STRUCT,
-        "device",
-        [Device, None],
-        None,
-    ),  # 4
-    (
-        5,
-        TType.STRUCT,
-        "origin_service",
-        [OriginService, None],
-        None,
-    ),  # 5
-    (
-        6,
-        TType.STRUCT,
-        "geolocation",
-        [Geolocation, None],
-        None,
-    ),  # 6
-    (
-        7,
-        TType.STRUCT,
-        "request_id",
-        [RequestId, None],
-        None,
-    ),  # 7
-    (
-        8,
-        TType.STRUCT,
-        "locale",
-        [Locale, None],
-        None,
-    ),  # 8
+    (1, TType.STRUCT, "loid", [Loid, None], None),  # 1
+    (2, TType.STRUCT, "session", [Session, None], None),  # 2
+    (3, TType.STRING, "authentication_token", "UTF8", None),  # 3
+    (4, TType.STRUCT, "device", [Device, None], None),  # 4
+    (5, TType.STRUCT, "origin_service", [OriginService, None], None),  # 5
+    (6, TType.STRUCT, "geolocation", [Geolocation, None], None),  # 6
+    (7, TType.STRUCT, "request_id", [RequestId, None], None),  # 7
+    (8, TType.STRUCT, "locale", [Locale, None], None),  # 8
 )
 fix_spec(all_structs)
 del all_structs
```

### Comparing `reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/PKG-INFO` & `reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,142 @@
 Metadata-Version: 2.1
-Name: reddit-edgecontext
-Version: 1.6.3
+Name: reddit_edgecontext
+Version: 1.7.1b1
 Summary: reddit edge request context baggage
 Home-page: https://github.com/reddit/edgecontext
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-edgecontext.readthedocs.io/
-Description: # edgecontext
-        
-        Python Documentation: https://reddit-edgecontext.readthedocs.io/en/latest/
-        
-        Go Documentation: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext
-        
-        Services deep within the backend often need to know information about the
-        client that originated the request, such as what user is authenticated or what
-        country they're in. Baseplate services can get this information from the edge
-        context which is automatically propagated along with calls between services.
-        
-        This library provides a Thrift specification of an edge context payload and a
-        corresponding implementation of the [`EdgeContextFactory`] interface from
-        Baseplate.py.
-        
-        [`EdgeContextFactory`]: https://baseplate.readthedocs.io/en/latest/api/baseplate/lib/edgecontext.html
-        
-        And an implementation of [`ecinterface`] from Baseplate.go.
-        
-        [`ecinterface`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface
-        
-        ## Usage
-        
-        ### Python
-        
-        Add the `EdgeContextFactory` to application startup:
-        
-        ```python
-        from baseplate import Baseplate
-        from baseplate.lib.secrets import secrets_store_from_config
-        from reddit_edgecontext import EdgeContextFactory
-        
-        
-        def make_processor(app_config):
-            secrets = secrets_store_from_config(app_config, timeout=60)
-            edgecontext_factory = EdgeContextFactory(secrets)
-        
-            # pass edgecontext_factory to your framework's integration
-            # for Thrift: baseplate.frameworks.thrift.baseplateify_processor
-            # for Pyramid: baseplate.frameworks.pyramid.BaseplateConfigurator
-        ```
-        
-        Then read fields while handling requests:
-        
-        ```python
-        def my_view(request):
-            return request.edge_context.user.id
-        ```
-        
-        See [the documentation] for all the available fields.
-        
-        [the documentation]: https://reddit-edgecontext.readthedocs.io/en/latest/
-        
-        ### Go
-        
-        Use [`edgecontext.Factory`] to create an [`ecinterface.Factory`] implementation
-        that's expected by [`baseplate.New`]:
-        
-        ```go
-        ctx, bp, err := baseplate.New(context.Background(), baseplate.NewArgs{
-          ConfigPath: configPath,
-          ServiceCfg: &cfg, // or nil if you don't have additional config to parse
-          EdgeContextFactory: edgecontext.Factory(edgecontext.Config{
-            Logger: log.ErrorWithSentryWrapper(),
-          }),
-        })
-        ```
-        
-        When using it, get the [`*EdgeRequestContext`] object out of context:
-        
-        ```go
-        if ec, ok := edgecontext.GetEdgeContext(ctx); ok {
-          user := ec.User()
-          loid, ok := user.LoID()
-          // Do something with loid
-        }
-        ```
-        
-        [`edgecontext.Factory`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#Factory
-        [`ecinterface.Factory`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface#Factory
-        [`baseplate.New`]: https://pkg.go.dev/github.com/reddit/baseplate.go#New
-        [`*EdgeRequestContext`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#EdgeRequestContext
-        
-        ## Development
-        
-        A Dockerfile is provided to get a development environment running. To use it,
-        build the base Docker image:
-        
-        ```console
-        $ docker build -t edgecontext .
-        ```
-        
-        And then fire up the environment and use the provided Makefile targets to do
-        common tasks:
-        
-        ```console
-        $ docker run -it -v $PWD:/src --user "$(id -u):$(id -g)" -w /src edgecontext
-        $ make fmt
-        ```
-        
-        The following make targets are provided:
-        
-        * `fmt`: Apply automatic formatting to the source code.
-        * `thrift`: Generate code from the Thrift IDL. Run `fmt` after doing this.
-        * `lint`: Run linters on the code.
-        * `test`: Run the test suite.
-        * `docs`: Build docs.
-            * Python output can be found in `lib/py/build/html/`.
-        
-        The generated Thrift code is committed to the Git repo, so if you change
-        `edgecontext.thrift` make sure to run `make thrift fmt` and commit those
-        changes as well.
-        
-        For Go, we do the same linting checks as Baseplate.go,
-        so please follow Baseplate.go's [Editor] guide to make sure you are doing the
-        same linting locally correctly.
-        Please also follow Baseplate.go's [Style] guide for code style.
-        
-        [Editor]: https://github.com/reddit/baseplate.go/blob/master/Editor.md
-        [Style]: https://github.com/reddit/baseplate.go/blob/master/Style.md
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: baseplate<3.0,>=1.5
+Requires-Dist: pyjwt<3.0,>=2.0.0
+Requires-Dist: thrift-unofficial<1.0,>=0.14
+Requires-Dist: cryptography>=3.0
+
+# edgecontext
+
+Python Documentation: https://reddit-edgecontext.readthedocs.io/en/latest/
+
+Go Documentation: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext
+
+Services deep within the backend often need to know information about the
+client that originated the request, such as what user is authenticated or what
+country they're in. Baseplate services can get this information from the edge
+context which is automatically propagated along with calls between services.
+
+This library provides a Thrift specification of an edge context payload and a
+corresponding implementation of the [`EdgeContextFactory`] interface from
+Baseplate.py.
+
+[`EdgeContextFactory`]: https://baseplate.readthedocs.io/en/latest/api/baseplate/lib/edgecontext.html
+
+And an implementation of [`ecinterface`] from Baseplate.go.
+
+[`ecinterface`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface
+
+## Usage
+
+### Python
+
+Add the `EdgeContextFactory` to application startup:
+
+```python
+from baseplate import Baseplate
+from baseplate.lib.secrets import secrets_store_from_config
+from reddit_edgecontext import EdgeContextFactory
+
+
+def make_processor(app_config):
+    secrets = secrets_store_from_config(app_config, timeout=60)
+    edgecontext_factory = EdgeContextFactory(secrets)
+
+    # pass edgecontext_factory to your framework's integration
+    # for Thrift: baseplate.frameworks.thrift.baseplateify_processor
+    # for Pyramid: baseplate.frameworks.pyramid.BaseplateConfigurator
+```
+
+Then read fields while handling requests:
+
+```python
+def my_view(request):
+    return request.edge_context.user.id
+```
+
+See [the documentation] for all the available fields.
+
+[the documentation]: https://reddit-edgecontext.readthedocs.io/en/latest/
+
+### Go
+
+Use [`edgecontext.Factory`] to create an [`ecinterface.Factory`] implementation
+that's expected by [`baseplate.New`]:
+
+```go
+ctx, bp, err := baseplate.New(context.Background(), baseplate.NewArgs{
+  ConfigPath: configPath,
+  ServiceCfg: &cfg, // or nil if you don't have additional config to parse
+  EdgeContextFactory: edgecontext.Factory(edgecontext.Config{
+    Logger: log.ErrorWithSentryWrapper(),
+  }),
+})
+```
+
+When using it, get the [`*EdgeRequestContext`] object out of context:
+
+```go
+if ec, ok := edgecontext.GetEdgeContext(ctx); ok {
+  user := ec.User()
+  loid, ok := user.LoID()
+  // Do something with loid
+}
+```
+
+[`edgecontext.Factory`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#Factory
+[`ecinterface.Factory`]: https://pkg.go.dev/github.com/reddit/baseplate.go/ecinterface#Factory
+[`baseplate.New`]: https://pkg.go.dev/github.com/reddit/baseplate.go#New
+[`*EdgeRequestContext`]: https://pkg.go.dev/github.com/reddit/edgecontext/lib/go/edgecontext#EdgeRequestContext
+
+## Development
+
+A Dockerfile is provided to get a development environment running. To use it,
+build the base Docker image:
+
+```console
+$ docker build -t edgecontext .
+```
+
+And then fire up the environment and use the provided Makefile targets to do
+common tasks:
+
+```console
+$ docker run -it -v $PWD:/src --user "$(id -u):$(id -g)" -w /src edgecontext
+$ make fmt
+```
+
+The following make targets are provided:
+
+* `fmt`: Apply automatic formatting to the source code.
+* `thrift`: Generate code from the Thrift IDL. Run `fmt` after doing this.
+* `lint`: Run linters on the code.
+* `test`: Run the test suite.
+* `docs`: Build docs.
+    * Python output can be found in `lib/py/build/html/`.
+
+The generated Thrift code is committed to the Git repo, so if you change
+`edgecontext.thrift` make sure to run `make thrift fmt` and commit those
+changes as well.
+
+For Go, we do the same linting checks as Baseplate.go,
+so please follow Baseplate.go's [Editor] guide to make sure you are doing the
+same linting locally correctly.
+Please also follow Baseplate.go's [Style] guide for code style.
+
+[Editor]: https://github.com/reddit/baseplate.go/blob/master/Editor.md
+[Style]: https://github.com/reddit/baseplate.go/blob/master/Style.md
```

### Comparing `reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/SOURCES.txt` & `reddit_edgecontext-1.7.1b1/reddit_edgecontext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/requirements-transitive.txt` & `reddit_edgecontext-1.7.1b1/requirements-transitive.txt`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/setup.cfg` & `reddit_edgecontext-1.7.1b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/setup.py` & `reddit_edgecontext-1.7.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.3/tests/edge_context_tests.py` & `reddit_edgecontext-1.7.1b1/tests/edge_context_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,14 +77,17 @@
     )
     # Empty locale struct
     + b"\x0c\x00\x08\x00"
     # end of EdgeContext
     + b"\x00"
 )
 
+SERIALIZED_EDGECONTEXT_WITH_VALID_SERVICE_AUTH = b"\x0c\x00\x01\x00\x0c\x00\x02\x00\x0b\x00\x03\x00\x00\x02\x0aeyJhbGciOiJSUzI1NiIsImtpZCI6IlNIQTI1NjpsWjBoa1dSc0RwYXBlQnUyZWtYOVdZMm9ZSW5Id2RSYVhUd3RCZWNEaWNJIiwidHlwIjoiSldUIn0.eyJzdWIiOiJzZXJ2aWNlL3Rlc3Qtc2VydmljZSIsImV4cCI6MjUyNDYwODAwMH0.P41Iahxu-Bbg5srTFSQTBkzwiff4ytlhVBUYuyYTFGY_7XCyKdZywUmVHRY_Q2w8Q2uaybnmuoM95JhRpdNYcTPIYWEby4Z5DSV-zMqqmHnP22aH_sAckFQl86Yw_2pdZpKKJ-KQkyT0vEkxe-vNs5HhEdBr6Rae0g2SKEr7RaPMoToq6xpucDAREVWa7yJMtyyNtiVixeLoxTegRLOZTFEVt4TTYKDuT2FdEY5P2b8BOSpFMoiv9w51gZO1qvn9Zjrl00Z-lI_onihMIkrG_viWVAlzEl8d5ZWuJVjHJvm7O0CS4OuhZocE2qbYQrw9THSS1Mh4YR-_r2v1ArYnVA\x0c\x00\x04\x00\x0c\x00\x05\x0b\x00\x01\x00\x00\x00\x0eorigin/service\x00\x0c\x00\x06\x00\x0c\x00\x07\x0b\x00\x01\x00\x00\x00$1566dce9-9567-4952-b23b-9fd72e111162\x00\x00"
+SERIALIZED_EDGECONTEXT_WITH_VALID_SERVICE_AUTH_AND_OPTIONS = b"\x0c\x00\x01\x00\x0c\x00\x02\x00\x0b\x00\x03\x00\x00\x02VeyJhbGciOiJSUzI1NiIsImtpZCI6IlNIQTI1NjpsWjBoa1dSc0RwYXBlQnUyZWtYOVdZMm9ZSW5Id2RSYVhUd3RCZWNEaWNJIiwidHlwIjoiSldUIn0.eyJzdWIiOiJzZXJ2aWNlL3Rlc3Qtc2VydmljZSIsImV4cCI6MjUyNDYwODAwMCwib2JvIjp7ImFpZCI6InQyX2RlYWRiZWVmIiwicm9sZXMiOlsiYWRtaW4iXX0sInNlYSI6dHJ1ZX0.PVefAKWUFfk_7QKen6Iz0Cfu95Yp92lYETlrxCUacLsa9u-qz36aet21iwFrdnJiz7gDeJRH7sOJyh6jRmkD0ptWs4Zl7VqpZY-ALgDOdhwSHoUIoV2L7twT-Dm3Tdyfbzq01fOni9ioq5akKnETC5IbLSOqp1ssWJcgo_9g-X-SdRiuf5u8YHD2Mrep5U21bkbYnm4rK9tX_oCnhrrp4rbXi5yogx594oNmOWUedIeyv6QY_xVGbaXOz7deBIWQY2fSYG3cpiBNtSYEJ4yDTbjGY0G1Vp78bX8YZlboc13TGoDpARdfHuHeQU0wAQEhi7pu0Q4FufEVua4q1f0P3A\x0c\x00\x04\x00\x0c\x00\x05\x0b\x00\x01\x00\x00\x00\x0eorigin/service\x00\x0c\x00\x06\x00\x0c\x00\x07\x0b\x00\x01\x00\x00\x00$a3b2d5c2-ab27-4948-9dae-78a3ffb46957\x00\x00"
+
 
 class AuthenticationTokenTests(unittest.TestCase):
     def test_validated_authentication_token(self):
         payload = {
             "sub": "t2_user",
             "exp": 1574458470,
             "client_id": "client_id",
@@ -124,14 +127,28 @@
         token = InvalidAuthenticationToken()
         for attr in dir(token):
             if attr.startswith("__"):
                 continue
             with self.assertRaises(NoAuthenticationError):
                 getattr(token, attr)
 
+    def test_validated_service_authentication_token(self):
+        payload = {
+            "sub": "service/test-service",
+            "exp": 1574458470,
+            "obo": {"aid": "t2_deadbeef", "roles": ["admin"]},
+            "sea": True,
+        }
+
+        token = ValidatedAuthenticationToken(payload)
+        self.assertEqual(token.subject, "service/test-service")
+        self.assertEqual(token.on_behalf_of_roles, ["admin"])
+        self.assertEqual(token.on_behalf_of_id, "t2_deadbeef")
+        self.assertEqual(token.requests_elevated_access, True)
+
 
 class EdgeContextTests(unittest.TestCase):
     LOID_ID = "t2_deadbeef"
     LOID_CREATED_MS = 100000
     SESSION_ID = "beefdead"
     DEVICE_ID = "becc50f6-ff3d-407a-aa49-fa49531363be"
     ORIGIN_NAME = "baseplate"
@@ -320,7 +337,25 @@
                 "user_id": None,
                 "logged_in": False,
                 "session_id": None,
                 "oauth_client_id": None,
                 "edge_request_id": REQUEST_ID,
             },
         )
+
+    def test_service_auth(self):
+        request_context = self.factory.from_upstream(SERIALIZED_EDGECONTEXT_WITH_VALID_SERVICE_AUTH)
+
+        self.assertEqual(request_context.service.name, "test-service")
+        self.assertEqual(request_context.service.on_behalf_of_id, None)
+        self.assertEqual(request_context.service.on_behalf_of_roles, None)
+        self.assertEqual(request_context.service.requests_elevated_access, None)
+
+    def test_service_auth_with_additional_options(self):
+        request_context = self.factory.from_upstream(
+            SERIALIZED_EDGECONTEXT_WITH_VALID_SERVICE_AUTH_AND_OPTIONS
+        )
+
+        self.assertEqual(request_context.service.name, "test-service")
+        self.assertEqual(request_context.service.on_behalf_of_id, "t2_deadbeef")
+        self.assertEqual(request_context.service.on_behalf_of_roles, ["admin"])
+        self.assertEqual(request_context.service.requests_elevated_access, True)
```

