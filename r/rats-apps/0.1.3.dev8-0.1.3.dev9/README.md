# Comparing `tmp/rats_apps-0.1.3.dev8-py3-none-any.whl.zip` & `tmp/rats_apps-0.1.3.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6695 bytes, number of entries: 13
--rw-r--r--  2.0 unx      858 b- defN 80-Jan-01 00:00 rats/apps/__init__.py
--rw-r--r--  2.0 unx     5125 b- defN 80-Jan-01 00:00 rats/apps/_annotations.py
+Zip file size: 7262 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1099 b- defN 80-Jan-01 00:00 rats/apps/__init__.py
+-rw-r--r--  2.0 unx     6993 b- defN 80-Jan-01 00:00 rats/apps/_annotations.py
 -rw-r--r--  2.0 unx      553 b- defN 80-Jan-01 00:00 rats/apps/_composite_container.py
 -rw-r--r--  2.0 unx     3129 b- defN 80-Jan-01 00:00 rats/apps/_container.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 rats/apps/_ids.py
 -rw-r--r--  2.0 unx      188 b- defN 80-Jan-01 00:00 rats/apps/_namespaces.py
 -rw-r--r--  2.0 unx      853 b- defN 80-Jan-01 00:00 rats/apps/_plugin_container.py
--rw-r--r--  2.0 unx     1305 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
+-rw-r--r--  2.0 unx     1453 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/apps/py.typed
--rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev8.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.3.dev8.dist-info/RECORD
-13 files, 14403 bytes uncompressed, 4943 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1046 b- defN 16-Jan-01 00:00 rats_apps-0.1.3.dev9.dist-info/RECORD
+13 files, 16661 bytes uncompressed, 5510 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: rats/apps/_scoping.py
 Comment: 
 
 Filename: rats/apps/py.typed
 Comment: 
 
-Filename: rats_apps-0.1.3.dev8.dist-info/METADATA
+Filename: rats_apps-0.1.3.dev9.dist-info/METADATA
 Comment: 
 
-Filename: rats_apps-0.1.3.dev8.dist-info/WHEEL
+Filename: rats_apps-0.1.3.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: rats_apps-0.1.3.dev8.dist-info/entry_points.txt
+Filename: rats_apps-0.1.3.dev9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_apps-0.1.3.dev8.dist-info/RECORD
+Filename: rats_apps-0.1.3.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rats/apps/__init__.py

```diff
@@ -3,25 +3,29 @@
 
 Applications give you the ability to define a development experience to match your project's
 domain.
 """
 
 from ._annotations import (
     AnnotatedContainer,
+    autoid_service,
     config,
     container,
     fallback_config,
     fallback_group,
     fallback_service,
     group,
+    method_service_id,
     service,
 )
+from ._composite_container import CompositeContainer
 from ._container import Container, DuplicateServiceError, ServiceNotFoundError
 from ._ids import ConfigId, ServiceId
 from ._namespaces import ProviderNamespaces
+from ._plugin_container import PluginContainers
 from ._scoping import autoscope
 
 __all__ = [
     "AnnotatedContainer",
     "ConfigId",
     "Container",
     "DuplicateServiceError",
@@ -32,8 +36,12 @@
     "config",
     "container",
     "fallback_config",
     "fallback_group",
     "fallback_service",
     "group",
     "service",
+    "method_service_id",
+    "autoid_service",
+    "CompositeContainer",
+    "PluginContainers",
 ]
```

## rats/apps/_annotations.py

