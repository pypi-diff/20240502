# Comparing `tmp/mpflash-0.7.3.tar.gz` & `tmp/mpflash-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.7.3.tar", max compression
+gzip compressed data, was "mpflash-0.7.4.tar", max compression
```

## Comparing `mpflash-0.7.3.tar` & `mpflash-0.7.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.3/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.3/mpflash/__init__.py
--rw-r--r--   0        0        0     8442 2024-04-29 18:55:09.404909 mpflash-0.7.3/mpflash/ask_input.py
--rw-r--r--   0        0        0     3266 2024-04-29 18:55:09.406130 mpflash-0.7.3/mpflash/cli_download.py
--rw-r--r--   0        0        0     5847 2024-04-29 18:55:09.407466 mpflash-0.7.3/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.3/mpflash/cli_group.py
--rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.3/mpflash/cli_list.py
--rw-r--r--   0        0        0      656 2024-04-29 18:55:09.408806 mpflash-0.7.3/mpflash/cli_main.py
--rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.3/mpflash/common.py
--rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.3/mpflash/config.py
--rw-r--r--   0        0        0    10991 2024-04-29 18:55:09.412110 mpflash-0.7.3/mpflash/download.py
--rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.3/mpflash/downloaded.py
--rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.3/mpflash/errors.py
--rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.3/mpflash/flash.py
--rw-r--r--   0        0        0     2316 2024-04-29 18:55:09.415109 mpflash-0.7.3/mpflash/flash_esp.py
--rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.3/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.3/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.3/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2093 2024-04-29 18:55:09.417421 mpflash-0.7.3/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.3/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4298 2024-04-05 19:52:32.898069 mpflash-0.7.3/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     1072 2024-04-05 19:52:32.900154 mpflash-0.7.3/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     4037 2024-05-01 12:41:39.214280 mpflash-0.7.3/mpflash/list.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.3/mpflash/logger.py
--rw-r--r--   0        0        0     3509 2024-04-29 18:55:09.418429 mpflash-0.7.3/mpflash/mpboard_id/__init__.py
--rw-r--r--   0        0        0     2386 2024-05-01 15:03:35.805669 mpflash-0.7.3/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.3/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-04-30 08:26:55.864409 mpflash-0.7.3/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0     7047 2024-05-01 15:03:35.781930 mpflash-0.7.3/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.3/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.3/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.3/mpflash/vendor/dfu.py
--rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.3/mpflash/vendor/pydfu.py
--rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.3/mpflash/vendor/readme.md
--rw-r--r--   0        0        0     3629 2024-04-29 18:55:09.425429 mpflash-0.7.3/mpflash/vendor/versions.py
--rw-r--r--   0        0        0     5299 2024-04-29 18:55:09.426431 mpflash-0.7.3/mpflash/worklist.py
--rw-r--r--   0        0        0     1648 2024-05-01 14:40:41.422907 mpflash-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.3/README.md
--rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 mpflash-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.4/mpflash/__init__.py
+-rw-r--r--   0        0        0     8442 2024-05-02 20:53:12.953952 mpflash-0.7.4/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3266 2024-05-02 20:53:12.958850 mpflash-0.7.4/mpflash/cli_download.py
+-rw-r--r--   0        0        0     5847 2024-05-02 20:53:12.961542 mpflash-0.7.4/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.4/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.4/mpflash/cli_list.py
+-rw-r--r--   0        0        0      656 2024-04-29 18:55:09.408806 mpflash-0.7.4/mpflash/cli_main.py
+-rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.4/mpflash/common.py
+-rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.4/mpflash/config.py
+-rw-r--r--   0        0        0    10991 2024-05-02 20:53:12.964386 mpflash-0.7.4/mpflash/download.py
+-rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.4/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.4/mpflash/errors.py
+-rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.4/mpflash/flash.py
+-rw-r--r--   0        0        0     2316 2024-05-02 20:53:12.964386 mpflash-0.7.4/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.4/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.4/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.4/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2093 2024-05-02 20:53:12.968640 mpflash-0.7.4/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.4/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4298 2024-05-02 20:53:12.968640 mpflash-0.7.4/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1072 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     3252 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.4/mpflash/logger.py
+-rw-r--r--   0        0        0     3509 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     2361 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.4/mpflash/mpboard_id/board_info.csv
+-rw-r--r--   0        0        0   674442 2024-04-30 08:26:55.864409 mpflash-0.7.4/mpflash/mpboard_id/board_info.json
+-rw-r--r--   0        0        0     7017 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.4/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.4/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.4/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.4/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.4/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3629 2024-04-29 18:55:09.425429 mpflash-0.7.4/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5299 2024-05-02 20:53:12.993284 mpflash-0.7.4/mpflash/worklist.py
+-rw-r--r--   0        0        0     1630 2024-05-02 20:54:16.528433 mpflash-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.4/README.md
+-rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 mpflash-0.7.4/PKG-INFO
```

### Comparing `mpflash-0.7.3/LICENSE` & `mpflash-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/ask_input.py` & `mpflash-0.7.4/mpflash/ask_input.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/cli_download.py` & `mpflash-0.7.4/mpflash/cli_download.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/cli_flash.py` & `mpflash-0.7.4/mpflash/cli_flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/cli_group.py` & `mpflash-0.7.4/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/cli_list.py` & `mpflash-0.7.4/mpflash/cli_list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/cli_main.py` & `mpflash-0.7.4/mpflash/cli_main.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/common.py` & `mpflash-0.7.4/mpflash/common.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/download.py` & `mpflash-0.7.4/mpflash/download.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/downloaded.py` & `mpflash-0.7.4/mpflash/downloaded.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash.py` & `mpflash-0.7.4/mpflash/flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_esp.py` & `mpflash-0.7.4/mpflash/flash_esp.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_stm32.py` & `mpflash-0.7.4/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_stm32_cube.py` & `mpflash-0.7.4/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_stm32_dfu.py` & `mpflash-0.7.4/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_uf2.py` & `mpflash-0.7.4/mpflash/flash_uf2.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_uf2_linux.py` & `mpflash-0.7.4/mpflash/flash_uf2_linux.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/flash_uf2_windows.py` & `mpflash-0.7.4/mpflash/flash_uf2_windows.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/list.py` & `mpflash-0.7.4/mpflash/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,67 +47,43 @@
     return conn_mcus
 
 
 def show_mcus(
     conn_mcus: List[MPRemoteBoard],
     title: str = "Connected boards",
     refresh: bool = True,
-):
-    console.print(mcu_table(conn_mcus, title, refresh))
-
-
-def abbrv_family(family: str, is_narrow: bool) -> str:
-    ABRV = {"micropython": "upy", "circuitpython": "cpy"}
-    if is_narrow:
-        if family in ABRV:
-            return ABRV[family]
-        return family[:4]
-    return family
-
-
-def mcu_table(
-    conn_mcus: List[MPRemoteBoard],
-    title: str = "Connected boards",
-    refresh: bool = True,
-):
+):  # sourcery skip: extract-duplicate-method
     """Show the list of connected boards in a nice table"""
     table = Table(
         title=title,
         title_style="magenta",
         header_style="bold magenta",
         collapse_padding=True,
-        padding=(0, 0),
-        # width=80,
+        width=110,
     )
