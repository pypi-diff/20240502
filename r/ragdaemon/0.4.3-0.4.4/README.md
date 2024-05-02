# Comparing `tmp/ragdaemon-0.4.3.tar.gz` & `tmp/ragdaemon-0.4.4.tar.gz`

## Comparing `ragdaemon-0.4.3.tar` & `ragdaemon-0.4.4.tar`

### file list

```diff
@@ -1,69 +1,68 @@
--rw-r--r--   0        0        0    14934 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/app.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/context.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/graph.py
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/app.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/context.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/graph.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/PKG-INFO
```

### Comparing `ragdaemon-0.4.3/tutorial.ipynb` & `ragdaemon-0.4.4/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/.github/workflows/run-tests.yml` & `ragdaemon-0.4.4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/app.py` & `ragdaemon-0.4.4/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/context.py` & `ragdaemon-0.4.4/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/daemon.py` & `ragdaemon-0.4.4/ragdaemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.verbose = verbose
         if graph_path is not None:
             self.graph_path = (cwd / graph_path).resolve()
         else:
             self.graph_path = (
                 mentat_dir_path / "ragdaemon" / f"ragdaemon-{self.cwd.name}.json"
             )
-        self.graph_path.parent.mkdir(exist_ok=True)
+        self.graph_path.parent.mkdir(parents=True, exist_ok=True)
         if spice_client is None:
             logging_dir = mentat_dir_path / "ragdaemon" / "spice_logs"
             logging_dir.mkdir(parents=True, exist_ok=True)
             spice_client = Spice(
                 default_text_model=DEFAULT_COMPLETION_MODEL,
                 default_embeddings_model=model,
                 logging_dir=mentat_dir_path / "ragdaemon" / "spice_logs",
```

### Comparing `ragdaemon-0.4.3/ragdaemon/get_paths.py` & `ragdaemon-0.4.4/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/graph.py` & `ragdaemon-0.4.4/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/utils.py` & `ragdaemon-0.4.4/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/__init__.py` & `ragdaemon-0.4.4/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.4/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.4.4/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.4/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.4/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.4/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.4/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.4/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.4/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.4.4/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/database/__init__.py` & `ragdaemon-0.4.4/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.4/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/database/database.py` & `ragdaemon-0.4.4/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.4/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.4.4/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.4/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.4/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.4/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/static/js/main.js` & `ragdaemon-0.4.4/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.4/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.4/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.4/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/ragdaemon/templates/index.html` & `ragdaemon-0.4.4/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/conftest.py` & `ragdaemon-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/test_comments.py` & `ragdaemon-0.4.4/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/test_context.py` & `ragdaemon-0.4.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/test_daemon.py` & `ragdaemon-0.4.4/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/test_get_paths.py` & `ragdaemon-0.4.4/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/test_sample.py` & `ragdaemon-0.4.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/annotators/test_chunker.py` & `ragdaemon-0.4.4/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.4/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/annotators/test_diff.py` & `ragdaemon-0.4.4/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.4/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.4/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/annotators/test_summarizer.py` & `ragdaemon-0.4.4/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/data/chunker_graph.json` & `ragdaemon-0.4.4/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/data/context_message.txt` & `ragdaemon-0.4.4/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/data/diff_graph.json` & `ragdaemon-0.4.4/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.4/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.4/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.4/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/tests/sample/src/interface.py` & `ragdaemon-0.4.4/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/LICENSE` & `ragdaemon-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/README.md` & `ragdaemon-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.3/pyproject.toml` & `ragdaemon-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.3"
+version = "0.4.4"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.4.3/PKG-INFO` & `ragdaemon-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.3
+Version: 0.4.4
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