```diff
@@ -1,17 +1,18 @@
 from collections import defaultdict
 from collections.abc import Callable, Iterator
 from functools import cache
-from typing import Any, cast
+from typing import Any, ParamSpec, cast
 
 from typing_extensions import NamedTuple
 
 from ._container import Container
 from ._ids import ConfigId, ServiceId, T_ConfigType, T_ServiceType
 from ._namespaces import ProviderNamespaces
+from ._scoping import scope_service_name
 
 DEFAULT_CONTAINER_GROUP = ServiceId[Container]("__default__")
 
 
 class GroupAnnotations(NamedTuple):
     """
     The list of service ids attached to a given function.
@@ -53,14 +54,17 @@
 
     def __init__(self) -> None:
         self._service_ids = defaultdict(list)
 
     def add(self, namespace: str, service_id: ServiceId[T_ServiceType]) -> None:
         self._service_ids[namespace].append(service_id)
 
+    def get_service_names(self, namespace: str) -> tuple[str, ...]:
+        return tuple(s.name for s in self._service_ids.get(namespace, []))
+
     def make(self, name: str) -> tuple[GroupAnnotations, ...]:
         return tuple(
             [
                 GroupAnnotations(name=name, namespace=namespace, groups=tuple(services))
                 for namespace, services in self._service_ids.items()
             ]
         )
@@ -80,65 +84,106 @@
             yield getattr(self, annotation.name)()
 
         for container in containers:
             c = getattr(self, container.name)()
             yield from c.get_namespaced_group(namespace, group_id)
 
 
+P = ParamSpec("P")
+
+
 def service(
     service_id: ServiceId[T_ServiceType],
-) -> Callable[..., Callable[..., T_ServiceType]]:
+) -> Callable[[Callable[P, T_ServiceType]], Callable[P, T_ServiceType]]:
     return fn_annotation_decorator(ProviderNamespaces.SERVICES, service_id)
 
 
+def autoid_service(fn: Callable[P, T_ServiceType]) -> Callable[P, T_ServiceType]:
+    _service_id = method_service_id(fn)
+    _add_annotation(ProviderNamespaces.SERVICES, fn, _service_id)
+    cached_fn = cache(fn)
+    return cast(Callable[P, T_ServiceType], cached_fn)
+
+
 def group(
     group_id: ServiceId[T_ServiceType],
-) -> Callable[..., Callable[..., T_ServiceType]]:
+) -> Callable[[Callable[P, T_ServiceType]], Callable[P, T_ServiceType]]:
     return fn_annotation_decorator(ProviderNamespaces.GROUPS, group_id)
 
 
 def config(
     config_id: ConfigId[T_ConfigType],
-) -> Callable[..., Callable[..., T_ConfigType]]:
+) -> Callable[[Callable[P, T_ConfigType]], Callable[P, T_ConfigType]]:
     return fn_annotation_decorator(ProviderNamespaces.SERVICES, config_id)
 
 
 def fallback_service(
     service_id: ServiceId[T_ServiceType],
-) -> Callable[..., Callable[..., T_ServiceType]]:
+) -> Callable[[Callable[P, T_ServiceType]], Callable[P, T_ServiceType]]:
     return fn_annotation_decorator(ProviderNamespaces.FALLBACK_SERVICES, service_id)
 
 
 def fallback_group(
     group_id: ServiceId[T_ServiceType],
-) -> Callable[..., Callable[..., T_ServiceType]]:
+) -> Callable[[Callable[P, T_ServiceType]], Callable[P, T_ServiceType]]:
     return fn_annotation_decorator(ProviderNamespaces.FALLBACK_GROUPS, group_id)
 
 
 def fallback_config(
     config_id: ConfigId[T_ConfigType],
-) -> Callable[..., Callable[..., T_ConfigType]]:
+) -> Callable[[Callable[P, T_ConfigType]], Callable[P, T_ConfigType]]:
     return fn_annotation_decorator(ProviderNamespaces.FALLBACK_SERVICES, config_id)
 
 
 def container(
     group_id: ServiceId[T_ServiceType] = DEFAULT_CONTAINER_GROUP,
-) -> Callable[..., Callable[..., T_ServiceType]]:
+) -> Callable[[Callable[P, T_ServiceType]], Callable[P, T_ServiceType]]:
     return fn_annotation_decorator(ProviderNamespaces.CONTAINERS, group_id)
 
 
+def _get_method_service_id_name(method: Callable[..., Any]) -> str:
+    existing_names = _get_annotations_builder(method).get_service_names(
+        ProviderNamespaces.SERVICES
+    )
+    if existing_names:
+        return existing_names[0]
+    else:
+        module_name = method.__module__
+        class_name, method_name = method.__qualname__.rsplit(".", 1)
+        service_name = scope_service_name(module_name, class_name, method_name)
+        return service_name
+
+
+def method_service_id(method: Callable[..., T_ServiceType]) -> ServiceId[T_ServiceType]:
+    """
+    Get a service id for a method.
+
+    The service id is constructed from the module, class and method name.  It should be identical
+    regardless of whether the method is bound or not, and regardless of the instance it is bound
+    to.
+
+    The service type is the return type of the method.
+    """
+    service_name = _get_method_service_id_name(method)
+    return ServiceId[T_ServiceType](service_name)
+
+
 def fn_annotation_decorator(
     namespace: str,
     service_id: ServiceId[T_ServiceType],
-) -> Callable[..., Callable[..., T_ServiceType]]:
+) -> Callable[[Callable[P, T_ServiceType]], Callable[P, T_ServiceType]]:
     def wrapper(
-        fn: Callable[..., T_ServiceType],
-    ) -> Callable[..., T_ServiceType]:
-        _add_annotation(namespace, fn, service_id)
-        return cache(fn)
+        fn: Callable[P, T_ServiceType],
+    ) -> Callable[P, T_ServiceType]:
+        _service_id = service_id
+        _add_annotation(namespace, fn, _service_id)
+        cached_fn = cache(fn)
+        # The static type of cached_fn should be correct, but it does not maintain the param-spec,
+        # so we need to cast.
+        return cast(Callable[P, T_ServiceType], cached_fn)
 
     return wrapper
 
 
 @cache
 def _extract_class_annotations(cls: Any) -> FunctionAnnotations:
     function_annotations: list[GroupAnnotations] = []
```

