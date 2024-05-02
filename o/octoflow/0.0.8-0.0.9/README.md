# Comparing `tmp/octoflow-0.0.8.tar.gz` & `tmp/octoflow-0.0.9.tar.gz`

## Comparing `octoflow-0.0.8.tar` & `octoflow-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/logging.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/__init__.py
--rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/base.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/client.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/experiment.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/package.py
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/run.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/value.py
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/value_utils.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/variable.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/artifact/__init__.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/core/artifact/handler.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/json_.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/pandas_.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/pickle_.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/safetensors_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/torch_.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/plugins/artifacts/transformers_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/utils/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 octoflow-0.0.8/octoflow/utils/mutation.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 octoflow-0.0.8/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.0.8/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.0.8/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.0.8/README.md
--rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 octoflow-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 octoflow-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/__init__.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/logging.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/__init__.py
+-rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/base.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/client.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/experiment.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/package.py
+-rw-r--r--   0        0        0    12973 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/run.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/value.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/value_utils.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/variable.py
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/artifact/__init__.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/artifact/handler.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/json_.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/pandas_.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/pickle_.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/safetensors_.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/torch_.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/transformers_.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/utils/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/utils/mutation.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 octoflow-0.0.9/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.0.9/AUTHORS.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.0.9/README.md
+-rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 octoflow-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 octoflow-0.0.9/PKG-INFO
```

### Comparing `octoflow-0.0.8/octoflow/logging.py` & `octoflow-0.0.9/octoflow/logging.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/base.py` & `octoflow-0.0.9/octoflow/core/base.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/client.py` & `octoflow-0.0.9/octoflow/core/client.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/experiment.py` & `octoflow-0.0.9/octoflow/core/experiment.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/package.py` & `octoflow-0.0.9/octoflow/core/package.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/run.py` & `octoflow-0.0.9/octoflow/core/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     DateTime,
     ForeignKey,
     Integer,
     String,
     Text,
 )
 from sqlalchemy.orm import Mapped, aliased, mapped_column
-from sqlalchemy.orm.exc import MultipleResultsFound
+from sqlalchemy.orm.exc import MultipleResultsFound, NoResultFound
 
 from octoflow.core import artifact, value_utils
 from octoflow.core.artifact import Artifact
 from octoflow.core.base import Base
 from octoflow.core.value import Value, ValueType
 from octoflow.core.variable import Variable, VariableType
 
 __all__ = [
     "Run",
 ]
 
+NOT_SPECIFIED = object()
+
 
 def generate_uuid() -> str:
     return str(uuid.uuid4())
 
 
 class Run(Base):
     """Run model."""
@@ -151,14 +153,63 @@
         return self._log_values(
             values=values,
             step=step,
             type=VariableType.parameter,
             prefix=prefix,
         )
 
+    def get_param(
+        self,
+        key: str,
+        default: Optional[ValueType] = NOT_SPECIFIED,
+        *,
+        step: Optional[Value] = NOT_SPECIFIED,
+    ) -> ValueType:
+        """Get a parameter.
+
+        Parameters
+        ----------
+        key : str
+            Parameter key.
+        default : Optional[ValueType], optional
+            Default value, by default NOT_SPECIFIED.
+        step : Optional[Value], optional
+            Step value, by default NOT_SPECIFIED.
+
+        Returns
+        -------
+        Value
+            Value instance.
+        """
+        with self.session() as session:
+            q = (
+                session.query(Value)
+                .join(Variable)
+                .filter(
+                    Value.run_id == self.id,
+                    Variable.key == key,
+                    Variable.type == VariableType.parameter,
+                )
+            )
+            if step is None:
+                q = q.filter(Value.step_id.is_(None))
+            if step is not NOT_SPECIFIED:
+                q = q.filter(Value.step_id == step.id)
+            try:
+                value = q.one().value
+            except NoResultFound as e:
+                if default is NOT_SPECIFIED:
+                    msg = f"parameter with key '{key}' does not exist"
+                    raise ValueError(msg) from e
+                value = default
+            except MultipleResultsFound as e:
+                msg = f"multiple parameters with key '{key}' exist"
+                raise ValueError(msg) from e
+        return value
+
     def log_metric(
         self,
         key: str,
         value: ValueType,
         step: Optional[Value] = None,
     ) -> Value:
         """Log a metric.
```

### Comparing `octoflow-0.0.8/octoflow/core/value.py` & `octoflow-0.0.9/octoflow/core/value.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/value_utils.py` & `octoflow-0.0.9/octoflow/core/value_utils.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/variable.py` & `octoflow-0.0.9/octoflow/core/variable.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/artifact/__init__.py` & `octoflow-0.0.9/octoflow/core/artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/core/artifact/handler.py` & `octoflow-0.0.9/octoflow/core/artifact/handler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/plugins/artifacts/__init__.py` & `octoflow-0.0.9/octoflow/plugins/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/plugins/artifacts/json_.py` & `octoflow-0.0.9/octoflow/plugins/artifacts/json_.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/plugins/artifacts/pandas_.py` & `octoflow-0.0.9/octoflow/plugins/artifacts/pandas_.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/plugins/artifacts/pickle_.py` & `octoflow-0.0.9/octoflow/plugins/artifacts/pickle_.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/plugins/artifacts/safetensors_.py` & `octoflow-0.0.9/octoflow/plugins/artifacts/safetensors_.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/plugins/artifacts/transformers_.py` & `octoflow-0.0.9/octoflow/plugins/artifacts/transformers_.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/octoflow/utils/mutation.py` & `octoflow-0.0.9/octoflow/utils/mutation.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/.gitignore` & `octoflow-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/LICENSE` & `octoflow-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/README.md` & `octoflow-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/pyproject.toml` & `octoflow-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.8/PKG-INFO` & `octoflow-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlining machine learning tracking for seamless experiment management.
 Project-URL: Documentation, https://github.com/ysenarath/octoflow
 Project-URL: Source, https://github.com/ysenarath/octoflow
 Author-email: Yasas Senarath <email@example.com>
 License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE
```

