# Comparing `tmp/kaiju_app-0.1.3-py3-none-any.whl.zip` & `tmp/kaiju_app-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18776 bytes, number of entries: 13
--rw-r--r--  2.0 unx      314 b- defN 24-Apr-27 14:25 kaiju_app/__init__.py
--rw-r--r--  2.0 unx    16952 b- defN 24-Apr-27 14:25 kaiju_app/app.py
--rw-r--r--  2.0 unx     1473 b- defN 24-Apr-27 14:25 kaiju_app/bases.py
--rw-r--r--  2.0 unx     4410 b- defN 24-Apr-27 14:25 kaiju_app/configurator.py
--rw-r--r--  2.0 unx      314 b- defN 24-Apr-27 14:25 kaiju_app/interfaces.py
--rw-r--r--  2.0 unx     9992 b- defN 24-Apr-27 14:25 kaiju_app/loader.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 14:25 kaiju_app/py.typed
--rw-r--r--  2.0 unx    14232 b- defN 24-Apr-27 14:25 kaiju_app/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5156 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1007 b- defN 24-Apr-27 14:25 kaiju_app-0.1.3.dist-info/RECORD
-13 files, 55021 bytes uncompressed, 17112 bytes compressed:  68.9%
+Zip file size: 18876 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      314 b- defN 24-May-02 15:12 kaiju_app/__init__.py
+-rw-r--r--  2.0 unx    16909 b- defN 24-May-02 15:12 kaiju_app/app.py
+-rw-r--r--  2.0 unx     1473 b- defN 24-May-02 15:12 kaiju_app/bases.py
+-rw-r--r--  2.0 unx     4545 b- defN 24-May-02 15:12 kaiju_app/configurator.py
+-rw-r--r--  2.0 unx      314 b- defN 24-May-02 15:12 kaiju_app/interfaces.py
+-rw-r--r--  2.0 unx    10494 b- defN 24-May-02 15:12 kaiju_app/loader.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 15:12 kaiju_app/py.typed
+-rw-r--r--  2.0 unx    14232 b- defN 24-May-02 15:12 kaiju_app/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5156 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1008 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/RECORD
+13 files, 55616 bytes uncompressed, 17212 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: kaiju_app/py.typed
 Comment: 
 
 Filename: kaiju_app/utils.py
 Comment: 
 
-Filename: kaiju_app-0.1.3.dist-info/LICENSE
+Filename: kaiju_app-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_app-0.1.3.dist-info/METADATA
+Filename: kaiju_app-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_app-0.1.3.dist-info/WHEEL
+Filename: kaiju_app-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_app-0.1.3.dist-info/top_level.txt
+Filename: kaiju_app-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_app-0.1.3.dist-info/RECORD
+Filename: kaiju_app-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_app/__init__.py

```diff
@@ -4,8 +4,8 @@
 from kaiju_app.bases import *
 from kaiju_app.configurator import *
 from kaiju_app.loader import *
 
 __python_version__ = "3.12"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## kaiju_app/app.py

```diff
@@ -12,14 +12,15 @@
 from kaiju_scheduler import Scheduler, ScheduledTask, Server
 from uvlog import Logger
 
 from kaiju_app.bases import Error
 from kaiju_app.utils import State, timeout, Namespace
 
 __all__ = [
+    "APP_CONTEXT",
     "Application",
     "service",
     "Service",
     "ServiceState",
     "ServiceFieldType",
     "Health",
     "Error",
@@ -29,15 +30,15 @@
     "Scheduler",
     "ScheduledTask",
 ]
 
 _AsyncCallable = Callable[..., Awaitable[Any]]
 _Application = TypeVar("_Application", bound="Application")
 _ServiceClasses = dict[str, type["Service"]]
-_Sentinel = ...
+_SENTINEL = ...
 
 
 APP_CONTEXT: ContextVar[dict | None] = ContextVar("APP_CONTEXT", default=None)
 """Application context variable."""
 
 
 @final
@@ -74,15 +75,15 @@
     def __init__(self, required: bool, nowait: bool, *args):
         """Initialize."""
         super().__init__(*args)
         self.required = required
         self.nowait = nowait
 
 