-    needs_build = any(mcu.build for mcu in conn_mcus)
-    is_narrow = console.width < 100
-    table.add_column("Ser." if is_narrow else "Serial", overflow="fold")
-    table.add_column("Fam." if is_narrow else "Family", overflow="crop", max_width=4 if is_narrow else None)
+    table.add_column("Serial", overflow="fold")
+    table.add_column("Family")
     table.add_column("Port")
     table.add_column("Board", overflow="fold")
     # table.add_column("Variant") # TODO: add variant
     table.add_column("CPU")
-    table.add_column("Version", overflow="fold", max_width=8 if is_narrow else None)
-    if needs_build:
-        table.add_column("Bld" if is_narrow else "Build", justify="right")
+    table.add_column("Version")
+    table.add_column("build", justify="right")
 
     for mcu in track(conn_mcus, description="Updating board info", transient=True, update_period=0.1):
         if refresh:
             try:
                 mcu.get_mcu_info()
             except ConnectionError:
                 continue
         description = f"[italic bright_cyan]{mcu.description}" if mcu.description else ""
-        row = [
+        table.add_row(
             mcu.serialport.replace("/dev/", ""),
-            abbrv_family(mcu.family, is_narrow),
+            mcu.family,
             mcu.port,
             f"{mcu.board}\n{description}".strip(),
             # mcu.variant,
             mcu.cpu,
             clean_version(mcu.version),
-        ]
-        if needs_build:
-            row.append(mcu.build)
-
-        table.add_row(*row)
-    return table
+            mcu.build,
+        )
+    console.print(table)
```

### Comparing `mpflash-0.7.3/mpflash/logger.py` & `mpflash-0.7.4/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/mpboard_id/__init__.py` & `mpflash-0.7.4/mpflash/mpboard_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/mpboard_id/board_id.py` & `mpflash-0.7.4/mpflash/mpboard_id/board_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 from mpflash.vendor.versions import clean_version
 
 ###############################################################################################
 HERE = Path(__file__).parent
 ###############################################################################################
 
 
