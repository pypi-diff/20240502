# Comparing `tmp/lacuscore-1.9.2.tar.gz` & `tmp/lacuscore-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.9.2.tar", max compression
+gzip compressed data, was "lacuscore-1.9.3.tar", max compression
```

## Comparing `lacuscore-1.9.2.tar` & `lacuscore-1.9.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1516 2024-04-19 10:50:12.818198 lacuscore-1.9.2/LICENSE
--rw-r--r--   0        0        0      941 2024-04-19 10:50:12.818198 lacuscore-1.9.2/README.md
--rw-r--r--   0        0        0      321 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/__init__.py
--rw-r--r--   0        0        0     2775 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    44432 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/py.typed
--rw-r--r--   0        0        0     1873 2024-04-19 10:50:12.822198 lacuscore-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 lacuscore-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-05-02 15:14:18.541012 lacuscore-1.9.3/LICENSE
+-rw-r--r--   0        0        0      941 2024-05-02 15:14:18.541012 lacuscore-1.9.3/README.md
+-rw-r--r--   0        0        0      341 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/__init__.py
+-rw-r--r--   0        0        0     2711 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/helpers.py
+-rw-r--r--   0        0        0     2775 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    42305 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/py.typed
+-rw-r--r--   0        0        0     1916 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/task_logger.py
+-rw-r--r--   0        0        0     1874 2024-05-02 15:14:18.541012 lacuscore-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 lacuscore-1.9.3/PKG-INFO
```

### Comparing `lacuscore-1.9.2/LICENSE` & `lacuscore-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.2/README.md` & `lacuscore-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.2/lacuscore/lacus_monitoring.py` & `lacuscore-1.9.3/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.2/lacuscore/lacuscore.py` & `lacuscore-1.9.3/lacuscore/lacuscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,37 @@
 import time
 import unicodedata
 import zlib
 
 from asyncio import Task
 from base64 import b64decode, b64encode
 from datetime import date, timedelta
-from enum import IntEnum, unique
 from ipaddress import ip_address, IPv4Address, IPv6Address
-from logging import LoggerAdapter
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Literal, Any, TypedDict, overload, cast, MutableMapping, Iterator
+from typing import Literal, Any, overload, cast, Iterator
 from uuid import uuid4
 from urllib.parse import urlsplit
 
 from dns import resolver
 from dns.exception import DNSException
 from dns.exception import Timeout as DNSTimeout
 
 from defang import refang  # type: ignore[import-untyped]
 from playwrightcapture import Capture, PlaywrightCaptureException
-from playwrightcapture.capture import CaptureResponse as PlaywrightCaptureResponse
 from redis import Redis
 from redis.exceptions import ConnectionError as RedisConnectionError
 from redis.exceptions import DataError
 from ua_parser import user_agent_parser  # type: ignore[import-untyped]
 
+from . import task_logger
+from .helpers import (
+    LacusCoreLogAdapter, CaptureError, RetryCapture, CaptureSettingsError,
+    CaptureStatus, CaptureResponse, CaptureResponseJson, CaptureSettings)
+
 if sys.version_info < (3, 11):
     from async_timeout import timeout
 else:
     from asyncio import timeout
 
 BROWSER = Literal['chromium', 'firefox', 'webkit']
 
@@ -61,103 +63,14 @@
     filename = str(_filename_ascii_strip_re.sub("", "_".join(filename.split()))).strip(
         "._"
     )
 
     return filename
 
 