-def service(*, name=_Sentinel, metadata=None, required: bool = True, nowait: bool = False):
+def service(*, name=_SENTINEL, metadata=None, required: bool = True, nowait: bool = False):
     """Service field describing another service dependency.
 
     :param name: custom service name
     :param required: this dependency is required for the service to work
     :param nowait: do not wait for this service initialization
     :param metadata: additional field metadata, stored in the dataclass field
 
@@ -224,70 +225,65 @@
     Service class name is used by default by the app service manager.
     When you declare more than one service of the same type you MUST explicitly provide unique names for them."""
 
     logger: Logger
     """Logger instance.
     During the app init a logger instance is provided automatically by the app constructor."""
 
-    state: State = field(init=False, default_factory=lambda: State(ServiceState, ServiceState.CLOSED))
-    """Service work state."""
-
     env: str
     """App environment (scope).
     See :py:obj:`~kaiju_base.app.Environment` for a list of standard environments. It's not mandatory but recommended.
     """
 
-    context: ContextVar[dict | None]
+    context: ContextVar[dict | None] = APP_CONTEXT
     """Context var to store a server call context."""
 
     debug: bool = False
     """Run app in debug mode."""
 
     service_start_timeout_s: float = 30.0
     """A timeout (sec) for each service start. An error will be produced if taking more than this interval."""
 
     post_init_timeout_s: float = 300.0
     """A post-init task timeout (sec) for ALL the services combined."""
 
     show_inspection_on_start: bool = False
     """Show inspection data in logs after the app start."""
 
-    max_parallel_tasks: int = 128
-    """Max parallel asyncio tasks submitted to the internal application server simultaneously."""
-
     metadata: dict = field(default_factory=dict)
     """Application metadata not used by it directly."""
 
-    scheduler: Scheduler = field(init=False)
+    optional_services: list[str] = field(default_factory=list)
+    """List of optional services not required for the app start."""
+
+    scheduler: Scheduler = field(default_factory=Scheduler)
     """Internal task scheduler."""
 
-    server: Server = field(init=False)
+    server: Server = field(default_factory=Server)
     """Internal task server."""
 
-    optional_services: list[str] = field(default_factory=list)
-    """List of optional services not required for the app start."""
+    namespace: Namespace = field(init=False)
+    """Application namespace for consistent key names across the app."""
 
-    services: MappingProxyType[str, Service] = field(init=False, default=MappingProxyType({}))
-    """Application services registry."""
+    state: State = field(init=False, default_factory=lambda: State(ServiceState, ServiceState.CLOSED))
+    """Service work state."""
 
-    namespace: Namespace = field(init=False, default=Namespace())
-    """Application namespace for consistent key names across the app."""
+    services: MappingProxyType[str, Service] = field(init=False)
+    """Application services registry."""
 
     _service_loading_order: list[Service] = field(init=False, default_factory=list)
     """List of services in order they must be initialized."""
 
     _service_map: dict[str, Service] = field(init=False, default_factory=dict)
     """Mutable mapping of all application services on their names."""
 
     _post_init_task: asyncio.Future | None = field(init=False, default=None)
 
     def __post_init__(self):
         """Initialize."""
