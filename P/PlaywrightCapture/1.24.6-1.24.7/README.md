# Comparing `tmp/playwrightcapture-1.24.6.tar.gz` & `tmp/playwrightcapture-1.24.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.6.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.7.tar", max compression
```

## Comparing `playwrightcapture-1.24.6.tar` & `playwrightcapture-1.24.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/LICENSE
--rw-r--r--   0        0        0     1441 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/README.md
--rw-r--r--   0        0        0      511 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    64094 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1488 2024-04-24 13:59:38.240310 playwrightcapture-1.24.6/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.6/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/LICENSE
+-rw-r--r--   0        0        0     1441 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/README.md
+-rw-r--r--   0        0        0      511 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    64760 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1543 2024-05-02 15:51:35.388237 playwrightcapture-1.24.7/pyproject.toml
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 playwrightcapture-1.24.7/PKG-INFO
```

### Comparing `playwrightcapture-1.24.6/LICENSE` & `playwrightcapture-1.24.7/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.6/README.md` & `playwrightcapture-1.24.7/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.6/playwrightcapture/capture.py` & `playwrightcapture-1.24.7/playwrightcapture/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,15 +663,14 @@
             page.on("requestfinished", store_request)
 
         try:
             # Parse the URL. If there is a fragment, we need to scroll to it manually
             parsed_url = urlparse(url, allow_fragments=True)
 
             try:
-                # NOTE 2022-12-02: allow 15s less than the general timeout to get a DOM
                 await page.goto(url, wait_until='domcontentloaded', referer=referer if referer else '')
                 page.on("download", handle_download)
             except Error as initial_error:
                 self._update_exceptions(initial_error)
                 # So this one is really annoying: chromium raises a net::ERR_ABORTED when it hits a download
                 if initial_error.name in ['Download is starting', 'net::ERR_ABORTED']:
                     # page.goto failed, but it triggered a download event.
@@ -828,35 +827,47 @@
                             self.logger.warning(f'Attempting to capture URLs from {page.url} but there are too many ({total_urls}) to capture in too little time. Only capturing the first {max_captures} URLs in the page.')
                             if max_captures <= 0:
                                 # We don't really have time for even one capture, but let's try anyway.
                                 child_urls = child_urls[:1]
                             else:
                                 child_urls = child_urls[:max_captures]
                         self.logger.info(f'Capturing children, {max_captures} URLs')
+                        consecutive_errors = 0
                         for index, url in enumerate(child_urls):
                             self.logger.info(f'Capture child {url} - Timeout: {max_capture_time}s')
                             start_time = time.time()
                             if page.is_closed():
                                 self.logger.info('Page is closed, unable to capture children.')
                                 break
                             try:
                                 async with timeout(max_capture_time + 1):  # just adding a bit of padding so playwright has the chance to raise the exception first
                                     child_capture = await self.capture_page(
                                         url=url, referer=page.url,
                                         page=page, depth=depth,
                                         rendered_hostname_only=rendered_hostname_only,
                                         max_depth_capture_time=max_capture_time)
                                     to_return['children'].append(child_capture)  # type: ignore[union-attr]
-                            except (TimeoutError, asyncio.exceptions.TimeoutError):
+                            except (TimeoutError, asyncio.exceptions.TimeoutError, asyncio.TimeoutError):
                                 self.logger.info(f'Timeout error, took more than {max_capture_time}s. Unable to capture {url}.')
+                                consecutive_errors += 1
                             except Exception as e:
                                 self.logger.warning(f'Error while capturing child "{url}": {e}. {len(child_urls) - index - 1} more to go.')
+                                consecutive_errors += 1
                             else:
+                                consecutive_errors = 0
                                 runtime = int(time.time() - start_time)
                                 self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {len(child_urls) - index - 1} to go.')
+
+                            if consecutive_errors >= 5:
+                                # if we have more than 5 consecutive errors, the capture is most probably broken, breaking.
+                                self.logger.warning('Got more than 5 consecutive errors while capturing children, breaking.')
+                                to_return['error'] = "Got more than 5 consecutive errors while capturing children"
+                                self.should_retry = True
+                                break
+
                             try:
                                 await page.go_back()
                             except PlaywrightTimeoutError:
                                 self.logger.info('Go back timed out, it is probably not a big deal.')
                             except Exception as e:
                                 self.logger.info(f'Unable to go back: {e}.')
```

### Comparing `playwrightcapture-1.24.6/playwrightcapture/helpers.py` & `playwrightcapture-1.24.7/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.6/pyproject.toml` & `playwrightcapture-1.24.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.6"
+version = "1.24.7"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -26,25 +26,26 @@
 requests = {extras = ["socks"], version = "^2.31.0"}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.3", optional = true}
 pytz = {"version" = "^2024.1", python = "<3.9"}
 tzdata = "^2024.1"
 playwright-stealth = "^1.0.6"
 setuptools = "^69.5.1"
-puremagic = "^1.21"
+puremagic = "^1.22"
+async-timeout = {version = "^4.0.3", python = "<3.11"}
 
 [tool.poetry.extras]
 recaptcha = ["requests", "pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 types-beautifulsoup4 = "^4.12.0.20240229"
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 mypy = "^1.10.0"
 types-dateparser = "^1.2.0.20240420"
 types-requests = "^2.31.0.20240406"
 types-pytz = "^2024.1.0.20240417"
 
 
 [build-system]
```

### Comparing `playwrightcapture-1.24.6/PKG-INFO` & `playwrightcapture-1.24.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.6
+Version: 1.24.7
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -17,19 +17,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.3,<4.0.0) ; extra == "recaptcha"
+Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; python_version < "3.11"
 Requires-Dist: beautifulsoup4[charset-normalizer,lxml] (>=4.12.3,<5.0.0)
 Requires-Dist: dateparser (>=1.2.0,<2.0.0)
 Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: playwright-stealth (>=1.0.6,<2.0.0)
-Requires-Dist: puremagic (>=1.21,<2.0)
+Requires-Dist: puremagic (>=1.22,<2.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2024.1,<2025.0) ; python_version < "3.9"
 Requires-Dist: requests[socks] (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Requires-Dist: tzdata (>=2024.1,<2025.0)
 Requires-Dist: w3lib (>=2.1.2,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
```