-class LacusCoreException(Exception):
-    pass
-
-
-class CaptureError(LacusCoreException):
-    pass
-
-
-class RetryCapture(LacusCoreException):
-    pass
-
-
-@unique
-class CaptureStatus(IntEnum):
-    '''The status of the capture'''
-    UNKNOWN = -1
-    QUEUED = 0
-    DONE = 1
-    ONGOING = 2
-
-
-class CaptureResponse(PlaywrightCaptureResponse, TypedDict, total=False):
-    '''A capture made by Lacus. With the base64 encoded image and downloaded file decoded to bytes.'''
-
-    # Need to make sure the type is what's expected down the line
-    children: list[CaptureResponse] | None  # type: ignore[misc]
-
-    status: int
-    runtime: float | None
-
-
-class CaptureResponseJson(TypedDict, total=False):
-    '''A capture made by Lacus. With the base64 encoded image and downloaded file *not* decoded.'''
-
-    status: int
-    last_redirected_url: str | None
-    har: dict[str, Any] | None
-    cookies: list[dict[str, str]] | None
-    error: str | None
-    html: str | None
-    png: str | None
-    downloaded_filename: str | None
-    downloaded_file: str | None
-    children: list[CaptureResponseJson] | None
-    runtime: float | None
-    potential_favicons: list[str] | None
-
-
-class CaptureSettings(TypedDict, total=False):
-    '''The capture settings that can be passed to Lacus.'''
-
-    url: str | None
-    document_name: str | None
-    document: str | None
-    browser: str | None
-    device_name: str | None
-    user_agent: str | None
-    proxy: str | dict[str, str] | None
-    general_timeout_in_sec: int | None
-    cookies: list[dict[str, Any]] | None
-    headers: str | dict[str, str] | None
-    http_credentials: dict[str, str] | None
-    geolocation: dict[str, float] | None
-    timezone_id: str | None
-    locale: str | None
-    color_scheme: str | None
-    viewport: dict[str, int] | None
-    referer: str | None
-    with_favicon: bool
-    allow_tracking: bool
-    force: bool
-    recapture_interval: int
-    priority: int
-    uuid: str | None
-
-    depth: int
-    rendered_hostname_only: bool  # Note: only used if depth is > 0
-
-
-class LacusCoreLogAdapter(LoggerAdapter):  # type: ignore[type-arg]
-    """
-    Prepend log entry with the UUID of the capture
-    """
-    def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> tuple[str, MutableMapping[str, Any]]:
-        if self.extra:
-            return '[{}] {}'.format(self.extra['uuid'], msg), kwargs
-        return msg, kwargs
-
-
 class LacusCore():
     """Capture URLs or web enabled documents using PlaywrightCapture.
 
     :param redis_connector: Pre-configured connector to a redis instance.
     :param max_capture time: If the capture takes more than that time, break (in seconds)
     :param tor_proxy: URL to a SOCKS 5 tor proxy. If you have tor installed, this is the default: socks5://127.0.0.1:9050.
     :param only_global_lookups: Discard captures that point to non-public IPs.
@@ -364,15 +277,15 @@
         p.set(f'lacus:query_hash:{hash_query}', perma_uuid, nx=True, ex=recapture_interval)
         p.hset(f'lacus:capture_settings:{perma_uuid}', mapping=mapping_capture)  # type: ignore[arg-type]
         p.zadd('lacus:to_capture', {perma_uuid: priority if priority is not None else 0})
         try:
             p.execute()
         except DataError:
             self.master_logger.exception(f'Unable to enqueue: {to_enqueue}')
-            raise LacusCoreException(f'Unable to enqueue: {to_enqueue}')
+            raise CaptureSettingsError(f'Unable to enqueue: {to_enqueue}')
         return perma_uuid
 
     def _encode_response(self, capture: CaptureResponse) -> CaptureResponseJson:
         encoded_capture = cast(CaptureResponseJson, capture)
         if capture.get('png') is not None and capture['png'] is not None:  # the second part is not needed, but makes mypy happy
             encoded_capture['png'] = b64encode(capture['png']).decode()
         if capture.get('downloaded_file') is not None and capture['downloaded_file'] is not None:  # the second part is not needed, but makes mypy happy
@@ -449,15 +362,18 @@
                 # Nothing to capture
                 break
             if not value[0]:
                 continue
             max_consume -= 1
             uuid: str = value[0][0].decode()
             priority: int = int(value[0][1])
-            yield asyncio.create_task(self._capture(uuid, priority), name=uuid)
+            logger = LacusCoreLogAdapter(self.master_logger, {'uuid': uuid})
+            yield task_logger.create_task(self._capture(uuid, priority), name=uuid,
+                                          logger=logger,
+                                          message='Capture raised an uncaught exception')
 
     async def _capture(self, uuid: str, priority: int) -> None:
         """Trigger a specific capture
 
         :param uuid: The UUID if the capture (given by enqueue)
         :param priority: Only for internal use, will decide on the priority of the capture if the try now fails.
         """
@@ -504,30 +420,30 @@
                         to_capture[k] = int(v)  # type: ignore[literal-required]
                     elif k in ['rendered_hostname_only', 'with_favicon', 'allow_tracking']:
                         # bool
                         to_capture[k] = bool(int(v))  # type: ignore[literal-required]
                     elif k == 'document':
                         document_as_bytes = b64decode(v)
                     else:
-                        raise LacusCoreException(f'Unexpected setting: {k}: {v}')
-            except LacusCoreException as e:
+                        raise CaptureSettingsError(f'Unexpected setting: {k}: {v}')
+            except CaptureSettingsError as e:
                 raise e
             except Exception as e:
-                raise LacusCoreException(f'Error while preparing settings: {e}')
+                raise CaptureSettingsError(f'Error while preparing settings: {e}')
 
             if not to_capture:
                 all_entries = self.redis.hgetall(f'lacus:capture_settings:{uuid}')
                 result = {'error': f'No capture settings for {uuid} - {all_entries}'}
                 raise CaptureError(f'No capture settings for {uuid} - {all_entries}')
 
             if document_as_bytes:
                 # we do not have a URL yet.
                 name = to_capture.pop('document_name', None)
                 if not name:
-                    raise LacusCoreException('No document name provided, settings are invalid')
+                    raise CaptureSettingsError('No document name provided, settings are invalid')
                 if not Path(name).suffix:
                     # The browser will simply display the file as text if there is no extension.
                     # Just add HTML as a fallback, as it will be the most comon one.
                     name = f'{name}.html'
                 document_name = Path(name).name
                 tmp_f = NamedTemporaryFile(suffix=document_name, delete=False)
                 with open(tmp_f.name, "wb") as f:
@@ -684,15 +600,15 @@
                 retry = True
                 self.redis.setex(f'lacus:capture_retry:{uuid}',
                                  self.max_capture_time * (self.max_retries + 1),
                                  self.max_retries)
             else:
                 current_retry = int(_current_retry.decode())
                 if current_retry > 0:
-                    logger.debug(f'Retrying {url} for the {self.max_retries-current_retry+1}th time.')
+                    logger.debug(f'Retrying {url} for the {self.max_retries - current_retry + 1}th time.')
                     self.redis.decr(f'lacus:capture_retry:{uuid}')
                     retry = True
                 else:
                     error_msg = result['error'] if result.get('error') else 'Unknown error'
                     logger.info(f'Retried too many times {url}: {error_msg}')
                     stats_pipeline.sadd(f'stats:{today}:retry_failed', url)
         except CaptureError:
```

### Comparing `lacuscore-1.9.2/pyproject.toml` & `lacuscore-1.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.9.2"
+version = "1.9.3"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -30,32 +30,32 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = [
    {version = "<7.2", python = "<3.9", optional = true},
    {version = "^7.2", python = ">=3.9", optional = true}
 ]
-playwrightcapture = {extras = ["recaptcha"], version = "^1.24.5"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.24.6"}
 defang = "^0.5.3"
 ua-parser = "^0.18.0"
-redis = {version = "^5.0.3", extras = ["hiredis"]}
+redis = {version = "^5.0.4", extras = ["hiredis"]}
 dnspython = "^2.6.1"
 async-timeout = {version = "^4.0.3", python = "<3.11"}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-types-redis = {version = "^4.6.0.20240417"}
-mypy = "^1.9.0"
+types-redis = {version = "^4.6.0.20240425"}
+mypy = "^1.10.0"
 types-requests = "^2.31.0.20240406"
 types-beautifulsoup4 = "^4.12.0.20240229"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.18.0", python = ">=3.9"},
     {version = "^8.19.0", python = ">=3.10"}
 ]
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.9.2/PKG-INFO` & `lacuscore-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.9.2
+Version: 1.9.3
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,16 @@
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; python_version < "3.11"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
 Requires-Dist: dnspython (>=2.6.1,<3.0.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.24.5,<2.0.0)
-Requires-Dist: redis[hiredis] (>=5.0.3,<6.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.24.6,<2.0.0)
+Requires-Dist: redis[hiredis] (>=5.0.4,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.18.0,<0.19.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/lacuscore/badge/?version=latest)](https://lacuscore.readthedocs.io/en/latest/?badge=latest)
```