-        self.scheduler = Scheduler(logger=self.logger.get_child("_scheduler"))
-        self.server = Server(logger=self.logger.get_child("_server"), max_parallel_tasks=self.max_parallel_tasks)
         self.services = MappingProxyType(self._service_map)
         self.namespace = Namespace(self.env, self.name)
 
     def add_services(self, *services: Service) -> None:
         """Add new services to the application.
 
         The loading order must be resolved.
@@ -311,35 +307,41 @@
         ctx = self.context.get()
         if ctx is not None and "_vars" in ctx:
             return ctx["_vars"].get(key)
         return None
 
     def json_repr(self) -> dict[str, Any]:
         return {
-            "cls": self.__class__.__name__,
-            "data": {
-                "env": self.env,
-                "debug": self.debug,
-                "metadata": self.metadata,
-                "scheduler": self.scheduler.json_repr(),
-                "services": [
-                    {
-                        "cls": _service.__class__.__name__,
-                        "data": {"name": _service.name, "state": _service.state.get().value, **_service.json_repr()},
-                    }
-                    for _service in self._service_loading_order
-                ],
-            },
+            "env": self.env,
+            "debug": self.debug,
+            "metadata": self.metadata,
+            "scheduler": self.scheduler.json_repr(),
+            "services": [
+                {
+                    "cls": _service.__class__.__name__,
+                    "data": {"name": _service.name, "state": _service.state.get().value, **_service.json_repr()},
+                }
+                for _service in self._service_loading_order
+            ],
+            "tasks": [
+                {
+                    "name": task.get_name(),
+                    "is_done": bool(task.done()),
+                    "is_cancelling": bool(task.cancelling()),
+                    "is_cancelled": bool(task.cancelled()),
+                }
+                for task in asyncio.all_tasks()
+            ],
         }
 
     async def inspect(self, services: list[str] | None = None) -> dict:
         """Inspect the app and get all services data and health."""
         app_data = self.json_repr()
         healthy = True
-        for service_data in app_data["data"]["services"]:
+        for service_data in app_data["services"]:
             service_name = service_data["data"]["name"]
             if services and service_name not in services:
                 continue
             _service = self.services[service_name]
             service_data["health"] = service_health = await _service.get_health()
             healthy = healthy and service_health["healthy"]
         app_data["health"] = Health(healthy=healthy, stats={}, errors=[])
@@ -347,14 +349,16 @@
 
     async def start(self) -> None:
         """Initialize all services and tasks."""
         self.logger.info("starting")
         if self.debug:
             self.logger.warning("running in debug mode")
 
+        await self.server.start()
+
         for n, _service in enumerate(self._service_loading_order):
             try:
                 await asyncio.wait_for(_service.start(), self.service_start_timeout_s)
             except asyncio.TimeoutError:
                 if _service.name not in self.optional_services:
                     await self.stop(n)
                     raise ServiceInitTimeout(
@@ -391,14 +395,15 @@
             *(self._close_service(_service) for _service in reversed(self._service_loading_order[:_idx])),
             return_exceptions=True,
         )
         if self._post_init_task and not self._post_init_task.done():
             with suppress(asyncio.CancelledError):
                 await self._post_init_task
         self._post_init_task = None
+        await self.server.stop()
         self.logger.info("stopped")
 
     async def _post_init_service(self, _service: Service, /) -> None:
         try:
             async with timeout(self.post_init_timeout_s):
                 await _service.post_init()
         except asyncio.TimeoutError:
```

## kaiju_app/configurator.py

```diff
@@ -28,15 +28,15 @@
     This class helps to prepare configuration dict from a list of configuration files.
 
     >>> template  = {'app': {'name': '[_doctest_app_name]', 'env': '[_doctest_app_env]'}}
     >>> env = {'_doctest_app_name': 'app', '_doctest_app_env': 'prod'}
     >>> configurator = Configurator()
     >>> configurator.create_configuration([template], [env])
     {'debug': False, 'packages': [], 'logging': {}, 'app': {'name': 'app', 'env': 'prod', 'loglevel': None, \
-'settings': {}, 'optional_services': [], 'services': []}}
+'settings': {}, 'scheduler': {}, 'server': {}, 'optional_services': [], 'services': []}}
 
     """
 
     def create_configuration(
         self,
         templates: list[dict[str, Any]],
         envs: list[dict[str, Any]],
@@ -110,14 +110,16 @@
             for service_config in services_config
         ]
         app = AppConfig(
             name=app_config["name"],
             env=app_config["env"],
             loglevel=app_config.get("loglevel", None),
             settings=app_config.get("settings", {}),
+            scheduler=app_config.get("scheduler", {}),
+            server=app_config.get("server", {}),
             optional_services=app_config.get("optional_services", []),
             services=services_config,
         )
         return ProjectConfig(
             debug=config_dict.get("debug", False),
             packages=config_dict.get("packages", []),
             logging=config_dict.get("logging", {}),
```

## kaiju_app/loader.py

```diff
@@ -3,14 +3,15 @@
 from contextvars import ContextVar
 from dataclasses import dataclass, field, fields
 from graphlib import CycleError, TopologicalSorter
 from importlib import import_module
 from typing import Mapping, Required, TypedDict, TypeVar
 
 import uvlog
+from kaiju_scheduler import Scheduler, Server
 
 from kaiju_app.app import APP_CONTEXT, Application, Service, ServiceFieldType
 
 __all__ = [
     "ApplicationLoader",
     "DependencyCycleError",
     "DependencyNotFound",
@@ -19,15 +20,15 @@
     "ProjectConfig",
     "AppConfig",
     "ServiceConfig",
 ]
 
 _Application = TypeVar("_Application", bound=Application)
 _Service = TypeVar("_Service", bound=Service)
-_Sentinel = ...
+_SENTINEL = ...
 
 
 class DependencyCycleError(RuntimeError):
     """Dependency cycle has been detected."""
 
 
 class DependencyNotFound(RuntimeError):
@@ -50,14 +51,16 @@
     settings: dict  #: args for service __init__
 
 
 class AppConfig(TypedDict, total=False):
     name: Required[str]  #: application unique name
     env: Required[str]  #: application environment name: prod, test, qa, etc.
     loglevel: uvlog.LevelName | None  #: default log level for the app and app services
+    scheduler: dict  #: app scheduler init settings
+    server: dict  #: app server init settings
     settings: dict  #: args for application __init__
     optional_services: list[str]  #: list of optional services (names)
     services: list[ServiceConfig]  #: list of service settings
 
 
 class ProjectConfig(TypedDict, total=False):
     debug: bool  #: run the project in debug mode
@@ -89,48 +92,55 @@
 
     def create_all(
         self, app_class: type[_Application], config: ProjectConfig, *, context: ContextVar[dict | None] = APP_CONTEXT
     ) -> _Application:
         """Load services from packages and return a new application."""
         self.configure_loggers(config["logging"], context)
         self.load_extensions(config["packages"])
-        return self.create_app(app_class, config["app"], context, config["debug"])
+        app = self.create_app(app_class, config["app"], context, config["debug"])
+        self.init_app_services(app, config["app"]["services"])
+        return app
 
     @staticmethod
     def configure_loggers(config: uvlog.uvlog._DictConfig, context: ContextVar[dict | None], /) -> None:
         uvlog.configure(config, context_var=context)
 
     def load_extensions(self, package_names: list[str], /) -> None:
         """Load services from specified packages."""
         for pkg_name in package_names:
             _module = import_module(f"{pkg_name}.services")
             for name, obj in _module.__dict__.items():
                 if issubclass(obj, Service):
                     self.service_classes[name] = obj
 
+    @staticmethod
     def create_app(
-        self, app_class: type[_Application], config: AppConfig, context: ContextVar[dict | None], debug: bool, /
+        app_class: type[_Application], config: AppConfig, context: ContextVar[dict | None], debug: bool, /
     ) -> _Application:
         app_logger = uvlog.get_logger(config["name"], persistent=True)
         loglevel = config["loglevel"]
         if loglevel is not None:
             app_logger.set_level(loglevel)
         app = app_class(
             env=config["env"],
             name=config["name"],
             context=context,
             debug=debug,
             logger=app_logger,
             optional_services=config["optional_services"],
+            scheduler=Scheduler(**config["scheduler"], logger=app_logger.get_child("_scheduler")),
+            server=Server(**config["server"], logger=app_logger.get_child("_server")),
             **config["settings"],
         )
-        app_services = self._create_app_services(app, config["services"])
+        return app
+
+    def init_app_services(self, app: _Application, config: list[ServiceConfig], /) -> None:
+        app_services = self._create_app_services(app, config)
         service_loading_order = self._get_service_loading_order(app_services)
         app.add_services(*service_loading_order)
-        return app
 
     def _create_app_services(self, app: _Application, config: list[ServiceConfig], /) -> dict[str, Service]:
         app_services = {}
         for service_config in config:
             if not service_config["enabled"]:
                 continue
             if service_config["name"] in app_services and not self.allow_service_name_overrides:
@@ -144,21 +154,21 @@
                 raise ConfigurationError(
                     f'Service class not found: {service_config["cls"]}\n\n'
                     f"Fix: Check if the class is registered in the app loader"
                     f" `service_classes` dict and that all the required kaiju packages are listed"
                     f" in the `packages` section of the config file."
                 ) from None
 
-            new_service = self._create_service(app, self.service_classes[service_config["cls"]], service_config)
+            new_service = self.create_service(app, self.service_classes[service_config["cls"]], service_config)
             app_services[new_service.name] = new_service
 
         return app_services
 
     @staticmethod
-    def _create_service(app: _Application, service_class: type[_Service], config: ServiceConfig, /) -> Service:
+    def create_service(app: _Application, service_class: type[_Service], config: ServiceConfig, /) -> Service:
         service_logger = app.logger.get_child(config["name"], persistent=True)
         loglevel = config["loglevel"]
         if loglevel is not None:
             service_logger.set_level(loglevel)
         try:
             new_service = service_class(app=app, name=config["name"], logger=service_logger, **config["settings"])
         except Exception as exc:
@@ -202,28 +212,28 @@
         self, service_map: Mapping[str, Service], service_: Service, field_: ServiceFieldType, /
     ) -> Service | None:
         """Discover and set a service dependency attribute and return it if exists."""
         name = getattr(service_, field_.name)
         if isinstance(name, Service):
             return name
 
