# Comparing `tmp/ufmt-2.5.1.tar.gz` & `tmp/ufmt-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufmt-2.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ufmt-2.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ufmt-2.5.1.tar` & `ufmt-2.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      180 2022-08-24 05:22:22.088722 ufmt-2.5.1/.flake8
--rw-r--r--   0        0        0     1825 2022-08-24 05:22:22.089380 ufmt-2.5.1/.gitignore
--rw-r--r--   0        0        0       45 2023-03-12 06:58:49.964569 ufmt-2.5.1/.mailmap
--rw-r--r--   0        0        0      202 2022-08-24 05:22:22.089533 ufmt-2.5.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      195 2023-10-19 04:08:48.470558 ufmt-2.5.1/.readthedocs.yml
--rw-r--r--   0        0        0     8070 2024-02-28 08:38:39.454752 ufmt-2.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      611 2023-08-02 02:55:24.080656 ufmt-2.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1071 2022-08-24 05:22:29.431182 ufmt-2.5.1/LICENSE
--rw-r--r--   0        0        0     4360 2024-02-28 06:25:56.292786 ufmt-2.5.1/README.md
--rw-r--r--   0        0        0     1804 2024-02-12 01:47:12.896998 ufmt-2.5.1/action.yml
--rw-r--r--   0        0        0      598 2022-08-24 05:22:22.090743 ufmt-2.5.1/docs/_static/custom.css
--rw-r--r--   0        0        0    42080 2022-08-24 05:22:22.091388 ufmt-2.5.1/docs/_static/omnilib.png
--rw-r--r--   0        0        0      342 2022-08-24 05:22:22.091641 ufmt-2.5.1/docs/_templates/badges.html
--rw-r--r--   0        0        0     1145 2022-08-24 05:22:22.091821 ufmt-2.5.1/docs/_templates/omnilib.html
--rw-r--r--   0        0        0     1402 2024-02-28 06:25:56.293013 ufmt-2.5.1/docs/api.rst
--rw-r--r--   0        0        0       70 2022-08-24 05:22:29.442268 ufmt-2.5.1/docs/changelog.rst
--rw-r--r--   0        0        0     3259 2022-08-24 05:22:29.445551 ufmt-2.5.1/docs/conf.py
--rw-r--r--   0        0        0       79 2022-08-24 05:22:29.448700 ufmt-2.5.1/docs/contributing.rst
--rw-r--r--   0        0        0     7429 2024-02-28 06:25:56.293299 ufmt-2.5.1/docs/guide.rst
--rw-r--r--   0        0        0      167 2022-08-24 05:22:29.454689 ufmt-2.5.1/docs/index.rst
--rw-r--r--   0        0        0     1017 2024-02-28 08:37:13.611204 ufmt-2.5.1/makefile
--rw-r--r--   0        0        0     2469 2024-02-28 08:37:13.611777 ufmt-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      870 2024-02-28 08:37:13.612150 ufmt-2.5.1/ufmt/__init__.py
--rw-r--r--   0        0        0       61 2022-08-24 05:22:29.490740 ufmt-2.5.1/ufmt/__main__.py
--rw-r--r--   0        0        0      156 2024-02-28 08:38:39.461064 ufmt-2.5.1/ufmt/__version__.py
--rw-r--r--   0        0        0     5254 2024-02-28 08:37:13.612632 ufmt-2.5.1/ufmt/cli.py
--rw-r--r--   0        0        0     1627 2024-02-28 07:42:45.010042 ufmt-2.5.1/ufmt/config.py
--rw-r--r--   0        0        0    18076 2024-02-28 08:37:13.613003 ufmt-2.5.1/ufmt/core.py
--rw-r--r--   0        0        0        0 2022-08-24 05:22:22.094333 ufmt-2.5.1/ufmt/py.typed
--rw-r--r--   0        0        0      176 2022-08-24 05:22:29.471932 ufmt-2.5.1/ufmt/tests/__init__.py
--rw-r--r--   0        0        0      236 2022-08-24 05:22:29.478841 ufmt-2.5.1/ufmt/tests/__main__.py
--rw-r--r--   0        0        0     2115 2024-02-28 08:37:13.613287 ufmt-2.5.1/ufmt/tests/benchmark.py
--rw-r--r--   0        0        0    19481 2024-02-28 08:37:13.613493 ufmt-2.5.1/ufmt/tests/cli.py
--rw-r--r--   0        0        0     8071 2024-02-28 08:37:13.613810 ufmt-2.5.1/ufmt/tests/config.py
--rw-r--r--   0        0        0    28671 2024-02-28 08:37:13.614059 ufmt-2.5.1/ufmt/tests/core.py
--rw-r--r--   0        0        0     2551 2024-02-28 08:37:13.614414 ufmt-2.5.1/ufmt/tests/util.py
--rw-r--r--   0        0        0     2744 2024-02-28 08:37:13.614657 ufmt-2.5.1/ufmt/types.py
--rw-r--r--   0        0        0     3343 2024-02-28 08:37:13.614995 ufmt-2.5.1/ufmt/util.py
--rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 ufmt-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2022-08-24 05:22:22.088722 ufmt-2.6.0/.flake8
+-rw-r--r--   0        0        0     1825 2022-08-24 05:22:22.089380 ufmt-2.6.0/.gitignore
+-rw-r--r--   0        0        0       45 2023-03-12 06:58:49.964569 ufmt-2.6.0/.mailmap
+-rw-r--r--   0        0        0      202 2022-08-24 05:22:22.089533 ufmt-2.6.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      195 2023-10-19 04:08:48.470558 ufmt-2.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8257 2024-05-02 01:42:27.169833 ufmt-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      611 2023-08-02 02:55:24.080656 ufmt-2.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1071 2022-08-24 05:22:29.431182 ufmt-2.6.0/LICENSE
+-rw-r--r--   0        0        0     4360 2024-02-28 06:25:56.292786 ufmt-2.6.0/README.md
+-rw-r--r--   0        0        0     1804 2024-02-12 01:47:12.896998 ufmt-2.6.0/action.yml
+-rw-r--r--   0        0        0      598 2022-08-24 05:22:22.090743 ufmt-2.6.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    42080 2022-08-24 05:22:22.091388 ufmt-2.6.0/docs/_static/omnilib.png
+-rw-r--r--   0        0        0      342 2022-08-24 05:22:22.091641 ufmt-2.6.0/docs/_templates/badges.html
+-rw-r--r--   0        0        0     1145 2022-08-24 05:22:22.091821 ufmt-2.6.0/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0     1402 2024-02-28 06:25:56.293013 ufmt-2.6.0/docs/api.rst
+-rw-r--r--   0        0        0       70 2022-08-24 05:22:29.442268 ufmt-2.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0     3259 2022-08-24 05:22:29.445551 ufmt-2.6.0/docs/conf.py
+-rw-r--r--   0        0        0       79 2022-08-24 05:22:29.448700 ufmt-2.6.0/docs/contributing.rst
+-rw-r--r--   0        0        0     7426 2024-05-02 01:41:38.313139 ufmt-2.6.0/docs/guide.rst
+-rw-r--r--   0        0        0      167 2022-08-24 05:22:29.454689 ufmt-2.6.0/docs/index.rst
+-rw-r--r--   0        0        0     1017 2024-02-28 08:37:13.611204 ufmt-2.6.0/makefile
+-rw-r--r--   0        0        0     2470 2024-05-02 01:41:38.313415 ufmt-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      870 2024-02-28 08:37:13.612150 ufmt-2.6.0/ufmt/__init__.py
+-rw-r--r--   0        0        0       61 2022-08-24 05:22:29.490740 ufmt-2.6.0/ufmt/__main__.py
+-rw-r--r--   0        0        0      156 2024-05-02 01:42:27.176144 ufmt-2.6.0/ufmt/__version__.py
+-rw-r--r--   0        0        0     5254 2024-02-28 08:37:13.612632 ufmt-2.6.0/ufmt/cli.py
+-rw-r--r--   0        0        0     1627 2024-02-28 07:42:45.010042 ufmt-2.6.0/ufmt/config.py
+-rw-r--r--   0        0        0    18826 2024-05-02 01:41:38.313721 ufmt-2.6.0/ufmt/core.py
+-rw-r--r--   0        0        0        0 2022-08-24 05:22:22.094333 ufmt-2.6.0/ufmt/py.typed
+-rw-r--r--   0        0        0      176 2022-08-24 05:22:29.471932 ufmt-2.6.0/ufmt/tests/__init__.py
+-rw-r--r--   0        0        0      236 2022-08-24 05:22:29.478841 ufmt-2.6.0/ufmt/tests/__main__.py
+-rw-r--r--   0        0        0     2115 2024-02-28 08:37:13.613287 ufmt-2.6.0/ufmt/tests/benchmark.py
+-rw-r--r--   0        0        0    19481 2024-02-28 08:37:13.613493 ufmt-2.6.0/ufmt/tests/cli.py
+-rw-r--r--   0        0        0     8071 2024-02-28 08:37:13.613810 ufmt-2.6.0/ufmt/tests/config.py
+-rw-r--r--   0        0        0    29293 2024-05-02 01:41:38.314048 ufmt-2.6.0/ufmt/tests/core.py
+-rw-r--r--   0        0        0     2551 2024-02-28 08:37:13.614414 ufmt-2.6.0/ufmt/tests/util.py
+-rw-r--r--   0        0        0     3150 2024-05-02 01:41:38.314382 ufmt-2.6.0/ufmt/types.py
+-rw-r--r--   0        0        0     3343 2024-02-28 08:37:13.614995 ufmt-2.6.0/ufmt/util.py
+-rw-r--r--   0        0        0     5799 1970-01-01 00:00:00.000000 ufmt-2.6.0/PKG-INFO
```

### Comparing `ufmt-2.5.1/.gitignore` & `ufmt-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/CHANGELOG.md` & `ufmt-2.6.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 µfmt
 ====
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v2.6.0
+------
+
+Feature release
+
+- Experimental support for using ruff's import sorter (#213)
+
+```text
+$ git shortlog -s v2.5.1...v2.6.0
+     2	Amethyst Reese
+     7	dependabot[bot]
+```
+
+
 v2.5.1
 ------
 
 Bugfix release
 
 - Fix: pass target file path to ufmt config factory (#196, #197)
 - Types: enforce mypy strict mode (#200)
```

### Comparing `ufmt-2.5.1/CONTRIBUTING.md` & `ufmt-2.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/LICENSE` & `ufmt-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/README.md` & `ufmt-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/action.yml` & `ufmt-2.6.0/action.yml`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/docs/_static/custom.css` & `ufmt-2.6.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/docs/_static/omnilib.png` & `ufmt-2.6.0/docs/_static/omnilib.png`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/docs/_templates/omnilib.html` & `ufmt-2.6.0/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/docs/api.rst` & `ufmt-2.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/docs/conf.py` & `ufmt-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/docs/guide.rst` & `ufmt-2.6.0/docs/guide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     .. code-block:: toml
       :caption: pyproject.toml
 
       [tool.ufmt]
       sorter = "usort"
 
-    See :class:`~ufmt.types.Formatter` for list of supported choices.
+    See :class:`~ufmt.types.Sorter` for list of supported choices.
 
 
 Integrations
 ------------
 
 µfmt supports integrations with the following tools and services:
```

### Comparing `ufmt-2.5.1/makefile` & `ufmt-2.6.0/makefile`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/pyproject.toml` & `ufmt-2.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     "trailrunner>=1.2.1",
     "typing-extensions>=4.0",
     "usort>=1.0",
 ]
 
 [project.optional-dependencies]
 ruff = [
-    "ruff-api>=0.0.1",
+    "ruff-api>=0.0.5",
 ]
 dev = [
-    "attribution==1.7.0",
-    "black==24.2.0",
-    "coverage==7.4.1",
+    "attribution==1.7.1",
+    "black==24.4.2",
+    "coverage==7.5.0",
     "flit==3.9.0",
     "flake8==7.0.0",
-    "mypy==1.8.0",
-    "ruff-api==0.0.3",
+    "mypy==1.10.0",
+    "ruff-api==0.0.5",
     "usort==1.0.8.post1",
 ]
 docs = [
-    "sphinx==7.2.6",
-    "sphinx-mdinclude==0.5.3",
+    "sphinx==7.3.7",
+    "sphinx-mdinclude==0.6.0",
 ]
 
 [project.urls]
 Documentation = "https://ufmt.omnilib.dev"
 Github = "https://github.com/omnilib/ufmt"
 Changelog = "https://ufmt.omnilib.dev/en/latest/changelog.html"
```

### Comparing `ufmt-2.5.1/ufmt/__init__.py` & `ufmt-2.6.0/ufmt/__init__.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/cli.py` & `ufmt-2.6.0/ufmt/cli.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/config.py` & `ufmt-2.6.0/ufmt/config.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/core.py` & `ufmt-2.6.0/ufmt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import black
 import black.mode
 import black.report
 from moreorless import unified_diff
 from trailrunner import Trailrunner
 from usort import usort
+from usort.config import CAT_FIRST_PARTY, CAT_STANDARD_LIBRARY
 
 try:
     import ruff_api
 except ImportError:  # pragma: nocover
     pass
 
 from .config import load_config
@@ -103,14 +104,31 @@
 
     # run configured sorter
     if ufmt_config.sorter == Sorter.usort:
         result = usort(content, usort_config, path)
         if result.error:
             raise result.error
         content = result.output
+    elif ufmt_config.sorter == Sorter.ruff_api:
+        ruff_isort_options = ruff_api.SortOptions(
+            first_party_modules=[
+                imp
+                for imp, category in usort_config.known.items()
+                if category == CAT_FIRST_PARTY
+            ],
+            standard_library_modules=[
+                imp
+                for imp, category in usort_config.known.items()
+                if category == CAT_STANDARD_LIBRARY
+            ],
+        )
+        content_str = ruff_api.isort_string(
+            path.as_posix(), content.decode(encoding), options=ruff_isort_options
+        )
+        content = content_str.encode(encoding)
     elif ufmt_config.sorter == Sorter.skip:
         pass
     else:
         raise ValueError(f"{ufmt_config.sorter!r} is not a supported sorter")
 
     if path.suffix == ".pyi":
         black_config = replace(black_config, is_pyi=True)
@@ -123,25 +141,25 @@
                 content_str,
                 fast=False,
                 mode=black_config,
             )
         except black.report.NothingChanged:
             content = result.output
     elif ufmt_config.formatter == Formatter.ruff_api:
-        options = ruff_api.FormatOptions(
+        ruff_format_options = ruff_api.FormatOptions(
             target_version=str(
                 black_config.target_versions.pop()
                 if black_config.target_versions
                 else {black.mode.TargetVersion.PY38}
             ),
             line_width=black_config.line_length,
             preview=black_config.preview,
         )
         content_str = ruff_api.format_string(
-            path.as_posix(), content_str, options=options
+            path.as_posix(), content_str, options=ruff_format_options
         )
     else:
         raise ValueError(f"{ufmt_config.formatter!r} is not a supported formatter")
     content = content_str.encode(encoding)
 
     if post_processor is not None:
         content = post_processor(path, content, encoding=encoding)
```

### Comparing `ufmt-2.5.1/ufmt/tests/benchmark.py` & `ufmt-2.6.0/ufmt/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/tests/cli.py` & `ufmt-2.6.0/ufmt/tests/cli.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/tests/config.py` & `ufmt-2.6.0/ufmt/tests/config.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/tests/core.py` & `ufmt-2.6.0/ufmt/tests/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,18 @@
                     black_config=black_config,
                     usort_config=usort_config,
                 )
             ruff_mock.assert_called_once()
             black_mock.assert_not_called()
 
     @patch("ufmt.core.usort", wraps=usort.usort)
-    def test_ufmt_bytes_alternate_sorter(self, usort_mock: Mock) -> None:
+    @patch("ufmt.core.ruff_api.isort_string", wraps=ruff_api.isort_string)
+    def test_ufmt_bytes_alternate_sorter(
+        self, ruff_mock: Mock, usort_mock: Mock
+    ) -> None:
         black_config = BlackConfig()
         usort_config = UsortConfig()
 
         with self.subTest("default"):
             usort_mock.reset_mock()
             result = ufmt.ufmt_bytes(
                 Path("foo.py"),
@@ -245,14 +248,27 @@
                 ufmt_config=UfmtConfig(),
                 black_config=black_config,
                 usort_config=usort_config,
             )
             self.assertEqual(CORRECTLY_FORMATTED_CODE.encode(), result)
             usort_mock.assert_called_once()
 
+        with self.subTest("ruff-api"):
+            usort_mock.reset_mock()
+            result = ufmt.ufmt_bytes(
+                Path("foo.py"),
+                POORLY_FORMATTED_CODE.encode(),
+                ufmt_config=UfmtConfig(sorter=Sorter.ruff_api),
+                black_config=black_config,
+                usort_config=usort_config,
+            )
+            self.assertEqual(CORRECTLY_FORMATTED_CODE.encode(), result)
+            usort_mock.assert_not_called()
+            ruff_mock.assert_called_once()
+
         with self.subTest("skip"):
             usort_mock.reset_mock()
             result = ufmt.ufmt_bytes(
                 Path("foo.py"),
                 POORLY_FORMATTED_CODE.encode(),
                 ufmt_config=UfmtConfig(sorter=Sorter.skip),
                 black_config=black_config,
```

### Comparing `ufmt-2.5.1/ufmt/tests/util.py` & `ufmt-2.6.0/ufmt/tests/util.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/ufmt/types.py` & `ufmt-2.6.0/ufmt/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,14 +62,26 @@
 
     skip = "skip"
     """Skip sorting imports"""
 
     usort = "usort"
     """Use µsort (default)."""
 
+    ruff_api = "ruff-api"
+    """
+    **Experimental:**
+    Use Ruff's isort lint rules via unofficial
+    `ruff-api <https://pypi.org/project/ruff-api>`_ extension.
+
+    .. note::
+        This implementation still depends on and uses the ``[tool.usort]`` configuration
+        table from ``pyproject.toml`` rather than Ruff's own configuration options.
+        This may change in future updates.
+    """
+
 
 @dataclass
 class UfmtConfig:
     project_root: Optional[Path] = None
     pyproject_path: Optional[Path] = None
     excludes: List[str] = field(default_factory=list)
     formatter: Formatter = Formatter.black
```

### Comparing `ufmt-2.5.1/ufmt/util.py` & `ufmt-2.6.0/ufmt/util.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.5.1/PKG-INFO` & `ufmt-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufmt
-Version: 2.5.1
+Version: 2.6.0
 Summary: Safe, atomic formatting with black and µsort
 Author-email: Amethyst Reese <amy@n7.gg>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,25 +14,25 @@
 Requires-Dist: click>=8.0
 Requires-Dist: libcst>=0.4.0
 Requires-Dist: moreorless>=0.4.0
 Requires-Dist: tomlkit>=0.7.2
 Requires-Dist: trailrunner>=1.2.1
 Requires-Dist: typing-extensions>=4.0
 Requires-Dist: usort>=1.0
-Requires-Dist: attribution==1.7.0 ; extra == "dev"
-Requires-Dist: black==24.2.0 ; extra == "dev"
-Requires-Dist: coverage==7.4.1 ; extra == "dev"
+Requires-Dist: attribution==1.7.1 ; extra == "dev"
+Requires-Dist: black==24.4.2 ; extra == "dev"
+Requires-Dist: coverage==7.5.0 ; extra == "dev"
 Requires-Dist: flit==3.9.0 ; extra == "dev"
 Requires-Dist: flake8==7.0.0 ; extra == "dev"
-Requires-Dist: mypy==1.8.0 ; extra == "dev"
-Requires-Dist: ruff-api==0.0.3 ; extra == "dev"
+Requires-Dist: mypy==1.10.0 ; extra == "dev"
+Requires-Dist: ruff-api==0.0.5 ; extra == "dev"
 Requires-Dist: usort==1.0.8.post1 ; extra == "dev"
-Requires-Dist: sphinx==7.2.6 ; extra == "docs"
-Requires-Dist: sphinx-mdinclude==0.5.3 ; extra == "docs"
-Requires-Dist: ruff-api>=0.0.1 ; extra == "ruff"
+Requires-Dist: sphinx==7.3.7 ; extra == "docs"
+Requires-Dist: sphinx-mdinclude==0.6.0 ; extra == "docs"
+Requires-Dist: ruff-api>=0.0.5 ; extra == "ruff"
 Project-URL: Changelog, https://ufmt.omnilib.dev/en/latest/changelog.html
 Project-URL: Documentation, https://ufmt.omnilib.dev
 Project-URL: Github, https://github.com/omnilib/ufmt
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ruff
```