## rats/apps/_scoping.py

```diff
@@ -4,40 +4,44 @@
 
 from ._ids import ServiceId
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
+def scope_service_name(module_name: str, cls_name: str, name: str) -> str:
+    return f"{module_name}:{cls_name}[{name}]"
+
+
 def autoscope(cls: type[T]) -> type[T]:
     """
     Decorator that replaces all ServiceId instances in the class with scoped ServiceId instances.
 
     The scoped ServiceId instances have a prefix to eliminate the chance of conflicts across
     packages.
     """
 
     def wrap(func: Callable[..., Any]) -> Callable[..., Any]:
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> ServiceId[Any]:
             result = func(*args, **kwargs)
             if not isinstance(result, ServiceId):
                 return result
 
-            return ServiceId[Any](f"{cls.__module__}:{cls.__name__}[{result.name}]")
+            return ServiceId[Any](scope_service_name(cls.__module__, cls.__name__, result.name))
 
         return cast(FunctionType, wrapper)
 
     props = [prop for prop in dir(cls) if not prop.startswith("_")]
 
     for prop_name in props:
         non_ns = getattr(cls, prop_name)
 
         if isinstance(non_ns, FunctionType):
             setattr(cls, prop_name, wrap(non_ns))
         else:
             if not isinstance(non_ns, ServiceId):
                 continue
 
-            prop = ServiceId[Any](f"{cls.__module__}:{cls.__name__}[{non_ns.name}]")
+            prop = ServiceId[Any](scope_service_name(cls.__module__, cls.__name__, non_ns.name))
             setattr(cls, prop_name, prop)
 
     return cls
```

## Comparing `rats_apps-0.1.3.dev8.dist-info/METADATA` & `rats_apps-0.1.3.dev9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-apps
-Version: 0.1.3.dev8
+Version: 0.1.3.dev9
 Summary: research analysis tools for building applications
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_apps-0.1.3.dev8.dist-info/RECORD` & `rats_apps-0.1.3.dev9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-rats/apps/__init__.py,sha256=JYVss3L2R4uxdOp4Ozfg_cHWgRvCWq79OyVZefFw9wY,858
-rats/apps/_annotations.py,sha256=NGCw1JMZdPMoK_pE61iXgjeI1Xn7P5WXLt7t8zWligg,5125
+rats/apps/__init__.py,sha256=5Mi9YL80YF6Z1Jy2uB_L1oWDG_w0Tl00yViprVuO_LQ,1099
+rats/apps/_annotations.py,sha256=GT2VGkLO2Re0oZsVd6oQlm0WdJj5NSirGA0cpPmmiik,6993
 rats/apps/_composite_container.py,sha256=wSWVQWPin2xxIlEoSgk_D1rlc3N2gpTxQ2y9UFdqXy0,553
 rats/apps/_container.py,sha256=5uiCyxN6HS2z97XcTOFP-t72cNoB1U1sJMkMcfSfDps,3129
 rats/apps/_ids.py,sha256=dxWCPMpMA_vpaTDJEKNByIBJaX97Db203XqWLhaOezo,457
 rats/apps/_namespaces.py,sha256=THUV_Xj5PtweC23Ob-zsSpk8exC4fT-qRwjpQ6IDm0U,188
 rats/apps/_plugin_container.py,sha256=W_xQD2btc0N2dEb3c5tXM-ZZ4A4diMpkCjbOZdlXYuI,853
-rats/apps/_scoping.py,sha256=lRV1DDq-U4mr4WOQhvFjTiCQe2dKY95LNn6b0RXRjFA,1305
+rats/apps/_scoping.py,sha256=plSVEq3rJ8JFAu2epVg2NQpuTbpSTA3a0Tha_DwJL_Y,1453
 rats/apps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_apps-0.1.3.dev8.dist-info/METADATA,sha256=mZp5dVow8ScTYqG5JaKsEPzABPF-b3r55srRYgJJ9y8,716
-rats_apps-0.1.3.dev8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_apps-0.1.3.dev8.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
-rats_apps-0.1.3.dev8.dist-info/RECORD,,
+rats_apps-0.1.3.dev9.dist-info/METADATA,sha256=rWKB-G07Xc5Nm0CIT0W3fyNrXWDPg632uRdkrYF6Z0o,716
+rats_apps-0.1.3.dev9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_apps-0.1.3.dev9.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
+rats_apps-0.1.3.dev9.dist-info/RECORD,,
```