-        if name is _Sentinel:
+        if name is _SENTINEL:
             _service_type = field_.type
             if isinstance(_service_type, str):
                 _service_type = self.service_classes[_service_type]
             dependency = next(
                 (srv for srv in service_map.values() if isinstance(srv, _service_type) and srv is not service_), None
             )
         else:
             dependency = service_map.get(name)
             if not isinstance(dependency, field_.type):
                 dependency = None
         setattr(service_, field_.name, dependency)
         if dependency is None and field_.required:
-            if name is _Sentinel:
+            if name is _SENTINEL:
                 name = "..."
             raise DependencyNotFound(
                 f"Dependency failed for service: {service_.name}\n\n"
                 f"Fix: Check if a service {name} of type {field_.type} is present in the config."
             ) from None
 
         return dependency
```

## Comparing `kaiju_app-0.1.3.dist-info/LICENSE` & `kaiju_app-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_app-0.1.3.dist-info/METADATA` & `kaiju_app-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-app
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python modular application and services
 Home-page: https://github.com/violet-black/kaiju-app
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: application,microservice,asyncio,infrastructure
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `kaiju_app-0.1.3.dist-info/RECORD` & `kaiju_app-0.1.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-kaiju_app/__init__.py,sha256=AmuMOMpnmObDZlW74-YXSkZnPX90toy0sI51qAfiyGA,314
-kaiju_app/app.py,sha256=JCnRR6pOgOwYhU3EUrP7YqpwDZMGriyOY1n9yfKNBHs,16952
+kaiju_app/__init__.py,sha256=rhZoLvFPQf3_TyVqS_MTrKyJiHcn5hfioF7BDeoWjOM,314
+kaiju_app/app.py,sha256=cu86bZifQgi8OjaeTgLYKzBI5DH41youQPKDhLjt7sk,16909
 kaiju_app/bases.py,sha256=5I-Icjqe-2MaNV9GseDE0hOHlJPW4tCZkSTLcR0e26k,1473
-kaiju_app/configurator.py,sha256=YnnN3ru-XDAbhU1BaMAdtIse59TCx0yBEpeRUslK6Lw,4410
+kaiju_app/configurator.py,sha256=4S56zroYvZrk2CP2_aAnt_2b63mdOG2JXLTX1tRe3wI,4545
 kaiju_app/interfaces.py,sha256=Rkz0pDMk_0AUC8MwOSTrq7cbhhCiXQISdpb5CJKIPGw,314
-kaiju_app/loader.py,sha256=zbDOu1QDbacpJgmJ23eo1gzTLz0X6STUCvO0sR3n_9Q,9992
+kaiju_app/loader.py,sha256=n7e7piO86Ym4rp_-wpeu7dfz5lOevF_vPeHnQP82-EQ,10494
 kaiju_app/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_app/utils.py,sha256=kkU_ENfQj2OfPgde193iYK3tOJkfeX-aGmt-sm5Q0TA,14232
-kaiju_app-0.1.3.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-kaiju_app-0.1.3.dist-info/METADATA,sha256=EA7Dezy-xPlCOZAmFuMgXRilpjBhBReAddrckZv2yEE,5156
-kaiju_app-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-kaiju_app-0.1.3.dist-info/top_level.txt,sha256=oaPejx2Wf_jdrr583PfUJWkCx3c4XqOCJGPVrNTQVbg,10
-kaiju_app-0.1.3.dist-info/RECORD,,
+kaiju_app-0.1.4.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+kaiju_app-0.1.4.dist-info/METADATA,sha256=cJ4ci2voiHq34NG_SDWtpPmjg1b62H6yC6CgBtIaIPw,5156
+kaiju_app-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kaiju_app-0.1.4.dist-info/top_level.txt,sha256=oaPejx2Wf_jdrr583PfUJWkCx3c4XqOCJGPVrNTQVbg,10
+kaiju_app-0.1.4.dist-info/RECORD,,
```

