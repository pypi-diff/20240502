# Comparing `tmp/sema4ai_actions-0.3.1.tar.gz` & `tmp/sema4ai_actions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.3.1.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.4.0.tar", max compression
```

## Comparing `sema4ai_actions-0.3.1.tar` & `sema4ai_actions-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     2971 2024-04-23 11:43:04.195086 sema4ai_actions-0.3.1/README.md
--rw-r--r--   0        0        0      971 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4975 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    11619 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7567 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11151 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8376 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    31250 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      336 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2141 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      252 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    11986 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     4355 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     4478 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_secret.py
--rw-r--r--   0        0        0     2277 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/README.md
+-rw-r--r--   0        0        0      971 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5474 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    11619 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11151 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8376 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    31250 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      336 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      252 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    11986 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     4355 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     4478 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_secret.py
+-rw-r--r--   0        0        0     3134 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/api.py
+-rw-r--r--   0        0        0     2277 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.4.0/PKG-INFO
```

### Comparing `sema4ai_actions-0.3.1/README.md` & `sema4ai_actions-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/pyproject.toml` & `sema4ai_actions-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.3.1"
+version = "0.4.0"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,25 +36,27 @@
 from typing import Callable, Optional, overload
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 from ._secret import Secret
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
 
 
 @overload
-def action(*, is_consequential: Optional[bool] = None) -> Callable:
+def action(
+    *, is_consequential: Optional[bool] = None, display_name: Optional[str] = None
+) -> Callable:
     ...
 
 
 def action(*args, **kwargs):
     """
     Decorator for actions (entry points) which can be executed by `sema4ai.actions`.
 
@@ -75,34 +77,45 @@
     python -m sema4ai.actions run actions.py -a enter_user
 
     Args:
         func: A function which is an action to `sema4ai.actions`.
         is_consequential: Whether the action is consequential or not.
             This will add `x-openai-isConsequential: true` to the action
             metadata and shown in OpenApi spec.
+        display_name: A name to be displayed for this action.
+            If given will be used as the openapi.json summary for this action.
     """
 
     def decorator(func, **kwargs):
         from sema4ai.actions import _hooks
 
         is_consequential = kwargs.pop("is_consequential", None)
         if is_consequential is not None:
             if not isinstance(is_consequential, bool):
                 raise ValueError(
                     "Expected 'is_consequential' argument to be a boolean."
                 )
 
+        display_name = kwargs.pop("display_name", None)
+        if display_name is not None:
+            if not isinstance(display_name, str):
+                raise ValueError("Expected 'display_name' argument to be a str.")
+
         if kwargs:
             raise ValueError(
                 f"Arguments accepted by @action: ['is_consequential']. Received arguments: {list(kwargs.keys())}"
             )
 
         # When an action is found, register it in the framework as a target for execution.
         _hooks.on_action_func_found(
-            func, options={"is_consequential": is_consequential}
+            func,
+            options={
+                "is_consequential": is_consequential,
+                "display_name": display_name,
+            },
         )
 
         return func
 
     if args and callable(args[0]):
         return decorator(args[0], **kwargs)
```

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_action_context.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_collect_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_commands.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/_secret.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.4.0/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.1/PKG-INFO` & `sema4ai_actions-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.3.1
+Version: 0.4.0
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

