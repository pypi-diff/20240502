# Comparing `tmp/quasarpy-0.1.6.tar.gz` & `tmp/quasarpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.1.6.tar", max compression
+gzip compressed data, was "quasarpy-0.1.7.tar", max compression
```

## Comparing `quasarpy-0.1.6.tar` & `quasarpy-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    31941 2024-04-28 20:01:21.586745 quasarpy-0.1.6/LICENSE
--rw-r--r--   0        0        0      700 2024-04-28 20:01:21.586745 quasarpy-0.1.6/README.md
--rw-r--r--   0        0        0  1387623 2024-04-28 20:01:21.586745 quasarpy-0.1.6/assets/logo_complete.png
--rw-r--r--   0        0        0   127970 2024-04-28 20:01:21.586745 quasarpy-0.1.6/assets/logo_complete_svg.svg
--rw-r--r--   0        0        0   182267 2024-04-28 20:01:21.590745 quasarpy-0.1.6/assets/logo_complete_tbg.png
--rw-r--r--   0        0        0   418415 2024-04-28 20:01:21.590745 quasarpy-0.1.6/assets/logo_icon.png
--rw-r--r--   0        0        0   166944 2024-04-28 20:01:21.590745 quasarpy-0.1.6/assets/logo_text.png
--rw-r--r--   0        0        0     1062 2024-04-28 20:01:21.594745 quasarpy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      698 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/__main__.py
--rw-r--r--   0        0        0       21 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2748 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4172 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2586 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4496 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-04-28 20:01:21.594745 quasarpy-0.1.6/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 quasarpy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-05-02 03:39:56.441356 quasarpy-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1843 2024-05-02 03:39:56.441356 quasarpy-0.1.7/README.md
+-rw-r--r--   0        0        0  1387623 2024-05-02 03:39:56.441356 quasarpy-0.1.7/assets/logo_complete.png
+-rw-r--r--   0        0        0   127970 2024-05-02 03:39:56.441356 quasarpy-0.1.7/assets/logo_complete_svg.svg
+-rw-r--r--   0        0        0   182267 2024-05-02 03:39:56.445356 quasarpy-0.1.7/assets/logo_complete_tbg.png
+-rw-r--r--   0        0        0   418415 2024-05-02 03:39:56.445356 quasarpy-0.1.7/assets/logo_icon.png
+-rw-r--r--   0        0        0   166944 2024-05-02 03:39:56.445356 quasarpy-0.1.7/assets/logo_text.png
+-rw-r--r--   0        0        0     1170 2024-05-02 03:39:56.449356 quasarpy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      673 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/__main__.py
+-rw-r--r--   0        0        0       21 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2857 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4172 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2586 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4524 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 quasarpy-0.1.7/PKG-INFO
```

### Comparing `quasarpy-0.1.6/LICENSE` & `quasarpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/assets/logo_complete.png` & `quasarpy-0.1.7/assets/logo_complete.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/assets/logo_complete_svg.svg` & `quasarpy-0.1.7/assets/logo_complete_svg.svg`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/assets/logo_complete_tbg.png` & `quasarpy-0.1.7/assets/logo_complete_tbg.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/assets/logo_icon.png` & `quasarpy-0.1.7/assets/logo_icon.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/assets/logo_text.png` & `quasarpy-0.1.7/assets/logo_text.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/pyproject.toml` & `quasarpy-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.1.6"
+version = "0.1.7"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 include = ["assets", 'LICENSE']
 
 [tool.poetry.scripts]
 quasar = "quasarpy:main"
 
+[tool.poetry-dynamic-versioning]
+enable = true
+
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "^7.2.6"
 click = "^8.1.7"
 pytest = "^8.0.0"
 python-dotenv = "^1.0.1"
 radon = "^6.0.1"
@@ -34,16 +37,16 @@
 twine = "^5.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.3"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 extend-include = ["*.ipynb", "__init__.py"]
 
 [radon]
 exclude = "tests/*"
```

### Comparing `quasarpy-0.1.6/quasarpy/__init__.py` & `quasarpy-0.1.7/quasarpy/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 '''This module contains the main() function, which is the entry point for the
 command line interface.'''
 from dotenv import load_dotenv
 from quasarpy.cli import cli
 from quasarpy.utils import logger
-from quasarpy._version import __version__ as _version
+from quasarpy._version import __version___ as _version
 
-__version__ = _version
 
 load_dotenv()  # Load environment variables from .env file
 
 
 def main():
     '''Entry point for the command line interface.'''
     logger.info(f"Quasar {_version} started")
     try: 
         cli()
     except NotImplementedError as e:
         logger.error(e)
     except ValueError as e:
         logger.error(e)
     finally:
-        logger.info(f"Quasar {__version__} stopped")
+        logger.info(f"Quasar {_version} stopped")
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `quasarpy-0.1.6/quasarpy/algorithm/detector.py` & `quasarpy-0.1.7/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/algorithm/llm.py` & `quasarpy-0.1.7/quasarpy/algorithm/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
     def _generate_online(self, prompt: str, **kwargs) -> str:
         try:
             try:
                 token = os.getenv("HUGGINGFACE_TOKEN")
             except KeyError:
                 self.logger.error("Hugging Face API token not found in the environment variables.")
+                with open(".env", "w") as f:
+                    f.write("HUGGINGFACE_TOKEN=YOUR_API_TOKEN")
                 raise
 
             client = huggingface_hub.InferenceClient(token=token)
             response = client.text_generation(
                 prompt=prompt,
                 model="mistralai/Mistral-7B-Instruct-v0.2",
                 max_new_tokens=self.model_config.max_new_tokens,
```

### Comparing `quasarpy-0.1.6/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.1.7/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.1.7/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/cli/__init__.py` & `quasarpy-0.1.7/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/handler/issue.py` & `quasarpy-0.1.7/quasarpy/handler/issue.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/tests/test_handler.py` & `quasarpy-0.1.7/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/tests/test_utils.py` & `quasarpy-0.1.7/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/utils/analyser.py` & `quasarpy-0.1.7/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/utils/ascii.py` & `quasarpy-0.1.7/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/utils/prompt_template.py` & `quasarpy-0.1.7/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.6/quasarpy/utils/redis_server.py` & `quasarpy-0.1.7/quasarpy/utils/redis_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,17 @@
         Union[Dict[str, Any], AnyStr]: The generated report. The return type can be either a dictionary or a string,
         depending on the specified format.
 
     """
 
     logger.info("Generating report")
 
-    env = Environment(loader=FileSystemLoader("quasarpy/utils/templates"))
+
+    env = Environment(loader=FileSystemLoader(os.path.join(os.path.dirname(__file__), "templates")))
+
     template = env.get_template("report_template.html")
     report_path_html = f"{report_path}.html"
 
     html = template.render(time_now=datetime.datetime.now(), files=data)
     with open(report_path_html, "w") as f:
         f.write(html)
```

### Comparing `quasarpy-0.1.6/quasarpy/utils/templates/report_template.html` & `quasarpy-0.1.7/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

