# Comparing `tmp/ragdaemon-0.4.2.tar.gz` & `tmp/ragdaemon-0.4.3.tar.gz`

## Comparing `ragdaemon-0.4.2.tar` & `ragdaemon-0.4.3.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/app.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/context.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/graph.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/llm.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    14934 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/app.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/context.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/graph.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.3/PKG-INFO
```

### Comparing `ragdaemon-0.4.2/tutorial.ipynb` & `ragdaemon-0.4.3/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/.github/workflows/run-tests.yml` & `ragdaemon-0.4.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/app.py` & `ragdaemon-0.4.3/ragdaemon/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,64 +6,47 @@
 from pathlib import Path
 from typing import Any
 
 import uvicorn
 from fastapi import FastAPI, Request
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
-from spice import Spice
 from starlette.templating import Jinja2Templates
 
 from ragdaemon.daemon import Daemon
-from ragdaemon.database import DEFAULT_EMBEDDING_MODEL
-from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
 
 # Load daemon with command line arguments and visualization annotators
 parser = argparse.ArgumentParser(description="Start the ragdaemon server.")
 parser.add_argument(
     "--refresh", "-r", action="store_true", help="Refresh active records."
 )
 parser.add_argument(
-    "--chunk-extensions",
+    "--code-extensions",
     "-c",
     nargs="*",
-    help="List of file extensions to chunk, e.g., .py .js",
-)
-parser.add_argument(
-    "--chunk-model",
-    default=DEFAULT_COMPLETION_MODEL,
-    help="Spice-compatible LLM  to use for ChunkerLLM.",
-)
-parser.add_argument(
-    "--embeddings-model",
-    default=DEFAULT_EMBEDDING_MODEL,
-    help="Spice-compatible embeddings model to use for Chroma database.",
+    help="List of file extensions to process as code, e.g., .py .js",
 )
 parser.add_argument(
     "--diff",
     "-d",
     default="",
     help="Annotate graph with 'git diff <target>'",
 )
 args = parser.parse_args()
 refresh = args.refresh
 verbose = True  # Always verbose in server mode
-chunk_extensions = None if args.chunk_extensions is None else set(args.chunk_extensions)
+code_extensions = None if args.code_extensions is None else set(args.code_extensions)
 diff = args.diff
 annotators = {
     "hierarchy": {},
-    "chunker_llm": {"chunk_extensions": chunk_extensions},
+    "chunker_llm": {"chunk_extensions": code_extensions},
+    "call_graph": {"call_extensions": code_extensions},
     "diff": {"diff": diff},
     "layout_hierarchy": {},
 }
-chunk_model = args.chunk_model
-embeddings_model = args.embeddings_model
-spice_client = Spice(
-    default_text_model=chunk_model, default_embeddings_model=embeddings_model
-)
 daemon = Daemon(Path.cwd(), annotators=annotators, verbose=verbose)
 
 
 # Start/run daemon in the background
 @asynccontextmanager
 async def lifespan(app: FastAPI):
     if refresh:
```

### Comparing `ragdaemon-0.4.2/ragdaemon/context.py` & `ragdaemon-0.4.3/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/daemon.py` & `ragdaemon-0.4.3/ragdaemon/daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from spice.spice import Model
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
-from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
-from ragdaemon.utils import mentat_dir_path
+from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, mentat_dir_path
 
 
 def default_annotators():
     return {
         "hierarchy": {},
         "chunker_line": {"lines_per_chunk": 30},
         "diff": {},
@@ -66,14 +65,27 @@
         # Initialize an empty graph
         self.graph = KnowledgeGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
             print("Initialized empty graph.")
 
         annotators = annotators if annotators is not None else default_annotators()
+
+        # TODO: Maybe this should be a base annotator method? validate against all
+        if "call_graph" in annotators:
+            try:
+                chunker_type = next(a for a in annotators if "chunker" in a)
+                chunker_cls = annotators_map[chunker_type]
+                chunk_field_id = chunker_cls.chunk_field_id
+                annotators["call_graph"]["chunk_field_id"] = chunk_field_id
+            except StopIteration:
+                raise ValueError(
+                    "Call graph annotator requires a chunker annotator to be specified."
+                )
+
         if self.verbose:
             print(f"Initializing annotators: {list(annotators.keys())}...")
         self.pipeline: dict[str, Annotator] = {
             ann: annotators_map[ann](
                 **kwargs, verbose=self.verbose, spice_client=spice_client
             )
             for ann, kwargs in annotators.items()
```

### Comparing `ragdaemon-0.4.2/ragdaemon/get_paths.py` & `ragdaemon-0.4.3/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/graph.py` & `ragdaemon-0.4.3/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/utils.py` & `ragdaemon-0.4.3/ragdaemon/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,52 @@
+import asyncio
 import hashlib
-import os
 import re
 import subprocess
 from base64 import b64encode
 from pathlib import Path
 
 from spice import Spice
-from spice.models import UnknownModel
+from spice.models import GPT_4_TURBO, UnknownModel
 from spice.spice import get_model_from_name
 
 from ragdaemon.errors import RagdaemonError
 
 mentat_dir_path = Path.home() / ".mentat"
 
 
+semaphore = asyncio.Semaphore(100)
+
+
+DEFAULT_CODE_EXTENSIONS = [
+    ".py",
+    ".js",
+    ".java",
+    ".html",
+    ".css",
+    ".sql",
+    ".php",
+    ".rb",
+    ".sh",
+    ".c",
+    ".cpp",
+    ".h",
+    ".hpp",
+    ".cs",
+    ".go",
+    ".ts",
+    ".jsx",
+    ".tsx",
+    ".scss",
+]
+
+
+DEFAULT_COMPLETION_MODEL = GPT_4_TURBO
+
+
 def hash_str(string: str) -> str:
     """Return the MD5 hash of the input string."""
     return hashlib.md5(string.encode()).hexdigest()
 
 
 def basic_auth(username: str, password: str):
     token = b64encode(f"{username}:{password}".encode("utf-8")).decode("ascii")
```

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.3/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.3/ragdaemon/annotators/chunker.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,45 +22,25 @@
 
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import Database, remove_add_to_db_duplicates
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.graph import KnowledgeGraph
-from ragdaemon.utils import get_document, hash_str, truncate
+from ragdaemon.utils import DEFAULT_CODE_EXTENSIONS, get_document, hash_str, truncate
 
 
 class Chunker(Annotator):
     name = "chunker"
     chunk_field_id = "chunks"
 
     def __init__(self, *args, chunk_extensions: Optional[list[str]] = None, **kwargs):
         super().__init__(*args, **kwargs)
         if chunk_extensions is None:
-            chunk_extensions = [
-                ".py",
-                ".js",
-                ".java",
-                ".html",
-                ".css",
-                ".sql",
-                ".php",
-                ".rb",
-                ".sh",
-                ".c",
-                ".cpp",
-                ".h",
-                ".hpp",
-                ".cs",
-                ".go",
-                ".ts",
-                ".jsx",
-                ".tsx",
-                ".scss",
-            ]
+            chunk_extensions = DEFAULT_CODE_EXTENSIONS
         self.chunk_extensions = chunk_extensions
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         for node, data in graph.nodes(data=True):
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") != "file":
@@ -159,16 +139,16 @@
                 )
                 edges_to_add.add((_parent, _id))
                 if _parent != base_id:
                     _link_to_base_chunk(_parent)
 
             if id != base_id:
                 _link_to_base_chunk(id)
-        for source, origin in edges_to_add:
-            graph.add_edge(source, origin, type="hierarchy")
+        for source, target in edges_to_add:
+            graph.add_edge(source, target, type="hierarchy")
         return add_to_db
 
     async def annotate(
         self, graph: KnowledgeGraph, db: Database, refresh: bool = False
     ) -> KnowledgeGraph:
         # Select file nodes and remove all existing chunk nodes from graph.
         files_with_chunks = []
@@ -176,15 +156,15 @@
         for node, data in all_nodes:
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") == "chunk":
                 graph.remove_node(node)
             elif data.get("type") == "file":
                 if self.chunk_extensions is None:
-                    files_with_chunks.append(node)
+                    files_with_chunks.append((node, data))
                 else:
                     extension = Path(data["ref"]).suffix
                     if extension in self.chunk_extensions:
                         files_with_chunks.append((node, data))
 
         # Generate/add chunk data for nodes that don't have it
         tasks = []
```

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.3/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.3/ragdaemon/annotators/chunker_llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
 import json
 from json.decoder import JSONDecodeError
 from typing import Any, Dict, List, Optional
 
 from spice import SpiceMessages
+from spice.models import TextModel
 
 from ragdaemon.annotators.chunker import Chunker
 from ragdaemon.errors import RagdaemonError
-from ragdaemon.utils import lines_set_to_ref
+from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, lines_set_to_ref, semaphore
 
 
 def is_chunk_valid(chunk: dict, last_valid_line: int):
     if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
         raise RagdaemonError(f"Chunk is missing fields: {chunk}")
     halves = chunk["id"].split(":")
     if len(halves) != 2 or not halves[0] or not halves[1]:
@@ -25,21 +26,27 @@
         raise RagdaemonError(f"Chunk lines are not valid: {chunk}")
     start, end = int(start), int(end)
     if not 1 <= start <= end <= last_valid_line:
         raise RagdaemonError(f"Chunk lines are out of bounds: {chunk}")
     # TODO: Validate the ref, i.e. a parent chunk exists
 
 
-semaphore = asyncio.Semaphore(100)
-
-
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
     chunk_field_id = "chunks_llm"
 
+    def __init__(
+        self,
+        *args,
+        model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.model = model
+
     async def get_llm_response(
         self,
         file: str,
         file_lines: list[str],
         last_chunk: Optional[dict[str, Any]] = None,
     ) -> List[Dict[str, Any]]:
         """Get one chunking response from the LLM model."""
@@ -52,18 +59,18 @@
             messages.add_system_prompt(
                 "chunker_llm.continuation", last_chunk=last_chunk
             )
         messages.add_user_prompt(
             "chunker_llm.user", path=file, code="\n".join(file_lines)
         )
 
-        global semaphore
         async with semaphore:
             response = await self.spice_client.get_response(
                 messages=messages,
+                model=self.model,
                 response_format={"type": "json_object"},
             )
         try:
             chunks = json.loads(response.text)["chunks"]
         except JSONDecodeError:
             raise RagdaemonError(
                 "Failed to parse JSON response. This could mean that the output is too "
```

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.3/ragdaemon/annotators/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,14 @@
                     _, _lines = parse_path_ref(_data["ref"])
                     if lines and _lines and lines.intersection(_lines):
                         edges_to_add.add(edge)
                     _link_to_successors(successor, visited)
 
             _link_to_successors(file_str)
 
-        for source, origin in edges_to_add:
-            graph.add_edge(source, origin, type="diff")
+        for source, target in edges_to_add:
+            graph.add_edge(source, target, type="diff")
         if len(add_to_db["ids"]) > 0:
             add_to_db = remove_add_to_db_duplicates(**add_to_db)
             db.upsert(**add_to_db)
 
         return graph
```

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.3/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.3/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.4.3/ragdaemon/annotators/summarizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 """
 Add a 1-sentence text summary to each file or chunk node
 """
 
 import asyncio
-from typing import Any, Coroutine
+from typing import Any, Optional
 
+from spice import SpiceMessage
+from spice.models import TextModel
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import Database
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
-from spice import SpiceMessage
+from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, semaphore
 
 summarizer_prompt = """\
 Generate a 1-sentence summary of the provided code. Follow conventions of docstrings: 
 write in the imerative voice and start with a verb. Do not include any preamble or 
 asides.
 
 It may be useful to name specific fucntions from the target repository (not built-in
 Python functions) which are integral to the functioning of the target code. Include a
 maximum of two (2) such named functions, but err on the side of brevity.
 """
 
 
-semaphore = asyncio.Semaphore(100)
-
-
 class Summarizer(Annotator):
     name = "summarizer"
 
+    def __init__(
+        self,
+        *args,
+        model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.model = model
+
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         return all(
             data.get("summary") is not None
             for _, data in graph.nodes(data=True)
             if data is not None and data.get("checksum") is not None
         )
 
     async def get_llm_response(self, document: str) -> str:
         if self.spice_client is None:
             raise RagdaemonError("Spice client is not initialized.")
-        global semaphore
+        messages: list[SpiceMessage] = [
+            {"role": "system", "content": summarizer_prompt},
+            {"role": "user", "content": document},
+        ]
         async with semaphore:
-            messages: list[SpiceMessage] = [
-                {"role": "system", "content": summarizer_prompt},
-                {"role": "user", "content": document},
-            ]
             response = await self.spice_client.get_response(
                 messages=messages,
+                model=self.model,
             )
-            return response.text
+        return response.text
 
     async def get_summary(self, data: dict[str, Any], db: Database):
         """Asynchronously generate summary and update graph and db"""
         record = db.get(data["checksum"])
         document = record["documents"][0]
         metadatas = record["metadatas"][0]
         summary = await self.get_llm_response(document)
```

### Comparing `ragdaemon-0.4.2/ragdaemon/database/__init__.py` & `ragdaemon-0.4.3/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.3/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/database/database.py` & `ragdaemon-0.4.3/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.3/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.3/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.3/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.3/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/static/js/main.js` & `ragdaemon-0.4.3/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.3/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.3/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.3/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/ragdaemon/templates/index.html` & `ragdaemon-0.4.3/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/conftest.py` & `ragdaemon-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/test_comments.py` & `ragdaemon-0.4.3/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/test_context.py` & `ragdaemon-0.4.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/test_daemon.py` & `ragdaemon-0.4.3/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/test_get_paths.py` & `ragdaemon-0.4.3/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/test_sample.py` & `ragdaemon-0.4.3/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/annotators/test_chunker.py` & `ragdaemon-0.4.3/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.3/tests/annotators/test_chunker_llm.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,27 +28,14 @@
             "ref": "src/calculator.py:17-18",
         },
         {"id": "src/calculator.py:Calculator.call", "ref": "src/calculator.py:20-28"},
         {"id": "src/calculator.py:main", "ref": "src/calculator.py:30-41"},
     ]
 
 
-"""
-
-{'id': 'src/calculator.py:BASE', 'ref': 'src/calculator.py:1-4,19,29,42-44'}, 
-{'id': 'src/calculator.py:Calculator', 'ref': 'src/calculator.py:5,10,13,16'}, 
-{'id': 'src/calculator.py:Calculator.__init__', 'ref': 'src/calculator.py:6-9'}, 
-{'id': 'src/calculator.py:Calculator.add_numbers', 'ref': 'src/calculator.py:11-12'}, 
-{'id': 'src/calculator.py:Calculator.subtract_numbers', 'ref': 'src/calculator.py:14-15'}, 
-{'id': 'src/calculator.py:Calculator.exp_numbers', 'ref': 'src/calculator.py:17-18'}, 
-{'id': 'src/calculator.py:call', 'ref': 'src/calculator.py:20-28'}, 
-{'id': 'src/calculator.py:main', 'ref': 'src/calculator.py:30-41'}
-"""
-
-
 @pytest.mark.skip(reason="This test requires calling an API")
 @pytest.mark.asyncio
 async def test_chunker_llm_edge_cases(cwd, expected_chunks):
     # NOTE: TO RUN THIS YOU HAVE TO COMMENT_OUT tests/conftest.py/mock_openai_api_key
     daemon = Daemon(cwd, annotators={"hierarchy": {}})
     chunker = ChunkerLLM(spice_client=daemon.spice_client)
```

### Comparing `ragdaemon-0.4.2/tests/annotators/test_diff.py` & `ragdaemon-0.4.3/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.3/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.3/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/annotators/test_summarizer.py` & `ragdaemon-0.4.3/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/data/chunker_graph.json` & `ragdaemon-0.4.3/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/data/context_message.txt` & `ragdaemon-0.4.3/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/data/diff_graph.json` & `ragdaemon-0.4.3/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.3/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.3/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.3/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/tests/sample/src/interface.py` & `ragdaemon-0.4.3/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/LICENSE` & `ragdaemon-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/README.md` & `ragdaemon-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.2/pyproject.toml` & `ragdaemon-0.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.2"
+version = "0.4.3"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
-    "spiceai~=0.2.0",
+    "spiceai~=0.3.0",
     "starlette==0.36.3",
     "tqdm==4.66.2",
     "uvicorn==0.29.0",
 ]
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ragdaemon-0.4.2/PKG-INFO` & `ragdaemon-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.2
+Version: 0.4.3
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: dict2xml==1.7.5
 Requires-Dist: fastapi==0.109.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: networkx==3.2.1
-Requires-Dist: spiceai~=0.2.0
+Requires-Dist: spiceai~=0.3.0
 Requires-Dist: starlette==0.36.3
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: uvicorn==0.29.0
 Provides-Extra: dev
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
```

