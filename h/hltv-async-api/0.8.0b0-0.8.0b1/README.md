# Comparing `tmp/hltv_async_api-0.8.0b0.tar.gz` & `tmp/hltv_async_api-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.8.0b0.tar", max compression
+gzip compressed data, was "hltv_async_api-0.8.0b1.tar", max compression
```

## Comparing `hltv_async_api-0.8.0b0.tar` & `hltv_async_api-0.8.0b1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      124 2024-04-30 11:24:20.003853 hltv_async_api-0.8.0b0/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    45823 2024-04-30 11:12:31.459993 hltv_async_api-0.8.0b0/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     4159 2024-04-30 11:02:43.900064 hltv_async_api-0.8.0b0/hltv_async_api/unreleased.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.8.0b0/LICENSE
--rw-r--r--   0        0        0      640 2024-04-30 11:24:19.991583 hltv_async_api-0.8.0b0/pyproject.toml
--rw-r--r--   0        0        0    16049 2024-04-30 11:23:03.942665 hltv_async_api-0.8.0b0/README.md
--rw-r--r--   0        0        0    16539 1970-01-01 00:00:00.000000 hltv_async_api-0.8.0b0/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-30 11:24:20.003853 hltv_async_api-0.8.0b1/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    46935 2024-04-30 12:10:21.347305 hltv_async_api-0.8.0b1/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     4159 2024-04-30 11:02:43.900064 hltv_async_api-0.8.0b1/hltv_async_api/unreleased.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.8.0b1/LICENSE
+-rw-r--r--   0        0        0      641 2024-04-30 12:11:41.845996 hltv_async_api-0.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0    16172 2024-04-30 12:04:54.250408 hltv_async_api-0.8.0b1/README.md
+-rw-r--r--   0        0        0    16652 1970-01-01 00:00:00.000000 hltv_async_api-0.8.0b1/PKG-INFO
```

### Comparing `hltv_async_api-0.8.0b0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.8.0b1/hltv_async_api/aiohltv.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
                  delete_proxy: bool = False,
                  tz: str | None = None,
+                 safe_mode: bool = True,
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "Europe/Copenhagen"
         }
         self.DEBUG = debug
@@ -54,14 +55,17 @@
             self.USE_PROXY = True
         else:
             self.USE_PROXY = False
 
         self.session = None
         self.loop = asyncio.get_running_loop()
 
+        self.SAFE = safe_mode
+        self._init_SAFE()
+
     async def __aenter__(self):
         self._create_session()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
 
@@ -85,15 +89,16 @@
                use_proxy: bool | None = None,
                proxy_file_path: str | None = None,
                proxy_list: list | None = None,
                debug: bool | None = None,
                max_retries: int | None = None,
                proxy_protocol: str | None = None,
                delete_proxy: bool | None = None,
-               tz: str = None,
+               tz: str | None = None,
+               safe_mode: bool | None = None,
                ):
         if max_delay:
             self.MAX_DELAY = max_delay
         if timeout:
             self.timeout = timeout
         if use_proxy is not None:
             self.USE_PROXY = use_proxy
@@ -110,23 +115,30 @@
             self._init_tz()
         if debug is not None:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
+        if safe_mode is not None:
+            self.SAFE = safe_mode
+            self._init_SAFE()
 
     def _init_tz(self, tz: str | None = None):
         if tz:
             try:
                 pytz.timezone(self.TIMEZONE)
             except pytz.exceptions.UnknownTimeZoneError:
                 self.logger.error('UnknownTimeZoneError, Using default timezone: Europe/Copenhagen')
                 self.TIMEZONE = None
 
+    def _init_SAFE(self):
+        if not self.SAFE:
+            self.logger.warning('Safe mode deactivated.')
+
     def _get_proxy(self):
         proxy = self.PROXY_LIST[0]
 
         if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
             proxy = self.PROXY_PROTOCOL + '://' + proxy
 
         return proxy
@@ -267,14 +279,19 @@
             if id:
                 return await self.get_team_info(id, title)
             else:
                 return await self.get_top_teams()
 
     async def get_matches(self, days: int = 1, min_rating: int = 1, live: bool = True, future: bool = True):
         """returns a list of all upcoming matches on HLTV"""
+
+        if self.SAFE:
+            self.logger.error('This function is not safe. Switch safe_mode to False to use this function')
+            return
+
         r = await self._fetch("https://www.hltv.org/matches")
         if not r:
             return
 
         matches = []
 
         try:
@@ -372,14 +389,18 @@
 
     async def get_match_info(self, id: str | int,
                              team1: str,
                              team2: str,
                              event_title: str,
                              stats: bool = True,
                              predicts: bool = True):
+        if self.SAFE:
+            self.logger.error('This function if SAFE. Switch safe to False to use this function')
+            return
+
         r = await self._fetch(f"https://www.hltv.org/matches/{str(id)}/"
                               f"{team1.replace(' ', '-')}-vs-"
                               f"{team2.replace(' ', '-')}-"
                               f"{event_title.replace(' ', '-')}")
         if not r:
             return
         status_ = {'Match over': 0, 'LIVE': 1}
@@ -501,14 +522,19 @@
 
     async def get_results(self, days: int = 1,
                           min_rating: int = 1,
                           max: int = 30,
                           featured: bool = True,
                           regular: bool = True) -> list[dict[str, Any]] | None:
         """returns a list of big event matches results"""
+
+        if self.SAFE:
+            self.logger.error('This function if SAFE. Switch safe to False to use this function')
+            return
+
         r = await self._fetch("https://www.hltv.org/results")
         if not r:
             return
 
         results = []
 
         if featured:
@@ -593,14 +619,19 @@
                         results.append(result_)
                         n += 1
 
         return results
 
     async def get_event_results(self, event_id: int | str, days: int = 1, max_: int = 10) -> list[
                                                                                                  dict[str, Any]] | None:
+
+        if self.SAFE:
+            self.logger.error('This function if SAFE. Switch safe to False to use this function')
+            return
+
         r = await self._fetch("https://www.hltv.org/results?event=" + str(event_id))
         if not r:
             return
 
         match_results = []
 
         n = 0
@@ -943,24 +974,27 @@
                     'age': age,
                     'weekstop30': weeks,
                     'last_trophy': last_trophy,
                     'total_trophies': total_trophies}
         except AttributeError:
             raise AttributeError("Parsing error, probably page not fully loaded")
 
-    async def get_top_players(self, top=40):
+    async def get_top_players(self, top: int = 40, year: str | int = datetime.strftime(datetime.utcnow(), '%Y')):
         """
         returns a list of the top (1-40) players in top 20 at the year
         :params:
         top: int = 40
         :returns:
         ('rank', 'name', 'team', 'maps', 'rating')
         maps - maps played
         """
-        year = datetime.strftime(datetime.utcnow(), '%Y')
+        if self.SAFE:
+            self.logger.error('This function is not safe. Switch safe_mode to False to use this function')
+            return
+
         r = await self._fetch(
             f"https://www.hltv.org/stats/players?startDate={year}-01-01&endDate={year}-12-31&rankingFilter=Top20")
 
         if not r:
             return
 
         players = []
@@ -1123,12 +1157,12 @@
                 break
 
         return news
 
 
 async def main():
     async with Hltv(proxy_path='proxies.txt', proxy_protocol='http', debug=True) as hltv:
-        print(await hltv.get_player_info(7998, 's1mple'))
+        print(await hltv.get_top_players())
 
 
 if __name__ == '__main__':
     asyncio.run(main())
```

### Comparing `hltv_async_api-0.8.0b0/hltv_async_api/unreleased.py` & `hltv_async_api-0.8.0b1/hltv_async_api/unreleased.py`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.8.0b0/LICENSE` & `hltv_async_api-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.8.0b0/pyproject.toml` & `hltv_async_api-0.8.0b1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.8.0b"
+version = "0.8.0b1"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.8.0b0/README.md` & `hltv_async_api-0.8.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,1004 +1,1011 @@
 00000000: 2320 686c 7476 2d61 7379 6e63 2d61 7069  # hltv-async-api
 00000010: 2061 6e20 2a2a 756e 6f66 6669 6369 616c   an **unofficial
 00000020: 2a2a 2061 7379 6e63 6872 6f6e 6f75 7320  ** asynchronous 
 00000030: 484c 5456 2041 5049 2057 7261 7070 6572  HLTV API Wrapper
-00000040: 2066 6f72 2050 7974 686f 6e2e 2055 7365   for Python. Use
-00000050: 206f 6e6c 7920 696e 206e 6f6e 2d63 6f6d   only in non-com
-00000060: 6d65 7263 6961 6c20 7075 7270 6f73 6573  mercial purposes
-00000070: 0d0a 0d0a 0d0a 2a2a 5468 6973 2070 6167  ......**This pag
-00000080: 6520 6973 206e 6f74 2063 6f6d 706c 6574  e is not complet
-00000090: 6564 2c20 6e6f 7420 616c 6c20 6d65 7468  ed, not all meth
-000000a0: 6f64 7320 616e 6420 636f 6e66 6967 7320  ods and configs 
-000000b0: 6172 6520 7772 6974 7465 6e2a 2a0d 0a0d  are written**...
-000000c0: 0a0d 0a23 2046 6561 7475 7265 730d 0a0d  ...# Features...
-000000d0: 0a0d 0a2a 202a 2a53 696d 706c 6520 5573  ...* **Simple Us
-000000e0: 6167 652a 2a20 2869 7473 2072 6561 6c6c  age** (its reall
-000000f0: 7920 7369 6d70 6c65 290d 0a0d 0a0d 0a2a  y simple)......*
-00000100: 202a 2a4e 6577 2061 6e64 206d 6f64 6572   **New and moder
-00000110: 6e20 6675 6c6c 7920 6173 796e 6320 6c69  n fully async li
-00000120: 6272 6172 792a 2a0d 0a0d 0a0d 0a2a 202a  brary**......* *
-00000130: 2a48 7567 6520 616d 6f75 6e74 206f 6620  *Huge amount of 
-00000140: 6f70 7469 6f6e 732a 2a0d 0a0d 0a0d 0a2a  options**......*
-00000150: 202a 2a53 7570 706f 7274 7320 7072 6f78   **Supports prox
-00000160: 7920 7573 6167 652a 2a0d 0a0d 0a0d 0a2a  y usage**......*
-00000170: 202a 2a4d 6164 6520 7769 7468 206c 6f76   **Made with lov
-00000180: 6520 3c33 2a2a 0d0a 0d0a 0d0a 2d2d 2d0d  e <3**......---.
-00000190: 0a0d 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
-000001a0: 6e0d 0a0d 0a60 6060 0d0a 7069 7020 696e  n....```..pip in
-000001b0: 7374 616c 6c20 686c 7476 2d61 7379 6e63  stall hltv-async
-000001c0: 2d61 7069 0d0a 6060 600d 0a0d 0a2d 2d2d  -api..```....---
-000001d0: 0d0a 0d0a 0d0a 2320 5369 6d70 6c65 2055  ......# Simple U
-000001e0: 7361 6765 0d0a 0d0a 2020 2020 6060 600d  sage....    ```.
-000001f0: 0a0d 0a20 2020 2066 726f 6d20 686c 7476  ...    from hltv
-00000200: 5f61 7379 6e63 5f61 7069 2069 6d70 6f72  _async_api impor
-00000210: 7420 486c 7476 0d0a 2020 2020 0d0a 2020  t Hltv..    ..  
-00000220: 2020 6173 796e 6320 7769 7468 2048 6c74    async with Hlt
-00000230: 7628 2920 6173 2068 6c74 763a 0d0a 2020  v() as hltv:..  
-00000240: 2020 2020 7072 696e 7428 6177 6169 7420      print(await 
-00000250: 686c 7476 2e67 6574 5f65 7665 6e74 5f69  hltv.get_event_i
-00000260: 6e66 6f28 3731 3438 2c20 2750 474c 2043  nfo(7148, 'PGL C
-00000270: 5332 204d 616a 6f72 2043 6f70 656e 6861  S2 Major Copenha
-00000280: 6765 6e32 3032 3427 2929 0d0a 0d0a 2020  gen2024'))....  
-00000290: 2020 6060 600d 0a0d 0a20 202a 2a4f 522a    ```....  **OR*
-000002a0: 2a0d 0a0d 0a20 2020 2060 6060 0d0a 0d0a  *....    ```....
-000002b0: 2020 2020 6672 6f6d 2068 6c74 765f 6173      from hltv_as
-000002c0: 796e 635f 6170 6920 696d 706f 7274 2048  ync_api import H
-000002d0: 6c74 760d 0a20 2020 200d 0a20 2020 2068  ltv..    ..    h
-000002e0: 6c74 7620 3d20 486c 7476 2829 0d0a 2020  ltv = Hltv()..  
-000002f0: 2020 7072 696e 7428 6177 6169 7420 686c    print(await hl
-00000300: 7476 2e67 6574 5f65 7665 6e74 5f69 6e66  tv.get_event_inf
-00000310: 6f28 3731 3438 2c20 2750 474c 2043 5332  o(7148, 'PGL CS2
-00000320: 204d 616a 6f72 2043 6f70 656e 6861 6765   Major Copenhage
-00000330: 6e32 3032 3427 2929 0d0a 2020 2020 6177  n2024'))..    aw
-00000340: 6169 7420 686c 7476 2e63 6c6f 7365 2829  ait hltv.close()
-00000350: 0d0a 0d0a 2020 2020 6060 600d 0a0d 0a2d  ....    ```....-
-00000360: 2d2d 0d0a 0d0a 2320 5072 6f78 7920 5573  --....# Proxy Us
-00000370: 6167 650d 0a0d 0a2a 2a4c 6f61 6420 5072  age....**Load Pr
-00000380: 6f78 6965 7320 6672 6f6d 206c 6973 742a  oxies from list*
-00000390: 2a0d 0a20 2020 200d 0a20 2020 2060 6060  *..    ..    ```
-000003a0: 0d0a 2020 2020 7072 6f78 795f 6c69 7374  ..    proxy_list
-000003b0: 203d 205b 2768 7474 703a 2f2f 3132 302e   = ['http://120.
-000003c0: 3233 342e 3230 332e 3137 313a 3930 3032  234.203.171:9002
-000003d0: 272c 2027 6874 7470 3a2f 2f31 3130 2e33  ', 'http://110.3
-000003e0: 382e 3638 2e33 383a 3830 275d 0d0a 2020  8.68.38:80']..  
-000003f0: 2020 0d0a 2020 2020 686c 7476 203d 2048    ..    hltv = H
-00000400: 6c74 7628 7072 6f78 795f 6c69 7374 3d70  ltv(proxy_list=p
-00000410: 726f 7879 5f6c 6973 7429 0d0a 0d0a 2020  roxy_list)....  
-00000420: 2020 6060 600d 0a0d 0a2a 2a4c 6f61 6420    ```....**Load 
-00000430: 5072 6f78 6965 7320 6672 6f6d 2066 696c  Proxies from fil
-00000440: 652a 2a0d 0a0d 0a20 2020 2060 6060 0d0a  e**....    ```..
-00000450: 2020 2020 686c 7476 203d 2048 6c74 7628      hltv = Hltv(
-00000460: 7072 6f78 795f 7061 7468 3d27 5041 5448  proxy_path='PATH
-00000470: 5f54 4f5f 5052 4f58 592e 5458 5427 290d  _TO_PROXY.TXT').
-00000480: 0a20 2020 2060 6060 0d0a 0d0a 0d0a 2a2a  .    ```......**
-00000490: 4465 6c65 7465 2070 726f 7879 2a2a 0d0a  Delete proxy**..
-000004a0: 0d0a 2020 2020 5265 6d6f 7665 7320 6261  ..    Removes ba
-000004b0: 6420 7072 6f78 6965 730d 0a20 2020 200d  d proxies..    .
-000004c0: 0a20 2020 2060 6060 0d0a 2020 2020 686c  .    ```..    hl
-000004d0: 7476 203d 2048 6c74 7628 7072 6f78 795f  tv = Hltv(proxy_
-000004e0: 7061 7468 3d27 5041 5448 5f54 4f5f 5052  path='PATH_TO_PR
-000004f0: 4f58 592e 5458 5427 2c20 6465 6c65 7465  OXY.TXT', delete
-00000500: 5f70 726f 7879 3d54 7275 6529 0d0a 2020  _proxy=True)..  
-00000510: 2020 6060 600d 0a0d 0a2a 2a50 726f 746f    ```....**Proto
-00000520: 636f 6c20 7573 6167 652a 2a0d 0a0d 0a20  col usage**.... 
-00000530: 2020 2060 6060 0d0a 2020 2020 7072 6f78     ```..    prox
-00000540: 795f 6c69 7374 203d 205b 2731 3230 2e32  y_list = ['120.2
-00000550: 3334 2e32 3033 2e31 3731 3a39 3030 3227  34.203.171:9002'
-00000560: 2c20 2731 3130 2e33 382e 3638 2e33 383a  , '110.38.68.38:
-00000570: 3830 275d 0d0a 2020 2020 0d0a 2020 2020  80']..    ..    
-00000580: 686c 7476 203d 2048 6c74 7628 7072 6f78  hltv = Hltv(prox
-00000590: 795f 6c69 7374 3d70 726f 7879 5f6c 6973  y_list=proxy_lis
-000005a0: 742c 2070 726f 7879 5f70 726f 746f 636f  t, proxy_protoco
-000005b0: 6c3d 2768 7474 7027 290d 0a20 2020 2060  l='http')..    `
-000005c0: 6060 0d0a 0d0a 2d2d 2d0d 0a23 204d 6574  ``....---..# Met
-000005d0: 686f 6473 0d0a 0d0a 2a20 2a2a 6765 745f  hods....* **get_
-000005e0: 6d61 7463 6865 7328 6461 7973 3a20 696e  matches(days: in
-000005f0: 7420 3d20 312c 206d 696e 5f73 7461 725f  t = 1, min_star_
-00000600: 7261 7469 6e67 3a20 696e 7420 3d20 312c  rating: int = 1,
-00000610: 206c 6976 653a 2062 6f6f 6c20 3d20 5472   live: bool = Tr
-00000620: 7565 2c20 6675 7475 7265 3a20 626f 6f6c  ue, future: bool
-00000630: 203d 2054 7275 6529 2a2a 0d0a 0d0a 2020   = True)**....  
-00000640: 2020 2d64 6179 7320 2874 6865 206e 756d    -days (the num
-00000650: 6265 7220 6f66 2064 6179 7320 696e 746f  ber of days into
-00000660: 2074 6865 2066 7574 7572 6520 746f 2066   the future to f
-00000670: 6574 6368 206d 6174 6368 6573 2066 6f72  etch matches for
-00000680: 290d 0a20 200d 0a20 2020 202d 6d69 6e5f  )..  ..    -min_
-00000690: 7374 6172 5f72 6174 696e 6720 2874 6865  star_rating (the
-000006a0: 206d 696e 696d 756d 2073 7461 7220 7261   minimum star ra
-000006b0: 7469 6e67 2066 6f72 206d 6174 6368 6573  ting for matches
-000006c0: 2074 6f20 696e 636c 7564 6529 0d0a 2020   to include)..  
-000006d0: 0d0a 2020 2020 6060 600d 0a20 2020 2061  ..    ```..    a
-000006e0: 7761 6974 2068 6c74 762e 6765 745f 6d61  wait hltv.get_ma
-000006f0: 7463 6865 7328 6461 7973 3d31 290d 0a20  tches(days=1).. 
-00000700: 2020 200d 0a20 2020 203e 3e3e 205b 7b27     ..    >>> [{'
-00000710: 6964 273a 2027 3233 3731 3230 3127 2c20  id': '2371201', 
-00000720: 2764 6174 6527 3a20 274c 4956 4527 2c20  'date': 'LIVE', 
-00000730: 2774 696d 6527 3a20 274c 4956 4527 2c20  'time': 'LIVE', 
-00000740: 2774 6561 6d31 273a 2027 496d 7065 7269  'team1': 'Imperi
-00000750: 616c 272c 2027 7465 616d 3227 3a20 274d  al', 'team2': 'M
-00000760: 4942 5227 2c20 2774 315f 6964 273a 2027  IBR', 't1_id': '
-00000770: 3934 3535 272c 2027 7432 5f69 6427 3a20  9455', 't2_id': 
-00000780: 2739 3231 3527 2c20 276d 6170 7327 3a20  '9215', 'maps': 
-00000790: 2733 272c 2027 7261 7469 6e67 273a 2031  '3', 'rating': 1
-000007a0: 2c20 2765 7665 6e74 273a 2027 5245 5320  , 'event': 'RES 
-000007b0: 5265 6769 6f6e 616c 2053 6572 6965 7320  Regional Series 
-000007c0: 3320 4c41 5441 4d27 7d2c 207b 2769 6427  3 LATAM'}, {'id'
-000007d0: 3a20 2732 3337 3039 3634 272c 2027 6461  : '2370964', 'da
-000007e0: 7465 273a 2027 3230 3234 2d30 342d 3136  te': '2024-04-16
-000007f0: 272c 2027 7469 6d65 273a 2027 3132 3a33  ', 'time': '12:3
-00000800: 3027 2c20 2774 6561 6d31 273a 2027 5341  0', 'team1': 'SA
-00000810: 5727 2c20 2774 6561 6d32 273a 2027 5361  W', 'team2': 'Sa
-00000820: 6d70 6927 2c20 2774 315f 6964 273a 2027  mpi', 't1_id': '
-00000830: 3130 3536 3727 2c20 2774 325f 6964 273a  10567', 't2_id':
-00000840: 2027 3130 3639 3527 2c20 276d 6170 7327   '10695', 'maps'
-00000850: 3a20 2733 272c 2027 7261 7469 6e67 273a  : '3', 'rating':
-00000860: 2031 2c20 2765 7665 6e74 273a 2027 5468   1, 'event': 'Th
-00000870: 756e 6465 7270 6963 6b20 576f 726c 6420  underpick World 
-00000880: 4368 616d 7069 6f6e 7368 6970 2032 3032  Championship 202
-00000890: 3420 4555 2043 6c6f 7365 6420 5175 616c  4 EU Closed Qual
-000008a0: 6966 6965 7220 3127 7d2c 207b 2769 6427  ifier 1'}, {'id'
-000008b0: 3a20 2732 3337 3133 3637 272c 2027 6461  : '2371367', 'da
-000008c0: 7465 273a 2027 3230 3234 2d30 342d 3136  te': '2024-04-16
-000008d0: 272c 2027 7469 6d65 273a 2027 3134 3a30  ', 'time': '14:0
-000008e0: 3027 2c20 2774 6561 6d31 273a 2027 4761  0', 'team1': 'Ga
-000008f0: 696d 696e 2047 6c61 6469 6174 6f72 7327  imin Gladiators'
-00000900: 2c20 2774 6561 6d32 273a 2027 5065 726d  , 'team2': 'Perm
-00000910: 6974 7461 272c 2027 7431 5f69 6427 3a20  itta', 't1_id': 
-00000920: 2731 3135 3731 272c 2027 7432 5f69 6427  '11571', 't2_id'
-00000930: 3a20 2731 3230 3039 272c 2027 6d61 7073  : '12009', 'maps
-00000940: 273a 2027 3327 2c20 2772 6174 696e 6727  ': '3', 'rating'
-00000950: 3a20 312c 2027 6576 656e 7427 3a20 2745  : 1, 'event': 'E
-00000960: 6c69 7361 2049 6e76 6974 6174 696f 6e61  lisa Invitationa
-00000970: 6c20 5370 7269 6e67 2032 3032 3427 7d5d  l Spring 2024'}]
-00000980: 0d0a 2020 2020 0d0a 2020 2020 6060 600d  ..    ..    ```.
-00000990: 0a0d 0a2a 202a 2a67 6574 5f6d 6174 6368  ...* **get_match
-000009a0: 5f69 6e66 6f28 6d61 7463 685f 6964 3a20  _info(match_id: 
-000009b0: 696e 7420 7c20 7374 722c 2074 6561 6d31  int | str, team1
-000009c0: 2c20 7465 616d 322c 2065 7665 6e74 5f74  , team2, event_t
-000009d0: 6974 6c65 2c20 7374 6174 733a 2062 6f6f  itle, stats: boo
-000009e0: 6c20 3d20 5472 7565 2c20 7072 6564 6963  l = True, predic
-000009f0: 7473 3a20 626f 6f6c 203d 2054 7275 6529  ts: bool = True)
-00000a00: 2a2a 0d0a 2020 0d0a 2020 2020 6060 600d  **..  ..    ```.
-00000a10: 0a20 2020 2061 7761 6974 2068 6c74 762e  .    await hltv.
-00000a20: 6765 745f 6d61 7463 685f 696e 666f 2832  get_match_info(2
-00000a30: 3337 3039 3331 2c20 274d 6f75 7a27 2c20  370931, 'Mouz', 
-00000a40: 2766 617a 6527 2c20 2769 656d 2d63 6865  'faze', 'iem-che
-00000a50: 6e67 6475 2d32 3032 3427 2920 200d 0a20  ngdu-2024')  .. 
-00000a60: 200d 0a20 2020 203e 3e3e 2832 3337 3039   ..    >>>(23709
-00000a70: 3331 2c20 2730 272c 2027 3227 2c20 274d  31, '0', '2', 'M
-00000a80: 6174 6368 206f 7665 7227 2c20 5b7b 276d  atch over', [{'m
-00000a90: 6170 6e61 6d65 273a 2027 4f76 6572 7061  apname': 'Overpa
-00000aa0: 7373 272c 2027 725f 7465 616d 3127 3a20  ss', 'r_team1': 
-00000ab0: 2731 3027 2c20 2772 5f74 6561 6d32 273a  '10', 'r_team2':
-00000ac0: 2027 3133 277d 2c20 7b27 6d61 706e 616d   '13'}, {'mapnam
-00000ad0: 6527 3a20 274e 756b 6527 2c20 2772 5f74  e': 'Nuke', 'r_t
-00000ae0: 6561 6d31 273a 2027 3627 2c20 2772 5f74  eam1': '6', 'r_t
-00000af0: 6561 6d32 273a 2027 3133 277d 2c20 7b27  eam2': '13'}, {'
-00000b00: 6d61 706e 616d 6527 3a20 274d 6972 6167  mapname': 'Mirag
-00000b10: 6527 2c20 2772 5f74 6561 6d31 273a 2027  e', 'r_team1': '
-00000b20: 2d27 2c20 2772 5f74 6561 6d32 273a 2027  -', 'r_team2': '
-00000b30: 2d27 7d5d 2c20 5b7b 2769 6427 3a20 2731  -'}], [{'id': '1
-00000b40: 3838 3530 272c 2027 6e69 636b 6e61 6d65  8850', 'nickname
-00000b50: 273a 2027 4a69 6d70 7068 6174 272c 2027  ': 'Jimpphat', '
-00000b60: 6b64 273a 2027 3333 2d32 3927 2c20 2761  kd': '33-29', 'a
-00000b70: 6472 273a 2027 3830 2e39 272c 2027 7261  dr': '80.9', 'ra
-00000b80: 7469 6e67 273a 2027 312e 3038 277d 2c20  ting': '1.08'}, 
-00000b90: 0d0a 2020 0d0a 2020 2020 7b27 6964 273a  ..  ..    {'id':
-00000ba0: 2027 3138 3037 3227 2c20 276e 6963 6b6e   '18072', 'nickn
-00000bb0: 616d 6527 3a20 2774 6f72 7a73 6927 2c20  ame': 'torzsi', 
-00000bc0: 276b 6427 3a20 2732 362d 3235 272c 2027  'kd': '26-25', '
-00000bd0: 6164 7227 3a20 2737 302e 3527 2c20 2772  adr': '70.5', 'r
-00000be0: 6174 696e 6727 3a20 2731 2e30 3227 7d2c  ating': '1.02'},
-00000bf0: 207b 2769 6427 3a20 2731 3336 3636 272c   {'id': '13666',
-00000c00: 2027 6e69 636b 6e61 6d65 273a 2027 4272   'nickname': 'Br
-00000c10: 6f6c 6c61 6e27 2c20 276b 6427 3a20 2732  ollan', 'kd': '2
-00000c20: 352d 3331 272c 2027 6164 7227 3a20 2736  5-31', 'adr': '6
-00000c30: 382e 3427 2c20 2772 6174 696e 6727 3a20  8.4', 'rating': 
-00000c40: 2730 2e39 3027 7d2c 207b 2769 6427 3a20  '0.90'}, {'id': 
-00000c50: 2732 3033 3132 272c 2027 6e69 636b 6e61  '20312', 'nickna
-00000c60: 6d65 273a 2027 7865 7274 696f 4e27 2c20  me': 'xertioN', 
-00000c70: 276b 6427 3a20 2732 332d 3331 272c 2027  'kd': '23-31', '
-00000c80: 6164 7227 3a20 2736 322e 3427 2c20 2772  adr': '62.4', 'r
-00000c90: 6174 696e 6727 3a20 2730 2e38 3227 7d2c  ating': '0.82'},
-00000ca0: 207b 2769 6427 3a20 2731 3638 3230 272c   {'id': '16820',
-00000cb0: 2027 6e69 636b 6e61 6d65 273a 2027 7369   'nickname': 'si
-00000cc0: 7568 7927 2c20 276b 6427 3a20 2731 372d  uhy', 'kd': '17-
-00000cd0: 3330 272c 2027 6164 7227 3a20 2735 312e  30', 'adr': '51.
-00000ce0: 3627 2c20 2772 6174 696e 6727 3a20 2730  6', 'rating': '0
-00000cf0: 2e37 3027 7d2c 207b 2769 6427 3a20 2731  .70'}, {'id': '1
-00000d00: 3830 3533 272c 2027 6e69 636b 6e61 6d65  8053', 'nickname
-00000d10: 273a 2027 6272 6f6b 7927 2c20 276b 6427  ': 'broky', 'kd'
-00000d20: 3a20 2733 342d 3232 272c 2027 6164 7227  : '34-22', 'adr'
-00000d30: 3a20 2737 392e 3327 2c20 2772 6174 696e  : '79.3', 'ratin
-00000d40: 6727 3a20 2731 2e33 3327 7d2c 207b 2769  g': '1.33'}, {'i
-00000d50: 6427 3a20 2739 3936 3027 2c20 276e 6963  d': '9960', 'nic
-00000d60: 6b6e 616d 6527 3a20 2766 726f 7a65 6e27  kname': 'frozen'
-00000d70: 2c20 276b 6427 3a20 2733 332d 3233 272c  , 'kd': '33-23',
-00000d80: 2027 6164 7227 3a20 2738 352e 3527 2c20   'adr': '85.5', 
-00000d90: 2772 6174 696e 6727 3a20 2731 2e33 3127  'rating': '1.31'
-00000da0: 7d2c 207b 2769 6427 3a20 2731 3138 3136  }, {'id': '11816
-00000db0: 272c 2027 6e69 636b 6e61 6d65 273a 2027  ', 'nickname': '
-00000dc0: 726f 707a 272c 2027 6b64 273a 2027 3331  ropz', 'kd': '31
-00000dd0: 2d32 3627 2c20 2761 6472 273a 2027 3733  -26', 'adr': '73
-00000de0: 2e30 272c 2027 7261 7469 6e67 273a 2027  .0', 'rating': '
-00000df0: 312e 3230 277d 2c20 7b27 6964 273a 2027  1.20'}, {'id': '
-00000e00: 3831 3833 272c 2027 6e69 636b 6e61 6d65  8183', 'nickname
-00000e10: 273a 2027 7261 696e 272c 2027 6b64 273a  ': 'rain', 'kd':
-00000e20: 2027 3237 2d32 3627 2c20 2761 6472 273a   '27-26', 'adr':
-00000e30: 2027 3832 2e30 272c 2027 7261 7469 6e67   '82.0', 'rating
-00000e40: 273a 2027 312e 3138 277d 2c20 7b27 6964  ': '1.18'}, {'id
-00000e50: 273a 2027 3432 3927 2c20 276e 6963 6b6e  ': '429', 'nickn
-00000e60: 616d 6527 3a20 276b 6172 7269 6761 6e27  ame': 'karrigan'
-00000e70: 2c20 276b 6427 3a20 2732 302d 3238 272c  , 'kd': '20-28',
-00000e80: 2027 6164 7227 3a20 2734 392e 3727 2c20   'adr': '49.7', 
-00000e90: 2772 6174 696e 6727 3a20 2730 2e38 3127  'rating': '0.81'
-00000ea0: 7d5d 2920 200d 0a20 2020 200d 0a20 2020  }])  ..    ..   
-00000eb0: 2060 6060 0d0a 2020 0d0a 2a20 2a2a 6765   ```..  ..* **ge
-00000ec0: 745f 7265 7375 6c74 7328 6461 7973 3a20  t_results(days: 
-00000ed0: 696e 7420 3d20 312c 206d 696e 5f72 6174  int = 1, min_rat
-00000ee0: 696e 673a 2069 6e74 203d 2031 2c20 6d61  ing: int = 1, ma
-00000ef0: 783a 2069 6e74 203d 2033 302c 2066 6561  x: int = 30, fea
-00000f00: 7475 7265 643a 2062 6f6f 6c20 3d20 5472  tured: bool = Tr
-00000f10: 7565 2c20 7265 6775 6c61 723a 2062 6f6f  ue, regular: boo
-00000f20: 6c20 3d20 5472 7565 2929 202d 3e2a 2a0d  l = True)) ->**.
-00000f30: 0a20 2020 200d 0a20 2020 2060 6060 0d0a  .    ..    ```..
-00000f40: 2020 2020 7072 696e 7428 6177 6169 7420      print(await 
-00000f50: 686c 7476 2e67 6574 5f72 6573 756c 7473  hltv.get_results
-00000f60: 2829 290d 0a20 200d 0a20 2020 205b 7b27  ())..  ..    [{'
-00000f70: 6964 273a 2027 3233 3730 3933 3127 2c20  id': '2370931', 
-00000f80: 2774 6561 6d31 273a 2027 4d4f 555a 272c  'team1': 'MOUZ',
-00000f90: 2027 7465 616d 3227 3a20 2746 615a 6527   'team2': 'FaZe'
-00000fa0: 2c20 2773 636f 7265 3127 3a20 2730 272c  , 'score1': '0',
-00000fb0: 2027 7363 6f72 6532 273a 2027 3227 2c20   'score2': '2', 
-00000fc0: 2772 6174 696e 6727 3a20 302c 2027 6576  'rating': 0, 'ev
-00000fd0: 656e 7427 3a20 2749 454d 2043 6865 6e67  ent': 'IEM Cheng
-00000fe0: 6475 2032 3032 3427 7d5d 0d0a 2020 2020  du 2024'}]..    
-00000ff0: 6060 600d 0a20 200d 0a2a 202a 2a67 6574  ```..  ..* **get
-00001000: 5f65 7665 6e74 7328 6f75 7467 6f69 6e67  _events(outgoing
-00001010: 3d54 7275 652c 2066 7574 7572 653d 5472  =True, future=Tr
-00001020: 7565 2c20 6d61 785f 6576 656e 7473 3d31  ue, max_events=1
-00001030: 3029 202d 3e20 5b28 2769 6427 2c20 2774  0) -> [('id', 't
-00001040: 6974 6c65 272c 2027 7374 6172 7464 6174  itle', 'startdat
-00001050: 6527 2c20 2765 6e64 6461 7465 2729 5d2a  e', 'enddate')]*
-00001060: 2a0d 0a0d 0a20 2020 2060 6060 0d0a 2020  *....    ```..  
-00001070: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
-00001080: 5f65 7665 6e74 7328 6675 7475 7265 3d46  _events(future=F
-00001090: 616c 7365 290d 0a20 2020 200d 0a20 2020  alse)..    ..   
-000010a0: 203e 3e3e 5b7b 2769 6427 3a20 2737 3734   >>>[{'id': '774
-000010b0: 3927 2c20 2774 6974 6c65 273a 2027 5468  9', 'title': 'Th
-000010c0: 756e 6465 7270 6963 6b20 576f 726c 6420  underpick World 
-000010d0: 4368 616d 7069 6f6e 7368 6970 2032 3032  Championship 202
-000010e0: 3420 4555 2043 6c6f 7365 6420 5175 616c  4 EU Closed Qual
-000010f0: 6966 6965 7220 3127 2c20 2773 7461 7274  ifier 1', 'start
-00001100: 5f64 6174 6527 3a20 2731 2d34 272c 2027  _date': '1-4', '
-00001110: 656e 645f 6461 7465 273a 2027 3232 2d34  end_date': '22-4
-00001120: 277d 2c20 7b27 6964 273a 2027 3736 3231  '}, {'id': '7621
-00001130: 272c 2027 7469 746c 6527 3a20 2745 534c  ', 'title': 'ESL
-00001140: 2043 6861 6c6c 656e 6765 7220 4c65 6167   Challenger Leag
-00001150: 7565 2053 6561 736f 6e20 3437 204e 6f72  ue Season 47 Nor
-00001160: 7468 2041 6d65 7269 6361 272c 2027 7374  th America', 'st
-00001170: 6172 745f 6461 7465 273a 2027 3133 2d32  art_date': '13-2
-00001180: 272c 2027 656e 645f 6461 7465 273a 2027  ', 'end_date': '
-00001190: 3136 2d36 277d 5d0d 0a20 2020 2020 200d  16-6'}]..      .
-000011a0: 0a20 2020 2060 6060 0d0a 0d0a 2a20 2a2a  .    ```....* **
-000011b0: 6765 745f 6576 656e 745f 7265 7375 6c74  get_event_result
-000011c0: 7328 6576 656e 745f 6964 3a20 696e 7420  s(event_id: int 
-000011d0: 7c20 7374 722c 2064 6179 733a 2069 6e74  | str, days: int
-000011e0: 203d 2031 2c20 6d61 785f 3a20 696e 7420   = 1, max_: int 
-000011f0: 3d20 3130 292a 2a0d 0a0d 0a20 200d 0a20  = 10)**....  .. 
-00001200: 2020 2060 6060 0d0a 2020 2020 6177 6169     ```..    awai
-00001210: 7420 6765 745f 6576 656e 745f 7265 7375  t get_event_resu
-00001220: 6c74 7328 3731 3438 290d 0a20 2020 200d  lts(7148)..    .
-00001230: 0a20 2020 203e 3e3e 5b7b 2769 6427 3a20  .    >>>[{'id': 
-00001240: 2732 3337 3039 3331 272c 2027 6461 7465  '2370931', 'date
-00001250: 273a 2027 3134 2d30 342d 3230 3234 272c  ': '14-04-2024',
-00001260: 2027 7465 616d 3127 3a20 274d 4f55 5a27   'team1': 'MOUZ'
-00001270: 2c20 2774 6561 6d32 273a 2027 4661 5a65  , 'team2': 'FaZe
-00001280: 272c 2027 7363 6f72 6531 273a 2027 3027  ', 'score1': '0'
-00001290: 2c20 2773 636f 7265 3227 3a20 2732 277d  , 'score2': '2'}
-000012a0: 5d0d 0a0d 0a20 2020 2060 6060 0d0a 0d0a  ]....    ```....
-000012b0: 2a20 2a2a 6765 745f 6576 656e 745f 6d61  * **get_event_ma
-000012c0: 7463 6865 7328 6576 656e 745f 6964 3a20  tches(event_id: 
-000012d0: 7374 7220 7c20 696e 742c 2064 6179 733a  str | int, days:
-000012e0: 2069 6e74 203d 2031 293a 2a2a 0d0a 2020   int = 1):**..  
-000012f0: 0d0a 2020 2020 6060 600d 0a20 2020 2061  ..    ```..    a
-00001300: 7761 6974 2068 6c74 762e 6765 745f 6576  wait hltv.get_ev
-00001310: 656e 745f 6d61 7463 6865 7328 3731 3438  ent_matches(7148
-00001320: 290d 0a20 2020 200d 0a20 2020 203e 3e3e  )..    ..    >>>
-00001330: 5b7b 2769 6427 3a20 2732 3337 3037 3731  [{'id': '2370771
-00001340: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
-00001350: 2d30 342d 3138 272c 2027 7469 6d65 273a  -04-18', 'time':
-00001360: 2027 3135 3a33 3027 2c20 2774 6561 6d31   '15:30', 'team1
-00001370: 273a 2027 4d6f 6e74 6527 2c20 2774 6561  ': 'Monte', 'tea
-00001380: 6d32 273a 2027 7061 694e 272c 2027 7431  m2': 'paiN', 't1
-00001390: 5f69 6427 3a20 2731 3138 3131 272c 2027  _id': '11811', '
-000013a0: 7432 5f69 6427 3a20 2734 3737 3327 7d2c  t2_id': '4773'},
-000013b0: 207b 2769 6427 3a20 2732 3337 3037 3732   {'id': '2370772
-000013c0: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
-000013d0: 2d30 342d 3138 272c 2027 7469 6d65 273a  -04-18', 'time':
-000013e0: 2027 3137 3a30 3027 2c20 2774 6561 6d31   '17:00', 'team1
-000013f0: 273a 2027 496d 7065 7269 616c 272c 2027  ': 'Imperial', '
-00001400: 7465 616d 3227 3a20 274d 6574 697a 706f  team2': 'Metizpo
-00001410: 7274 272c 2027 7431 5f69 6427 3a20 2739  rt', 't1_id': '9
-00001420: 3435 3527 2c20 2774 325f 6964 273a 2027  455', 't2_id': '
-00001430: 3131 3634 3127 7d2c 207b 2769 6427 3a20  11641'}, {'id': 
-00001440: 2732 3337 3037 3733 272c 2027 6461 7465  '2370773', 'date
-00001450: 273a 2027 3230 3234 2d30 342d 3138 272c  ': '2024-04-18',
-00001460: 2027 7469 6d65 273a 2027 3138 3a33 3027   'time': '18:30'
-00001470: 2c20 2774 6561 6d31 273a 2027 4655 5249  , 'team1': 'FURI
-00001480: 4127 2c20 2774 6561 6d32 273a 2027 397a  A', 'team2': '9z
-00001490: 272c 2027 7431 5f69 6427 3a20 2738 3239  ', 't1_id': '829
-000014a0: 3727 2c20 2774 325f 6964 273a 2027 3939  7', 't2_id': '99
-000014b0: 3936 277d 2c20 7b27 6964 273a 2027 3233  96'}, {'id': '23
-000014c0: 3730 3737 3427 2c20 2764 6174 6527 3a20  70774', 'date': 
-000014d0: 2732 3032 342d 3034 2d31 3827 2c20 2774  '2024-04-18', 't
-000014e0: 696d 6527 3a20 2732 303a 3030 272c 2027  ime': '20:00', '
-000014f0: 7465 616d 3127 3a20 274d 4942 5227 2c20  team1': 'MIBR', 
-00001500: 2774 6561 6d32 273a 2027 4f47 272c 2027  'team2': 'OG', '
-00001510: 7431 5f69 6427 3a20 2739 3231 3527 2c20  t1_id': '9215', 
-00001520: 2774 325f 6964 273a 2027 3130 3530 3327  't2_id': '10503'
-00001530: 7d2c 207b 2769 6427 3a20 2732 3337 3037  }, {'id': '23707
-00001540: 3735 272c 2027 6461 7465 273a 2027 3230  75', 'date': '20
-00001550: 3234 2d30 342d 3138 272c 2027 7469 6d65  24-04-18', 'time
-00001560: 273a 2027 3231 3a33 3027 2c20 2774 6561  ': '21:30', 'tea
-00001570: 6d31 273a 2027 5442 4427 2c20 2774 6561  m1': 'TBD', 'tea
-00001580: 6d32 273a 2027 5442 4427 2c20 2774 315f  m2': 'TBD', 't1_
-00001590: 6964 273a 2030 2c20 2774 325f 6964 273a  id': 0, 't2_id':
-000015a0: 2030 7d2c 207b 2769 6427 3a20 2732 3337   0}, {'id': '237
-000015b0: 3037 3736 272c 2027 6461 7465 273a 2027  0776', 'date': '
-000015c0: 3230 3234 2d30 342d 3138 272c 2027 7469  2024-04-18', 'ti
-000015d0: 6d65 273a 2027 3233 3a30 3027 2c20 2774  me': '23:00', 't
-000015e0: 6561 6d31 273a 2027 5442 4427 2c20 2774  eam1': 'TBD', 't
-000015f0: 6561 6d32 273a 2027 5442 4427 2c20 2774  eam2': 'TBD', 't
-00001600: 315f 6964 273a 2030 2c20 2774 325f 6964  1_id': 0, 't2_id
-00001610: 273a 2030 7d2c 207b 2769 6427 3a20 2732  ': 0}, {'id': '2
-00001620: 3337 3037 3737 272c 2027 6461 7465 273a  370777', 'date':
-00001630: 2027 3230 3234 2d30 342d 3139 272c 2027   '2024-04-19', '
-00001640: 7469 6d65 273a 2027 3030 3a30 3027 2c20  time': '00:00', 
-00001650: 2774 6561 6d31 273a 2027 5442 4427 2c20  'team1': 'TBD', 
-00001660: 2774 6561 6d32 273a 2027 5442 4427 2c20  'team2': 'TBD', 
-00001670: 2774 315f 6964 273a 2030 2c20 2774 325f  't1_id': 0, 't2_
-00001680: 6964 273a 2030 7d2c 207b 2769 6427 3a20  id': 0}, {'id': 
-00001690: 2732 3337 3037 3738 272c 2027 6461 7465  '2370778', 'date
-000016a0: 273a 2027 3230 3234 2d30 342d 3139 272c  ': '2024-04-19',
-000016b0: 2027 7469 6d65 273a 2027 3135 3a30 3027   'time': '15:00'
-000016c0: 2c20 2774 6561 6d31 273a 2027 5442 4427  , 'team1': 'TBD'
-000016d0: 2c20 2774 6561 6d32 273a 2027 5442 4427  , 'team2': 'TBD'
-000016e0: 2c20 2774 315f 6964 273a 2030 2c20 2774  , 't1_id': 0, 't
-000016f0: 325f 6964 273a 2030 7d2c 207b 2769 6427  2_id': 0}, {'id'
-00001700: 3a20 2732 3337 3037 3739 272c 2027 6461  : '2370779', 'da
-00001710: 7465 273a 2027 3230 3234 2d30 342d 3139  te': '2024-04-19
-00001720: 272c 2027 7469 6d65 273a 2027 3137 3a33  ', 'time': '17:3
-00001730: 3027 2c20 2774 6561 6d31 273a 2027 5442  0', 'team1': 'TB
-00001740: 4427 2c20 2774 6561 6d32 273a 2027 5442  D', 'team2': 'TB
-00001750: 4427 2c20 2774 315f 6964 273a 2030 2c20  D', 't1_id': 0, 
-00001760: 2774 325f 6964 273a 2030 7d2c 207b 2769  't2_id': 0}, {'i
-00001770: 6427 3a20 2732 3337 3037 3830 272c 2027  d': '2370780', '
-00001780: 6461 7465 273a 2027 3230 3234 2d30 342d  date': '2024-04-
-00001790: 3139 272c 2027 7469 6d65 273a 2027 3230  19', 'time': '20
-000017a0: 3a30 3027 2c20 2774 6561 6d31 273a 2027  :00', 'team1': '
-000017b0: 5442 4427 2c20 2774 6561 6d32 273a 2027  TBD', 'team2': '
-000017c0: 5442 4427 2c20 2774 315f 6964 273a 2030  TBD', 't1_id': 0
-000017d0: 2c20 2774 325f 6964 273a 2030 7d2c 207b  , 't2_id': 0}, {
-000017e0: 2769 6427 3a20 2732 3337 3037 3831 272c  'id': '2370781',
-000017f0: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
-00001800: 342d 3139 272c 2027 7469 6d65 273a 2027  4-19', 'time': '
-00001810: 3232 3a33 3027 2c20 2774 6561 6d31 273a  22:30', 'team1':
-00001820: 2027 5442 4427 2c20 2774 6561 6d32 273a   'TBD', 'team2':
-00001830: 2027 5442 4427 2c20 2774 315f 6964 273a   'TBD', 't1_id':
-00001840: 2030 2c20 2774 325f 6964 273a 2030 7d2c   0, 't2_id': 0},
-00001850: 207b 2769 6427 3a20 2732 3337 3037 3832   {'id': '2370782
-00001860: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
-00001870: 2d30 342d 3230 272c 2027 7469 6d65 273a  -04-20', 'time':
-00001880: 2027 3030 3a33 3027 2c20 2774 6561 6d31   '00:30', 'team1
-00001890: 273a 2027 5442 4427 2c20 2774 6561 6d32  ': 'TBD', 'team2
-000018a0: 273a 2027 5442 4427 2c20 2774 315f 6964  ': 'TBD', 't1_id
-000018b0: 273a 2030 2c20 2774 325f 6964 273a 2030  ': 0, 't2_id': 0
-000018c0: 7d2c 207b 2769 6427 3a20 2732 3337 3037  }, {'id': '23707
-000018d0: 3833 272c 2027 6461 7465 273a 2027 3230  83', 'date': '20
-000018e0: 3234 2d30 342d 3230 272c 2027 7469 6d65  24-04-20', 'time
-000018f0: 273a 2027 3135 3a30 3027 2c20 2774 6561  ': '15:00', 'tea
-00001900: 6d31 273a 2027 5442 4427 2c20 2774 6561  m1': 'TBD', 'tea
-00001910: 6d32 273a 2027 5442 4427 2c20 2774 315f  m2': 'TBD', 't1_
-00001920: 6964 273a 2030 2c20 2774 325f 6964 273a  id': 0, 't2_id':
-00001930: 2030 7d2c 207b 2769 6427 3a20 2732 3337   0}, {'id': '237
-00001940: 3037 3834 272c 2027 6461 7465 273a 2027  0784', 'date': '
-00001950: 3230 3234 2d30 342d 3230 272c 2027 7469  2024-04-20', 'ti
-00001960: 6d65 273a 2027 3138 3a30 3027 2c20 2774  me': '18:00', 't
-00001970: 6561 6d31 273a 2027 5442 4427 2c20 2774  eam1': 'TBD', 't
-00001980: 6561 6d32 273a 2027 5442 4427 2c20 2774  eam2': 'TBD', 't
-00001990: 315f 6964 273a 2030 2c20 2774 325f 6964  1_id': 0, 't2_id
-000019a0: 273a 2030 7d5d 0d0a 2020 0d0a 2020 2020  ': 0}]..  ..    
-000019b0: 6060 600d 0a0d 0a2a 202a 2a67 6574 5f65  ```....* **get_e
-000019c0: 7665 6e74 5f69 6e66 6f28 6576 656e 745f  vent_info(event_
-000019d0: 6964 3a20 7374 7220 7c20 696e 742c 2065  id: str | int, e
-000019e0: 7665 6e74 5f74 6974 6c65 3a20 7374 7229  vent_title: str)
-000019f0: 202d 3e20 2865 7665 6e74 5f69 642c 2065   -> (event_id, e
-00001a00: 7665 6e74 5f74 6974 6c65 2c20 6576 656e  vent_title, even
-00001a10: 745f 7374 6172 742c 2065 7665 6e74 5f65  t_start, event_e
-00001a20: 6e64 2c20 7072 697a 652c 2074 6561 6d5f  nd, prize, team_
-00001a30: 6e75 6d2c 206c 6f63 6174 696f 6e2c 2067  num, location, g
-00001a40: 726f 7570 7329 2a2a 0d0a 0d0a 2020 2020  roups)**....    
-00001a50: 6060 600d 0a20 2020 2061 7761 6974 2068  ```..    await h
-00001a60: 6c74 762e 6765 745f 6576 656e 745f 696e  ltv.get_event_in
-00001a70: 666f 2837 3134 382c 2027 5047 4c20 4353  fo(7148, 'PGL CS
-00001a80: 3220 4d61 6a6f 7220 436f 7065 6e68 6167  2 Major Copenhag
-00001a90: 656e 3230 3234 2729 0d0a 2020 2020 0d0a  en2024')..    ..
-00001aa0: 2020 2020 7b27 6964 273a 2037 3134 382c      {'id': 7148,
-00001ab0: 2027 7469 746c 6527 3a20 2750 474c 2043   'title': 'PGL C
-00001ac0: 5332 204d 616a 6f72 2043 6f70 656e 6861  S2 Major Copenha
-00001ad0: 6765 6e32 3032 3427 2c20 2773 7461 7274  gen2024', 'start
-00001ae0: 273a 2027 3231 2d33 272c 2027 656e 6427  ': '21-3', 'end'
-00001af0: 3a20 2733 312d 3327 2c20 2770 7269 7a65  : '31-3', 'prize
-00001b00: 273a 2027 2431 2c32 3530 2c30 3030 272c  ': '$1,250,000',
-00001b10: 2027 7465 616d 7327 3a20 2731 3627 2c20   'teams': '16', 
-00001b20: 276c 6f63 6174 696f 6e27 3a20 2743 6f70  'location': 'Cop
-00001b30: 656e 6861 6765 6e2c 2044 656e 6d61 726b  enhagen, Denmark
-00001b40: 272c 2027 6772 6f75 7027 3a20 5b5d 7d0d  ', 'group': []}.
-00001b50: 0a20 2020 0d0a 2020 2020 6060 600d 0a0d  .   ..    ```...
-00001b60: 0a0d 0a2a 202a 2a67 6574 5f74 6f70 5f74  ...* **get_top_t
-00001b70: 6561 6d73 286d 6178 5f74 6561 6d73 3d33  eams(max_teams=3
-00001b80: 3029 202d 3e20 5b27 7261 6e6b 272c 2027  0) -> ['rank', '
-00001b90: 7469 746c 6527 2c20 2770 6f69 6e74 7327  title', 'points'
-00001ba0: 2c20 2763 6861 6e67 6527 2c20 2769 6427  , 'change', 'id'
-00001bb0: 5d2a 2a0d 0a0d 0a20 2020 2060 6060 0d0a  ]**....    ```..
-00001bc0: 2020 2020 6177 6169 7420 686c 7476 2e67      await hltv.g
-00001bd0: 6574 5f74 6f70 5f74 6561 6d73 2832 290d  et_top_teams(2).
-00001be0: 0a20 2020 200d 0a20 2020 203e 3e3e 5b7b  .    ..    >>>[{
-00001bf0: 2769 6427 3a20 2731 3131 3127 2c20 2772  'id': '1111', 'r
-00001c00: 616e 6b27 3a20 2731 272c 2027 7469 746c  ank': '1', 'titl
-00001c10: 6527 3a20 2746 615a 6527 2c20 2770 6f69  e': 'FaZe', 'poi
-00001c20: 6e74 7327 3a20 2739 3339 272c 2027 6368  nts': '939', 'ch
-00001c30: 616e 6765 273a 2027 2d27 2c20 2769 6427  ange': '-', 'id'
-00001c40: 3a20 2736 3636 3727 7d2c 207b 2769 6427  : '6667'}, {'id'
-00001c50: 3a20 2731 3131 3127 2c20 2772 616e 6b27  : '1111', 'rank'
-00001c60: 3a20 2732 272c 2027 7469 746c 6527 3a20  : '2', 'title': 
-00001c70: 274e 6174 7573 2056 696e 6365 7265 272c  'Natus Vincere',
-00001c80: 2027 706f 696e 7473 273a 2027 3735 3727   'points': '757'
-00001c90: 2c20 2763 6861 6e67 6527 3a20 272b 3427  , 'change': '+4'
-00001ca0: 2c20 2769 6427 3a20 2734 3630 3827 7d5d  , 'id': '4608'}]
-00001cb0: 0d0a 2020 2020 6060 600d 0a0d 0a2a 202a  ..    ```....* *
-00001cc0: 2a67 6574 5f74 6561 6d5f 696e 666f 2874  *get_team_info(t
-00001cd0: 6561 6d5f 6964 3a20 696e 7420 7c20 7374  eam_id: int | st
-00001ce0: 722c 2074 6974 6c65 3a20 7374 7229 202d  r, title: str) -
-00001cf0: 3e20 2874 6561 6d5f 6964 2c20 7465 616d  > (team_id, team
-00001d00: 5f74 6974 6c65 2c20 7261 6e6b 2c20 7b70  _title, rank, {p
-00001d10: 6c61 7965 723a 706c 6179 6572 5f69 647d  layer:player_id}
-00001d20: 2c20 636f 6163 682c 2061 7665 7261 6765  , coach, average
-00001d30: 5f61 6765 2c20 7765 656b 735f 696e 5f74  _age, weeks_in_t
-00001d40: 6f70 5f32 302c 206c 6173 745f 7472 6f70  op_20, last_trop
-00001d50: 6879 2c20 746f 7461 6c5f 7472 6f70 6879  hy, total_trophy
-00001d60: 7329 2a2a 0d0a 0d0a 2020 2020 6060 600d  s)**....    ```.
-00001d70: 0a20 2020 2061 7761 6974 2068 6c74 762e  .    await hltv.
-00001d80: 6765 745f 7465 616d 5f69 6e66 6f28 3636  get_team_info(66
-00001d90: 3637 2c20 2766 617a 6527 290d 0a20 2020  67, 'faze')..   
-00001da0: 200d 0a20 2020 203e 3e3e 2836 3636 372c   ..    >>>(6667,
-00001db0: 2027 6661 7a65 272c 2027 3127 2c20 5b27   'faze', '1', ['
-00001dc0: 6b61 7272 6967 616e 272c 2027 7261 696e  karrigan', 'rain
-00001dd0: 272c 2027 6672 6f7a 656e 272c 2027 726f  ', 'frozen', 'ro
-00001de0: 707a 272c 2027 6272 6f6b 7927 5d2c 2027  pz', 'broky'], '
-00001df0: 4e45 4f27 2c20 2732 362e 3627 2c20 2732  NEO', '26.6', '2
-00001e00: 3538 272c 2027 4945 4d20 4368 656e 6764  58', 'IEM Chengd
-00001e10: 7520 3230 3234 272c 2032 3229 0d0a 2020  u 2024', 22)..  
-00001e20: 2020 6060 600d 0a0d 0a2a 202a 2a67 6574    ```....* **get
-00001e30: 5f6c 6173 745f 6e65 7773 286d 6178 5f72  _last_news(max_r
-00001e40: 6567 5f6e 6577 733d 322c 206f 6e6c 795f  eg_news=2, only_
-00001e50: 746f 6461 793d 5472 7565 2c20 6f6e 6c79  today=True, only
-00001e60: 5f66 6561 7475 7265 643d 4661 6c73 6529  _featured=False)
-00001e70: 202d 3e20 5b64 6174 652c 205b 6665 6174   -> [date, [feat
-00001e80: 7572 6564 5f69 642c 2066 6561 7475 7265  ured_id, feature
-00001e90: 645f 7469 746c 652c 2066 6561 7475 7265  d_title, feature
-00001ea0: 645f 6465 7363 6970 7469 6f6e 5d2c 205b  d_desciption], [
-00001eb0: 7265 6775 6c61 725f 6964 2c20 7265 675f  regular_id, reg_
-00001ec0: 7469 746c 652c 2072 6567 5f74 696d 655d  title, reg_time]
-00001ed0: 5d2a 2a0d 0a0d 0a20 2020 2060 6060 0d0a  ]**....    ```..
-00001ee0: 2020 2020 6177 6169 7420 686c 7476 2e67      await hltv.g
-00001ef0: 6574 5f6c 6173 745f 6e65 7773 286f 6e6c  et_last_news(onl
-00001f00: 795f 746f 6461 793d 5472 7565 290d 0a20  y_today=True).. 
-00001f10: 2020 200d 0a20 2020 203e 3e3e 5b7b 2764     ..    >>>[{'d
-00001f20: 6174 6527 3a20 2731 352d 3034 272c 2027  ate': '15-04', '
-00001f30: 665f 6e65 7773 273a 205b 5d2c 2027 6e65  f_news': [], 'ne
-00001f40: 7773 273a 205b 7b27 6964 273a 2027 3338  ws': [{'id': '38
-00001f50: 3738 3427 2c20 2774 6974 6c65 273a 2027  784', 'title': '
-00001f60: 4d65 6469 613a 2046 5552 4941 2070 7261  Media: FURIA pra
-00001f70: 6374 6963 696e 6720 7769 7468 206b 7965  cticing with kye
-00001f80: 2069 6e20 706c 6163 6520 6f66 2061 7254   in place of arT
-00001f90: 272c 2027 706f 7374 6564 273a 2027 616e  ', 'posted': 'an
-00001fa0: 2068 6f75 7220 6167 6f27 7d2c 207b 2769   hour ago'}, {'i
-00001fb0: 6427 3a20 2733 3837 3833 272c 2027 7469  d': '38783', 'ti
-00001fc0: 746c 6527 3a20 2765 6c65 6374 726f 4e69  tle': 'electroNi
-00001fd0: 6320 746f 2070 6c61 7920 666f 7220 5669  c to play for Vi
-00001fe0: 7274 7573 2e70 726f 2061 7420 4553 4c20  rtus.pro at ESL 
-00001ff0: 5072 6f20 4c65 6167 7565 2053 3139 272c  Pro League S19',
-00002000: 2027 706f 7374 6564 273a 2027 3220 686f   'posted': '2 ho
-00002010: 7572 7320 6167 6f27 7d2c 207b 2769 6427  urs ago'}, {'id'
-00002020: 3a20 2733 3837 3831 272c 2027 7469 746c  : '38781', 'titl
-00002030: 6527 3a20 2754 6865 2045 5650 7320 616e  e': 'The EVPs an
-00002040: 6420 4265 7374 2046 6976 6520 6f66 2049  d Best Five of I
-00002050: 454d 2043 6865 6e67 6475 272c 2027 706f  EM Chengdu', 'po
-00002060: 7374 6564 273a 2027 3720 686f 7572 7320  sted': '7 hours 
-00002070: 6167 6f27 7d5d 7d5d 0d0a 2020 0d0a 2020  ago'}]}]..  ..  
-00002080: 2020 6060 600d 0a0d 0a2a 202a 2a67 6574    ```....* **get
-00002090: 5f62 6573 745f 706c 6179 6572 7328 746f  _best_players(to
-000020a0: 703a 2069 6e74 203d 2034 3029 202d 3e20  p: int = 40) -> 
-000020b0: 2827 7261 6e6b 272c 2027 6e61 6d65 272c  ('rank', 'name',
-000020c0: 2027 7465 616d 272c 2027 6d61 7073 272c   'team', 'maps',
-000020d0: 2027 7261 7469 6e67 2729 2a2a 0d0a 0d0a   'rating')**....
-000020e0: 2020 2020 6060 600d 0a20 2020 2061 7761      ```..    awa
-000020f0: 6974 2068 6c74 762e 6765 745f 6265 7374  it hltv.get_best
-00002100: 5f70 6c61 7965 7273 2832 290d 0a20 2020  _players(2)..   
-00002110: 200d 0a20 2020 203e 3e3e 5b7b 2769 6427   ..    >>>[{'id'
-00002120: 3a20 2731 3932 3330 272c 2027 7261 6e6b  : '19230', 'rank
-00002130: 273a 2031 2c20 276e 616d 6527 3a20 276d  ': 1, 'name': 'm
-00002140: 304e 4553 5927 2c20 2774 6561 6d27 3a20  0NESY', 'team': 
-00002150: 2747 3227 2c20 276d 6170 7327 3a20 2734  'G2', 'maps': '4
-00002160: 3427 2c20 2772 6174 696e 6727 3a20 2731  4', 'rating': '1
-00002170: 2e33 3727 7d2c 207b 2769 6427 3a20 2731  .37'}, {'id': '1
-00002180: 3830 3533 272c 2027 7261 6e6b 273a 2032  8053', 'rank': 2
-00002190: 2c20 276e 616d 6527 3a20 2762 726f 6b79  , 'name': 'broky
-000021a0: 272c 2027 7465 616d 273a 2027 4661 5a65  ', 'team': 'FaZe
-000021b0: 272c 2027 6d61 7073 273a 2027 3534 272c  ', 'maps': '54',
-000021c0: 2027 7261 7469 6e67 273a 2027 312e 3139   'rating': '1.19
-000021d0: 277d 5d0d 0a20 2020 2060 6060 0d0a 0d0a  '}]..    ```....
-000021e0: 2a20 2a2a 6765 745f 706c 6179 6572 5f69  * **get_player_i
-000021f0: 6e66 6f28 6964 3a20 7374 7220 7c20 696e  nfo(id: str | in
-00002200: 742c 206e 6963 6b6e 616d 653a 2073 7472  t, nickname: str
-00002210: 292a 2a0d 0a20 200d 0a20 2060 6060 0d0a  )**..  ..  ```..
-00002220: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
-00002230: 5f70 6c61 7965 725f 696e 666f 2837 3939  _player_info(799
-00002240: 382c 2027 7331 6d70 6c65 2729 0d0a 2020  8, 's1mple')..  
-00002250: 0d0a 2020 7b27 6964 273a 2037 3939 382c  ..  {'id': 7998,
-00002260: 2027 6e69 636b 6e61 6d65 273a 2027 7331   'nickname': 's1
-00002270: 6d70 6c65 272c 2027 7465 616d 273a 2027  mple', 'team': '
-00002280: 4e61 7475 7320 5669 6e63 6572 6527 2c20  Natus Vincere', 
-00002290: 2774 6561 6d5f 6964 273a 2034 3630 382c  'team_id': 4608,
-000022a0: 2027 6e61 6d65 273a 2027 4f6c 656b 7361   'name': 'Oleksa
-000022b0: 6e64 7220 4b6f 7374 796c 6965 7627 2c20  ndr Kostyliev', 
-000022c0: 276e 6174 696f 6e61 6c69 7479 273a 2027  'nationality': '
-000022d0: 556b 7261 696e 6527 2c20 2761 6765 273a  Ukraine', 'age':
-000022e0: 2032 362c 2027 7261 7469 6e67 273a 2027   26, 'rating': '
-000022f0: 302e 3934 272c 2027 6b70 7227 3a20 2730  0.94', 'kpr': '0
-00002300: 2e36 3027 2c20 2768 7327 3a20 2735 372e  .60', 'hs': '57.
-00002310: 3925 272c 2027 6c61 7374 5f6d 6174 6368  9%', 'last_match
-00002320: 6573 273a 205b 3130 3330 3539 2c20 3939  es': [103059, 99
-00002330: 3734 352c 2039 3937 3238 2c20 3939 3639  745, 99728, 9969
-00002340: 362c 2039 3934 3731 2c20 3939 3336 345d  6, 99471, 99364]
-00002350: 2c20 276c 6173 745f 7472 6f70 6879 273a  , 'last_trophy':
-00002360: 2027 424c 4153 5420 5072 656d 6965 7220   'BLAST Premier 
-00002370: 5370 7269 6e67 2046 696e 616c 2032 3032  Spring Final 202
-00002380: 3227 2c20 2774 6f74 616c 5f74 726f 7068  2', 'total_troph
-00002390: 6965 7327 3a20 3330 2c20 2774 6f74 616c  ies': 30, 'total
-000023a0: 5f6d 7670 7327 3a20 3231 7d0d 0a20 2060  _mvps': 21}..  `
-000023b0: 6060 0d0a 0d0a 2a20 2a2a 6765 7428 7479  ``....* **get(ty
-000023c0: 7065 3a20 7374 722c 2069 643a 2069 6e74  pe: str, id: int
-000023d0: 207c 2073 7472 207c 204e 6f6e 6520 3d20   | str | None = 
-000023e0: 4e6f 6e65 2c20 7469 746c 653a 2073 7472  None, title: str
-000023f0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c20   | None = None, 
-00002400: 7465 616d 313a 2073 7472 207c 204e 6f6e  team1: str | Non
-00002410: 6520 3d20 4e6f 6e65 2c20 7465 616d 323a  e = None, team2:
-00002420: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
-00002430: 6e65 293a 2a2a 0d0a 2020 2842 4554 4129  ne):**..  (BETA)
-00002440: 2054 6869 7320 6d65 7468 6f64 2069 7320   This method is 
-00002450: 6e6f 7420 6669 6e69 7368 6564 2e20 506f  not finished. Po
-00002460: 7373 6962 6c65 2074 7970 6573 2027 6576  ssible types 'ev
-00002470: 656e 7473 272c 2027 6d61 7463 6865 7327  ents', 'matches'
-00002480: 2c20 2774 6561 6d73 272c 2061 6c73 6f20  , 'teams', also 
-00002490: 7520 6361 6e20 6164 6420 6964 207c 2074  u can add id | t
-000024a0: 6974 6c65 207c 2074 6561 6d31 207c 2074  itle | team1 | t
-000024b0: 6561 6d32 2c20 746f 2070 6172 7365 206d  eam2, to parse m
-000024c0: 6f72 652e 0d0a 2020 0d0a 2020 6060 600d  ore...  ..  ```.
-000024d0: 0a20 200d 0a20 2061 7761 6974 2068 6c74  .  ..  await hlt
-000024e0: 762e 6765 7428 276d 6174 6368 6573 272c  v.get('matches',
-000024f0: 2032 3337 3132 3031 2c20 2772 6573 2d72   2371201, 'res-r
-00002500: 6567 696f 6e61 6c2d 7365 7269 6573 2d33  egional-series-3
-00002510: 2d6c 6174 616d 272c 2027 494d 5045 5249  -latam', 'IMPERI
-00002520: 414c 272c 2027 4d49 4252 2729 0d0a 2020  AL', 'MIBR')..  
-00002530: 0d0a 2020 3e3e 3e20 2832 3337 3132 3031  ..  >>> (2371201
-00002540: 2c20 302c 2030 2c20 274c 4956 4527 2c20  , 0, 0, 'LIVE', 
-00002550: 5b7b 276d 6170 6e61 6d65 273a 2027 5665  [{'mapname': 'Ve
-00002560: 7274 6967 6f27 2c20 2772 5f74 6561 6d31  rtigo', 'r_team1
-00002570: 273a 2027 3627 2c20 2772 5f74 6561 6d32  ': '6', 'r_team2
-00002580: 273a 2027 3133 277d 2c20 7b27 6d61 706e  ': '13'}, {'mapn
-00002590: 616d 6527 3a20 274d 6972 6167 6527 2c20  ame': 'Mirage', 
-000025a0: 2772 5f74 6561 6d31 273a 2027 2d27 2c20  'r_team1': '-', 
-000025b0: 2772 5f74 6561 6d32 273a 2027 2d27 7d2c  'r_team2': '-'},
-000025c0: 207b 276d 6170 6e61 6d65 273a 2027 416e   {'mapname': 'An
-000025d0: 7562 6973 272c 2027 725f 7465 616d 3127  ubis', 'r_team1'
-000025e0: 3a20 272d 272c 2027 725f 7465 616d 3227  : '-', 'r_team2'
-000025f0: 3a20 272d 277d 5d2c 205b 5d29 0d0a 2020  : '-'}], [])..  
-00002600: 0d0a 2020 6060 600d 0a2d 2d2d 0d0a 2320  ..  ```..---..# 
-00002610: 436f 6e66 6967 730d 0a0d 0a2a 206d 6178  Configs....* max
-00002620: 5f64 656c 6179 3a20 696e 7420 3d20 3135  _delay: int = 15
-00002630: 0d0a 0d0a 2020 2020 4175 746f 6d61 7469  ....    Automati
-00002640: 6361 6c6c 7920 696e 6372 6561 7369 6e67  cally increasing
-00002650: 2072 6563 6f6e 6e65 6374 696e 6720 6465   reconnecting de
-00002660: 6c61 7920 6279 2031 2073 6563 2074 6f20  lay by 1 sec to 
-00002670: 6d61 785f 6465 6c61 7920 2866 726f 6d20  max_delay (from 
-00002680: 3173 2074 6f20 3573 290d 0a0d 0a20 2020  1s to 5s)....   
-00002690: 2060 6060 0d0a 2020 2020 686c 7476 203d   ```..    hltv =
-000026a0: 2048 6c74 7628 6d61 785f 6465 6c61 793d   Hltv(max_delay=
-000026b0: 3529 0d0a 2020 2020 0d0a 2020 2020 3e3e  5)..    ..    >>
-000026c0: 3e46 6574 6368 696e 6720 6874 7470 733a  >Fetching https:
-000026d0: 2f2f 7777 772e 686c 7476 2e6f 7267 2f6d  //www.hltv.org/m
-000026e0: 6174 6368 6573 2f32 3337 3037 3237 2f66  atches/2370727/f
-000026f0: 617a 652d 7673 2d6e 6174 7573 2d76 696e  aze-vs-natus-vin
-00002700: 6365 7265 2d70 676c 2d63 7332 2d6d 616a  cere-pgl-cs2-maj
-00002710: 6f72 2d63 6f70 656e 6861 6765 6e2d 3230  or-copenhagen-20
-00002720: 3234 2c20 636f 6465 3a20 3430 330d 0a20  24, code: 403.. 
-00002730: 2020 203e 3e3e 476f 7420 3430 3320 666f     >>>Got 403 fo
-00002740: 7262 6974 7465 6e0d 0a20 2020 203e 3e3e  rbitten..    >>>
-00002750: 4361 6c6c 696e 6720 6167 6169 6e2c 2069  Calling again, i
-00002760: 6e63 7265 6173 696e 6720 6465 6c61 7920  ncreasing delay 
-00002770: 746f 2034 730d 0a20 2020 203e 3e3e 4665  to 4s..    >>>Fe
-00002780: 7463 6869 6e67 2068 7474 7073 3a2f 2f77  tching https://w
-00002790: 7777 2e68 6c74 762e 6f72 672f 6d61 7463  ww.hltv.org/matc
-000027a0: 6865 732f 3233 3730 3732 372f 6661 7a65  hes/2370727/faze
-000027b0: 2d76 732d 6e61 7475 732d 7669 6e63 6572  -vs-natus-vincer
-000027c0: 652d 7067 6c2d 6373 322d 6d61 6a6f 722d  e-pgl-cs2-major-
-000027d0: 636f 7065 6e68 6167 656e 2d32 3032 342c  copenhagen-2024,
-000027e0: 2063 6f64 653a 2034 3033 0d0a 2020 2020   code: 403..    
-000027f0: 3e3e 3e47 6f74 2034 3033 2066 6f72 6269  >>>Got 403 forbi
-00002800: 7474 656e 0d0a 2020 2020 3e3e 3e43 616c  tten..    >>>Cal
-00002810: 6c69 6e67 2061 6761 696e 2c20 696e 6372  ling again, incr
-00002820: 6561 7369 6e67 2064 656c 6179 2074 6f20  easing delay to 
-00002830: 3573 0d0a 2020 2020 6060 600d 0a0d 0a2a  5s..    ```....*
-00002840: 206d 6178 5f72 6574 7269 6573 3a20 696e   max_retries: in
-00002850: 7420 3d20 300d 0a0d 0a20 2020 204d 6178  t = 0....    Max
-00002860: 2072 6574 7269 6573 2e20 3020 6f72 202d   retries. 0 or -
-00002870: 3120 666f 7220 696e 6669 6e69 7479 2074  1 for infinity t
-00002880: 7269 6573 2e0d 0a20 2020 200d 0a20 2020  ries...    ..   
-00002890: 2060 6060 0d0a 2020 2020 686c 7476 203d   ```..    hltv =
-000028a0: 2048 6c74 7628 6d61 785f 7265 7472 6965   Hltv(max_retrie
-000028b0: 733d 322c 2064 6562 7567 3d54 7275 6529  s=2, debug=True)
-000028c0: 0d0a 2020 2020 7072 696e 7428 6177 6169  ..    print(awai
-000028d0: 7420 686c 7476 2e67 6574 5f62 6573 745f  t hltv.get_best_
-000028e0: 706c 6179 6572 7328 2929 0d0a 2020 2020  players())..    
-000028f0: 0d0a 2020 2020 4372 6561 7469 6e67 2053  ..    Creating S
-00002900: 6573 7369 6f6e 0d0a 2020 2020 5472 7969  ession..    Tryi
-00002910: 6e67 2063 6f6e 6e65 6374 2074 6f20 6874  ng connect to ht
-00002920: 7470 733a 2f2f 7777 772e 686c 7476 2e6f  tps://www.hltv.o
-00002930: 7267 2f73 7461 7473 2f70 6c61 7965 7273  rg/stats/players
-00002940: 3f73 7461 7274 4461 7465 3d32 3032 342d  ?startDate=2024-
-00002950: 3031 2d30 3126 656e 6444 6174 653d 3230  01-01&endDate=20
-00002960: 3234 2d31 322d 3331 2672 616e 6b69 6e67  24-12-31&ranking
-00002970: 4669 6c74 6572 3d54 6f70 3230 2c20 7472  Filter=Top20, tr
-00002980: 7920 312f 320d 0a20 2020 2054 7279 696e  y 1/2..    Tryin
-00002990: 6720 636f 6e6e 6563 7420 746f 2068 7474  g connect to htt
-000029a0: 7073 3a2f 2f77 7777 2e68 6c74 762e 6f72  ps://www.hltv.or
-000029b0: 672f 7374 6174 732f 706c 6179 6572 733f  g/stats/players?
-000029c0: 7374 6172 7444 6174 653d 3230 3234 2d30  startDate=2024-0
-000029d0: 312d 3031 2665 6e64 4461 7465 3d32 3032  1-01&endDate=202
-000029e0: 342d 3132 2d33 3126 7261 6e6b 696e 6746  4-12-31&rankingF
-000029f0: 696c 7465 723d 546f 7032 302c 2074 7279  ilter=Top20, try
-00002a00: 2032 2f32 0d0a 2020 2020 436f 6e6e 6563   2/2..    Connec
-00002a10: 7469 6f6e 2066 6169 6c65 640d 0a20 2020  tion failed..   
-00002a20: 2060 6060 0d0a 0d0a 2a20 7072 6f78 795f   ```....* proxy_
-00002a30: 6c69 7374 3a20 6c69 7374 207c 204e 6f6e  list: list | Non
-00002a40: 6520 3d20 4e6f 6e65 0d0a 0d0a 2020 2020  e = None....    
-00002a50: 6c69 7374 206f 6620 796f 7572 2070 726f  list of your pro
-00002a60: 7869 6573 2c20 6966 2079 6f75 7220 7072  xies, if your pr
-00002a70: 6f78 6965 7320 646f 6573 6e74 2068 6176  oxies doesnt hav
-00002a80: 6520 616e 7920 7072 6f74 6f63 6f6c 2079  e any protocol y
-00002a90: 6f75 2063 616e 2075 7365 2070 726f 7879  ou can use proxy
-00002aa0: 5f70 726f 746f 636f 6c2e 0d0a 2020 2020  _protocol...    
-00002ab0: 4e6f 7465 3a20 546f 2061 6464 206e 6f6e  Note: To add non
-00002ac0: 7072 6f78 7920 746f 206c 6973 7420 6a75  proxy to list ju
-00002ad0: 7374 2070 7574 2027 2720 746f 2069 742c  st put '' to it,
-00002ae0: 2079 6f75 2063 616e 2066 696e 6420 6578   you can find ex
-00002af0: 616d 706c 6520 7769 7468 2061 720d 0a0d  ample with ar...
-00002b00: 0a2a 2070 726f 7879 5f70 6174 683a 2073  .* proxy_path: s
-00002b10: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
-00002b20: 0d0a 0d0a 2020 2020 5061 7468 2074 6f20  ....    Path to 
-00002b30: 796f 7572 2070 726f 7879 2028 7072 6f78  your proxy (prox
-00002b40: 795f 6c69 7374 2077 696c 6c20 6265 2069  y_list will be i
-00002b50: 676e 6f72 6564 292e 2049 6620 796f 7572  gnored). If your
-00002b60: 2070 726f 7869 6573 2064 6f65 736e 7420   proxies doesnt 
-00002b70: 6861 7665 2061 6e79 2070 726f 746f 636f  have any protoco
-00002b80: 6c20 796f 7520 6361 6e20 7573 6520 7072  l you can use pr
-00002b90: 6f78 795f 7072 6f74 6f63 6f6c 0d0a 0d0a  oxy_protocol....
-00002ba0: 2a20 7072 6f78 795f 7072 6f74 6f63 6f6c  * proxy_protocol
-00002bb0: 3a20 7374 7220 7c20 4e6f 6e65 203d 204e  : str | None = N
-00002bc0: 6f6e 652c 0d0a 0d0a 2020 2020 5072 6f78  one,....    Prox
-00002bd0: 7920 7072 6f74 6f63 6f6c 2e20 596f 7572  y protocol. Your
-00002be0: 2070 726f 7869 6573 2060 6060 686c 7476   proxies ```hltv
-00002bf0: 203d 2048 6c74 7628 7072 6f78 795f 7072   = Hltv(proxy_pr
-00002c00: 6f74 6f63 6f6c 3d27 6874 7470 2720 2e2e  otocol='http' ..
-00002c10: 2e29 202d 3e20 2731 312e 3131 2e31 312e  .) -> '11.11.11.
-00002c20: 3131 3a31 3131 3127 202d 3e20 2768 7474  11:1111' -> 'htt
-00002c30: 703a 2f2f 3131 2e31 312e 3131 2e31 313a  p://11.11.11.11:
-00002c40: 3131 3131 270d 0a0d 0a2a 2064 656c 6574  1111'....* delet
-00002c50: 655f 7072 6f78 793a 2062 6f6f 6c20 3d20  e_proxy: bool = 
-00002c60: 4661 6c73 650d 0a0d 0a20 2020 2052 656d  False....    Rem
-00002c70: 6f76 6573 2070 726f 7879 2066 726f 6d20  oves proxy from 
-00002c80: 6c69 7374 2028 7072 6f78 795f 7061 7468  list (proxy_path
-00002c90: 2069 6e63 6c75 6465 6429 2069 6620 636f   included) if co
-00002ca0: 6e6e 6563 7469 6f6e 2075 6e73 7563 6365  nnection unsucce
-00002cb0: 7373 6675 6c6c 790d 0a0d 0a2a 2074 696d  ssfully....* tim
-00002cc0: 656f 7574 3a20 696e 7420 3d20 350d 0a0d  eout: int = 5...
-00002cd0: 0a20 2020 204d 6178 2074 696d 6520 746f  .    Max time to
-00002ce0: 2063 6c6f 7365 2063 6f6e 6e65 6374 696f   close connectio
-00002cf0: 6e2e 2052 6563 6f6d 6d65 6e64 6564 2074  n. Recommended t
-00002d00: 6f20 7573 6520 7469 6d65 6f75 743d 3120  o use timeout=1 
-00002d10: 6966 2079 6f75 2061 7265 2075 7369 6e67  if you are using
-00002d20: 2072 616e 646f 6d20 7072 6f78 6965 732e   random proxies.
-00002d30: 0d0a 0d0a 2a20 6465 6275 673a 2062 6f6f  ....* debug: boo
-00002d40: 6c20 3d20 4661 6c73 650d 0a0d 0a2a 2074  l = False....* t
-00002d50: 7a3a 2073 7472 203d 2027 4575 726f 7065  z: str = 'Europe
-00002d60: 2f43 6f70 656e 6861 6765 6e27 3a0d 0a20  /Copenhagen':.. 
-00002d70: 2020 200d 0a20 2020 2054 696d 657a 6f6e     ..    Timezon
-00002d80: 6520 636f 6e66 6967 2e20 0d0a 200d 0a20  e config. .. .. 
-00002d90: 2020 203c 6120 6872 6566 3d27 6874 7470     <a href='http
-00002da0: 733a 2f2f 6769 7374 2e67 6974 6875 622e  s://gist.github.
-00002db0: 636f 6d2f 6865 7961 6c65 7865 6a2f 3862  com/heyalexej/8b
-00002dc0: 6636 3838 6664 3637 6437 3139 3962 6534  f688fd67d7199be4
-00002dd0: 6131 3638 3262 3365 6563 3735 3638 273e  a1682b3eec7568'>
-00002de0: 5461 7020 6865 7265 203c 2f61 3e20 746f  Tap here </a> to
-00002df0: 2073 6565 2061 6c6c 2061 7661 696c 6162   see all availab
-00002e00: 6c65 2074 696d 657a 6f6e 6573 0d0a 0d0a  le timezones....
-00002e10: 0d0a 2d2d 2d0d 0a23 2045 7861 6d70 6c65  ..---..# Example
-00002e20: 730d 0a0d 0a2a 2a2a 2a53 696d 706c 6520  s....****Simple 
-00002e30: 4578 616d 706c 652a 2a2a 2a0d 0a0d 0a60  Example****....`
-00002e40: 6060 0d0a 6672 6f6d 2068 6c74 765f 6173  ``..from hltv_as
-00002e50: 796e 635f 6170 6920 696d 706f 7274 2048  ync_api import H
-00002e60: 6c74 760d 0a0d 0a0d 0a61 7379 6e63 2064  ltv......async d
-00002e70: 6566 2074 6573 7428 293a 0d0a 0d0a 2020  ef test():....  
-00002e80: 2020 6173 796e 6320 7769 7468 2048 6c74    async with Hlt
-00002e90: 7628 2920 6173 2068 6c74 763a 0d0a 2020  v() as hltv:..  
-00002ea0: 2020 2020 7072 696e 7428 6177 6169 7420      print(await 
-00002eb0: 686c 7476 2e67 6574 5f65 7665 6e74 5f69  hltv.get_event_i
-00002ec0: 6e66 6f28 3731 3438 2c20 2770 676c 2d63  nfo(7148, 'pgl-c
-00002ed0: 7332 2d6d 616a 6f72 2d63 6f70 656e 6861  s2-major-copenha
-00002ee0: 6765 6e2d 3230 3234 2729 290d 0a0d 0a69  gen-2024'))....i
-00002ef0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
-00002f00: 5f6d 6169 6e5f 5f22 3a0d 0a20 2020 2061  _main__":..    a
-00002f10: 7379 6e63 696f 2e72 756e 2874 6573 7428  syncio.run(test(
-00002f20: 2929 0d0a 6060 600d 0a0d 0a2a 2a2a 2a50  ))..```....****P
-00002f30: 726f 7879 2050 6172 7365 722a 2a2a 2a0d  roxy Parser****.
-00002f40: 0a0d 0a60 6060 0d0a 6672 6f6d 2068 6c74  ...```..from hlt
-00002f50: 765f 6173 796e 635f 6170 6920 696d 706f  v_async_api impo
-00002f60: 7274 2048 6c74 760d 0a0d 0a0d 0a61 7379  rt Hltv......asy
-00002f70: 6e63 2064 6566 2074 6573 7428 293a 0d0a  nc def test():..
-00002f80: 0d0a 2020 2020 686c 7476 203d 2048 6c74  ..    hltv = Hlt
-00002f90: 7628 6465 6275 673d 5472 7565 2c20 7072  v(debug=True, pr
-00002fa0: 6f78 795f 7061 7468 3d27 7072 6f78 795f  oxy_path='proxy_
-00002fb0: 7465 7374 2e74 7874 272c 2074 696d 656f  test.txt', timeo
-00002fc0: 7574 3d31 2c20 6465 6c65 7465 5f70 726f  ut=1, delete_pro
-00002fd0: 7879 3d54 7275 652c 2070 726f 7879 5f70  xy=True, proxy_p
-00002fe0: 726f 746f 636f 6c3d 2768 7474 7027 290d  rotocol='http').
-00002ff0: 0a20 2020 200d 0a20 2020 2070 7269 6e74  .    ..    print
-00003000: 2861 7761 6974 2068 6c74 762e 6765 745f  (await hltv.get_
-00003010: 6576 656e 745f 696e 666f 2837 3134 382c  event_info(7148,
-00003020: 2027 7067 6c2d 6373 322d 6d61 6a6f 722d   'pgl-cs2-major-
-00003030: 636f 7065 6e68 6167 656e 2d32 3032 3427  copenhagen-2024'
-00003040: 2929 0d0a 0d0a 6966 205f 5f6e 616d 655f  ))....if __name_
-00003050: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
-00003060: 0d0a 2020 2020 6173 796e 6369 6f2e 7275  ..    asyncio.ru
-00003070: 6e28 7465 7374 2829 290d 0a60 6060 0d0a  n(test())..```..
-00003080: 0d0a 2a2a 2a2a 4175 746f 6d61 7469 6320  ..****Automatic 
-00003090: 7061 7273 6572 2077 6974 6820 6172 7120  parser with arq 
-000030a0: 616e 6420 7265 6469 732a 2a2a 2a0d 0a0d  and redis****...
-000030b0: 0a2d 2074 6f20 7275 6e20 7479 7065 2022  .- to run type "
-000030c0: 6172 7120 5041 5448 5f54 4f5f 4649 4c45  arq PATH_TO_FILE
-000030d0: 2e57 6f72 6b65 7253 6574 7469 6e67 7322  .WorkerSettings"
-000030e0: 0d0a 0d0a 2020 2020 6060 600d 0a20 2020  ....    ```..   
-000030f0: 2069 6d70 6f72 7420 756a 736f 6e0d 0a20   import ujson.. 
-00003100: 2020 2069 6d70 6f72 7420 6173 796e 6369     import asynci
-00003110: 6f0d 0a20 2020 2066 726f 6d20 6172 7120  o..    from arq 
-00003120: 696d 706f 7274 2063 726f 6e0d 0a20 2020  import cron..   
-00003130: 2066 726f 6d20 7265 6469 732e 6173 796e   from redis.asyn
-00003140: 6369 6f20 696d 706f 7274 2052 6564 6973  cio import Redis
-00003150: 2c20 436f 6e6e 6563 7469 6f6e 506f 6f6c  , ConnectionPool
-00003160: 0d0a 2020 2020 0d0a 2020 2020 6672 6f6d  ..    ..    from
-00003170: 2068 6c74 765f 6173 796e 635f 6170 6920   hltv_async_api 
-00003180: 696d 706f 7274 2048 6c74 760d 0a20 2020  import Hltv..   
-00003190: 200d 0a20 2020 200d 0a20 2020 200d 0a20   ..    ..    .. 
-000031a0: 2020 2061 7379 6e63 2064 6566 2073 7461     async def sta
-000031b0: 7274 7570 2863 7478 293a 0d0a 2020 2020  rtup(ctx):..    
-000031c0: 2020 2020 6173 796e 6320 7769 7468 2048      async with H
-000031d0: 6c74 7628 6d61 785f 6465 6c61 793d 352c  ltv(max_delay=5,
-000031e0: 2070 726f 7879 5f70 6174 683d 2770 726f   proxy_path='pro
-000031f0: 7869 6573 2e74 7874 272c 2064 6562 7567  xies.txt', debug
-00003200: 3d54 7275 6529 2061 7320 686c 7476 3a0d  =True) as hltv:.
-00003210: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
-00003220: 7478 5b22 686c 7476 225d 203d 2068 6c74  tx["hltv"] = hlt
-00003230: 760d 0a20 200d 0a20 2020 2020 2020 2063  v..  ..        c
-00003240: 7478 5b22 7265 6469 7322 5d20 3d20 7265  tx["redis"] = re
-00003250: 6469 735f 636c 6965 6e74 203d 2052 6564  dis_client = Red
-00003260: 6973 280d 0a20 2020 2020 2020 2020 2020  is(..           
-00003270: 2063 6f6e 6e65 6374 696f 6e5f 706f 6f6c   connection_pool
-00003280: 3d43 6f6e 6e65 6374 696f 6e50 6f6f 6c2e  =ConnectionPool.
-00003290: 6672 6f6d 5f75 726c 2873 6574 7469 6e67  from_url(setting
-000032a0: 732e 7265 6469 735f 7572 6c29 290d 0a20  s.redis_url)).. 
-000032b0: 2020 2020 2020 206c 6f67 6765 722e 7375         logger.su
-000032c0: 6363 6573 7328 6622 5363 6865 6475 6c65  ccess(f"Schedule
-000032d0: 7220 7374 6172 7465 642e 2055 5443 2074  r started. UTC t
-000032e0: 696d 6520 7b64 6174 6574 696d 652e 7574  ime {datetime.ut
-000032f0: 636e 6f77 2829 7d22 290d 0a20 2020 200d  cnow()}")..    .
-00003300: 0a20 2020 200d 0a20 2020 2061 7379 6e63  .    ..    async
-00003310: 2064 6566 2073 6875 7464 6f77 6e28 6374   def shutdown(ct
-00003320: 7829 3a0d 0a20 2020 2020 2020 2061 7761  x):..        awa
-00003330: 6974 2063 7478 5b22 7265 6469 7322 5d2e  it ctx["redis"].
-00003340: 636c 6f73 6528 290d 0a20 2020 200d 0a20  close()..    .. 
-00003350: 2020 200d 0a20 2020 2061 7379 6e63 2064     ..    async d
-00003360: 6566 2070 6172 7365 5f6d 6174 6368 6573  ef parse_matches
-00003370: 2863 7478 293a 0d0a 2020 2020 2020 2020  (ctx):..        
-00003380: 686c 7476 203d 2063 7478 5b22 686c 7476  hltv = ctx["hltv
-00003390: 225d 0d0a 2020 2020 2020 2020 7265 6469  "]..        redi
-000033a0: 7320 3d20 6374 785b 2272 6564 6973 225d  s = ctx["redis"]
-000033b0: 0d0a 2020 2020 2020 2020 6d61 7463 6865  ..        matche
-000033c0: 7320 3d20 6177 6169 7420 686c 7476 2e67  s = await hltv.g
-000033d0: 6574 5f75 7063 6f6d 696e 675f 6d61 7463  et_upcoming_matc
-000033e0: 6865 7328 312c 2031 290d 0a20 2020 2020  hes(1, 1)..     
-000033f0: 2020 2069 6620 6d61 7463 6865 733a 0d0a     if matches:..
-00003400: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00003410: 7420 7265 6469 732e 7365 7428 226d 6174  t redis.set("mat
-00003420: 6368 6573 222c 2075 6a73 6f6e 2e64 756d  ches", ujson.dum
-00003430: 7073 286d 6174 6368 6573 2929 0d0a 2020  ps(matches))..  
-00003440: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00003450: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00003460: 6572 726f 7228 2265 7272 6f72 2070 6172  error("error par
-00003470: 7369 6e67 206d 6174 6368 6573 2229 0d0a  sing matches")..
-00003480: 2020 2020 0d0a 2020 2020 6173 796e 6320      ..    async 
-00003490: 6465 6620 7061 7273 655f 6576 656e 7473  def parse_events
-000034a0: 2863 7478 293a 0d0a 2020 2020 2020 2020  (ctx):..        
-000034b0: 686c 7476 203d 2063 7478 5b22 686c 7476  hltv = ctx["hltv
-000034c0: 225d 0d0a 2020 2020 2020 2020 7265 6469  "]..        redi
-000034d0: 7320 3d20 6374 785b 2272 6564 6973 225d  s = ctx["redis"]
-000034e0: 0d0a 2020 2020 2020 2020 6576 656e 7473  ..        events
-000034f0: 203d 2061 7761 6974 2068 6c74 762e 6765   = await hltv.ge
-00003500: 745f 6576 656e 7473 2829 0d0a 2020 2020  t_events()..    
-00003510: 2020 2020 6966 2065 7665 6e74 733a 0d0a      if events:..
-00003520: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00003530: 7420 7265 6469 732e 7365 7428 2265 7665  t redis.set("eve
-00003540: 6e74 7322 2c20 756a 736f 6e2e 6475 6d70  nts", ujson.dump
-00003550: 7328 6576 656e 7473 2929 0d0a 2020 2020  s(events))..    
-00003560: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00003570: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
-00003580: 726f 7228 2265 7272 6f72 2070 6172 7369  ror("error parsi
-00003590: 6e67 2065 7665 6e74 7322 290d 0a20 2020  ng events")..   
-000035a0: 200d 0a20 2020 200d 0a20 2020 2061 7379   ..    ..    asy
-000035b0: 6e63 2064 6566 2070 6172 7365 5f74 6f70  nc def parse_top
-000035c0: 5f74 6561 6d73 2863 7478 293a 0d0a 2020  _teams(ctx):..  
-000035d0: 2020 2020 2020 686c 7476 203d 2063 7478        hltv = ctx
-000035e0: 5b22 686c 7476 225d 0d0a 2020 2020 2020  ["hltv"]..      
-000035f0: 2020 7265 6469 7320 3d20 6374 785b 2272    redis = ctx["r
-00003600: 6564 6973 225d 0d0a 2020 2020 2020 2020  edis"]..        
-00003610: 746f 705f 7465 616d 7320 3d20 6177 6169  top_teams = awai
-00003620: 7420 686c 7476 2e67 6574 5f74 6f70 5f74  t hltv.get_top_t
-00003630: 6561 6d73 2833 3029 0d0a 2020 2020 2020  eams(30)..      
-00003640: 2020 6966 2074 6f70 5f74 6561 6d73 3a0d    if top_teams:.
-00003650: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-00003660: 6974 2072 6564 6973 2e73 6574 2822 746f  it redis.set("to
-00003670: 705f 7465 616d 7322 2c20 756a 736f 6e2e  p_teams", ujson.
-00003680: 6475 6d70 7328 746f 705f 7465 616d 7329  dumps(top_teams)
-00003690: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-000036a0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-000036b0: 6767 6572 2e65 7272 6f72 2822 6572 726f  gger.error("erro
-000036c0: 7220 7061 7273 696e 6720 746f 7020 7465  r parsing top te
-000036d0: 616d 7322 290d 0a20 2020 200d 0a20 2020  ams")..    ..   
-000036e0: 200d 0a20 2020 2061 7379 6e63 2064 6566   ..    async def
-000036f0: 2070 6172 7365 5f74 6f70 5f70 6c61 7965   parse_top_playe
-00003700: 7273 2863 7478 293a 0d0a 2020 2020 2020  rs(ctx):..      
-00003710: 2020 686c 7476 203d 2063 7478 5b22 686c    hltv = ctx["hl
-00003720: 7476 225d 0d0a 2020 2020 2020 2020 7265  tv"]..        re
-00003730: 6469 7320 3d20 6374 785b 2272 6564 6973  dis = ctx["redis
-00003740: 225d 0d0a 2020 2020 2020 2020 746f 705f  "]..        top_
-00003750: 706c 6179 6572 7320 3d20 6177 6169 7420  players = await 
-00003760: 686c 7476 2e67 6574 5f62 6573 745f 706c  hltv.get_best_pl
-00003770: 6179 6572 7328 3330 290d 0a20 2020 2020  ayers(30)..     
-00003780: 2020 2069 6620 746f 705f 706c 6179 6572     if top_player
-00003790: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000037a0: 6177 6169 7420 7265 6469 732e 7365 7428  await redis.set(
-000037b0: 2274 6f70 5f74 6561 6d73 222c 2075 6a73  "top_teams", ujs
-000037c0: 6f6e 2e64 756d 7073 2874 6f70 5f70 6c61  on.dumps(top_pla
-000037d0: 7965 7273 2929 0d0a 2020 2020 2020 2020  yers))..        
-000037e0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000037f0: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
-00003800: 2265 7272 6f72 2070 6172 7369 6e67 2074  "error parsing t
-00003810: 6f70 2070 6c61 7965 7273 2229 0d0a 2020  op players")..  
-00003820: 2020 0d0a 2020 2020 0d0a 2020 2020 6173    ..    ..    as
-00003830: 796e 6320 6465 6620 7061 7273 655f 6c61  ync def parse_la
-00003840: 7374 5f6e 6577 7328 6374 7829 3a0d 0a20  st_news(ctx):.. 
-00003850: 2020 2020 2020 2068 6c74 7620 3d20 6374         hltv = ct
-00003860: 785b 2268 6c74 7622 5d0d 0a20 2020 2020  x["hltv"]..     
-00003870: 2020 2072 6564 6973 203d 2063 7478 5b22     redis = ctx["
-00003880: 7265 6469 7322 5d0d 0a20 2020 2020 2020  redis"]..       
-00003890: 206e 6577 7320 3d20 6177 6169 7420 686c   news = await hl
-000038a0: 7476 2e67 6574 5f6c 6173 745f 6e65 7773  tv.get_last_news
-000038b0: 286f 6e6c 795f 746f 6461 793d 5472 7565  (only_today=True
-000038c0: 2c20 6d61 785f 7265 675f 6e65 7773 3d34  , max_reg_news=4
-000038d0: 290d 0a20 2020 2020 2020 2069 6620 6e65  )..        if ne
-000038e0: 7773 3a0d 0a20 2020 2020 2020 2020 2020  ws:..           
-000038f0: 2061 7761 6974 2072 6564 6973 2e73 6574   await redis.set
-00003900: 2822 6e65 7773 222c 2075 6a73 6f6e 2e64  ("news", ujson.d
-00003910: 756d 7073 286e 6577 7329 290d 0a20 2020  umps(news))..   
-00003920: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00003930: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00003940: 7272 6f72 2822 6572 726f 7220 7061 7273  rror("error pars
-00003950: 696e 6720 6e65 7773 2229 0d0a 2020 2020  ing news")..    
-00003960: 0d0a 2020 2020 0d0a 2020 2020 636c 6173  ..    ..    clas
-00003970: 7320 576f 726b 6572 5365 7474 696e 6773  s WorkerSettings
-00003980: 3a0d 0a20 2020 2020 2020 2072 6564 6973  :..        redis
-00003990: 5f73 6574 7469 6e67 7320 3d20 7365 7474  _settings = sett
-000039a0: 696e 6773 2e72 6564 6973 5f70 6f6f 6c0d  ings.redis_pool.
-000039b0: 0a20 2020 2020 2020 206f 6e5f 7374 6172  .        on_star
-000039c0: 7475 7020 3d20 7374 6172 7475 700d 0a20  tup = startup.. 
-000039d0: 2020 2020 2020 206f 6e5f 7368 7574 646f         on_shutdo
-000039e0: 776e 203d 2073 6875 7464 6f77 6e0d 0a20  wn = shutdown.. 
-000039f0: 2020 2020 2020 2066 756e 6374 696f 6e73         functions
-00003a00: 203d 205b 7061 7273 655f 6d61 7463 6865   = [parse_matche
-00003a10: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00003a20: 2020 2020 2020 2020 2070 6172 7365 5f65           parse_e
-00003a30: 7665 6e74 732c 0d0a 2020 2020 2020 2020  vents,..        
-00003a40: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00003a50: 7365 5f74 6f70 5f74 6561 6d73 2c0d 0a20  se_top_teams,.. 
-00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a70: 2020 2020 7061 7273 655f 746f 705f 706c      parse_top_pl
-00003a80: 6179 6572 732c 0d0a 2020 2020 2020 2020  ayers,..        
-00003a90: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00003aa0: 7365 5f6c 6173 745f 6e65 7773 2c0d 0a20  se_last_news,.. 
-00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 2020 2020 5d0d 0a20 2020 2020 2020 2063      ]..        c
-00003ad0: 726f 6e5f 6a6f 6273 203d 205b 0d0a 2020  ron_jobs = [..  
-00003ae0: 2020 2020 2020 2020 2020 6372 6f6e 2870            cron(p
-00003af0: 6172 7365 5f6d 6174 6368 6573 2c20 6d69  arse_matches, mi
-00003b00: 6e75 7465 3d35 3929 2c0d 0a20 2020 2020  nute=59),..     
-00003b10: 2020 2020 2020 2063 726f 6e28 7061 7273         cron(pars
-00003b20: 655f 6576 656e 7473 2c20 686f 7572 3d30  e_events, hour=0
-00003b30: 2c20 6d69 6e75 7465 3d30 2c20 7365 636f  , minute=0, seco
-00003b40: 6e64 3d30 292c 0d0a 2020 2020 2020 2020  nd=0),..        
-00003b50: 2020 2020 6372 6f6e 2870 6172 7365 5f74      cron(parse_t
-00003b60: 6f70 5f74 6561 6d73 2c20 6461 793d 302c  op_teams, day=0,
-00003b70: 2068 6f75 723d 3138 2c20 6d69 6e75 7465   hour=18, minute
-00003b80: 3d31 2c20 7365 636f 6e64 3d33 3029 2c0d  =1, second=30),.
-00003b90: 0a20 2020 2020 2020 2020 2020 2063 726f  .            cro
-00003ba0: 6e28 7061 7273 655f 746f 705f 706c 6179  n(parse_top_play
-00003bb0: 6572 732c 2064 6179 3d30 2c20 686f 7572  ers, day=0, hour
-00003bc0: 3d32 302c 206d 696e 7574 653d 302c 2073  =20, minute=0, s
-00003bd0: 6563 6f6e 643d 3029 2c0d 0a20 2020 2020  econd=0),..     
-00003be0: 2020 2020 2020 2063 726f 6e28 7061 7273         cron(pars
-00003bf0: 655f 6c61 7374 5f6e 6577 732c 206d 696e  e_last_news, min
-00003c00: 7574 653d 3535 292c 0d0a 2020 2020 2020  ute=55),..      
-00003c10: 2020 5d0d 0a0d 0a20 2020 2060 6060 0d0a    ]....    ```..
-00003c20: 0d0a 2320 5465 7374 733a 0d0a 0d0a 2a2a  ..# Tests:....**
-00003c30: 3c61 2068 7265 663d 2768 7474 7073 3a2f  <a href='https:/
-00003c40: 2f67 6974 6875 622e 636f 6d2f 616b 696d  /github.com/akim
-00003c50: 6572 736c 7973 2f68 6c74 762d 6173 796e  erslys/hltv-asyn
-00003c60: 632d 6170 692f 626c 6f62 2f6d 6169 6e2f  c-api/blob/main/
-00003c70: 7465 7374 2f68 6172 645f 7465 7374 2e70  test/hard_test.p
-00003c80: 7927 3e54 6f20 7465 7374 206c 6962 7261  y'>To test libra
-00003c90: 7279 2079 6f75 2063 616e 2075 7365 2074  ry you can use t
-00003ca0: 656d 706f 7261 7269 6c79 2074 6573 7420  emporarily test 
-00003cb0: 6669 6c65 3c2f 613e 2a2a 0d0a 0d0a 6060  file</a>**....``
-00003cc0: 600d 0a0d 0a50 6172 7365 6420 3230 3820  `....Parsed 208 
-00003cd0: 6d61 7463 6865 732e 2839 3773 2920 4552  matches.(97s) ER
-00003ce0: 524f 5253 3a20 302f 3230 380d 0a50 6172  RORS: 0/208..Par
-00003cf0: 7365 6420 3235 2065 7665 6e74 732e 2832  sed 25 events.(2
-00003d00: 3373 2920 4552 524f 5253 3a20 302f 3235  3s) ERRORS: 0/25
-00003d10: 0d0a 5061 7273 6564 2033 3120 7465 616d  ..Parsed 31 team
-00003d20: 732e 2834 3173 2920 4552 524f 5253 3a20  s.(41s) ERRORS: 
-00003d30: 302f 3331 0d0a 5061 7273 6564 2033 3120  0/31..Parsed 31 
-00003d40: 706c 6179 6572 732e 2832 3873 2920 4552  players.(28s) ER
-00003d50: 524f 5253 3a20 302f 3331 0d0a 4552 524f  RORS: 0/31..ERRO
-00003d60: 5253 3d30 0d0a 5355 4343 4553 533d 3238  RS=0..SUCCESS=28
-00003d70: 340d 0a54 6f74 616c 2070 6172 7365 643d  4..Total parsed=
-00003d80: 3238 340d 0a54 6f74 616c 2074 696d 6520  284..Total time 
-00003d90: 3936 2e38 3336 380d 0a0d 0a60 6060 0d0a  96.8368....```..
-00003da0: 0d0a 2320 4265 7461 202f 2055 6e72 656c  ..# Beta / Unrel
-00003db0: 6561 7365 640d 0a0d 0a2a 2a54 6861 7420  eased....**That 
-00003dc0: 6675 6e63 7469 6f6e 7320 7765 7265 206d  functions were m
-00003dd0: 6164 6520 666f 7220 6d79 7365 6c66 2c20  ade for myself, 
-00003de0: 6265 666f 7265 2075 7369 6e67 2072 6563  before using rec
-00003df0: 6f6d 6d65 6e64 2079 6f75 2074 6f20 6368  ommend you to ch
-00003e00: 6563 6b20 7468 6520 6669 6c65 2a2a 0d0a  eck the file**..
-00003e10: 0d0a 2320 5265 7175 6972 656d 656e 7473  ..# Requirements
-00003e20: 3a0d 0a0d 0a50 7974 686f 6e20 332e 392b  :....Python 3.9+
-00003e30: 0d0a 0d0a 4c69 6365 6e73 653a 0d0a 484c  ....License:..HL
-00003e40: 5456 2041 7379 6e63 2069 7320 6c69 6365  TV Async is lice
-00003e50: 6e73 6564 2075 6e64 6572 2074 6865 204d  nsed under the M
-00003e60: 4954 204c 6963 656e 7365 2c20 616c 6c6f  IT License, allo
-00003e70: 7769 6e67 2066 6f72 2070 6572 736f 6e61  wing for persona
-00003e80: 6c20 616e 6420 636f 6d6d 6572 6369 616c  l and commercial
-00003e90: 2075 7365 2077 6974 6820 6d69 6e69 6d61   use with minima
-00003ea0: 6c20 7265 7374 7269 6374 696f 6e73 2e0d  l restrictions..
-00003eb0: 0a                                       .
+00000040: 2066 6f72 2050 7974 686f 6e2e 200d 0a23   for Python. ..#
+00000050: 2055 7365 206f 6e6c 7920 696e 206e 6f6e   Use only in non
+00000060: 2d63 6f6d 6d65 7263 6961 6c20 7075 7270  -commercial purp
+00000070: 6f73 6573 0d0a 0d0a 0d0a 2a2a 5468 6973  oses......**This
+00000080: 2070 6167 6520 6973 206e 6f74 2063 6f6d   page is not com
+00000090: 706c 6574 6564 2c20 6e6f 7420 616c 6c20  pleted, not all 
+000000a0: 6d65 7468 6f64 7320 616e 6420 636f 6e66  methods and conf
+000000b0: 6967 7320 6172 6520 7772 6974 7465 6e2a  igs are written*
+000000c0: 2a0d 0a0d 0a0d 0a23 2046 6561 7475 7265  *......# Feature
+000000d0: 730d 0a0d 0a0d 0a2a 202a 2a53 696d 706c  s......* **Simpl
+000000e0: 6520 5573 6167 652a 2a20 2869 7473 2072  e Usage** (its r
+000000f0: 6561 6c6c 7920 7369 6d70 6c65 290d 0a0d  eally simple)...
+00000100: 0a0d 0a2a 202a 2a4e 6577 2061 6e64 206d  ...* **New and m
+00000110: 6f64 6572 6e20 6675 6c6c 7920 6173 796e  odern fully asyn
+00000120: 6320 6c69 6272 6172 792a 2a0d 0a0d 0a0d  c library**.....
+00000130: 0a2a 202a 2a48 7567 6520 616d 6f75 6e74  .* **Huge amount
+00000140: 206f 6620 6f70 7469 6f6e 732a 2a0d 0a0d   of options**...
+00000150: 0a0d 0a2a 202a 2a53 7570 706f 7274 7320  ...* **Supports 
+00000160: 7072 6f78 7920 7573 6167 652a 2a0d 0a0d  proxy usage**...
+00000170: 0a0d 0a2a 202a 2a4d 6164 6520 7769 7468  ...* **Made with
+00000180: 206c 6f76 6520 3c33 2a2a 0d0a 0d0a 0d0a   love <3**......
+00000190: 2d2d 2d0d 0a0d 0a23 2049 6e73 7461 6c6c  ---....# Install
+000001a0: 6174 696f 6e0d 0a0d 0a60 6060 0d0a 7069  ation....```..pi
+000001b0: 7020 696e 7374 616c 6c20 686c 7476 2d61  p install hltv-a
+000001c0: 7379 6e63 2d61 7069 0d0a 6060 600d 0a0d  sync-api..```...
+000001d0: 0a2d 2d2d 0d0a 0d0a 0d0a 2320 5369 6d70  .---......# Simp
+000001e0: 6c65 2055 7361 6765 0d0a 0d0a 2020 2020  le Usage....    
+000001f0: 6060 600d 0a0d 0a20 2020 2066 726f 6d20  ```....    from 
+00000200: 686c 7476 5f61 7379 6e63 5f61 7069 2069  hltv_async_api i
+00000210: 6d70 6f72 7420 486c 7476 0d0a 2020 2020  mport Hltv..    
+00000220: 0d0a 2020 2020 6173 796e 6320 7769 7468  ..    async with
+00000230: 2048 6c74 7628 2920 6173 2068 6c74 763a   Hltv() as hltv:
+00000240: 0d0a 2020 2020 2020 7072 696e 7428 6177  ..      print(aw
+00000250: 6169 7420 686c 7476 2e67 6574 5f65 7665  ait hltv.get_eve
+00000260: 6e74 5f69 6e66 6f28 3731 3438 2c20 2750  nt_info(7148, 'P
+00000270: 474c 2043 5332 204d 616a 6f72 2043 6f70  GL CS2 Major Cop
+00000280: 656e 6861 6765 6e32 3032 3427 2929 0d0a  enhagen2024'))..
+00000290: 0d0a 2020 2020 6060 600d 0a0d 0a20 202a  ..    ```....  *
+000002a0: 2a4f 522a 2a0d 0a0d 0a20 2020 2060 6060  *OR**....    ```
+000002b0: 0d0a 0d0a 2020 2020 6672 6f6d 2068 6c74  ....    from hlt
+000002c0: 765f 6173 796e 635f 6170 6920 696d 706f  v_async_api impo
+000002d0: 7274 2048 6c74 760d 0a20 2020 200d 0a20  rt Hltv..    .. 
+000002e0: 2020 2068 6c74 7620 3d20 486c 7476 2829     hltv = Hltv()
+000002f0: 0d0a 2020 2020 7072 696e 7428 6177 6169  ..    print(awai
+00000300: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
+00000310: 5f69 6e66 6f28 3731 3438 2c20 2750 474c  _info(7148, 'PGL
+00000320: 2043 5332 204d 616a 6f72 2043 6f70 656e   CS2 Major Copen
+00000330: 6861 6765 6e32 3032 3427 2929 0d0a 2020  hagen2024'))..  
+00000340: 2020 6177 6169 7420 686c 7476 2e63 6c6f    await hltv.clo
+00000350: 7365 2829 0d0a 0d0a 2020 2020 6060 600d  se()....    ```.
+00000360: 0a0d 0a0d 0a2d 2d2d 0d0a 0d0a 2320 436f  .....---....# Co
+00000370: 6e66 6967 730d 0a0d 0a2a 206d 6178 5f64  nfigs....* max_d
+00000380: 656c 6179 3a20 696e 7420 3d20 3135 0d0a  elay: int = 15..
+00000390: 0d0a 2020 2020 4175 746f 6d61 7469 6361  ..    Automatica
+000003a0: 6c6c 7920 696e 6372 6561 7369 6e67 2072  lly increasing r
+000003b0: 6563 6f6e 6e65 6374 696e 6720 6465 6c61  econnecting dela
+000003c0: 7920 6279 2031 2073 6563 2074 6f20 6d61  y by 1 sec to ma
+000003d0: 785f 6465 6c61 7920 2866 726f 6d20 3173  x_delay (from 1s
+000003e0: 2074 6f20 3573 290d 0a0d 0a20 2020 2060   to 5s)....    `
+000003f0: 6060 0d0a 2020 2020 686c 7476 203d 2048  ``..    hltv = H
+00000400: 6c74 7628 6d61 785f 6465 6c61 793d 3529  ltv(max_delay=5)
+00000410: 0d0a 2020 2020 0d0a 2020 2020 3e3e 3e46  ..    ..    >>>F
+00000420: 6574 6368 696e 6720 6874 7470 733a 2f2f  etching https://
+00000430: 7777 772e 686c 7476 2e6f 7267 2f6d 6174  www.hltv.org/mat
+00000440: 6368 6573 2f32 3337 3037 3237 2f66 617a  ches/2370727/faz
+00000450: 652d 7673 2d6e 6174 7573 2d76 696e 6365  e-vs-natus-vince
+00000460: 7265 2d70 676c 2d63 7332 2d6d 616a 6f72  re-pgl-cs2-major
+00000470: 2d63 6f70 656e 6861 6765 6e2d 3230 3234  -copenhagen-2024
+00000480: 2c20 636f 6465 3a20 3430 330d 0a20 2020  , code: 403..   
+00000490: 203e 3e3e 476f 7420 3430 3320 666f 7262   >>>Got 403 forb
+000004a0: 6974 7465 6e0d 0a20 2020 203e 3e3e 4361  itten..    >>>Ca
+000004b0: 6c6c 696e 6720 6167 6169 6e2c 2069 6e63  lling again, inc
+000004c0: 7265 6173 696e 6720 6465 6c61 7920 746f  reasing delay to
+000004d0: 2034 730d 0a20 2020 203e 3e3e 4665 7463   4s..    >>>Fetc
+000004e0: 6869 6e67 2068 7474 7073 3a2f 2f77 7777  hing https://www
+000004f0: 2e68 6c74 762e 6f72 672f 6d61 7463 6865  .hltv.org/matche
+00000500: 732f 3233 3730 3732 372f 6661 7a65 2d76  s/2370727/faze-v
+00000510: 732d 6e61 7475 732d 7669 6e63 6572 652d  s-natus-vincere-
+00000520: 7067 6c2d 6373 322d 6d61 6a6f 722d 636f  pgl-cs2-major-co
+00000530: 7065 6e68 6167 656e 2d32 3032 342c 2063  penhagen-2024, c
+00000540: 6f64 653a 2034 3033 0d0a 2020 2020 3e3e  ode: 403..    >>
+00000550: 3e47 6f74 2034 3033 2066 6f72 6269 7474  >Got 403 forbitt
+00000560: 656e 0d0a 2020 2020 3e3e 3e43 616c 6c69  en..    >>>Calli
+00000570: 6e67 2061 6761 696e 2c20 696e 6372 6561  ng again, increa
+00000580: 7369 6e67 2064 656c 6179 2074 6f20 3573  sing delay to 5s
+00000590: 0d0a 2020 2020 6060 600d 0a0d 0a2a 206d  ..    ```....* m
+000005a0: 6178 5f72 6574 7269 6573 3a20 696e 7420  ax_retries: int 
+000005b0: 3d20 300d 0a0d 0a20 2020 204d 6178 2072  = 0....    Max r
+000005c0: 6574 7269 6573 2e20 3020 6f72 202d 3120  etries. 0 or -1 
+000005d0: 666f 7220 696e 6669 6e69 7479 2074 7269  for infinity tri
+000005e0: 6573 2e0d 0a20 2020 200d 0a20 2020 2060  es...    ..    `
+000005f0: 6060 0d0a 2020 2020 686c 7476 203d 2048  ``..    hltv = H
+00000600: 6c74 7628 6d61 785f 7265 7472 6965 733d  ltv(max_retries=
+00000610: 322c 2064 6562 7567 3d54 7275 6529 0d0a  2, debug=True)..
+00000620: 2020 2020 7072 696e 7428 6177 6169 7420      print(await 
+00000630: 686c 7476 2e67 6574 5f62 6573 745f 706c  hltv.get_best_pl
+00000640: 6179 6572 7328 2929 0d0a 2020 2020 0d0a  ayers())..    ..
+00000650: 2020 2020 4372 6561 7469 6e67 2053 6573      Creating Ses
+00000660: 7369 6f6e 0d0a 2020 2020 5472 7969 6e67  sion..    Trying
+00000670: 2063 6f6e 6e65 6374 2074 6f20 6874 7470   connect to http
+00000680: 733a 2f2f 7777 772e 686c 7476 2e6f 7267  s://www.hltv.org
+00000690: 2f73 7461 7473 2f70 6c61 7965 7273 3f73  /stats/players?s
+000006a0: 7461 7274 4461 7465 3d32 3032 342d 3031  tartDate=2024-01
+000006b0: 2d30 3126 656e 6444 6174 653d 3230 3234  -01&endDate=2024
+000006c0: 2d31 322d 3331 2672 616e 6b69 6e67 4669  -12-31&rankingFi
+000006d0: 6c74 6572 3d54 6f70 3230 2c20 7472 7920  lter=Top20, try 
+000006e0: 312f 320d 0a20 2020 2054 7279 696e 6720  1/2..    Trying 
+000006f0: 636f 6e6e 6563 7420 746f 2068 7474 7073  connect to https
+00000700: 3a2f 2f77 7777 2e68 6c74 762e 6f72 672f  ://www.hltv.org/
+00000710: 7374 6174 732f 706c 6179 6572 733f 7374  stats/players?st
+00000720: 6172 7444 6174 653d 3230 3234 2d30 312d  artDate=2024-01-
+00000730: 3031 2665 6e64 4461 7465 3d32 3032 342d  01&endDate=2024-
+00000740: 3132 2d33 3126 7261 6e6b 696e 6746 696c  12-31&rankingFil
+00000750: 7465 723d 546f 7032 302c 2074 7279 2032  ter=Top20, try 2
+00000760: 2f32 0d0a 2020 2020 436f 6e6e 6563 7469  /2..    Connecti
+00000770: 6f6e 2066 6169 6c65 640d 0a20 2020 2060  on failed..    `
+00000780: 6060 0d0a 0d0a 2a20 7072 6f78 795f 6c69  ``....* proxy_li
+00000790: 7374 3a20 6c69 7374 207c 204e 6f6e 6520  st: list | None 
+000007a0: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 6c69  = None....    li
+000007b0: 7374 206f 6620 796f 7572 2070 726f 7869  st of your proxi
+000007c0: 6573 2c20 6966 2079 6f75 7220 7072 6f78  es, if your prox
+000007d0: 6965 7320 646f 6573 6e74 2068 6176 6520  ies doesnt have 
+000007e0: 616e 7920 7072 6f74 6f63 6f6c 2079 6f75  any protocol you
+000007f0: 2063 616e 2075 7365 2070 726f 7879 5f70   can use proxy_p
+00000800: 726f 746f 636f 6c2e 0d0a 2020 2020 4e6f  rotocol...    No
+00000810: 7465 3a20 546f 2061 6464 206e 6f6e 2d70  te: To add non-p
+00000820: 726f 7879 2074 6f20 6c69 7374 206a 7573  roxy to list jus
+00000830: 7420 7075 7420 2727 2074 6f20 6974 2c20  t put '' to it, 
+00000840: 796f 7520 6361 6e20 6669 6e64 2065 7861  you can find exa
+00000850: 6d70 6c65 2077 6974 6820 6172 0d0a 0d0a  mple with ar....
+00000860: 2a20 7072 6f78 795f 7061 7468 3a20 7374  * proxy_path: st
+00000870: 7220 7c20 4e6f 6e65 203d 204e 6f6e 650d  r | None = None.
+00000880: 0a0d 0a20 2020 2050 6174 6820 746f 2079  ...    Path to y
+00000890: 6f75 7220 7072 6f78 7920 2870 726f 7879  our proxy (proxy
+000008a0: 5f6c 6973 7420 7769 6c6c 2062 6520 6967  _list will be ig
+000008b0: 6e6f 7265 6429 2e20 4966 2079 6f75 7220  nored). If your 
+000008c0: 7072 6f78 6965 7320 646f 6573 6e74 2068  proxies doesnt h
+000008d0: 6176 6520 616e 7920 7072 6f74 6f63 6f6c  ave any protocol
+000008e0: 2079 6f75 2063 616e 2075 7365 2070 726f   you can use pro
+000008f0: 7879 5f70 726f 746f 636f 6c0d 0a0d 0a2a  xy_protocol....*
+00000900: 2070 726f 7879 5f70 726f 746f 636f 6c3a   proxy_protocol:
+00000910: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
+00000920: 6e65 2c0d 0a0d 0a20 2020 2050 726f 7879  ne,....    Proxy
+00000930: 2070 726f 746f 636f 6c2e 2059 6f75 7220   protocol. Your 
+00000940: 7072 6f78 6965 7320 6060 6068 6c74 7620  proxies ```hltv 
+00000950: 3d20 486c 7476 2870 726f 7879 5f70 726f  = Hltv(proxy_pro
+00000960: 746f 636f 6c3d 2768 7474 7027 202e 2e2e  tocol='http' ...
+00000970: 2920 2d3e 2027 3131 2e31 312e 3131 2e31  ) -> '11.11.11.1
+00000980: 313a 3131 3131 2720 2d3e 2027 6874 7470  1:1111' -> 'http
+00000990: 3a2f 2f31 312e 3131 2e31 312e 3131 3a31  ://11.11.11.11:1
+000009a0: 3131 3127 0d0a 0d0a 2a20 6465 6c65 7465  111'....* delete
+000009b0: 5f70 726f 7879 3a20 626f 6f6c 203d 2046  _proxy: bool = F
+000009c0: 616c 7365 0d0a 0d0a 2020 2020 5265 6d6f  alse....    Remo
+000009d0: 7665 7320 7072 6f78 7920 6672 6f6d 206c  ves proxy from l
+000009e0: 6973 7420 2870 726f 7879 5f70 6174 6820  ist (proxy_path 
+000009f0: 696e 636c 7564 6564 2920 6966 2063 6f6e  included) if con
+00000a00: 6e65 6374 696f 6e20 756e 7375 6363 6573  nection unsucces
+00000a10: 7366 756c 6c79 0d0a 0d0a 2a20 7469 6d65  sfully....* time
+00000a20: 6f75 743a 2069 6e74 203d 2035 0d0a 0d0a  out: int = 5....
+00000a30: 2020 2020 4d61 7820 7469 6d65 2074 6f20      Max time to 
+00000a40: 636c 6f73 6520 636f 6e6e 6563 7469 6f6e  close connection
+00000a50: 2e20 5265 636f 6d6d 656e 6465 6420 746f  . Recommended to
+00000a60: 2075 7365 2074 696d 656f 7574 3d31 2069   use timeout=1 i
+00000a70: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
+00000a80: 7261 6e64 6f6d 2070 726f 7869 6573 2e0d  random proxies..
+00000a90: 0a0d 0a2a 2064 6562 7567 3a20 626f 6f6c  ...* debug: bool
+00000aa0: 203d 2046 616c 7365 0d0a 0d0a 2a20 747a   = False....* tz
+00000ab0: 3a20 7374 7220 3d20 2745 7572 6f70 652f  : str = 'Europe/
+00000ac0: 436f 7065 6e68 6167 656e 273a 0d0a 2020  Copenhagen':..  
+00000ad0: 2020 0d0a 2020 2020 5469 6d65 7a6f 6e65    ..    Timezone
+00000ae0: 2063 6f6e 6669 672e 200d 0a20 0d0a 2020   config. .. ..  
+00000af0: 2020 3c61 2068 7265 663d 2768 7474 7073    <a href='https
+00000b00: 3a2f 2f67 6973 742e 6769 7468 7562 2e63  ://gist.github.c
+00000b10: 6f6d 2f68 6579 616c 6578 656a 2f38 6266  om/heyalexej/8bf
+00000b20: 3638 3866 6436 3764 3731 3939 6265 3461  688fd67d7199be4a
+00000b30: 3136 3832 6233 6565 6337 3536 3827 3e54  1682b3eec7568'>T
+00000b40: 6170 2068 6572 6520 3c2f 613e 2074 6f20  ap here </a> to 
+00000b50: 7365 6520 616c 6c20 6176 6169 6c61 626c  see all availabl
+00000b60: 6520 7469 6d65 7a6f 6e65 730d 0a0d 0a2a  e timezones....*
+00000b70: 2073 6166 655f 6d6f 6465 3a20 626f 6f6c   safe_mode: bool
+00000b80: 203d 2054 7275 650d 0a0d 0a20 2020 2044   = True....    D
+00000b90: 6973 616c 6c6f 7720 746f 2077 7261 7020  isallow to wrap 
+00000ba0: 7265 7374 7269 6374 6564 2064 6174 612e  restricted data.
+00000bb0: 2053 7769 7463 6820 746f 2046 616c 7365   Switch to False
+00000bc0: 206f 6e6c 7920 6174 2079 6f75 7220 6f77   only at your ow
+00000bd0: 6e20 7269 736b 2e0d 0a0d 0a0d 0a2d 2d2d  n risk.......---
+00000be0: 0d0a 0d0a 2320 5072 6f78 7920 5573 6167  ....# Proxy Usag
+00000bf0: 650d 0a0d 0a2a 2a4c 6f61 6420 5072 6f78  e....**Load Prox
+00000c00: 6965 7320 6672 6f6d 206c 6973 742a 2a0d  ies from list**.
+00000c10: 0a20 2020 200d 0a20 2020 2060 6060 0d0a  .    ..    ```..
+00000c20: 2020 2020 7072 6f78 795f 6c69 7374 203d      proxy_list =
+00000c30: 205b 2768 7474 703a 2f2f 3132 302e 3233   ['http://120.23
+00000c40: 342e 3230 332e 3137 313a 3930 3032 272c  4.203.171:9002',
+00000c50: 2027 6874 7470 3a2f 2f31 3130 2e33 382e   'http://110.38.
+00000c60: 3638 2e33 383a 3830 275d 0d0a 2020 2020  68.38:80']..    
+00000c70: 0d0a 2020 2020 686c 7476 203d 2048 6c74  ..    hltv = Hlt
+00000c80: 7628 7072 6f78 795f 6c69 7374 3d70 726f  v(proxy_list=pro
+00000c90: 7879 5f6c 6973 7429 0d0a 0d0a 2020 2020  xy_list)....    
+00000ca0: 6060 600d 0a0d 0a2a 2a4c 6f61 6420 5072  ```....**Load Pr
+00000cb0: 6f78 6965 7320 6672 6f6d 2066 696c 652a  oxies from file*
+00000cc0: 2a0d 0a0d 0a20 2020 2060 6060 0d0a 2020  *....    ```..  
+00000cd0: 2020 686c 7476 203d 2048 6c74 7628 7072    hltv = Hltv(pr
+00000ce0: 6f78 795f 7061 7468 3d27 5041 5448 5f54  oxy_path='PATH_T
+00000cf0: 4f5f 5052 4f58 592e 5458 5427 290d 0a20  O_PROXY.TXT').. 
+00000d00: 2020 2060 6060 0d0a 0d0a 0d0a 2a2a 4465     ```......**De
+00000d10: 6c65 7465 2070 726f 7879 2a2a 0d0a 0d0a  lete proxy**....
+00000d20: 2020 2020 5265 6d6f 7665 7320 6261 6420      Removes bad 
+00000d30: 7072 6f78 6965 730d 0a20 2020 200d 0a20  proxies..    .. 
+00000d40: 2020 2060 6060 0d0a 2020 2020 686c 7476     ```..    hltv
+00000d50: 203d 2048 6c74 7628 7072 6f78 795f 7061   = Hltv(proxy_pa
+00000d60: 7468 3d27 5041 5448 5f54 4f5f 5052 4f58  th='PATH_TO_PROX
+00000d70: 592e 5458 5427 2c20 6465 6c65 7465 5f70  Y.TXT', delete_p
+00000d80: 726f 7879 3d54 7275 6529 0d0a 2020 2020  roxy=True)..    
+00000d90: 6060 600d 0a0d 0a2a 2a50 726f 746f 636f  ```....**Protoco
+00000da0: 6c20 7573 6167 652a 2a0d 0a0d 0a20 2020  l usage**....   
+00000db0: 2060 6060 0d0a 2020 2020 7072 6f78 795f   ```..    proxy_
+00000dc0: 6c69 7374 203d 205b 2731 3230 2e32 3334  list = ['120.234
+00000dd0: 2e32 3033 2e31 3731 3a39 3030 3227 2c20  .203.171:9002', 
+00000de0: 2731 3130 2e33 382e 3638 2e33 383a 3830  '110.38.68.38:80
+00000df0: 275d 0d0a 2020 2020 0d0a 2020 2020 686c  ']..    ..    hl
+00000e00: 7476 203d 2048 6c74 7628 7072 6f78 795f  tv = Hltv(proxy_
+00000e10: 6c69 7374 3d70 726f 7879 5f6c 6973 742c  list=proxy_list,
+00000e20: 2070 726f 7879 5f70 726f 746f 636f 6c3d   proxy_protocol=
+00000e30: 2768 7474 7027 290d 0a20 2020 2060 6060  'http')..    ```
+00000e40: 0d0a 0d0a 2d2d 2d0d 0a0d 0a23 204d 6574  ....---....# Met
+00000e50: 686f 6473 0d0a 0d0a 2a20 2a2a 6765 745f  hods....* **get_
+00000e60: 6d61 7463 6865 7328 6461 7973 3a20 696e  matches(days: in
+00000e70: 7420 3d20 312c 206d 696e 5f73 7461 725f  t = 1, min_star_
+00000e80: 7261 7469 6e67 3a20 696e 7420 3d20 312c  rating: int = 1,
+00000e90: 206c 6976 653a 2062 6f6f 6c20 3d20 5472   live: bool = Tr
+00000ea0: 7565 2c20 6675 7475 7265 3a20 626f 6f6c  ue, future: bool
+00000eb0: 203d 2054 7275 6529 2a2a 0d0a 0d0a 2020   = True)**....  
+00000ec0: 2020 2d64 6179 7320 2874 6865 206e 756d    -days (the num
+00000ed0: 6265 7220 6f66 2064 6179 7320 696e 746f  ber of days into
+00000ee0: 2074 6865 2066 7574 7572 6520 746f 2066   the future to f
+00000ef0: 6574 6368 206d 6174 6368 6573 2066 6f72  etch matches for
+00000f00: 290d 0a20 200d 0a20 2020 202d 6d69 6e5f  )..  ..    -min_
+00000f10: 7374 6172 5f72 6174 696e 6720 2874 6865  star_rating (the
+00000f20: 206d 696e 696d 756d 2073 7461 7220 7261   minimum star ra
+00000f30: 7469 6e67 2066 6f72 206d 6174 6368 6573  ting for matches
+00000f40: 2074 6f20 696e 636c 7564 6529 0d0a 2020   to include)..  
+00000f50: 0d0a 2020 2020 6060 600d 0a20 2020 2061  ..    ```..    a
+00000f60: 7761 6974 2068 6c74 762e 6765 745f 6d61  wait hltv.get_ma
+00000f70: 7463 6865 7328 6461 7973 3d31 290d 0a20  tches(days=1).. 
+00000f80: 2020 200d 0a20 2020 203e 3e3e 205b 7b27     ..    >>> [{'
+00000f90: 6964 273a 2027 3233 3731 3230 3127 2c20  id': '2371201', 
+00000fa0: 2764 6174 6527 3a20 274c 4956 4527 2c20  'date': 'LIVE', 
+00000fb0: 2774 696d 6527 3a20 274c 4956 4527 2c20  'time': 'LIVE', 
+00000fc0: 2774 6561 6d31 273a 2027 496d 7065 7269  'team1': 'Imperi
+00000fd0: 616c 272c 2027 7465 616d 3227 3a20 274d  al', 'team2': 'M
+00000fe0: 4942 5227 2c20 2774 315f 6964 273a 2027  IBR', 't1_id': '
+00000ff0: 3934 3535 272c 2027 7432 5f69 6427 3a20  9455', 't2_id': 
+00001000: 2739 3231 3527 2c20 276d 6170 7327 3a20  '9215', 'maps': 
+00001010: 2733 272c 2027 7261 7469 6e67 273a 2031  '3', 'rating': 1
+00001020: 2c20 2765 7665 6e74 273a 2027 5245 5320  , 'event': 'RES 
+00001030: 5265 6769 6f6e 616c 2053 6572 6965 7320  Regional Series 
+00001040: 3320 4c41 5441 4d27 7d2c 207b 2769 6427  3 LATAM'}, {'id'
+00001050: 3a20 2732 3337 3039 3634 272c 2027 6461  : '2370964', 'da
+00001060: 7465 273a 2027 3230 3234 2d30 342d 3136  te': '2024-04-16
+00001070: 272c 2027 7469 6d65 273a 2027 3132 3a33  ', 'time': '12:3
+00001080: 3027 2c20 2774 6561 6d31 273a 2027 5341  0', 'team1': 'SA
+00001090: 5727 2c20 2774 6561 6d32 273a 2027 5361  W', 'team2': 'Sa
+000010a0: 6d70 6927 2c20 2774 315f 6964 273a 2027  mpi', 't1_id': '
+000010b0: 3130 3536 3727 2c20 2774 325f 6964 273a  10567', 't2_id':
+000010c0: 2027 3130 3639 3527 2c20 276d 6170 7327   '10695', 'maps'
+000010d0: 3a20 2733 272c 2027 7261 7469 6e67 273a  : '3', 'rating':
+000010e0: 2031 2c20 2765 7665 6e74 273a 2027 5468   1, 'event': 'Th
+000010f0: 756e 6465 7270 6963 6b20 576f 726c 6420  underpick World 
+00001100: 4368 616d 7069 6f6e 7368 6970 2032 3032  Championship 202
+00001110: 3420 4555 2043 6c6f 7365 6420 5175 616c  4 EU Closed Qual
+00001120: 6966 6965 7220 3127 7d2c 207b 2769 6427  ifier 1'}, {'id'
+00001130: 3a20 2732 3337 3133 3637 272c 2027 6461  : '2371367', 'da
+00001140: 7465 273a 2027 3230 3234 2d30 342d 3136  te': '2024-04-16
+00001150: 272c 2027 7469 6d65 273a 2027 3134 3a30  ', 'time': '14:0
+00001160: 3027 2c20 2774 6561 6d31 273a 2027 4761  0', 'team1': 'Ga
+00001170: 696d 696e 2047 6c61 6469 6174 6f72 7327  imin Gladiators'
+00001180: 2c20 2774 6561 6d32 273a 2027 5065 726d  , 'team2': 'Perm
+00001190: 6974 7461 272c 2027 7431 5f69 6427 3a20  itta', 't1_id': 
+000011a0: 2731 3135 3731 272c 2027 7432 5f69 6427  '11571', 't2_id'
+000011b0: 3a20 2731 3230 3039 272c 2027 6d61 7073  : '12009', 'maps
+000011c0: 273a 2027 3327 2c20 2772 6174 696e 6727  ': '3', 'rating'
+000011d0: 3a20 312c 2027 6576 656e 7427 3a20 2745  : 1, 'event': 'E
+000011e0: 6c69 7361 2049 6e76 6974 6174 696f 6e61  lisa Invitationa
+000011f0: 6c20 5370 7269 6e67 2032 3032 3427 7d5d  l Spring 2024'}]
+00001200: 0d0a 2020 2020 0d0a 2020 2020 6060 600d  ..    ..    ```.
+00001210: 0a0d 0a2a 202a 2a67 6574 5f6d 6174 6368  ...* **get_match
+00001220: 5f69 6e66 6f28 6d61 7463 685f 6964 3a20  _info(match_id: 
+00001230: 696e 7420 7c20 7374 722c 2074 6561 6d31  int | str, team1
+00001240: 2c20 7465 616d 322c 2065 7665 6e74 5f74  , team2, event_t
+00001250: 6974 6c65 2c20 7374 6174 733a 2062 6f6f  itle, stats: boo
+00001260: 6c20 3d20 5472 7565 2c20 7072 6564 6963  l = True, predic
+00001270: 7473 3a20 626f 6f6c 203d 2054 7275 6529  ts: bool = True)
+00001280: 2a2a 0d0a 2020 0d0a 2020 2020 6060 600d  **..  ..    ```.
+00001290: 0a20 2020 2061 7761 6974 2068 6c74 762e  .    await hltv.
+000012a0: 6765 745f 6d61 7463 685f 696e 666f 2832  get_match_info(2
+000012b0: 3337 3039 3331 2c20 274d 6f75 7a27 2c20  370931, 'Mouz', 
+000012c0: 2766 617a 6527 2c20 2769 656d 2d63 6865  'faze', 'iem-che
+000012d0: 6e67 6475 2d32 3032 3427 2920 200d 0a20  ngdu-2024')  .. 
+000012e0: 200d 0a20 2020 203e 3e3e 2832 3337 3039   ..    >>>(23709
+000012f0: 3331 2c20 2730 272c 2027 3227 2c20 274d  31, '0', '2', 'M
+00001300: 6174 6368 206f 7665 7227 2c20 5b7b 276d  atch over', [{'m
+00001310: 6170 6e61 6d65 273a 2027 4f76 6572 7061  apname': 'Overpa
+00001320: 7373 272c 2027 725f 7465 616d 3127 3a20  ss', 'r_team1': 
+00001330: 2731 3027 2c20 2772 5f74 6561 6d32 273a  '10', 'r_team2':
+00001340: 2027 3133 277d 2c20 7b27 6d61 706e 616d   '13'}, {'mapnam
+00001350: 6527 3a20 274e 756b 6527 2c20 2772 5f74  e': 'Nuke', 'r_t
+00001360: 6561 6d31 273a 2027 3627 2c20 2772 5f74  eam1': '6', 'r_t
+00001370: 6561 6d32 273a 2027 3133 277d 2c20 7b27  eam2': '13'}, {'
+00001380: 6d61 706e 616d 6527 3a20 274d 6972 6167  mapname': 'Mirag
+00001390: 6527 2c20 2772 5f74 6561 6d31 273a 2027  e', 'r_team1': '
+000013a0: 2d27 2c20 2772 5f74 6561 6d32 273a 2027  -', 'r_team2': '
+000013b0: 2d27 7d5d 2c20 5b7b 2769 6427 3a20 2731  -'}], [{'id': '1
+000013c0: 3838 3530 272c 2027 6e69 636b 6e61 6d65  8850', 'nickname
+000013d0: 273a 2027 4a69 6d70 7068 6174 272c 2027  ': 'Jimpphat', '
+000013e0: 6b64 273a 2027 3333 2d32 3927 2c20 2761  kd': '33-29', 'a
+000013f0: 6472 273a 2027 3830 2e39 272c 2027 7261  dr': '80.9', 'ra
+00001400: 7469 6e67 273a 2027 312e 3038 277d 2c20  ting': '1.08'}, 
+00001410: 0d0a 2020 0d0a 2020 2020 7b27 6964 273a  ..  ..    {'id':
+00001420: 2027 3138 3037 3227 2c20 276e 6963 6b6e   '18072', 'nickn
+00001430: 616d 6527 3a20 2774 6f72 7a73 6927 2c20  ame': 'torzsi', 
+00001440: 276b 6427 3a20 2732 362d 3235 272c 2027  'kd': '26-25', '
+00001450: 6164 7227 3a20 2737 302e 3527 2c20 2772  adr': '70.5', 'r
+00001460: 6174 696e 6727 3a20 2731 2e30 3227 7d2c  ating': '1.02'},
+00001470: 207b 2769 6427 3a20 2731 3336 3636 272c   {'id': '13666',
+00001480: 2027 6e69 636b 6e61 6d65 273a 2027 4272   'nickname': 'Br
+00001490: 6f6c 6c61 6e27 2c20 276b 6427 3a20 2732  ollan', 'kd': '2
+000014a0: 352d 3331 272c 2027 6164 7227 3a20 2736  5-31', 'adr': '6
+000014b0: 382e 3427 2c20 2772 6174 696e 6727 3a20  8.4', 'rating': 
+000014c0: 2730 2e39 3027 7d2c 207b 2769 6427 3a20  '0.90'}, {'id': 
+000014d0: 2732 3033 3132 272c 2027 6e69 636b 6e61  '20312', 'nickna
+000014e0: 6d65 273a 2027 7865 7274 696f 4e27 2c20  me': 'xertioN', 
+000014f0: 276b 6427 3a20 2732 332d 3331 272c 2027  'kd': '23-31', '
+00001500: 6164 7227 3a20 2736 322e 3427 2c20 2772  adr': '62.4', 'r
+00001510: 6174 696e 6727 3a20 2730 2e38 3227 7d2c  ating': '0.82'},
+00001520: 207b 2769 6427 3a20 2731 3638 3230 272c   {'id': '16820',
+00001530: 2027 6e69 636b 6e61 6d65 273a 2027 7369   'nickname': 'si
+00001540: 7568 7927 2c20 276b 6427 3a20 2731 372d  uhy', 'kd': '17-
+00001550: 3330 272c 2027 6164 7227 3a20 2735 312e  30', 'adr': '51.
+00001560: 3627 2c20 2772 6174 696e 6727 3a20 2730  6', 'rating': '0
+00001570: 2e37 3027 7d2c 207b 2769 6427 3a20 2731  .70'}, {'id': '1
+00001580: 3830 3533 272c 2027 6e69 636b 6e61 6d65  8053', 'nickname
+00001590: 273a 2027 6272 6f6b 7927 2c20 276b 6427  ': 'broky', 'kd'
+000015a0: 3a20 2733 342d 3232 272c 2027 6164 7227  : '34-22', 'adr'
+000015b0: 3a20 2737 392e 3327 2c20 2772 6174 696e  : '79.3', 'ratin
+000015c0: 6727 3a20 2731 2e33 3327 7d2c 207b 2769  g': '1.33'}, {'i
+000015d0: 6427 3a20 2739 3936 3027 2c20 276e 6963  d': '9960', 'nic
+000015e0: 6b6e 616d 6527 3a20 2766 726f 7a65 6e27  kname': 'frozen'
+000015f0: 2c20 276b 6427 3a20 2733 332d 3233 272c  , 'kd': '33-23',
+00001600: 2027 6164 7227 3a20 2738 352e 3527 2c20   'adr': '85.5', 
+00001610: 2772 6174 696e 6727 3a20 2731 2e33 3127  'rating': '1.31'
+00001620: 7d2c 207b 2769 6427 3a20 2731 3138 3136  }, {'id': '11816
+00001630: 272c 2027 6e69 636b 6e61 6d65 273a 2027  ', 'nickname': '
+00001640: 726f 707a 272c 2027 6b64 273a 2027 3331  ropz', 'kd': '31
+00001650: 2d32 3627 2c20 2761 6472 273a 2027 3733  -26', 'adr': '73
+00001660: 2e30 272c 2027 7261 7469 6e67 273a 2027  .0', 'rating': '
+00001670: 312e 3230 277d 2c20 7b27 6964 273a 2027  1.20'}, {'id': '
+00001680: 3831 3833 272c 2027 6e69 636b 6e61 6d65  8183', 'nickname
+00001690: 273a 2027 7261 696e 272c 2027 6b64 273a  ': 'rain', 'kd':
+000016a0: 2027 3237 2d32 3627 2c20 2761 6472 273a   '27-26', 'adr':
+000016b0: 2027 3832 2e30 272c 2027 7261 7469 6e67   '82.0', 'rating
+000016c0: 273a 2027 312e 3138 277d 2c20 7b27 6964  ': '1.18'}, {'id
+000016d0: 273a 2027 3432 3927 2c20 276e 6963 6b6e  ': '429', 'nickn
+000016e0: 616d 6527 3a20 276b 6172 7269 6761 6e27  ame': 'karrigan'
+000016f0: 2c20 276b 6427 3a20 2732 302d 3238 272c  , 'kd': '20-28',
+00001700: 2027 6164 7227 3a20 2734 392e 3727 2c20   'adr': '49.7', 
+00001710: 2772 6174 696e 6727 3a20 2730 2e38 3127  'rating': '0.81'
+00001720: 7d5d 2920 200d 0a20 2020 200d 0a20 2020  }])  ..    ..   
+00001730: 2060 6060 0d0a 2020 0d0a 2a20 2a2a 6765   ```..  ..* **ge
+00001740: 745f 7265 7375 6c74 7328 6461 7973 3a20  t_results(days: 
+00001750: 696e 7420 3d20 312c 206d 696e 5f72 6174  int = 1, min_rat
+00001760: 696e 673a 2069 6e74 203d 2031 2c20 6d61  ing: int = 1, ma
+00001770: 783a 2069 6e74 203d 2033 302c 2066 6561  x: int = 30, fea
+00001780: 7475 7265 643a 2062 6f6f 6c20 3d20 5472  tured: bool = Tr
+00001790: 7565 2c20 7265 6775 6c61 723a 2062 6f6f  ue, regular: boo
+000017a0: 6c20 3d20 5472 7565 2929 202d 3e2a 2a0d  l = True)) ->**.
+000017b0: 0a20 2020 200d 0a20 2020 2060 6060 0d0a  .    ..    ```..
+000017c0: 2020 2020 7072 696e 7428 6177 6169 7420      print(await 
+000017d0: 686c 7476 2e67 6574 5f72 6573 756c 7473  hltv.get_results
+000017e0: 2829 290d 0a20 200d 0a20 2020 205b 7b27  ())..  ..    [{'
+000017f0: 6964 273a 2027 3233 3730 3933 3127 2c20  id': '2370931', 
+00001800: 2774 6561 6d31 273a 2027 4d4f 555a 272c  'team1': 'MOUZ',
+00001810: 2027 7465 616d 3227 3a20 2746 615a 6527   'team2': 'FaZe'
+00001820: 2c20 2773 636f 7265 3127 3a20 2730 272c  , 'score1': '0',
+00001830: 2027 7363 6f72 6532 273a 2027 3227 2c20   'score2': '2', 
+00001840: 2772 6174 696e 6727 3a20 302c 2027 6576  'rating': 0, 'ev
+00001850: 656e 7427 3a20 2749 454d 2043 6865 6e67  ent': 'IEM Cheng
+00001860: 6475 2032 3032 3427 7d5d 0d0a 2020 2020  du 2024'}]..    
+00001870: 6060 600d 0a20 200d 0a2a 202a 2a67 6574  ```..  ..* **get
+00001880: 5f65 7665 6e74 7328 6f75 7467 6f69 6e67  _events(outgoing
+00001890: 3d54 7275 652c 2066 7574 7572 653d 5472  =True, future=Tr
+000018a0: 7565 2c20 6d61 785f 6576 656e 7473 3d31  ue, max_events=1
+000018b0: 3029 202d 3e20 5b28 2769 6427 2c20 2774  0) -> [('id', 't
+000018c0: 6974 6c65 272c 2027 7374 6172 7464 6174  itle', 'startdat
+000018d0: 6527 2c20 2765 6e64 6461 7465 2729 5d2a  e', 'enddate')]*
+000018e0: 2a0d 0a0d 0a20 2020 2060 6060 0d0a 2020  *....    ```..  
+000018f0: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+00001900: 5f65 7665 6e74 7328 6675 7475 7265 3d46  _events(future=F
+00001910: 616c 7365 290d 0a20 2020 200d 0a20 2020  alse)..    ..   
+00001920: 203e 3e3e 5b7b 2769 6427 3a20 2737 3734   >>>[{'id': '774
+00001930: 3927 2c20 2774 6974 6c65 273a 2027 5468  9', 'title': 'Th
+00001940: 756e 6465 7270 6963 6b20 576f 726c 6420  underpick World 
+00001950: 4368 616d 7069 6f6e 7368 6970 2032 3032  Championship 202
+00001960: 3420 4555 2043 6c6f 7365 6420 5175 616c  4 EU Closed Qual
+00001970: 6966 6965 7220 3127 2c20 2773 7461 7274  ifier 1', 'start
+00001980: 5f64 6174 6527 3a20 2731 2d34 272c 2027  _date': '1-4', '
+00001990: 656e 645f 6461 7465 273a 2027 3232 2d34  end_date': '22-4
+000019a0: 277d 2c20 7b27 6964 273a 2027 3736 3231  '}, {'id': '7621
+000019b0: 272c 2027 7469 746c 6527 3a20 2745 534c  ', 'title': 'ESL
+000019c0: 2043 6861 6c6c 656e 6765 7220 4c65 6167   Challenger Leag
+000019d0: 7565 2053 6561 736f 6e20 3437 204e 6f72  ue Season 47 Nor
+000019e0: 7468 2041 6d65 7269 6361 272c 2027 7374  th America', 'st
+000019f0: 6172 745f 6461 7465 273a 2027 3133 2d32  art_date': '13-2
+00001a00: 272c 2027 656e 645f 6461 7465 273a 2027  ', 'end_date': '
+00001a10: 3136 2d36 277d 5d0d 0a20 2020 2020 200d  16-6'}]..      .
+00001a20: 0a20 2020 2060 6060 0d0a 0d0a 2a20 2a2a  .    ```....* **
+00001a30: 6765 745f 6576 656e 745f 7265 7375 6c74  get_event_result
+00001a40: 7328 6576 656e 745f 6964 3a20 696e 7420  s(event_id: int 
+00001a50: 7c20 7374 722c 2064 6179 733a 2069 6e74  | str, days: int
+00001a60: 203d 2031 2c20 6d61 785f 3a20 696e 7420   = 1, max_: int 
+00001a70: 3d20 3130 292a 2a0d 0a0d 0a20 200d 0a20  = 10)**....  .. 
+00001a80: 2020 2060 6060 0d0a 2020 2020 6177 6169     ```..    awai
+00001a90: 7420 6765 745f 6576 656e 745f 7265 7375  t get_event_resu
+00001aa0: 6c74 7328 3731 3438 290d 0a20 2020 200d  lts(7148)..    .
+00001ab0: 0a20 2020 203e 3e3e 5b7b 2769 6427 3a20  .    >>>[{'id': 
+00001ac0: 2732 3337 3039 3331 272c 2027 6461 7465  '2370931', 'date
+00001ad0: 273a 2027 3134 2d30 342d 3230 3234 272c  ': '14-04-2024',
+00001ae0: 2027 7465 616d 3127 3a20 274d 4f55 5a27   'team1': 'MOUZ'
+00001af0: 2c20 2774 6561 6d32 273a 2027 4661 5a65  , 'team2': 'FaZe
+00001b00: 272c 2027 7363 6f72 6531 273a 2027 3027  ', 'score1': '0'
+00001b10: 2c20 2773 636f 7265 3227 3a20 2732 277d  , 'score2': '2'}
+00001b20: 5d0d 0a0d 0a20 2020 2060 6060 0d0a 0d0a  ]....    ```....
+00001b30: 2a20 2a2a 6765 745f 6576 656e 745f 6d61  * **get_event_ma
+00001b40: 7463 6865 7328 6576 656e 745f 6964 3a20  tches(event_id: 
+00001b50: 7374 7220 7c20 696e 742c 2064 6179 733a  str | int, days:
+00001b60: 2069 6e74 203d 2031 293a 2a2a 0d0a 2020   int = 1):**..  
+00001b70: 0d0a 2020 2020 6060 600d 0a20 2020 2061  ..    ```..    a
+00001b80: 7761 6974 2068 6c74 762e 6765 745f 6576  wait hltv.get_ev
+00001b90: 656e 745f 6d61 7463 6865 7328 3731 3438  ent_matches(7148
+00001ba0: 290d 0a20 2020 200d 0a20 2020 203e 3e3e  )..    ..    >>>
+00001bb0: 5b7b 2769 6427 3a20 2732 3337 3037 3731  [{'id': '2370771
+00001bc0: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
+00001bd0: 2d30 342d 3138 272c 2027 7469 6d65 273a  -04-18', 'time':
+00001be0: 2027 3135 3a33 3027 2c20 2774 6561 6d31   '15:30', 'team1
+00001bf0: 273a 2027 4d6f 6e74 6527 2c20 2774 6561  ': 'Monte', 'tea
+00001c00: 6d32 273a 2027 7061 694e 272c 2027 7431  m2': 'paiN', 't1
+00001c10: 5f69 6427 3a20 2731 3138 3131 272c 2027  _id': '11811', '
+00001c20: 7432 5f69 6427 3a20 2734 3737 3327 7d2c  t2_id': '4773'},
+00001c30: 207b 2769 6427 3a20 2732 3337 3037 3732   {'id': '2370772
+00001c40: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
+00001c50: 2d30 342d 3138 272c 2027 7469 6d65 273a  -04-18', 'time':
+00001c60: 2027 3137 3a30 3027 2c20 2774 6561 6d31   '17:00', 'team1
+00001c70: 273a 2027 496d 7065 7269 616c 272c 2027  ': 'Imperial', '
+00001c80: 7465 616d 3227 3a20 274d 6574 697a 706f  team2': 'Metizpo
+00001c90: 7274 272c 2027 7431 5f69 6427 3a20 2739  rt', 't1_id': '9
+00001ca0: 3435 3527 2c20 2774 325f 6964 273a 2027  455', 't2_id': '
+00001cb0: 3131 3634 3127 7d2c 207b 2769 6427 3a20  11641'}, {'id': 
+00001cc0: 2732 3337 3037 3733 272c 2027 6461 7465  '2370773', 'date
+00001cd0: 273a 2027 3230 3234 2d30 342d 3138 272c  ': '2024-04-18',
+00001ce0: 2027 7469 6d65 273a 2027 3138 3a33 3027   'time': '18:30'
+00001cf0: 2c20 2774 6561 6d31 273a 2027 4655 5249  , 'team1': 'FURI
+00001d00: 4127 2c20 2774 6561 6d32 273a 2027 397a  A', 'team2': '9z
+00001d10: 272c 2027 7431 5f69 6427 3a20 2738 3239  ', 't1_id': '829
+00001d20: 3727 2c20 2774 325f 6964 273a 2027 3939  7', 't2_id': '99
+00001d30: 3936 277d 2c20 7b27 6964 273a 2027 3233  96'}, {'id': '23
+00001d40: 3730 3737 3427 2c20 2764 6174 6527 3a20  70774', 'date': 
+00001d50: 2732 3032 342d 3034 2d31 3827 2c20 2774  '2024-04-18', 't
+00001d60: 696d 6527 3a20 2732 303a 3030 272c 2027  ime': '20:00', '
+00001d70: 7465 616d 3127 3a20 274d 4942 5227 2c20  team1': 'MIBR', 
+00001d80: 2774 6561 6d32 273a 2027 4f47 272c 2027  'team2': 'OG', '
+00001d90: 7431 5f69 6427 3a20 2739 3231 3527 2c20  t1_id': '9215', 
+00001da0: 2774 325f 6964 273a 2027 3130 3530 3327  't2_id': '10503'
+00001db0: 7d2c 207b 2769 6427 3a20 2732 3337 3037  }, {'id': '23707
+00001dc0: 3735 272c 2027 6461 7465 273a 2027 3230  75', 'date': '20
+00001dd0: 3234 2d30 342d 3138 272c 2027 7469 6d65  24-04-18', 'time
+00001de0: 273a 2027 3231 3a33 3027 2c20 2774 6561  ': '21:30', 'tea
+00001df0: 6d31 273a 2027 5442 4427 2c20 2774 6561  m1': 'TBD', 'tea
+00001e00: 6d32 273a 2027 5442 4427 2c20 2774 315f  m2': 'TBD', 't1_
+00001e10: 6964 273a 2030 2c20 2774 325f 6964 273a  id': 0, 't2_id':
+00001e20: 2030 7d2c 207b 2769 6427 3a20 2732 3337   0}, {'id': '237
+00001e30: 3037 3736 272c 2027 6461 7465 273a 2027  0776', 'date': '
+00001e40: 3230 3234 2d30 342d 3138 272c 2027 7469  2024-04-18', 'ti
+00001e50: 6d65 273a 2027 3233 3a30 3027 2c20 2774  me': '23:00', 't
+00001e60: 6561 6d31 273a 2027 5442 4427 2c20 2774  eam1': 'TBD', 't
+00001e70: 6561 6d32 273a 2027 5442 4427 2c20 2774  eam2': 'TBD', 't
+00001e80: 315f 6964 273a 2030 2c20 2774 325f 6964  1_id': 0, 't2_id
+00001e90: 273a 2030 7d2c 207b 2769 6427 3a20 2732  ': 0}, {'id': '2
+00001ea0: 3337 3037 3737 272c 2027 6461 7465 273a  370777', 'date':
+00001eb0: 2027 3230 3234 2d30 342d 3139 272c 2027   '2024-04-19', '
+00001ec0: 7469 6d65 273a 2027 3030 3a30 3027 2c20  time': '00:00', 
+00001ed0: 2774 6561 6d31 273a 2027 5442 4427 2c20  'team1': 'TBD', 
+00001ee0: 2774 6561 6d32 273a 2027 5442 4427 2c20  'team2': 'TBD', 
+00001ef0: 2774 315f 6964 273a 2030 2c20 2774 325f  't1_id': 0, 't2_
+00001f00: 6964 273a 2030 7d2c 207b 2769 6427 3a20  id': 0}, {'id': 
+00001f10: 2732 3337 3037 3738 272c 2027 6461 7465  '2370778', 'date
+00001f20: 273a 2027 3230 3234 2d30 342d 3139 272c  ': '2024-04-19',
+00001f30: 2027 7469 6d65 273a 2027 3135 3a30 3027   'time': '15:00'
+00001f40: 2c20 2774 6561 6d31 273a 2027 5442 4427  , 'team1': 'TBD'
+00001f50: 2c20 2774 6561 6d32 273a 2027 5442 4427  , 'team2': 'TBD'
+00001f60: 2c20 2774 315f 6964 273a 2030 2c20 2774  , 't1_id': 0, 't
+00001f70: 325f 6964 273a 2030 7d2c 207b 2769 6427  2_id': 0}, {'id'
+00001f80: 3a20 2732 3337 3037 3739 272c 2027 6461  : '2370779', 'da
+00001f90: 7465 273a 2027 3230 3234 2d30 342d 3139  te': '2024-04-19
+00001fa0: 272c 2027 7469 6d65 273a 2027 3137 3a33  ', 'time': '17:3
+00001fb0: 3027 2c20 2774 6561 6d31 273a 2027 5442  0', 'team1': 'TB
+00001fc0: 4427 2c20 2774 6561 6d32 273a 2027 5442  D', 'team2': 'TB
+00001fd0: 4427 2c20 2774 315f 6964 273a 2030 2c20  D', 't1_id': 0, 
+00001fe0: 2774 325f 6964 273a 2030 7d2c 207b 2769  't2_id': 0}, {'i
+00001ff0: 6427 3a20 2732 3337 3037 3830 272c 2027  d': '2370780', '
+00002000: 6461 7465 273a 2027 3230 3234 2d30 342d  date': '2024-04-
+00002010: 3139 272c 2027 7469 6d65 273a 2027 3230  19', 'time': '20
+00002020: 3a30 3027 2c20 2774 6561 6d31 273a 2027  :00', 'team1': '
+00002030: 5442 4427 2c20 2774 6561 6d32 273a 2027  TBD', 'team2': '
+00002040: 5442 4427 2c20 2774 315f 6964 273a 2030  TBD', 't1_id': 0
+00002050: 2c20 2774 325f 6964 273a 2030 7d2c 207b  , 't2_id': 0}, {
+00002060: 2769 6427 3a20 2732 3337 3037 3831 272c  'id': '2370781',
+00002070: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
+00002080: 342d 3139 272c 2027 7469 6d65 273a 2027  4-19', 'time': '
+00002090: 3232 3a33 3027 2c20 2774 6561 6d31 273a  22:30', 'team1':
+000020a0: 2027 5442 4427 2c20 2774 6561 6d32 273a   'TBD', 'team2':
+000020b0: 2027 5442 4427 2c20 2774 315f 6964 273a   'TBD', 't1_id':
+000020c0: 2030 2c20 2774 325f 6964 273a 2030 7d2c   0, 't2_id': 0},
+000020d0: 207b 2769 6427 3a20 2732 3337 3037 3832   {'id': '2370782
+000020e0: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
+000020f0: 2d30 342d 3230 272c 2027 7469 6d65 273a  -04-20', 'time':
+00002100: 2027 3030 3a33 3027 2c20 2774 6561 6d31   '00:30', 'team1
+00002110: 273a 2027 5442 4427 2c20 2774 6561 6d32  ': 'TBD', 'team2
+00002120: 273a 2027 5442 4427 2c20 2774 315f 6964  ': 'TBD', 't1_id
+00002130: 273a 2030 2c20 2774 325f 6964 273a 2030  ': 0, 't2_id': 0
+00002140: 7d2c 207b 2769 6427 3a20 2732 3337 3037  }, {'id': '23707
+00002150: 3833 272c 2027 6461 7465 273a 2027 3230  83', 'date': '20
+00002160: 3234 2d30 342d 3230 272c 2027 7469 6d65  24-04-20', 'time
+00002170: 273a 2027 3135 3a30 3027 2c20 2774 6561  ': '15:00', 'tea
+00002180: 6d31 273a 2027 5442 4427 2c20 2774 6561  m1': 'TBD', 'tea
+00002190: 6d32 273a 2027 5442 4427 2c20 2774 315f  m2': 'TBD', 't1_
+000021a0: 6964 273a 2030 2c20 2774 325f 6964 273a  id': 0, 't2_id':
+000021b0: 2030 7d2c 207b 2769 6427 3a20 2732 3337   0}, {'id': '237
+000021c0: 3037 3834 272c 2027 6461 7465 273a 2027  0784', 'date': '
+000021d0: 3230 3234 2d30 342d 3230 272c 2027 7469  2024-04-20', 'ti
+000021e0: 6d65 273a 2027 3138 3a30 3027 2c20 2774  me': '18:00', 't
+000021f0: 6561 6d31 273a 2027 5442 4427 2c20 2774  eam1': 'TBD', 't
+00002200: 6561 6d32 273a 2027 5442 4427 2c20 2774  eam2': 'TBD', 't
+00002210: 315f 6964 273a 2030 2c20 2774 325f 6964  1_id': 0, 't2_id
+00002220: 273a 2030 7d5d 0d0a 2020 0d0a 2020 2020  ': 0}]..  ..    
+00002230: 6060 600d 0a0d 0a2a 202a 2a67 6574 5f65  ```....* **get_e
+00002240: 7665 6e74 5f69 6e66 6f28 6576 656e 745f  vent_info(event_
+00002250: 6964 3a20 7374 7220 7c20 696e 742c 2065  id: str | int, e
+00002260: 7665 6e74 5f74 6974 6c65 3a20 7374 7229  vent_title: str)
+00002270: 202d 3e20 2865 7665 6e74 5f69 642c 2065   -> (event_id, e
+00002280: 7665 6e74 5f74 6974 6c65 2c20 6576 656e  vent_title, even
+00002290: 745f 7374 6172 742c 2065 7665 6e74 5f65  t_start, event_e
+000022a0: 6e64 2c20 7072 697a 652c 2074 6561 6d5f  nd, prize, team_
+000022b0: 6e75 6d2c 206c 6f63 6174 696f 6e2c 2067  num, location, g
+000022c0: 726f 7570 7329 2a2a 0d0a 0d0a 2020 2020  roups)**....    
+000022d0: 6060 600d 0a20 2020 2061 7761 6974 2068  ```..    await h
+000022e0: 6c74 762e 6765 745f 6576 656e 745f 696e  ltv.get_event_in
+000022f0: 666f 2837 3134 382c 2027 5047 4c20 4353  fo(7148, 'PGL CS
+00002300: 3220 4d61 6a6f 7220 436f 7065 6e68 6167  2 Major Copenhag
+00002310: 656e 3230 3234 2729 0d0a 2020 2020 0d0a  en2024')..    ..
+00002320: 2020 2020 7b27 6964 273a 2037 3134 382c      {'id': 7148,
+00002330: 2027 7469 746c 6527 3a20 2750 474c 2043   'title': 'PGL C
+00002340: 5332 204d 616a 6f72 2043 6f70 656e 6861  S2 Major Copenha
+00002350: 6765 6e32 3032 3427 2c20 2773 7461 7274  gen2024', 'start
+00002360: 273a 2027 3231 2d33 272c 2027 656e 6427  ': '21-3', 'end'
+00002370: 3a20 2733 312d 3327 2c20 2770 7269 7a65  : '31-3', 'prize
+00002380: 273a 2027 2431 2c32 3530 2c30 3030 272c  ': '$1,250,000',
+00002390: 2027 7465 616d 7327 3a20 2731 3627 2c20   'teams': '16', 
+000023a0: 276c 6f63 6174 696f 6e27 3a20 2743 6f70  'location': 'Cop
+000023b0: 656e 6861 6765 6e2c 2044 656e 6d61 726b  enhagen, Denmark
+000023c0: 272c 2027 6772 6f75 7027 3a20 5b5d 7d0d  ', 'group': []}.
+000023d0: 0a20 2020 0d0a 2020 2020 6060 600d 0a0d  .   ..    ```...
+000023e0: 0a0d 0a2a 202a 2a67 6574 5f74 6f70 5f74  ...* **get_top_t
+000023f0: 6561 6d73 286d 6178 5f74 6561 6d73 3d33  eams(max_teams=3
+00002400: 3029 202d 3e20 5b27 7261 6e6b 272c 2027  0) -> ['rank', '
+00002410: 7469 746c 6527 2c20 2770 6f69 6e74 7327  title', 'points'
+00002420: 2c20 2763 6861 6e67 6527 2c20 2769 6427  , 'change', 'id'
+00002430: 5d2a 2a0d 0a0d 0a20 2020 2060 6060 0d0a  ]**....    ```..
+00002440: 2020 2020 6177 6169 7420 686c 7476 2e67      await hltv.g
+00002450: 6574 5f74 6f70 5f74 6561 6d73 2832 290d  et_top_teams(2).
+00002460: 0a20 2020 200d 0a20 2020 203e 3e3e 5b7b  .    ..    >>>[{
+00002470: 2769 6427 3a20 2731 3131 3127 2c20 2772  'id': '1111', 'r
+00002480: 616e 6b27 3a20 2731 272c 2027 7469 746c  ank': '1', 'titl
+00002490: 6527 3a20 2746 615a 6527 2c20 2770 6f69  e': 'FaZe', 'poi
+000024a0: 6e74 7327 3a20 2739 3339 272c 2027 6368  nts': '939', 'ch
+000024b0: 616e 6765 273a 2027 2d27 2c20 2769 6427  ange': '-', 'id'
+000024c0: 3a20 2736 3636 3727 7d2c 207b 2769 6427  : '6667'}, {'id'
+000024d0: 3a20 2731 3131 3127 2c20 2772 616e 6b27  : '1111', 'rank'
+000024e0: 3a20 2732 272c 2027 7469 746c 6527 3a20  : '2', 'title': 
+000024f0: 274e 6174 7573 2056 696e 6365 7265 272c  'Natus Vincere',
+00002500: 2027 706f 696e 7473 273a 2027 3735 3727   'points': '757'
+00002510: 2c20 2763 6861 6e67 6527 3a20 272b 3427  , 'change': '+4'
+00002520: 2c20 2769 6427 3a20 2734 3630 3827 7d5d  , 'id': '4608'}]
+00002530: 0d0a 2020 2020 6060 600d 0a0d 0a2a 202a  ..    ```....* *
+00002540: 2a67 6574 5f74 6561 6d5f 696e 666f 2874  *get_team_info(t
+00002550: 6561 6d5f 6964 3a20 696e 7420 7c20 7374  eam_id: int | st
+00002560: 722c 2074 6974 6c65 3a20 7374 7229 202d  r, title: str) -
+00002570: 3e20 2874 6561 6d5f 6964 2c20 7465 616d  > (team_id, team
+00002580: 5f74 6974 6c65 2c20 7261 6e6b 2c20 7b70  _title, rank, {p
+00002590: 6c61 7965 723a 706c 6179 6572 5f69 647d  layer:player_id}
+000025a0: 2c20 636f 6163 682c 2061 7665 7261 6765  , coach, average
+000025b0: 5f61 6765 2c20 7765 656b 735f 696e 5f74  _age, weeks_in_t
+000025c0: 6f70 5f32 302c 206c 6173 745f 7472 6f70  op_20, last_trop
+000025d0: 6879 2c20 746f 7461 6c5f 7472 6f70 6879  hy, total_trophy
+000025e0: 7329 2a2a 0d0a 0d0a 2020 2020 6060 600d  s)**....    ```.
+000025f0: 0a20 2020 2061 7761 6974 2068 6c74 762e  .    await hltv.
+00002600: 6765 745f 7465 616d 5f69 6e66 6f28 3636  get_team_info(66
+00002610: 3637 2c20 2766 617a 6527 290d 0a20 2020  67, 'faze')..   
+00002620: 200d 0a20 2020 203e 3e3e 2836 3636 372c   ..    >>>(6667,
+00002630: 2027 6661 7a65 272c 2027 3127 2c20 5b27   'faze', '1', ['
+00002640: 6b61 7272 6967 616e 272c 2027 7261 696e  karrigan', 'rain
+00002650: 272c 2027 6672 6f7a 656e 272c 2027 726f  ', 'frozen', 'ro
+00002660: 707a 272c 2027 6272 6f6b 7927 5d2c 2027  pz', 'broky'], '
+00002670: 4e45 4f27 2c20 2732 362e 3627 2c20 2732  NEO', '26.6', '2
+00002680: 3538 272c 2027 4945 4d20 4368 656e 6764  58', 'IEM Chengd
+00002690: 7520 3230 3234 272c 2032 3229 0d0a 2020  u 2024', 22)..  
+000026a0: 2020 6060 600d 0a0d 0a2a 202a 2a67 6574    ```....* **get
+000026b0: 5f6c 6173 745f 6e65 7773 286d 6178 5f72  _last_news(max_r
+000026c0: 6567 5f6e 6577 733d 322c 206f 6e6c 795f  eg_news=2, only_
+000026d0: 746f 6461 793d 5472 7565 2c20 6f6e 6c79  today=True, only
+000026e0: 5f66 6561 7475 7265 643d 4661 6c73 6529  _featured=False)
+000026f0: 202d 3e20 5b64 6174 652c 205b 6665 6174   -> [date, [feat
+00002700: 7572 6564 5f69 642c 2066 6561 7475 7265  ured_id, feature
+00002710: 645f 7469 746c 652c 2066 6561 7475 7265  d_title, feature
+00002720: 645f 6465 7363 6970 7469 6f6e 5d2c 205b  d_desciption], [
+00002730: 7265 6775 6c61 725f 6964 2c20 7265 675f  regular_id, reg_
+00002740: 7469 746c 652c 2072 6567 5f74 696d 655d  title, reg_time]
+00002750: 5d2a 2a0d 0a0d 0a20 2020 2060 6060 0d0a  ]**....    ```..
+00002760: 2020 2020 6177 6169 7420 686c 7476 2e67      await hltv.g
+00002770: 6574 5f6c 6173 745f 6e65 7773 286f 6e6c  et_last_news(onl
+00002780: 795f 746f 6461 793d 5472 7565 290d 0a20  y_today=True).. 
+00002790: 2020 200d 0a20 2020 203e 3e3e 5b7b 2764     ..    >>>[{'d
+000027a0: 6174 6527 3a20 2731 352d 3034 272c 2027  ate': '15-04', '
+000027b0: 665f 6e65 7773 273a 205b 5d2c 2027 6e65  f_news': [], 'ne
+000027c0: 7773 273a 205b 7b27 6964 273a 2027 3338  ws': [{'id': '38
+000027d0: 3738 3427 2c20 2774 6974 6c65 273a 2027  784', 'title': '
+000027e0: 4d65 6469 613a 2046 5552 4941 2070 7261  Media: FURIA pra
+000027f0: 6374 6963 696e 6720 7769 7468 206b 7965  cticing with kye
+00002800: 2069 6e20 706c 6163 6520 6f66 2061 7254   in place of arT
+00002810: 272c 2027 706f 7374 6564 273a 2027 616e  ', 'posted': 'an
+00002820: 2068 6f75 7220 6167 6f27 7d2c 207b 2769   hour ago'}, {'i
+00002830: 6427 3a20 2733 3837 3833 272c 2027 7469  d': '38783', 'ti
+00002840: 746c 6527 3a20 2765 6c65 6374 726f 4e69  tle': 'electroNi
+00002850: 6320 746f 2070 6c61 7920 666f 7220 5669  c to play for Vi
+00002860: 7274 7573 2e70 726f 2061 7420 4553 4c20  rtus.pro at ESL 
+00002870: 5072 6f20 4c65 6167 7565 2053 3139 272c  Pro League S19',
+00002880: 2027 706f 7374 6564 273a 2027 3220 686f   'posted': '2 ho
+00002890: 7572 7320 6167 6f27 7d2c 207b 2769 6427  urs ago'}, {'id'
+000028a0: 3a20 2733 3837 3831 272c 2027 7469 746c  : '38781', 'titl
+000028b0: 6527 3a20 2754 6865 2045 5650 7320 616e  e': 'The EVPs an
+000028c0: 6420 4265 7374 2046 6976 6520 6f66 2049  d Best Five of I
+000028d0: 454d 2043 6865 6e67 6475 272c 2027 706f  EM Chengdu', 'po
+000028e0: 7374 6564 273a 2027 3720 686f 7572 7320  sted': '7 hours 
+000028f0: 6167 6f27 7d5d 7d5d 0d0a 2020 0d0a 2020  ago'}]}]..  ..  
+00002900: 2020 6060 600d 0a0d 0a2a 202a 2a67 6574    ```....* **get
+00002910: 5f62 6573 745f 706c 6179 6572 7328 746f  _best_players(to
+00002920: 703a 2069 6e74 203d 2034 3029 202d 3e20  p: int = 40) -> 
+00002930: 2827 7261 6e6b 272c 2027 6e61 6d65 272c  ('rank', 'name',
+00002940: 2027 7465 616d 272c 2027 6d61 7073 272c   'team', 'maps',
+00002950: 2027 7261 7469 6e67 2729 2a2a 0d0a 0d0a   'rating')**....
+00002960: 2020 2020 6060 600d 0a20 2020 2061 7761      ```..    awa
+00002970: 6974 2068 6c74 762e 6765 745f 6265 7374  it hltv.get_best
+00002980: 5f70 6c61 7965 7273 2832 290d 0a20 2020  _players(2)..   
+00002990: 200d 0a20 2020 203e 3e3e 5b7b 2769 6427   ..    >>>[{'id'
+000029a0: 3a20 2731 3932 3330 272c 2027 7261 6e6b  : '19230', 'rank
+000029b0: 273a 2031 2c20 276e 616d 6527 3a20 276d  ': 1, 'name': 'm
+000029c0: 304e 4553 5927 2c20 2774 6561 6d27 3a20  0NESY', 'team': 
+000029d0: 2747 3227 2c20 276d 6170 7327 3a20 2734  'G2', 'maps': '4
+000029e0: 3427 2c20 2772 6174 696e 6727 3a20 2731  4', 'rating': '1
+000029f0: 2e33 3727 7d2c 207b 2769 6427 3a20 2731  .37'}, {'id': '1
+00002a00: 3830 3533 272c 2027 7261 6e6b 273a 2032  8053', 'rank': 2
+00002a10: 2c20 276e 616d 6527 3a20 2762 726f 6b79  , 'name': 'broky
+00002a20: 272c 2027 7465 616d 273a 2027 4661 5a65  ', 'team': 'FaZe
+00002a30: 272c 2027 6d61 7073 273a 2027 3534 272c  ', 'maps': '54',
+00002a40: 2027 7261 7469 6e67 273a 2027 312e 3139   'rating': '1.19
+00002a50: 277d 5d0d 0a20 2020 2060 6060 0d0a 0d0a  '}]..    ```....
+00002a60: 2a20 2a2a 6765 745f 706c 6179 6572 5f69  * **get_player_i
+00002a70: 6e66 6f28 6964 3a20 7374 7220 7c20 696e  nfo(id: str | in
+00002a80: 742c 206e 6963 6b6e 616d 653a 2073 7472  t, nickname: str
+00002a90: 292a 2a0d 0a20 200d 0a20 2060 6060 0d0a  )**..  ..  ```..
+00002aa0: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+00002ab0: 5f70 6c61 7965 725f 696e 666f 2837 3939  _player_info(799
+00002ac0: 382c 2027 7331 6d70 6c65 2729 0d0a 2020  8, 's1mple')..  
+00002ad0: 0d0a 2020 7b27 6964 273a 2037 3939 382c  ..  {'id': 7998,
+00002ae0: 2027 6e69 636b 6e61 6d65 273a 2027 7331   'nickname': 's1
+00002af0: 6d70 6c65 272c 2027 7465 616d 273a 2027  mple', 'team': '
+00002b00: 4e61 7475 7320 5669 6e63 6572 6527 2c20  Natus Vincere', 
+00002b10: 2774 6561 6d5f 6964 273a 2034 3630 382c  'team_id': 4608,
+00002b20: 2027 6e61 6d65 273a 2027 4f6c 656b 7361   'name': 'Oleksa
+00002b30: 6e64 7220 4b6f 7374 796c 6965 7627 2c20  ndr Kostyliev', 
+00002b40: 276e 6174 696f 6e61 6c69 7479 273a 2027  'nationality': '
+00002b50: 556b 7261 696e 6527 2c20 2761 6765 273a  Ukraine', 'age':
+00002b60: 2032 362c 2027 7261 7469 6e67 273a 2027   26, 'rating': '
+00002b70: 302e 3934 272c 2027 6b70 7227 3a20 2730  0.94', 'kpr': '0
+00002b80: 2e36 3027 2c20 2768 7327 3a20 2735 372e  .60', 'hs': '57.
+00002b90: 3925 272c 2027 6c61 7374 5f6d 6174 6368  9%', 'last_match
+00002ba0: 6573 273a 205b 3130 3330 3539 2c20 3939  es': [103059, 99
+00002bb0: 3734 352c 2039 3937 3238 2c20 3939 3639  745, 99728, 9969
+00002bc0: 362c 2039 3934 3731 2c20 3939 3336 345d  6, 99471, 99364]
+00002bd0: 2c20 276c 6173 745f 7472 6f70 6879 273a  , 'last_trophy':
+00002be0: 2027 424c 4153 5420 5072 656d 6965 7220   'BLAST Premier 
+00002bf0: 5370 7269 6e67 2046 696e 616c 2032 3032  Spring Final 202
+00002c00: 3227 2c20 2774 6f74 616c 5f74 726f 7068  2', 'total_troph
+00002c10: 6965 7327 3a20 3330 2c20 2774 6f74 616c  ies': 30, 'total
+00002c20: 5f6d 7670 7327 3a20 3231 7d0d 0a20 2060  _mvps': 21}..  `
+00002c30: 6060 0d0a 0d0a 2a20 2a2a 6765 7428 7479  ``....* **get(ty
+00002c40: 7065 3a20 7374 722c 2069 643a 2069 6e74  pe: str, id: int
+00002c50: 207c 2073 7472 207c 204e 6f6e 6520 3d20   | str | None = 
+00002c60: 4e6f 6e65 2c20 7469 746c 653a 2073 7472  None, title: str
+00002c70: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c20   | None = None, 
+00002c80: 7465 616d 313a 2073 7472 207c 204e 6f6e  team1: str | Non
+00002c90: 6520 3d20 4e6f 6e65 2c20 7465 616d 323a  e = None, team2:
+00002ca0: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
+00002cb0: 6e65 293a 2a2a 0d0a 2020 2842 4554 4129  ne):**..  (BETA)
+00002cc0: 2054 6869 7320 6d65 7468 6f64 2069 7320   This method is 
+00002cd0: 6e6f 7420 6669 6e69 7368 6564 2e20 506f  not finished. Po
+00002ce0: 7373 6962 6c65 2074 7970 6573 2027 6576  ssible types 'ev
+00002cf0: 656e 7473 272c 2027 6d61 7463 6865 7327  ents', 'matches'
+00002d00: 2c20 2774 6561 6d73 272c 2061 6c73 6f20  , 'teams', also 
+00002d10: 7520 6361 6e20 6164 6420 6964 207c 2074  u can add id | t
+00002d20: 6974 6c65 207c 2074 6561 6d31 207c 2074  itle | team1 | t
+00002d30: 6561 6d32 2c20 746f 2070 6172 7365 206d  eam2, to parse m
+00002d40: 6f72 652e 0d0a 2020 0d0a 2020 6060 600d  ore...  ..  ```.
+00002d50: 0a20 200d 0a20 2061 7761 6974 2068 6c74  .  ..  await hlt
+00002d60: 762e 6765 7428 276d 6174 6368 6573 272c  v.get('matches',
+00002d70: 2032 3337 3132 3031 2c20 2772 6573 2d72   2371201, 'res-r
+00002d80: 6567 696f 6e61 6c2d 7365 7269 6573 2d33  egional-series-3
+00002d90: 2d6c 6174 616d 272c 2027 494d 5045 5249  -latam', 'IMPERI
+00002da0: 414c 272c 2027 4d49 4252 2729 0d0a 2020  AL', 'MIBR')..  
+00002db0: 0d0a 2020 3e3e 3e20 2832 3337 3132 3031  ..  >>> (2371201
+00002dc0: 2c20 302c 2030 2c20 274c 4956 4527 2c20  , 0, 0, 'LIVE', 
+00002dd0: 5b7b 276d 6170 6e61 6d65 273a 2027 5665  [{'mapname': 'Ve
+00002de0: 7274 6967 6f27 2c20 2772 5f74 6561 6d31  rtigo', 'r_team1
+00002df0: 273a 2027 3627 2c20 2772 5f74 6561 6d32  ': '6', 'r_team2
+00002e00: 273a 2027 3133 277d 2c20 7b27 6d61 706e  ': '13'}, {'mapn
+00002e10: 616d 6527 3a20 274d 6972 6167 6527 2c20  ame': 'Mirage', 
+00002e20: 2772 5f74 6561 6d31 273a 2027 2d27 2c20  'r_team1': '-', 
+00002e30: 2772 5f74 6561 6d32 273a 2027 2d27 7d2c  'r_team2': '-'},
+00002e40: 207b 276d 6170 6e61 6d65 273a 2027 416e   {'mapname': 'An
+00002e50: 7562 6973 272c 2027 725f 7465 616d 3127  ubis', 'r_team1'
+00002e60: 3a20 272d 272c 2027 725f 7465 616d 3227  : '-', 'r_team2'
+00002e70: 3a20 272d 277d 5d2c 205b 5d29 0d0a 2020  : '-'}], [])..  
+00002e80: 0d0a 2020 6060 600d 0a0d 0a0d 0a2d 2d2d  ..  ```......---
+00002e90: 0d0a 2320 4578 616d 706c 6573 0d0a 0d0a  ..# Examples....
+00002ea0: 2a2a 2a2a 5369 6d70 6c65 2045 7861 6d70  ****Simple Examp
+00002eb0: 6c65 2a2a 2a2a 0d0a 0d0a 6060 600d 0a66  le****....```..f
+00002ec0: 726f 6d20 686c 7476 5f61 7379 6e63 5f61  rom hltv_async_a
+00002ed0: 7069 2069 6d70 6f72 7420 486c 7476 0d0a  pi import Hltv..
+00002ee0: 0d0a 0d0a 6173 796e 6320 6465 6620 7465  ....async def te
+00002ef0: 7374 2829 3a0d 0a0d 0a20 2020 2061 7379  st():....    asy
+00002f00: 6e63 2077 6974 6820 486c 7476 2829 2061  nc with Hltv() a
+00002f10: 7320 686c 7476 3a0d 0a20 2020 2020 2070  s hltv:..      p
+00002f20: 7269 6e74 2861 7761 6974 2068 6c74 762e  rint(await hltv.
+00002f30: 6765 745f 6576 656e 745f 696e 666f 2837  get_event_info(7
+00002f40: 3134 382c 2027 7067 6c2d 6373 322d 6d61  148, 'pgl-cs2-ma
+00002f50: 6a6f 722d 636f 7065 6e68 6167 656e 2d32  jor-copenhagen-2
+00002f60: 3032 3427 2929 0d0a 0d0a 6966 205f 5f6e  024'))....if __n
+00002f70: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00002f80: 5f5f 223a 0d0a 2020 2020 6173 796e 6369  __":..    asynci
+00002f90: 6f2e 7275 6e28 7465 7374 2829 290d 0a60  o.run(test())..`
+00002fa0: 6060 0d0a 0d0a 2a2a 2a2a 5072 6f78 7920  ``....****Proxy 
+00002fb0: 5061 7273 6572 2a2a 2a2a 0d0a 0d0a 6060  Parser****....``
+00002fc0: 600d 0a66 726f 6d20 686c 7476 5f61 7379  `..from hltv_asy
+00002fd0: 6e63 5f61 7069 2069 6d70 6f72 7420 486c  nc_api import Hl
+00002fe0: 7476 0d0a 0d0a 0d0a 6173 796e 6320 6465  tv......async de
+00002ff0: 6620 7465 7374 2829 3a0d 0a0d 0a20 2020  f test():....   
+00003000: 2068 6c74 7620 3d20 486c 7476 2864 6562   hltv = Hltv(deb
+00003010: 7567 3d54 7275 652c 2070 726f 7879 5f70  ug=True, proxy_p
+00003020: 6174 683d 2770 726f 7879 5f74 6573 742e  ath='proxy_test.
+00003030: 7478 7427 2c20 7469 6d65 6f75 743d 312c  txt', timeout=1,
+00003040: 2064 656c 6574 655f 7072 6f78 793d 5472   delete_proxy=Tr
+00003050: 7565 2c20 7072 6f78 795f 7072 6f74 6f63  ue, proxy_protoc
+00003060: 6f6c 3d27 6874 7470 2729 0d0a 2020 2020  ol='http')..    
+00003070: 0d0a 2020 2020 7072 696e 7428 6177 6169  ..    print(awai
+00003080: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
+00003090: 5f69 6e66 6f28 3731 3438 2c20 2770 676c  _info(7148, 'pgl
+000030a0: 2d63 7332 2d6d 616a 6f72 2d63 6f70 656e  -cs2-major-copen
+000030b0: 6861 6765 6e2d 3230 3234 2729 290d 0a0d  hagen-2024'))...
+000030c0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+000030d0: 225f 5f6d 6169 6e5f 5f22 3a0d 0a20 2020  "__main__":..   
+000030e0: 2061 7379 6e63 696f 2e72 756e 2874 6573   asyncio.run(tes
+000030f0: 7428 2929 0d0a 6060 600d 0a0d 0a2a 2a2a  t())..```....***
+00003100: 2a41 7574 6f6d 6174 6963 2070 6172 7365  *Automatic parse
+00003110: 7220 7769 7468 2061 7271 2061 6e64 2072  r with arq and r
+00003120: 6564 6973 2a2a 2a2a 0d0a 0d0a 2d20 746f  edis****....- to
+00003130: 2072 756e 2074 7970 6520 2261 7271 2050   run type "arq P
+00003140: 4154 485f 544f 5f46 494c 452e 576f 726b  ATH_TO_FILE.Work
+00003150: 6572 5365 7474 696e 6773 220d 0a0d 0a20  erSettings".... 
+00003160: 2020 2060 6060 0d0a 2020 2020 696d 706f     ```..    impo
+00003170: 7274 2075 6a73 6f6e 0d0a 2020 2020 696d  rt ujson..    im
+00003180: 706f 7274 2061 7379 6e63 696f 0d0a 2020  port asyncio..  
+00003190: 2020 6672 6f6d 2061 7271 2069 6d70 6f72    from arq impor
+000031a0: 7420 6372 6f6e 0d0a 2020 2020 6672 6f6d  t cron..    from
+000031b0: 2072 6564 6973 2e61 7379 6e63 696f 2069   redis.asyncio i
+000031c0: 6d70 6f72 7420 5265 6469 732c 2043 6f6e  mport Redis, Con
+000031d0: 6e65 6374 696f 6e50 6f6f 6c0d 0a20 2020  nectionPool..   
+000031e0: 200d 0a20 2020 2066 726f 6d20 686c 7476   ..    from hltv
+000031f0: 5f61 7379 6e63 5f61 7069 2069 6d70 6f72  _async_api impor
+00003200: 7420 486c 7476 0d0a 2020 2020 0d0a 2020  t Hltv..    ..  
+00003210: 2020 0d0a 2020 2020 0d0a 2020 2020 6173    ..    ..    as
+00003220: 796e 6320 6465 6620 7374 6172 7475 7028  ync def startup(
+00003230: 6374 7829 3a0d 0a20 2020 2020 2020 2061  ctx):..        a
+00003240: 7379 6e63 2077 6974 6820 486c 7476 286d  sync with Hltv(m
+00003250: 6178 5f64 656c 6179 3d35 2c20 7072 6f78  ax_delay=5, prox
+00003260: 795f 7061 7468 3d27 7072 6f78 6965 732e  y_path='proxies.
+00003270: 7478 7427 2c20 6465 6275 673d 5472 7565  txt', debug=True
+00003280: 2920 6173 2068 6c74 763a 0d0a 2020 2020  ) as hltv:..    
+00003290: 2020 2020 2020 2020 2020 6374 785b 2268            ctx["h
+000032a0: 6c74 7622 5d20 3d20 686c 7476 0d0a 2020  ltv"] = hltv..  
+000032b0: 0d0a 2020 2020 2020 2020 6374 785b 2272  ..        ctx["r
+000032c0: 6564 6973 225d 203d 2072 6564 6973 5f63  edis"] = redis_c
+000032d0: 6c69 656e 7420 3d20 5265 6469 7328 0d0a  lient = Redis(..
+000032e0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+000032f0: 6563 7469 6f6e 5f70 6f6f 6c3d 436f 6e6e  ection_pool=Conn
+00003300: 6563 7469 6f6e 506f 6f6c 2e66 726f 6d5f  ectionPool.from_
+00003310: 7572 6c28 7365 7474 696e 6773 2e72 6564  url(settings.red
+00003320: 6973 5f75 726c 2929 0d0a 2020 2020 2020  is_url))..      
+00003330: 2020 6c6f 6767 6572 2e73 7563 6365 7373    logger.success
+00003340: 2866 2253 6368 6564 756c 6572 2073 7461  (f"Scheduler sta
+00003350: 7274 6564 2e20 5554 4320 7469 6d65 207b  rted. UTC time {
+00003360: 6461 7465 7469 6d65 2e75 7463 6e6f 7728  datetime.utcnow(
+00003370: 297d 2229 0d0a 2020 2020 0d0a 2020 2020  )}")..    ..    
+00003380: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00003390: 7368 7574 646f 776e 2863 7478 293a 0d0a  shutdown(ctx):..
+000033a0: 2020 2020 2020 2020 6177 6169 7420 6374          await ct
+000033b0: 785b 2272 6564 6973 225d 2e63 6c6f 7365  x["redis"].close
+000033c0: 2829 0d0a 2020 2020 0d0a 2020 2020 0d0a  ()..    ..    ..
+000033d0: 2020 2020 6173 796e 6320 6465 6620 7061      async def pa
+000033e0: 7273 655f 6d61 7463 6865 7328 6374 7829  rse_matches(ctx)
+000033f0: 3a0d 0a20 2020 2020 2020 2068 6c74 7620  :..        hltv 
+00003400: 3d20 6374 785b 2268 6c74 7622 5d0d 0a20  = ctx["hltv"].. 
+00003410: 2020 2020 2020 2072 6564 6973 203d 2063         redis = c
+00003420: 7478 5b22 7265 6469 7322 5d0d 0a20 2020  tx["redis"]..   
+00003430: 2020 2020 206d 6174 6368 6573 203d 2061       matches = a
+00003440: 7761 6974 2068 6c74 762e 6765 745f 7570  wait hltv.get_up
+00003450: 636f 6d69 6e67 5f6d 6174 6368 6573 2831  coming_matches(1
+00003460: 2c20 3129 0d0a 2020 2020 2020 2020 6966  , 1)..        if
+00003470: 206d 6174 6368 6573 3a0d 0a20 2020 2020   matches:..     
+00003480: 2020 2020 2020 2061 7761 6974 2072 6564         await red
+00003490: 6973 2e73 6574 2822 6d61 7463 6865 7322  is.set("matches"
+000034a0: 2c20 756a 736f 6e2e 6475 6d70 7328 6d61  , ujson.dumps(ma
+000034b0: 7463 6865 7329 290d 0a20 2020 2020 2020  tches))..       
+000034c0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000034d0: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
+000034e0: 2822 6572 726f 7220 7061 7273 696e 6720  ("error parsing 
+000034f0: 6d61 7463 6865 7322 290d 0a20 2020 200d  matches")..    .
+00003500: 0a20 2020 2061 7379 6e63 2064 6566 2070  .    async def p
+00003510: 6172 7365 5f65 7665 6e74 7328 6374 7829  arse_events(ctx)
+00003520: 3a0d 0a20 2020 2020 2020 2068 6c74 7620  :..        hltv 
+00003530: 3d20 6374 785b 2268 6c74 7622 5d0d 0a20  = ctx["hltv"].. 
+00003540: 2020 2020 2020 2072 6564 6973 203d 2063         redis = c
+00003550: 7478 5b22 7265 6469 7322 5d0d 0a20 2020  tx["redis"]..   
+00003560: 2020 2020 2065 7665 6e74 7320 3d20 6177       events = aw
+00003570: 6169 7420 686c 7476 2e67 6574 5f65 7665  ait hltv.get_eve
+00003580: 6e74 7328 290d 0a20 2020 2020 2020 2069  nts()..        i
+00003590: 6620 6576 656e 7473 3a0d 0a20 2020 2020  f events:..     
+000035a0: 2020 2020 2020 2061 7761 6974 2072 6564         await red
+000035b0: 6973 2e73 6574 2822 6576 656e 7473 222c  is.set("events",
+000035c0: 2075 6a73 6f6e 2e64 756d 7073 2865 7665   ujson.dumps(eve
+000035d0: 6e74 7329 290d 0a20 2020 2020 2020 2065  nts))..        e
+000035e0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000035f0: 2020 6c6f 6767 6572 2e65 7272 6f72 2822    logger.error("
+00003600: 6572 726f 7220 7061 7273 696e 6720 6576  error parsing ev
+00003610: 656e 7473 2229 0d0a 2020 2020 0d0a 2020  ents")..    ..  
+00003620: 2020 0d0a 2020 2020 6173 796e 6320 6465    ..    async de
+00003630: 6620 7061 7273 655f 746f 705f 7465 616d  f parse_top_team
+00003640: 7328 6374 7829 3a0d 0a20 2020 2020 2020  s(ctx):..       
+00003650: 2068 6c74 7620 3d20 6374 785b 2268 6c74   hltv = ctx["hlt
+00003660: 7622 5d0d 0a20 2020 2020 2020 2072 6564  v"]..        red
+00003670: 6973 203d 2063 7478 5b22 7265 6469 7322  is = ctx["redis"
+00003680: 5d0d 0a20 2020 2020 2020 2074 6f70 5f74  ]..        top_t
+00003690: 6561 6d73 203d 2061 7761 6974 2068 6c74  eams = await hlt
+000036a0: 762e 6765 745f 746f 705f 7465 616d 7328  v.get_top_teams(
+000036b0: 3330 290d 0a20 2020 2020 2020 2069 6620  30)..        if 
+000036c0: 746f 705f 7465 616d 733a 0d0a 2020 2020  top_teams:..    
+000036d0: 2020 2020 2020 2020 6177 6169 7420 7265          await re
+000036e0: 6469 732e 7365 7428 2274 6f70 5f74 6561  dis.set("top_tea
+000036f0: 6d73 222c 2075 6a73 6f6e 2e64 756d 7073  ms", ujson.dumps
+00003700: 2874 6f70 5f74 6561 6d73 2929 0d0a 2020  (top_teams))..  
+00003710: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00003720: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00003730: 6572 726f 7228 2265 7272 6f72 2070 6172  error("error par
+00003740: 7369 6e67 2074 6f70 2074 6561 6d73 2229  sing top teams")
+00003750: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
+00003760: 2020 6173 796e 6320 6465 6620 7061 7273    async def pars
+00003770: 655f 746f 705f 706c 6179 6572 7328 6374  e_top_players(ct
+00003780: 7829 3a0d 0a20 2020 2020 2020 2068 6c74  x):..        hlt
+00003790: 7620 3d20 6374 785b 2268 6c74 7622 5d0d  v = ctx["hltv"].
+000037a0: 0a20 2020 2020 2020 2072 6564 6973 203d  .        redis =
+000037b0: 2063 7478 5b22 7265 6469 7322 5d0d 0a20   ctx["redis"].. 
+000037c0: 2020 2020 2020 2074 6f70 5f70 6c61 7965         top_playe
+000037d0: 7273 203d 2061 7761 6974 2068 6c74 762e  rs = await hltv.
+000037e0: 6765 745f 6265 7374 5f70 6c61 7965 7273  get_best_players
+000037f0: 2833 3029 0d0a 2020 2020 2020 2020 6966  (30)..        if
+00003800: 2074 6f70 5f70 6c61 7965 7273 3a0d 0a20   top_players:.. 
+00003810: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00003820: 2072 6564 6973 2e73 6574 2822 746f 705f   redis.set("top_
+00003830: 7465 616d 7322 2c20 756a 736f 6e2e 6475  teams", ujson.du
+00003840: 6d70 7328 746f 705f 706c 6179 6572 7329  mps(top_players)
+00003850: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00003860: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00003870: 6767 6572 2e65 7272 6f72 2822 6572 726f  gger.error("erro
+00003880: 7220 7061 7273 696e 6720 746f 7020 706c  r parsing top pl
+00003890: 6179 6572 7322 290d 0a20 2020 200d 0a20  ayers")..    .. 
+000038a0: 2020 200d 0a20 2020 2061 7379 6e63 2064     ..    async d
+000038b0: 6566 2070 6172 7365 5f6c 6173 745f 6e65  ef parse_last_ne
+000038c0: 7773 2863 7478 293a 0d0a 2020 2020 2020  ws(ctx):..      
+000038d0: 2020 686c 7476 203d 2063 7478 5b22 686c    hltv = ctx["hl
+000038e0: 7476 225d 0d0a 2020 2020 2020 2020 7265  tv"]..        re
+000038f0: 6469 7320 3d20 6374 785b 2272 6564 6973  dis = ctx["redis
+00003900: 225d 0d0a 2020 2020 2020 2020 6e65 7773  "]..        news
+00003910: 203d 2061 7761 6974 2068 6c74 762e 6765   = await hltv.ge
+00003920: 745f 6c61 7374 5f6e 6577 7328 6f6e 6c79  t_last_news(only
+00003930: 5f74 6f64 6179 3d54 7275 652c 206d 6178  _today=True, max
+00003940: 5f72 6567 5f6e 6577 733d 3429 0d0a 2020  _reg_news=4)..  
+00003950: 2020 2020 2020 6966 206e 6577 733a 0d0a        if news:..
+00003960: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00003970: 7420 7265 6469 732e 7365 7428 226e 6577  t redis.set("new
+00003980: 7322 2c20 756a 736f 6e2e 6475 6d70 7328  s", ujson.dumps(
+00003990: 6e65 7773 2929 0d0a 2020 2020 2020 2020  news))..        
+000039a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000039b0: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
+000039c0: 2265 7272 6f72 2070 6172 7369 6e67 206e  "error parsing n
+000039d0: 6577 7322 290d 0a20 2020 200d 0a20 2020  ews")..    ..   
+000039e0: 200d 0a20 2020 2063 6c61 7373 2057 6f72   ..    class Wor
+000039f0: 6b65 7253 6574 7469 6e67 733a 0d0a 2020  kerSettings:..  
+00003a00: 2020 2020 2020 7265 6469 735f 7365 7474        redis_sett
+00003a10: 696e 6773 203d 2073 6574 7469 6e67 732e  ings = settings.
+00003a20: 7265 6469 735f 706f 6f6c 0d0a 2020 2020  redis_pool..    
+00003a30: 2020 2020 6f6e 5f73 7461 7274 7570 203d      on_startup =
+00003a40: 2073 7461 7274 7570 0d0a 2020 2020 2020   startup..      
+00003a50: 2020 6f6e 5f73 6875 7464 6f77 6e20 3d20    on_shutdown = 
+00003a60: 7368 7574 646f 776e 0d0a 2020 2020 2020  shutdown..      
+00003a70: 2020 6675 6e63 7469 6f6e 7320 3d20 5b70    functions = [p
+00003a80: 6172 7365 5f6d 6174 6368 6573 2c0d 0a20  arse_matches,.. 
+00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003aa0: 2020 2020 7061 7273 655f 6576 656e 7473      parse_events
+00003ab0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003ac0: 2020 2020 2020 2020 7061 7273 655f 746f          parse_to
+00003ad0: 705f 7465 616d 732c 0d0a 2020 2020 2020  p_teams,..      
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003af0: 6172 7365 5f74 6f70 5f70 6c61 7965 7273  arse_top_players
+00003b00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003b10: 2020 2020 2020 2020 7061 7273 655f 6c61          parse_la
+00003b20: 7374 5f6e 6577 732c 0d0a 2020 2020 2020  st_news,..      
+00003b30: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00003b40: 0d0a 2020 2020 2020 2020 6372 6f6e 5f6a  ..        cron_j
+00003b50: 6f62 7320 3d20 5b0d 0a20 2020 2020 2020  obs = [..       
+00003b60: 2020 2020 2063 726f 6e28 7061 7273 655f       cron(parse_
+00003b70: 6d61 7463 6865 732c 206d 696e 7574 653d  matches, minute=
+00003b80: 3539 292c 0d0a 2020 2020 2020 2020 2020  59),..          
+00003b90: 2020 6372 6f6e 2870 6172 7365 5f65 7665    cron(parse_eve
+00003ba0: 6e74 732c 2068 6f75 723d 302c 206d 696e  nts, hour=0, min
+00003bb0: 7574 653d 302c 2073 6563 6f6e 643d 3029  ute=0, second=0)
+00003bc0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00003bd0: 726f 6e28 7061 7273 655f 746f 705f 7465  ron(parse_top_te
+00003be0: 616d 732c 2064 6179 3d30 2c20 686f 7572  ams, day=0, hour
+00003bf0: 3d31 382c 206d 696e 7574 653d 312c 2073  =18, minute=1, s
+00003c00: 6563 6f6e 643d 3330 292c 0d0a 2020 2020  econd=30),..    
+00003c10: 2020 2020 2020 2020 6372 6f6e 2870 6172          cron(par
+00003c20: 7365 5f74 6f70 5f70 6c61 7965 7273 2c20  se_top_players, 
+00003c30: 6461 793d 302c 2068 6f75 723d 3230 2c20  day=0, hour=20, 
+00003c40: 6d69 6e75 7465 3d30 2c20 7365 636f 6e64  minute=0, second
+00003c50: 3d30 292c 0d0a 2020 2020 2020 2020 2020  =0),..          
+00003c60: 2020 6372 6f6e 2870 6172 7365 5f6c 6173    cron(parse_las
+00003c70: 745f 6e65 7773 2c20 6d69 6e75 7465 3d35  t_news, minute=5
+00003c80: 3529 2c0d 0a20 2020 2020 2020 205d 0d0a  5),..        ]..
+00003c90: 0d0a 2020 2020 6060 600d 0a0d 0a23 2054  ..    ```....# T
+00003ca0: 6573 7473 3a0d 0a0d 0a2a 2a3c 6120 6872  ests:....**<a hr
+00003cb0: 6566 3d27 6874 7470 733a 2f2f 6769 7468  ef='https://gith
+00003cc0: 7562 2e63 6f6d 2f61 6b69 6d65 7273 6c79  ub.com/akimersly
+00003cd0: 732f 686c 7476 2d61 7379 6e63 2d61 7069  s/hltv-async-api
+00003ce0: 2f62 6c6f 622f 6d61 696e 2f74 6573 742f  /blob/main/test/
+00003cf0: 6861 7264 5f74 6573 742e 7079 273e 546f  hard_test.py'>To
+00003d00: 2074 6573 7420 6c69 6272 6172 7920 796f   test library yo
+00003d10: 7520 6361 6e20 7573 6520 7465 6d70 6f72  u can use tempor
+00003d20: 6172 696c 7920 7465 7374 2066 696c 653c  arily test file<
+00003d30: 2f61 3e2a 2a0d 0a0d 0a60 6060 0d0a 0d0a  /a>**....```....
+00003d40: 5061 7273 6564 2032 3038 206d 6174 6368  Parsed 208 match
+00003d50: 6573 2e28 3937 7329 2045 5252 4f52 533a  es.(97s) ERRORS:
+00003d60: 2030 2f32 3038 0d0a 5061 7273 6564 2032   0/208..Parsed 2
+00003d70: 3520 6576 656e 7473 2e28 3233 7329 2045  5 events.(23s) E
+00003d80: 5252 4f52 533a 2030 2f32 350d 0a50 6172  RRORS: 0/25..Par
+00003d90: 7365 6420 3331 2074 6561 6d73 2e28 3431  sed 31 teams.(41
+00003da0: 7329 2045 5252 4f52 533a 2030 2f33 310d  s) ERRORS: 0/31.
+00003db0: 0a50 6172 7365 6420 3331 2070 6c61 7965  .Parsed 31 playe
+00003dc0: 7273 2e28 3238 7329 2045 5252 4f52 533a  rs.(28s) ERRORS:
+00003dd0: 2030 2f33 310d 0a45 5252 4f52 533d 300d   0/31..ERRORS=0.
+00003de0: 0a53 5543 4345 5353 3d32 3834 0d0a 546f  .SUCCESS=284..To
+00003df0: 7461 6c20 7061 7273 6564 3d32 3834 0d0a  tal parsed=284..
+00003e00: 546f 7461 6c20 7469 6d65 2039 362e 3833  Total time 96.83
+00003e10: 3638 0d0a 0d0a 6060 600d 0a0d 0a23 2042  68....```....# B
+00003e20: 6574 6120 2f20 556e 7265 6c65 6173 6564  eta / Unreleased
+00003e30: 0d0a 0d0a 2a2a 5468 6174 2066 756e 6374  ....**That funct
+00003e40: 696f 6e73 2077 6572 6520 6d61 6465 2066  ions were made f
+00003e50: 6f72 206d 7973 656c 662c 2062 6566 6f72  or myself, befor
+00003e60: 6520 7573 696e 6720 7265 636f 6d6d 656e  e using recommen
+00003e70: 6420 796f 7520 746f 2063 6865 636b 2074  d you to check t
+00003e80: 6865 2066 696c 652a 2a0d 0a0d 0a23 2052  he file**....# R
+00003e90: 6571 7569 7265 6d65 6e74 733a 0d0a 0d0a  equirements:....
+00003ea0: 5079 7468 6f6e 2033 2e39 2b0d 0a0d 0a4c  Python 3.9+....L
+00003eb0: 6963 656e 7365 3a0d 0a48 4c54 5620 4173  icense:..HLTV As
+00003ec0: 796e 6320 6973 206c 6963 656e 7365 6420  ync is licensed 
+00003ed0: 756e 6465 7220 7468 6520 4d49 5420 4c69  under the MIT Li
+00003ee0: 6365 6e73 652c 2061 6c6c 6f77 696e 6720  cense, allowing 
+00003ef0: 666f 7220 7065 7273 6f6e 616c 2061 6e64  for personal and
+00003f00: 2063 6f6d 6d65 7263 6961 6c20 7573 6520   commercial use 
+00003f10: 7769 7468 206d 696e 696d 616c 2072 6573  with minimal res
+00003f20: 7472 6963 7469 6f6e 732e 0d0a            trictions...
```

### Comparing `hltv_async_api-0.8.0b0/PKG-INFO` & `hltv_async_api-0.8.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 686c 7476  : 2.1.Name: hltv
 00000020: 5f61 7379 6e63 5f61 7069 0a56 6572 7369  _async_api.Versi
-00000030: 6f6e 3a20 302e 382e 3062 300a 5375 6d6d  on: 0.8.0b0.Summ
+00000030: 6f6e 3a20 302e 382e 3062 310a 5375 6d6d  on: 0.8.0b1.Summ
 00000040: 6172 793a 2041 6e20 756e 6f66 6669 6369  ary: An unoffici
 00000050: 616c 2061 7379 6e63 6872 6f6e 6f75 7320  al asynchronous 
 00000060: 484c 5456 2041 5049 2057 7261 7070 6572  HLTV API Wrapper
 00000070: 2066 6f72 2050 7974 686f 6e0a 4175 7468   for Python.Auth
 00000080: 6f72 3a20 416b 696d 2053 6c79 730a 4175  or: Akim Slys.Au
 00000090: 7468 6f72 2d65 6d61 696c 3a20 616b 696d  thor-email: akim
 000000a0: 736c 7973 3230 3033 4067 6d61 696c 2e63  slys2003@gmail.c
@@ -56,979 +56,986 @@
 00000370: 7375 6573 0a44 6573 6372 6970 7469 6f6e  sues.Description
 00000380: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
 00000390: 6578 742f 6d61 726b 646f 776e 0a0a 2320  ext/markdown..# 
 000003a0: 686c 7476 2d61 7379 6e63 2d61 7069 2061  hltv-async-api a
 000003b0: 6e20 2a2a 756e 6f66 6669 6369 616c 2a2a  n **unofficial**
 000003c0: 2061 7379 6e63 6872 6f6e 6f75 7320 484c   asynchronous HL
 000003d0: 5456 2041 5049 2057 7261 7070 6572 2066  TV API Wrapper f
-000003e0: 6f72 2050 7974 686f 6e2e 2055 7365 206f  or Python. Use o
-000003f0: 6e6c 7920 696e 206e 6f6e 2d63 6f6d 6d65  nly in non-comme
-00000400: 7263 6961 6c20 7075 7270 6f73 6573 0a0a  rcial purposes..
-00000410: 0a2a 2a54 6869 7320 7061 6765 2069 7320  .**This page is 
-00000420: 6e6f 7420 636f 6d70 6c65 7465 642c 206e  not completed, n
-00000430: 6f74 2061 6c6c 206d 6574 686f 6473 2061  ot all methods a
-00000440: 6e64 2063 6f6e 6669 6773 2061 7265 2077  nd configs are w
-00000450: 7269 7474 656e 2a2a 0a0a 0a23 2046 6561  ritten**...# Fea
-00000460: 7475 7265 730a 0a0a 2a20 2a2a 5369 6d70  tures...* **Simp
-00000470: 6c65 2055 7361 6765 2a2a 2028 6974 7320  le Usage** (its 
-00000480: 7265 616c 6c79 2073 696d 706c 6529 0a0a  really simple)..
-00000490: 0a2a 202a 2a4e 6577 2061 6e64 206d 6f64  .* **New and mod
-000004a0: 6572 6e20 6675 6c6c 7920 6173 796e 6320  ern fully async 
-000004b0: 6c69 6272 6172 792a 2a0a 0a0a 2a20 2a2a  library**...* **
-000004c0: 4875 6765 2061 6d6f 756e 7420 6f66 206f  Huge amount of o
-000004d0: 7074 696f 6e73 2a2a 0a0a 0a2a 202a 2a53  ptions**...* **S
-000004e0: 7570 706f 7274 7320 7072 6f78 7920 7573  upports proxy us
-000004f0: 6167 652a 2a0a 0a0a 2a20 2a2a 4d61 6465  age**...* **Made
-00000500: 2077 6974 6820 6c6f 7665 203c 332a 2a0a   with love <3**.
-00000510: 0a0a 2d2d 2d0a 0a23 2049 6e73 7461 6c6c  ..---..# Install
-00000520: 6174 696f 6e0a 0a60 6060 0a70 6970 2069  ation..```.pip i
-00000530: 6e73 7461 6c6c 2068 6c74 762d 6173 796e  nstall hltv-asyn
-00000540: 632d 6170 690a 6060 600a 0a2d 2d2d 0a0a  c-api.```..---..
-00000550: 0a23 2053 696d 706c 6520 5573 6167 650a  .# Simple Usage.
-00000560: 0a20 2020 2060 6060 0a0a 2020 2020 6672  .    ```..    fr
-00000570: 6f6d 2068 6c74 765f 6173 796e 635f 6170  om hltv_async_ap
-00000580: 6920 696d 706f 7274 2048 6c74 760a 2020  i import Hltv.  
-00000590: 2020 0a20 2020 2061 7379 6e63 2077 6974    .    async wit
-000005a0: 6820 486c 7476 2829 2061 7320 686c 7476  h Hltv() as hltv
-000005b0: 3a0a 2020 2020 2020 7072 696e 7428 6177  :.      print(aw
-000005c0: 6169 7420 686c 7476 2e67 6574 5f65 7665  ait hltv.get_eve
-000005d0: 6e74 5f69 6e66 6f28 3731 3438 2c20 2750  nt_info(7148, 'P
-000005e0: 474c 2043 5332 204d 616a 6f72 2043 6f70  GL CS2 Major Cop
-000005f0: 656e 6861 6765 6e32 3032 3427 2929 0a0a  enhagen2024'))..
-00000600: 2020 2020 6060 600a 0a20 202a 2a4f 522a      ```..  **OR*
-00000610: 2a0a 0a20 2020 2060 6060 0a0a 2020 2020  *..    ```..    
-00000620: 6672 6f6d 2068 6c74 765f 6173 796e 635f  from hltv_async_
-00000630: 6170 6920 696d 706f 7274 2048 6c74 760a  api import Hltv.
-00000640: 2020 2020 0a20 2020 2068 6c74 7620 3d20      .    hltv = 
-00000650: 486c 7476 2829 0a20 2020 2070 7269 6e74  Hltv().    print
-00000660: 2861 7761 6974 2068 6c74 762e 6765 745f  (await hltv.get_
-00000670: 6576 656e 745f 696e 666f 2837 3134 382c  event_info(7148,
-00000680: 2027 5047 4c20 4353 3220 4d61 6a6f 7220   'PGL CS2 Major 
-00000690: 436f 7065 6e68 6167 656e 3230 3234 2729  Copenhagen2024')
-000006a0: 290a 2020 2020 6177 6169 7420 686c 7476  ).    await hltv
-000006b0: 2e63 6c6f 7365 2829 0a0a 2020 2020 6060  .close()..    ``
-000006c0: 600a 0a2d 2d2d 0a0a 2320 5072 6f78 7920  `..---..# Proxy 
-000006d0: 5573 6167 650a 0a2a 2a4c 6f61 6420 5072  Usage..**Load Pr
-000006e0: 6f78 6965 7320 6672 6f6d 206c 6973 742a  oxies from list*
-000006f0: 2a0a 2020 2020 0a20 2020 2060 6060 0a20  *.    .    ```. 
-00000700: 2020 2070 726f 7879 5f6c 6973 7420 3d20     proxy_list = 
-00000710: 5b27 6874 7470 3a2f 2f31 3230 2e32 3334  ['http://120.234
-00000720: 2e32 3033 2e31 3731 3a39 3030 3227 2c20  .203.171:9002', 
-00000730: 2768 7474 703a 2f2f 3131 302e 3338 2e36  'http://110.38.6
-00000740: 382e 3338 3a38 3027 5d0a 2020 2020 0a20  8.38:80'].    . 
-00000750: 2020 2068 6c74 7620 3d20 486c 7476 2870     hltv = Hltv(p
-00000760: 726f 7879 5f6c 6973 743d 7072 6f78 795f  roxy_list=proxy_
-00000770: 6c69 7374 290a 0a20 2020 2060 6060 0a0a  list)..    ```..
-00000780: 2a2a 4c6f 6164 2050 726f 7869 6573 2066  **Load Proxies f
-00000790: 726f 6d20 6669 6c65 2a2a 0a0a 2020 2020  rom file**..    
-000007a0: 6060 600a 2020 2020 686c 7476 203d 2048  ```.    hltv = H
-000007b0: 6c74 7628 7072 6f78 795f 7061 7468 3d27  ltv(proxy_path='
-000007c0: 5041 5448 5f54 4f5f 5052 4f58 592e 5458  PATH_TO_PROXY.TX
-000007d0: 5427 290a 2020 2020 6060 600a 0a0a 2a2a  T').    ```...**
-000007e0: 4465 6c65 7465 2070 726f 7879 2a2a 0a0a  Delete proxy**..
-000007f0: 2020 2020 5265 6d6f 7665 7320 6261 6420      Removes bad 
-00000800: 7072 6f78 6965 730a 2020 2020 0a20 2020  proxies.    .   
-00000810: 2060 6060 0a20 2020 2068 6c74 7620 3d20   ```.    hltv = 
-00000820: 486c 7476 2870 726f 7879 5f70 6174 683d  Hltv(proxy_path=
-00000830: 2750 4154 485f 544f 5f50 524f 5859 2e54  'PATH_TO_PROXY.T
-00000840: 5854 272c 2064 656c 6574 655f 7072 6f78  XT', delete_prox
-00000850: 793d 5472 7565 290a 2020 2020 6060 600a  y=True).    ```.
-00000860: 0a2a 2a50 726f 746f 636f 6c20 7573 6167  .**Protocol usag
-00000870: 652a 2a0a 0a20 2020 2060 6060 0a20 2020  e**..    ```.   
-00000880: 2070 726f 7879 5f6c 6973 7420 3d20 5b27   proxy_list = ['
-00000890: 3132 302e 3233 342e 3230 332e 3137 313a  120.234.203.171:
-000008a0: 3930 3032 272c 2027 3131 302e 3338 2e36  9002', '110.38.6
-000008b0: 382e 3338 3a38 3027 5d0a 2020 2020 0a20  8.38:80'].    . 
-000008c0: 2020 2068 6c74 7620 3d20 486c 7476 2870     hltv = Hltv(p
-000008d0: 726f 7879 5f6c 6973 743d 7072 6f78 795f  roxy_list=proxy_
-000008e0: 6c69 7374 2c20 7072 6f78 795f 7072 6f74  list, proxy_prot
-000008f0: 6f63 6f6c 3d27 6874 7470 2729 0a20 2020  ocol='http').   
-00000900: 2060 6060 0a0a 2d2d 2d0a 2320 4d65 7468   ```..---.# Meth
-00000910: 6f64 730a 0a2a 202a 2a67 6574 5f6d 6174  ods..* **get_mat
-00000920: 6368 6573 2864 6179 733a 2069 6e74 203d  ches(days: int =
-00000930: 2031 2c20 6d69 6e5f 7374 6172 5f72 6174   1, min_star_rat
-00000940: 696e 673a 2069 6e74 203d 2031 2c20 6c69  ing: int = 1, li
-00000950: 7665 3a20 626f 6f6c 203d 2054 7275 652c  ve: bool = True,
-00000960: 2066 7574 7572 653a 2062 6f6f 6c20 3d20   future: bool = 
-00000970: 5472 7565 292a 2a0a 0a20 2020 202d 6461  True)**..    -da
-00000980: 7973 2028 7468 6520 6e75 6d62 6572 206f  ys (the number o
-00000990: 6620 6461 7973 2069 6e74 6f20 7468 6520  f days into the 
-000009a0: 6675 7475 7265 2074 6f20 6665 7463 6820  future to fetch 
-000009b0: 6d61 7463 6865 7320 666f 7229 0a20 200a  matches for).  .
-000009c0: 2020 2020 2d6d 696e 5f73 7461 725f 7261      -min_star_ra
-000009d0: 7469 6e67 2028 7468 6520 6d69 6e69 6d75  ting (the minimu
-000009e0: 6d20 7374 6172 2072 6174 696e 6720 666f  m star rating fo
-000009f0: 7220 6d61 7463 6865 7320 746f 2069 6e63  r matches to inc
-00000a00: 6c75 6465 290a 2020 0a20 2020 2060 6060  lude).  .    ```
-00000a10: 0a20 2020 2061 7761 6974 2068 6c74 762e  .    await hltv.
-00000a20: 6765 745f 6d61 7463 6865 7328 6461 7973  get_matches(days
-00000a30: 3d31 290a 2020 2020 0a20 2020 203e 3e3e  =1).    .    >>>
-00000a40: 205b 7b27 6964 273a 2027 3233 3731 3230   [{'id': '237120
-00000a50: 3127 2c20 2764 6174 6527 3a20 274c 4956  1', 'date': 'LIV
-00000a60: 4527 2c20 2774 696d 6527 3a20 274c 4956  E', 'time': 'LIV
-00000a70: 4527 2c20 2774 6561 6d31 273a 2027 496d  E', 'team1': 'Im
-00000a80: 7065 7269 616c 272c 2027 7465 616d 3227  perial', 'team2'
-00000a90: 3a20 274d 4942 5227 2c20 2774 315f 6964  : 'MIBR', 't1_id
-00000aa0: 273a 2027 3934 3535 272c 2027 7432 5f69  ': '9455', 't2_i
-00000ab0: 6427 3a20 2739 3231 3527 2c20 276d 6170  d': '9215', 'map
-00000ac0: 7327 3a20 2733 272c 2027 7261 7469 6e67  s': '3', 'rating
-00000ad0: 273a 2031 2c20 2765 7665 6e74 273a 2027  ': 1, 'event': '
-00000ae0: 5245 5320 5265 6769 6f6e 616c 2053 6572  RES Regional Ser
-00000af0: 6965 7320 3320 4c41 5441 4d27 7d2c 207b  ies 3 LATAM'}, {
-00000b00: 2769 6427 3a20 2732 3337 3039 3634 272c  'id': '2370964',
-00000b10: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
-00000b20: 342d 3136 272c 2027 7469 6d65 273a 2027  4-16', 'time': '
-00000b30: 3132 3a33 3027 2c20 2774 6561 6d31 273a  12:30', 'team1':
-00000b40: 2027 5341 5727 2c20 2774 6561 6d32 273a   'SAW', 'team2':
-00000b50: 2027 5361 6d70 6927 2c20 2774 315f 6964   'Sampi', 't1_id
-00000b60: 273a 2027 3130 3536 3727 2c20 2774 325f  ': '10567', 't2_
-00000b70: 6964 273a 2027 3130 3639 3527 2c20 276d  id': '10695', 'm
-00000b80: 6170 7327 3a20 2733 272c 2027 7261 7469  aps': '3', 'rati
-00000b90: 6e67 273a 2031 2c20 2765 7665 6e74 273a  ng': 1, 'event':
-00000ba0: 2027 5468 756e 6465 7270 6963 6b20 576f   'Thunderpick Wo
-00000bb0: 726c 6420 4368 616d 7069 6f6e 7368 6970  rld Championship
-00000bc0: 2032 3032 3420 4555 2043 6c6f 7365 6420   2024 EU Closed 
-00000bd0: 5175 616c 6966 6965 7220 3127 7d2c 207b  Qualifier 1'}, {
-00000be0: 2769 6427 3a20 2732 3337 3133 3637 272c  'id': '2371367',
-00000bf0: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
-00000c00: 342d 3136 272c 2027 7469 6d65 273a 2027  4-16', 'time': '
-00000c10: 3134 3a30 3027 2c20 2774 6561 6d31 273a  14:00', 'team1':
-00000c20: 2027 4761 696d 696e 2047 6c61 6469 6174   'Gaimin Gladiat
-00000c30: 6f72 7327 2c20 2774 6561 6d32 273a 2027  ors', 'team2': '
-00000c40: 5065 726d 6974 7461 272c 2027 7431 5f69  Permitta', 't1_i
-00000c50: 6427 3a20 2731 3135 3731 272c 2027 7432  d': '11571', 't2
-00000c60: 5f69 6427 3a20 2731 3230 3039 272c 2027  _id': '12009', '
-00000c70: 6d61 7073 273a 2027 3327 2c20 2772 6174  maps': '3', 'rat
-00000c80: 696e 6727 3a20 312c 2027 6576 656e 7427  ing': 1, 'event'
-00000c90: 3a20 2745 6c69 7361 2049 6e76 6974 6174  : 'Elisa Invitat
-00000ca0: 696f 6e61 6c20 5370 7269 6e67 2032 3032  ional Spring 202
-00000cb0: 3427 7d5d 0a20 2020 200a 2020 2020 6060  4'}].    .    ``
-00000cc0: 600a 0a2a 202a 2a67 6574 5f6d 6174 6368  `..* **get_match
-00000cd0: 5f69 6e66 6f28 6d61 7463 685f 6964 3a20  _info(match_id: 
-00000ce0: 696e 7420 7c20 7374 722c 2074 6561 6d31  int | str, team1
-00000cf0: 2c20 7465 616d 322c 2065 7665 6e74 5f74  , team2, event_t
-00000d00: 6974 6c65 2c20 7374 6174 733a 2062 6f6f  itle, stats: boo
-00000d10: 6c20 3d20 5472 7565 2c20 7072 6564 6963  l = True, predic
-00000d20: 7473 3a20 626f 6f6c 203d 2054 7275 6529  ts: bool = True)
-00000d30: 2a2a 0a20 200a 2020 2020 6060 600a 2020  **.  .    ```.  
-00000d40: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
-00000d50: 5f6d 6174 6368 5f69 6e66 6f28 3233 3730  _match_info(2370
-00000d60: 3933 312c 2027 4d6f 757a 272c 2027 6661  931, 'Mouz', 'fa
-00000d70: 7a65 272c 2027 6965 6d2d 6368 656e 6764  ze', 'iem-chengd
-00000d80: 752d 3230 3234 2729 2020 0a20 200a 2020  u-2024')  .  .  
-00000d90: 2020 3e3e 3e28 3233 3730 3933 312c 2027    >>>(2370931, '
-00000da0: 3027 2c20 2732 272c 2027 4d61 7463 6820  0', '2', 'Match 
-00000db0: 6f76 6572 272c 205b 7b27 6d61 706e 616d  over', [{'mapnam
-00000dc0: 6527 3a20 274f 7665 7270 6173 7327 2c20  e': 'Overpass', 
-00000dd0: 2772 5f74 6561 6d31 273a 2027 3130 272c  'r_team1': '10',
-00000de0: 2027 725f 7465 616d 3227 3a20 2731 3327   'r_team2': '13'
-00000df0: 7d2c 207b 276d 6170 6e61 6d65 273a 2027  }, {'mapname': '
-00000e00: 4e75 6b65 272c 2027 725f 7465 616d 3127  Nuke', 'r_team1'
-00000e10: 3a20 2736 272c 2027 725f 7465 616d 3227  : '6', 'r_team2'
-00000e20: 3a20 2731 3327 7d2c 207b 276d 6170 6e61  : '13'}, {'mapna
-00000e30: 6d65 273a 2027 4d69 7261 6765 272c 2027  me': 'Mirage', '
-00000e40: 725f 7465 616d 3127 3a20 272d 272c 2027  r_team1': '-', '
-00000e50: 725f 7465 616d 3227 3a20 272d 277d 5d2c  r_team2': '-'}],
-00000e60: 205b 7b27 6964 273a 2027 3138 3835 3027   [{'id': '18850'
-00000e70: 2c20 276e 6963 6b6e 616d 6527 3a20 274a  , 'nickname': 'J
-00000e80: 696d 7070 6861 7427 2c20 276b 6427 3a20  impphat', 'kd': 
-00000e90: 2733 332d 3239 272c 2027 6164 7227 3a20  '33-29', 'adr': 
-00000ea0: 2738 302e 3927 2c20 2772 6174 696e 6727  '80.9', 'rating'
-00000eb0: 3a20 2731 2e30 3827 7d2c 200a 2020 0a20  : '1.08'}, .  . 
-00000ec0: 2020 207b 2769 6427 3a20 2731 3830 3732     {'id': '18072
-00000ed0: 272c 2027 6e69 636b 6e61 6d65 273a 2027  ', 'nickname': '
-00000ee0: 746f 727a 7369 272c 2027 6b64 273a 2027  torzsi', 'kd': '
-00000ef0: 3236 2d32 3527 2c20 2761 6472 273a 2027  26-25', 'adr': '
-00000f00: 3730 2e35 272c 2027 7261 7469 6e67 273a  70.5', 'rating':
-00000f10: 2027 312e 3032 277d 2c20 7b27 6964 273a   '1.02'}, {'id':
-00000f20: 2027 3133 3636 3627 2c20 276e 6963 6b6e   '13666', 'nickn
-00000f30: 616d 6527 3a20 2742 726f 6c6c 616e 272c  ame': 'Brollan',
-00000f40: 2027 6b64 273a 2027 3235 2d33 3127 2c20   'kd': '25-31', 
-00000f50: 2761 6472 273a 2027 3638 2e34 272c 2027  'adr': '68.4', '
-00000f60: 7261 7469 6e67 273a 2027 302e 3930 277d  rating': '0.90'}
-00000f70: 2c20 7b27 6964 273a 2027 3230 3331 3227  , {'id': '20312'
-00000f80: 2c20 276e 6963 6b6e 616d 6527 3a20 2778  , 'nickname': 'x
-00000f90: 6572 7469 6f4e 272c 2027 6b64 273a 2027  ertioN', 'kd': '
-00000fa0: 3233 2d33 3127 2c20 2761 6472 273a 2027  23-31', 'adr': '
-00000fb0: 3632 2e34 272c 2027 7261 7469 6e67 273a  62.4', 'rating':
-00000fc0: 2027 302e 3832 277d 2c20 7b27 6964 273a   '0.82'}, {'id':
-00000fd0: 2027 3136 3832 3027 2c20 276e 6963 6b6e   '16820', 'nickn
-00000fe0: 616d 6527 3a20 2773 6975 6879 272c 2027  ame': 'siuhy', '
-00000ff0: 6b64 273a 2027 3137 2d33 3027 2c20 2761  kd': '17-30', 'a
-00001000: 6472 273a 2027 3531 2e36 272c 2027 7261  dr': '51.6', 'ra
-00001010: 7469 6e67 273a 2027 302e 3730 277d 2c20  ting': '0.70'}, 
-00001020: 7b27 6964 273a 2027 3138 3035 3327 2c20  {'id': '18053', 
-00001030: 276e 6963 6b6e 616d 6527 3a20 2762 726f  'nickname': 'bro
-00001040: 6b79 272c 2027 6b64 273a 2027 3334 2d32  ky', 'kd': '34-2
-00001050: 3227 2c20 2761 6472 273a 2027 3739 2e33  2', 'adr': '79.3
-00001060: 272c 2027 7261 7469 6e67 273a 2027 312e  ', 'rating': '1.
-00001070: 3333 277d 2c20 7b27 6964 273a 2027 3939  33'}, {'id': '99
-00001080: 3630 272c 2027 6e69 636b 6e61 6d65 273a  60', 'nickname':
-00001090: 2027 6672 6f7a 656e 272c 2027 6b64 273a   'frozen', 'kd':
-000010a0: 2027 3333 2d32 3327 2c20 2761 6472 273a   '33-23', 'adr':
-000010b0: 2027 3835 2e35 272c 2027 7261 7469 6e67   '85.5', 'rating
-000010c0: 273a 2027 312e 3331 277d 2c20 7b27 6964  ': '1.31'}, {'id
-000010d0: 273a 2027 3131 3831 3627 2c20 276e 6963  ': '11816', 'nic
-000010e0: 6b6e 616d 6527 3a20 2772 6f70 7a27 2c20  kname': 'ropz', 
-000010f0: 276b 6427 3a20 2733 312d 3236 272c 2027  'kd': '31-26', '
-00001100: 6164 7227 3a20 2737 332e 3027 2c20 2772  adr': '73.0', 'r
-00001110: 6174 696e 6727 3a20 2731 2e32 3027 7d2c  ating': '1.20'},
-00001120: 207b 2769 6427 3a20 2738 3138 3327 2c20   {'id': '8183', 
-00001130: 276e 6963 6b6e 616d 6527 3a20 2772 6169  'nickname': 'rai
-00001140: 6e27 2c20 276b 6427 3a20 2732 372d 3236  n', 'kd': '27-26
-00001150: 272c 2027 6164 7227 3a20 2738 322e 3027  ', 'adr': '82.0'
-00001160: 2c20 2772 6174 696e 6727 3a20 2731 2e31  , 'rating': '1.1
-00001170: 3827 7d2c 207b 2769 6427 3a20 2734 3239  8'}, {'id': '429
-00001180: 272c 2027 6e69 636b 6e61 6d65 273a 2027  ', 'nickname': '
-00001190: 6b61 7272 6967 616e 272c 2027 6b64 273a  karrigan', 'kd':
-000011a0: 2027 3230 2d32 3827 2c20 2761 6472 273a   '20-28', 'adr':
-000011b0: 2027 3439 2e37 272c 2027 7261 7469 6e67   '49.7', 'rating
-000011c0: 273a 2027 302e 3831 277d 5d29 2020 0a20  ': '0.81'}])  . 
-000011d0: 2020 200a 2020 2020 6060 600a 2020 0a2a     .    ```.  .*
-000011e0: 202a 2a67 6574 5f72 6573 756c 7473 2864   **get_results(d
-000011f0: 6179 733a 2069 6e74 203d 2031 2c20 6d69  ays: int = 1, mi
-00001200: 6e5f 7261 7469 6e67 3a20 696e 7420 3d20  n_rating: int = 
-00001210: 312c 206d 6178 3a20 696e 7420 3d20 3330  1, max: int = 30
-00001220: 2c20 6665 6174 7572 6564 3a20 626f 6f6c  , featured: bool
-00001230: 203d 2054 7275 652c 2072 6567 756c 6172   = True, regular
-00001240: 3a20 626f 6f6c 203d 2054 7275 6529 2920  : bool = True)) 
-00001250: 2d3e 2a2a 0a20 2020 200a 2020 2020 6060  ->**.    .    ``
-00001260: 600a 2020 2020 7072 696e 7428 6177 6169  `.    print(awai
-00001270: 7420 686c 7476 2e67 6574 5f72 6573 756c  t hltv.get_resul
-00001280: 7473 2829 290a 2020 0a20 2020 205b 7b27  ts()).  .    [{'
-00001290: 6964 273a 2027 3233 3730 3933 3127 2c20  id': '2370931', 
-000012a0: 2774 6561 6d31 273a 2027 4d4f 555a 272c  'team1': 'MOUZ',
-000012b0: 2027 7465 616d 3227 3a20 2746 615a 6527   'team2': 'FaZe'
-000012c0: 2c20 2773 636f 7265 3127 3a20 2730 272c  , 'score1': '0',
-000012d0: 2027 7363 6f72 6532 273a 2027 3227 2c20   'score2': '2', 
-000012e0: 2772 6174 696e 6727 3a20 302c 2027 6576  'rating': 0, 'ev
-000012f0: 656e 7427 3a20 2749 454d 2043 6865 6e67  ent': 'IEM Cheng
-00001300: 6475 2032 3032 3427 7d5d 0a20 2020 2060  du 2024'}].    `
-00001310: 6060 0a20 200a 2a20 2a2a 6765 745f 6576  ``.  .* **get_ev
-00001320: 656e 7473 286f 7574 676f 696e 673d 5472  ents(outgoing=Tr
-00001330: 7565 2c20 6675 7475 7265 3d54 7275 652c  ue, future=True,
-00001340: 206d 6178 5f65 7665 6e74 733d 3130 2920   max_events=10) 
-00001350: 2d3e 205b 2827 6964 272c 2027 7469 746c  -> [('id', 'titl
-00001360: 6527 2c20 2773 7461 7274 6461 7465 272c  e', 'startdate',
-00001370: 2027 656e 6464 6174 6527 295d 2a2a 0a0a   'enddate')]**..
-00001380: 2020 2020 6060 600a 2020 2020 6177 6169      ```.    awai
-00001390: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
-000013a0: 7328 6675 7475 7265 3d46 616c 7365 290a  s(future=False).
-000013b0: 2020 2020 0a20 2020 203e 3e3e 5b7b 2769      .    >>>[{'i
-000013c0: 6427 3a20 2737 3734 3927 2c20 2774 6974  d': '7749', 'tit
-000013d0: 6c65 273a 2027 5468 756e 6465 7270 6963  le': 'Thunderpic
-000013e0: 6b20 576f 726c 6420 4368 616d 7069 6f6e  k World Champion
-000013f0: 7368 6970 2032 3032 3420 4555 2043 6c6f  ship 2024 EU Clo
-00001400: 7365 6420 5175 616c 6966 6965 7220 3127  sed Qualifier 1'
-00001410: 2c20 2773 7461 7274 5f64 6174 6527 3a20  , 'start_date': 
-00001420: 2731 2d34 272c 2027 656e 645f 6461 7465  '1-4', 'end_date
-00001430: 273a 2027 3232 2d34 277d 2c20 7b27 6964  ': '22-4'}, {'id
-00001440: 273a 2027 3736 3231 272c 2027 7469 746c  ': '7621', 'titl
-00001450: 6527 3a20 2745 534c 2043 6861 6c6c 656e  e': 'ESL Challen
-00001460: 6765 7220 4c65 6167 7565 2053 6561 736f  ger League Seaso
-00001470: 6e20 3437 204e 6f72 7468 2041 6d65 7269  n 47 North Ameri
-00001480: 6361 272c 2027 7374 6172 745f 6461 7465  ca', 'start_date
-00001490: 273a 2027 3133 2d32 272c 2027 656e 645f  ': '13-2', 'end_
-000014a0: 6461 7465 273a 2027 3136 2d36 277d 5d0a  date': '16-6'}].
-000014b0: 2020 2020 2020 0a20 2020 2060 6060 0a0a        .    ```..
-000014c0: 2a20 2a2a 6765 745f 6576 656e 745f 7265  * **get_event_re
-000014d0: 7375 6c74 7328 6576 656e 745f 6964 3a20  sults(event_id: 
-000014e0: 696e 7420 7c20 7374 722c 2064 6179 733a  int | str, days:
-000014f0: 2069 6e74 203d 2031 2c20 6d61 785f 3a20   int = 1, max_: 
-00001500: 696e 7420 3d20 3130 292a 2a0a 0a20 200a  int = 10)**..  .
-00001510: 2020 2020 6060 600a 2020 2020 6177 6169      ```.    awai
-00001520: 7420 6765 745f 6576 656e 745f 7265 7375  t get_event_resu
-00001530: 6c74 7328 3731 3438 290a 2020 2020 0a20  lts(7148).    . 
-00001540: 2020 203e 3e3e 5b7b 2769 6427 3a20 2732     >>>[{'id': '2
-00001550: 3337 3039 3331 272c 2027 6461 7465 273a  370931', 'date':
-00001560: 2027 3134 2d30 342d 3230 3234 272c 2027   '14-04-2024', '
-00001570: 7465 616d 3127 3a20 274d 4f55 5a27 2c20  team1': 'MOUZ', 
-00001580: 2774 6561 6d32 273a 2027 4661 5a65 272c  'team2': 'FaZe',
-00001590: 2027 7363 6f72 6531 273a 2027 3027 2c20   'score1': '0', 
-000015a0: 2773 636f 7265 3227 3a20 2732 277d 5d0a  'score2': '2'}].
-000015b0: 0a20 2020 2060 6060 0a0a 2a20 2a2a 6765  .    ```..* **ge
-000015c0: 745f 6576 656e 745f 6d61 7463 6865 7328  t_event_matches(
-000015d0: 6576 656e 745f 6964 3a20 7374 7220 7c20  event_id: str | 
-000015e0: 696e 742c 2064 6179 733a 2069 6e74 203d  int, days: int =
-000015f0: 2031 293a 2a2a 0a20 200a 2020 2020 6060   1):**.  .    ``
-00001600: 600a 2020 2020 6177 6169 7420 686c 7476  `.    await hltv
-00001610: 2e67 6574 5f65 7665 6e74 5f6d 6174 6368  .get_event_match
-00001620: 6573 2837 3134 3829 0a20 2020 200a 2020  es(7148).    .  
-00001630: 2020 3e3e 3e5b 7b27 6964 273a 2027 3233    >>>[{'id': '23
-00001640: 3730 3737 3127 2c20 2764 6174 6527 3a20  70771', 'date': 
-00001650: 2732 3032 342d 3034 2d31 3827 2c20 2774  '2024-04-18', 't
-00001660: 696d 6527 3a20 2731 353a 3330 272c 2027  ime': '15:30', '
-00001670: 7465 616d 3127 3a20 274d 6f6e 7465 272c  team1': 'Monte',
-00001680: 2027 7465 616d 3227 3a20 2770 6169 4e27   'team2': 'paiN'
-00001690: 2c20 2774 315f 6964 273a 2027 3131 3831  , 't1_id': '1181
-000016a0: 3127 2c20 2774 325f 6964 273a 2027 3437  1', 't2_id': '47
-000016b0: 3733 277d 2c20 7b27 6964 273a 2027 3233  73'}, {'id': '23
-000016c0: 3730 3737 3227 2c20 2764 6174 6527 3a20  70772', 'date': 
-000016d0: 2732 3032 342d 3034 2d31 3827 2c20 2774  '2024-04-18', 't
-000016e0: 696d 6527 3a20 2731 373a 3030 272c 2027  ime': '17:00', '
-000016f0: 7465 616d 3127 3a20 2749 6d70 6572 6961  team1': 'Imperia
-00001700: 6c27 2c20 2774 6561 6d32 273a 2027 4d65  l', 'team2': 'Me
-00001710: 7469 7a70 6f72 7427 2c20 2774 315f 6964  tizport', 't1_id
-00001720: 273a 2027 3934 3535 272c 2027 7432 5f69  ': '9455', 't2_i
-00001730: 6427 3a20 2731 3136 3431 277d 2c20 7b27  d': '11641'}, {'
-00001740: 6964 273a 2027 3233 3730 3737 3327 2c20  id': '2370773', 
-00001750: 2764 6174 6527 3a20 2732 3032 342d 3034  'date': '2024-04
-00001760: 2d31 3827 2c20 2774 696d 6527 3a20 2731  -18', 'time': '1
-00001770: 383a 3330 272c 2027 7465 616d 3127 3a20  8:30', 'team1': 
-00001780: 2746 5552 4941 272c 2027 7465 616d 3227  'FURIA', 'team2'
-00001790: 3a20 2739 7a27 2c20 2774 315f 6964 273a  : '9z', 't1_id':
-000017a0: 2027 3832 3937 272c 2027 7432 5f69 6427   '8297', 't2_id'
-000017b0: 3a20 2739 3939 3627 7d2c 207b 2769 6427  : '9996'}, {'id'
-000017c0: 3a20 2732 3337 3037 3734 272c 2027 6461  : '2370774', 'da
-000017d0: 7465 273a 2027 3230 3234 2d30 342d 3138  te': '2024-04-18
-000017e0: 272c 2027 7469 6d65 273a 2027 3230 3a30  ', 'time': '20:0
-000017f0: 3027 2c20 2774 6561 6d31 273a 2027 4d49  0', 'team1': 'MI
-00001800: 4252 272c 2027 7465 616d 3227 3a20 274f  BR', 'team2': 'O
-00001810: 4727 2c20 2774 315f 6964 273a 2027 3932  G', 't1_id': '92
-00001820: 3135 272c 2027 7432 5f69 6427 3a20 2731  15', 't2_id': '1
-00001830: 3035 3033 277d 2c20 7b27 6964 273a 2027  0503'}, {'id': '
-00001840: 3233 3730 3737 3527 2c20 2764 6174 6527  2370775', 'date'
-00001850: 3a20 2732 3032 342d 3034 2d31 3827 2c20  : '2024-04-18', 
-00001860: 2774 696d 6527 3a20 2732 313a 3330 272c  'time': '21:30',
-00001870: 2027 7465 616d 3127 3a20 2754 4244 272c   'team1': 'TBD',
-00001880: 2027 7465 616d 3227 3a20 2754 4244 272c   'team2': 'TBD',
-00001890: 2027 7431 5f69 6427 3a20 302c 2027 7432   't1_id': 0, 't2
-000018a0: 5f69 6427 3a20 307d 2c20 7b27 6964 273a  _id': 0}, {'id':
-000018b0: 2027 3233 3730 3737 3627 2c20 2764 6174   '2370776', 'dat
-000018c0: 6527 3a20 2732 3032 342d 3034 2d31 3827  e': '2024-04-18'
-000018d0: 2c20 2774 696d 6527 3a20 2732 333a 3030  , 'time': '23:00
-000018e0: 272c 2027 7465 616d 3127 3a20 2754 4244  ', 'team1': 'TBD
-000018f0: 272c 2027 7465 616d 3227 3a20 2754 4244  ', 'team2': 'TBD
-00001900: 272c 2027 7431 5f69 6427 3a20 302c 2027  ', 't1_id': 0, '
-00001910: 7432 5f69 6427 3a20 307d 2c20 7b27 6964  t2_id': 0}, {'id
-00001920: 273a 2027 3233 3730 3737 3727 2c20 2764  ': '2370777', 'd
-00001930: 6174 6527 3a20 2732 3032 342d 3034 2d31  ate': '2024-04-1
-00001940: 3927 2c20 2774 696d 6527 3a20 2730 303a  9', 'time': '00:
-00001950: 3030 272c 2027 7465 616d 3127 3a20 2754  00', 'team1': 'T
-00001960: 4244 272c 2027 7465 616d 3227 3a20 2754  BD', 'team2': 'T
-00001970: 4244 272c 2027 7431 5f69 6427 3a20 302c  BD', 't1_id': 0,
-00001980: 2027 7432 5f69 6427 3a20 307d 2c20 7b27   't2_id': 0}, {'
-00001990: 6964 273a 2027 3233 3730 3737 3827 2c20  id': '2370778', 
-000019a0: 2764 6174 6527 3a20 2732 3032 342d 3034  'date': '2024-04
-000019b0: 2d31 3927 2c20 2774 696d 6527 3a20 2731  -19', 'time': '1
-000019c0: 353a 3030 272c 2027 7465 616d 3127 3a20  5:00', 'team1': 
-000019d0: 2754 4244 272c 2027 7465 616d 3227 3a20  'TBD', 'team2': 
-000019e0: 2754 4244 272c 2027 7431 5f69 6427 3a20  'TBD', 't1_id': 
-000019f0: 302c 2027 7432 5f69 6427 3a20 307d 2c20  0, 't2_id': 0}, 
-00001a00: 7b27 6964 273a 2027 3233 3730 3737 3927  {'id': '2370779'
-00001a10: 2c20 2764 6174 6527 3a20 2732 3032 342d  , 'date': '2024-
-00001a20: 3034 2d31 3927 2c20 2774 696d 6527 3a20  04-19', 'time': 
-00001a30: 2731 373a 3330 272c 2027 7465 616d 3127  '17:30', 'team1'
-00001a40: 3a20 2754 4244 272c 2027 7465 616d 3227  : 'TBD', 'team2'
-00001a50: 3a20 2754 4244 272c 2027 7431 5f69 6427  : 'TBD', 't1_id'
-00001a60: 3a20 302c 2027 7432 5f69 6427 3a20 307d  : 0, 't2_id': 0}
-00001a70: 2c20 7b27 6964 273a 2027 3233 3730 3738  , {'id': '237078
-00001a80: 3027 2c20 2764 6174 6527 3a20 2732 3032  0', 'date': '202
-00001a90: 342d 3034 2d31 3927 2c20 2774 696d 6527  4-04-19', 'time'
-00001aa0: 3a20 2732 303a 3030 272c 2027 7465 616d  : '20:00', 'team
-00001ab0: 3127 3a20 2754 4244 272c 2027 7465 616d  1': 'TBD', 'team
-00001ac0: 3227 3a20 2754 4244 272c 2027 7431 5f69  2': 'TBD', 't1_i
-00001ad0: 6427 3a20 302c 2027 7432 5f69 6427 3a20  d': 0, 't2_id': 
-00001ae0: 307d 2c20 7b27 6964 273a 2027 3233 3730  0}, {'id': '2370
-00001af0: 3738 3127 2c20 2764 6174 6527 3a20 2732  781', 'date': '2
-00001b00: 3032 342d 3034 2d31 3927 2c20 2774 696d  024-04-19', 'tim
-00001b10: 6527 3a20 2732 323a 3330 272c 2027 7465  e': '22:30', 'te
-00001b20: 616d 3127 3a20 2754 4244 272c 2027 7465  am1': 'TBD', 'te
-00001b30: 616d 3227 3a20 2754 4244 272c 2027 7431  am2': 'TBD', 't1
-00001b40: 5f69 6427 3a20 302c 2027 7432 5f69 6427  _id': 0, 't2_id'
-00001b50: 3a20 307d 2c20 7b27 6964 273a 2027 3233  : 0}, {'id': '23
-00001b60: 3730 3738 3227 2c20 2764 6174 6527 3a20  70782', 'date': 
-00001b70: 2732 3032 342d 3034 2d32 3027 2c20 2774  '2024-04-20', 't
-00001b80: 696d 6527 3a20 2730 303a 3330 272c 2027  ime': '00:30', '
-00001b90: 7465 616d 3127 3a20 2754 4244 272c 2027  team1': 'TBD', '
-00001ba0: 7465 616d 3227 3a20 2754 4244 272c 2027  team2': 'TBD', '
-00001bb0: 7431 5f69 6427 3a20 302c 2027 7432 5f69  t1_id': 0, 't2_i
-00001bc0: 6427 3a20 307d 2c20 7b27 6964 273a 2027  d': 0}, {'id': '
-00001bd0: 3233 3730 3738 3327 2c20 2764 6174 6527  2370783', 'date'
-00001be0: 3a20 2732 3032 342d 3034 2d32 3027 2c20  : '2024-04-20', 
-00001bf0: 2774 696d 6527 3a20 2731 353a 3030 272c  'time': '15:00',
-00001c00: 2027 7465 616d 3127 3a20 2754 4244 272c   'team1': 'TBD',
-00001c10: 2027 7465 616d 3227 3a20 2754 4244 272c   'team2': 'TBD',
-00001c20: 2027 7431 5f69 6427 3a20 302c 2027 7432   't1_id': 0, 't2
-00001c30: 5f69 6427 3a20 307d 2c20 7b27 6964 273a  _id': 0}, {'id':
-00001c40: 2027 3233 3730 3738 3427 2c20 2764 6174   '2370784', 'dat
-00001c50: 6527 3a20 2732 3032 342d 3034 2d32 3027  e': '2024-04-20'
-00001c60: 2c20 2774 696d 6527 3a20 2731 383a 3030  , 'time': '18:00
-00001c70: 272c 2027 7465 616d 3127 3a20 2754 4244  ', 'team1': 'TBD
-00001c80: 272c 2027 7465 616d 3227 3a20 2754 4244  ', 'team2': 'TBD
-00001c90: 272c 2027 7431 5f69 6427 3a20 302c 2027  ', 't1_id': 0, '
-00001ca0: 7432 5f69 6427 3a20 307d 5d0a 2020 0a20  t2_id': 0}].  . 
-00001cb0: 2020 2060 6060 0a0a 2a20 2a2a 6765 745f     ```..* **get_
-00001cc0: 6576 656e 745f 696e 666f 2865 7665 6e74  event_info(event
-00001cd0: 5f69 643a 2073 7472 207c 2069 6e74 2c20  _id: str | int, 
-00001ce0: 6576 656e 745f 7469 746c 653a 2073 7472  event_title: str
-00001cf0: 2920 2d3e 2028 6576 656e 745f 6964 2c20  ) -> (event_id, 
-00001d00: 6576 656e 745f 7469 746c 652c 2065 7665  event_title, eve
-00001d10: 6e74 5f73 7461 7274 2c20 6576 656e 745f  nt_start, event_
-00001d20: 656e 642c 2070 7269 7a65 2c20 7465 616d  end, prize, team
-00001d30: 5f6e 756d 2c20 6c6f 6361 7469 6f6e 2c20  _num, location, 
-00001d40: 6772 6f75 7073 292a 2a0a 0a20 2020 2060  groups)**..    `
-00001d50: 6060 0a20 2020 2061 7761 6974 2068 6c74  ``.    await hlt
-00001d60: 762e 6765 745f 6576 656e 745f 696e 666f  v.get_event_info
-00001d70: 2837 3134 382c 2027 5047 4c20 4353 3220  (7148, 'PGL CS2 
-00001d80: 4d61 6a6f 7220 436f 7065 6e68 6167 656e  Major Copenhagen
-00001d90: 3230 3234 2729 0a20 2020 200a 2020 2020  2024').    .    
-00001da0: 7b27 6964 273a 2037 3134 382c 2027 7469  {'id': 7148, 'ti
-00001db0: 746c 6527 3a20 2750 474c 2043 5332 204d  tle': 'PGL CS2 M
-00001dc0: 616a 6f72 2043 6f70 656e 6861 6765 6e32  ajor Copenhagen2
-00001dd0: 3032 3427 2c20 2773 7461 7274 273a 2027  024', 'start': '
-00001de0: 3231 2d33 272c 2027 656e 6427 3a20 2733  21-3', 'end': '3
-00001df0: 312d 3327 2c20 2770 7269 7a65 273a 2027  1-3', 'prize': '
-00001e00: 2431 2c32 3530 2c30 3030 272c 2027 7465  $1,250,000', 'te
-00001e10: 616d 7327 3a20 2731 3627 2c20 276c 6f63  ams': '16', 'loc
-00001e20: 6174 696f 6e27 3a20 2743 6f70 656e 6861  ation': 'Copenha
-00001e30: 6765 6e2c 2044 656e 6d61 726b 272c 2027  gen, Denmark', '
-00001e40: 6772 6f75 7027 3a20 5b5d 7d0a 2020 200a  group': []}.   .
-00001e50: 2020 2020 6060 600a 0a0a 2a20 2a2a 6765      ```...* **ge
-00001e60: 745f 746f 705f 7465 616d 7328 6d61 785f  t_top_teams(max_
-00001e70: 7465 616d 733d 3330 2920 2d3e 205b 2772  teams=30) -> ['r
-00001e80: 616e 6b27 2c20 2774 6974 6c65 272c 2027  ank', 'title', '
-00001e90: 706f 696e 7473 272c 2027 6368 616e 6765  points', 'change
-00001ea0: 272c 2027 6964 275d 2a2a 0a0a 2020 2020  ', 'id']**..    
-00001eb0: 6060 600a 2020 2020 6177 6169 7420 686c  ```.    await hl
-00001ec0: 7476 2e67 6574 5f74 6f70 5f74 6561 6d73  tv.get_top_teams
-00001ed0: 2832 290a 2020 2020 0a20 2020 203e 3e3e  (2).    .    >>>
-00001ee0: 5b7b 2769 6427 3a20 2731 3131 3127 2c20  [{'id': '1111', 
-00001ef0: 2772 616e 6b27 3a20 2731 272c 2027 7469  'rank': '1', 'ti
-00001f00: 746c 6527 3a20 2746 615a 6527 2c20 2770  tle': 'FaZe', 'p
-00001f10: 6f69 6e74 7327 3a20 2739 3339 272c 2027  oints': '939', '
-00001f20: 6368 616e 6765 273a 2027 2d27 2c20 2769  change': '-', 'i
-00001f30: 6427 3a20 2736 3636 3727 7d2c 207b 2769  d': '6667'}, {'i
-00001f40: 6427 3a20 2731 3131 3127 2c20 2772 616e  d': '1111', 'ran
-00001f50: 6b27 3a20 2732 272c 2027 7469 746c 6527  k': '2', 'title'
-00001f60: 3a20 274e 6174 7573 2056 696e 6365 7265  : 'Natus Vincere
-00001f70: 272c 2027 706f 696e 7473 273a 2027 3735  ', 'points': '75
-00001f80: 3727 2c20 2763 6861 6e67 6527 3a20 272b  7', 'change': '+
-00001f90: 3427 2c20 2769 6427 3a20 2734 3630 3827  4', 'id': '4608'
-00001fa0: 7d5d 0a20 2020 2060 6060 0a0a 2a20 2a2a  }].    ```..* **
-00001fb0: 6765 745f 7465 616d 5f69 6e66 6f28 7465  get_team_info(te
-00001fc0: 616d 5f69 643a 2069 6e74 207c 2073 7472  am_id: int | str
-00001fd0: 2c20 7469 746c 653a 2073 7472 2920 2d3e  , title: str) ->
-00001fe0: 2028 7465 616d 5f69 642c 2074 6561 6d5f   (team_id, team_
-00001ff0: 7469 746c 652c 2072 616e 6b2c 207b 706c  title, rank, {pl
-00002000: 6179 6572 3a70 6c61 7965 725f 6964 7d2c  ayer:player_id},
-00002010: 2063 6f61 6368 2c20 6176 6572 6167 655f   coach, average_
-00002020: 6167 652c 2077 6565 6b73 5f69 6e5f 746f  age, weeks_in_to
-00002030: 705f 3230 2c20 6c61 7374 5f74 726f 7068  p_20, last_troph
-00002040: 792c 2074 6f74 616c 5f74 726f 7068 7973  y, total_trophys
-00002050: 292a 2a0a 0a20 2020 2060 6060 0a20 2020  )**..    ```.   
-00002060: 2061 7761 6974 2068 6c74 762e 6765 745f   await hltv.get_
-00002070: 7465 616d 5f69 6e66 6f28 3636 3637 2c20  team_info(6667, 
-00002080: 2766 617a 6527 290a 2020 2020 0a20 2020  'faze').    .   
-00002090: 203e 3e3e 2836 3636 372c 2027 6661 7a65   >>>(6667, 'faze
-000020a0: 272c 2027 3127 2c20 5b27 6b61 7272 6967  ', '1', ['karrig
-000020b0: 616e 272c 2027 7261 696e 272c 2027 6672  an', 'rain', 'fr
-000020c0: 6f7a 656e 272c 2027 726f 707a 272c 2027  ozen', 'ropz', '
-000020d0: 6272 6f6b 7927 5d2c 2027 4e45 4f27 2c20  broky'], 'NEO', 
-000020e0: 2732 362e 3627 2c20 2732 3538 272c 2027  '26.6', '258', '
-000020f0: 4945 4d20 4368 656e 6764 7520 3230 3234  IEM Chengdu 2024
-00002100: 272c 2032 3229 0a20 2020 2060 6060 0a0a  ', 22).    ```..
-00002110: 2a20 2a2a 6765 745f 6c61 7374 5f6e 6577  * **get_last_new
-00002120: 7328 6d61 785f 7265 675f 6e65 7773 3d32  s(max_reg_news=2
-00002130: 2c20 6f6e 6c79 5f74 6f64 6179 3d54 7275  , only_today=Tru
-00002140: 652c 206f 6e6c 795f 6665 6174 7572 6564  e, only_featured
-00002150: 3d46 616c 7365 2920 2d3e 205b 6461 7465  =False) -> [date
-00002160: 2c20 5b66 6561 7475 7265 645f 6964 2c20  , [featured_id, 
-00002170: 6665 6174 7572 6564 5f74 6974 6c65 2c20  featured_title, 
-00002180: 6665 6174 7572 6564 5f64 6573 6369 7074  featured_descipt
-00002190: 696f 6e5d 2c20 5b72 6567 756c 6172 5f69  ion], [regular_i
-000021a0: 642c 2072 6567 5f74 6974 6c65 2c20 7265  d, reg_title, re
-000021b0: 675f 7469 6d65 5d5d 2a2a 0a0a 2020 2020  g_time]]**..    
-000021c0: 6060 600a 2020 2020 6177 6169 7420 686c  ```.    await hl
-000021d0: 7476 2e67 6574 5f6c 6173 745f 6e65 7773  tv.get_last_news
-000021e0: 286f 6e6c 795f 746f 6461 793d 5472 7565  (only_today=True
-000021f0: 290a 2020 2020 0a20 2020 203e 3e3e 5b7b  ).    .    >>>[{
-00002200: 2764 6174 6527 3a20 2731 352d 3034 272c  'date': '15-04',
-00002210: 2027 665f 6e65 7773 273a 205b 5d2c 2027   'f_news': [], '
-00002220: 6e65 7773 273a 205b 7b27 6964 273a 2027  news': [{'id': '
-00002230: 3338 3738 3427 2c20 2774 6974 6c65 273a  38784', 'title':
-00002240: 2027 4d65 6469 613a 2046 5552 4941 2070   'Media: FURIA p
-00002250: 7261 6374 6963 696e 6720 7769 7468 206b  racticing with k
-00002260: 7965 2069 6e20 706c 6163 6520 6f66 2061  ye in place of a
-00002270: 7254 272c 2027 706f 7374 6564 273a 2027  rT', 'posted': '
-00002280: 616e 2068 6f75 7220 6167 6f27 7d2c 207b  an hour ago'}, {
-00002290: 2769 6427 3a20 2733 3837 3833 272c 2027  'id': '38783', '
-000022a0: 7469 746c 6527 3a20 2765 6c65 6374 726f  title': 'electro
-000022b0: 4e69 6320 746f 2070 6c61 7920 666f 7220  Nic to play for 
-000022c0: 5669 7274 7573 2e70 726f 2061 7420 4553  Virtus.pro at ES
-000022d0: 4c20 5072 6f20 4c65 6167 7565 2053 3139  L Pro League S19
-000022e0: 272c 2027 706f 7374 6564 273a 2027 3220  ', 'posted': '2 
-000022f0: 686f 7572 7320 6167 6f27 7d2c 207b 2769  hours ago'}, {'i
-00002300: 6427 3a20 2733 3837 3831 272c 2027 7469  d': '38781', 'ti
-00002310: 746c 6527 3a20 2754 6865 2045 5650 7320  tle': 'The EVPs 
-00002320: 616e 6420 4265 7374 2046 6976 6520 6f66  and Best Five of
-00002330: 2049 454d 2043 6865 6e67 6475 272c 2027   IEM Chengdu', '
-00002340: 706f 7374 6564 273a 2027 3720 686f 7572  posted': '7 hour
-00002350: 7320 6167 6f27 7d5d 7d5d 0a20 200a 2020  s ago'}]}].  .  
-00002360: 2020 6060 600a 0a2a 202a 2a67 6574 5f62    ```..* **get_b
-00002370: 6573 745f 706c 6179 6572 7328 746f 703a  est_players(top:
-00002380: 2069 6e74 203d 2034 3029 202d 3e20 2827   int = 40) -> ('
-00002390: 7261 6e6b 272c 2027 6e61 6d65 272c 2027  rank', 'name', '
-000023a0: 7465 616d 272c 2027 6d61 7073 272c 2027  team', 'maps', '
-000023b0: 7261 7469 6e67 2729 2a2a 0a0a 2020 2020  rating')**..    
-000023c0: 6060 600a 2020 2020 6177 6169 7420 686c  ```.    await hl
-000023d0: 7476 2e67 6574 5f62 6573 745f 706c 6179  tv.get_best_play
-000023e0: 6572 7328 3229 0a20 2020 200a 2020 2020  ers(2).    .    
-000023f0: 3e3e 3e5b 7b27 6964 273a 2027 3139 3233  >>>[{'id': '1923
-00002400: 3027 2c20 2772 616e 6b27 3a20 312c 2027  0', 'rank': 1, '
-00002410: 6e61 6d65 273a 2027 6d30 4e45 5359 272c  name': 'm0NESY',
-00002420: 2027 7465 616d 273a 2027 4732 272c 2027   'team': 'G2', '
-00002430: 6d61 7073 273a 2027 3434 272c 2027 7261  maps': '44', 'ra
-00002440: 7469 6e67 273a 2027 312e 3337 277d 2c20  ting': '1.37'}, 
-00002450: 7b27 6964 273a 2027 3138 3035 3327 2c20  {'id': '18053', 
-00002460: 2772 616e 6b27 3a20 322c 2027 6e61 6d65  'rank': 2, 'name
-00002470: 273a 2027 6272 6f6b 7927 2c20 2774 6561  ': 'broky', 'tea
-00002480: 6d27 3a20 2746 615a 6527 2c20 276d 6170  m': 'FaZe', 'map
-00002490: 7327 3a20 2735 3427 2c20 2772 6174 696e  s': '54', 'ratin
-000024a0: 6727 3a20 2731 2e31 3927 7d5d 0a20 2020  g': '1.19'}].   
-000024b0: 2060 6060 0a0a 2a20 2a2a 6765 745f 706c   ```..* **get_pl
-000024c0: 6179 6572 5f69 6e66 6f28 6964 3a20 7374  ayer_info(id: st
-000024d0: 7220 7c20 696e 742c 206e 6963 6b6e 616d  r | int, nicknam
-000024e0: 653a 2073 7472 292a 2a0a 2020 0a20 2060  e: str)**.  .  `
-000024f0: 6060 0a20 2061 7761 6974 2068 6c74 762e  ``.  await hltv.
-00002500: 6765 745f 706c 6179 6572 5f69 6e66 6f28  get_player_info(
-00002510: 3739 3938 2c20 2773 316d 706c 6527 290a  7998, 's1mple').
-00002520: 2020 0a20 207b 2769 6427 3a20 3739 3938    .  {'id': 7998
-00002530: 2c20 276e 6963 6b6e 616d 6527 3a20 2773  , 'nickname': 's
-00002540: 316d 706c 6527 2c20 2774 6561 6d27 3a20  1mple', 'team': 
-00002550: 274e 6174 7573 2056 696e 6365 7265 272c  'Natus Vincere',
-00002560: 2027 7465 616d 5f69 6427 3a20 3436 3038   'team_id': 4608
-00002570: 2c20 276e 616d 6527 3a20 274f 6c65 6b73  , 'name': 'Oleks
-00002580: 616e 6472 204b 6f73 7479 6c69 6576 272c  andr Kostyliev',
-00002590: 2027 6e61 7469 6f6e 616c 6974 7927 3a20   'nationality': 
-000025a0: 2755 6b72 6169 6e65 272c 2027 6167 6527  'Ukraine', 'age'
-000025b0: 3a20 3236 2c20 2772 6174 696e 6727 3a20  : 26, 'rating': 
-000025c0: 2730 2e39 3427 2c20 276b 7072 273a 2027  '0.94', 'kpr': '
-000025d0: 302e 3630 272c 2027 6873 273a 2027 3537  0.60', 'hs': '57
-000025e0: 2e39 2527 2c20 276c 6173 745f 6d61 7463  .9%', 'last_matc
-000025f0: 6865 7327 3a20 5b31 3033 3035 392c 2039  hes': [103059, 9
-00002600: 3937 3435 2c20 3939 3732 382c 2039 3936  9745, 99728, 996
-00002610: 3936 2c20 3939 3437 312c 2039 3933 3634  96, 99471, 99364
-00002620: 5d2c 2027 6c61 7374 5f74 726f 7068 7927  ], 'last_trophy'
-00002630: 3a20 2742 4c41 5354 2050 7265 6d69 6572  : 'BLAST Premier
-00002640: 2053 7072 696e 6720 4669 6e61 6c20 3230   Spring Final 20
-00002650: 3232 272c 2027 746f 7461 6c5f 7472 6f70  22', 'total_trop
-00002660: 6869 6573 273a 2033 302c 2027 746f 7461  hies': 30, 'tota
-00002670: 6c5f 6d76 7073 273a 2032 317d 0a20 2060  l_mvps': 21}.  `
-00002680: 6060 0a0a 2a20 2a2a 6765 7428 7479 7065  ``..* **get(type
-00002690: 3a20 7374 722c 2069 643a 2069 6e74 207c  : str, id: int |
-000026a0: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
-000026b0: 6e65 2c20 7469 746c 653a 2073 7472 207c  ne, title: str |
-000026c0: 204e 6f6e 6520 3d20 4e6f 6e65 2c20 7465   None = None, te
-000026d0: 616d 313a 2073 7472 207c 204e 6f6e 6520  am1: str | None 
-000026e0: 3d20 4e6f 6e65 2c20 7465 616d 323a 2073  = None, team2: s
-000026f0: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
-00002700: 293a 2a2a 0a20 2028 4245 5441 2920 5468  ):**.  (BETA) Th
-00002710: 6973 206d 6574 686f 6420 6973 206e 6f74  is method is not
-00002720: 2066 696e 6973 6865 642e 2050 6f73 7369   finished. Possi
-00002730: 626c 6520 7479 7065 7320 2765 7665 6e74  ble types 'event
-00002740: 7327 2c20 276d 6174 6368 6573 272c 2027  s', 'matches', '
-00002750: 7465 616d 7327 2c20 616c 736f 2075 2063  teams', also u c
-00002760: 616e 2061 6464 2069 6420 7c20 7469 746c  an add id | titl
-00002770: 6520 7c20 7465 616d 3120 7c20 7465 616d  e | team1 | team
-00002780: 322c 2074 6f20 7061 7273 6520 6d6f 7265  2, to parse more
-00002790: 2e0a 2020 0a20 2060 6060 0a20 200a 2020  ..  .  ```.  .  
-000027a0: 6177 6169 7420 686c 7476 2e67 6574 2827  await hltv.get('
-000027b0: 6d61 7463 6865 7327 2c20 3233 3731 3230  matches', 237120
-000027c0: 312c 2027 7265 732d 7265 6769 6f6e 616c  1, 'res-regional
-000027d0: 2d73 6572 6965 732d 332d 6c61 7461 6d27  -series-3-latam'
-000027e0: 2c20 2749 4d50 4552 4941 4c27 2c20 274d  , 'IMPERIAL', 'M
-000027f0: 4942 5227 290a 2020 0a20 203e 3e3e 2028  IBR').  .  >>> (
-00002800: 3233 3731 3230 312c 2030 2c20 302c 2027  2371201, 0, 0, '
-00002810: 4c49 5645 272c 205b 7b27 6d61 706e 616d  LIVE', [{'mapnam
-00002820: 6527 3a20 2756 6572 7469 676f 272c 2027  e': 'Vertigo', '
-00002830: 725f 7465 616d 3127 3a20 2736 272c 2027  r_team1': '6', '
-00002840: 725f 7465 616d 3227 3a20 2731 3327 7d2c  r_team2': '13'},
-00002850: 207b 276d 6170 6e61 6d65 273a 2027 4d69   {'mapname': 'Mi
-00002860: 7261 6765 272c 2027 725f 7465 616d 3127  rage', 'r_team1'
-00002870: 3a20 272d 272c 2027 725f 7465 616d 3227  : '-', 'r_team2'
-00002880: 3a20 272d 277d 2c20 7b27 6d61 706e 616d  : '-'}, {'mapnam
-00002890: 6527 3a20 2741 6e75 6269 7327 2c20 2772  e': 'Anubis', 'r
-000028a0: 5f74 6561 6d31 273a 2027 2d27 2c20 2772  _team1': '-', 'r
-000028b0: 5f74 6561 6d32 273a 2027 2d27 7d5d 2c20  _team2': '-'}], 
-000028c0: 5b5d 290a 2020 0a20 2060 6060 0a2d 2d2d  []).  .  ```.---
-000028d0: 0a23 2043 6f6e 6669 6773 0a0a 2a20 6d61  .# Configs..* ma
-000028e0: 785f 6465 6c61 793a 2069 6e74 203d 2031  x_delay: int = 1
-000028f0: 350a 0a20 2020 2041 7574 6f6d 6174 6963  5..    Automatic
-00002900: 616c 6c79 2069 6e63 7265 6173 696e 6720  ally increasing 
-00002910: 7265 636f 6e6e 6563 7469 6e67 2064 656c  reconnecting del
-00002920: 6179 2062 7920 3120 7365 6320 746f 206d  ay by 1 sec to m
-00002930: 6178 5f64 656c 6179 2028 6672 6f6d 2031  ax_delay (from 1
-00002940: 7320 746f 2035 7329 0a0a 2020 2020 6060  s to 5s)..    ``
-00002950: 600a 2020 2020 686c 7476 203d 2048 6c74  `.    hltv = Hlt
-00002960: 7628 6d61 785f 6465 6c61 793d 3529 0a20  v(max_delay=5). 
-00002970: 2020 200a 2020 2020 3e3e 3e46 6574 6368     .    >>>Fetch
-00002980: 696e 6720 6874 7470 733a 2f2f 7777 772e  ing https://www.
-00002990: 686c 7476 2e6f 7267 2f6d 6174 6368 6573  hltv.org/matches
-000029a0: 2f32 3337 3037 3237 2f66 617a 652d 7673  /2370727/faze-vs
-000029b0: 2d6e 6174 7573 2d76 696e 6365 7265 2d70  -natus-vincere-p
-000029c0: 676c 2d63 7332 2d6d 616a 6f72 2d63 6f70  gl-cs2-major-cop
-000029d0: 656e 6861 6765 6e2d 3230 3234 2c20 636f  enhagen-2024, co
-000029e0: 6465 3a20 3430 330a 2020 2020 3e3e 3e47  de: 403.    >>>G
-000029f0: 6f74 2034 3033 2066 6f72 6269 7474 656e  ot 403 forbitten
-00002a00: 0a20 2020 203e 3e3e 4361 6c6c 696e 6720  .    >>>Calling 
-00002a10: 6167 6169 6e2c 2069 6e63 7265 6173 696e  again, increasin
-00002a20: 6720 6465 6c61 7920 746f 2034 730a 2020  g delay to 4s.  
-00002a30: 2020 3e3e 3e46 6574 6368 696e 6720 6874    >>>Fetching ht
-00002a40: 7470 733a 2f2f 7777 772e 686c 7476 2e6f  tps://www.hltv.o
-00002a50: 7267 2f6d 6174 6368 6573 2f32 3337 3037  rg/matches/23707
-00002a60: 3237 2f66 617a 652d 7673 2d6e 6174 7573  27/faze-vs-natus
-00002a70: 2d76 696e 6365 7265 2d70 676c 2d63 7332  -vincere-pgl-cs2
-00002a80: 2d6d 616a 6f72 2d63 6f70 656e 6861 6765  -major-copenhage
-00002a90: 6e2d 3230 3234 2c20 636f 6465 3a20 3430  n-2024, code: 40
-00002aa0: 330a 2020 2020 3e3e 3e47 6f74 2034 3033  3.    >>>Got 403
-00002ab0: 2066 6f72 6269 7474 656e 0a20 2020 203e   forbitten.    >
-00002ac0: 3e3e 4361 6c6c 696e 6720 6167 6169 6e2c  >>Calling again,
-00002ad0: 2069 6e63 7265 6173 696e 6720 6465 6c61   increasing dela
-00002ae0: 7920 746f 2035 730a 2020 2020 6060 600a  y to 5s.    ```.
-00002af0: 0a2a 206d 6178 5f72 6574 7269 6573 3a20  .* max_retries: 
-00002b00: 696e 7420 3d20 300a 0a20 2020 204d 6178  int = 0..    Max
-00002b10: 2072 6574 7269 6573 2e20 3020 6f72 202d   retries. 0 or -
-00002b20: 3120 666f 7220 696e 6669 6e69 7479 2074  1 for infinity t
-00002b30: 7269 6573 2e0a 2020 2020 0a20 2020 2060  ries..    .    `
-00002b40: 6060 0a20 2020 2068 6c74 7620 3d20 486c  ``.    hltv = Hl
-00002b50: 7476 286d 6178 5f72 6574 7269 6573 3d32  tv(max_retries=2
-00002b60: 2c20 6465 6275 673d 5472 7565 290a 2020  , debug=True).  
-00002b70: 2020 7072 696e 7428 6177 6169 7420 686c    print(await hl
-00002b80: 7476 2e67 6574 5f62 6573 745f 706c 6179  tv.get_best_play
-00002b90: 6572 7328 2929 0a20 2020 200a 2020 2020  ers()).    .    
-00002ba0: 4372 6561 7469 6e67 2053 6573 7369 6f6e  Creating Session
-00002bb0: 0a20 2020 2054 7279 696e 6720 636f 6e6e  .    Trying conn
-00002bc0: 6563 7420 746f 2068 7474 7073 3a2f 2f77  ect to https://w
-00002bd0: 7777 2e68 6c74 762e 6f72 672f 7374 6174  ww.hltv.org/stat
-00002be0: 732f 706c 6179 6572 733f 7374 6172 7444  s/players?startD
-00002bf0: 6174 653d 3230 3234 2d30 312d 3031 2665  ate=2024-01-01&e
-00002c00: 6e64 4461 7465 3d32 3032 342d 3132 2d33  ndDate=2024-12-3
-00002c10: 3126 7261 6e6b 696e 6746 696c 7465 723d  1&rankingFilter=
-00002c20: 546f 7032 302c 2074 7279 2031 2f32 0a20  Top20, try 1/2. 
-00002c30: 2020 2054 7279 696e 6720 636f 6e6e 6563     Trying connec
-00002c40: 7420 746f 2068 7474 7073 3a2f 2f77 7777  t to https://www
-00002c50: 2e68 6c74 762e 6f72 672f 7374 6174 732f  .hltv.org/stats/
-00002c60: 706c 6179 6572 733f 7374 6172 7444 6174  players?startDat
-00002c70: 653d 3230 3234 2d30 312d 3031 2665 6e64  e=2024-01-01&end
-00002c80: 4461 7465 3d32 3032 342d 3132 2d33 3126  Date=2024-12-31&
-00002c90: 7261 6e6b 696e 6746 696c 7465 723d 546f  rankingFilter=To
-00002ca0: 7032 302c 2074 7279 2032 2f32 0a20 2020  p20, try 2/2.   
-00002cb0: 2043 6f6e 6e65 6374 696f 6e20 6661 696c   Connection fail
-00002cc0: 6564 0a20 2020 2060 6060 0a0a 2a20 7072  ed.    ```..* pr
-00002cd0: 6f78 795f 6c69 7374 3a20 6c69 7374 207c  oxy_list: list |
-00002ce0: 204e 6f6e 6520 3d20 4e6f 6e65 0a0a 2020   None = None..  
-00002cf0: 2020 6c69 7374 206f 6620 796f 7572 2070    list of your p
-00002d00: 726f 7869 6573 2c20 6966 2079 6f75 7220  roxies, if your 
-00002d10: 7072 6f78 6965 7320 646f 6573 6e74 2068  proxies doesnt h
-00002d20: 6176 6520 616e 7920 7072 6f74 6f63 6f6c  ave any protocol
-00002d30: 2079 6f75 2063 616e 2075 7365 2070 726f   you can use pro
-00002d40: 7879 5f70 726f 746f 636f 6c2e 0a20 2020  xy_protocol..   
-00002d50: 204e 6f74 653a 2054 6f20 6164 6420 6e6f   Note: To add no
-00002d60: 6e70 726f 7879 2074 6f20 6c69 7374 206a  nproxy to list j
-00002d70: 7573 7420 7075 7420 2727 2074 6f20 6974  ust put '' to it
-00002d80: 2c20 796f 7520 6361 6e20 6669 6e64 2065  , you can find e
-00002d90: 7861 6d70 6c65 2077 6974 6820 6172 0a0a  xample with ar..
-00002da0: 2a20 7072 6f78 795f 7061 7468 3a20 7374  * proxy_path: st
-00002db0: 7220 7c20 4e6f 6e65 203d 204e 6f6e 650a  r | None = None.
-00002dc0: 0a20 2020 2050 6174 6820 746f 2079 6f75  .    Path to you
-00002dd0: 7220 7072 6f78 7920 2870 726f 7879 5f6c  r proxy (proxy_l
-00002de0: 6973 7420 7769 6c6c 2062 6520 6967 6e6f  ist will be igno
-00002df0: 7265 6429 2e20 4966 2079 6f75 7220 7072  red). If your pr
-00002e00: 6f78 6965 7320 646f 6573 6e74 2068 6176  oxies doesnt hav
-00002e10: 6520 616e 7920 7072 6f74 6f63 6f6c 2079  e any protocol y
-00002e20: 6f75 2063 616e 2075 7365 2070 726f 7879  ou can use proxy
-00002e30: 5f70 726f 746f 636f 6c0a 0a2a 2070 726f  _protocol..* pro
-00002e40: 7879 5f70 726f 746f 636f 6c3a 2073 7472  xy_protocol: str
-00002e50: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
-00002e60: 0a20 2020 2050 726f 7879 2070 726f 746f  .    Proxy proto
-00002e70: 636f 6c2e 2059 6f75 7220 7072 6f78 6965  col. Your proxie
-00002e80: 7320 6060 6068 6c74 7620 3d20 486c 7476  s ```hltv = Hltv
-00002e90: 2870 726f 7879 5f70 726f 746f 636f 6c3d  (proxy_protocol=
-00002ea0: 2768 7474 7027 202e 2e2e 2920 2d3e 2027  'http' ...) -> '
-00002eb0: 3131 2e31 312e 3131 2e31 313a 3131 3131  11.11.11.11:1111
-00002ec0: 2720 2d3e 2027 6874 7470 3a2f 2f31 312e  ' -> 'http://11.
-00002ed0: 3131 2e31 312e 3131 3a31 3131 3127 0a0a  11.11.11:1111'..
-00002ee0: 2a20 6465 6c65 7465 5f70 726f 7879 3a20  * delete_proxy: 
-00002ef0: 626f 6f6c 203d 2046 616c 7365 0a0a 2020  bool = False..  
-00002f00: 2020 5265 6d6f 7665 7320 7072 6f78 7920    Removes proxy 
-00002f10: 6672 6f6d 206c 6973 7420 2870 726f 7879  from list (proxy
-00002f20: 5f70 6174 6820 696e 636c 7564 6564 2920  _path included) 
-00002f30: 6966 2063 6f6e 6e65 6374 696f 6e20 756e  if connection un
-00002f40: 7375 6363 6573 7366 756c 6c79 0a0a 2a20  successfully..* 
-00002f50: 7469 6d65 6f75 743a 2069 6e74 203d 2035  timeout: int = 5
-00002f60: 0a0a 2020 2020 4d61 7820 7469 6d65 2074  ..    Max time t
-00002f70: 6f20 636c 6f73 6520 636f 6e6e 6563 7469  o close connecti
-00002f80: 6f6e 2e20 5265 636f 6d6d 656e 6465 6420  on. Recommended 
-00002f90: 746f 2075 7365 2074 696d 656f 7574 3d31  to use timeout=1
-00002fa0: 2069 6620 796f 7520 6172 6520 7573 696e   if you are usin
-00002fb0: 6720 7261 6e64 6f6d 2070 726f 7869 6573  g random proxies
-00002fc0: 2e0a 0a2a 2064 6562 7567 3a20 626f 6f6c  ...* debug: bool
-00002fd0: 203d 2046 616c 7365 0a0a 2a20 747a 3a20   = False..* tz: 
-00002fe0: 7374 7220 3d20 2745 7572 6f70 652f 436f  str = 'Europe/Co
-00002ff0: 7065 6e68 6167 656e 273a 0a20 2020 200a  penhagen':.    .
-00003000: 2020 2020 5469 6d65 7a6f 6e65 2063 6f6e      Timezone con
-00003010: 6669 672e 200a 200a 2020 2020 3c61 2068  fig. . .    <a h
-00003020: 7265 663d 2768 7474 7073 3a2f 2f67 6973  ref='https://gis
-00003030: 742e 6769 7468 7562 2e63 6f6d 2f68 6579  t.github.com/hey
-00003040: 616c 6578 656a 2f38 6266 3638 3866 6436  alexej/8bf688fd6
-00003050: 3764 3731 3939 6265 3461 3136 3832 6233  7d7199be4a1682b3
-00003060: 6565 6337 3536 3827 3e54 6170 2068 6572  eec7568'>Tap her
-00003070: 6520 3c2f 613e 2074 6f20 7365 6520 616c  e </a> to see al
-00003080: 6c20 6176 6169 6c61 626c 6520 7469 6d65  l available time
-00003090: 7a6f 6e65 730a 0a0a 2d2d 2d0a 2320 4578  zones...---.# Ex
-000030a0: 616d 706c 6573 0a0a 2a2a 2a2a 5369 6d70  amples..****Simp
-000030b0: 6c65 2045 7861 6d70 6c65 2a2a 2a2a 0a0a  le Example****..
-000030c0: 6060 600a 6672 6f6d 2068 6c74 765f 6173  ```.from hltv_as
-000030d0: 796e 635f 6170 6920 696d 706f 7274 2048  ync_api import H
-000030e0: 6c74 760a 0a0a 6173 796e 6320 6465 6620  ltv...async def 
-000030f0: 7465 7374 2829 3a0a 0a20 2020 2061 7379  test():..    asy
-00003100: 6e63 2077 6974 6820 486c 7476 2829 2061  nc with Hltv() a
-00003110: 7320 686c 7476 3a0a 2020 2020 2020 7072  s hltv:.      pr
-00003120: 696e 7428 6177 6169 7420 686c 7476 2e67  int(await hltv.g
-00003130: 6574 5f65 7665 6e74 5f69 6e66 6f28 3731  et_event_info(71
-00003140: 3438 2c20 2770 676c 2d63 7332 2d6d 616a  48, 'pgl-cs2-maj
-00003150: 6f72 2d63 6f70 656e 6861 6765 6e2d 3230  or-copenhagen-20
-00003160: 3234 2729 290a 0a69 6620 5f5f 6e61 6d65  24'))..if __name
-00003170: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00003180: 3a0a 2020 2020 6173 796e 6369 6f2e 7275  :.    asyncio.ru
-00003190: 6e28 7465 7374 2829 290a 6060 600a 0a2a  n(test()).```..*
-000031a0: 2a2a 2a50 726f 7879 2050 6172 7365 722a  ***Proxy Parser*
-000031b0: 2a2a 2a0a 0a60 6060 0a66 726f 6d20 686c  ***..```.from hl
-000031c0: 7476 5f61 7379 6e63 5f61 7069 2069 6d70  tv_async_api imp
-000031d0: 6f72 7420 486c 7476 0a0a 0a61 7379 6e63  ort Hltv...async
-000031e0: 2064 6566 2074 6573 7428 293a 0a0a 2020   def test():..  
-000031f0: 2020 686c 7476 203d 2048 6c74 7628 6465    hltv = Hltv(de
-00003200: 6275 673d 5472 7565 2c20 7072 6f78 795f  bug=True, proxy_
-00003210: 7061 7468 3d27 7072 6f78 795f 7465 7374  path='proxy_test
-00003220: 2e74 7874 272c 2074 696d 656f 7574 3d31  .txt', timeout=1
-00003230: 2c20 6465 6c65 7465 5f70 726f 7879 3d54  , delete_proxy=T
-00003240: 7275 652c 2070 726f 7879 5f70 726f 746f  rue, proxy_proto
-00003250: 636f 6c3d 2768 7474 7027 290a 2020 2020  col='http').    
-00003260: 0a20 2020 2070 7269 6e74 2861 7761 6974  .    print(await
-00003270: 2068 6c74 762e 6765 745f 6576 656e 745f   hltv.get_event_
-00003280: 696e 666f 2837 3134 382c 2027 7067 6c2d  info(7148, 'pgl-
-00003290: 6373 322d 6d61 6a6f 722d 636f 7065 6e68  cs2-major-copenh
-000032a0: 6167 656e 2d32 3032 3427 2929 0a0a 6966  agen-2024'))..if
-000032b0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-000032c0: 6d61 696e 5f5f 223a 0a20 2020 2061 7379  main__":.    asy
-000032d0: 6e63 696f 2e72 756e 2874 6573 7428 2929  ncio.run(test())
-000032e0: 0a60 6060 0a0a 2a2a 2a2a 4175 746f 6d61  .```..****Automa
-000032f0: 7469 6320 7061 7273 6572 2077 6974 6820  tic parser with 
-00003300: 6172 7120 616e 6420 7265 6469 732a 2a2a  arq and redis***
-00003310: 2a0a 0a2d 2074 6f20 7275 6e20 7479 7065  *..- to run type
-00003320: 2022 6172 7120 5041 5448 5f54 4f5f 4649   "arq PATH_TO_FI
-00003330: 4c45 2e57 6f72 6b65 7253 6574 7469 6e67  LE.WorkerSetting
-00003340: 7322 0a0a 2020 2020 6060 600a 2020 2020  s"..    ```.    
-00003350: 696d 706f 7274 2075 6a73 6f6e 0a20 2020  import ujson.   
-00003360: 2069 6d70 6f72 7420 6173 796e 6369 6f0a   import asyncio.
-00003370: 2020 2020 6672 6f6d 2061 7271 2069 6d70      from arq imp
-00003380: 6f72 7420 6372 6f6e 0a20 2020 2066 726f  ort cron.    fro
-00003390: 6d20 7265 6469 732e 6173 796e 6369 6f20  m redis.asyncio 
-000033a0: 696d 706f 7274 2052 6564 6973 2c20 436f  import Redis, Co
-000033b0: 6e6e 6563 7469 6f6e 506f 6f6c 0a20 2020  nnectionPool.   
-000033c0: 200a 2020 2020 6672 6f6d 2068 6c74 765f   .    from hltv_
-000033d0: 6173 796e 635f 6170 6920 696d 706f 7274  async_api import
-000033e0: 2048 6c74 760a 2020 2020 0a20 2020 200a   Hltv.    .    .
-000033f0: 2020 2020 0a20 2020 2061 7379 6e63 2064      .    async d
-00003400: 6566 2073 7461 7274 7570 2863 7478 293a  ef startup(ctx):
-00003410: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-00003420: 6974 6820 486c 7476 286d 6178 5f64 656c  ith Hltv(max_del
-00003430: 6179 3d35 2c20 7072 6f78 795f 7061 7468  ay=5, proxy_path
-00003440: 3d27 7072 6f78 6965 732e 7478 7427 2c20  ='proxies.txt', 
-00003450: 6465 6275 673d 5472 7565 2920 6173 2068  debug=True) as h
-00003460: 6c74 763a 0a20 2020 2020 2020 2020 2020  ltv:.           
-00003470: 2020 2063 7478 5b22 686c 7476 225d 203d     ctx["hltv"] =
-00003480: 2068 6c74 760a 2020 0a20 2020 2020 2020   hltv.  .       
-00003490: 2063 7478 5b22 7265 6469 7322 5d20 3d20   ctx["redis"] = 
-000034a0: 7265 6469 735f 636c 6965 6e74 203d 2052  redis_client = R
-000034b0: 6564 6973 280a 2020 2020 2020 2020 2020  edis(.          
-000034c0: 2020 636f 6e6e 6563 7469 6f6e 5f70 6f6f    connection_poo
-000034d0: 6c3d 436f 6e6e 6563 7469 6f6e 506f 6f6c  l=ConnectionPool
-000034e0: 2e66 726f 6d5f 7572 6c28 7365 7474 696e  .from_url(settin
-000034f0: 6773 2e72 6564 6973 5f75 726c 2929 0a20  gs.redis_url)). 
-00003500: 2020 2020 2020 206c 6f67 6765 722e 7375         logger.su
-00003510: 6363 6573 7328 6622 5363 6865 6475 6c65  ccess(f"Schedule
-00003520: 7220 7374 6172 7465 642e 2055 5443 2074  r started. UTC t
-00003530: 696d 6520 7b64 6174 6574 696d 652e 7574  ime {datetime.ut
-00003540: 636e 6f77 2829 7d22 290a 2020 2020 0a20  cnow()}").    . 
-00003550: 2020 200a 2020 2020 6173 796e 6320 6465     .    async de
-00003560: 6620 7368 7574 646f 776e 2863 7478 293a  f shutdown(ctx):
-00003570: 0a20 2020 2020 2020 2061 7761 6974 2063  .        await c
-00003580: 7478 5b22 7265 6469 7322 5d2e 636c 6f73  tx["redis"].clos
-00003590: 6528 290a 2020 2020 0a20 2020 200a 2020  e().    .    .  
-000035a0: 2020 6173 796e 6320 6465 6620 7061 7273    async def pars
-000035b0: 655f 6d61 7463 6865 7328 6374 7829 3a0a  e_matches(ctx):.
-000035c0: 2020 2020 2020 2020 686c 7476 203d 2063          hltv = c
-000035d0: 7478 5b22 686c 7476 225d 0a20 2020 2020  tx["hltv"].     
-000035e0: 2020 2072 6564 6973 203d 2063 7478 5b22     redis = ctx["
-000035f0: 7265 6469 7322 5d0a 2020 2020 2020 2020  redis"].        
-00003600: 6d61 7463 6865 7320 3d20 6177 6169 7420  matches = await 
-00003610: 686c 7476 2e67 6574 5f75 7063 6f6d 696e  hltv.get_upcomin
-00003620: 675f 6d61 7463 6865 7328 312c 2031 290a  g_matches(1, 1).
-00003630: 2020 2020 2020 2020 6966 206d 6174 6368          if match
-00003640: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00003650: 6177 6169 7420 7265 6469 732e 7365 7428  await redis.set(
-00003660: 226d 6174 6368 6573 222c 2075 6a73 6f6e  "matches", ujson
-00003670: 2e64 756d 7073 286d 6174 6368 6573 2929  .dumps(matches))
-00003680: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00003690: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000036a0: 722e 6572 726f 7228 2265 7272 6f72 2070  r.error("error p
-000036b0: 6172 7369 6e67 206d 6174 6368 6573 2229  arsing matches")
-000036c0: 0a20 2020 200a 2020 2020 6173 796e 6320  .    .    async 
-000036d0: 6465 6620 7061 7273 655f 6576 656e 7473  def parse_events
-000036e0: 2863 7478 293a 0a20 2020 2020 2020 2068  (ctx):.        h
-000036f0: 6c74 7620 3d20 6374 785b 2268 6c74 7622  ltv = ctx["hltv"
-00003700: 5d0a 2020 2020 2020 2020 7265 6469 7320  ].        redis 
-00003710: 3d20 6374 785b 2272 6564 6973 225d 0a20  = ctx["redis"]. 
-00003720: 2020 2020 2020 2065 7665 6e74 7320 3d20         events = 
-00003730: 6177 6169 7420 686c 7476 2e67 6574 5f65  await hltv.get_e
-00003740: 7665 6e74 7328 290a 2020 2020 2020 2020  vents().        
-00003750: 6966 2065 7665 6e74 733a 0a20 2020 2020  if events:.     
-00003760: 2020 2020 2020 2061 7761 6974 2072 6564         await red
-00003770: 6973 2e73 6574 2822 6576 656e 7473 222c  is.set("events",
-00003780: 2075 6a73 6f6e 2e64 756d 7073 2865 7665   ujson.dumps(eve
-00003790: 6e74 7329 290a 2020 2020 2020 2020 656c  nts)).        el
-000037a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000037b0: 6c6f 6767 6572 2e65 7272 6f72 2822 6572  logger.error("er
-000037c0: 726f 7220 7061 7273 696e 6720 6576 656e  ror parsing even
-000037d0: 7473 2229 0a20 2020 200a 2020 2020 0a20  ts").    .    . 
-000037e0: 2020 2061 7379 6e63 2064 6566 2070 6172     async def par
-000037f0: 7365 5f74 6f70 5f74 6561 6d73 2863 7478  se_top_teams(ctx
-00003800: 293a 0a20 2020 2020 2020 2068 6c74 7620  ):.        hltv 
-00003810: 3d20 6374 785b 2268 6c74 7622 5d0a 2020  = ctx["hltv"].  
-00003820: 2020 2020 2020 7265 6469 7320 3d20 6374        redis = ct
-00003830: 785b 2272 6564 6973 225d 0a20 2020 2020  x["redis"].     
-00003840: 2020 2074 6f70 5f74 6561 6d73 203d 2061     top_teams = a
-00003850: 7761 6974 2068 6c74 762e 6765 745f 746f  wait hltv.get_to
-00003860: 705f 7465 616d 7328 3330 290a 2020 2020  p_teams(30).    
-00003870: 2020 2020 6966 2074 6f70 5f74 6561 6d73      if top_teams
-00003880: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-00003890: 6169 7420 7265 6469 732e 7365 7428 2274  ait redis.set("t
-000038a0: 6f70 5f74 6561 6d73 222c 2075 6a73 6f6e  op_teams", ujson
-000038b0: 2e64 756d 7073 2874 6f70 5f74 6561 6d73  .dumps(top_teams
-000038c0: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
-000038d0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-000038e0: 6765 722e 6572 726f 7228 2265 7272 6f72  ger.error("error
-000038f0: 2070 6172 7369 6e67 2074 6f70 2074 6561   parsing top tea
-00003900: 6d73 2229 0a20 2020 200a 2020 2020 0a20  ms").    .    . 
-00003910: 2020 2061 7379 6e63 2064 6566 2070 6172     async def par
-00003920: 7365 5f74 6f70 5f70 6c61 7965 7273 2863  se_top_players(c
-00003930: 7478 293a 0a20 2020 2020 2020 2068 6c74  tx):.        hlt
-00003940: 7620 3d20 6374 785b 2268 6c74 7622 5d0a  v = ctx["hltv"].
-00003950: 2020 2020 2020 2020 7265 6469 7320 3d20          redis = 
-00003960: 6374 785b 2272 6564 6973 225d 0a20 2020  ctx["redis"].   
-00003970: 2020 2020 2074 6f70 5f70 6c61 7965 7273       top_players
-00003980: 203d 2061 7761 6974 2068 6c74 762e 6765   = await hltv.ge
-00003990: 745f 6265 7374 5f70 6c61 7965 7273 2833  t_best_players(3
-000039a0: 3029 0a20 2020 2020 2020 2069 6620 746f  0).        if to
-000039b0: 705f 706c 6179 6572 733a 0a20 2020 2020  p_players:.     
-000039c0: 2020 2020 2020 2061 7761 6974 2072 6564         await red
-000039d0: 6973 2e73 6574 2822 746f 705f 7465 616d  is.set("top_team
-000039e0: 7322 2c20 756a 736f 6e2e 6475 6d70 7328  s", ujson.dumps(
-000039f0: 746f 705f 706c 6179 6572 7329 290a 2020  top_players)).  
-00003a00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00003a10: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00003a20: 7272 6f72 2822 6572 726f 7220 7061 7273  rror("error pars
-00003a30: 696e 6720 746f 7020 706c 6179 6572 7322  ing top players"
-00003a40: 290a 2020 2020 0a20 2020 200a 2020 2020  ).    .    .    
-00003a50: 6173 796e 6320 6465 6620 7061 7273 655f  async def parse_
-00003a60: 6c61 7374 5f6e 6577 7328 6374 7829 3a0a  last_news(ctx):.
-00003a70: 2020 2020 2020 2020 686c 7476 203d 2063          hltv = c
-00003a80: 7478 5b22 686c 7476 225d 0a20 2020 2020  tx["hltv"].     
-00003a90: 2020 2072 6564 6973 203d 2063 7478 5b22     redis = ctx["
-00003aa0: 7265 6469 7322 5d0a 2020 2020 2020 2020  redis"].        
-00003ab0: 6e65 7773 203d 2061 7761 6974 2068 6c74  news = await hlt
-00003ac0: 762e 6765 745f 6c61 7374 5f6e 6577 7328  v.get_last_news(
-00003ad0: 6f6e 6c79 5f74 6f64 6179 3d54 7275 652c  only_today=True,
-00003ae0: 206d 6178 5f72 6567 5f6e 6577 733d 3429   max_reg_news=4)
-00003af0: 0a20 2020 2020 2020 2069 6620 6e65 7773  .        if news
-00003b00: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-00003b10: 6169 7420 7265 6469 732e 7365 7428 226e  ait redis.set("n
-00003b20: 6577 7322 2c20 756a 736f 6e2e 6475 6d70  ews", ujson.dump
-00003b30: 7328 6e65 7773 2929 0a20 2020 2020 2020  s(news)).       
-00003b40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003b50: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
-00003b60: 2265 7272 6f72 2070 6172 7369 6e67 206e  "error parsing n
-00003b70: 6577 7322 290a 2020 2020 0a20 2020 200a  ews").    .    .
-00003b80: 2020 2020 636c 6173 7320 576f 726b 6572      class Worker
-00003b90: 5365 7474 696e 6773 3a0a 2020 2020 2020  Settings:.      
-00003ba0: 2020 7265 6469 735f 7365 7474 696e 6773    redis_settings
-00003bb0: 203d 2073 6574 7469 6e67 732e 7265 6469   = settings.redi
-00003bc0: 735f 706f 6f6c 0a20 2020 2020 2020 206f  s_pool.        o
-00003bd0: 6e5f 7374 6172 7475 7020 3d20 7374 6172  n_startup = star
-00003be0: 7475 700a 2020 2020 2020 2020 6f6e 5f73  tup.        on_s
-00003bf0: 6875 7464 6f77 6e20 3d20 7368 7574 646f  hutdown = shutdo
-00003c00: 776e 0a20 2020 2020 2020 2066 756e 6374  wn.        funct
-00003c10: 696f 6e73 203d 205b 7061 7273 655f 6d61  ions = [parse_ma
-00003c20: 7463 6865 732c 0a20 2020 2020 2020 2020  tches,.         
-00003c30: 2020 2020 2020 2020 2020 2020 7061 7273              pars
-00003c40: 655f 6576 656e 7473 2c0a 2020 2020 2020  e_events,.      
-00003c50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003c60: 6172 7365 5f74 6f70 5f74 6561 6d73 2c0a  arse_top_teams,.
-00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 2020 2020 2070 6172 7365 5f74 6f70 5f70       parse_top_p
-00003c90: 6c61 7965 7273 2c0a 2020 2020 2020 2020  layers,.        
+000003e0: 6f72 2050 7974 686f 6e2e 200a 2320 5573  or Python. .# Us
+000003f0: 6520 6f6e 6c79 2069 6e20 6e6f 6e2d 636f  e only in non-co
+00000400: 6d6d 6572 6369 616c 2070 7572 706f 7365  mmercial purpose
+00000410: 730a 0a0a 2a2a 5468 6973 2070 6167 6520  s...**This page 
+00000420: 6973 206e 6f74 2063 6f6d 706c 6574 6564  is not completed
+00000430: 2c20 6e6f 7420 616c 6c20 6d65 7468 6f64  , not all method
+00000440: 7320 616e 6420 636f 6e66 6967 7320 6172  s and configs ar
+00000450: 6520 7772 6974 7465 6e2a 2a0a 0a0a 2320  e written**...# 
+00000460: 4665 6174 7572 6573 0a0a 0a2a 202a 2a53  Features...* **S
+00000470: 696d 706c 6520 5573 6167 652a 2a20 2869  imple Usage** (i
+00000480: 7473 2072 6561 6c6c 7920 7369 6d70 6c65  ts really simple
+00000490: 290a 0a0a 2a20 2a2a 4e65 7720 616e 6420  )...* **New and 
+000004a0: 6d6f 6465 726e 2066 756c 6c79 2061 7379  modern fully asy
+000004b0: 6e63 206c 6962 7261 7279 2a2a 0a0a 0a2a  nc library**...*
+000004c0: 202a 2a48 7567 6520 616d 6f75 6e74 206f   **Huge amount o
+000004d0: 6620 6f70 7469 6f6e 732a 2a0a 0a0a 2a20  f options**...* 
+000004e0: 2a2a 5375 7070 6f72 7473 2070 726f 7879  **Supports proxy
+000004f0: 2075 7361 6765 2a2a 0a0a 0a2a 202a 2a4d   usage**...* **M
+00000500: 6164 6520 7769 7468 206c 6f76 6520 3c33  ade with love <3
+00000510: 2a2a 0a0a 0a2d 2d2d 0a0a 2320 496e 7374  **...---..# Inst
+00000520: 616c 6c61 7469 6f6e 0a0a 6060 600a 7069  allation..```.pi
+00000530: 7020 696e 7374 616c 6c20 686c 7476 2d61  p install hltv-a
+00000540: 7379 6e63 2d61 7069 0a60 6060 0a0a 2d2d  sync-api.```..--
+00000550: 2d0a 0a0a 2320 5369 6d70 6c65 2055 7361  -...# Simple Usa
+00000560: 6765 0a0a 2020 2020 6060 600a 0a20 2020  ge..    ```..   
+00000570: 2066 726f 6d20 686c 7476 5f61 7379 6e63   from hltv_async
+00000580: 5f61 7069 2069 6d70 6f72 7420 486c 7476  _api import Hltv
+00000590: 0a20 2020 200a 2020 2020 6173 796e 6320  .    .    async 
+000005a0: 7769 7468 2048 6c74 7628 2920 6173 2068  with Hltv() as h
+000005b0: 6c74 763a 0a20 2020 2020 2070 7269 6e74  ltv:.      print
+000005c0: 2861 7761 6974 2068 6c74 762e 6765 745f  (await hltv.get_
+000005d0: 6576 656e 745f 696e 666f 2837 3134 382c  event_info(7148,
+000005e0: 2027 5047 4c20 4353 3220 4d61 6a6f 7220   'PGL CS2 Major 
+000005f0: 436f 7065 6e68 6167 656e 3230 3234 2729  Copenhagen2024')
+00000600: 290a 0a20 2020 2060 6060 0a0a 2020 2a2a  )..    ```..  **
+00000610: 4f52 2a2a 0a0a 2020 2020 6060 600a 0a20  OR**..    ```.. 
+00000620: 2020 2066 726f 6d20 686c 7476 5f61 7379     from hltv_asy
+00000630: 6e63 5f61 7069 2069 6d70 6f72 7420 486c  nc_api import Hl
+00000640: 7476 0a20 2020 200a 2020 2020 686c 7476  tv.    .    hltv
+00000650: 203d 2048 6c74 7628 290a 2020 2020 7072   = Hltv().    pr
+00000660: 696e 7428 6177 6169 7420 686c 7476 2e67  int(await hltv.g
+00000670: 6574 5f65 7665 6e74 5f69 6e66 6f28 3731  et_event_info(71
+00000680: 3438 2c20 2750 474c 2043 5332 204d 616a  48, 'PGL CS2 Maj
+00000690: 6f72 2043 6f70 656e 6861 6765 6e32 3032  or Copenhagen202
+000006a0: 3427 2929 0a20 2020 2061 7761 6974 2068  4')).    await h
+000006b0: 6c74 762e 636c 6f73 6528 290a 0a20 2020  ltv.close()..   
+000006c0: 2060 6060 0a0a 0a2d 2d2d 0a0a 2320 436f   ```...---..# Co
+000006d0: 6e66 6967 730a 0a2a 206d 6178 5f64 656c  nfigs..* max_del
+000006e0: 6179 3a20 696e 7420 3d20 3135 0a0a 2020  ay: int = 15..  
+000006f0: 2020 4175 746f 6d61 7469 6361 6c6c 7920    Automatically 
+00000700: 696e 6372 6561 7369 6e67 2072 6563 6f6e  increasing recon
+00000710: 6e65 6374 696e 6720 6465 6c61 7920 6279  necting delay by
+00000720: 2031 2073 6563 2074 6f20 6d61 785f 6465   1 sec to max_de
+00000730: 6c61 7920 2866 726f 6d20 3173 2074 6f20  lay (from 1s to 
+00000740: 3573 290a 0a20 2020 2060 6060 0a20 2020  5s)..    ```.   
+00000750: 2068 6c74 7620 3d20 486c 7476 286d 6178   hltv = Hltv(max
+00000760: 5f64 656c 6179 3d35 290a 2020 2020 0a20  _delay=5).    . 
+00000770: 2020 203e 3e3e 4665 7463 6869 6e67 2068     >>>Fetching h
+00000780: 7474 7073 3a2f 2f77 7777 2e68 6c74 762e  ttps://www.hltv.
+00000790: 6f72 672f 6d61 7463 6865 732f 3233 3730  org/matches/2370
+000007a0: 3732 372f 6661 7a65 2d76 732d 6e61 7475  727/faze-vs-natu
+000007b0: 732d 7669 6e63 6572 652d 7067 6c2d 6373  s-vincere-pgl-cs
+000007c0: 322d 6d61 6a6f 722d 636f 7065 6e68 6167  2-major-copenhag
+000007d0: 656e 2d32 3032 342c 2063 6f64 653a 2034  en-2024, code: 4
+000007e0: 3033 0a20 2020 203e 3e3e 476f 7420 3430  03.    >>>Got 40
+000007f0: 3320 666f 7262 6974 7465 6e0a 2020 2020  3 forbitten.    
+00000800: 3e3e 3e43 616c 6c69 6e67 2061 6761 696e  >>>Calling again
+00000810: 2c20 696e 6372 6561 7369 6e67 2064 656c  , increasing del
+00000820: 6179 2074 6f20 3473 0a20 2020 203e 3e3e  ay to 4s.    >>>
+00000830: 4665 7463 6869 6e67 2068 7474 7073 3a2f  Fetching https:/
+00000840: 2f77 7777 2e68 6c74 762e 6f72 672f 6d61  /www.hltv.org/ma
+00000850: 7463 6865 732f 3233 3730 3732 372f 6661  tches/2370727/fa
+00000860: 7a65 2d76 732d 6e61 7475 732d 7669 6e63  ze-vs-natus-vinc
+00000870: 6572 652d 7067 6c2d 6373 322d 6d61 6a6f  ere-pgl-cs2-majo
+00000880: 722d 636f 7065 6e68 6167 656e 2d32 3032  r-copenhagen-202
+00000890: 342c 2063 6f64 653a 2034 3033 0a20 2020  4, code: 403.   
+000008a0: 203e 3e3e 476f 7420 3430 3320 666f 7262   >>>Got 403 forb
+000008b0: 6974 7465 6e0a 2020 2020 3e3e 3e43 616c  itten.    >>>Cal
+000008c0: 6c69 6e67 2061 6761 696e 2c20 696e 6372  ling again, incr
+000008d0: 6561 7369 6e67 2064 656c 6179 2074 6f20  easing delay to 
+000008e0: 3573 0a20 2020 2060 6060 0a0a 2a20 6d61  5s.    ```..* ma
+000008f0: 785f 7265 7472 6965 733a 2069 6e74 203d  x_retries: int =
+00000900: 2030 0a0a 2020 2020 4d61 7820 7265 7472   0..    Max retr
+00000910: 6965 732e 2030 206f 7220 2d31 2066 6f72  ies. 0 or -1 for
+00000920: 2069 6e66 696e 6974 7920 7472 6965 732e   infinity tries.
+00000930: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
+00000940: 2020 686c 7476 203d 2048 6c74 7628 6d61    hltv = Hltv(ma
+00000950: 785f 7265 7472 6965 733d 322c 2064 6562  x_retries=2, deb
+00000960: 7567 3d54 7275 6529 0a20 2020 2070 7269  ug=True).    pri
+00000970: 6e74 2861 7761 6974 2068 6c74 762e 6765  nt(await hltv.ge
+00000980: 745f 6265 7374 5f70 6c61 7965 7273 2829  t_best_players()
+00000990: 290a 2020 2020 0a20 2020 2043 7265 6174  ).    .    Creat
+000009a0: 696e 6720 5365 7373 696f 6e0a 2020 2020  ing Session.    
+000009b0: 5472 7969 6e67 2063 6f6e 6e65 6374 2074  Trying connect t
+000009c0: 6f20 6874 7470 733a 2f2f 7777 772e 686c  o https://www.hl
+000009d0: 7476 2e6f 7267 2f73 7461 7473 2f70 6c61  tv.org/stats/pla
+000009e0: 7965 7273 3f73 7461 7274 4461 7465 3d32  yers?startDate=2
+000009f0: 3032 342d 3031 2d30 3126 656e 6444 6174  024-01-01&endDat
+00000a00: 653d 3230 3234 2d31 322d 3331 2672 616e  e=2024-12-31&ran
+00000a10: 6b69 6e67 4669 6c74 6572 3d54 6f70 3230  kingFilter=Top20
+00000a20: 2c20 7472 7920 312f 320a 2020 2020 5472  , try 1/2.    Tr
+00000a30: 7969 6e67 2063 6f6e 6e65 6374 2074 6f20  ying connect to 
+00000a40: 6874 7470 733a 2f2f 7777 772e 686c 7476  https://www.hltv
+00000a50: 2e6f 7267 2f73 7461 7473 2f70 6c61 7965  .org/stats/playe
+00000a60: 7273 3f73 7461 7274 4461 7465 3d32 3032  rs?startDate=202
+00000a70: 342d 3031 2d30 3126 656e 6444 6174 653d  4-01-01&endDate=
+00000a80: 3230 3234 2d31 322d 3331 2672 616e 6b69  2024-12-31&ranki
+00000a90: 6e67 4669 6c74 6572 3d54 6f70 3230 2c20  ngFilter=Top20, 
+00000aa0: 7472 7920 322f 320a 2020 2020 436f 6e6e  try 2/2.    Conn
+00000ab0: 6563 7469 6f6e 2066 6169 6c65 640a 2020  ection failed.  
+00000ac0: 2020 6060 600a 0a2a 2070 726f 7879 5f6c    ```..* proxy_l
+00000ad0: 6973 743a 206c 6973 7420 7c20 4e6f 6e65  ist: list | None
+00000ae0: 203d 204e 6f6e 650a 0a20 2020 206c 6973   = None..    lis
+00000af0: 7420 6f66 2079 6f75 7220 7072 6f78 6965  t of your proxie
+00000b00: 732c 2069 6620 796f 7572 2070 726f 7869  s, if your proxi
+00000b10: 6573 2064 6f65 736e 7420 6861 7665 2061  es doesnt have a
+00000b20: 6e79 2070 726f 746f 636f 6c20 796f 7520  ny protocol you 
+00000b30: 6361 6e20 7573 6520 7072 6f78 795f 7072  can use proxy_pr
+00000b40: 6f74 6f63 6f6c 2e0a 2020 2020 4e6f 7465  otocol..    Note
+00000b50: 3a20 546f 2061 6464 206e 6f6e 2d70 726f  : To add non-pro
+00000b60: 7879 2074 6f20 6c69 7374 206a 7573 7420  xy to list just 
+00000b70: 7075 7420 2727 2074 6f20 6974 2c20 796f  put '' to it, yo
+00000b80: 7520 6361 6e20 6669 6e64 2065 7861 6d70  u can find examp
+00000b90: 6c65 2077 6974 6820 6172 0a0a 2a20 7072  le with ar..* pr
+00000ba0: 6f78 795f 7061 7468 3a20 7374 7220 7c20  oxy_path: str | 
+00000bb0: 4e6f 6e65 203d 204e 6f6e 650a 0a20 2020  None = None..   
+00000bc0: 2050 6174 6820 746f 2079 6f75 7220 7072   Path to your pr
+00000bd0: 6f78 7920 2870 726f 7879 5f6c 6973 7420  oxy (proxy_list 
+00000be0: 7769 6c6c 2062 6520 6967 6e6f 7265 6429  will be ignored)
+00000bf0: 2e20 4966 2079 6f75 7220 7072 6f78 6965  . If your proxie
+00000c00: 7320 646f 6573 6e74 2068 6176 6520 616e  s doesnt have an
+00000c10: 7920 7072 6f74 6f63 6f6c 2079 6f75 2063  y protocol you c
+00000c20: 616e 2075 7365 2070 726f 7879 5f70 726f  an use proxy_pro
+00000c30: 746f 636f 6c0a 0a2a 2070 726f 7879 5f70  tocol..* proxy_p
+00000c40: 726f 746f 636f 6c3a 2073 7472 207c 204e  rotocol: str | N
+00000c50: 6f6e 6520 3d20 4e6f 6e65 2c0a 0a20 2020  one = None,..   
+00000c60: 2050 726f 7879 2070 726f 746f 636f 6c2e   Proxy protocol.
+00000c70: 2059 6f75 7220 7072 6f78 6965 7320 6060   Your proxies ``
+00000c80: 6068 6c74 7620 3d20 486c 7476 2870 726f  `hltv = Hltv(pro
+00000c90: 7879 5f70 726f 746f 636f 6c3d 2768 7474  xy_protocol='htt
+00000ca0: 7027 202e 2e2e 2920 2d3e 2027 3131 2e31  p' ...) -> '11.1
+00000cb0: 312e 3131 2e31 313a 3131 3131 2720 2d3e  1.11.11:1111' ->
+00000cc0: 2027 6874 7470 3a2f 2f31 312e 3131 2e31   'http://11.11.1
+00000cd0: 312e 3131 3a31 3131 3127 0a0a 2a20 6465  1.11:1111'..* de
+00000ce0: 6c65 7465 5f70 726f 7879 3a20 626f 6f6c  lete_proxy: bool
+00000cf0: 203d 2046 616c 7365 0a0a 2020 2020 5265   = False..    Re
+00000d00: 6d6f 7665 7320 7072 6f78 7920 6672 6f6d  moves proxy from
+00000d10: 206c 6973 7420 2870 726f 7879 5f70 6174   list (proxy_pat
+00000d20: 6820 696e 636c 7564 6564 2920 6966 2063  h included) if c
+00000d30: 6f6e 6e65 6374 696f 6e20 756e 7375 6363  onnection unsucc
+00000d40: 6573 7366 756c 6c79 0a0a 2a20 7469 6d65  essfully..* time
+00000d50: 6f75 743a 2069 6e74 203d 2035 0a0a 2020  out: int = 5..  
+00000d60: 2020 4d61 7820 7469 6d65 2074 6f20 636c    Max time to cl
+00000d70: 6f73 6520 636f 6e6e 6563 7469 6f6e 2e20  ose connection. 
+00000d80: 5265 636f 6d6d 656e 6465 6420 746f 2075  Recommended to u
+00000d90: 7365 2074 696d 656f 7574 3d31 2069 6620  se timeout=1 if 
+00000da0: 796f 7520 6172 6520 7573 696e 6720 7261  you are using ra
+00000db0: 6e64 6f6d 2070 726f 7869 6573 2e0a 0a2a  ndom proxies...*
+00000dc0: 2064 6562 7567 3a20 626f 6f6c 203d 2046   debug: bool = F
+00000dd0: 616c 7365 0a0a 2a20 747a 3a20 7374 7220  alse..* tz: str 
+00000de0: 3d20 2745 7572 6f70 652f 436f 7065 6e68  = 'Europe/Copenh
+00000df0: 6167 656e 273a 0a20 2020 200a 2020 2020  agen':.    .    
+00000e00: 5469 6d65 7a6f 6e65 2063 6f6e 6669 672e  Timezone config.
+00000e10: 200a 200a 2020 2020 3c61 2068 7265 663d   . .    <a href=
+00000e20: 2768 7474 7073 3a2f 2f67 6973 742e 6769  'https://gist.gi
+00000e30: 7468 7562 2e63 6f6d 2f68 6579 616c 6578  thub.com/heyalex
+00000e40: 656a 2f38 6266 3638 3866 6436 3764 3731  ej/8bf688fd67d71
+00000e50: 3939 6265 3461 3136 3832 6233 6565 6337  99be4a1682b3eec7
+00000e60: 3536 3827 3e54 6170 2068 6572 6520 3c2f  568'>Tap here </
+00000e70: 613e 2074 6f20 7365 6520 616c 6c20 6176  a> to see all av
+00000e80: 6169 6c61 626c 6520 7469 6d65 7a6f 6e65  ailable timezone
+00000e90: 730a 0a2a 2073 6166 655f 6d6f 6465 3a20  s..* safe_mode: 
+00000ea0: 626f 6f6c 203d 2054 7275 650a 0a20 2020  bool = True..   
+00000eb0: 2044 6973 616c 6c6f 7720 746f 2077 7261   Disallow to wra
+00000ec0: 7020 7265 7374 7269 6374 6564 2064 6174  p restricted dat
+00000ed0: 612e 2053 7769 7463 6820 746f 2046 616c  a. Switch to Fal
+00000ee0: 7365 206f 6e6c 7920 6174 2079 6f75 7220  se only at your 
+00000ef0: 6f77 6e20 7269 736b 2e0a 0a0a 2d2d 2d0a  own risk....---.
+00000f00: 0a23 2050 726f 7879 2055 7361 6765 0a0a  .# Proxy Usage..
+00000f10: 2a2a 4c6f 6164 2050 726f 7869 6573 2066  **Load Proxies f
+00000f20: 726f 6d20 6c69 7374 2a2a 0a20 2020 200a  rom list**.    .
+00000f30: 2020 2020 6060 600a 2020 2020 7072 6f78      ```.    prox
+00000f40: 795f 6c69 7374 203d 205b 2768 7474 703a  y_list = ['http:
+00000f50: 2f2f 3132 302e 3233 342e 3230 332e 3137  //120.234.203.17
+00000f60: 313a 3930 3032 272c 2027 6874 7470 3a2f  1:9002', 'http:/
+00000f70: 2f31 3130 2e33 382e 3638 2e33 383a 3830  /110.38.68.38:80
+00000f80: 275d 0a20 2020 200a 2020 2020 686c 7476  '].    .    hltv
+00000f90: 203d 2048 6c74 7628 7072 6f78 795f 6c69   = Hltv(proxy_li
+00000fa0: 7374 3d70 726f 7879 5f6c 6973 7429 0a0a  st=proxy_list)..
+00000fb0: 2020 2020 6060 600a 0a2a 2a4c 6f61 6420      ```..**Load 
+00000fc0: 5072 6f78 6965 7320 6672 6f6d 2066 696c  Proxies from fil
+00000fd0: 652a 2a0a 0a20 2020 2060 6060 0a20 2020  e**..    ```.   
+00000fe0: 2068 6c74 7620 3d20 486c 7476 2870 726f   hltv = Hltv(pro
+00000ff0: 7879 5f70 6174 683d 2750 4154 485f 544f  xy_path='PATH_TO
+00001000: 5f50 524f 5859 2e54 5854 2729 0a20 2020  _PROXY.TXT').   
+00001010: 2060 6060 0a0a 0a2a 2a44 656c 6574 6520   ```...**Delete 
+00001020: 7072 6f78 792a 2a0a 0a20 2020 2052 656d  proxy**..    Rem
+00001030: 6f76 6573 2062 6164 2070 726f 7869 6573  oves bad proxies
+00001040: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
+00001050: 2020 686c 7476 203d 2048 6c74 7628 7072    hltv = Hltv(pr
+00001060: 6f78 795f 7061 7468 3d27 5041 5448 5f54  oxy_path='PATH_T
+00001070: 4f5f 5052 4f58 592e 5458 5427 2c20 6465  O_PROXY.TXT', de
+00001080: 6c65 7465 5f70 726f 7879 3d54 7275 6529  lete_proxy=True)
+00001090: 0a20 2020 2060 6060 0a0a 2a2a 5072 6f74  .    ```..**Prot
+000010a0: 6f63 6f6c 2075 7361 6765 2a2a 0a0a 2020  ocol usage**..  
+000010b0: 2020 6060 600a 2020 2020 7072 6f78 795f    ```.    proxy_
+000010c0: 6c69 7374 203d 205b 2731 3230 2e32 3334  list = ['120.234
+000010d0: 2e32 3033 2e31 3731 3a39 3030 3227 2c20  .203.171:9002', 
+000010e0: 2731 3130 2e33 382e 3638 2e33 383a 3830  '110.38.68.38:80
+000010f0: 275d 0a20 2020 200a 2020 2020 686c 7476  '].    .    hltv
+00001100: 203d 2048 6c74 7628 7072 6f78 795f 6c69   = Hltv(proxy_li
+00001110: 7374 3d70 726f 7879 5f6c 6973 742c 2070  st=proxy_list, p
+00001120: 726f 7879 5f70 726f 746f 636f 6c3d 2768  roxy_protocol='h
+00001130: 7474 7027 290a 2020 2020 6060 600a 0a2d  ttp').    ```..-
+00001140: 2d2d 0a0a 2320 4d65 7468 6f64 730a 0a2a  --..# Methods..*
+00001150: 202a 2a67 6574 5f6d 6174 6368 6573 2864   **get_matches(d
+00001160: 6179 733a 2069 6e74 203d 2031 2c20 6d69  ays: int = 1, mi
+00001170: 6e5f 7374 6172 5f72 6174 696e 673a 2069  n_star_rating: i
+00001180: 6e74 203d 2031 2c20 6c69 7665 3a20 626f  nt = 1, live: bo
+00001190: 6f6c 203d 2054 7275 652c 2066 7574 7572  ol = True, futur
+000011a0: 653a 2062 6f6f 6c20 3d20 5472 7565 292a  e: bool = True)*
+000011b0: 2a0a 0a20 2020 202d 6461 7973 2028 7468  *..    -days (th
+000011c0: 6520 6e75 6d62 6572 206f 6620 6461 7973  e number of days
+000011d0: 2069 6e74 6f20 7468 6520 6675 7475 7265   into the future
+000011e0: 2074 6f20 6665 7463 6820 6d61 7463 6865   to fetch matche
+000011f0: 7320 666f 7229 0a20 200a 2020 2020 2d6d  s for).  .    -m
+00001200: 696e 5f73 7461 725f 7261 7469 6e67 2028  in_star_rating (
+00001210: 7468 6520 6d69 6e69 6d75 6d20 7374 6172  the minimum star
+00001220: 2072 6174 696e 6720 666f 7220 6d61 7463   rating for matc
+00001230: 6865 7320 746f 2069 6e63 6c75 6465 290a  hes to include).
+00001240: 2020 0a20 2020 2060 6060 0a20 2020 2061    .    ```.    a
+00001250: 7761 6974 2068 6c74 762e 6765 745f 6d61  wait hltv.get_ma
+00001260: 7463 6865 7328 6461 7973 3d31 290a 2020  tches(days=1).  
+00001270: 2020 0a20 2020 203e 3e3e 205b 7b27 6964    .    >>> [{'id
+00001280: 273a 2027 3233 3731 3230 3127 2c20 2764  ': '2371201', 'd
+00001290: 6174 6527 3a20 274c 4956 4527 2c20 2774  ate': 'LIVE', 't
+000012a0: 696d 6527 3a20 274c 4956 4527 2c20 2774  ime': 'LIVE', 't
+000012b0: 6561 6d31 273a 2027 496d 7065 7269 616c  eam1': 'Imperial
+000012c0: 272c 2027 7465 616d 3227 3a20 274d 4942  ', 'team2': 'MIB
+000012d0: 5227 2c20 2774 315f 6964 273a 2027 3934  R', 't1_id': '94
+000012e0: 3535 272c 2027 7432 5f69 6427 3a20 2739  55', 't2_id': '9
+000012f0: 3231 3527 2c20 276d 6170 7327 3a20 2733  215', 'maps': '3
+00001300: 272c 2027 7261 7469 6e67 273a 2031 2c20  ', 'rating': 1, 
+00001310: 2765 7665 6e74 273a 2027 5245 5320 5265  'event': 'RES Re
+00001320: 6769 6f6e 616c 2053 6572 6965 7320 3320  gional Series 3 
+00001330: 4c41 5441 4d27 7d2c 207b 2769 6427 3a20  LATAM'}, {'id': 
+00001340: 2732 3337 3039 3634 272c 2027 6461 7465  '2370964', 'date
+00001350: 273a 2027 3230 3234 2d30 342d 3136 272c  ': '2024-04-16',
+00001360: 2027 7469 6d65 273a 2027 3132 3a33 3027   'time': '12:30'
+00001370: 2c20 2774 6561 6d31 273a 2027 5341 5727  , 'team1': 'SAW'
+00001380: 2c20 2774 6561 6d32 273a 2027 5361 6d70  , 'team2': 'Samp
+00001390: 6927 2c20 2774 315f 6964 273a 2027 3130  i', 't1_id': '10
+000013a0: 3536 3727 2c20 2774 325f 6964 273a 2027  567', 't2_id': '
+000013b0: 3130 3639 3527 2c20 276d 6170 7327 3a20  10695', 'maps': 
+000013c0: 2733 272c 2027 7261 7469 6e67 273a 2031  '3', 'rating': 1
+000013d0: 2c20 2765 7665 6e74 273a 2027 5468 756e  , 'event': 'Thun
+000013e0: 6465 7270 6963 6b20 576f 726c 6420 4368  derpick World Ch
+000013f0: 616d 7069 6f6e 7368 6970 2032 3032 3420  ampionship 2024 
+00001400: 4555 2043 6c6f 7365 6420 5175 616c 6966  EU Closed Qualif
+00001410: 6965 7220 3127 7d2c 207b 2769 6427 3a20  ier 1'}, {'id': 
+00001420: 2732 3337 3133 3637 272c 2027 6461 7465  '2371367', 'date
+00001430: 273a 2027 3230 3234 2d30 342d 3136 272c  ': '2024-04-16',
+00001440: 2027 7469 6d65 273a 2027 3134 3a30 3027   'time': '14:00'
+00001450: 2c20 2774 6561 6d31 273a 2027 4761 696d  , 'team1': 'Gaim
+00001460: 696e 2047 6c61 6469 6174 6f72 7327 2c20  in Gladiators', 
+00001470: 2774 6561 6d32 273a 2027 5065 726d 6974  'team2': 'Permit
+00001480: 7461 272c 2027 7431 5f69 6427 3a20 2731  ta', 't1_id': '1
+00001490: 3135 3731 272c 2027 7432 5f69 6427 3a20  1571', 't2_id': 
+000014a0: 2731 3230 3039 272c 2027 6d61 7073 273a  '12009', 'maps':
+000014b0: 2027 3327 2c20 2772 6174 696e 6727 3a20   '3', 'rating': 
+000014c0: 312c 2027 6576 656e 7427 3a20 2745 6c69  1, 'event': 'Eli
+000014d0: 7361 2049 6e76 6974 6174 696f 6e61 6c20  sa Invitational 
+000014e0: 5370 7269 6e67 2032 3032 3427 7d5d 0a20  Spring 2024'}]. 
+000014f0: 2020 200a 2020 2020 6060 600a 0a2a 202a     .    ```..* *
+00001500: 2a67 6574 5f6d 6174 6368 5f69 6e66 6f28  *get_match_info(
+00001510: 6d61 7463 685f 6964 3a20 696e 7420 7c20  match_id: int | 
+00001520: 7374 722c 2074 6561 6d31 2c20 7465 616d  str, team1, team
+00001530: 322c 2065 7665 6e74 5f74 6974 6c65 2c20  2, event_title, 
+00001540: 7374 6174 733a 2062 6f6f 6c20 3d20 5472  stats: bool = Tr
+00001550: 7565 2c20 7072 6564 6963 7473 3a20 626f  ue, predicts: bo
+00001560: 6f6c 203d 2054 7275 6529 2a2a 0a20 200a  ol = True)**.  .
+00001570: 2020 2020 6060 600a 2020 2020 6177 6169      ```.    awai
+00001580: 7420 686c 7476 2e67 6574 5f6d 6174 6368  t hltv.get_match
+00001590: 5f69 6e66 6f28 3233 3730 3933 312c 2027  _info(2370931, '
+000015a0: 4d6f 757a 272c 2027 6661 7a65 272c 2027  Mouz', 'faze', '
+000015b0: 6965 6d2d 6368 656e 6764 752d 3230 3234  iem-chengdu-2024
+000015c0: 2729 2020 0a20 200a 2020 2020 3e3e 3e28  ')  .  .    >>>(
+000015d0: 3233 3730 3933 312c 2027 3027 2c20 2732  2370931, '0', '2
+000015e0: 272c 2027 4d61 7463 6820 6f76 6572 272c  ', 'Match over',
+000015f0: 205b 7b27 6d61 706e 616d 6527 3a20 274f   [{'mapname': 'O
+00001600: 7665 7270 6173 7327 2c20 2772 5f74 6561  verpass', 'r_tea
+00001610: 6d31 273a 2027 3130 272c 2027 725f 7465  m1': '10', 'r_te
+00001620: 616d 3227 3a20 2731 3327 7d2c 207b 276d  am2': '13'}, {'m
+00001630: 6170 6e61 6d65 273a 2027 4e75 6b65 272c  apname': 'Nuke',
+00001640: 2027 725f 7465 616d 3127 3a20 2736 272c   'r_team1': '6',
+00001650: 2027 725f 7465 616d 3227 3a20 2731 3327   'r_team2': '13'
+00001660: 7d2c 207b 276d 6170 6e61 6d65 273a 2027  }, {'mapname': '
+00001670: 4d69 7261 6765 272c 2027 725f 7465 616d  Mirage', 'r_team
+00001680: 3127 3a20 272d 272c 2027 725f 7465 616d  1': '-', 'r_team
+00001690: 3227 3a20 272d 277d 5d2c 205b 7b27 6964  2': '-'}], [{'id
+000016a0: 273a 2027 3138 3835 3027 2c20 276e 6963  ': '18850', 'nic
+000016b0: 6b6e 616d 6527 3a20 274a 696d 7070 6861  kname': 'Jimppha
+000016c0: 7427 2c20 276b 6427 3a20 2733 332d 3239  t', 'kd': '33-29
+000016d0: 272c 2027 6164 7227 3a20 2738 302e 3927  ', 'adr': '80.9'
+000016e0: 2c20 2772 6174 696e 6727 3a20 2731 2e30  , 'rating': '1.0
+000016f0: 3827 7d2c 200a 2020 0a20 2020 207b 2769  8'}, .  .    {'i
+00001700: 6427 3a20 2731 3830 3732 272c 2027 6e69  d': '18072', 'ni
+00001710: 636b 6e61 6d65 273a 2027 746f 727a 7369  ckname': 'torzsi
+00001720: 272c 2027 6b64 273a 2027 3236 2d32 3527  ', 'kd': '26-25'
+00001730: 2c20 2761 6472 273a 2027 3730 2e35 272c  , 'adr': '70.5',
+00001740: 2027 7261 7469 6e67 273a 2027 312e 3032   'rating': '1.02
+00001750: 277d 2c20 7b27 6964 273a 2027 3133 3636  '}, {'id': '1366
+00001760: 3627 2c20 276e 6963 6b6e 616d 6527 3a20  6', 'nickname': 
+00001770: 2742 726f 6c6c 616e 272c 2027 6b64 273a  'Brollan', 'kd':
+00001780: 2027 3235 2d33 3127 2c20 2761 6472 273a   '25-31', 'adr':
+00001790: 2027 3638 2e34 272c 2027 7261 7469 6e67   '68.4', 'rating
+000017a0: 273a 2027 302e 3930 277d 2c20 7b27 6964  ': '0.90'}, {'id
+000017b0: 273a 2027 3230 3331 3227 2c20 276e 6963  ': '20312', 'nic
+000017c0: 6b6e 616d 6527 3a20 2778 6572 7469 6f4e  kname': 'xertioN
+000017d0: 272c 2027 6b64 273a 2027 3233 2d33 3127  ', 'kd': '23-31'
+000017e0: 2c20 2761 6472 273a 2027 3632 2e34 272c  , 'adr': '62.4',
+000017f0: 2027 7261 7469 6e67 273a 2027 302e 3832   'rating': '0.82
+00001800: 277d 2c20 7b27 6964 273a 2027 3136 3832  '}, {'id': '1682
+00001810: 3027 2c20 276e 6963 6b6e 616d 6527 3a20  0', 'nickname': 
+00001820: 2773 6975 6879 272c 2027 6b64 273a 2027  'siuhy', 'kd': '
+00001830: 3137 2d33 3027 2c20 2761 6472 273a 2027  17-30', 'adr': '
+00001840: 3531 2e36 272c 2027 7261 7469 6e67 273a  51.6', 'rating':
+00001850: 2027 302e 3730 277d 2c20 7b27 6964 273a   '0.70'}, {'id':
+00001860: 2027 3138 3035 3327 2c20 276e 6963 6b6e   '18053', 'nickn
+00001870: 616d 6527 3a20 2762 726f 6b79 272c 2027  ame': 'broky', '
+00001880: 6b64 273a 2027 3334 2d32 3227 2c20 2761  kd': '34-22', 'a
+00001890: 6472 273a 2027 3739 2e33 272c 2027 7261  dr': '79.3', 'ra
+000018a0: 7469 6e67 273a 2027 312e 3333 277d 2c20  ting': '1.33'}, 
+000018b0: 7b27 6964 273a 2027 3939 3630 272c 2027  {'id': '9960', '
+000018c0: 6e69 636b 6e61 6d65 273a 2027 6672 6f7a  nickname': 'froz
+000018d0: 656e 272c 2027 6b64 273a 2027 3333 2d32  en', 'kd': '33-2
+000018e0: 3327 2c20 2761 6472 273a 2027 3835 2e35  3', 'adr': '85.5
+000018f0: 272c 2027 7261 7469 6e67 273a 2027 312e  ', 'rating': '1.
+00001900: 3331 277d 2c20 7b27 6964 273a 2027 3131  31'}, {'id': '11
+00001910: 3831 3627 2c20 276e 6963 6b6e 616d 6527  816', 'nickname'
+00001920: 3a20 2772 6f70 7a27 2c20 276b 6427 3a20  : 'ropz', 'kd': 
+00001930: 2733 312d 3236 272c 2027 6164 7227 3a20  '31-26', 'adr': 
+00001940: 2737 332e 3027 2c20 2772 6174 696e 6727  '73.0', 'rating'
+00001950: 3a20 2731 2e32 3027 7d2c 207b 2769 6427  : '1.20'}, {'id'
+00001960: 3a20 2738 3138 3327 2c20 276e 6963 6b6e  : '8183', 'nickn
+00001970: 616d 6527 3a20 2772 6169 6e27 2c20 276b  ame': 'rain', 'k
+00001980: 6427 3a20 2732 372d 3236 272c 2027 6164  d': '27-26', 'ad
+00001990: 7227 3a20 2738 322e 3027 2c20 2772 6174  r': '82.0', 'rat
+000019a0: 696e 6727 3a20 2731 2e31 3827 7d2c 207b  ing': '1.18'}, {
+000019b0: 2769 6427 3a20 2734 3239 272c 2027 6e69  'id': '429', 'ni
+000019c0: 636b 6e61 6d65 273a 2027 6b61 7272 6967  ckname': 'karrig
+000019d0: 616e 272c 2027 6b64 273a 2027 3230 2d32  an', 'kd': '20-2
+000019e0: 3827 2c20 2761 6472 273a 2027 3439 2e37  8', 'adr': '49.7
+000019f0: 272c 2027 7261 7469 6e67 273a 2027 302e  ', 'rating': '0.
+00001a00: 3831 277d 5d29 2020 0a20 2020 200a 2020  81'}])  .    .  
+00001a10: 2020 6060 600a 2020 0a2a 202a 2a67 6574    ```.  .* **get
+00001a20: 5f72 6573 756c 7473 2864 6179 733a 2069  _results(days: i
+00001a30: 6e74 203d 2031 2c20 6d69 6e5f 7261 7469  nt = 1, min_rati
+00001a40: 6e67 3a20 696e 7420 3d20 312c 206d 6178  ng: int = 1, max
+00001a50: 3a20 696e 7420 3d20 3330 2c20 6665 6174  : int = 30, feat
+00001a60: 7572 6564 3a20 626f 6f6c 203d 2054 7275  ured: bool = Tru
+00001a70: 652c 2072 6567 756c 6172 3a20 626f 6f6c  e, regular: bool
+00001a80: 203d 2054 7275 6529 2920 2d3e 2a2a 0a20   = True)) ->**. 
+00001a90: 2020 200a 2020 2020 6060 600a 2020 2020     .    ```.    
+00001aa0: 7072 696e 7428 6177 6169 7420 686c 7476  print(await hltv
+00001ab0: 2e67 6574 5f72 6573 756c 7473 2829 290a  .get_results()).
+00001ac0: 2020 0a20 2020 205b 7b27 6964 273a 2027    .    [{'id': '
+00001ad0: 3233 3730 3933 3127 2c20 2774 6561 6d31  2370931', 'team1
+00001ae0: 273a 2027 4d4f 555a 272c 2027 7465 616d  ': 'MOUZ', 'team
+00001af0: 3227 3a20 2746 615a 6527 2c20 2773 636f  2': 'FaZe', 'sco
+00001b00: 7265 3127 3a20 2730 272c 2027 7363 6f72  re1': '0', 'scor
+00001b10: 6532 273a 2027 3227 2c20 2772 6174 696e  e2': '2', 'ratin
+00001b20: 6727 3a20 302c 2027 6576 656e 7427 3a20  g': 0, 'event': 
+00001b30: 2749 454d 2043 6865 6e67 6475 2032 3032  'IEM Chengdu 202
+00001b40: 3427 7d5d 0a20 2020 2060 6060 0a20 200a  4'}].    ```.  .
+00001b50: 2a20 2a2a 6765 745f 6576 656e 7473 286f  * **get_events(o
+00001b60: 7574 676f 696e 673d 5472 7565 2c20 6675  utgoing=True, fu
+00001b70: 7475 7265 3d54 7275 652c 206d 6178 5f65  ture=True, max_e
+00001b80: 7665 6e74 733d 3130 2920 2d3e 205b 2827  vents=10) -> [('
+00001b90: 6964 272c 2027 7469 746c 6527 2c20 2773  id', 'title', 's
+00001ba0: 7461 7274 6461 7465 272c 2027 656e 6464  tartdate', 'endd
+00001bb0: 6174 6527 295d 2a2a 0a0a 2020 2020 6060  ate')]**..    ``
+00001bc0: 600a 2020 2020 6177 6169 7420 686c 7476  `.    await hltv
+00001bd0: 2e67 6574 5f65 7665 6e74 7328 6675 7475  .get_events(futu
+00001be0: 7265 3d46 616c 7365 290a 2020 2020 0a20  re=False).    . 
+00001bf0: 2020 203e 3e3e 5b7b 2769 6427 3a20 2737     >>>[{'id': '7
+00001c00: 3734 3927 2c20 2774 6974 6c65 273a 2027  749', 'title': '
+00001c10: 5468 756e 6465 7270 6963 6b20 576f 726c  Thunderpick Worl
+00001c20: 6420 4368 616d 7069 6f6e 7368 6970 2032  d Championship 2
+00001c30: 3032 3420 4555 2043 6c6f 7365 6420 5175  024 EU Closed Qu
+00001c40: 616c 6966 6965 7220 3127 2c20 2773 7461  alifier 1', 'sta
+00001c50: 7274 5f64 6174 6527 3a20 2731 2d34 272c  rt_date': '1-4',
+00001c60: 2027 656e 645f 6461 7465 273a 2027 3232   'end_date': '22
+00001c70: 2d34 277d 2c20 7b27 6964 273a 2027 3736  -4'}, {'id': '76
+00001c80: 3231 272c 2027 7469 746c 6527 3a20 2745  21', 'title': 'E
+00001c90: 534c 2043 6861 6c6c 656e 6765 7220 4c65  SL Challenger Le
+00001ca0: 6167 7565 2053 6561 736f 6e20 3437 204e  ague Season 47 N
+00001cb0: 6f72 7468 2041 6d65 7269 6361 272c 2027  orth America', '
+00001cc0: 7374 6172 745f 6461 7465 273a 2027 3133  start_date': '13
+00001cd0: 2d32 272c 2027 656e 645f 6461 7465 273a  -2', 'end_date':
+00001ce0: 2027 3136 2d36 277d 5d0a 2020 2020 2020   '16-6'}].      
+00001cf0: 0a20 2020 2060 6060 0a0a 2a20 2a2a 6765  .    ```..* **ge
+00001d00: 745f 6576 656e 745f 7265 7375 6c74 7328  t_event_results(
+00001d10: 6576 656e 745f 6964 3a20 696e 7420 7c20  event_id: int | 
+00001d20: 7374 722c 2064 6179 733a 2069 6e74 203d  str, days: int =
+00001d30: 2031 2c20 6d61 785f 3a20 696e 7420 3d20   1, max_: int = 
+00001d40: 3130 292a 2a0a 0a20 200a 2020 2020 6060  10)**..  .    ``
+00001d50: 600a 2020 2020 6177 6169 7420 6765 745f  `.    await get_
+00001d60: 6576 656e 745f 7265 7375 6c74 7328 3731  event_results(71
+00001d70: 3438 290a 2020 2020 0a20 2020 203e 3e3e  48).    .    >>>
+00001d80: 5b7b 2769 6427 3a20 2732 3337 3039 3331  [{'id': '2370931
+00001d90: 272c 2027 6461 7465 273a 2027 3134 2d30  ', 'date': '14-0
+00001da0: 342d 3230 3234 272c 2027 7465 616d 3127  4-2024', 'team1'
+00001db0: 3a20 274d 4f55 5a27 2c20 2774 6561 6d32  : 'MOUZ', 'team2
+00001dc0: 273a 2027 4661 5a65 272c 2027 7363 6f72  ': 'FaZe', 'scor
+00001dd0: 6531 273a 2027 3027 2c20 2773 636f 7265  e1': '0', 'score
+00001de0: 3227 3a20 2732 277d 5d0a 0a20 2020 2060  2': '2'}]..    `
+00001df0: 6060 0a0a 2a20 2a2a 6765 745f 6576 656e  ``..* **get_even
+00001e00: 745f 6d61 7463 6865 7328 6576 656e 745f  t_matches(event_
+00001e10: 6964 3a20 7374 7220 7c20 696e 742c 2064  id: str | int, d
+00001e20: 6179 733a 2069 6e74 203d 2031 293a 2a2a  ays: int = 1):**
+00001e30: 0a20 200a 2020 2020 6060 600a 2020 2020  .  .    ```.    
+00001e40: 6177 6169 7420 686c 7476 2e67 6574 5f65  await hltv.get_e
+00001e50: 7665 6e74 5f6d 6174 6368 6573 2837 3134  vent_matches(714
+00001e60: 3829 0a20 2020 200a 2020 2020 3e3e 3e5b  8).    .    >>>[
+00001e70: 7b27 6964 273a 2027 3233 3730 3737 3127  {'id': '2370771'
+00001e80: 2c20 2764 6174 6527 3a20 2732 3032 342d  , 'date': '2024-
+00001e90: 3034 2d31 3827 2c20 2774 696d 6527 3a20  04-18', 'time': 
+00001ea0: 2731 353a 3330 272c 2027 7465 616d 3127  '15:30', 'team1'
+00001eb0: 3a20 274d 6f6e 7465 272c 2027 7465 616d  : 'Monte', 'team
+00001ec0: 3227 3a20 2770 6169 4e27 2c20 2774 315f  2': 'paiN', 't1_
+00001ed0: 6964 273a 2027 3131 3831 3127 2c20 2774  id': '11811', 't
+00001ee0: 325f 6964 273a 2027 3437 3733 277d 2c20  2_id': '4773'}, 
+00001ef0: 7b27 6964 273a 2027 3233 3730 3737 3227  {'id': '2370772'
+00001f00: 2c20 2764 6174 6527 3a20 2732 3032 342d  , 'date': '2024-
+00001f10: 3034 2d31 3827 2c20 2774 696d 6527 3a20  04-18', 'time': 
+00001f20: 2731 373a 3030 272c 2027 7465 616d 3127  '17:00', 'team1'
+00001f30: 3a20 2749 6d70 6572 6961 6c27 2c20 2774  : 'Imperial', 't
+00001f40: 6561 6d32 273a 2027 4d65 7469 7a70 6f72  eam2': 'Metizpor
+00001f50: 7427 2c20 2774 315f 6964 273a 2027 3934  t', 't1_id': '94
+00001f60: 3535 272c 2027 7432 5f69 6427 3a20 2731  55', 't2_id': '1
+00001f70: 3136 3431 277d 2c20 7b27 6964 273a 2027  1641'}, {'id': '
+00001f80: 3233 3730 3737 3327 2c20 2764 6174 6527  2370773', 'date'
+00001f90: 3a20 2732 3032 342d 3034 2d31 3827 2c20  : '2024-04-18', 
+00001fa0: 2774 696d 6527 3a20 2731 383a 3330 272c  'time': '18:30',
+00001fb0: 2027 7465 616d 3127 3a20 2746 5552 4941   'team1': 'FURIA
+00001fc0: 272c 2027 7465 616d 3227 3a20 2739 7a27  ', 'team2': '9z'
+00001fd0: 2c20 2774 315f 6964 273a 2027 3832 3937  , 't1_id': '8297
+00001fe0: 272c 2027 7432 5f69 6427 3a20 2739 3939  ', 't2_id': '999
+00001ff0: 3627 7d2c 207b 2769 6427 3a20 2732 3337  6'}, {'id': '237
+00002000: 3037 3734 272c 2027 6461 7465 273a 2027  0774', 'date': '
+00002010: 3230 3234 2d30 342d 3138 272c 2027 7469  2024-04-18', 'ti
+00002020: 6d65 273a 2027 3230 3a30 3027 2c20 2774  me': '20:00', 't
+00002030: 6561 6d31 273a 2027 4d49 4252 272c 2027  eam1': 'MIBR', '
+00002040: 7465 616d 3227 3a20 274f 4727 2c20 2774  team2': 'OG', 't
+00002050: 315f 6964 273a 2027 3932 3135 272c 2027  1_id': '9215', '
+00002060: 7432 5f69 6427 3a20 2731 3035 3033 277d  t2_id': '10503'}
+00002070: 2c20 7b27 6964 273a 2027 3233 3730 3737  , {'id': '237077
+00002080: 3527 2c20 2764 6174 6527 3a20 2732 3032  5', 'date': '202
+00002090: 342d 3034 2d31 3827 2c20 2774 696d 6527  4-04-18', 'time'
+000020a0: 3a20 2732 313a 3330 272c 2027 7465 616d  : '21:30', 'team
+000020b0: 3127 3a20 2754 4244 272c 2027 7465 616d  1': 'TBD', 'team
+000020c0: 3227 3a20 2754 4244 272c 2027 7431 5f69  2': 'TBD', 't1_i
+000020d0: 6427 3a20 302c 2027 7432 5f69 6427 3a20  d': 0, 't2_id': 
+000020e0: 307d 2c20 7b27 6964 273a 2027 3233 3730  0}, {'id': '2370
+000020f0: 3737 3627 2c20 2764 6174 6527 3a20 2732  776', 'date': '2
+00002100: 3032 342d 3034 2d31 3827 2c20 2774 696d  024-04-18', 'tim
+00002110: 6527 3a20 2732 333a 3030 272c 2027 7465  e': '23:00', 'te
+00002120: 616d 3127 3a20 2754 4244 272c 2027 7465  am1': 'TBD', 'te
+00002130: 616d 3227 3a20 2754 4244 272c 2027 7431  am2': 'TBD', 't1
+00002140: 5f69 6427 3a20 302c 2027 7432 5f69 6427  _id': 0, 't2_id'
+00002150: 3a20 307d 2c20 7b27 6964 273a 2027 3233  : 0}, {'id': '23
+00002160: 3730 3737 3727 2c20 2764 6174 6527 3a20  70777', 'date': 
+00002170: 2732 3032 342d 3034 2d31 3927 2c20 2774  '2024-04-19', 't
+00002180: 696d 6527 3a20 2730 303a 3030 272c 2027  ime': '00:00', '
+00002190: 7465 616d 3127 3a20 2754 4244 272c 2027  team1': 'TBD', '
+000021a0: 7465 616d 3227 3a20 2754 4244 272c 2027  team2': 'TBD', '
+000021b0: 7431 5f69 6427 3a20 302c 2027 7432 5f69  t1_id': 0, 't2_i
+000021c0: 6427 3a20 307d 2c20 7b27 6964 273a 2027  d': 0}, {'id': '
+000021d0: 3233 3730 3737 3827 2c20 2764 6174 6527  2370778', 'date'
+000021e0: 3a20 2732 3032 342d 3034 2d31 3927 2c20  : '2024-04-19', 
+000021f0: 2774 696d 6527 3a20 2731 353a 3030 272c  'time': '15:00',
+00002200: 2027 7465 616d 3127 3a20 2754 4244 272c   'team1': 'TBD',
+00002210: 2027 7465 616d 3227 3a20 2754 4244 272c   'team2': 'TBD',
+00002220: 2027 7431 5f69 6427 3a20 302c 2027 7432   't1_id': 0, 't2
+00002230: 5f69 6427 3a20 307d 2c20 7b27 6964 273a  _id': 0}, {'id':
+00002240: 2027 3233 3730 3737 3927 2c20 2764 6174   '2370779', 'dat
+00002250: 6527 3a20 2732 3032 342d 3034 2d31 3927  e': '2024-04-19'
+00002260: 2c20 2774 696d 6527 3a20 2731 373a 3330  , 'time': '17:30
+00002270: 272c 2027 7465 616d 3127 3a20 2754 4244  ', 'team1': 'TBD
+00002280: 272c 2027 7465 616d 3227 3a20 2754 4244  ', 'team2': 'TBD
+00002290: 272c 2027 7431 5f69 6427 3a20 302c 2027  ', 't1_id': 0, '
+000022a0: 7432 5f69 6427 3a20 307d 2c20 7b27 6964  t2_id': 0}, {'id
+000022b0: 273a 2027 3233 3730 3738 3027 2c20 2764  ': '2370780', 'd
+000022c0: 6174 6527 3a20 2732 3032 342d 3034 2d31  ate': '2024-04-1
+000022d0: 3927 2c20 2774 696d 6527 3a20 2732 303a  9', 'time': '20:
+000022e0: 3030 272c 2027 7465 616d 3127 3a20 2754  00', 'team1': 'T
+000022f0: 4244 272c 2027 7465 616d 3227 3a20 2754  BD', 'team2': 'T
+00002300: 4244 272c 2027 7431 5f69 6427 3a20 302c  BD', 't1_id': 0,
+00002310: 2027 7432 5f69 6427 3a20 307d 2c20 7b27   't2_id': 0}, {'
+00002320: 6964 273a 2027 3233 3730 3738 3127 2c20  id': '2370781', 
+00002330: 2764 6174 6527 3a20 2732 3032 342d 3034  'date': '2024-04
+00002340: 2d31 3927 2c20 2774 696d 6527 3a20 2732  -19', 'time': '2
+00002350: 323a 3330 272c 2027 7465 616d 3127 3a20  2:30', 'team1': 
+00002360: 2754 4244 272c 2027 7465 616d 3227 3a20  'TBD', 'team2': 
+00002370: 2754 4244 272c 2027 7431 5f69 6427 3a20  'TBD', 't1_id': 
+00002380: 302c 2027 7432 5f69 6427 3a20 307d 2c20  0, 't2_id': 0}, 
+00002390: 7b27 6964 273a 2027 3233 3730 3738 3227  {'id': '2370782'
+000023a0: 2c20 2764 6174 6527 3a20 2732 3032 342d  , 'date': '2024-
+000023b0: 3034 2d32 3027 2c20 2774 696d 6527 3a20  04-20', 'time': 
+000023c0: 2730 303a 3330 272c 2027 7465 616d 3127  '00:30', 'team1'
+000023d0: 3a20 2754 4244 272c 2027 7465 616d 3227  : 'TBD', 'team2'
+000023e0: 3a20 2754 4244 272c 2027 7431 5f69 6427  : 'TBD', 't1_id'
+000023f0: 3a20 302c 2027 7432 5f69 6427 3a20 307d  : 0, 't2_id': 0}
+00002400: 2c20 7b27 6964 273a 2027 3233 3730 3738  , {'id': '237078
+00002410: 3327 2c20 2764 6174 6527 3a20 2732 3032  3', 'date': '202
+00002420: 342d 3034 2d32 3027 2c20 2774 696d 6527  4-04-20', 'time'
+00002430: 3a20 2731 353a 3030 272c 2027 7465 616d  : '15:00', 'team
+00002440: 3127 3a20 2754 4244 272c 2027 7465 616d  1': 'TBD', 'team
+00002450: 3227 3a20 2754 4244 272c 2027 7431 5f69  2': 'TBD', 't1_i
+00002460: 6427 3a20 302c 2027 7432 5f69 6427 3a20  d': 0, 't2_id': 
+00002470: 307d 2c20 7b27 6964 273a 2027 3233 3730  0}, {'id': '2370
+00002480: 3738 3427 2c20 2764 6174 6527 3a20 2732  784', 'date': '2
+00002490: 3032 342d 3034 2d32 3027 2c20 2774 696d  024-04-20', 'tim
+000024a0: 6527 3a20 2731 383a 3030 272c 2027 7465  e': '18:00', 'te
+000024b0: 616d 3127 3a20 2754 4244 272c 2027 7465  am1': 'TBD', 'te
+000024c0: 616d 3227 3a20 2754 4244 272c 2027 7431  am2': 'TBD', 't1
+000024d0: 5f69 6427 3a20 302c 2027 7432 5f69 6427  _id': 0, 't2_id'
+000024e0: 3a20 307d 5d0a 2020 0a20 2020 2060 6060  : 0}].  .    ```
+000024f0: 0a0a 2a20 2a2a 6765 745f 6576 656e 745f  ..* **get_event_
+00002500: 696e 666f 2865 7665 6e74 5f69 643a 2073  info(event_id: s
+00002510: 7472 207c 2069 6e74 2c20 6576 656e 745f  tr | int, event_
+00002520: 7469 746c 653a 2073 7472 2920 2d3e 2028  title: str) -> (
+00002530: 6576 656e 745f 6964 2c20 6576 656e 745f  event_id, event_
+00002540: 7469 746c 652c 2065 7665 6e74 5f73 7461  title, event_sta
+00002550: 7274 2c20 6576 656e 745f 656e 642c 2070  rt, event_end, p
+00002560: 7269 7a65 2c20 7465 616d 5f6e 756d 2c20  rize, team_num, 
+00002570: 6c6f 6361 7469 6f6e 2c20 6772 6f75 7073  location, groups
+00002580: 292a 2a0a 0a20 2020 2060 6060 0a20 2020  )**..    ```.   
+00002590: 2061 7761 6974 2068 6c74 762e 6765 745f   await hltv.get_
+000025a0: 6576 656e 745f 696e 666f 2837 3134 382c  event_info(7148,
+000025b0: 2027 5047 4c20 4353 3220 4d61 6a6f 7220   'PGL CS2 Major 
+000025c0: 436f 7065 6e68 6167 656e 3230 3234 2729  Copenhagen2024')
+000025d0: 0a20 2020 200a 2020 2020 7b27 6964 273a  .    .    {'id':
+000025e0: 2037 3134 382c 2027 7469 746c 6527 3a20   7148, 'title': 
+000025f0: 2750 474c 2043 5332 204d 616a 6f72 2043  'PGL CS2 Major C
+00002600: 6f70 656e 6861 6765 6e32 3032 3427 2c20  openhagen2024', 
+00002610: 2773 7461 7274 273a 2027 3231 2d33 272c  'start': '21-3',
+00002620: 2027 656e 6427 3a20 2733 312d 3327 2c20   'end': '31-3', 
+00002630: 2770 7269 7a65 273a 2027 2431 2c32 3530  'prize': '$1,250
+00002640: 2c30 3030 272c 2027 7465 616d 7327 3a20  ,000', 'teams': 
+00002650: 2731 3627 2c20 276c 6f63 6174 696f 6e27  '16', 'location'
+00002660: 3a20 2743 6f70 656e 6861 6765 6e2c 2044  : 'Copenhagen, D
+00002670: 656e 6d61 726b 272c 2027 6772 6f75 7027  enmark', 'group'
+00002680: 3a20 5b5d 7d0a 2020 200a 2020 2020 6060  : []}.   .    ``
+00002690: 600a 0a0a 2a20 2a2a 6765 745f 746f 705f  `...* **get_top_
+000026a0: 7465 616d 7328 6d61 785f 7465 616d 733d  teams(max_teams=
+000026b0: 3330 2920 2d3e 205b 2772 616e 6b27 2c20  30) -> ['rank', 
+000026c0: 2774 6974 6c65 272c 2027 706f 696e 7473  'title', 'points
+000026d0: 272c 2027 6368 616e 6765 272c 2027 6964  ', 'change', 'id
+000026e0: 275d 2a2a 0a0a 2020 2020 6060 600a 2020  ']**..    ```.  
+000026f0: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+00002700: 5f74 6f70 5f74 6561 6d73 2832 290a 2020  _top_teams(2).  
+00002710: 2020 0a20 2020 203e 3e3e 5b7b 2769 6427    .    >>>[{'id'
+00002720: 3a20 2731 3131 3127 2c20 2772 616e 6b27  : '1111', 'rank'
+00002730: 3a20 2731 272c 2027 7469 746c 6527 3a20  : '1', 'title': 
+00002740: 2746 615a 6527 2c20 2770 6f69 6e74 7327  'FaZe', 'points'
+00002750: 3a20 2739 3339 272c 2027 6368 616e 6765  : '939', 'change
+00002760: 273a 2027 2d27 2c20 2769 6427 3a20 2736  ': '-', 'id': '6
+00002770: 3636 3727 7d2c 207b 2769 6427 3a20 2731  667'}, {'id': '1
+00002780: 3131 3127 2c20 2772 616e 6b27 3a20 2732  111', 'rank': '2
+00002790: 272c 2027 7469 746c 6527 3a20 274e 6174  ', 'title': 'Nat
+000027a0: 7573 2056 696e 6365 7265 272c 2027 706f  us Vincere', 'po
+000027b0: 696e 7473 273a 2027 3735 3727 2c20 2763  ints': '757', 'c
+000027c0: 6861 6e67 6527 3a20 272b 3427 2c20 2769  hange': '+4', 'i
+000027d0: 6427 3a20 2734 3630 3827 7d5d 0a20 2020  d': '4608'}].   
+000027e0: 2060 6060 0a0a 2a20 2a2a 6765 745f 7465   ```..* **get_te
+000027f0: 616d 5f69 6e66 6f28 7465 616d 5f69 643a  am_info(team_id:
+00002800: 2069 6e74 207c 2073 7472 2c20 7469 746c   int | str, titl
+00002810: 653a 2073 7472 2920 2d3e 2028 7465 616d  e: str) -> (team
+00002820: 5f69 642c 2074 6561 6d5f 7469 746c 652c  _id, team_title,
+00002830: 2072 616e 6b2c 207b 706c 6179 6572 3a70   rank, {player:p
+00002840: 6c61 7965 725f 6964 7d2c 2063 6f61 6368  layer_id}, coach
+00002850: 2c20 6176 6572 6167 655f 6167 652c 2077  , average_age, w
+00002860: 6565 6b73 5f69 6e5f 746f 705f 3230 2c20  eeks_in_top_20, 
+00002870: 6c61 7374 5f74 726f 7068 792c 2074 6f74  last_trophy, tot
+00002880: 616c 5f74 726f 7068 7973 292a 2a0a 0a20  al_trophys)**.. 
+00002890: 2020 2060 6060 0a20 2020 2061 7761 6974     ```.    await
+000028a0: 2068 6c74 762e 6765 745f 7465 616d 5f69   hltv.get_team_i
+000028b0: 6e66 6f28 3636 3637 2c20 2766 617a 6527  nfo(6667, 'faze'
+000028c0: 290a 2020 2020 0a20 2020 203e 3e3e 2836  ).    .    >>>(6
+000028d0: 3636 372c 2027 6661 7a65 272c 2027 3127  667, 'faze', '1'
+000028e0: 2c20 5b27 6b61 7272 6967 616e 272c 2027  , ['karrigan', '
+000028f0: 7261 696e 272c 2027 6672 6f7a 656e 272c  rain', 'frozen',
+00002900: 2027 726f 707a 272c 2027 6272 6f6b 7927   'ropz', 'broky'
+00002910: 5d2c 2027 4e45 4f27 2c20 2732 362e 3627  ], 'NEO', '26.6'
+00002920: 2c20 2732 3538 272c 2027 4945 4d20 4368  , '258', 'IEM Ch
+00002930: 656e 6764 7520 3230 3234 272c 2032 3229  engdu 2024', 22)
+00002940: 0a20 2020 2060 6060 0a0a 2a20 2a2a 6765  .    ```..* **ge
+00002950: 745f 6c61 7374 5f6e 6577 7328 6d61 785f  t_last_news(max_
+00002960: 7265 675f 6e65 7773 3d32 2c20 6f6e 6c79  reg_news=2, only
+00002970: 5f74 6f64 6179 3d54 7275 652c 206f 6e6c  _today=True, onl
+00002980: 795f 6665 6174 7572 6564 3d46 616c 7365  y_featured=False
+00002990: 2920 2d3e 205b 6461 7465 2c20 5b66 6561  ) -> [date, [fea
+000029a0: 7475 7265 645f 6964 2c20 6665 6174 7572  tured_id, featur
+000029b0: 6564 5f74 6974 6c65 2c20 6665 6174 7572  ed_title, featur
+000029c0: 6564 5f64 6573 6369 7074 696f 6e5d 2c20  ed_desciption], 
+000029d0: 5b72 6567 756c 6172 5f69 642c 2072 6567  [regular_id, reg
+000029e0: 5f74 6974 6c65 2c20 7265 675f 7469 6d65  _title, reg_time
+000029f0: 5d5d 2a2a 0a0a 2020 2020 6060 600a 2020  ]]**..    ```.  
+00002a00: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+00002a10: 5f6c 6173 745f 6e65 7773 286f 6e6c 795f  _last_news(only_
+00002a20: 746f 6461 793d 5472 7565 290a 2020 2020  today=True).    
+00002a30: 0a20 2020 203e 3e3e 5b7b 2764 6174 6527  .    >>>[{'date'
+00002a40: 3a20 2731 352d 3034 272c 2027 665f 6e65  : '15-04', 'f_ne
+00002a50: 7773 273a 205b 5d2c 2027 6e65 7773 273a  ws': [], 'news':
+00002a60: 205b 7b27 6964 273a 2027 3338 3738 3427   [{'id': '38784'
+00002a70: 2c20 2774 6974 6c65 273a 2027 4d65 6469  , 'title': 'Medi
+00002a80: 613a 2046 5552 4941 2070 7261 6374 6963  a: FURIA practic
+00002a90: 696e 6720 7769 7468 206b 7965 2069 6e20  ing with kye in 
+00002aa0: 706c 6163 6520 6f66 2061 7254 272c 2027  place of arT', '
+00002ab0: 706f 7374 6564 273a 2027 616e 2068 6f75  posted': 'an hou
+00002ac0: 7220 6167 6f27 7d2c 207b 2769 6427 3a20  r ago'}, {'id': 
+00002ad0: 2733 3837 3833 272c 2027 7469 746c 6527  '38783', 'title'
+00002ae0: 3a20 2765 6c65 6374 726f 4e69 6320 746f  : 'electroNic to
+00002af0: 2070 6c61 7920 666f 7220 5669 7274 7573   play for Virtus
+00002b00: 2e70 726f 2061 7420 4553 4c20 5072 6f20  .pro at ESL Pro 
+00002b10: 4c65 6167 7565 2053 3139 272c 2027 706f  League S19', 'po
+00002b20: 7374 6564 273a 2027 3220 686f 7572 7320  sted': '2 hours 
+00002b30: 6167 6f27 7d2c 207b 2769 6427 3a20 2733  ago'}, {'id': '3
+00002b40: 3837 3831 272c 2027 7469 746c 6527 3a20  8781', 'title': 
+00002b50: 2754 6865 2045 5650 7320 616e 6420 4265  'The EVPs and Be
+00002b60: 7374 2046 6976 6520 6f66 2049 454d 2043  st Five of IEM C
+00002b70: 6865 6e67 6475 272c 2027 706f 7374 6564  hengdu', 'posted
+00002b80: 273a 2027 3720 686f 7572 7320 6167 6f27  ': '7 hours ago'
+00002b90: 7d5d 7d5d 0a20 200a 2020 2020 6060 600a  }]}].  .    ```.
+00002ba0: 0a2a 202a 2a67 6574 5f62 6573 745f 706c  .* **get_best_pl
+00002bb0: 6179 6572 7328 746f 703a 2069 6e74 203d  ayers(top: int =
+00002bc0: 2034 3029 202d 3e20 2827 7261 6e6b 272c   40) -> ('rank',
+00002bd0: 2027 6e61 6d65 272c 2027 7465 616d 272c   'name', 'team',
+00002be0: 2027 6d61 7073 272c 2027 7261 7469 6e67   'maps', 'rating
+00002bf0: 2729 2a2a 0a0a 2020 2020 6060 600a 2020  ')**..    ```.  
+00002c00: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+00002c10: 5f62 6573 745f 706c 6179 6572 7328 3229  _best_players(2)
+00002c20: 0a20 2020 200a 2020 2020 3e3e 3e5b 7b27  .    .    >>>[{'
+00002c30: 6964 273a 2027 3139 3233 3027 2c20 2772  id': '19230', 'r
+00002c40: 616e 6b27 3a20 312c 2027 6e61 6d65 273a  ank': 1, 'name':
+00002c50: 2027 6d30 4e45 5359 272c 2027 7465 616d   'm0NESY', 'team
+00002c60: 273a 2027 4732 272c 2027 6d61 7073 273a  ': 'G2', 'maps':
+00002c70: 2027 3434 272c 2027 7261 7469 6e67 273a   '44', 'rating':
+00002c80: 2027 312e 3337 277d 2c20 7b27 6964 273a   '1.37'}, {'id':
+00002c90: 2027 3138 3035 3327 2c20 2772 616e 6b27   '18053', 'rank'
+00002ca0: 3a20 322c 2027 6e61 6d65 273a 2027 6272  : 2, 'name': 'br
+00002cb0: 6f6b 7927 2c20 2774 6561 6d27 3a20 2746  oky', 'team': 'F
+00002cc0: 615a 6527 2c20 276d 6170 7327 3a20 2735  aZe', 'maps': '5
+00002cd0: 3427 2c20 2772 6174 696e 6727 3a20 2731  4', 'rating': '1
+00002ce0: 2e31 3927 7d5d 0a20 2020 2060 6060 0a0a  .19'}].    ```..
+00002cf0: 2a20 2a2a 6765 745f 706c 6179 6572 5f69  * **get_player_i
+00002d00: 6e66 6f28 6964 3a20 7374 7220 7c20 696e  nfo(id: str | in
+00002d10: 742c 206e 6963 6b6e 616d 653a 2073 7472  t, nickname: str
+00002d20: 292a 2a0a 2020 0a20 2060 6060 0a20 2061  )**.  .  ```.  a
+00002d30: 7761 6974 2068 6c74 762e 6765 745f 706c  wait hltv.get_pl
+00002d40: 6179 6572 5f69 6e66 6f28 3739 3938 2c20  ayer_info(7998, 
+00002d50: 2773 316d 706c 6527 290a 2020 0a20 207b  's1mple').  .  {
+00002d60: 2769 6427 3a20 3739 3938 2c20 276e 6963  'id': 7998, 'nic
+00002d70: 6b6e 616d 6527 3a20 2773 316d 706c 6527  kname': 's1mple'
+00002d80: 2c20 2774 6561 6d27 3a20 274e 6174 7573  , 'team': 'Natus
+00002d90: 2056 696e 6365 7265 272c 2027 7465 616d   Vincere', 'team
+00002da0: 5f69 6427 3a20 3436 3038 2c20 276e 616d  _id': 4608, 'nam
+00002db0: 6527 3a20 274f 6c65 6b73 616e 6472 204b  e': 'Oleksandr K
+00002dc0: 6f73 7479 6c69 6576 272c 2027 6e61 7469  ostyliev', 'nati
+00002dd0: 6f6e 616c 6974 7927 3a20 2755 6b72 6169  onality': 'Ukrai
+00002de0: 6e65 272c 2027 6167 6527 3a20 3236 2c20  ne', 'age': 26, 
+00002df0: 2772 6174 696e 6727 3a20 2730 2e39 3427  'rating': '0.94'
+00002e00: 2c20 276b 7072 273a 2027 302e 3630 272c  , 'kpr': '0.60',
+00002e10: 2027 6873 273a 2027 3537 2e39 2527 2c20   'hs': '57.9%', 
+00002e20: 276c 6173 745f 6d61 7463 6865 7327 3a20  'last_matches': 
+00002e30: 5b31 3033 3035 392c 2039 3937 3435 2c20  [103059, 99745, 
+00002e40: 3939 3732 382c 2039 3936 3936 2c20 3939  99728, 99696, 99
+00002e50: 3437 312c 2039 3933 3634 5d2c 2027 6c61  471, 99364], 'la
+00002e60: 7374 5f74 726f 7068 7927 3a20 2742 4c41  st_trophy': 'BLA
+00002e70: 5354 2050 7265 6d69 6572 2053 7072 696e  ST Premier Sprin
+00002e80: 6720 4669 6e61 6c20 3230 3232 272c 2027  g Final 2022', '
+00002e90: 746f 7461 6c5f 7472 6f70 6869 6573 273a  total_trophies':
+00002ea0: 2033 302c 2027 746f 7461 6c5f 6d76 7073   30, 'total_mvps
+00002eb0: 273a 2032 317d 0a20 2060 6060 0a0a 2a20  ': 21}.  ```..* 
+00002ec0: 2a2a 6765 7428 7479 7065 3a20 7374 722c  **get(type: str,
+00002ed0: 2069 643a 2069 6e74 207c 2073 7472 207c   id: int | str |
+00002ee0: 204e 6f6e 6520 3d20 4e6f 6e65 2c20 7469   None = None, ti
+00002ef0: 746c 653a 2073 7472 207c 204e 6f6e 6520  tle: str | None 
+00002f00: 3d20 4e6f 6e65 2c20 7465 616d 313a 2073  = None, team1: s
+00002f10: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
+00002f20: 2c20 7465 616d 323a 2073 7472 207c 204e  , team2: str | N
+00002f30: 6f6e 6520 3d20 4e6f 6e65 293a 2a2a 0a20  one = None):**. 
+00002f40: 2028 4245 5441 2920 5468 6973 206d 6574   (BETA) This met
+00002f50: 686f 6420 6973 206e 6f74 2066 696e 6973  hod is not finis
+00002f60: 6865 642e 2050 6f73 7369 626c 6520 7479  hed. Possible ty
+00002f70: 7065 7320 2765 7665 6e74 7327 2c20 276d  pes 'events', 'm
+00002f80: 6174 6368 6573 272c 2027 7465 616d 7327  atches', 'teams'
+00002f90: 2c20 616c 736f 2075 2063 616e 2061 6464  , also u can add
+00002fa0: 2069 6420 7c20 7469 746c 6520 7c20 7465   id | title | te
+00002fb0: 616d 3120 7c20 7465 616d 322c 2074 6f20  am1 | team2, to 
+00002fc0: 7061 7273 6520 6d6f 7265 2e0a 2020 0a20  parse more..  . 
+00002fd0: 2060 6060 0a20 200a 2020 6177 6169 7420   ```.  .  await 
+00002fe0: 686c 7476 2e67 6574 2827 6d61 7463 6865  hltv.get('matche
+00002ff0: 7327 2c20 3233 3731 3230 312c 2027 7265  s', 2371201, 're
+00003000: 732d 7265 6769 6f6e 616c 2d73 6572 6965  s-regional-serie
+00003010: 732d 332d 6c61 7461 6d27 2c20 2749 4d50  s-3-latam', 'IMP
+00003020: 4552 4941 4c27 2c20 274d 4942 5227 290a  ERIAL', 'MIBR').
+00003030: 2020 0a20 203e 3e3e 2028 3233 3731 3230    .  >>> (237120
+00003040: 312c 2030 2c20 302c 2027 4c49 5645 272c  1, 0, 0, 'LIVE',
+00003050: 205b 7b27 6d61 706e 616d 6527 3a20 2756   [{'mapname': 'V
+00003060: 6572 7469 676f 272c 2027 725f 7465 616d  ertigo', 'r_team
+00003070: 3127 3a20 2736 272c 2027 725f 7465 616d  1': '6', 'r_team
+00003080: 3227 3a20 2731 3327 7d2c 207b 276d 6170  2': '13'}, {'map
+00003090: 6e61 6d65 273a 2027 4d69 7261 6765 272c  name': 'Mirage',
+000030a0: 2027 725f 7465 616d 3127 3a20 272d 272c   'r_team1': '-',
+000030b0: 2027 725f 7465 616d 3227 3a20 272d 277d   'r_team2': '-'}
+000030c0: 2c20 7b27 6d61 706e 616d 6527 3a20 2741  , {'mapname': 'A
+000030d0: 6e75 6269 7327 2c20 2772 5f74 6561 6d31  nubis', 'r_team1
+000030e0: 273a 2027 2d27 2c20 2772 5f74 6561 6d32  ': '-', 'r_team2
+000030f0: 273a 2027 2d27 7d5d 2c20 5b5d 290a 2020  ': '-'}], []).  
+00003100: 0a20 2060 6060 0a0a 0a2d 2d2d 0a23 2045  .  ```...---.# E
+00003110: 7861 6d70 6c65 730a 0a2a 2a2a 2a53 696d  xamples..****Sim
+00003120: 706c 6520 4578 616d 706c 652a 2a2a 2a0a  ple Example****.
+00003130: 0a60 6060 0a66 726f 6d20 686c 7476 5f61  .```.from hltv_a
+00003140: 7379 6e63 5f61 7069 2069 6d70 6f72 7420  sync_api import 
+00003150: 486c 7476 0a0a 0a61 7379 6e63 2064 6566  Hltv...async def
+00003160: 2074 6573 7428 293a 0a0a 2020 2020 6173   test():..    as
+00003170: 796e 6320 7769 7468 2048 6c74 7628 2920  ync with Hltv() 
+00003180: 6173 2068 6c74 763a 0a20 2020 2020 2070  as hltv:.      p
+00003190: 7269 6e74 2861 7761 6974 2068 6c74 762e  rint(await hltv.
+000031a0: 6765 745f 6576 656e 745f 696e 666f 2837  get_event_info(7
+000031b0: 3134 382c 2027 7067 6c2d 6373 322d 6d61  148, 'pgl-cs2-ma
+000031c0: 6a6f 722d 636f 7065 6e68 6167 656e 2d32  jor-copenhagen-2
+000031d0: 3032 3427 2929 0a0a 6966 205f 5f6e 616d  024'))..if __nam
+000031e0: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
+000031f0: 223a 0a20 2020 2061 7379 6e63 696f 2e72  ":.    asyncio.r
+00003200: 756e 2874 6573 7428 2929 0a60 6060 0a0a  un(test()).```..
+00003210: 2a2a 2a2a 5072 6f78 7920 5061 7273 6572  ****Proxy Parser
+00003220: 2a2a 2a2a 0a0a 6060 600a 6672 6f6d 2068  ****..```.from h
+00003230: 6c74 765f 6173 796e 635f 6170 6920 696d  ltv_async_api im
+00003240: 706f 7274 2048 6c74 760a 0a0a 6173 796e  port Hltv...asyn
+00003250: 6320 6465 6620 7465 7374 2829 3a0a 0a20  c def test():.. 
+00003260: 2020 2068 6c74 7620 3d20 486c 7476 2864     hltv = Hltv(d
+00003270: 6562 7567 3d54 7275 652c 2070 726f 7879  ebug=True, proxy
+00003280: 5f70 6174 683d 2770 726f 7879 5f74 6573  _path='proxy_tes
+00003290: 742e 7478 7427 2c20 7469 6d65 6f75 743d  t.txt', timeout=
+000032a0: 312c 2064 656c 6574 655f 7072 6f78 793d  1, delete_proxy=
+000032b0: 5472 7565 2c20 7072 6f78 795f 7072 6f74  True, proxy_prot
+000032c0: 6f63 6f6c 3d27 6874 7470 2729 0a20 2020  ocol='http').   
+000032d0: 200a 2020 2020 7072 696e 7428 6177 6169   .    print(awai
+000032e0: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
+000032f0: 5f69 6e66 6f28 3731 3438 2c20 2770 676c  _info(7148, 'pgl
+00003300: 2d63 7332 2d6d 616a 6f72 2d63 6f70 656e  -cs2-major-copen
+00003310: 6861 6765 6e2d 3230 3234 2729 290a 0a69  hagen-2024'))..i
+00003320: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+00003330: 5f6d 6169 6e5f 5f22 3a0a 2020 2020 6173  _main__":.    as
+00003340: 796e 6369 6f2e 7275 6e28 7465 7374 2829  yncio.run(test()
+00003350: 290a 6060 600a 0a2a 2a2a 2a41 7574 6f6d  ).```..****Autom
+00003360: 6174 6963 2070 6172 7365 7220 7769 7468  atic parser with
+00003370: 2061 7271 2061 6e64 2072 6564 6973 2a2a   arq and redis**
+00003380: 2a2a 0a0a 2d20 746f 2072 756e 2074 7970  **..- to run typ
+00003390: 6520 2261 7271 2050 4154 485f 544f 5f46  e "arq PATH_TO_F
+000033a0: 494c 452e 576f 726b 6572 5365 7474 696e  ILE.WorkerSettin
+000033b0: 6773 220a 0a20 2020 2060 6060 0a20 2020  gs"..    ```.   
+000033c0: 2069 6d70 6f72 7420 756a 736f 6e0a 2020   import ujson.  
+000033d0: 2020 696d 706f 7274 2061 7379 6e63 696f    import asyncio
+000033e0: 0a20 2020 2066 726f 6d20 6172 7120 696d  .    from arq im
+000033f0: 706f 7274 2063 726f 6e0a 2020 2020 6672  port cron.    fr
+00003400: 6f6d 2072 6564 6973 2e61 7379 6e63 696f  om redis.asyncio
+00003410: 2069 6d70 6f72 7420 5265 6469 732c 2043   import Redis, C
+00003420: 6f6e 6e65 6374 696f 6e50 6f6f 6c0a 2020  onnectionPool.  
+00003430: 2020 0a20 2020 2066 726f 6d20 686c 7476    .    from hltv
+00003440: 5f61 7379 6e63 5f61 7069 2069 6d70 6f72  _async_api impor
+00003450: 7420 486c 7476 0a20 2020 200a 2020 2020  t Hltv.    .    
+00003460: 0a20 2020 200a 2020 2020 6173 796e 6320  .    .    async 
+00003470: 6465 6620 7374 6172 7475 7028 6374 7829  def startup(ctx)
+00003480: 3a0a 2020 2020 2020 2020 6173 796e 6320  :.        async 
+00003490: 7769 7468 2048 6c74 7628 6d61 785f 6465  with Hltv(max_de
+000034a0: 6c61 793d 352c 2070 726f 7879 5f70 6174  lay=5, proxy_pat
+000034b0: 683d 2770 726f 7869 6573 2e74 7874 272c  h='proxies.txt',
+000034c0: 2064 6562 7567 3d54 7275 6529 2061 7320   debug=True) as 
+000034d0: 686c 7476 3a0a 2020 2020 2020 2020 2020  hltv:.          
+000034e0: 2020 2020 6374 785b 2268 6c74 7622 5d20      ctx["hltv"] 
+000034f0: 3d20 686c 7476 0a20 200a 2020 2020 2020  = hltv.  .      
+00003500: 2020 6374 785b 2272 6564 6973 225d 203d    ctx["redis"] =
+00003510: 2072 6564 6973 5f63 6c69 656e 7420 3d20   redis_client = 
+00003520: 5265 6469 7328 0a20 2020 2020 2020 2020  Redis(.         
+00003530: 2020 2063 6f6e 6e65 6374 696f 6e5f 706f     connection_po
+00003540: 6f6c 3d43 6f6e 6e65 6374 696f 6e50 6f6f  ol=ConnectionPoo
+00003550: 6c2e 6672 6f6d 5f75 726c 2873 6574 7469  l.from_url(setti
+00003560: 6e67 732e 7265 6469 735f 7572 6c29 290a  ngs.redis_url)).
+00003570: 2020 2020 2020 2020 6c6f 6767 6572 2e73          logger.s
+00003580: 7563 6365 7373 2866 2253 6368 6564 756c  uccess(f"Schedul
+00003590: 6572 2073 7461 7274 6564 2e20 5554 4320  er started. UTC 
+000035a0: 7469 6d65 207b 6461 7465 7469 6d65 2e75  time {datetime.u
+000035b0: 7463 6e6f 7728 297d 2229 0a20 2020 200a  tcnow()}").    .
+000035c0: 2020 2020 0a20 2020 2061 7379 6e63 2064      .    async d
+000035d0: 6566 2073 6875 7464 6f77 6e28 6374 7829  ef shutdown(ctx)
+000035e0: 3a0a 2020 2020 2020 2020 6177 6169 7420  :.        await 
+000035f0: 6374 785b 2272 6564 6973 225d 2e63 6c6f  ctx["redis"].clo
+00003600: 7365 2829 0a20 2020 200a 2020 2020 0a20  se().    .    . 
+00003610: 2020 2061 7379 6e63 2064 6566 2070 6172     async def par
+00003620: 7365 5f6d 6174 6368 6573 2863 7478 293a  se_matches(ctx):
+00003630: 0a20 2020 2020 2020 2068 6c74 7620 3d20  .        hltv = 
+00003640: 6374 785b 2268 6c74 7622 5d0a 2020 2020  ctx["hltv"].    
+00003650: 2020 2020 7265 6469 7320 3d20 6374 785b      redis = ctx[
+00003660: 2272 6564 6973 225d 0a20 2020 2020 2020  "redis"].       
+00003670: 206d 6174 6368 6573 203d 2061 7761 6974   matches = await
+00003680: 2068 6c74 762e 6765 745f 7570 636f 6d69   hltv.get_upcomi
+00003690: 6e67 5f6d 6174 6368 6573 2831 2c20 3129  ng_matches(1, 1)
+000036a0: 0a20 2020 2020 2020 2069 6620 6d61 7463  .        if matc
+000036b0: 6865 733a 0a20 2020 2020 2020 2020 2020  hes:.           
+000036c0: 2061 7761 6974 2072 6564 6973 2e73 6574   await redis.set
+000036d0: 2822 6d61 7463 6865 7322 2c20 756a 736f  ("matches", ujso
+000036e0: 6e2e 6475 6d70 7328 6d61 7463 6865 7329  n.dumps(matches)
+000036f0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00003700: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00003710: 6572 2e65 7272 6f72 2822 6572 726f 7220  er.error("error 
+00003720: 7061 7273 696e 6720 6d61 7463 6865 7322  parsing matches"
+00003730: 290a 2020 2020 0a20 2020 2061 7379 6e63  ).    .    async
+00003740: 2064 6566 2070 6172 7365 5f65 7665 6e74   def parse_event
+00003750: 7328 6374 7829 3a0a 2020 2020 2020 2020  s(ctx):.        
+00003760: 686c 7476 203d 2063 7478 5b22 686c 7476  hltv = ctx["hltv
+00003770: 225d 0a20 2020 2020 2020 2072 6564 6973  "].        redis
+00003780: 203d 2063 7478 5b22 7265 6469 7322 5d0a   = ctx["redis"].
+00003790: 2020 2020 2020 2020 6576 656e 7473 203d          events =
+000037a0: 2061 7761 6974 2068 6c74 762e 6765 745f   await hltv.get_
+000037b0: 6576 656e 7473 2829 0a20 2020 2020 2020  events().       
+000037c0: 2069 6620 6576 656e 7473 3a0a 2020 2020   if events:.    
+000037d0: 2020 2020 2020 2020 6177 6169 7420 7265          await re
+000037e0: 6469 732e 7365 7428 2265 7665 6e74 7322  dis.set("events"
+000037f0: 2c20 756a 736f 6e2e 6475 6d70 7328 6576  , ujson.dumps(ev
+00003800: 656e 7473 2929 0a20 2020 2020 2020 2065  ents)).        e
+00003810: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003820: 206c 6f67 6765 722e 6572 726f 7228 2265   logger.error("e
+00003830: 7272 6f72 2070 6172 7369 6e67 2065 7665  rror parsing eve
+00003840: 6e74 7322 290a 2020 2020 0a20 2020 200a  nts").    .    .
+00003850: 2020 2020 6173 796e 6320 6465 6620 7061      async def pa
+00003860: 7273 655f 746f 705f 7465 616d 7328 6374  rse_top_teams(ct
+00003870: 7829 3a0a 2020 2020 2020 2020 686c 7476  x):.        hltv
+00003880: 203d 2063 7478 5b22 686c 7476 225d 0a20   = ctx["hltv"]. 
+00003890: 2020 2020 2020 2072 6564 6973 203d 2063         redis = c
+000038a0: 7478 5b22 7265 6469 7322 5d0a 2020 2020  tx["redis"].    
+000038b0: 2020 2020 746f 705f 7465 616d 7320 3d20      top_teams = 
+000038c0: 6177 6169 7420 686c 7476 2e67 6574 5f74  await hltv.get_t
+000038d0: 6f70 5f74 6561 6d73 2833 3029 0a20 2020  op_teams(30).   
+000038e0: 2020 2020 2069 6620 746f 705f 7465 616d       if top_team
+000038f0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00003900: 7761 6974 2072 6564 6973 2e73 6574 2822  wait redis.set("
+00003910: 746f 705f 7465 616d 7322 2c20 756a 736f  top_teams", ujso
+00003920: 6e2e 6475 6d70 7328 746f 705f 7465 616d  n.dumps(top_team
+00003930: 7329 290a 2020 2020 2020 2020 656c 7365  s)).        else
+00003940: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00003950: 6767 6572 2e65 7272 6f72 2822 6572 726f  gger.error("erro
+00003960: 7220 7061 7273 696e 6720 746f 7020 7465  r parsing top te
+00003970: 616d 7322 290a 2020 2020 0a20 2020 200a  ams").    .    .
+00003980: 2020 2020 6173 796e 6320 6465 6620 7061      async def pa
+00003990: 7273 655f 746f 705f 706c 6179 6572 7328  rse_top_players(
+000039a0: 6374 7829 3a0a 2020 2020 2020 2020 686c  ctx):.        hl
+000039b0: 7476 203d 2063 7478 5b22 686c 7476 225d  tv = ctx["hltv"]
+000039c0: 0a20 2020 2020 2020 2072 6564 6973 203d  .        redis =
+000039d0: 2063 7478 5b22 7265 6469 7322 5d0a 2020   ctx["redis"].  
+000039e0: 2020 2020 2020 746f 705f 706c 6179 6572        top_player
+000039f0: 7320 3d20 6177 6169 7420 686c 7476 2e67  s = await hltv.g
+00003a00: 6574 5f62 6573 745f 706c 6179 6572 7328  et_best_players(
+00003a10: 3330 290a 2020 2020 2020 2020 6966 2074  30).        if t
+00003a20: 6f70 5f70 6c61 7965 7273 3a0a 2020 2020  op_players:.    
+00003a30: 2020 2020 2020 2020 6177 6169 7420 7265          await re
+00003a40: 6469 732e 7365 7428 2274 6f70 5f74 6561  dis.set("top_tea
+00003a50: 6d73 222c 2075 6a73 6f6e 2e64 756d 7073  ms", ujson.dumps
+00003a60: 2874 6f70 5f70 6c61 7965 7273 2929 0a20  (top_players)). 
+00003a70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003a80: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00003a90: 6572 726f 7228 2265 7272 6f72 2070 6172  error("error par
+00003aa0: 7369 6e67 2074 6f70 2070 6c61 7965 7273  sing top players
+00003ab0: 2229 0a20 2020 200a 2020 2020 0a20 2020  ").    .    .   
+00003ac0: 2061 7379 6e63 2064 6566 2070 6172 7365   async def parse
+00003ad0: 5f6c 6173 745f 6e65 7773 2863 7478 293a  _last_news(ctx):
+00003ae0: 0a20 2020 2020 2020 2068 6c74 7620 3d20  .        hltv = 
+00003af0: 6374 785b 2268 6c74 7622 5d0a 2020 2020  ctx["hltv"].    
+00003b00: 2020 2020 7265 6469 7320 3d20 6374 785b      redis = ctx[
+00003b10: 2272 6564 6973 225d 0a20 2020 2020 2020  "redis"].       
+00003b20: 206e 6577 7320 3d20 6177 6169 7420 686c   news = await hl
+00003b30: 7476 2e67 6574 5f6c 6173 745f 6e65 7773  tv.get_last_news
+00003b40: 286f 6e6c 795f 746f 6461 793d 5472 7565  (only_today=True
+00003b50: 2c20 6d61 785f 7265 675f 6e65 7773 3d34  , max_reg_news=4
+00003b60: 290a 2020 2020 2020 2020 6966 206e 6577  ).        if new
+00003b70: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00003b80: 7761 6974 2072 6564 6973 2e73 6574 2822  wait redis.set("
+00003b90: 6e65 7773 222c 2075 6a73 6f6e 2e64 756d  news", ujson.dum
+00003ba0: 7073 286e 6577 7329 290a 2020 2020 2020  ps(news)).      
+00003bb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003bc0: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
+00003bd0: 2822 6572 726f 7220 7061 7273 696e 6720  ("error parsing 
+00003be0: 6e65 7773 2229 0a20 2020 200a 2020 2020  news").    .    
+00003bf0: 0a20 2020 2063 6c61 7373 2057 6f72 6b65  .    class Worke
+00003c00: 7253 6574 7469 6e67 733a 0a20 2020 2020  rSettings:.     
+00003c10: 2020 2072 6564 6973 5f73 6574 7469 6e67     redis_setting
+00003c20: 7320 3d20 7365 7474 696e 6773 2e72 6564  s = settings.red
+00003c30: 6973 5f70 6f6f 6c0a 2020 2020 2020 2020  is_pool.        
+00003c40: 6f6e 5f73 7461 7274 7570 203d 2073 7461  on_startup = sta
+00003c50: 7274 7570 0a20 2020 2020 2020 206f 6e5f  rtup.        on_
+00003c60: 7368 7574 646f 776e 203d 2073 6875 7464  shutdown = shutd
+00003c70: 6f77 6e0a 2020 2020 2020 2020 6675 6e63  own.        func
+00003c80: 7469 6f6e 7320 3d20 5b70 6172 7365 5f6d  tions = [parse_m
+00003c90: 6174 6368 6573 2c0a 2020 2020 2020 2020  atches,.        
 00003ca0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00003cb0: 7365 5f6c 6173 745f 6e65 7773 2c0a 2020  se_last_news,.  
+00003cb0: 7365 5f65 7665 6e74 732c 0a20 2020 2020  se_events,.     
 00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 2020 205d 0a20 2020 2020 2020 2063 726f     ].        cro
-00003ce0: 6e5f 6a6f 6273 203d 205b 0a20 2020 2020  n_jobs = [.     
-00003cf0: 2020 2020 2020 2063 726f 6e28 7061 7273         cron(pars
-00003d00: 655f 6d61 7463 6865 732c 206d 696e 7574  e_matches, minut
-00003d10: 653d 3539 292c 0a20 2020 2020 2020 2020  e=59),.         
-00003d20: 2020 2063 726f 6e28 7061 7273 655f 6576     cron(parse_ev
-00003d30: 656e 7473 2c20 686f 7572 3d30 2c20 6d69  ents, hour=0, mi
-00003d40: 6e75 7465 3d30 2c20 7365 636f 6e64 3d30  nute=0, second=0
-00003d50: 292c 0a20 2020 2020 2020 2020 2020 2063  ),.            c
-00003d60: 726f 6e28 7061 7273 655f 746f 705f 7465  ron(parse_top_te
-00003d70: 616d 732c 2064 6179 3d30 2c20 686f 7572  ams, day=0, hour
-00003d80: 3d31 382c 206d 696e 7574 653d 312c 2073  =18, minute=1, s
-00003d90: 6563 6f6e 643d 3330 292c 0a20 2020 2020  econd=30),.     
-00003da0: 2020 2020 2020 2063 726f 6e28 7061 7273         cron(pars
-00003db0: 655f 746f 705f 706c 6179 6572 732c 2064  e_top_players, d
-00003dc0: 6179 3d30 2c20 686f 7572 3d32 302c 206d  ay=0, hour=20, m
-00003dd0: 696e 7574 653d 302c 2073 6563 6f6e 643d  inute=0, second=
-00003de0: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-00003df0: 6372 6f6e 2870 6172 7365 5f6c 6173 745f  cron(parse_last_
-00003e00: 6e65 7773 2c20 6d69 6e75 7465 3d35 3529  news, minute=55)
-00003e10: 2c0a 2020 2020 2020 2020 5d0a 0a20 2020  ,.        ]..   
-00003e20: 2060 6060 0a0a 2320 5465 7374 733a 0a0a   ```..# Tests:..
-00003e30: 2a2a 3c61 2068 7265 663d 2768 7474 7073  **<a href='https
-00003e40: 3a2f 2f67 6974 6875 622e 636f 6d2f 616b  ://github.com/ak
-00003e50: 696d 6572 736c 7973 2f68 6c74 762d 6173  imerslys/hltv-as
-00003e60: 796e 632d 6170 692f 626c 6f62 2f6d 6169  ync-api/blob/mai
-00003e70: 6e2f 7465 7374 2f68 6172 645f 7465 7374  n/test/hard_test
-00003e80: 2e70 7927 3e54 6f20 7465 7374 206c 6962  .py'>To test lib
-00003e90: 7261 7279 2079 6f75 2063 616e 2075 7365  rary you can use
-00003ea0: 2074 656d 706f 7261 7269 6c79 2074 6573   temporarily tes
-00003eb0: 7420 6669 6c65 3c2f 613e 2a2a 0a0a 6060  t file</a>**..``
-00003ec0: 600a 0a50 6172 7365 6420 3230 3820 6d61  `..Parsed 208 ma
-00003ed0: 7463 6865 732e 2839 3773 2920 4552 524f  tches.(97s) ERRO
-00003ee0: 5253 3a20 302f 3230 380a 5061 7273 6564  RS: 0/208.Parsed
-00003ef0: 2032 3520 6576 656e 7473 2e28 3233 7329   25 events.(23s)
-00003f00: 2045 5252 4f52 533a 2030 2f32 350a 5061   ERRORS: 0/25.Pa
-00003f10: 7273 6564 2033 3120 7465 616d 732e 2834  rsed 31 teams.(4
-00003f20: 3173 2920 4552 524f 5253 3a20 302f 3331  1s) ERRORS: 0/31
-00003f30: 0a50 6172 7365 6420 3331 2070 6c61 7965  .Parsed 31 playe
-00003f40: 7273 2e28 3238 7329 2045 5252 4f52 533a  rs.(28s) ERRORS:
-00003f50: 2030 2f33 310a 4552 524f 5253 3d30 0a53   0/31.ERRORS=0.S
-00003f60: 5543 4345 5353 3d32 3834 0a54 6f74 616c  UCCESS=284.Total
-00003f70: 2070 6172 7365 643d 3238 340a 546f 7461   parsed=284.Tota
-00003f80: 6c20 7469 6d65 2039 362e 3833 3638 0a0a  l time 96.8368..
-00003f90: 6060 600a 0a23 2042 6574 6120 2f20 556e  ```..# Beta / Un
-00003fa0: 7265 6c65 6173 6564 0a0a 2a2a 5468 6174  released..**That
-00003fb0: 2066 756e 6374 696f 6e73 2077 6572 6520   functions were 
-00003fc0: 6d61 6465 2066 6f72 206d 7973 656c 662c  made for myself,
-00003fd0: 2062 6566 6f72 6520 7573 696e 6720 7265   before using re
-00003fe0: 636f 6d6d 656e 6420 796f 7520 746f 2063  commend you to c
-00003ff0: 6865 636b 2074 6865 2066 696c 652a 2a0a  heck the file**.
-00004000: 0a23 2052 6571 7569 7265 6d65 6e74 733a  .# Requirements:
-00004010: 0a0a 5079 7468 6f6e 2033 2e39 2b0a 0a4c  ..Python 3.9+..L
-00004020: 6963 656e 7365 3a0a 484c 5456 2041 7379  icense:.HLTV Asy
-00004030: 6e63 2069 7320 6c69 6365 6e73 6564 2075  nc is licensed u
-00004040: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
-00004050: 656e 7365 2c20 616c 6c6f 7769 6e67 2066  ense, allowing f
-00004060: 6f72 2070 6572 736f 6e61 6c20 616e 6420  or personal and 
-00004070: 636f 6d6d 6572 6369 616c 2075 7365 2077  commercial use w
-00004080: 6974 6820 6d69 6e69 6d61 6c20 7265 7374  ith minimal rest
-00004090: 7269 6374 696f 6e73 2e0a 0a              rictions...
+00003cd0: 7061 7273 655f 746f 705f 7465 616d 732c  parse_top_teams,
+00003ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cf0: 2020 2020 2020 7061 7273 655f 746f 705f        parse_top_
+00003d00: 706c 6179 6572 732c 0a20 2020 2020 2020  players,.       
+00003d10: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00003d20: 7273 655f 6c61 7374 5f6e 6577 732c 0a20  rse_last_news,. 
+00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d40: 2020 2020 5d0a 2020 2020 2020 2020 6372      ].        cr
+00003d50: 6f6e 5f6a 6f62 7320 3d20 5b0a 2020 2020  on_jobs = [.    
+00003d60: 2020 2020 2020 2020 6372 6f6e 2870 6172          cron(par
+00003d70: 7365 5f6d 6174 6368 6573 2c20 6d69 6e75  se_matches, minu
+00003d80: 7465 3d35 3929 2c0a 2020 2020 2020 2020  te=59),.        
+00003d90: 2020 2020 6372 6f6e 2870 6172 7365 5f65      cron(parse_e
+00003da0: 7665 6e74 732c 2068 6f75 723d 302c 206d  vents, hour=0, m
+00003db0: 696e 7574 653d 302c 2073 6563 6f6e 643d  inute=0, second=
+00003dc0: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
+00003dd0: 6372 6f6e 2870 6172 7365 5f74 6f70 5f74  cron(parse_top_t
+00003de0: 6561 6d73 2c20 6461 793d 302c 2068 6f75  eams, day=0, hou
+00003df0: 723d 3138 2c20 6d69 6e75 7465 3d31 2c20  r=18, minute=1, 
+00003e00: 7365 636f 6e64 3d33 3029 2c0a 2020 2020  second=30),.    
+00003e10: 2020 2020 2020 2020 6372 6f6e 2870 6172          cron(par
+00003e20: 7365 5f74 6f70 5f70 6c61 7965 7273 2c20  se_top_players, 
+00003e30: 6461 793d 302c 2068 6f75 723d 3230 2c20  day=0, hour=20, 
+00003e40: 6d69 6e75 7465 3d30 2c20 7365 636f 6e64  minute=0, second
+00003e50: 3d30 292c 0a20 2020 2020 2020 2020 2020  =0),.           
+00003e60: 2063 726f 6e28 7061 7273 655f 6c61 7374   cron(parse_last
+00003e70: 5f6e 6577 732c 206d 696e 7574 653d 3535  _news, minute=55
+00003e80: 292c 0a20 2020 2020 2020 205d 0a0a 2020  ),.        ]..  
+00003e90: 2020 6060 600a 0a23 2054 6573 7473 3a0a    ```..# Tests:.
+00003ea0: 0a2a 2a3c 6120 6872 6566 3d27 6874 7470  .**<a href='http
+00003eb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00003ec0: 6b69 6d65 7273 6c79 732f 686c 7476 2d61  kimerslys/hltv-a
+00003ed0: 7379 6e63 2d61 7069 2f62 6c6f 622f 6d61  sync-api/blob/ma
+00003ee0: 696e 2f74 6573 742f 6861 7264 5f74 6573  in/test/hard_tes
+00003ef0: 742e 7079 273e 546f 2074 6573 7420 6c69  t.py'>To test li
+00003f00: 6272 6172 7920 796f 7520 6361 6e20 7573  brary you can us
+00003f10: 6520 7465 6d70 6f72 6172 696c 7920 7465  e temporarily te
+00003f20: 7374 2066 696c 653c 2f61 3e2a 2a0a 0a60  st file</a>**..`
+00003f30: 6060 0a0a 5061 7273 6564 2032 3038 206d  ``..Parsed 208 m
+00003f40: 6174 6368 6573 2e28 3937 7329 2045 5252  atches.(97s) ERR
+00003f50: 4f52 533a 2030 2f32 3038 0a50 6172 7365  ORS: 0/208.Parse
+00003f60: 6420 3235 2065 7665 6e74 732e 2832 3373  d 25 events.(23s
+00003f70: 2920 4552 524f 5253 3a20 302f 3235 0a50  ) ERRORS: 0/25.P
+00003f80: 6172 7365 6420 3331 2074 6561 6d73 2e28  arsed 31 teams.(
+00003f90: 3431 7329 2045 5252 4f52 533a 2030 2f33  41s) ERRORS: 0/3
+00003fa0: 310a 5061 7273 6564 2033 3120 706c 6179  1.Parsed 31 play
+00003fb0: 6572 732e 2832 3873 2920 4552 524f 5253  ers.(28s) ERRORS
+00003fc0: 3a20 302f 3331 0a45 5252 4f52 533d 300a  : 0/31.ERRORS=0.
+00003fd0: 5355 4343 4553 533d 3238 340a 546f 7461  SUCCESS=284.Tota
+00003fe0: 6c20 7061 7273 6564 3d32 3834 0a54 6f74  l parsed=284.Tot
+00003ff0: 616c 2074 696d 6520 3936 2e38 3336 380a  al time 96.8368.
+00004000: 0a60 6060 0a0a 2320 4265 7461 202f 2055  .```..# Beta / U
+00004010: 6e72 656c 6561 7365 640a 0a2a 2a54 6861  nreleased..**Tha
+00004020: 7420 6675 6e63 7469 6f6e 7320 7765 7265  t functions were
+00004030: 206d 6164 6520 666f 7220 6d79 7365 6c66   made for myself
+00004040: 2c20 6265 666f 7265 2075 7369 6e67 2072  , before using r
+00004050: 6563 6f6d 6d65 6e64 2079 6f75 2074 6f20  ecommend you to 
+00004060: 6368 6563 6b20 7468 6520 6669 6c65 2a2a  check the file**
+00004070: 0a0a 2320 5265 7175 6972 656d 656e 7473  ..# Requirements
+00004080: 3a0a 0a50 7974 686f 6e20 332e 392b 0a0a  :..Python 3.9+..
+00004090: 4c69 6365 6e73 653a 0a48 4c54 5620 4173  License:.HLTV As
+000040a0: 796e 6320 6973 206c 6963 656e 7365 6420  ync is licensed 
+000040b0: 756e 6465 7220 7468 6520 4d49 5420 4c69  under the MIT Li
+000040c0: 6365 6e73 652c 2061 6c6c 6f77 696e 6720  cense, allowing 
+000040d0: 666f 7220 7065 7273 6f6e 616c 2061 6e64  for personal and
+000040e0: 2063 6f6d 6d65 7263 6961 6c20 7573 6520   commercial use 
+000040f0: 7769 7468 206d 696e 696d 616c 2072 6573  with minimal res
+00004100: 7472 6963 7469 6f6e 732e 0a0a            trictions...
```