-def find_board_id_by_description(
+def find_board_id(
     descr: str, short_descr: str, board_info: Optional[Path] = None, version: str = "stable"
 ) -> Optional[str]:
     """Find the MicroPython BOARD_ID based on the description in the firmware"""
     try:
-        boards = _find_board_id_by_description(
+        boards = find_board_id_by_description(
             descr=descr,
             short_descr=short_descr,
             board_info=board_info,
             version=clean_version(version),
         )
         return boards[-1]["board"]
     except MPFlashError:
         return "UNKNOWN_BOARD"
 
 
 @functools.lru_cache(maxsize=20)
-def _find_board_id_by_description(
-    *, descr: str, short_descr: str, version="v1.21.0", board_info: Optional[Path] = None
-):
+def find_board_id_by_description(*, descr: str, short_descr: str, version="v1.21.0", board_info: Optional[Path] = None):
     """
     Find the MicroPython BOARD_ID based on the description in the firmware
     using the pre-built board_info.json file
     """
     if not board_info:
         board_info = HERE / "board_info.json"
     if not board_info.exists():
```

### Comparing `mpflash-0.7.3/mpflash/mpboard_id/board_info.csv` & `mpflash-0.7.4/mpflash/mpboard_id/board_info.csv`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/mpboard_id/board_info.json` & `mpflash-0.7.4/mpflash/mpboard_id/board_info.json`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/mpremoteboard/__init__.py` & `mpflash-0.7.4/mpflash/mpremoteboard/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import serial.tools.list_ports
 from loguru import logger as log
 from rich.progress import track
 from tenacity import retry, stop_after_attempt, wait_fixed
 
 from mpflash.errors import MPFlashError
-from mpflash.mpboard_id.board_id import find_board_id_by_description
+from mpflash.mpboard_id.board_id import find_board_id
 from mpflash.mpremoteboard.runner import run
 
 ###############################################################################################
 # TODO : make this a bit nicer
 HERE = Path(__file__).parent
 
 OK = 0
@@ -112,15 +112,15 @@
             self.port = info["port"]
             self.cpu = info["cpu"]
             self.arch = info["arch"]
             self.mpy = info["mpy"]
             self.description = descr = info["board"]
             pos = descr.rfind(" with")
             short_descr = descr[:pos].strip() if pos != -1 else ""
-            if board_name := find_board_id_by_description(descr, short_descr):
+            if board_name := find_board_id(descr, short_descr):
                 self.board = board_name
             else:
                 self.board = "UNKNOWN"
 
     def disconnect(self) -> bool:
         """
         Disconnect from a board.
```

### Comparing `mpflash-0.7.3/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.7.4/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/mpremoteboard/runner.py` & `mpflash-0.7.4/mpflash/mpremoteboard/runner.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/vendor/dfu.py` & `mpflash-0.7.4/mpflash/vendor/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/vendor/pydfu.py` & `mpflash-0.7.4/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/vendor/versions.py` & `mpflash-0.7.4/mpflash/vendor/versions.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/mpflash/worklist.py` & `mpflash-0.7.4/mpflash/worklist.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/pyproject.toml` & `mpflash-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.7.3"
+version = "0.7.4"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
@@ -46,13 +46,12 @@
 pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
 pytest-json-report = "^1.5.0"
 pytest-metadata = ">=2.0.2,<4.0.0"
 pytest-mock = "^3.10.0"
 mock = "^4.0.3"
 distro = "^1.8.0"
 fasteners = "^0.19"
-jsons = "^1.6.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpflash-0.7.3/README.md` & `mpflash-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.3/PKG-INFO` & `mpflash-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.7.3
+Version: 0.7.4
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
```

