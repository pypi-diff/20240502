# Comparing `tmp/flet_contrib_runtime-2024.4.28.2241.tar.gz` & `tmp/flet_contrib_runtime-2024.5.2.1633.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_runtime-2024.4.28.2241.tar", max compression
+gzip compressed data, was "flet_contrib_runtime-2024.5.2.1633.tar", max compression
```

## Comparing `flet_contrib_runtime-2024.4.28.2241.tar` & `flet_contrib_runtime-2024.5.2.1633.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      204 2024-04-28 22:41:13.016649 flet_contrib_runtime-2024.4.28.2241/README.md
--rw-r--r--   0        0        0      702 2024-04-28 22:41:58.692898 flet_contrib_runtime-2024.4.28.2241/pyproject.toml
--rw-r--r--   0        0        0      242 2024-04-28 22:41:13.016649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    15956 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/app.py
--rw-r--r--   0        0        0      252 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0      493 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8684 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc
--rw-r--r--   0        0        0      560 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc
--rw-r--r--   0        0        0     2066 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc
--rw-r--r--   0        0        0     1264 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc
--rw-r--r--   0        0        0      571 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     9278 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1806 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0     7402 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/flet_socket_server.py
--rw-r--r--   0        0        0     2163 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/security/__init__.py
--rw-r--r--   0        0        0     1587 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/uploads.py
--rw-r--r--   0        0        0     4787 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__init__.py
--rw-r--r--   0        0        0     6018 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      743 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc
--rw-r--r--   0        0        0     2719 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc
--rw-r--r--   0        0        0      347 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/once.py
--rw-r--r--   0        0        0     3202 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/patch_index.py
--rw-r--r--   0        0        0      103 2024-04-28 22:41:13.020649 flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 flet_contrib_runtime-2024.4.28.2241/PKG-INFO
+-rw-r--r--   0        0        0      204 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/README.md
+-rw-r--r--   0        0        0      702 2024-05-02 16:33:54.387515 flet_contrib_runtime-2024.5.2.1633/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    15946 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/app.py
+-rw-r--r--   0        0        0      252 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0      500 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8691 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc
+-rw-r--r--   0        0        0      567 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc
+-rw-r--r--   0        0        0     2073 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1271 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc
+-rw-r--r--   0        0        0      578 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     9278 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1806 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0     7402 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/flet_socket_server.py
+-rw-r--r--   0        0        0     2163 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/security/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/uploads.py
+-rw-r--r--   0        0        0     4787 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6025 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      750 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc
+-rw-r--r--   0        0        0     2726 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc
+-rw-r--r--   0        0        0      347 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/once.py
+-rw-r--r--   0        0        0     3202 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/patch_index.py
+-rw-r--r--   0        0        0      103 2024-05-02 16:33:07.119091 flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 flet_contrib_runtime-2024.5.2.1633/PKG-INFO
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/pyproject.toml` & `flet_contrib_runtime-2024.5.2.1633/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-runtime"
-version = "2024.04.28.2241"
+version = "2024.05.02.1633"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-flet-contrib-core = "2024.04.28.2241"
+flet-contrib-core = "2024.05.02.1633"
 oauthlib = "^3.2.2"
 httpx = "^0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/app.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,16 +404,17 @@
                     temp_flet_dir.mkdir(parents=True, exist_ok=True)
                     with zipfile.ZipFile(zip_file, "r") as zip_arch:
                         zip_arch.extractall(str(temp_flet_dir))
                 flet_path = str(temp_flet_dir.joinpath("flet", flet_exe))
         args = [flet_path, page_url, pid_file]
     elif is_macos():
         # build version-specific path to Flet.app
-        #temp_flet_dir = Path.home().joinpath(".flet_contribute", "bin", f"flet-{version.version}")
-        temp_flet_dir = Path.home().joinpath(".flet", "bin", f"flet-0.22.0")
+        #temp_flet_dir = Path.home().joinpath(".flet", "bin", f"flet-0.22.0")
+        temp_flet_dir = Path.home().joinpath(".flet", "bin", f"flet-{version.version}")
+
 
         # check if flet.exe is in FLET_VIEW_PATH (flet developer mode)
         flet_path = os.environ.get("FLET_VIEW_PATH")
         if flet_path:
             logger.info(f"Flet.app is set via FLET_VIEW_PATH: {flet_path}")
             temp_flet_dir = Path(flet_path)
         else:
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 9278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 3e24 0000  a........9)f>$..
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 3e24 0000  a........./f>$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 6d07 5a07 6d08 5a08 0100 6400 6401 6c09  m.Z.m.Z...d.d.l.
 00000070: 5a09 6400 6403 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
@@ -71,473 +71,474 @@
 00000460: 00da 1a5f 4175 7468 6f72 697a 6174 696f  ..._Authorizatio
 00000470: 6e5f 5f61 7379 6e63 5f6c 6f63 6bda 0665  n__async_lock..e
 00000480: 7874 656e 645a 0673 636f 7065 735a 0b75  xtendZ.scopesZ.u
 00000490: 7365 725f 7363 6f70 6573 da06 6170 7065  ser_scopes..appe
 000004a0: 6e64 5a0c 6772 6f75 705f 7363 6f70 6573  ndZ.group_scopes
 000004b0: 2906 da04 7365 6c66 7210 0000 0072 1100  )...selfr....r..
 000004c0: 0000 7212 0000 0072 1300 0000 da01 73a9  ..r....r......s.
-000004d0: 0072 2100 0000 fa64 2f77 6f72 6b73 7061  .r!....d/workspa
+000004d0: 0072 2100 0000 fa6b 2f77 6f72 6b73 7061  .r!....k/workspa
 000004e0: 6365 732f 636f 6e74 7269 6266 6c65 742f  ces/contribflet/
-000004f0: 666c 6574 2f73 646b 2f70 7974 686f 6e2f  flet/sdk/python/
-00000500: 7061 636b 6167 6573 2f66 6c65 742d 7275  packages/flet-ru
-00000510: 6e74 696d 652f 7372 632f 666c 6574 5f72  ntime/src/flet_r
-00000520: 756e 7469 6d65 2f61 7574 682f 6175 7468  untime/auth/auth
-00000530: 6f72 697a 6174 696f 6e2e 7079 da08 5f5f  orization.py..__
-00000540: 696e 6974 5f5f 1500 0000 7322 0000 0000  init__....s"....
-00000550: 0706 0106 0112 0106 0106 0106 0116 0116  ................
-00000560: 0310 0106 010c 010a 010e 0106 010c 010a  ................
-00000570: 017a 1641 7574 686f 7269 7a61 7469 6f6e  .z.Authorization
-00000580: 2e5f 5f69 6e69 745f 5f29 01da 0b73 6176  .__init__)...sav
-00000590: 6564 5f74 6f6b 656e 6302 0000 0000 0000  ed_tokenc.......
-000005a0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000005b0: 0073 2000 0000 7400 a001 7c01 a101 7c00  .s ...t...|...|.
-000005c0: 5f02 7c00 a003 a100 0100 7c00 a004 a100  _.|.......|.....
-000005d0: 0100 6400 5300 7215 0000 0029 0572 0d00  ..d.S.r....).r..
-000005e0: 0000 da09 6672 6f6d 5f6a 736f 6e72 1600  ....from_jsonr..
-000005f0: 0000 da1d 5f41 7574 686f 7269 7a61 7469  ...._Authorizati
-00000600: 6f6e 5f5f 7265 6672 6573 685f 746f 6b65  on__refresh_toke
-00000610: 6eda 255f 4175 7468 6f72 697a 6174 696f  n.%_Authorizatio
-00000620: 6e5f 5f66 6574 6368 5f75 7365 725f 616e  n__fetch_user_an
-00000630: 645f 6772 6f75 7073 a902 721f 0000 0072  d_groups..r....r
-00000640: 2400 0000 7221 0000 0072 2100 0000 7222  $...r!...r!...r"
-00000650: 0000 00da 0f64 6568 7964 7261 7465 5f74  .....dehydrate_t
-00000660: 6f6b 656e 3000 0000 7306 0000 0000 010c  oken0...s.......
-00000670: 0108 017a 1d41 7574 686f 7269 7a61 7469  ...z.Authorizati
-00000680: 6f6e 2e64 6568 7964 7261 7465 5f74 6f6b  on.dehydrate_tok
-00000690: 656e 6302 0000 0000 0000 0000 0000 0002  enc.............
-000006a0: 0000 0003 0000 00c3 0000 0073 2c00 0000  ...........s,...
-000006b0: 7400 a001 7c01 a101 7c00 5f02 7c00 a003  t...|...|._.|...
-000006c0: a100 4900 6400 4800 0100 7c00 a004 a100  ..I.d.H...|.....
-000006d0: 4900 6400 4800 0100 6400 5300 7215 0000  I.d.H...d.S.r...
-000006e0: 0029 0572 0d00 0000 7225 0000 0072 1600  .).r....r%...r..
-000006f0: 0000 da23 5f41 7574 686f 7269 7a61 7469  ...#_Authorizati
-00000700: 6f6e 5f5f 7265 6672 6573 685f 746f 6b65  on__refresh_toke
-00000710: 6e5f 6173 796e 63da 2b5f 4175 7468 6f72  n_async.+_Author
-00000720: 697a 6174 696f 6e5f 5f66 6574 6368 5f75  ization__fetch_u
-00000730: 7365 725f 616e 645f 6772 6f75 7073 5f61  ser_and_groups_a
-00000740: 7379 6e63 7228 0000 0072 2100 0000 7221  syncr(...r!...r!
-00000750: 0000 0072 2200 0000 da15 6465 6879 6472  ...r".....dehydr
-00000760: 6174 655f 746f 6b65 6e5f 6173 796e 6335  ate_token_async5
-00000770: 0000 0073 0600 0000 0001 0c01 0e01 7a23  ...s..........z#
-00000780: 4175 7468 6f72 697a 6174 696f 6e2e 6465  Authorization.de
-00000790: 6879 6472 6174 655f 746f 6b65 6e5f 6173  hydrate_token_as
-000007a0: 796e 6329 0172 1400 0000 6301 0000 0000  ync).r....c.....
-000007b0: 0000 0000 0000 0001 0000 0008 0000 0043  ...............C
-000007c0: 0000 0073 3800 0000 7c00 6a00 8f1e 0100  ...s8...|.j.....
-000007d0: 7c00 a001 a100 0100 7c00 6a02 5700 0200  |.......|.j.W...
-000007e0: 6400 0400 0400 8303 0100 5300 3100 732a  d.........S.1.s*
-000007f0: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
-00000800: 7215 0000 0029 0372 1a00 0000 7226 0000  r....).r....r&..
-00000810: 0072 1600 0000 a901 721f 0000 0072 2100  .r......r....r!.
-00000820: 0000 7221 0000 0072 2200 0000 da05 746f  ..r!...r".....to
-00000830: 6b65 6e3b 0000 0073 0600 0000 0002 0801  ken;...s........
-00000840: 0801 7a13 4175 7468 6f72 697a 6174 696f  ..z.Authorizatio
-00000850: 6e2e 746f 6b65 6e63 0100 0000 0000 0000  n.tokenc........
-00000860: 0000 0000 0100 0000 0900 0000 c300 0000  ................
-00000870: 7352 0000 007c 006a 0034 0049 0064 0048  sR...|.j.4.I.d.H
-00000880: 009a 2a01 007c 00a0 01a1 0049 0064 0048  ..*..|.....I.d.H
-00000890: 0001 007c 006a 0257 0002 0064 0004 0004  ...|.j.W...d....
-000008a0: 0083 0349 0064 0048 0001 0053 0031 0049  ...I.d.H...S.1.I
-000008b0: 0064 0048 0073 4430 0001 0001 0001 0059  .d.H.sD0.......Y
-000008c0: 0001 0064 0053 0072 1500 0000 2903 721c  ...d.S.r....).r.
-000008d0: 0000 0072 2a00 0000 7216 0000 0072 2d00  ...r*...r....r-.
-000008e0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-000008f0: 00da 0b74 6f6b 656e 5f61 7379 6e63 4200  ...token_asyncB.
-00000900: 0000 7306 0000 0000 0210 010e 017a 1941  ..s..........z.A
-00000910: 7574 686f 7269 7a61 7469 6f6e 2e74 6f6b  uthorization.tok
-00000920: 656e 5f61 7379 6e63 6301 0000 0000 0000  en_asyncc.......
-00000930: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00000940: 0073 4c00 0000 7400 a001 6401 a101 7c00  .sL...t...d...|.
-00000950: 5f02 7403 7c00 6a04 6a05 8301 7d01 7c01  _.t.|.j.j...}.|.
-00000960: 6a06 7c00 6a04 6a07 7c00 6a04 6a08 7c00  j.|.j.j.|.j.j.|.
-00000970: 6a09 7c00 6a02 7c00 6a04 6a0a 7c00 6a04  j.|.j.|.j.j.|.j.
-00000980: 6a0b 6402 8d06 7d02 7c02 7c00 6a02 6602  j.d...}.|.|.j.f.
-00000990: 5300 2903 4ee9 1000 0000 2904 7213 0000  S.).N.....).r...
-000009a0: 00da 0573 7461 7465 da0e 636f 6465 5f63  ...state..code_c
-000009b0: 6861 6c6c 656e 6765 da15 636f 6465 5f63  hallenge..code_c
-000009c0: 6861 6c6c 656e 6765 5f6d 6574 686f 6429  hallenge_method)
-000009d0: 0cda 0773 6563 7265 7473 da0d 746f 6b65  ...secrets..toke
-000009e0: 6e5f 7572 6c73 6166 6572 3100 0000 720a  n_urlsafer1...r.
-000009f0: 0000 0072 1000 0000 da09 636c 6965 6e74  ...r......client
-00000a00: 5f69 645a 1370 7265 7061 7265 5f72 6571  _idZ.prepare_req
-00000a10: 7565 7374 5f75 7269 5a16 6175 7468 6f72  uest_uriZ.author
-00000a20: 697a 6174 696f 6e5f 656e 6470 6f69 6e74  ization_endpoint
-00000a30: da0c 7265 6469 7265 6374 5f75 726c 7213  ..redirect_urlr.
-00000a40: 0000 0072 3200 0000 7233 0000 0029 0372  ...r2...r3...).r
-00000a50: 1f00 0000 da06 636c 6965 6e74 da11 6175  ......client..au
-00000a60: 7468 6f72 697a 6174 696f 6e5f 7572 6c72  thorization_urlr
-00000a70: 2100 0000 7221 0000 0072 2200 0000 da16  !...r!...r".....
-00000a80: 6765 745f 6175 7468 6f72 697a 6174 696f  get_authorizatio
-00000a90: 6e5f 6461 7461 4800 0000 7316 0000 0000  n_dataH...s.....
-00000aa0: 010c 010c 0104 0106 0106 0104 0104 0106  ................
-00000ab0: 0106 fa06 087a 2441 7574 686f 7269 7a61  .....z$Authoriza
-00000ac0: 7469 6f6e 2e67 6574 5f61 7574 686f 7269  tion.get_authori
-00000ad0: 7a61 7469 6f6e 5f64 6174 6129 01da 0463  zation_data)...c
-00000ae0: 6f64 6563 0200 0000 0000 0000 0000 0000  odec............
-00000af0: 0600 0000 0800 0000 4300 0000 7378 0000  ........C...sx..
-00000b00: 007c 00a0 007c 01a1 017d 0274 016a 0264  .|...|...}.t.j.d
-00000b10: 0164 028d 018f 4e7d 037c 03a0 037c 02a1  .d....N}.|...|..
-00000b20: 017d 047c 04a0 04a1 0001 0074 057c 006a  .}.|.......t.|.j
-00000b30: 066a 0783 017d 037c 03a0 087c 046a 09a1  .j...}.|...|.j..
-00000b40: 017d 057c 00a0 0a7c 05a1 017c 005f 0b7c  .}.|...|...|._.|
-00000b50: 00a0 0ca1 0001 0057 0064 0004 0004 0083  .......W.d......
-00000b60: 0301 006e 1031 0073 6a30 0001 0001 0001  ...n.1.sj0......
-00000b70: 0059 0001 0064 0053 00a9 034e 5429 015a  .Y...d.S...NT).Z
-00000b80: 1066 6f6c 6c6f 775f 7265 6469 7265 6374  .follow_redirect
-00000b90: 7329 0dda 295f 4175 7468 6f72 697a 6174  s)..)_Authorizat
-00000ba0: 696f 6e5f 5f67 6574 5f72 6571 7565 7374  ion__get_request
-00000bb0: 5f74 6f6b 656e 5f72 6571 7565 7374 da05  _token_request..
-00000bc0: 6874 7470 78da 0643 6c69 656e 74da 0473  httpx..Client..s
-00000bd0: 656e 64da 1072 6169 7365 5f66 6f72 5f73  end..raise_for_s
-00000be0: 7461 7475 7372 0a00 0000 7210 0000 0072  tatusr....r....r
-00000bf0: 3600 0000 da1b 7061 7273 655f 7265 7175  6.....parse_requ
-00000c00: 6573 745f 626f 6479 5f72 6573 706f 6e73  est_body_respons
-00000c10: 65da 0474 6578 74da 1d5f 4175 7468 6f72  e..text.._Author
-00000c20: 697a 6174 696f 6e5f 5f63 6f6e 7665 7274  ization__convert
-00000c30: 5f74 6f6b 656e 7216 0000 0072 2700 0000  _tokenr....r'...
-00000c40: a906 721f 0000 0072 3b00 0000 da03 7265  ..r....r;.....re
-00000c50: 7172 3800 0000 5a04 7265 7370 da01 7472  qr8...Z.resp..tr
-00000c60: 2100 0000 7221 0000 0072 2200 0000 da0d  !...r!...r".....
-00000c70: 7265 7175 6573 745f 746f 6b65 6e55 0000  request_tokenU..
-00000c80: 0073 1000 0000 0001 0a01 0e01 0a01 0801  .s..............
-00000c90: 0c01 0c01 0c01 7a1b 4175 7468 6f72 697a  ......z.Authoriz
-00000ca0: 6174 696f 6e2e 7265 7175 6573 745f 746f  ation.request_to
-00000cb0: 6b65 6e63 0200 0000 0000 0000 0000 0000  kenc............
-00000cc0: 0600 0000 0900 0000 c300 0000 7398 0000  ............s...
-00000cd0: 007c 00a0 007c 01a1 017d 0274 016a 0264  .|...|...}.t.j.d
-00000ce0: 0164 028d 0134 0049 0064 0048 009a 607d  .d...4.I.d.H..`}
-00000cf0: 037c 03a0 037c 02a1 0149 0064 0048 007d  .|...|...I.d.H.}
-00000d00: 047c 04a0 04a1 0001 0074 057c 006a 066a  .|.......t.|.j.j
-00000d10: 0783 017d 037c 03a0 087c 046a 09a1 017d  ...}.|...|.j...}
-00000d20: 057c 00a0 0a7c 05a1 017c 005f 0b7c 00a0  .|...|...|._.|..
-00000d30: 0ca1 0049 0064 0048 0001 0057 0064 0004  ...I.d.H...W.d..
-00000d40: 0004 0083 0349 0064 0048 0001 0071 9431  .....I.d.H...q.1
-00000d50: 0049 0064 0048 0073 8a30 0001 0001 0001  .I.d.H.s.0......
-00000d60: 0059 0001 0064 0053 0072 3c00 0000 290d  .Y...d.S.r<...).
-00000d70: 723d 0000 0072 3e00 0000 da0b 4173 796e  r=...r>.....Asyn
-00000d80: 6343 6c69 656e 7472 4000 0000 7241 0000  cClientr@...rA..
-00000d90: 0072 0a00 0000 7210 0000 0072 3600 0000  .r....r....r6...
-00000da0: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00000db0: 1600 0000 722b 0000 0072 4500 0000 7221  ....r+...rE...r!
-00000dc0: 0000 0072 2100 0000 7222 0000 00da 1372  ...r!...r".....r
-00000dd0: 6571 7565 7374 5f74 6f6b 656e 5f61 7379  equest_token_asy
-00000de0: 6e63 5f00 0000 7310 0000 0000 010a 0116  nc_...s.........
-00000df0: 0110 0108 010c 010c 010c 017a 2141 7574  ...........z!Aut
-00000e00: 686f 7269 7a61 7469 6f6e 2e72 6571 7565  horization.reque
-00000e10: 7374 5f74 6f6b 656e 5f61 7379 6e63 6302  st_token_asyncc.
-00000e20: 0000 0000 0000 0000 0000 0005 0000 0007  ................
-00000e30: 0000 0043 0000 0073 5200 0000 7400 7c00  ...C...sR...t.|.
-00000e40: 6a01 6a02 8301 7d02 7c02 6a03 7c01 7c00  j.j...}.|.j.|.|.
-00000e50: 6a01 6a04 7c00 6a01 6a05 6401 7c00 6a01  j.j.|.j.j.d.|.j.
-00000e60: 6a06 6402 8d05 7d03 7c00 a007 a100 7d04  j.d...}.|.....}.
-00000e70: 6403 7c04 6404 3c00 7408 6a09 6405 7c00  d.|.d.<.t.j.d.|.
-00000e80: 6a01 6a0a 7c03 7c04 6406 8d04 5300 2907  j.j.|.|.d...S.).
-00000e90: 4e54 2905 723b 0000 00da 0c72 6564 6972  NT).r;.....redir
-00000ea0: 6563 745f 7572 69da 0d63 6c69 656e 745f  ect_uri..client_
-00000eb0: 7365 6372 6574 5a11 696e 636c 7564 655f  secretZ.include_
-00000ec0: 636c 6965 6e74 5f69 64da 0d63 6f64 655f  client_id..code_
-00000ed0: 7665 7269 6669 6572 fa21 6170 706c 6963  verifier.!applic
-00000ee0: 6174 696f 6e2f 782d 7777 772d 666f 726d  ation/x-www-form
-00000ef0: 2d75 726c 656e 636f 6465 64fa 0c63 6f6e  -urlencoded..con
-00000f00: 7465 6e74 2d74 7970 65da 0450 4f53 5429  tent-type..POST)
-00000f10: 02da 0763 6f6e 7465 6e74 da07 6865 6164  ...content..head
-00000f20: 6572 7329 0b72 0a00 0000 7210 0000 0072  ers).r....r....r
-00000f30: 3600 0000 5a14 7072 6570 6172 655f 7265  6...Z.prepare_re
-00000f40: 7175 6573 745f 626f 6479 7237 0000 0072  quest_bodyr7...r
-00000f50: 4c00 0000 724d 0000 00da 235f 4175 7468  L...rM....#_Auth
-00000f60: 6f72 697a 6174 696f 6e5f 5f67 6574 5f64  orization__get_d
-00000f70: 6566 6175 6c74 5f68 6561 6465 7273 723e  efault_headersr>
-00000f80: 0000 00da 0752 6571 7565 7374 da0e 746f  .....Request..to
-00000f90: 6b65 6e5f 656e 6470 6f69 6e74 2905 721f  ken_endpoint).r.
-00000fa0: 0000 0072 3b00 0000 7238 0000 00da 0464  ...r;...r8.....d
-00000fb0: 6174 6172 5200 0000 7221 0000 0072 2100  atarR...r!...r!.
-00000fc0: 0000 7222 0000 005a 1b5f 5f67 6574 5f72  ..r"...Z.__get_r
-00000fd0: 6571 7565 7374 5f74 6f6b 656e 5f72 6571  equest_token_req
-00000fe0: 7565 7374 6900 0000 731a 0000 0000 010c  uesti...s.......
-00000ff0: 0104 0102 0106 0106 0102 0106 fb06 0708  ................
-00001000: 0108 0104 010c ff7a 2941 7574 686f 7269  .......z)Authori
-00001010: 7a61 7469 6f6e 2e5f 5f67 6574 5f72 6571  zation.__get_req
-00001020: 7565 7374 5f74 6f6b 656e 5f72 6571 7565  uest_token_reque
-00001030: 7374 6301 0000 0000 0000 0000 0000 0001  stc.............
-00001040: 0000 0003 0000 0043 0000 0073 8200 0000  .......C...s....
-00001050: 7c00 6a00 6400 7501 730e 4a00 8201 7c00  |.j.d.u.s.J...|.
-00001060: 6a01 727e 7c00 6a02 a003 7c00 6a00 6a04  j.r~|.j...|.j.j.
-00001070: a101 7c00 5f05 7c00 6a05 6400 7500 725a  ..|._.|.j.d.u.rZ
-00001080: 7c00 6a02 6a06 6400 7501 725a 7c00 6a02  |.j.j.d.u.rZ|.j.
-00001090: 6a07 6400 7500 7250 7408 6401 8301 8201  j.d.u.rPt.d.....
-000010a0: 7c00 a009 a100 7c00 5f05 7c00 6a0a 727e  |.....|._.|.j.r~
-000010b0: 7c00 6a05 6400 7501 727e 7c00 6a02 a00b  |.j.d.u.r~|.j...
-000010c0: 7c00 6a00 6a04 a101 7c00 6a05 5f0c 6400  |.j.j...|.j._.d.
-000010d0: 5300 a902 4e7a 3d75 7365 725f 6964 5f66  S...Nz=user_id_f
-000010e0: 6e20 6d75 7374 2062 6520 7370 6563 6966  n must be specif
-000010f0: 6965 6420 746f 6f20 6966 2075 7365 725f  ied too if user_
-00001100: 656e 6470 6f69 6e74 2069 7320 6e6f 7420  endpoint is not 
-00001110: 4e6f 6e65 290d 7216 0000 0072 1100 0000  None).r....r....
-00001120: 7210 0000 005a 0b5f 6665 7463 685f 7573  r....Z._fetch_us
-00001130: 6572 da0c 6163 6365 7373 5f74 6f6b 656e  er..access_token
-00001140: 7217 0000 00da 0d75 7365 725f 656e 6470  r......user_endp
-00001150: 6f69 6e74 da0a 7573 6572 5f69 645f 666e  oint..user_id_fn
-00001160: da09 4578 6365 7074 696f 6eda 185f 4175  ..Exception.._Au
-00001170: 7468 6f72 697a 6174 696f 6e5f 5f67 6574  thorization__get
-00001180: 5f75 7365 7272 1200 0000 5a0d 5f66 6574  _userr....Z._fet
-00001190: 6368 5f67 726f 7570 73da 0667 726f 7570  ch_groups..group
-000011a0: 7372 2d00 0000 7221 0000 0072 2100 0000  sr-...r!...r!...
-000011b0: 7222 0000 005a 175f 5f66 6574 6368 5f75  r"...Z.__fetch_u
-000011c0: 7365 725f 616e 645f 6772 6f75 7073 7800  ser_and_groupsx.
-000011d0: 0000 731a 0000 0000 010e 0106 0112 0116  ..s.............
-000011e0: 010c 0102 0102 ff04 030a 0110 0106 0106  ................
-000011f0: ff7a 2541 7574 686f 7269 7a61 7469 6f6e  .z%Authorization
-00001200: 2e5f 5f66 6574 6368 5f75 7365 725f 616e  .__fetch_user_an
-00001210: 645f 6772 6f75 7073 6301 0000 0000 0000  d_groupsc.......
-00001220: 0000 0000 0001 0000 0003 0000 00c3 0000  ................
-00001230: 0073 9400 0000 7c00 6a00 6400 7501 730e  .s....|.j.d.u.s.
-00001240: 4a00 8201 7c00 6a01 7290 7c00 6a02 a003  J...|.j.r.|.j...
-00001250: 7c00 6a00 6a04 a101 4900 6400 4800 7c00  |.j.j...I.d.H.|.
-00001260: 5f05 7c00 6a05 6400 7500 7266 7c00 6a02  _.|.j.d.u.rf|.j.
-00001270: 6a06 6400 7501 7266 7c00 6a02 6a07 6400  j.d.u.rf|.j.j.d.
-00001280: 7500 7256 7408 6401 8301 8201 7c00 a009  u.rVt.d.....|...
-00001290: a100 4900 6400 4800 7c00 5f05 7c00 6a0a  ..I.d.H.|._.|.j.
-000012a0: 7290 7c00 6a05 6400 7501 7290 7c00 6a02  r.|.j.d.u.r.|.j.
-000012b0: a00b 7c00 6a00 6a04 a101 4900 6400 4800  ..|.j.j...I.d.H.
-000012c0: 7c00 6a05 5f0c 6400 5300 7257 0000 0029  |.j._.d.S.rW...)
-000012d0: 0d72 1600 0000 7211 0000 0072 1000 0000  .r....r....r....
-000012e0: 5a11 5f66 6574 6368 5f75 7365 725f 6173  Z._fetch_user_as
-000012f0: 796e 6372 5800 0000 7217 0000 0072 5900  yncrX...r....rY.
-00001300: 0000 725a 0000 0072 5b00 0000 da1e 5f41  ..rZ...r[....._A
-00001310: 7574 686f 7269 7a61 7469 6f6e 5f5f 6765  uthorization__ge
-00001320: 745f 7573 6572 5f61 7379 6e63 7212 0000  t_user_asyncr...
-00001330: 005a 135f 6665 7463 685f 6772 6f75 7073  .Z._fetch_groups
-00001340: 5f61 7379 6e63 725d 0000 0072 2d00 0000  _asyncr]...r-...
-00001350: 7221 0000 0072 2100 0000 7222 0000 005a  r!...r!...r"...Z
-00001360: 1d5f 5f66 6574 6368 5f75 7365 725f 616e  .__fetch_user_an
-00001370: 645f 6772 6f75 7073 5f61 7379 6e63 8700  d_groups_async..
-00001380: 0000 731a 0000 0000 010e 0106 0118 0116  ..s.............
-00001390: 010c 0102 0102 ff04 0310 0110 0106 0106  ................
-000013a0: ff7a 2b41 7574 686f 7269 7a61 7469 6f6e  .z+Authorization
-000013b0: 2e5f 5f66 6574 6368 5f75 7365 725f 616e  .__fetch_user_an
-000013c0: 645f 6772 6f75 7073 5f61 7379 6e63 2901  d_groups_async).
-000013d0: 7247 0000 0063 0200 0000 0000 0000 0000  rG...c..........
-000013e0: 0000 0200 0000 0900 0000 4300 0000 7336  ..........C...s6
-000013f0: 0000 0074 007c 0164 0119 007c 01a0 0164  ...t.|.d...|...d
-00001400: 02a1 017c 01a0 0164 03a1 017c 01a0 0164  ...|...d...|...d
-00001410: 04a1 017c 01a0 0164 05a1 017c 01a0 0164  ...|...d...|...d
-00001420: 06a1 0164 078d 0653 0029 084e 7258 0000  ...d...S.).NrX..
-00001430: 0072 1300 0000 da0a 746f 6b65 6e5f 7479  .r......token_ty
-00001440: 7065 da0a 6578 7069 7265 735f 696e da0a  pe..expires_in..
-00001450: 6578 7069 7265 735f 6174 da0d 7265 6672  expires_at..refr
-00001460: 6573 685f 746f 6b65 6e29 0672 5800 0000  esh_token).rX...
-00001470: 7213 0000 0072 5f00 0000 7260 0000 0072  r....r_...r`...r
-00001480: 6100 0000 7262 0000 0029 0272 0d00 0000  a...rb...).r....
-00001490: da03 6765 7429 0272 1f00 0000 7247 0000  ..get).r....rG..
-000014a0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-000014b0: 5a0f 5f5f 636f 6e76 6572 745f 746f 6b65  Z.__convert_toke
-000014c0: 6e96 0000 0073 1000 0000 0001 0201 0601  n....s..........
-000014d0: 0801 0801 0801 0801 08fa 7a1d 4175 7468  ..........z.Auth
-000014e0: 6f72 697a 6174 696f 6e2e 5f5f 636f 6e76  orization.__conv
-000014f0: 6572 745f 746f 6b65 6e63 0100 0000 0000  ert_tokenc......
-00001500: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-00001510: 0000 7350 0000 007c 00a0 00a1 007d 017c  ..sP...|.....}.|
-00001520: 0172 4c74 016a 0264 0164 028d 018f 247d  .rLt.j.d.d....$}
-00001530: 027c 02a0 037c 01a1 017d 037c 00a0 047c  .|...|...}.|...|
-00001540: 03a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00001550: 006e 1031 0073 4230 0001 0001 0001 0059  .n.1.sB0.......Y
-00001560: 0001 0064 0053 0072 3c00 0000 2905 da29  ...d.S.r<...)..)
-00001570: 5f41 7574 686f 7269 7a61 7469 6f6e 5f5f  _Authorization__
-00001580: 6765 745f 7265 6672 6573 685f 746f 6b65  get_refresh_toke
-00001590: 6e5f 7265 7175 6573 7472 3e00 0000 723f  n_requestr>...r?
-000015a0: 0000 0072 4000 0000 da2e 5f41 7574 686f  ...r@....._Autho
-000015b0: 7269 7a61 7469 6f6e 5f5f 636f 6d70 6c65  rization__comple
-000015c0: 7465 5f72 6566 7265 7368 5f74 6f6b 656e  te_refresh_token
-000015d0: 5f72 6571 7565 7374 a904 721f 0000 005a  _request..r....Z
-000015e0: 0b72 6566 7265 7368 5f72 6571 7238 0000  .refresh_reqr8..
-000015f0: 00da 0c72 6566 7265 7368 5f72 6573 7072  ...refresh_respr
-00001600: 2100 0000 7221 0000 0072 2200 0000 5a0f  !...r!...r"...Z.
-00001610: 5f5f 7265 6672 6573 685f 746f 6b65 6ea0  __refresh_token.
-00001620: 0000 0073 0a00 0000 0001 0801 0401 0e01  ...s............
-00001630: 0a01 7a1d 4175 7468 6f72 697a 6174 696f  ..z.Authorizatio
-00001640: 6e2e 5f5f 7265 6672 6573 685f 746f 6b65  n.__refresh_toke
-00001650: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
-00001660: 0000 0900 0000 c300 0000 736a 0000 007c  ..........sj...|
-00001670: 00a0 00a1 007d 017c 0172 6674 016a 0264  .....}.|.rft.j.d
-00001680: 0164 028d 0134 0049 0064 0048 009a 307d  .d...4.I.d.H..0}
-00001690: 027c 02a0 037c 01a1 0149 0064 0048 007d  .|...|...I.d.H.}
-000016a0: 037c 00a0 047c 03a1 0101 0057 0064 0004  .|...|.....W.d..
-000016b0: 0004 0083 0349 0064 0048 0001 0071 6631  .....I.d.H...qf1
-000016c0: 0049 0064 0048 0073 5c30 0001 0001 0001  .I.d.H.s\0......
-000016d0: 0059 0001 0064 0053 0072 3c00 0000 2905  .Y...d.S.r<...).
-000016e0: 7264 0000 0072 3e00 0000 7249 0000 0072  rd...r>...rI...r
-000016f0: 4000 0000 7265 0000 0072 6600 0000 7221  @...re...rf...r!
-00001700: 0000 0072 2100 0000 7222 0000 005a 155f  ...r!...r"...Z._
-00001710: 5f72 6566 7265 7368 5f74 6f6b 656e 5f61  _refresh_token_a
-00001720: 7379 6e63 a700 0000 730a 0000 0000 0108  sync....s.......
-00001730: 0104 0116 0110 017a 2341 7574 686f 7269  .......z#Authori
-00001740: 7a61 7469 6f6e 2e5f 5f72 6566 7265 7368  zation.__refresh
-00001750: 5f74 6f6b 656e 5f61 7379 6e63 6301 0000  _token_asyncc...
-00001760: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00001770: 0043 0000 0073 9800 0000 7c00 6a00 6400  .C...s....|.j.d.
-00001780: 7500 7332 7c00 6a00 6a01 6400 7500 7332  u.s2|.j.j.d.u.s2
-00001790: 7c00 6a00 6a02 6400 7500 7332 7403 a003  |.j.j.d.u.s2t...
-000017a0: a100 7c00 6a00 6a01 6b00 7236 6400 5300  ..|.j.j.k.r6d.S.
-000017b0: 7c00 6a00 6400 7501 7344 4a00 8201 7404  |.j.d.u.sDJ...t.
-000017c0: 7c00 6a05 6a06 8301 7d01 7c01 6a07 7c00  |.j.j...}.|.j.|.
-000017d0: 6a05 6a06 7c00 6a05 6a08 7c00 6a00 6a02  j.j.|.j.j.|.j.j.
-000017e0: 7c00 6a05 6a09 6401 8d04 7d02 7c00 a00a  |.j.j.d...}.|...
-000017f0: a100 7d03 6402 7c03 6403 3c00 740b 6a0c  ..}.d.|.d.<.t.j.
-00001800: 6404 7c00 6a05 6a0d 7c02 7c03 6405 8d04  d.|.j.j.|.|.d...
-00001810: 5300 2906 4e29 0472 3600 0000 724c 0000  S.).N).r6...rL..
-00001820: 0072 6200 0000 724b 0000 0072 4e00 0000  .rb...rK...rN...
-00001830: 724f 0000 0072 5000 0000 2903 da03 7572  rO...rP...)...ur
-00001840: 6c72 5100 0000 7252 0000 0029 0e72 1600  lrQ...rR...).r..
-00001850: 0000 7261 0000 0072 6200 0000 da04 7469  ..ra...rb.....ti
-00001860: 6d65 720a 0000 0072 1000 0000 7236 0000  mer....r....r6..
-00001870: 005a 1470 7265 7061 7265 5f72 6566 7265  .Z.prepare_refre
-00001880: 7368 5f62 6f64 7972 4c00 0000 7237 0000  sh_bodyrL...r7..
-00001890: 0072 5300 0000 723e 0000 0072 5400 0000  .rS...r>...rT...
-000018a0: 7255 0000 0029 0472 1f00 0000 7238 0000  rU...).r....r8..
-000018b0: 0072 5600 0000 7252 0000 0072 2100 0000  .rV...rR...r!...
-000018c0: 7221 0000 0072 2200 0000 5a1b 5f5f 6765  r!...r"...Z.__ge
-000018d0: 745f 7265 6672 6573 685f 746f 6b65 6e5f  t_refresh_token_
-000018e0: 7265 7175 6573 74ae 0000 0073 2c00 0000  request....s,...
-000018f0: 0002 08ff 0202 0afe 0203 0afd 0204 0efc  ................
-00001900: 0206 0402 0e01 0c01 0401 0601 0601 0601  ................
-00001910: 06fc 0606 0801 0801 0401 0cff 7a29 4175  ............z)Au
-00001920: 7468 6f72 697a 6174 696f 6e2e 5f5f 6765  thorization.__ge
-00001930: 745f 7265 6672 6573 685f 746f 6b65 6e5f  t_refresh_token_
-00001940: 7265 7175 6573 7463 0200 0000 0000 0000  requestc........
-00001950: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
-00001960: 7358 0000 007c 01a0 00a1 0001 007c 006a  sX...|.......|.j
-00001970: 0164 0075 0173 164a 0082 0174 027c 006a  .d.u.s.J...t.|.j
-00001980: 036a 0483 017d 027c 02a0 057c 016a 06a1  .j...}.|...|.j..
-00001990: 017d 037c 03a0 0764 01a1 0164 0075 0072  .}.|...d...d.u.r
-000019a0: 487c 006a 016a 087c 0364 013c 007c 00a0  H|.j.j.|.d.<.|..
-000019b0: 097c 03a1 017c 005f 0164 0053 0029 024e  .|...|._.d.S.).N
-000019c0: 7262 0000 0029 0a72 4100 0000 7216 0000  rb...).rA...r...
-000019d0: 0072 0a00 0000 7210 0000 0072 3600 0000  .r....r....r6...
-000019e0: 7242 0000 0072 4300 0000 7263 0000 0072  rB...rC...rc...r
-000019f0: 6200 0000 7244 0000 0029 0472 1f00 0000  b...rD...).r....
-00001a00: 7267 0000 0072 3800 0000 7247 0000 0072  rg...r8...rG...r
-00001a10: 2100 0000 7221 0000 0072 2200 0000 5a20  !...r!...r"...Z 
-00001a20: 5f5f 636f 6d70 6c65 7465 5f72 6566 7265  __complete_refre
-00001a30: 7368 5f74 6f6b 656e 5f72 6571 7565 7374  sh_token_request
-00001a40: c500 0000 730e 0000 0000 0108 010e 010c  ....s...........
-00001a50: 010c 010e 010c 017a 2e41 7574 686f 7269  .......z.Authori
-00001a60: 7a61 7469 6f6e 2e5f 5f63 6f6d 706c 6574  zation.__complet
-00001a70: 655f 7265 6672 6573 685f 746f 6b65 6e5f  e_refresh_token_
-00001a80: 7265 7175 6573 7463 0100 0000 0000 0000  requestc........
-00001a90: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-00001aa0: 7348 0000 007c 00a0 00a1 007d 0174 01a0  sH...|.....}.t..
-00001ab0: 02a1 008f 247d 027c 02a0 037c 01a1 017d  ....$}.|...|...}
-00001ac0: 037c 00a0 047c 03a1 0157 0002 0064 0004  .|...|...W...d..
-00001ad0: 0004 0083 0301 0053 0031 0073 3a30 0001  .......S.1.s:0..
-00001ae0: 0001 0001 0059 0001 0064 0053 0072 1500  .....Y...d.S.r..
-00001af0: 0000 2905 da20 5f41 7574 686f 7269 7a61  ..).. _Authoriza
-00001b00: 7469 6f6e 5f5f 6765 745f 7573 6572 5f72  tion__get_user_r
-00001b10: 6571 7565 7374 723e 0000 0072 3f00 0000  equestr>...r?...
-00001b20: 7240 0000 00da 255f 4175 7468 6f72 697a  r@....%_Authoriz
-00001b30: 6174 696f 6e5f 5f63 6f6d 706c 6574 655f  ation__complete_
-00001b40: 7573 6572 5f72 6571 7565 7374 a904 721f  user_request..r.
-00001b50: 0000 005a 0875 7365 725f 7265 7172 3800  ...Z.user_reqr8.
-00001b60: 0000 da09 7573 6572 5f72 6573 7072 2100  ....user_respr!.
-00001b70: 0000 7221 0000 0072 2200 0000 5a0a 5f5f  ..r!...r"...Z.__
-00001b80: 6765 745f 7573 6572 ce00 0000 7308 0000  get_user....s...
-00001b90: 0000 0108 010a 010a 017a 1841 7574 686f  .........z.Autho
-00001ba0: 7269 7a61 7469 6f6e 2e5f 5f67 6574 5f75  rization.__get_u
-00001bb0: 7365 7263 0100 0000 0000 0000 0000 0000  serc............
-00001bc0: 0400 0000 0900 0000 c300 0000 7366 0000  ............sf..
-00001bd0: 007c 00a0 00a1 007d 0174 016a 0264 0164  .|.....}.t.j.d.d
-00001be0: 028d 0134 0049 0064 0048 009a 307d 027c  ...4.I.d.H..0}.|
-00001bf0: 02a0 037c 01a1 0149 0064 0048 007d 037c  ...|...I.d.H.}.|
-00001c00: 00a0 047c 03a1 0157 0002 0064 0004 0004  ...|...W...d....
-00001c10: 0083 0349 0064 0048 0001 0053 0031 0049  ...I.d.H...S.1.I
-00001c20: 0064 0048 0073 5830 0001 0001 0001 0059  .d.H.sX0.......Y
-00001c30: 0001 0064 0053 0072 3c00 0000 2905 726a  ...d.S.r<...).rj
-00001c40: 0000 0072 3e00 0000 7249 0000 0072 4000  ...r>...rI...r@.
-00001c50: 0000 726b 0000 0072 6c00 0000 7221 0000  ..rk...rl...r!..
-00001c60: 0072 2100 0000 7222 0000 005a 105f 5f67  .r!...r"...Z.__g
-00001c70: 6574 5f75 7365 725f 6173 796e 63d4 0000  et_user_async...
-00001c80: 0073 0800 0000 0001 0801 1601 1001 7a1e  .s............z.
-00001c90: 4175 7468 6f72 697a 6174 696f 6e2e 5f5f  Authorization.__
-00001ca0: 6765 745f 7573 6572 5f61 7379 6e63 6301  get_user_asyncc.
-00001cb0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00001cc0: 0000 0043 0000 0073 4c00 0000 7c00 6a00  ...C...sL...|.j.
-00001cd0: 6400 7501 730e 4a00 8201 7c00 6a01 6a02  d.u.s.J...|.j.j.
-00001ce0: 6400 7501 731e 4a00 8201 7c00 a003 a100  d.u.s.J...|.....
-00001cf0: 7d01 6401 7c00 6a00 6a04 9b00 9d02 7c01  }.d.|.j.j.....|.
-00001d00: 6402 3c00 7405 6a06 6403 7c00 6a01 6a02  d.<.t.j.d.|.j.j.
-00001d10: 7c01 6404 8d03 5300 2905 4e7a 0742 6561  |.d...S.).Nz.Bea
-00001d20: 7265 7220 720f 0000 005a 0347 4554 2901  rer r....Z.GET).
-00001d30: 7252 0000 0029 0772 2e00 0000 7210 0000  rR...).r....r...
-00001d40: 0072 5900 0000 7253 0000 0072 5800 0000  .rY...rS...rX...
-00001d50: 723e 0000 0072 5400 0000 2902 721f 0000  r>...rT...).r...
-00001d60: 0072 5200 0000 7221 0000 0072 2100 0000  .rR...r!...r!...
-00001d70: 7222 0000 005a 125f 5f67 6574 5f75 7365  r"...Z.__get_use
-00001d80: 725f 7265 7175 6573 74da 0000 0073 0a00  r_request....s..
-00001d90: 0000 0001 0e01 1001 0801 1201 7a20 4175  ............z Au
-00001da0: 7468 6f72 697a 6174 696f 6e2e 5f5f 6765  thorization.__ge
-00001db0: 745f 7573 6572 5f72 6571 7565 7374 6302  t_user_requestc.
-00001dc0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
-00001dd0: 0000 0043 0000 0073 3a00 0000 7c01 a000  ...C...s:...|...
-00001de0: a100 0100 7c00 6a01 6a02 6400 7501 7318  ....|.j.j.d.u.s.
-00001df0: 4a00 8201 7403 a004 7c01 6a05 a101 7d02  J...t...|.j...}.
-00001e00: 7406 7c02 7407 7c00 6a01 a002 7c02 a101  t.|.t.|.j...|...
-00001e10: 8301 8302 5300 7215 0000 0029 0872 4100  ....S.r....).rA.
-00001e20: 0000 7210 0000 0072 5a00 0000 da04 6a73  ..r....rZ.....js
-00001e30: 6f6e da05 6c6f 6164 7372 4300 0000 720e  on..loadsrC...r.
-00001e40: 0000 00da 0373 7472 2903 721f 0000 0072  .....str).r....r
-00001e50: 6d00 0000 5a02 756a 7221 0000 0072 2100  m...Z.ujr!...r!.
-00001e60: 0000 7222 0000 005a 175f 5f63 6f6d 706c  ..r"...Z.__compl
-00001e70: 6574 655f 7573 6572 5f72 6571 7565 7374  ete_user_request
-00001e80: e100 0000 7308 0000 0000 0108 0110 010c  ....s...........
-00001e90: 017a 2541 7574 686f 7269 7a61 7469 6f6e  .z%Authorization
-00001ea0: 2e5f 5f63 6f6d 706c 6574 655f 7573 6572  .__complete_user
-00001eb0: 5f72 6571 7565 7374 6301 0000 0000 0000  _requestc.......
-00001ec0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00001ed0: 0073 0e00 0000 6401 6402 7400 9b00 9d02  .s....d.d.t.....
-00001ee0: 6901 5300 2903 4e7a 0a55 7365 722d 4167  i.S.).Nz.User-Ag
-00001ef0: 656e 747a 0546 6c65 742f 7205 0000 0072  entz.Flet/r....r
-00001f00: 2d00 0000 7221 0000 0072 2100 0000 7222  -...r!...r!...r"
-00001f10: 0000 005a 155f 5f67 6574 5f64 6566 6175  ...Z.__get_defau
-00001f20: 6c74 5f68 6561 6465 7273 e700 0000 7304  lt_headers....s.
-00001f30: 0000 0000 020a ff7a 2341 7574 686f 7269  .......z#Authori
-00001f40: 7a61 7469 6f6e 2e5f 5f67 6574 5f64 6566  zation.__get_def
-00001f50: 6175 6c74 5f68 6561 6465 7273 2901 4e29  ault_headers).N)
-00001f60: 21da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  !..__name__..__m
-00001f70: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001f80: 616d 655f 5f72 0c00 0000 da04 626f 6f6c  ame__r......bool
-00001f90: 7203 0000 0072 0200 0000 7270 0000 0072  r....r....rp...r
-00001fa0: 2300 0000 7229 0000 0072 2c00 0000 da08  #...r)...r,.....
-00001fb0: 7072 6f70 6572 7479 720d 0000 0072 2e00  propertyr....r..
-00001fc0: 0000 722f 0000 0072 0400 0000 723a 0000  ..r/...r....r:..
-00001fd0: 0072 4800 0000 724a 0000 0072 3d00 0000  .rH...rJ...r=...
-00001fe0: 7227 0000 0072 2b00 0000 720b 0000 0072  r'...r+...r....r
-00001ff0: 4400 0000 7226 0000 0072 2a00 0000 7264  D...r&...r*...rd
-00002000: 0000 0072 6500 0000 725c 0000 0072 5e00  ...re...r\...r^.
-00002010: 0000 726a 0000 0072 6b00 0000 7253 0000  ..rj...rk...rS..
-00002020: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
-00002030: 7222 0000 0072 0f00 0000 1400 0000 733c  r"...r........s<
-00002040: 0000 0008 0600 fb02 0202 0102 0102 010a  ................
-00002050: 0102 fa0c 1b0e 050e 0602 0114 0602 0114  ................
-00002060: 0516 0d0e 0a0e 0a0e 0f08 0f08 0f0e 0a08  ................
-00002070: 0708 0708 1708 0908 0608 0608 0708 0672  ...............r
-00002080: 0f00 0000 291c 721b 0000 0072 6e00 0000  ....).r....rn...
-00002090: 7234 0000 0072 1800 0000 7269 0000 00da  r4...r....ri....
-000020a0: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-000020b0: 0072 0400 0000 723e 0000 005a 0c66 6c65  .r....r>...Z.fle
-000020c0: 742e 7665 7273 696f 6e72 0600 0000 da0f  t.versionr......
-000020d0: 666c 6574 5f63 6f72 652e 6c6f 636b 7372  flet_core.locksr
-000020e0: 0700 0000 7208 0000 00da 0f66 6c65 745f  ....r......flet_
-000020f0: 636f 7265 2e75 7469 6c73 7209 0000 005a  core.utilsr....Z
-00002100: 0f6f 6175 7468 6c69 622e 6f61 7574 6832  .oauthlib.oauth2
-00002110: 720a 0000 005a 1e6f 6175 7468 6c69 622e  r....Z.oauthlib.
-00002120: 6f61 7574 6832 2e72 6663 3637 3439 2e74  oauth2.rfc6749.t
-00002130: 6f6b 656e 7372 0b00 0000 da20 666c 6574  okensr..... flet
-00002140: 5f72 756e 7469 6d65 2e61 7574 682e 6f61  _runtime.auth.oa
-00002150: 7574 685f 7072 6f76 6964 6572 720c 0000  uth_providerr...
-00002160: 00da 1d66 6c65 745f 7275 6e74 696d 652e  ...flet_runtime.
-00002170: 6175 7468 2e6f 6175 7468 5f74 6f6b 656e  auth.oauth_token
-00002180: 720d 0000 00da 1666 6c65 745f 7275 6e74  r......flet_runt
-00002190: 696d 652e 6175 7468 2e75 7365 7272 0e00  ime.auth.userr..
-000021a0: 0000 720f 0000 0072 2100 0000 7221 0000  ..r....r!...r!..
-000021b0: 0072 2100 0000 7222 0000 00da 083c 6d6f  .r!...r".....<mo
-000021c0: 6475 6c65 3e01 0000 0073 1e00 0000 0801  dule>....s......
-000021d0: 0801 0801 0801 0801 1402 0801 0c01 1001  ................
-000021e0: 0c01 0c01 0c02 0c01 0c01 0c03            ............
+000004f0: 666c 6574 636f 6e74 7269 622f 7364 6b2f  fletcontrib/sdk/
+00000500: 7079 7468 6f6e 2f70 6163 6b61 6765 732f  python/packages/
+00000510: 666c 6574 2d72 756e 7469 6d65 2f73 7263  flet-runtime/src
+00000520: 2f66 6c65 745f 7275 6e74 696d 652f 6175  /flet_runtime/au
+00000530: 7468 2f61 7574 686f 7269 7a61 7469 6f6e  th/authorization
+00000540: 2e70 79da 085f 5f69 6e69 745f 5f15 0000  .py..__init__...
+00000550: 0073 2200 0000 0007 0601 0601 1201 0601  .s".............
+00000560: 0601 0601 1601 1603 1001 0601 0c01 0a01  ................
+00000570: 0e01 0601 0c01 0a01 7a16 4175 7468 6f72  ........z.Author
+00000580: 697a 6174 696f 6e2e 5f5f 696e 6974 5f5f  ization.__init__
+00000590: 2901 da0b 7361 7665 645f 746f 6b65 6e63  )...saved_tokenc
+000005a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000005b0: 0300 0000 4300 0000 7320 0000 0074 00a0  ....C...s ...t..
+000005c0: 017c 01a1 017c 005f 027c 00a0 03a1 0001  .|...|._.|......
+000005d0: 007c 00a0 04a1 0001 0064 0053 0072 1500  .|.......d.S.r..
+000005e0: 0000 2905 720d 0000 00da 0966 726f 6d5f  ..).r......from_
+000005f0: 6a73 6f6e 7216 0000 00da 1d5f 4175 7468  jsonr......_Auth
+00000600: 6f72 697a 6174 696f 6e5f 5f72 6566 7265  orization__refre
+00000610: 7368 5f74 6f6b 656e da25 5f41 7574 686f  sh_token.%_Autho
+00000620: 7269 7a61 7469 6f6e 5f5f 6665 7463 685f  rization__fetch_
+00000630: 7573 6572 5f61 6e64 5f67 726f 7570 73a9  user_and_groups.
+00000640: 0272 1f00 0000 7224 0000 0072 2100 0000  .r....r$...r!...
+00000650: 7221 0000 0072 2200 0000 da0f 6465 6879  r!...r".....dehy
+00000660: 6472 6174 655f 746f 6b65 6e30 0000 0073  drate_token0...s
+00000670: 0600 0000 0001 0c01 0801 7a1d 4175 7468  ..........z.Auth
+00000680: 6f72 697a 6174 696f 6e2e 6465 6879 6472  orization.dehydr
+00000690: 6174 655f 746f 6b65 6e63 0200 0000 0000  ate_tokenc......
+000006a0: 0000 0000 0000 0200 0000 0300 0000 c300  ................
+000006b0: 0000 732c 0000 0074 00a0 017c 01a1 017c  ..s,...t...|...|
+000006c0: 005f 027c 00a0 03a1 0049 0064 0048 0001  ._.|.....I.d.H..
+000006d0: 007c 00a0 04a1 0049 0064 0048 0001 0064  .|.....I.d.H...d
+000006e0: 0053 0072 1500 0000 2905 720d 0000 0072  .S.r....).r....r
+000006f0: 2500 0000 7216 0000 00da 235f 4175 7468  %...r.....#_Auth
+00000700: 6f72 697a 6174 696f 6e5f 5f72 6566 7265  orization__refre
+00000710: 7368 5f74 6f6b 656e 5f61 7379 6e63 da2b  sh_token_async.+
+00000720: 5f41 7574 686f 7269 7a61 7469 6f6e 5f5f  _Authorization__
+00000730: 6665 7463 685f 7573 6572 5f61 6e64 5f67  fetch_user_and_g
+00000740: 726f 7570 735f 6173 796e 6372 2800 0000  roups_asyncr(...
+00000750: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00000760: 1564 6568 7964 7261 7465 5f74 6f6b 656e  .dehydrate_token
+00000770: 5f61 7379 6e63 3500 0000 7306 0000 0000  _async5...s.....
+00000780: 010c 010e 017a 2341 7574 686f 7269 7a61  .....z#Authoriza
+00000790: 7469 6f6e 2e64 6568 7964 7261 7465 5f74  tion.dehydrate_t
+000007a0: 6f6b 656e 5f61 7379 6e63 2901 7214 0000  oken_async).r...
+000007b0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+000007c0: 0000 0800 0000 4300 0000 7338 0000 007c  ......C...s8...|
+000007d0: 006a 008f 1e01 007c 00a0 01a1 0001 007c  .j.....|.......|
+000007e0: 006a 0257 0002 0064 0004 0004 0083 0301  .j.W...d........
+000007f0: 0053 0031 0073 2a30 0001 0001 0001 0059  .S.1.s*0.......Y
+00000800: 0001 0064 0053 0072 1500 0000 2903 721a  ...d.S.r....).r.
+00000810: 0000 0072 2600 0000 7216 0000 00a9 0172  ...r&...r......r
+00000820: 1f00 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00000830: 0000 00da 0574 6f6b 656e 3b00 0000 7306  .....token;...s.
+00000840: 0000 0000 0208 0108 017a 1341 7574 686f  .........z.Autho
+00000850: 7269 7a61 7469 6f6e 2e74 6f6b 656e 6301  rization.tokenc.
+00000860: 0000 0000 0000 0000 0000 0001 0000 0009  ................
+00000870: 0000 00c3 0000 0073 5200 0000 7c00 6a00  .......sR...|.j.
+00000880: 3400 4900 6400 4800 9a2a 0100 7c00 a001  4.I.d.H..*..|...
+00000890: a100 4900 6400 4800 0100 7c00 6a02 5700  ..I.d.H...|.j.W.
+000008a0: 0200 6400 0400 0400 8303 4900 6400 4800  ..d.......I.d.H.
+000008b0: 0100 5300 3100 4900 6400 4800 7344 3000  ..S.1.I.d.H.sD0.
+000008c0: 0100 0100 0100 5900 0100 6400 5300 7215  ......Y...d.S.r.
+000008d0: 0000 0029 0372 1c00 0000 722a 0000 0072  ...).r....r*...r
+000008e0: 1600 0000 722d 0000 0072 2100 0000 7221  ....r-...r!...r!
+000008f0: 0000 0072 2200 0000 da0b 746f 6b65 6e5f  ...r".....token_
+00000900: 6173 796e 6342 0000 0073 0600 0000 0002  asyncB...s......
+00000910: 1001 0e01 7a19 4175 7468 6f72 697a 6174  ....z.Authorizat
+00000920: 696f 6e2e 746f 6b65 6e5f 6173 796e 6363  ion.token_asyncc
+00000930: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00000940: 0800 0000 4300 0000 734c 0000 0074 00a0  ....C...sL...t..
+00000950: 0164 01a1 017c 005f 0274 037c 006a 046a  .d...|._.t.|.j.j
+00000960: 0583 017d 017c 016a 067c 006a 046a 077c  ...}.|.j.|.j.j.|
+00000970: 006a 046a 087c 006a 097c 006a 027c 006a  .j.j.|.j.|.j.|.j
+00000980: 046a 0a7c 006a 046a 0b64 028d 067d 027c  .j.|.j.j.d...}.|
+00000990: 027c 006a 0266 0253 0029 034e e910 0000  .|.j.f.S.).N....
+000009a0: 0029 0472 1300 0000 da05 7374 6174 65da  .).r......state.
+000009b0: 0e63 6f64 655f 6368 616c 6c65 6e67 65da  .code_challenge.
+000009c0: 1563 6f64 655f 6368 616c 6c65 6e67 655f  .code_challenge_
+000009d0: 6d65 7468 6f64 290c da07 7365 6372 6574  method)...secret
+000009e0: 73da 0d74 6f6b 656e 5f75 726c 7361 6665  s..token_urlsafe
+000009f0: 7231 0000 0072 0a00 0000 7210 0000 00da  r1...r....r.....
+00000a00: 0963 6c69 656e 745f 6964 5a13 7072 6570  .client_idZ.prep
+00000a10: 6172 655f 7265 7175 6573 745f 7572 695a  are_request_uriZ
+00000a20: 1661 7574 686f 7269 7a61 7469 6f6e 5f65  .authorization_e
+00000a30: 6e64 706f 696e 74da 0c72 6564 6972 6563  ndpoint..redirec
+00000a40: 745f 7572 6c72 1300 0000 7232 0000 0072  t_urlr....r2...r
+00000a50: 3300 0000 2903 721f 0000 00da 0663 6c69  3...).r......cli
+00000a60: 656e 74da 1161 7574 686f 7269 7a61 7469  ent..authorizati
+00000a70: 6f6e 5f75 726c 7221 0000 0072 2100 0000  on_urlr!...r!...
+00000a80: 7222 0000 00da 1667 6574 5f61 7574 686f  r".....get_autho
+00000a90: 7269 7a61 7469 6f6e 5f64 6174 6148 0000  rization_dataH..
+00000aa0: 0073 1600 0000 0001 0c01 0c01 0401 0601  .s..............
+00000ab0: 0601 0401 0401 0601 06fa 0608 7a24 4175  ............z$Au
+00000ac0: 7468 6f72 697a 6174 696f 6e2e 6765 745f  thorization.get_
+00000ad0: 6175 7468 6f72 697a 6174 696f 6e5f 6461  authorization_da
+00000ae0: 7461 2901 da04 636f 6465 6302 0000 0000  ta)...codec.....
+00000af0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00000b00: 0000 0073 7800 0000 7c00 a000 7c01 a101  ...sx...|...|...
+00000b10: 7d02 7401 6a02 6401 6402 8d01 8f4e 7d03  }.t.j.d.d....N}.
+00000b20: 7c03 a003 7c02 a101 7d04 7c04 a004 a100  |...|...}.|.....
+00000b30: 0100 7405 7c00 6a06 6a07 8301 7d03 7c03  ..t.|.j.j...}.|.
+00000b40: a008 7c04 6a09 a101 7d05 7c00 a00a 7c05  ..|.j...}.|...|.
+00000b50: a101 7c00 5f0b 7c00 a00c a100 0100 5700  ..|._.|.......W.
+00000b60: 6400 0400 0400 8303 0100 6e10 3100 736a  d.........n.1.sj
+00000b70: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00000b80: a903 4e54 2901 5a10 666f 6c6c 6f77 5f72  ..NT).Z.follow_r
+00000b90: 6564 6972 6563 7473 290d da29 5f41 7574  edirects)..)_Aut
+00000ba0: 686f 7269 7a61 7469 6f6e 5f5f 6765 745f  horization__get_
+00000bb0: 7265 7175 6573 745f 746f 6b65 6e5f 7265  request_token_re
+00000bc0: 7175 6573 74da 0568 7474 7078 da06 436c  quest..httpx..Cl
+00000bd0: 6965 6e74 da04 7365 6e64 da10 7261 6973  ient..send..rais
+00000be0: 655f 666f 725f 7374 6174 7573 720a 0000  e_for_statusr...
+00000bf0: 0072 1000 0000 7236 0000 00da 1b70 6172  .r....r6.....par
+00000c00: 7365 5f72 6571 7565 7374 5f62 6f64 795f  se_request_body_
+00000c10: 7265 7370 6f6e 7365 da04 7465 7874 da1d  response..text..
+00000c20: 5f41 7574 686f 7269 7a61 7469 6f6e 5f5f  _Authorization__
+00000c30: 636f 6e76 6572 745f 746f 6b65 6e72 1600  convert_tokenr..
+00000c40: 0000 7227 0000 00a9 0672 1f00 0000 723b  ..r'.....r....r;
+00000c50: 0000 00da 0372 6571 7238 0000 005a 0472  .....reqr8...Z.r
+00000c60: 6573 70da 0174 7221 0000 0072 2100 0000  esp..tr!...r!...
+00000c70: 7222 0000 00da 0d72 6571 7565 7374 5f74  r".....request_t
+00000c80: 6f6b 656e 5500 0000 7310 0000 0000 010a  okenU...s.......
+00000c90: 010e 010a 0108 010c 010c 010c 017a 1b41  .............z.A
+00000ca0: 7574 686f 7269 7a61 7469 6f6e 2e72 6571  uthorization.req
+00000cb0: 7565 7374 5f74 6f6b 656e 6302 0000 0000  uest_tokenc.....
+00000cc0: 0000 0000 0000 0006 0000 0009 0000 00c3  ................
+00000cd0: 0000 0073 9800 0000 7c00 a000 7c01 a101  ...s....|...|...
+00000ce0: 7d02 7401 6a02 6401 6402 8d01 3400 4900  }.t.j.d.d...4.I.
+00000cf0: 6400 4800 9a60 7d03 7c03 a003 7c02 a101  d.H..`}.|...|...
+00000d00: 4900 6400 4800 7d04 7c04 a004 a100 0100  I.d.H.}.|.......
+00000d10: 7405 7c00 6a06 6a07 8301 7d03 7c03 a008  t.|.j.j...}.|...
+00000d20: 7c04 6a09 a101 7d05 7c00 a00a 7c05 a101  |.j...}.|...|...
+00000d30: 7c00 5f0b 7c00 a00c a100 4900 6400 4800  |._.|.....I.d.H.
+00000d40: 0100 5700 6400 0400 0400 8303 4900 6400  ..W.d.......I.d.
+00000d50: 4800 0100 7194 3100 4900 6400 4800 738a  H...q.1.I.d.H.s.
+00000d60: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00000d70: 723c 0000 0029 0d72 3d00 0000 723e 0000  r<...).r=...r>..
+00000d80: 00da 0b41 7379 6e63 436c 6965 6e74 7240  ...AsyncClientr@
+00000d90: 0000 0072 4100 0000 720a 0000 0072 1000  ...rA...r....r..
+00000da0: 0000 7236 0000 0072 4200 0000 7243 0000  ..r6...rB...rC..
+00000db0: 0072 4400 0000 7216 0000 0072 2b00 0000  .rD...r....r+...
+00000dc0: 7245 0000 0072 2100 0000 7221 0000 0072  rE...r!...r!...r
+00000dd0: 2200 0000 da13 7265 7175 6573 745f 746f  ".....request_to
+00000de0: 6b65 6e5f 6173 796e 635f 0000 0073 1000  ken_async_...s..
+00000df0: 0000 0001 0a01 1601 1001 0801 0c01 0c01  ................
+00000e00: 0c01 7a21 4175 7468 6f72 697a 6174 696f  ..z!Authorizatio
+00000e10: 6e2e 7265 7175 6573 745f 746f 6b65 6e5f  n.request_token_
+00000e20: 6173 796e 6363 0200 0000 0000 0000 0000  asyncc..........
+00000e30: 0000 0500 0000 0700 0000 4300 0000 7352  ..........C...sR
+00000e40: 0000 0074 007c 006a 016a 0283 017d 027c  ...t.|.j.j...}.|
+00000e50: 026a 037c 017c 006a 016a 047c 006a 016a  .j.|.|.j.j.|.j.j
+00000e60: 0564 017c 006a 016a 0664 028d 057d 037c  .d.|.j.j.d...}.|
+00000e70: 00a0 07a1 007d 0464 037c 0464 043c 0074  .....}.d.|.d.<.t
+00000e80: 086a 0964 057c 006a 016a 0a7c 037c 0464  .j.d.|.j.j.|.|.d
+00000e90: 068d 0453 0029 074e 5429 0572 3b00 0000  ...S.).NT).r;...
+00000ea0: da0c 7265 6469 7265 6374 5f75 7269 da0d  ..redirect_uri..
+00000eb0: 636c 6965 6e74 5f73 6563 7265 745a 1169  client_secretZ.i
+00000ec0: 6e63 6c75 6465 5f63 6c69 656e 745f 6964  nclude_client_id
+00000ed0: da0d 636f 6465 5f76 6572 6966 6965 72fa  ..code_verifier.
+00000ee0: 2161 7070 6c69 6361 7469 6f6e 2f78 2d77  !application/x-w
+00000ef0: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
+00000f00: 6564 fa0c 636f 6e74 656e 742d 7479 7065  ed..content-type
+00000f10: da04 504f 5354 2902 da07 636f 6e74 656e  ..POST)...conten
+00000f20: 74da 0768 6561 6465 7273 290b 720a 0000  t..headers).r...
+00000f30: 0072 1000 0000 7236 0000 005a 1470 7265  .r....r6...Z.pre
+00000f40: 7061 7265 5f72 6571 7565 7374 5f62 6f64  pare_request_bod
+00000f50: 7972 3700 0000 724c 0000 0072 4d00 0000  yr7...rL...rM...
+00000f60: da23 5f41 7574 686f 7269 7a61 7469 6f6e  .#_Authorization
+00000f70: 5f5f 6765 745f 6465 6661 756c 745f 6865  __get_default_he
+00000f80: 6164 6572 7372 3e00 0000 da07 5265 7175  adersr>.....Requ
+00000f90: 6573 74da 0e74 6f6b 656e 5f65 6e64 706f  est..token_endpo
+00000fa0: 696e 7429 0572 1f00 0000 723b 0000 0072  int).r....r;...r
+00000fb0: 3800 0000 da04 6461 7461 7252 0000 0072  8.....datarR...r
+00000fc0: 2100 0000 7221 0000 0072 2200 0000 5a1b  !...r!...r"...Z.
+00000fd0: 5f5f 6765 745f 7265 7175 6573 745f 746f  __get_request_to
+00000fe0: 6b65 6e5f 7265 7175 6573 7469 0000 0073  ken_requesti...s
+00000ff0: 1a00 0000 0001 0c01 0401 0201 0601 0601  ................
+00001000: 0201 06fb 0607 0801 0801 0401 0cff 7a29  ..............z)
+00001010: 4175 7468 6f72 697a 6174 696f 6e2e 5f5f  Authorization.__
+00001020: 6765 745f 7265 7175 6573 745f 746f 6b65  get_request_toke
+00001030: 6e5f 7265 7175 6573 7463 0100 0000 0000  n_requestc......
+00001040: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001050: 0000 7382 0000 007c 006a 0064 0075 0173  ..s....|.j.d.u.s
+00001060: 0e4a 0082 017c 006a 0172 7e7c 006a 02a0  .J...|.j.r~|.j..
+00001070: 037c 006a 006a 04a1 017c 005f 057c 006a  .|.j.j...|._.|.j
+00001080: 0564 0075 0072 5a7c 006a 026a 0664 0075  .d.u.rZ|.j.j.d.u
+00001090: 0172 5a7c 006a 026a 0764 0075 0072 5074  .rZ|.j.j.d.u.rPt
+000010a0: 0864 0183 0182 017c 00a0 09a1 007c 005f  .d.....|.....|._
+000010b0: 057c 006a 0a72 7e7c 006a 0564 0075 0172  .|.j.r~|.j.d.u.r
+000010c0: 7e7c 006a 02a0 0b7c 006a 006a 04a1 017c  ~|.j...|.j.j...|
+000010d0: 006a 055f 0c64 0053 00a9 024e 7a3d 7573  .j._.d.S...Nz=us
+000010e0: 6572 5f69 645f 666e 206d 7573 7420 6265  er_id_fn must be
+000010f0: 2073 7065 6369 6669 6564 2074 6f6f 2069   specified too i
+00001100: 6620 7573 6572 5f65 6e64 706f 696e 7420  f user_endpoint 
+00001110: 6973 206e 6f74 204e 6f6e 6529 0d72 1600  is not None).r..
+00001120: 0000 7211 0000 0072 1000 0000 5a0b 5f66  ..r....r....Z._f
+00001130: 6574 6368 5f75 7365 72da 0c61 6363 6573  etch_user..acces
+00001140: 735f 746f 6b65 6e72 1700 0000 da0d 7573  s_tokenr......us
+00001150: 6572 5f65 6e64 706f 696e 74da 0a75 7365  er_endpoint..use
+00001160: 725f 6964 5f66 6eda 0945 7863 6570 7469  r_id_fn..Excepti
+00001170: 6f6e da18 5f41 7574 686f 7269 7a61 7469  on.._Authorizati
+00001180: 6f6e 5f5f 6765 745f 7573 6572 7212 0000  on__get_userr...
+00001190: 005a 0d5f 6665 7463 685f 6772 6f75 7073  .Z._fetch_groups
+000011a0: da06 6772 6f75 7073 722d 0000 0072 2100  ..groupsr-...r!.
+000011b0: 0000 7221 0000 0072 2200 0000 5a17 5f5f  ..r!...r"...Z.__
+000011c0: 6665 7463 685f 7573 6572 5f61 6e64 5f67  fetch_user_and_g
+000011d0: 726f 7570 7378 0000 0073 1a00 0000 0001  roupsx...s......
+000011e0: 0e01 0601 1201 1601 0c01 0201 02ff 0403  ................
+000011f0: 0a01 1001 0601 06ff 7a25 4175 7468 6f72  ........z%Author
+00001200: 697a 6174 696f 6e2e 5f5f 6665 7463 685f  ization.__fetch_
+00001210: 7573 6572 5f61 6e64 5f67 726f 7570 7363  user_and_groupsc
+00001220: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001230: 0300 0000 c300 0000 7394 0000 007c 006a  ........s....|.j
+00001240: 0064 0075 0173 0e4a 0082 017c 006a 0172  .d.u.s.J...|.j.r
+00001250: 907c 006a 02a0 037c 006a 006a 04a1 0149  .|.j...|.j.j...I
+00001260: 0064 0048 007c 005f 057c 006a 0564 0075  .d.H.|._.|.j.d.u
+00001270: 0072 667c 006a 026a 0664 0075 0172 667c  .rf|.j.j.d.u.rf|
+00001280: 006a 026a 0764 0075 0072 5674 0864 0183  .j.j.d.u.rVt.d..
+00001290: 0182 017c 00a0 09a1 0049 0064 0048 007c  ...|.....I.d.H.|
+000012a0: 005f 057c 006a 0a72 907c 006a 0564 0075  ._.|.j.r.|.j.d.u
+000012b0: 0172 907c 006a 02a0 0b7c 006a 006a 04a1  .r.|.j...|.j.j..
+000012c0: 0149 0064 0048 007c 006a 055f 0c64 0053  .I.d.H.|.j._.d.S
+000012d0: 0072 5700 0000 290d 7216 0000 0072 1100  .rW...).r....r..
+000012e0: 0000 7210 0000 005a 115f 6665 7463 685f  ..r....Z._fetch_
+000012f0: 7573 6572 5f61 7379 6e63 7258 0000 0072  user_asyncrX...r
+00001300: 1700 0000 7259 0000 0072 5a00 0000 725b  ....rY...rZ...r[
+00001310: 0000 00da 1e5f 4175 7468 6f72 697a 6174  ....._Authorizat
+00001320: 696f 6e5f 5f67 6574 5f75 7365 725f 6173  ion__get_user_as
+00001330: 796e 6372 1200 0000 5a13 5f66 6574 6368  yncr....Z._fetch
+00001340: 5f67 726f 7570 735f 6173 796e 6372 5d00  _groups_asyncr].
+00001350: 0000 722d 0000 0072 2100 0000 7221 0000  ..r-...r!...r!..
+00001360: 0072 2200 0000 5a1d 5f5f 6665 7463 685f  .r"...Z.__fetch_
+00001370: 7573 6572 5f61 6e64 5f67 726f 7570 735f  user_and_groups_
+00001380: 6173 796e 6387 0000 0073 1a00 0000 0001  async....s......
+00001390: 0e01 0601 1801 1601 0c01 0201 02ff 0403  ................
+000013a0: 1001 1001 0601 06ff 7a2b 4175 7468 6f72  ........z+Author
+000013b0: 697a 6174 696f 6e2e 5f5f 6665 7463 685f  ization.__fetch_
+000013c0: 7573 6572 5f61 6e64 5f67 726f 7570 735f  user_and_groups_
+000013d0: 6173 796e 6329 0172 4700 0000 6302 0000  async).rG...c...
+000013e0: 0000 0000 0000 0000 0002 0000 0009 0000  ................
+000013f0: 0043 0000 0073 3600 0000 7400 7c01 6401  .C...s6...t.|.d.
+00001400: 1900 7c01 a001 6402 a101 7c01 a001 6403  ..|...d...|...d.
+00001410: a101 7c01 a001 6404 a101 7c01 a001 6405  ..|...d...|...d.
+00001420: a101 7c01 a001 6406 a101 6407 8d06 5300  ..|...d...d...S.
+00001430: 2908 4e72 5800 0000 7213 0000 00da 0a74  ).NrX...r......t
+00001440: 6f6b 656e 5f74 7970 65da 0a65 7870 6972  oken_type..expir
+00001450: 6573 5f69 6eda 0a65 7870 6972 6573 5f61  es_in..expires_a
+00001460: 74da 0d72 6566 7265 7368 5f74 6f6b 656e  t..refresh_token
+00001470: 2906 7258 0000 0072 1300 0000 725f 0000  ).rX...r....r_..
+00001480: 0072 6000 0000 7261 0000 0072 6200 0000  .r`...ra...rb...
+00001490: 2902 720d 0000 00da 0367 6574 2902 721f  ).r......get).r.
+000014a0: 0000 0072 4700 0000 7221 0000 0072 2100  ...rG...r!...r!.
+000014b0: 0000 7222 0000 005a 0f5f 5f63 6f6e 7665  ..r"...Z.__conve
+000014c0: 7274 5f74 6f6b 656e 9600 0000 7310 0000  rt_token....s...
+000014d0: 0000 0102 0106 0108 0108 0108 0108 0108  ................
+000014e0: fa7a 1d41 7574 686f 7269 7a61 7469 6f6e  .z.Authorization
+000014f0: 2e5f 5f63 6f6e 7665 7274 5f74 6f6b 656e  .__convert_token
+00001500: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00001510: 0008 0000 0043 0000 0073 5000 0000 7c00  .....C...sP...|.
+00001520: a000 a100 7d01 7c01 724c 7401 6a02 6401  ....}.|.rLt.j.d.
+00001530: 6402 8d01 8f24 7d02 7c02 a003 7c01 a101  d....$}.|...|...
+00001540: 7d03 7c00 a004 7c03 a101 0100 5700 6400  }.|...|.....W.d.
+00001550: 0400 0400 8303 0100 6e10 3100 7342 3000  ........n.1.sB0.
+00001560: 0100 0100 0100 5900 0100 6400 5300 723c  ......Y...d.S.r<
+00001570: 0000 0029 05da 295f 4175 7468 6f72 697a  ...)..)_Authoriz
+00001580: 6174 696f 6e5f 5f67 6574 5f72 6566 7265  ation__get_refre
+00001590: 7368 5f74 6f6b 656e 5f72 6571 7565 7374  sh_token_request
+000015a0: 723e 0000 0072 3f00 0000 7240 0000 00da  r>...r?...r@....
+000015b0: 2e5f 4175 7468 6f72 697a 6174 696f 6e5f  ._Authorization_
+000015c0: 5f63 6f6d 706c 6574 655f 7265 6672 6573  _complete_refres
+000015d0: 685f 746f 6b65 6e5f 7265 7175 6573 74a9  h_token_request.
+000015e0: 0472 1f00 0000 5a0b 7265 6672 6573 685f  .r....Z.refresh_
+000015f0: 7265 7172 3800 0000 da0c 7265 6672 6573  reqr8.....refres
+00001600: 685f 7265 7370 7221 0000 0072 2100 0000  h_respr!...r!...
+00001610: 7222 0000 005a 0f5f 5f72 6566 7265 7368  r"...Z.__refresh
+00001620: 5f74 6f6b 656e a000 0000 730a 0000 0000  _token....s.....
+00001630: 0108 0104 010e 010a 017a 1d41 7574 686f  .........z.Autho
+00001640: 7269 7a61 7469 6f6e 2e5f 5f72 6566 7265  rization.__refre
+00001650: 7368 5f74 6f6b 656e 6301 0000 0000 0000  sh_tokenc.......
+00001660: 0000 0000 0004 0000 0009 0000 00c3 0000  ................
+00001670: 0073 6a00 0000 7c00 a000 a100 7d01 7c01  .sj...|.....}.|.
+00001680: 7266 7401 6a02 6401 6402 8d01 3400 4900  rft.j.d.d...4.I.
+00001690: 6400 4800 9a30 7d02 7c02 a003 7c01 a101  d.H..0}.|...|...
+000016a0: 4900 6400 4800 7d03 7c00 a004 7c03 a101  I.d.H.}.|...|...
+000016b0: 0100 5700 6400 0400 0400 8303 4900 6400  ..W.d.......I.d.
+000016c0: 4800 0100 7166 3100 4900 6400 4800 735c  H...qf1.I.d.H.s\
+000016d0: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+000016e0: 723c 0000 0029 0572 6400 0000 723e 0000  r<...).rd...r>..
+000016f0: 0072 4900 0000 7240 0000 0072 6500 0000  .rI...r@...re...
+00001700: 7266 0000 0072 2100 0000 7221 0000 0072  rf...r!...r!...r
+00001710: 2200 0000 5a15 5f5f 7265 6672 6573 685f  "...Z.__refresh_
+00001720: 746f 6b65 6e5f 6173 796e 63a7 0000 0073  token_async....s
+00001730: 0a00 0000 0001 0801 0401 1601 1001 7a23  ..............z#
+00001740: 4175 7468 6f72 697a 6174 696f 6e2e 5f5f  Authorization.__
+00001750: 7265 6672 6573 685f 746f 6b65 6e5f 6173  refresh_token_as
+00001760: 796e 6363 0100 0000 0000 0000 0000 0000  yncc............
+00001770: 0400 0000 0600 0000 4300 0000 7398 0000  ........C...s...
+00001780: 007c 006a 0064 0075 0073 327c 006a 006a  .|.j.d.u.s2|.j.j
+00001790: 0164 0075 0073 327c 006a 006a 0264 0075  .d.u.s2|.j.j.d.u
+000017a0: 0073 3274 03a0 03a1 007c 006a 006a 016b  .s2t.....|.j.j.k
+000017b0: 0072 3664 0053 007c 006a 0064 0075 0173  .r6d.S.|.j.d.u.s
+000017c0: 444a 0082 0174 047c 006a 056a 0683 017d  DJ...t.|.j.j...}
+000017d0: 017c 016a 077c 006a 056a 067c 006a 056a  .|.j.|.j.j.|.j.j
+000017e0: 087c 006a 006a 027c 006a 056a 0964 018d  .|.j.j.|.j.j.d..
+000017f0: 047d 027c 00a0 0aa1 007d 0364 027c 0364  .}.|.....}.d.|.d
+00001800: 033c 0074 0b6a 0c64 047c 006a 056a 0d7c  .<.t.j.d.|.j.j.|
+00001810: 027c 0364 058d 0453 0029 064e 2904 7236  .|.d...S.).N).r6
+00001820: 0000 0072 4c00 0000 7262 0000 0072 4b00  ...rL...rb...rK.
+00001830: 0000 724e 0000 0072 4f00 0000 7250 0000  ..rN...rO...rP..
+00001840: 0029 03da 0375 726c 7251 0000 0072 5200  .)...urlrQ...rR.
+00001850: 0000 290e 7216 0000 0072 6100 0000 7262  ..).r....ra...rb
+00001860: 0000 00da 0474 696d 6572 0a00 0000 7210  .....timer....r.
+00001870: 0000 0072 3600 0000 5a14 7072 6570 6172  ...r6...Z.prepar
+00001880: 655f 7265 6672 6573 685f 626f 6479 724c  e_refresh_bodyrL
+00001890: 0000 0072 3700 0000 7253 0000 0072 3e00  ...r7...rS...r>.
+000018a0: 0000 7254 0000 0072 5500 0000 2904 721f  ..rT...rU...).r.
+000018b0: 0000 0072 3800 0000 7256 0000 0072 5200  ...r8...rV...rR.
+000018c0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+000018d0: 005a 1b5f 5f67 6574 5f72 6566 7265 7368  .Z.__get_refresh
+000018e0: 5f74 6f6b 656e 5f72 6571 7565 7374 ae00  _token_request..
+000018f0: 0000 732c 0000 0000 0208 ff02 020a fe02  ..s,............
+00001900: 030a fd02 040e fc02 0604 020e 010c 0104  ................
+00001910: 0106 0106 0106 0106 fc06 0608 0108 0104  ................
+00001920: 010c ff7a 2941 7574 686f 7269 7a61 7469  ...z)Authorizati
+00001930: 6f6e 2e5f 5f67 6574 5f72 6566 7265 7368  on.__get_refresh
+00001940: 5f74 6f6b 656e 5f72 6571 7565 7374 6302  _token_requestc.
+00001950: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00001960: 0000 0043 0000 0073 5800 0000 7c01 a000  ...C...sX...|...
+00001970: a100 0100 7c00 6a01 6400 7501 7316 4a00  ....|.j.d.u.s.J.
+00001980: 8201 7402 7c00 6a03 6a04 8301 7d02 7c02  ..t.|.j.j...}.|.
+00001990: a005 7c01 6a06 a101 7d03 7c03 a007 6401  ..|.j...}.|...d.
+000019a0: a101 6400 7500 7248 7c00 6a01 6a08 7c03  ..d.u.rH|.j.j.|.
+000019b0: 6401 3c00 7c00 a009 7c03 a101 7c00 5f01  d.<.|...|...|._.
+000019c0: 6400 5300 2902 4e72 6200 0000 290a 7241  d.S.).Nrb...).rA
+000019d0: 0000 0072 1600 0000 720a 0000 0072 1000  ...r....r....r..
+000019e0: 0000 7236 0000 0072 4200 0000 7243 0000  ..r6...rB...rC..
+000019f0: 0072 6300 0000 7262 0000 0072 4400 0000  .rc...rb...rD...
+00001a00: 2904 721f 0000 0072 6700 0000 7238 0000  ).r....rg...r8..
+00001a10: 0072 4700 0000 7221 0000 0072 2100 0000  .rG...r!...r!...
+00001a20: 7222 0000 005a 205f 5f63 6f6d 706c 6574  r"...Z __complet
+00001a30: 655f 7265 6672 6573 685f 746f 6b65 6e5f  e_refresh_token_
+00001a40: 7265 7175 6573 74c5 0000 0073 0e00 0000  request....s....
+00001a50: 0001 0801 0e01 0c01 0c01 0e01 0c01 7a2e  ..............z.
+00001a60: 4175 7468 6f72 697a 6174 696f 6e2e 5f5f  Authorization.__
+00001a70: 636f 6d70 6c65 7465 5f72 6566 7265 7368  complete_refresh
+00001a80: 5f74 6f6b 656e 5f72 6571 7565 7374 6301  _token_requestc.
+00001a90: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+00001aa0: 0000 0043 0000 0073 4800 0000 7c00 a000  ...C...sH...|...
+00001ab0: a100 7d01 7401 a002 a100 8f24 7d02 7c02  ..}.t......$}.|.
+00001ac0: a003 7c01 a101 7d03 7c00 a004 7c03 a101  ..|...}.|...|...
+00001ad0: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
+00001ae0: 3100 733a 3000 0100 0100 0100 5900 0100  1.s:0.......Y...
+00001af0: 6400 5300 7215 0000 0029 05da 205f 4175  d.S.r....).. _Au
+00001b00: 7468 6f72 697a 6174 696f 6e5f 5f67 6574  thorization__get
+00001b10: 5f75 7365 725f 7265 7175 6573 7472 3e00  _user_requestr>.
+00001b20: 0000 723f 0000 0072 4000 0000 da25 5f41  ..r?...r@....%_A
+00001b30: 7574 686f 7269 7a61 7469 6f6e 5f5f 636f  uthorization__co
+00001b40: 6d70 6c65 7465 5f75 7365 725f 7265 7175  mplete_user_requ
+00001b50: 6573 74a9 0472 1f00 0000 5a08 7573 6572  est..r....Z.user
+00001b60: 5f72 6571 7238 0000 00da 0975 7365 725f  _reqr8.....user_
+00001b70: 7265 7370 7221 0000 0072 2100 0000 7222  respr!...r!...r"
+00001b80: 0000 005a 0a5f 5f67 6574 5f75 7365 72ce  ...Z.__get_user.
+00001b90: 0000 0073 0800 0000 0001 0801 0a01 0a01  ...s............
+00001ba0: 7a18 4175 7468 6f72 697a 6174 696f 6e2e  z.Authorization.
+00001bb0: 5f5f 6765 745f 7573 6572 6301 0000 0000  __get_userc.....
+00001bc0: 0000 0000 0000 0004 0000 0009 0000 00c3  ................
+00001bd0: 0000 0073 6600 0000 7c00 a000 a100 7d01  ...sf...|.....}.
+00001be0: 7401 6a02 6401 6402 8d01 3400 4900 6400  t.j.d.d...4.I.d.
+00001bf0: 4800 9a30 7d02 7c02 a003 7c01 a101 4900  H..0}.|...|...I.
+00001c00: 6400 4800 7d03 7c00 a004 7c03 a101 5700  d.H.}.|...|...W.
+00001c10: 0200 6400 0400 0400 8303 4900 6400 4800  ..d.......I.d.H.
+00001c20: 0100 5300 3100 4900 6400 4800 7358 3000  ..S.1.I.d.H.sX0.
+00001c30: 0100 0100 0100 5900 0100 6400 5300 723c  ......Y...d.S.r<
+00001c40: 0000 0029 0572 6a00 0000 723e 0000 0072  ...).rj...r>...r
+00001c50: 4900 0000 7240 0000 0072 6b00 0000 726c  I...r@...rk...rl
+00001c60: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001c70: 0000 5a10 5f5f 6765 745f 7573 6572 5f61  ..Z.__get_user_a
+00001c80: 7379 6e63 d400 0000 7308 0000 0000 0108  sync....s.......
+00001c90: 0116 0110 017a 1e41 7574 686f 7269 7a61  .....z.Authoriza
+00001ca0: 7469 6f6e 2e5f 5f67 6574 5f75 7365 725f  tion.__get_user_
+00001cb0: 6173 796e 6363 0100 0000 0000 0000 0000  asyncc..........
+00001cc0: 0000 0200 0000 0500 0000 4300 0000 734c  ..........C...sL
+00001cd0: 0000 007c 006a 0064 0075 0173 0e4a 0082  ...|.j.d.u.s.J..
+00001ce0: 017c 006a 016a 0264 0075 0173 1e4a 0082  .|.j.j.d.u.s.J..
+00001cf0: 017c 00a0 03a1 007d 0164 017c 006a 006a  .|.....}.d.|.j.j
+00001d00: 049b 009d 027c 0164 023c 0074 056a 0664  .....|.d.<.t.j.d
+00001d10: 037c 006a 016a 027c 0164 048d 0353 0029  .|.j.j.|.d...S.)
+00001d20: 054e 7a07 4265 6172 6572 2072 0f00 0000  .Nz.Bearer r....
+00001d30: 5a03 4745 5429 0172 5200 0000 2907 722e  Z.GET).rR...).r.
+00001d40: 0000 0072 1000 0000 7259 0000 0072 5300  ...r....rY...rS.
+00001d50: 0000 7258 0000 0072 3e00 0000 7254 0000  ..rX...r>...rT..
+00001d60: 0029 0272 1f00 0000 7252 0000 0072 2100  .).r....rR...r!.
+00001d70: 0000 7221 0000 0072 2200 0000 5a12 5f5f  ..r!...r"...Z.__
+00001d80: 6765 745f 7573 6572 5f72 6571 7565 7374  get_user_request
+00001d90: da00 0000 730a 0000 0000 010e 0110 0108  ....s...........
+00001da0: 0112 017a 2041 7574 686f 7269 7a61 7469  ...z Authorizati
+00001db0: 6f6e 2e5f 5f67 6574 5f75 7365 725f 7265  on.__get_user_re
+00001dc0: 7175 6573 7463 0200 0000 0000 0000 0000  questc..........
+00001dd0: 0000 0300 0000 0600 0000 4300 0000 733a  ..........C...s:
+00001de0: 0000 007c 01a0 00a1 0001 007c 006a 016a  ...|.......|.j.j
+00001df0: 0264 0075 0173 184a 0082 0174 03a0 047c  .d.u.s.J...t...|
+00001e00: 016a 05a1 017d 0274 067c 0274 077c 006a  .j...}.t.|.t.|.j
+00001e10: 01a0 027c 02a1 0183 0183 0253 0072 1500  ...|.......S.r..
+00001e20: 0000 2908 7241 0000 0072 1000 0000 725a  ..).rA...r....rZ
+00001e30: 0000 00da 046a 736f 6eda 056c 6f61 6473  .....json..loads
+00001e40: 7243 0000 0072 0e00 0000 da03 7374 7229  rC...r......str)
+00001e50: 0372 1f00 0000 726d 0000 005a 0275 6a72  .r....rm...Z.ujr
+00001e60: 2100 0000 7221 0000 0072 2200 0000 5a17  !...r!...r"...Z.
+00001e70: 5f5f 636f 6d70 6c65 7465 5f75 7365 725f  __complete_user_
+00001e80: 7265 7175 6573 74e1 0000 0073 0800 0000  request....s....
+00001e90: 0001 0801 1001 0c01 7a25 4175 7468 6f72  ........z%Author
+00001ea0: 697a 6174 696f 6e2e 5f5f 636f 6d70 6c65  ization.__comple
+00001eb0: 7465 5f75 7365 725f 7265 7175 6573 7463  te_user_requestc
+00001ec0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001ed0: 0300 0000 4300 0000 730e 0000 0064 0164  ....C...s....d.d
+00001ee0: 0274 009b 009d 0269 0153 0029 034e 7a0a  .t.....i.S.).Nz.
+00001ef0: 5573 6572 2d41 6765 6e74 7a05 466c 6574  User-Agentz.Flet
+00001f00: 2f72 0500 0000 722d 0000 0072 2100 0000  /r....r-...r!...
+00001f10: 7221 0000 0072 2200 0000 5a15 5f5f 6765  r!...r"...Z.__ge
+00001f20: 745f 6465 6661 756c 745f 6865 6164 6572  t_default_header
+00001f30: 73e7 0000 0073 0400 0000 0002 0aff 7a23  s....s........z#
+00001f40: 4175 7468 6f72 697a 6174 696f 6e2e 5f5f  Authorization.__
+00001f50: 6765 745f 6465 6661 756c 745f 6865 6164  get_default_head
+00001f60: 6572 7329 014e 2921 da08 5f5f 6e61 6d65  ers).N)!..__name
+00001f70: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001f80: 5f5f 7175 616c 6e61 6d65 5f5f 720c 0000  __qualname__r...
+00001f90: 00da 0462 6f6f 6c72 0300 0000 7202 0000  ...boolr....r...
+00001fa0: 0072 7000 0000 7223 0000 0072 2900 0000  .rp...r#...r)...
+00001fb0: 722c 0000 00da 0870 726f 7065 7274 7972  r,.....propertyr
+00001fc0: 0d00 0000 722e 0000 0072 2f00 0000 7204  ....r....r/...r.
+00001fd0: 0000 0072 3a00 0000 7248 0000 0072 4a00  ...r:...rH...rJ.
+00001fe0: 0000 723d 0000 0072 2700 0000 722b 0000  ..r=...r'...r+..
+00001ff0: 0072 0b00 0000 7244 0000 0072 2600 0000  .r....rD...r&...
+00002000: 722a 0000 0072 6400 0000 7265 0000 0072  r*...rd...re...r
+00002010: 5c00 0000 725e 0000 0072 6a00 0000 726b  \...r^...rj...rk
+00002020: 0000 0072 5300 0000 7221 0000 0072 2100  ...rS...r!...r!.
+00002030: 0000 7221 0000 0072 2200 0000 720f 0000  ..r!...r"...r...
+00002040: 0014 0000 0073 3c00 0000 0806 00fb 0202  .....s<.........
+00002050: 0201 0201 0201 0a01 02fa 0c1b 0e05 0e06  ................
+00002060: 0201 1406 0201 1405 160d 0e0a 0e0a 0e0f  ................
+00002070: 080f 080f 0e0a 0807 0807 0817 0809 0806  ................
+00002080: 0806 0807 0806 720f 0000 0029 1c72 1b00  ......r....).r..
+00002090: 0000 726e 0000 0072 3400 0000 7218 0000  ..rn...r4...r...
+000020a0: 0072 6900 0000 da06 7479 7069 6e67 7202  .ri.....typingr.
+000020b0: 0000 0072 0300 0000 7204 0000 0072 3e00  ...r....r....r>.
+000020c0: 0000 5a0c 666c 6574 2e76 6572 7369 6f6e  ..Z.flet.version
+000020d0: 7206 0000 00da 0f66 6c65 745f 636f 7265  r......flet_core
+000020e0: 2e6c 6f63 6b73 7207 0000 0072 0800 0000  .locksr....r....
+000020f0: da0f 666c 6574 5f63 6f72 652e 7574 696c  ..flet_core.util
+00002100: 7372 0900 0000 5a0f 6f61 7574 686c 6962  sr....Z.oauthlib
+00002110: 2e6f 6175 7468 3272 0a00 0000 5a1e 6f61  .oauth2r....Z.oa
+00002120: 7574 686c 6962 2e6f 6175 7468 322e 7266  uthlib.oauth2.rf
+00002130: 6336 3734 392e 746f 6b65 6e73 720b 0000  c6749.tokensr...
+00002140: 00da 2066 6c65 745f 7275 6e74 696d 652e  .. flet_runtime.
+00002150: 6175 7468 2e6f 6175 7468 5f70 726f 7669  auth.oauth_provi
+00002160: 6465 7272 0c00 0000 da1d 666c 6574 5f72  derr......flet_r
+00002170: 756e 7469 6d65 2e61 7574 682e 6f61 7574  untime.auth.oaut
+00002180: 685f 746f 6b65 6e72 0d00 0000 da16 666c  h_tokenr......fl
+00002190: 6574 5f72 756e 7469 6d65 2e61 7574 682e  et_runtime.auth.
+000021a0: 7573 6572 720e 0000 0072 0f00 0000 7221  userr....r....r!
+000021b0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+000021c0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000021d0: 731e 0000 0008 0108 0108 0108 0108 0114  s...............
+000021e0: 0208 010c 0110 010c 010c 010c 020c 010c  ................
+000021f0: 010c 03                                  ...
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 128 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 8000 0000  a........9)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 9200 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1400 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 6402  d.d...d.e...Z.d.
 00000040: 5300 2903 6300 0000 0000 0000 0000 0000  S.).c...........
 00000050: 0000 0000 0004 0000 0000 0000 0073 2400  .............s$.
 00000060: 0000 6500 5a01 6400 5a02 6503 6401 6402  ..e.Z.d.Z.e.d.d.
 00000070: 9c02 8700 6601 6403 6404 840c 5a04 8700  ....f.d.d...Z...
-00000080: 0400 5a05 5300 2905 da05 4772 6f75 704e  ..Z.S.)...GroupN
-00000090: 2902 da04 6e61 6d65 da06 7265 7475 726e  )...name..return
-000000a0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000000b0: 0003 0000 0003 0000 0073 1600 0000 7400  .........s....t.
-000000c0: 8300 a001 7c01 a101 0100 7c02 7c00 5f02  ....|.....|.|._.
-000000d0: 6400 5300 2901 4e29 03da 0573 7570 6572  d.S.).N)...super
-000000e0: da08 5f5f 696e 6974 5f5f 7202 0000 0029  ..__init__r....)
-000000f0: 03da 0473 656c 66da 066b 7761 7267 7372  ...self..kwargsr
-00000100: 0200 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
-00000110: 5fa9 00fa 5c2f 776f 726b 7370 6163 6573  _...\/workspaces
-00000120: 2f63 6f6e 7472 6962 666c 6574 2f66 6c65  /contribflet/fle
-00000130: 742f 7364 6b2f 7079 7468 6f6e 2f70 6163  t/sdk/python/pac
-00000140: 6b61 6765 732f 666c 6574 2d72 756e 7469  kages/flet-runti
-00000150: 6d65 2f73 7263 2f66 6c65 745f 7275 6e74  me/src/flet_runt
-00000160: 696d 652f 6175 7468 2f67 726f 7570 2e70  ime/auth/group.p
-00000170: 7972 0500 0000 0200 0000 7304 0000 0000  yr........s.....
-00000180: 010c 017a 0e47 726f 7570 2e5f 5f69 6e69  ...z.Group.__ini
-00000190: 745f 5f29 06da 085f 5f6e 616d 655f 5fda  t__)...__name__.
-000001a0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000001b0: 7561 6c6e 616d 655f 5fda 0373 7472 7205  ualname__..strr.
-000001c0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-000001d0: 5f5f 720a 0000 0072 0a00 0000 7208 0000  __r....r....r...
-000001e0: 0072 0b00 0000 7201 0000 0001 0000 0073  .r....r........s
-000001f0: 0200 0000 0801 7201 0000 004e 2902 da04  ......r....N)...
-00000200: 6469 6374 7201 0000 0072 0a00 0000 720a  dictr....r....r.
-00000210: 0000 0072 0a00 0000 720b 0000 00da 083c  ...r....r......<
-00000220: 6d6f 6475 6c65 3e01 0000 00f3 0000 0000  module>.........
+00000080: 0400 5a05 5300 2905 da04 5573 6572 4e29  ..Z.S.)...UserN)
+00000090: 02da 0269 64da 0672 6574 7572 6e63 0300  ...id..returnc..
+000000a0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000000b0: 0000 0300 0000 731c 0000 0074 0083 00a0  ......s....t....
+000000c0: 017c 01a1 0101 007c 027c 005f 0267 007c  .|.....|.|._.g.|
+000000d0: 005f 0364 0053 0029 014e 2904 da05 7375  ._.d.S.).N)...su
+000000e0: 7065 72da 085f 5f69 6e69 745f 5f72 0200  per..__init__r..
+000000f0: 0000 da06 6772 6f75 7073 2903 da04 7365  ....groups)...se
+00000100: 6c66 da06 6b77 6172 6773 7202 0000 00a9  lf..kwargsr.....
+00000110: 01da 095f 5f63 6c61 7373 5f5f a900 fa62  ...__class__...b
+00000120: 2f77 6f72 6b73 7061 6365 732f 636f 6e74  /workspaces/cont
+00000130: 7269 6266 6c65 742f 666c 6574 636f 6e74  ribflet/fletcont
+00000140: 7269 622f 7364 6b2f 7079 7468 6f6e 2f70  rib/sdk/python/p
+00000150: 6163 6b61 6765 732f 666c 6574 2d72 756e  ackages/flet-run
+00000160: 7469 6d65 2f73 7263 2f66 6c65 745f 7275  time/src/flet_ru
+00000170: 6e74 696d 652f 6175 7468 2f75 7365 722e  ntime/auth/user.
+00000180: 7079 7205 0000 0002 0000 0073 0600 0000  pyr........s....
+00000190: 0001 0c01 0601 7a0d 5573 6572 2e5f 5f69  ......z.User.__i
+000001a0: 6e69 745f 5f29 06da 085f 5f6e 616d 655f  nit__)...__name_
+000001b0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000001c0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
+000001d0: 7205 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
+000001e0: 6c6c 5f5f 720b 0000 0072 0b00 0000 7209  ll__r....r....r.
+000001f0: 0000 0072 0c00 0000 7201 0000 0001 0000  ...r....r.......
+00000200: 0073 0200 0000 0801 7201 0000 004e 2902  .s......r....N).
+00000210: da04 6469 6374 7201 0000 0072 0b00 0000  ..dictr....r....
+00000220: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000230: 083c 6d6f 6475 6c65 3e01 0000 00f3 0000  .<module>.......
+00000240: 0000                                     ..
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 1806 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 0e07 0000  a........9)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 0e07 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000060: 8400 6405 8302 5a08 6406 5300 2907 e900  ..d...Z.d.S.)...
 00000070: 0000 0029 03da 0843 616c 6c61 626c 65da  ...)...Callable.
@@ -50,81 +50,81 @@
 00000310: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
 00000320: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
 00000330: 0000 290e da04 7365 6c66 7208 0000 0072  ..)...selfr....r
 00000340: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
 00000350: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
 00000360: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
 00000370: 0072 1300 0000 7214 0000 00a9 0072 1800  .r....r......r..
-00000380: 0000 fa65 2f77 6f72 6b73 7061 6365 732f  ...e/workspaces/
+00000380: 0000 fa6c 2f77 6f72 6b73 7061 6365 732f  ...l/workspaces/
 00000390: 636f 6e74 7269 6266 6c65 742f 666c 6574  contribflet/flet
-000003a0: 2f73 646b 2f70 7974 686f 6e2f 7061 636b  /sdk/python/pack
-000003b0: 6167 6573 2f66 6c65 742d 7275 6e74 696d  ages/flet-runtim
-000003c0: 652f 7372 632f 666c 6574 5f72 756e 7469  e/src/flet_runti
-000003d0: 6d65 2f61 7574 682f 6f61 7574 685f 7072  me/auth/oauth_pr
-000003e0: 6f76 6964 6572 2e70 79da 085f 5f69 6e69  ovider.py..__ini
-000003f0: 745f 5f08 0000 0073 1a00 0000 0010 0601  t__....s........
-00000400: 0601 0601 0601 0601 1201 1201 0601 0601  ................
-00000410: 1201 0601 0601 7a16 4f41 7574 6850 726f  ......z.OAuthPro
-00000420: 7669 6465 722e 5f5f 696e 6974 5f5f 6301  vider.__init__c.
-00000430: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000440: 0000 0043 0000 0073 0c00 0000 7400 6401  ...C...s....t.d.
-00000450: 8301 8201 6400 5300 2902 4e7a 0f4e 6f74  ....d.S.).Nz.Not
-00000460: 2069 6d70 6c65 6d65 6e74 6564 2901 da09   implemented)...
-00000470: 4578 6365 7074 696f 6e29 0172 1700 0000  Exception).r....
-00000480: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000490: 055f 6e61 6d65 2600 0000 7302 0000 0000  ._name&...s.....
-000004a0: 017a 134f 4175 7468 5072 6f76 6964 6572  .z.OAuthProvider
-000004b0: 2e5f 6e61 6d65 2902 da0c 6163 6365 7373  ._name)...access
-000004c0: 5f74 6f6b 656e 7215 0000 0063 0200 0000  _tokenr....c....
-000004d0: 0000 0000 0000 0000 0200 0000 0100 0000  ................
-000004e0: 4300 0000 7304 0000 0067 0053 0072 1600  C...s....g.S.r..
-000004f0: 0000 7218 0000 00a9 0272 1700 0000 721d  ..r......r....r.
-00000500: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000510: 0000 da0d 5f66 6574 6368 5f67 726f 7570  ...._fetch_group
-00000520: 7329 0000 0073 0200 0000 0001 7a1b 4f41  s)...s......z.OA
-00000530: 7574 6850 726f 7669 6465 722e 5f66 6574  uthProvider._fet
-00000540: 6368 5f67 726f 7570 7363 0200 0000 0000  ch_groupsc......
-00000550: 0000 0000 0000 0200 0000 0100 0000 c300  ................
-00000560: 0000 7304 0000 0067 0053 0072 1600 0000  ..s....g.S.r....
-00000570: 7218 0000 0072 1e00 0000 7218 0000 0072  r....r....r....r
-00000580: 1800 0000 7219 0000 00da 135f 6665 7463  ....r......_fetc
-00000590: 685f 6772 6f75 7073 5f61 7379 6e63 2c00  h_groups_async,.
-000005a0: 0000 7302 0000 0000 017a 214f 4175 7468  ..s......z!OAuth
-000005b0: 5072 6f76 6964 6572 2e5f 6665 7463 685f  Provider._fetch_
-000005c0: 6772 6f75 7073 5f61 7379 6e63 6302 0000  groups_asyncc...
-000005d0: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-000005e0: 0043 0000 0073 0400 0000 6400 5300 7216  .C...s....d.S.r.
-000005f0: 0000 0072 1800 0000 721e 0000 0072 1800  ...r....r....r..
-00000600: 0000 7218 0000 0072 1900 0000 da0b 5f66  ..r....r......_f
-00000610: 6574 6368 5f75 7365 722f 0000 0073 0200  etch_user/...s..
-00000620: 0000 0001 7a19 4f41 7574 6850 726f 7669  ....z.OAuthProvi
-00000630: 6465 722e 5f66 6574 6368 5f75 7365 7263  der._fetch_userc
-00000640: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000650: 0100 0000 c300 0000 7304 0000 0064 0053  ........s....d.S
-00000660: 0072 1600 0000 7218 0000 0072 1e00 0000  .r....r....r....
-00000670: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000680: 115f 6665 7463 685f 7573 6572 5f61 7379  ._fetch_user_asy
-00000690: 6e63 3200 0000 7302 0000 0000 017a 1f4f  nc2...s......z.O
-000006a0: 4175 7468 5072 6f76 6964 6572 2e5f 6665  AuthProvider._fe
-000006b0: 7463 685f 7573 6572 5f61 7379 6e63 2908  tch_user_async).
-000006c0: 4e4e 4e4e 4e4e 4e4e 290f da08 5f5f 6e61  NNNNNNNN)...__na
-000006d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000006e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da03  ..__qualname__..
-000006f0: 7374 7272 0400 0000 7203 0000 0072 0200  strr....r....r..
-00000700: 0000 721a 0000 0072 1c00 0000 7205 0000  ..r....r....r...
-00000710: 0072 1f00 0000 7220 0000 0072 0600 0000  .r....r ...r....
-00000720: 7221 0000 0072 2200 0000 7218 0000 0072  r!...r"...r....r
-00000730: 1800 0000 7218 0000 0072 1900 0000 7207  ....r....r....r.
-00000740: 0000 0007 0000 0073 3a00 0000 0808 0001  .......s:.......
-00000750: 0001 0001 0001 0001 0001 0001 00f2 0202  ................
-00000760: 0201 0201 0201 0201 0201 0a01 0a01 0601  ................
-00000770: 0601 0a01 0601 0601 0601 02f1 0c1e 0803  ................
-00000780: 1403 1403 1403 7207 0000 004e 2909 da06  ......r....N)...
-00000790: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-000007a0: 7204 0000 00da 1766 6c65 745f 7275 6e74  r......flet_runt
-000007b0: 696d 652e 6175 7468 2e67 726f 7570 7205  ime.auth.groupr.
-000007c0: 0000 00da 1666 6c65 745f 7275 6e74 696d  .....flet_runtim
-000007d0: 652e 6175 7468 2e75 7365 7272 0600 0000  e.auth.userr....
-000007e0: 7207 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-000007f0: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
-00000800: 6c65 3e01 0000 0073 0600 0000 1402 0c01  le>....s........
-00000810: 0c03                                     ..
+000003a0: 636f 6e74 7269 622f 7364 6b2f 7079 7468  contrib/sdk/pyth
+000003b0: 6f6e 2f70 6163 6b61 6765 732f 666c 6574  on/packages/flet
+000003c0: 2d72 756e 7469 6d65 2f73 7263 2f66 6c65  -runtime/src/fle
+000003d0: 745f 7275 6e74 696d 652f 6175 7468 2f6f  t_runtime/auth/o
+000003e0: 6175 7468 5f70 726f 7669 6465 722e 7079  auth_provider.py
+000003f0: da08 5f5f 696e 6974 5f5f 0800 0000 731a  ..__init__....s.
+00000400: 0000 0000 1006 0106 0106 0106 0106 0112  ................
+00000410: 0112 0106 0106 0112 0106 0106 017a 164f  .............z.O
+00000420: 4175 7468 5072 6f76 6964 6572 2e5f 5f69  AuthProvider.__i
+00000430: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000440: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
+00000450: 0000 0074 0064 0183 0182 0164 0053 0029  ...t.d.....d.S.)
+00000460: 024e 7a0f 4e6f 7420 696d 706c 656d 656e  .Nz.Not implemen
+00000470: 7465 6429 01da 0945 7863 6570 7469 6f6e  ted)...Exception
+00000480: 2901 7217 0000 0072 1800 0000 7218 0000  ).r....r....r...
+00000490: 0072 1900 0000 da05 5f6e 616d 6526 0000  .r......_name&..
+000004a0: 0073 0200 0000 0001 7a13 4f41 7574 6850  .s......z.OAuthP
+000004b0: 726f 7669 6465 722e 5f6e 616d 6529 02da  rovider._name)..
+000004c0: 0c61 6363 6573 735f 746f 6b65 6e72 1500  .access_tokenr..
+000004d0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+000004e0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
+000004f0: 6700 5300 7216 0000 0072 1800 0000 a902  g.S.r....r......
+00000500: 7217 0000 0072 1d00 0000 7218 0000 0072  r....r....r....r
+00000510: 1800 0000 7219 0000 00da 0d5f 6665 7463  ....r......_fetc
+00000520: 685f 6772 6f75 7073 2900 0000 7302 0000  h_groups)...s...
+00000530: 0000 017a 1b4f 4175 7468 5072 6f76 6964  ...z.OAuthProvid
+00000540: 6572 2e5f 6665 7463 685f 6772 6f75 7073  er._fetch_groups
+00000550: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000560: 0001 0000 00c3 0000 0073 0400 0000 6700  .........s....g.
+00000570: 5300 7216 0000 0072 1800 0000 721e 0000  S.r....r....r...
+00000580: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000590: da13 5f66 6574 6368 5f67 726f 7570 735f  .._fetch_groups_
+000005a0: 6173 796e 632c 0000 0073 0200 0000 0001  async,...s......
+000005b0: 7a21 4f41 7574 6850 726f 7669 6465 722e  z!OAuthProvider.
+000005c0: 5f66 6574 6368 5f67 726f 7570 735f 6173  _fetch_groups_as
+000005d0: 796e 6363 0200 0000 0000 0000 0000 0000  yncc............
+000005e0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000005f0: 0064 0053 0072 1600 0000 7218 0000 0072  .d.S.r....r....r
+00000600: 1e00 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+00000610: 0000 00da 0b5f 6665 7463 685f 7573 6572  ....._fetch_user
+00000620: 2f00 0000 7302 0000 0000 017a 194f 4175  /...s......z.OAu
+00000630: 7468 5072 6f76 6964 6572 2e5f 6665 7463  thProvider._fetc
+00000640: 685f 7573 6572 6302 0000 0000 0000 0000  h_userc.........
+00000650: 0000 0002 0000 0001 0000 00c3 0000 0073  ...............s
+00000660: 0400 0000 6400 5300 7216 0000 0072 1800  ....d.S.r....r..
+00000670: 0000 721e 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00000680: 0072 1900 0000 da11 5f66 6574 6368 5f75  .r......_fetch_u
+00000690: 7365 725f 6173 796e 6332 0000 0073 0200  ser_async2...s..
+000006a0: 0000 0001 7a1f 4f41 7574 6850 726f 7669  ....z.OAuthProvi
+000006b0: 6465 722e 5f66 6574 6368 5f75 7365 725f  der._fetch_user_
+000006c0: 6173 796e 6329 084e 4e4e 4e4e 4e4e 4e29  async).NNNNNNNN)
+000006d0: 0fda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000006e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000006f0: 616d 655f 5fda 0373 7472 7204 0000 0072  ame__..strr....r
+00000700: 0300 0000 7202 0000 0072 1a00 0000 721c  ....r....r....r.
+00000710: 0000 0072 0500 0000 721f 0000 0072 2000  ...r....r....r .
+00000720: 0000 7206 0000 0072 2100 0000 7222 0000  ..r....r!...r"..
+00000730: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
+00000740: 7219 0000 0072 0700 0000 0700 0000 733a  r....r........s:
+00000750: 0000 0008 0800 0100 0100 0100 0100 0100  ................
+00000760: 0100 0100 f202 0202 0102 0102 0102 0102  ................
+00000770: 010a 010a 0106 0106 010a 0106 0106 0106  ................
+00000780: 0102 f10c 1e08 0314 0314 0314 0372 0700  .............r..
+00000790: 0000 4e29 09da 0674 7970 696e 6772 0200  ..N)...typingr..
+000007a0: 0000 7203 0000 0072 0400 0000 da17 666c  ..r....r......fl
+000007b0: 6574 5f72 756e 7469 6d65 2e61 7574 682e  et_runtime.auth.
+000007c0: 6772 6f75 7072 0500 0000 da16 666c 6574  groupr......flet
+000007d0: 5f72 756e 7469 6d65 2e61 7574 682e 7573  _runtime.auth.us
+000007e0: 6572 7206 0000 0072 0700 0000 7218 0000  err....r....r...
+000007f0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000800: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
+00000810: 0000 0014 020c 010c 03                   .........
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 847 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 4f03 0000  a........9)fO...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 4f03 0000  a........./fO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a06  ..G.d.d...d...Z.
 00000060: 6401 5300 2906 e900 0000 004e 2902 da04  d.S.)......N)...
 00000070: 4c69 7374 da08 4f70 7469 6f6e 616c 2901  List..Optional).
@@ -26,54 +26,55 @@
 00000190: 027c 005f 017c 037c 005f 027c 047c 005f  .|._.|.|._.|.|._
 000001a0: 037c 057c 005f 047c 067c 005f 0564 0053  .|.|._.|.|._.d.S
 000001b0: 00a9 014e 2906 7206 0000 0072 0700 0000  ...N).r....r....
 000001c0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 000001d0: 0b00 0000 2907 da04 7365 6c66 7206 0000  ....)...selfr...
 000001e0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
 000001f0: 720a 0000 0072 0b00 0000 a900 720f 0000  r....r......r...
-00000200: 00fa 622f 776f 726b 7370 6163 6573 2f63  ..b/workspaces/c
-00000210: 6f6e 7472 6962 666c 6574 2f66 6c65 742f  ontribflet/flet/
-00000220: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
-00000230: 6765 732f 666c 6574 2d72 756e 7469 6d65  ges/flet-runtime
-00000240: 2f73 7263 2f66 6c65 745f 7275 6e74 696d  /src/flet_runtim
-00000250: 652f 6175 7468 2f6f 6175 7468 5f74 6f6b  e/auth/oauth_tok
-00000260: 656e 2e70 79da 085f 5f69 6e69 745f 5f08  en.py..__init__.
-00000270: 0000 0073 0c00 0000 0009 0601 0601 0601  ...s............
-00000280: 0601 0601 7a13 4f41 7574 6854 6f6b 656e  ....z.OAuthToken
-00000290: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-000002a0: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
-000002b0: 0000 7310 0000 0074 006a 017c 0074 0264  ..s....t.j.|.t.d
-000002c0: 0164 028d 0353 0029 034e 2902 fa01 2cfa  .d...S.).N)...,.
-000002d0: 013a 2902 da03 636c 73da 0a73 6570 6172  .:)...cls..separ
-000002e0: 6174 6f72 7329 03da 046a 736f 6eda 0564  ators)...json..d
-000002f0: 756d 7073 7204 0000 0029 0172 0e00 0000  umpsr....).r....
-00000300: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00000310: 0774 6f5f 6a73 6f6e 1800 0000 7302 0000  .to_json....s...
-00000320: 0000 017a 124f 4175 7468 546f 6b65 6e2e  ...z.OAuthToken.
-00000330: 746f 5f6a 736f 6e29 01da 0464 6174 6163  to_json)...datac
-00000340: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000350: 0400 0000 4300 0000 7318 0000 0074 00a0  ....C...s....t..
-00000360: 017c 00a1 017d 0174 0266 0069 007c 01a4  .|...}.t.f.i.|..
-00000370: 018e 0153 0072 0d00 0000 2903 7216 0000  ...S.r....).r...
-00000380: 00da 056c 6f61 6473 7205 0000 0029 0272  ...loadsr....).r
-00000390: 1900 0000 da01 7472 0f00 0000 720f 0000  ......tr....r...
-000003a0: 0072 1000 0000 da09 6672 6f6d 5f6a 736f  .r......from_jso
-000003b0: 6e1b 0000 0073 0400 0000 0002 0a01 7a14  n....s........z.
-000003c0: 4f41 7574 6854 6f6b 656e 2e66 726f 6d5f  OAuthToken.from_
-000003d0: 6a73 6f6e 2905 4e4e 4e4e 4e29 0cda 085f  json).NNNNN)..._
-000003e0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000003f0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000400: 5fda 0373 7472 7203 0000 0072 0200 0000  _..strr....r....
-00000410: da03 696e 74da 0566 6c6f 6174 7211 0000  ..int..floatr...
-00000420: 0072 1800 0000 da0c 7374 6174 6963 6d65  .r......staticme
-00000430: 7468 6f64 721c 0000 0072 0f00 0000 720f  thodr....r....r.
-00000440: 0000 0072 0f00 0000 7210 0000 0072 0500  ...r....r....r..
-00000450: 0000 0700 0000 7322 0000 0008 0400 0100  ......s"........
-00000460: 0100 0100 0100 f902 0202 010a 0106 0106  ................
-00000470: 0106 0106 0102 f80c 1008 0302 0172 0500  .............r..
-00000480: 0000 2907 7216 0000 00da 0674 7970 696e  ..).r......typin
-00000490: 6772 0200 0000 7203 0000 00da 1c66 6c65  gr....r......fle
-000004a0: 745f 636f 7265 2e65 6d62 6564 5f6a 736f  t_core.embed_jso
-000004b0: 6e5f 656e 636f 6465 7272 0400 0000 7205  n_encoderr....r.
-000004c0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-000004d0: 0000 7210 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000004e0: 3e01 0000 0073 0600 0000 0801 1002 0c03  >....s..........
+00000200: 00fa 692f 776f 726b 7370 6163 6573 2f63  ..i/workspaces/c
+00000210: 6f6e 7472 6962 666c 6574 2f66 6c65 7463  ontribflet/fletc
+00000220: 6f6e 7472 6962 2f73 646b 2f70 7974 686f  ontrib/sdk/pytho
+00000230: 6e2f 7061 636b 6167 6573 2f66 6c65 742d  n/packages/flet-
+00000240: 7275 6e74 696d 652f 7372 632f 666c 6574  runtime/src/flet
+00000250: 5f72 756e 7469 6d65 2f61 7574 682f 6f61  _runtime/auth/oa
+00000260: 7574 685f 746f 6b65 6e2e 7079 da08 5f5f  uth_token.py..__
+00000270: 696e 6974 5f5f 0800 0000 730c 0000 0000  init__....s.....
+00000280: 0906 0106 0106 0106 0106 017a 134f 4175  ...........z.OAu
+00000290: 7468 546f 6b65 6e2e 5f5f 696e 6974 5f5f  thToken.__init__
+000002a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000002b0: 0005 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
+000002c0: 6a01 7c00 7402 6401 6402 8d03 5300 2903  j.|.t.d.d...S.).
+000002d0: 4e29 02fa 012c fa01 3a29 02da 0363 6c73  N)...,..:)...cls
+000002e0: da0a 7365 7061 7261 746f 7273 2903 da04  ..separators)...
+000002f0: 6a73 6f6e da05 6475 6d70 7372 0400 0000  json..dumpsr....
+00000300: 2901 720e 0000 0072 0f00 0000 720f 0000  ).r....r....r...
+00000310: 0072 1000 0000 da07 746f 5f6a 736f 6e18  .r......to_json.
+00000320: 0000 0073 0200 0000 0001 7a12 4f41 7574  ...s......z.OAut
+00000330: 6854 6f6b 656e 2e74 6f5f 6a73 6f6e 2901  hToken.to_json).
+00000340: da04 6461 7461 6301 0000 0000 0000 0000  ..datac.........
+00000350: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000360: 1800 0000 7400 a001 7c00 a101 7d01 7402  ....t...|...}.t.
+00000370: 6600 6900 7c01 a401 8e01 5300 720d 0000  f.i.|.....S.r...
+00000380: 0029 0372 1600 0000 da05 6c6f 6164 7372  .).r......loadsr
+00000390: 0500 0000 2902 7219 0000 00da 0174 720f  ....).r......tr.
+000003a0: 0000 0072 0f00 0000 7210 0000 00da 0966  ...r....r......f
+000003b0: 726f 6d5f 6a73 6f6e 1b00 0000 7304 0000  rom_json....s...
+000003c0: 0000 020a 017a 144f 4175 7468 546f 6b65  .....z.OAuthToke
+000003d0: 6e2e 6672 6f6d 5f6a 736f 6e29 054e 4e4e  n.from_json).NNN
+000003e0: 4e4e 290c da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
+000003f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000400: 616c 6e61 6d65 5f5f da03 7374 7272 0300  alname__..strr..
+00000410: 0000 7202 0000 00da 0369 6e74 da05 666c  ..r......int..fl
+00000420: 6f61 7472 1100 0000 7218 0000 00da 0c73  oatr....r......s
+00000430: 7461 7469 636d 6574 686f 6472 1c00 0000  taticmethodr....
+00000440: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000450: 1000 0000 7205 0000 0007 0000 0073 2200  ....r........s".
+00000460: 0000 0804 0001 0001 0001 0001 00f9 0202  ................
+00000470: 0201 0a01 0601 0601 0601 0601 02f8 0c10  ................
+00000480: 0803 0201 7205 0000 0029 0772 1600 0000  ....r....).r....
+00000490: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
+000004a0: 0000 da1c 666c 6574 5f63 6f72 652e 656d  ....flet_core.em
+000004b0: 6265 645f 6a73 6f6e 5f65 6e63 6f64 6572  bed_json_encoder
+000004c0: 7204 0000 0072 0500 0000 720f 0000 0072  r....r....r....r
+000004d0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+000004e0: 3c6d 6f64 756c 653e 0100 0000 7306 0000  <module>....s...
+000004f0: 0008 0110 020c 03                        .......
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/authorization.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/oauth_provider.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/oauth_token.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/flet_socket_server.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/flet_socket_server.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/security/__init__.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/security/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/uploads.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/uploads.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__init__.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 4787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 b312 0000  a........9)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 b312 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
@@ -33,345 +33,345 @@
 00000200: 0000 0000 0000 0000 0000 0002 0000 0003  ................
 00000210: 0000 0043 0000 0073 2200 0000 7400 a001  ...C...s"...t...
 00000220: 7c00 a101 7d01 7c01 6400 7501 721e 7c01  |...}.|.d.u.r.|.
 00000230: a002 a100 6401 7600 5300 6400 5300 2902  ....d.v.S.d.S.).
 00000240: 4e29 03da 0474 7275 65da 0131 da03 7965  N)...true..1..ye
 00000250: 7329 03da 026f 73da 0667 6574 656e 76da  s)...os..getenv.
 00000260: 056c 6f77 6572 2902 7207 0000 00da 0176  .lower).r......v
-00000270: a900 720f 0000 00fa 602f 776f 726b 7370  ..r.....`/worksp
+00000270: a900 720f 0000 00fa 672f 776f 726b 7370  ..r.....g/worksp
 00000280: 6163 6573 2f63 6f6e 7472 6962 666c 6574  aces/contribflet
-00000290: 2f66 6c65 742f 7364 6b2f 7079 7468 6f6e  /flet/sdk/python
-000002a0: 2f70 6163 6b61 6765 732f 666c 6574 2d72  /packages/flet-r
-000002b0: 756e 7469 6d65 2f73 7263 2f66 6c65 745f  untime/src/flet_
-000002c0: 7275 6e74 696d 652f 7574 696c 732f 5f5f  runtime/utils/__
-000002d0: 696e 6974 5f5f 2e70 79da 1067 6574 5f62  init__.py..get_b
-000002e0: 6f6f 6c5f 656e 765f 7661 720d 0000 0073  ool_env_var....s
-000002f0: 0400 0000 0001 0a01 7211 0000 0063 0000  ........r....c..
-00000300: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000310: 0000 4300 0000 730e 0000 0074 00a0 0164  ..C...s....t...d
-00000320: 01a1 0164 026b 0253 0029 034e da0d 464c  ...d.k.S.).N..FL
-00000330: 4554 5f50 4c41 5446 4f52 4dda 0369 6f73  ET_PLATFORM..ios
-00000340: a902 720b 0000 0072 0c00 0000 720f 0000  ..r....r....r...
-00000350: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000360: da06 6973 5f69 6f73 1200 0000 7302 0000  ..is_ios....s...
-00000370: 0000 0172 1500 0000 6300 0000 0000 0000  ...r....c.......
-00000380: 0000 0000 0000 0000 0003 0000 0043 0000  .............C..
-00000390: 0073 0e00 0000 7400 a001 6401 a101 6402  .s....t...d...d.
-000003a0: 6b02 5300 2903 4e72 1200 0000 da07 616e  k.S.).Nr......an
-000003b0: 6472 6f69 6472 1400 0000 720f 0000 0072  droidr....r....r
-000003c0: 0f00 0000 720f 0000 0072 1000 0000 da0a  ....r....r......
-000003d0: 6973 5f61 6e64 726f 6964 1600 0000 7302  is_android....s.
-000003e0: 0000 0000 0172 1700 0000 6300 0000 0000  .....r....c.....
-000003f0: 0000 0000 0000 0000 0000 0003 0000 0043  ...............C
-00000400: 0000 0073 0e00 0000 7400 a001 6401 a101  ...s....t...d...
-00000410: 6400 7501 5300 2902 4e72 1200 0000 7214  d.u.S.).Nr....r.
-00000420: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-00000430: 0000 7210 0000 00da 0b69 735f 656d 6265  ..r......is_embe
-00000440: 6464 6564 1a00 0000 7302 0000 0000 0172  dded....s......r
-00000450: 1800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000460: 0000 0000 0001 0000 0043 0000 0073 0c00  .........C...s..
-00000470: 0000 7400 8300 700a 7401 8300 5300 a901  ..t...p.t...S...
-00000480: 4e29 0272 1500 0000 7217 0000 0072 0f00  N).r....r....r..
-00000490: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000004a0: 00da 0969 735f 6d6f 6269 6c65 1e00 0000  ...is_mobile....
-000004b0: 7302 0000 0000 0172 1a00 0000 6300 0000  s......r....c...
-000004c0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-000004d0: 0043 0000 0073 1400 0000 7400 8300 0c00  .C...s....t.....
-000004e0: 6f12 7401 a002 a100 6401 6b02 5300 2902  o.t.....d.k.S.).
-000004f0: 4eda 0757 696e 646f 7773 a903 721a 0000  N..Windows..r...
-00000500: 00da 0870 6c61 7466 6f72 6dda 0673 7973  ...platform..sys
-00000510: 7465 6d72 0f00 0000 720f 0000 0072 0f00  temr....r....r..
-00000520: 0000 7210 0000 00da 0a69 735f 7769 6e64  ..r......is_wind
-00000530: 6f77 7327 0000 0073 0200 0000 0001 721f  ows'...s......r.
-00000540: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000550: 0000 0000 0200 0000 4300 0000 7314 0000  ........C...s...
-00000560: 0074 0083 000c 006f 1274 01a0 02a1 0064  .t.....o.t.....d
-00000570: 016b 0253 0029 024e da05 4c69 6e75 7872  .k.S.).N..Linuxr
-00000580: 1c00 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
-00000590: 0000 0072 1000 0000 da08 6973 5f6c 696e  ...r......is_lin
-000005a0: 7578 2b00 0000 7302 0000 0000 0172 2100  ux+...s......r!.
-000005b0: 0000 6300 0000 0000 0000 0000 0000 0002  ..c.............
-000005c0: 0000 0008 0000 0043 0000 0073 7c00 0000  .......C...s|...
-000005d0: 7400 8300 7378 7401 a002 a100 6401 6b02  t...sxt.....d.k.
-000005e0: 7278 6402 7d00 7403 6a04 a005 7c00 a101  rxd.}.t.j...|...
-000005f0: 7268 7406 7c00 6403 8302 8f2c 7d01 6404  rht.|.d....,}.d.
-00000600: 7c01 a007 a100 7600 724a 5700 6400 0400  |.....v.rJW.d...
-00000610: 0400 8303 0100 6405 5300 5700 6400 0400  ......d.S.W.d...
-00000620: 0400 8303 0100 6e10 3100 735e 3000 0100  ......n.1.s^0...
-00000630: 0100 0100 5900 0100 7403 6a08 a009 6406  ....Y...t.j...d.
-00000640: a101 6400 7500 5300 6405 5300 2907 4e72  ..d.u.S.d.S.).Nr
-00000650: 2000 0000 7a0d 2f70 726f 632f 7665 7273   ...z./proc/vers
-00000660: 696f 6eda 0172 5a09 6d69 6372 6f73 6f66  ion..rZ.microsof
-00000670: 7446 5a07 4449 5350 4c41 5929 0a72 1a00  tFZ.DISPLAY).r..
-00000680: 0000 721d 0000 0072 1e00 0000 720b 0000  ..r....r....r...
-00000690: 00da 0470 6174 68da 0665 7869 7374 73da  ...path..exists.
-000006a0: 046f 7065 6eda 0472 6561 64da 0765 6e76  .open..read..env
-000006b0: 6972 6f6e da03 6765 7429 02da 0170 da04  iron..get)...p..
-000006c0: 6669 6c65 720f 0000 0072 0f00 0000 7210  filer....r....r.
-000006d0: 0000 00da 0f69 735f 6c69 6e75 785f 7365  .....is_linux_se
-000006e0: 7276 6572 2f00 0000 7310 0000 0000 0112  rver/...s.......
-000006f0: 0204 010c 010c 010c 012e 0110 0172 2b00  .............r+.
-00000700: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000710: 0000 0002 0000 0043 0000 0073 1400 0000  .......C...s....
-00000720: 7400 8300 0c00 6f12 7401 a002 a100 6401  t.....o.t.....d.
-00000730: 6b02 5300 2902 4eda 0644 6172 7769 6e72  k.S.).N..Darwinr
-00000740: 1c00 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
-00000750: 0000 0072 1000 0000 da08 6973 5f6d 6163  ...r......is_mac
-00000760: 6f73 3b00 0000 7302 0000 0000 0172 2d00  os;...s......r-.
-00000770: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
-00000780: 0000 0003 0000 0043 0000 0073 4600 0000  .......C...sF...
-00000790: 7400 8300 730e 7401 a002 a100 6e02 6401  t...s.t.....n.d.
-000007a0: 7d00 7403 8300 721c 6402 5300 7c00 6403  }.t...r.d.S.|.d.
-000007b0: 6b02 7228 6404 5300 7c00 6405 6b02 7234  k.r(d.S.|.d.k.r4
-000007c0: 6406 5300 7404 6407 7c00 9b00 9d02 8301  d.S.t.d.|.......
-000007d0: 8201 6400 5300 2908 4eda 00da 0777 696e  ..d.S.).N....win
-000007e0: 646f 7773 7220 0000 00da 056c 696e 7578  dowsr .....linux
-000007f0: 722c 0000 00da 0664 6172 7769 6e7a 1655  r,.....darwinz.U
-00000800: 6e73 7570 706f 7274 6564 2070 6c61 7466  nsupported platf
-00000810: 6f72 6d3a 2029 0572 1a00 0000 721d 0000  orm: ).r....r...
-00000820: 0072 1e00 0000 721f 0000 00da 0945 7863  .r....r......Exc
-00000830: 6570 7469 6f6e 2901 7229 0000 0072 0f00  eption).r)...r..
-00000840: 0000 720f 0000 0072 1000 0000 da0c 6765  ..r....r......ge
-00000850: 745f 706c 6174 666f 726d 3f00 0000 7310  t_platform?...s.
-00000860: 0000 0000 0112 0106 0104 0108 0104 0108  ................
-00000870: 0104 0272 3300 0000 6300 0000 0000 0000  ...r3...c.......
-00000880: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000890: 0073 5e00 0000 7400 8300 7312 7401 a002  .s^...t...s.t...
-000008a0: a100 a003 a100 6e02 6401 7d00 7c00 6402  ......n.d.}.|.d.
-000008b0: 6b02 7326 7c00 6403 6b02 722a 6403 5300  k.s&|.d.k.r*d.S.
-000008c0: 7c00 6404 6b02 733a 7c00 6405 6b02 723e  |.d.k.s:|.d.k.r>
-000008d0: 6404 5300 7c00 a004 6406 a101 724c 6407  d.S.|...d...rLd.
-000008e0: 5300 7405 6408 7c00 9b00 9d02 8301 8201  S.t.d.|.........
-000008f0: 6400 5300 2909 4e72 2e00 0000 5a06 7838  d.S.).Nr....Z.x8
-00000900: 365f 3634 5a05 616d 6436 345a 0561 726d  6_64Z.amd64Z.arm
-00000910: 3634 5a07 6161 7263 6836 345a 0361 726d  64Z.aarch64Z.arm
-00000920: 5a05 6172 6d5f 377a 1a55 6e73 7570 706f  Z.arm_7z.Unsuppo
-00000930: 7274 6564 2061 7263 6869 7465 6374 7572  rted architectur
-00000940: 653a 2029 0672 1a00 0000 721d 0000 00da  e: ).r....r.....
-00000950: 076d 6163 6869 6e65 720d 0000 00da 0a73  .machiner......s
-00000960: 7461 7274 7377 6974 6872 3200 0000 2901  tartswithr2...).
-00000970: da01 6172 0f00 0000 720f 0000 0072 1000  ..ar....r....r..
-00000980: 0000 da08 6765 745f 6172 6368 4b00 0000  ....get_archK...
-00000990: 7310 0000 0000 0116 0110 0104 0110 0104  s...............
-000009a0: 010a 0104 0272 3700 0000 6301 0000 0000  .....r7...c.....
-000009b0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-000009c0: 0000 0073 1400 0000 7400 8300 7310 7401  ...s....t...s.t.
-000009d0: a002 7c00 a101 0100 6400 5300 7219 0000  ..|.....d.S.r...
-000009e0: 0029 0372 1a00 0000 da0a 7765 6262 726f  .).r......webbro
-000009f0: 7773 6572 7225 0000 00a9 01da 0375 726c  wserr%.......url
-00000a00: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00000a10: 0f6f 7065 6e5f 696e 5f62 726f 7773 6572  .open_in_browser
-00000a20: 5700 0000 7304 0000 0000 0106 0172 3b00  W...s........r;.
-00000a30: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
-00000a40: 0000 0005 0000 0003 0000 0073 6e00 0000  ...........sn...
-00000a50: 6401 6400 6c00 8900 8700 6601 6402 6403  d.d.l.....f.d.d.
-00000a60: 8408 7d02 8800 6a01 6404 1900 a002 8800  ..}...j.d.......
-00000a70: 6a03 a101 4400 5d42 7d03 8800 6a04 a005  j...D.]B}...j...
-00000a80: 7c03 7c00 a102 7d04 7c02 7c04 8301 7226  |.|...}.|.|...r&
-00000a90: 7c01 6400 7500 7360 7c01 6400 7501 7226  |.d.u.s`|.d.u.r&
-00000aa0: 7c01 a006 a100 7c04 a006 a100 6b03 7226  |.....|.....k.r&
-00000ab0: 7c04 0200 0100 5300 7126 6400 5300 2905  |.....S.q&d.S.).
-00000ac0: 4e72 0100 0000 6301 0000 0000 0000 0000  Nr....c.........
-00000ad0: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
-00000ae0: 1a00 0000 8800 6a00 a001 7c00 a101 6f18  ......j...|...o.
-00000af0: 8800 a002 7c00 8800 6a03 a102 5300 7219  ....|...j...S.r.
-00000b00: 0000 0029 0472 2300 0000 da06 6973 6669  ...).r#.....isfi
-00000b10: 6c65 da06 6163 6365 7373 da04 585f 4f4b  le..access..X_OK
-00000b20: 2901 5a05 6670 6174 68a9 0172 0b00 0000  ).Z.fpath..r....
-00000b30: 720f 0000 0072 1000 0000 da06 6973 5f65  r....r......is_e
-00000b40: 7865 6000 0000 7302 0000 0000 017a 1577  xe`...s......z.w
-00000b50: 6869 6368 2e3c 6c6f 6361 6c73 3e2e 6973  hich.<locals>.is
-00000b60: 5f65 7865 da04 5041 5448 2907 720b 0000  _exe..PATH).r...
-00000b70: 0072 2700 0000 da05 7370 6c69 74da 0770  .r'.....split..p
-00000b80: 6174 6873 6570 7223 0000 00da 046a 6f69  athsepr#.....joi
-00000b90: 6e72 0d00 0000 2905 da07 7072 6f67 7261  nr....)...progra
-00000ba0: 6d5a 0b65 7863 6c75 6465 5f65 7865 7240  mZ.exclude_exer@
-00000bb0: 0000 0072 2300 0000 5a08 6578 655f 6669  ...r#...Z.exe_fi
-00000bc0: 6c65 720f 0000 0072 3f00 0000 7210 0000  ler....r?...r...
-00000bd0: 00da 0577 6869 6368 5d00 0000 731a 0000  ...which]...s...
-00000be0: 0000 0108 020c 0316 010e 0108 0106 ff02  ................
-00000bf0: 0206 fe02 020e fe02 040a 0272 4600 0000  ...........rF...
-00000c00: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00000c10: 0004 0000 0043 0000 0073 3000 0000 7400  .....C...s0...t.
-00000c20: 6a01 a002 7c00 a101 7d02 7400 6a01 a002  j...|...}.t.j...
-00000c30: 7c01 a101 7d03 7400 6a01 a003 7c02 7c03  |...}.t.j...|.|.
-00000c40: 6702 a101 7d04 7c04 7c02 6b02 5300 7219  g...}.|.|.k.S.r.
-00000c50: 0000 0029 0472 0b00 0000 7223 0000 00da  ...).r....r#....
-00000c60: 0761 6273 7061 7468 da0c 636f 6d6d 6f6e  .abspath..common
-00000c70: 7072 6566 6978 2905 da09 6469 7265 6374  prefix)...direct
-00000c80: 6f72 79da 0674 6172 6765 745a 0d61 6273  ory..targetZ.abs
-00000c90: 5f64 6972 6563 746f 7279 5a0a 6162 735f  _directoryZ.abs_
-00000ca0: 7461 7267 6574 da06 7072 6566 6978 720f  target..prefixr.
-00000cb0: 0000 0072 0f00 0000 7210 0000 00da 1369  ...r....r......i
-00000cc0: 735f 7769 7468 696e 5f64 6972 6563 746f  s_within_directo
-00000cd0: 7279 6e00 0000 7308 0000 0000 010c 010c  ryn...s.........
-00000ce0: 0210 0272 4c00 0000 da01 2e46 a901 da0d  ...rL......F....
-00000cf0: 6e75 6d65 7269 635f 6f77 6e65 7263 0300  numeric_ownerc..
-00000d00: 0000 0000 0000 0100 0000 0600 0000 0500  ................
-00000d10: 0000 4300 0000 7344 0000 007c 00a0 00a1  ..C...sD...|....
-00000d20: 0044 005d 267d 0474 016a 02a0 037c 017c  .D.]&}.t.j...|.|
-00000d30: 046a 04a1 027d 0574 057c 017c 0583 0273  .j...}.t.|.|...s
-00000d40: 0874 0664 0183 0182 0171 087c 006a 077c  .t.d.....q.|.j.|
-00000d50: 017c 027c 0364 028d 0301 0064 0053 0029  .|.|.d.....d.S.)
-00000d60: 034e 7a24 4174 7465 6d70 7465 6420 5061  .Nz$Attempted Pa
-00000d70: 7468 2054 7261 7665 7273 616c 2069 6e20  th Traversal in 
-00000d80: 5461 7220 4669 6c65 724e 0000 0029 08da  Tar FilerN...)..
-00000d90: 0a67 6574 6d65 6d62 6572 7372 0b00 0000  .getmembersr....
-00000da0: 7223 0000 0072 4400 0000 7207 0000 0072  r#...rD...r....r
-00000db0: 4c00 0000 7232 0000 00da 0a65 7874 7261  L...r2.....extra
-00000dc0: 6374 616c 6c29 06da 0374 6172 7223 0000  ctall)...tarr#..
-00000dd0: 00da 076d 656d 6265 7273 724f 0000 00da  ...membersrO....
-00000de0: 066d 656d 6265 725a 0b6d 656d 6265 725f  .memberZ.member_
-00000df0: 7061 7468 720f 0000 0072 0f00 0000 7210  pathr....r....r.
-00000e00: 0000 00da 1373 6166 655f 7461 725f 6578  .....safe_tar_ex
-00000e10: 7472 6163 7461 6c6c 7700 0000 730a 0000  tractallw...s...
-00000e20: 0000 010c 0110 010a 010a 0272 5500 0000  ...........rU...
-00000e30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000e40: 0002 0000 0043 0000 0073 2000 0000 6401  .....C...s ...d.
-00000e50: 7c00 7600 701e 6402 7c00 7600 701e 6403  |.v.p.d.|.v.p.d.
-00000e60: 7c00 7600 701e 6404 7c00 7600 5300 2905  |.v.p.d.|.v.S.).
-00000e70: 4e7a 0d3a 2f2f 6c6f 6361 6c68 6f73 742f  Nz.://localhost/
-00000e80: 7a0d 3a2f 2f6c 6f63 616c 686f 7374 3a7a  z.://localhost:z
-00000e90: 0d3a 2f2f 3132 372e 302e 302e 312f 7a0d  .://127.0.0.1/z.
-00000ea0: 3a2f 2f31 3237 2e30 2e30 2e31 3a72 0f00  ://127.0.0.1:r..
-00000eb0: 0000 7239 0000 0072 0f00 0000 720f 0000  ..r9...r....r...
-00000ec0: 0072 1000 0000 da10 6973 5f6c 6f63 616c  .r......is_local
-00000ed0: 686f 7374 5f75 726c 8000 0000 730e 0000  host_url....s...
-00000ee0: 0000 0208 0106 ff02 0206 fe02 0306 fc72  ...............r
-00000ef0: 5600 0000 2901 da14 6765 745f 7061 636b  V...)...get_pack
-00000f00: 6167 655f 726f 6f74 5f64 6972 6300 0000  age_root_dirc...
-00000f10: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000f20: 0043 0000 0073 0e00 0000 7400 7401 7402  .C...s....t.t.t.
-00000f30: 8301 6a03 8301 5300 7219 0000 0029 04da  ..j...S.r....)..
-00000f40: 0373 7472 7202 0000 00da 085f 5f66 696c  .strr......__fil
-00000f50: 655f 5fda 0670 6172 656e 7472 0f00 0000  e__..parentr....
-00000f60: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000f70: 5700 0000 8d00 0000 7302 0000 0000 0172  W.......s......r
-00000f80: 5700 0000 6300 0000 0000 0000 0000 0000  W...c...........
-00000f90: 0000 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00000fa0: 0000 7400 6a01 a002 7403 8300 6401 a102  ..t.j...t...d...
-00000fb0: 5300 2902 4eda 0362 696e 2904 720b 0000  S.).N..bin).r...
-00000fc0: 0072 2300 0000 7244 0000 0072 5700 0000  .r#...rD...rW...
-00000fd0: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000fe0: 1000 0000 da13 6765 745f 7061 636b 6167  ......get_packag
-00000ff0: 655f 6269 6e5f 6469 7291 0000 0073 0200  e_bin_dir....s..
-00001000: 0000 0001 725c 0000 0063 0000 0000 0000  ....r\...c......
-00001010: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00001020: 0000 7324 0000 0074 006a 01a0 0264 01a1  ..s$...t.j...d..
-00001030: 017d 007c 0072 147c 0053 0074 006a 03a0  .}.|.r.|.S.t.j..
-00001040: 0474 0583 0064 02a1 0253 0029 034e 5a0d  .t...d...S.).NZ.
-00001050: 464c 4554 5f57 4542 5f50 4154 48da 0377  FLET_WEB_PATH..w
-00001060: 6562 2906 720b 0000 0072 2700 0000 7228  eb).r....r'...r(
-00001070: 0000 0072 2300 0000 7244 0000 0072 5700  ...r#...rD...rW.
-00001080: 0000 2901 5a0c 7765 625f 726f 6f74 5f64  ..).Z.web_root_d
-00001090: 6972 720f 0000 0072 0f00 0000 7210 0000  irr....r....r...
-000010a0: 00da 1367 6574 5f70 6163 6b61 6765 5f77  ...get_package_w
-000010b0: 6562 5f64 6972 9500 0000 7304 0000 0000  eb_dir....s.....
-000010c0: 010c 0172 5e00 0000 6300 0000 0000 0000  ...r^...c.......
-000010d0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-000010e0: 0073 1e00 0000 7400 a000 a100 7d00 7c00  .s....t.....}.|.
-000010f0: a001 6401 a101 0100 7c00 a002 a100 6402  ..d.....|.....d.
-00001100: 1900 5300 2903 4e29 0272 2e00 0000 7201  ..S.).N).r....r.
-00001110: 0000 00e9 0100 0000 2903 da06 736f 636b  ........)...sock
-00001120: 6574 da04 6269 6e64 da0b 6765 7473 6f63  et..bind..getsoc
-00001130: 6b6e 616d 6529 01da 0473 6f63 6b72 0f00  kname)...sockr..
-00001140: 0000 720f 0000 0072 1000 0000 da11 6765  ..r....r......ge
-00001150: 745f 6672 6565 5f74 6370 5f70 6f72 749a  t_free_tcp_port.
-00001160: 0000 0073 0600 0000 0001 0801 0a01 7264  ...s..........rd
-00001170: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001180: 0300 0000 0800 0000 4300 0000 7376 0000  ........C...sv..
-00001190: 007a 4c74 00a0 0074 006a 0174 006a 02a1  .zLt...t.j.t.j..
-000011a0: 028f 267d 007c 00a0 0364 01a1 0101 007c  ..&}.|...d.....|
-000011b0: 00a0 04a1 0064 0219 007d 0157 0064 0004  .....d...}.W.d..
-000011c0: 0004 0083 0301 006e 1031 0073 3e30 0001  .......n.1.s>0..
-000011d0: 0001 0001 0059 0001 007c 0157 0053 0004  .....Y...|.W.S..
-000011e0: 0074 0579 7001 0001 0001 0074 00a0 06a1  .t.yp......t....
-000011f0: 007d 0274 00a0 077c 02a1 0106 0059 0053  .}.t...|.....Y.S
-00001200: 0030 0064 0053 0029 034e 2902 7a07 382e  .0.d.S.).N).z.8.
-00001210: 382e 382e 38e9 5000 0000 7201 0000 0029  8.8.8.P...r....)
-00001220: 0872 6000 0000 da07 4146 5f49 4e45 54da  .r`.....AF_INET.
-00001230: 0a53 4f43 4b5f 4447 5241 4dda 0763 6f6e  .SOCK_DGRAM..con
-00001240: 6e65 6374 7262 0000 0072 3200 0000 da0b  nectrb...r2.....
-00001250: 6765 7468 6f73 746e 616d 65da 0d67 6574  gethostname..get
-00001260: 686f 7374 6279 6e61 6d65 2903 da01 735a  hostbyname)...sZ
-00001270: 086c 6f63 616c 5f69 70da 0868 6f73 746e  .local_ip..hostn
-00001280: 616d 6572 0f00 0000 720f 0000 0072 1000  amer....r....r..
-00001290: 0000 da0c 6765 745f 6c6f 6361 6c5f 6970  ....get_local_ip
-000012a0: a000 0000 7310 0000 0000 0102 0112 010a  ....s...........
-000012b0: 012a 0106 010c 0108 0172 6d00 0000 6300  .*.......rm...c.
-000012c0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000012d0: 0000 0043 0000 0073 1e00 0000 7400 6a01  ...C...s....t.j.
-000012e0: a002 7403 6a04 6401 1900 a101 7d00 7400  ..t.j.d.....}.t.
-000012f0: 6a01 a005 7c00 a101 5300 2902 4e72 0100  j...|...S.).Nr..
-00001300: 0000 2906 720b 0000 0072 2300 0000 da07  ..).r....r#.....
-00001310: 6469 726e 616d 65da 0373 7973 da04 6172  dirname..sys..ar
-00001320: 6776 7247 0000 0029 01da 0870 6174 686e  gvrG...)...pathn
-00001330: 616d 6572 0f00 0000 720f 0000 0072 1000  amer....r....r..
-00001340: 0000 da16 6765 745f 6375 7272 656e 745f  ....get_current_
-00001350: 7363 7269 7074 5f64 6972 ab00 0000 7304  script_dir....s.
-00001360: 0000 0000 0112 0172 7200 0000 e900 0001  .......rr.......
-00001370: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
-00001380: 0000 0800 0000 4300 0000 7356 0000 0074  ......C...sV...t
-00001390: 00a0 01a1 007d 0274 027c 0064 0183 028f  .....}.t.|.d....
-000013a0: 2c7d 037c 03a0 037c 01a1 017d 047c 0473  ,}.|...|...}.|.s
-000013b0: 2471 307c 02a0 047c 04a1 0101 0071 1457  $q0|...|.....q.W
-000013c0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-000013d0: 4430 0001 0001 0001 0059 0001 007c 02a0  D0.......Y...|..
-000013e0: 05a1 0053 0029 024e da02 7262 2906 da07  ...S.).N..rb)...
-000013f0: 6861 7368 6c69 62da 0673 6861 3235 3672  hashlib..sha256r
-00001400: 2500 0000 7226 0000 00da 0675 7064 6174  %...r&.....updat
-00001410: 65da 0968 6578 6469 6765 7374 2905 7223  e..hexdigest).r#
-00001420: 0000 00da 0962 6c6f 636b 7369 7a65 da01  .....blocksize..
-00001430: 68da 0166 da04 6461 7461 720f 0000 0072  h..f..datar....r
-00001440: 0f00 0000 7210 0000 00da 1363 616c 6375  ....r......calcu
-00001450: 6c61 7465 5f66 696c 655f 6861 7368 b000  late_file_hash..
-00001460: 0000 730e 0000 0000 0108 010c 020a 0104  ..s.............
-00001470: 0102 012a 0172 7d00 0000 6303 0000 0000  ...*.r}...c.....
-00001480: 0000 0000 0000 0003 0000 0007 0000 0043  ...............C
-00001490: 0000 0073 1400 0000 7400 6a01 7c00 7c01  ...s....t.j.|.|.
-000014a0: 7c02 6401 6401 6402 8d05 5300 2903 4e54  |.d.d.d...S.).NT
-000014b0: 2903 da06 6967 6e6f 7265 da08 7379 6d6c  )...ignore..syml
-000014c0: 696e 6b73 da0d 6469 7273 5f65 7869 7374  inks..dirs_exist
-000014d0: 5f6f 6b29 02da 0673 6875 7469 6cda 0863  _ok)...shutil..c
-000014e0: 6f70 7974 7265 6529 03da 0373 7263 da03  opytree)...src..
-000014f0: 6473 7472 7e00 0000 720f 0000 0072 0f00  dstr~...r....r..
-00001500: 0000 7210 0000 00da 0963 6f70 795f 7472  ..r......copy_tr
-00001510: 6565 bb00 0000 7302 0000 0000 0172 8500  ee....s......r..
-00001520: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001530: 0000 0005 0000 0043 0000 0073 2000 0000  .......C...s ...
-00001540: 7400 a001 a100 7d01 7c01 a002 7c00 a003  t.....}.|...|...
-00001550: 6401 a101 a101 0100 7c01 a004 a100 5300  d.......|.....S.
-00001560: 2902 4e7a 0575 7466 2d38 2905 7275 0000  ).Nz.utf-8).ru..
-00001570: 00da 0473 6861 3172 7700 0000 da06 656e  ...sha1rw.....en
-00001580: 636f 6465 7278 0000 0029 025a 0c69 6e70  coderx...).Z.inp
-00001590: 7574 5f73 7472 696e 675a 0973 6861 315f  ut_stringZ.sha1_
-000015a0: 6861 7368 720f 0000 0072 0f00 0000 7210  hashr....r....r.
-000015b0: 0000 0072 8600 0000 bf00 0000 7306 0000  ...r........s...
-000015c0: 0000 0108 0110 0172 8600 0000 2901 4e29  .......r....).N)
-000015d0: 0272 4d00 0000 4e29 0172 7300 0000 2901  .rM...N).rs...).
-000015e0: 4e29 2c72 7500 0000 720b 0000 0072 8100  N),ru...r....r..
-000015f0: 0000 7260 0000 0072 6f00 0000 da07 7061  ..r`...ro.....pa
-00001600: 7468 6c69 6272 0200 0000 da0f 666c 6574  thlibr......flet
-00001610: 5f63 6f72 652e 7479 7065 7372 0300 0000  _core.typesr....
-00001620: 5a17 666c 6574 5f72 756e 7469 6d65 2e75  Z.flet_runtime.u
-00001630: 7469 6c73 2e6f 6e63 6572 0400 0000 5a1e  tils.oncer....Z.
-00001640: 666c 6574 5f72 756e 7469 6d65 2e75 7469  flet_runtime.uti
-00001650: 6c73 2e70 6174 6368 5f69 6e64 6578 7205  ls.patch_indexr.
-00001660: 0000 0072 0600 0000 7258 0000 0072 1100  ...r....rX...r..
-00001670: 0000 7215 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001680: 0072 1a00 0000 721d 0000 0072 3800 0000  .r....r....r8...
-00001690: 721f 0000 0072 2100 0000 722b 0000 0072  r....r!...r+...r
-000016a0: 2d00 0000 7233 0000 0072 3700 0000 723b  -...r3...r7...r;
-000016b0: 0000 0072 4600 0000 724c 0000 0072 5500  ...rF...rL...rU.
-000016c0: 0000 7256 0000 005a 0a66 6c65 742e 7574  ..rV...Z.flet.ut
-000016d0: 696c 7372 5700 0000 da0b 496d 706f 7274  ilsrW.....Import
-000016e0: 4572 726f 7272 5c00 0000 725e 0000 0072  Errorr\...r^...r
-000016f0: 6400 0000 726d 0000 0072 7200 0000 727d  d...rm...rr...r}
-00001700: 0000 0072 8500 0000 7286 0000 0072 0f00  ...r....r....r..
-00001710: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00001720: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001730: 4e00 0000 0801 0801 0801 0801 0801 0c02  N...............
-00001740: 0c01 0c01 1003 0e05 0804 0804 0804 0804  ................
-00001750: 0601 0801 0803 0804 0804 080c 0804 080c  ................
-00001760: 080c 0806 0a11 0809 1009 0809 0201 1001  ................
-00001770: 0e02 0e04 0804 0805 0806 080b 0805 0a0b  ................
-00001780: 0a04                                     ..
+00000290: 2f66 6c65 7463 6f6e 7472 6962 2f73 646b  /fletcontrib/sdk
+000002a0: 2f70 7974 686f 6e2f 7061 636b 6167 6573  /python/packages
+000002b0: 2f66 6c65 742d 7275 6e74 696d 652f 7372  /flet-runtime/sr
+000002c0: 632f 666c 6574 5f72 756e 7469 6d65 2f75  c/flet_runtime/u
+000002d0: 7469 6c73 2f5f 5f69 6e69 745f 5f2e 7079  tils/__init__.py
+000002e0: da10 6765 745f 626f 6f6c 5f65 6e76 5f76  ..get_bool_env_v
+000002f0: 6172 0d00 0000 7304 0000 0000 010a 0172  ar....s........r
+00000300: 1100 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000310: 0000 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
+00000320: 0000 7400 a001 6401 a101 6402 6b02 5300  ..t...d...d.k.S.
+00000330: 2903 4eda 0d46 4c45 545f 504c 4154 464f  ).N..FLET_PLATFO
+00000340: 524d da03 696f 73a9 0272 0b00 0000 720c  RM..ios..r....r.
+00000350: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+00000360: 0000 7210 0000 00da 0669 735f 696f 7312  ..r......is_ios.
+00000370: 0000 0073 0200 0000 0001 7215 0000 0063  ...s......r....c
+00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000390: 0300 0000 4300 0000 730e 0000 0074 00a0  ....C...s....t..
+000003a0: 0164 01a1 0164 026b 0253 0029 034e 7212  .d...d.k.S.).Nr.
+000003b0: 0000 00da 0761 6e64 726f 6964 7214 0000  .....androidr...
+000003c0: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+000003d0: 7210 0000 00da 0a69 735f 616e 6472 6f69  r......is_androi
+000003e0: 6416 0000 0073 0200 0000 0001 7217 0000  d....s......r...
+000003f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000400: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
+00000410: 00a0 0164 01a1 0164 0075 0153 0029 024e  ...d...d.u.S.).N
+00000420: 7212 0000 0072 1400 0000 720f 0000 0072  r....r....r....r
+00000430: 0f00 0000 720f 0000 0072 1000 0000 da0b  ....r....r......
+00000440: 6973 5f65 6d62 6564 6465 641a 0000 0073  is_embedded....s
+00000450: 0200 0000 0001 7218 0000 0063 0000 0000  ......r....c....
+00000460: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000470: 4300 0000 730c 0000 0074 0083 0070 0a74  C...s....t...p.t
+00000480: 0183 0053 00a9 014e 2902 7215 0000 0072  ...S...N).r....r
+00000490: 1700 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
+000004a0: 0000 0072 1000 0000 da09 6973 5f6d 6f62  ...r......is_mob
+000004b0: 696c 651e 0000 0073 0200 0000 0001 721a  ile....s......r.
+000004c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000004d0: 0000 0000 0200 0000 4300 0000 7314 0000  ........C...s...
+000004e0: 0074 0083 000c 006f 1274 01a0 02a1 0064  .t.....o.t.....d
+000004f0: 016b 0253 0029 024e da07 5769 6e64 6f77  .k.S.).N..Window
+00000500: 73a9 0372 1a00 0000 da08 706c 6174 666f  s..r......platfo
+00000510: 726d da06 7379 7374 656d 720f 0000 0072  rm..systemr....r
+00000520: 0f00 0000 720f 0000 0072 1000 0000 da0a  ....r....r......
+00000530: 6973 5f77 696e 646f 7773 2700 0000 7302  is_windows'...s.
+00000540: 0000 0000 0172 1f00 0000 6300 0000 0000  .....r....c.....
+00000550: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+00000560: 0000 0073 1400 0000 7400 8300 0c00 6f12  ...s....t.....o.
+00000570: 7401 a002 a100 6401 6b02 5300 2902 4eda  t.....d.k.S.).N.
+00000580: 054c 696e 7578 721c 0000 0072 0f00 0000  .Linuxr....r....
+00000590: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+000005a0: 0869 735f 6c69 6e75 782b 0000 0073 0200  .is_linux+...s..
+000005b0: 0000 0001 7221 0000 0063 0000 0000 0000  ....r!...c......
+000005c0: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
+000005d0: 0000 737c 0000 0074 0083 0073 7874 01a0  ..s|...t...sxt..
+000005e0: 02a1 0064 016b 0272 7864 027d 0074 036a  ...d.k.rxd.}.t.j
+000005f0: 04a0 057c 00a1 0172 6874 067c 0064 0383  ...|...rht.|.d..
+00000600: 028f 2c7d 0164 047c 01a0 07a1 0076 0072  ..,}.d.|.....v.r
+00000610: 4a57 0064 0004 0004 0083 0301 0064 0553  JW.d.........d.S
+00000620: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00000630: 0073 5e30 0001 0001 0001 0059 0001 0074  .s^0.......Y...t
+00000640: 036a 08a0 0964 06a1 0164 0075 0053 0064  .j...d...d.u.S.d
+00000650: 0553 0029 074e 7220 0000 007a 0d2f 7072  .S.).Nr ...z./pr
+00000660: 6f63 2f76 6572 7369 6f6e da01 725a 096d  oc/version..rZ.m
+00000670: 6963 726f 736f 6674 465a 0744 4953 504c  icrosoftFZ.DISPL
+00000680: 4159 290a 721a 0000 0072 1d00 0000 721e  AY).r....r....r.
+00000690: 0000 0072 0b00 0000 da04 7061 7468 da06  ...r......path..
+000006a0: 6578 6973 7473 da04 6f70 656e da04 7265  exists..open..re
+000006b0: 6164 da07 656e 7669 726f 6eda 0367 6574  ad..environ..get
+000006c0: 2902 da01 70da 0466 696c 6572 0f00 0000  )...p..filer....
+000006d0: 720f 0000 0072 1000 0000 da0f 6973 5f6c  r....r......is_l
+000006e0: 696e 7578 5f73 6572 7665 722f 0000 0073  inux_server/...s
+000006f0: 1000 0000 0001 1202 0401 0c01 0c01 0c01  ................
+00000700: 2e01 1001 722b 0000 0063 0000 0000 0000  ....r+...c......
+00000710: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00000720: 0000 7314 0000 0074 0083 000c 006f 1274  ..s....t.....o.t
+00000730: 01a0 02a1 0064 016b 0253 0029 024e da06  .....d.k.S.).N..
+00000740: 4461 7277 696e 721c 0000 0072 0f00 0000  Darwinr....r....
+00000750: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00000760: 0869 735f 6d61 636f 733b 0000 0073 0200  .is_macos;...s..
+00000770: 0000 0001 722d 0000 0063 0000 0000 0000  ....r-...c......
+00000780: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000790: 0000 7346 0000 0074 0083 0073 0e74 01a0  ..sF...t...s.t..
+000007a0: 02a1 006e 0264 017d 0074 0383 0072 1c64  ...n.d.}.t...r.d
+000007b0: 0253 007c 0064 036b 0272 2864 0453 007c  .S.|.d.k.r(d.S.|
+000007c0: 0064 056b 0272 3464 0653 0074 0464 077c  .d.k.r4d.S.t.d.|
+000007d0: 009b 009d 0283 0182 0164 0053 0029 084e  .........d.S.).N
+000007e0: da00 da07 7769 6e64 6f77 7372 2000 0000  ....windowsr ...
+000007f0: da05 6c69 6e75 7872 2c00 0000 da06 6461  ..linuxr,.....da
+00000800: 7277 696e 7a16 556e 7375 7070 6f72 7465  rwinz.Unsupporte
+00000810: 6420 706c 6174 666f 726d 3a20 2905 721a  d platform: ).r.
+00000820: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000830: 0000 da09 4578 6365 7074 696f 6e29 0172  ....Exception).r
+00000840: 2900 0000 720f 0000 0072 0f00 0000 7210  )...r....r....r.
+00000850: 0000 00da 0c67 6574 5f70 6c61 7466 6f72  .....get_platfor
+00000860: 6d3f 0000 0073 1000 0000 0001 1201 0601  m?...s..........
+00000870: 0401 0801 0401 0801 0402 7233 0000 0063  ..........r3...c
+00000880: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000890: 0300 0000 4300 0000 735e 0000 0074 0083  ....C...s^...t..
+000008a0: 0073 1274 01a0 02a1 00a0 03a1 006e 0264  .s.t.........n.d
+000008b0: 017d 007c 0064 026b 0273 267c 0064 036b  .}.|.d.k.s&|.d.k
+000008c0: 0272 2a64 0353 007c 0064 046b 0273 3a7c  .r*d.S.|.d.k.s:|
+000008d0: 0064 056b 0272 3e64 0453 007c 00a0 0464  .d.k.r>d.S.|...d
+000008e0: 06a1 0172 4c64 0753 0074 0564 087c 009b  ...rLd.S.t.d.|..
+000008f0: 009d 0283 0182 0164 0053 0029 094e 722e  .......d.S.).Nr.
+00000900: 0000 005a 0678 3836 5f36 345a 0561 6d64  ...Z.x86_64Z.amd
+00000910: 3634 5a05 6172 6d36 345a 0761 6172 6368  64Z.arm64Z.aarch
+00000920: 3634 5a03 6172 6d5a 0561 726d 5f37 7a1a  64Z.armZ.arm_7z.
+00000930: 556e 7375 7070 6f72 7465 6420 6172 6368  Unsupported arch
+00000940: 6974 6563 7475 7265 3a20 2906 721a 0000  itecture: ).r...
+00000950: 0072 1d00 0000 da07 6d61 6368 696e 6572  .r......machiner
+00000960: 0d00 0000 da0a 7374 6172 7473 7769 7468  ......startswith
+00000970: 7232 0000 0029 01da 0161 720f 0000 0072  r2...)...ar....r
+00000980: 0f00 0000 7210 0000 00da 0867 6574 5f61  ....r......get_a
+00000990: 7263 684b 0000 0073 1000 0000 0001 1601  rchK...s........
+000009a0: 1001 0401 1001 0401 0a01 0402 7237 0000  ............r7..
+000009b0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+000009c0: 0000 0300 0000 4300 0000 7314 0000 0074  ......C...s....t
+000009d0: 0083 0073 1074 01a0 027c 00a1 0101 0064  ...s.t...|.....d
+000009e0: 0053 0072 1900 0000 2903 721a 0000 00da  .S.r....).r.....
+000009f0: 0a77 6562 6272 6f77 7365 7272 2500 0000  .webbrowserr%...
+00000a00: a901 da03 7572 6c72 0f00 0000 720f 0000  ....urlr....r...
+00000a10: 0072 1000 0000 da0f 6f70 656e 5f69 6e5f  .r......open_in_
+00000a20: 6272 6f77 7365 7257 0000 0073 0400 0000  browserW...s....
+00000a30: 0001 0601 723b 0000 0063 0200 0000 0000  ....r;...c......
+00000a40: 0000 0000 0000 0500 0000 0500 0000 0300  ................
+00000a50: 0000 736e 0000 0064 0164 006c 0089 0087  ..sn...d.d.l....
+00000a60: 0066 0164 0264 0384 087d 0288 006a 0164  .f.d.d...}...j.d
+00000a70: 0419 00a0 0288 006a 03a1 0144 005d 427d  .......j...D.]B}
+00000a80: 0388 006a 04a0 057c 037c 00a1 027d 047c  ...j...|.|...}.|
+00000a90: 027c 0483 0172 267c 0164 0075 0073 607c  .|...r&|.d.u.s`|
+00000aa0: 0164 0075 0172 267c 01a0 06a1 007c 04a0  .d.u.r&|.....|..
+00000ab0: 06a1 006b 0372 267c 0402 0001 0053 0071  ...k.r&|.....S.q
+00000ac0: 2664 0053 0029 054e 7201 0000 0063 0100  &d.S.).Nr....c..
+00000ad0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000ae0: 0000 1300 0000 731a 0000 0088 006a 00a0  ......s......j..
+00000af0: 017c 00a1 016f 1888 00a0 027c 0088 006a  .|...o.....|...j
+00000b00: 03a1 0253 0072 1900 0000 2904 7223 0000  ...S.r....).r#..
+00000b10: 00da 0669 7366 696c 65da 0661 6363 6573  ...isfile..acces
+00000b20: 73da 0458 5f4f 4b29 015a 0566 7061 7468  s..X_OK).Z.fpath
+00000b30: a901 720b 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000b40: 00da 0669 735f 6578 6560 0000 0073 0200  ...is_exe`...s..
+00000b50: 0000 0001 7a15 7768 6963 682e 3c6c 6f63  ....z.which.<loc
+00000b60: 616c 733e 2e69 735f 6578 65da 0450 4154  als>.is_exe..PAT
+00000b70: 4829 0772 0b00 0000 7227 0000 00da 0573  H).r....r'.....s
+00000b80: 706c 6974 da07 7061 7468 7365 7072 2300  plit..pathsepr#.
+00000b90: 0000 da04 6a6f 696e 720d 0000 0029 05da  ....joinr....)..
+00000ba0: 0770 726f 6772 616d 5a0b 6578 636c 7564  .programZ.exclud
+00000bb0: 655f 6578 6572 4000 0000 7223 0000 005a  e_exer@...r#...Z
+00000bc0: 0865 7865 5f66 696c 6572 0f00 0000 723f  .exe_filer....r?
+00000bd0: 0000 0072 1000 0000 da05 7768 6963 685d  ...r......which]
+00000be0: 0000 0073 1a00 0000 0001 0802 0c03 1601  ...s............
+00000bf0: 0e01 0801 06ff 0202 06fe 0202 0efe 0204  ................
+00000c00: 0a02 7246 0000 0063 0200 0000 0000 0000  ..rF...c........
+00000c10: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00000c20: 7330 0000 0074 006a 01a0 027c 00a1 017d  s0...t.j...|...}
+00000c30: 0274 006a 01a0 027c 01a1 017d 0374 006a  .t.j...|...}.t.j
+00000c40: 01a0 037c 027c 0367 02a1 017d 047c 047c  ...|.|.g...}.|.|
+00000c50: 026b 0253 0072 1900 0000 2904 720b 0000  .k.S.r....).r...
+00000c60: 0072 2300 0000 da07 6162 7370 6174 68da  .r#.....abspath.
+00000c70: 0c63 6f6d 6d6f 6e70 7265 6669 7829 05da  .commonprefix)..
+00000c80: 0964 6972 6563 746f 7279 da06 7461 7267  .directory..targ
+00000c90: 6574 5a0d 6162 735f 6469 7265 6374 6f72  etZ.abs_director
+00000ca0: 795a 0a61 6273 5f74 6172 6765 74da 0670  yZ.abs_target..p
+00000cb0: 7265 6669 7872 0f00 0000 720f 0000 0072  refixr....r....r
+00000cc0: 1000 0000 da13 6973 5f77 6974 6869 6e5f  ......is_within_
+00000cd0: 6469 7265 6374 6f72 796e 0000 0073 0800  directoryn...s..
+00000ce0: 0000 0001 0c01 0c02 1002 724c 0000 00da  ..........rL....
+00000cf0: 012e 46a9 01da 0d6e 756d 6572 6963 5f6f  ..F....numeric_o
+00000d00: 776e 6572 6303 0000 0000 0000 0001 0000  wnerc...........
+00000d10: 0006 0000 0005 0000 0043 0000 0073 4400  .........C...sD.
+00000d20: 0000 7c00 a000 a100 4400 5d26 7d04 7401  ..|.....D.]&}.t.
+00000d30: 6a02 a003 7c01 7c04 6a04 a102 7d05 7405  j...|.|.j...}.t.
+00000d40: 7c01 7c05 8302 7308 7406 6401 8301 8201  |.|...s.t.d.....
+00000d50: 7108 7c00 6a07 7c01 7c02 7c03 6402 8d03  q.|.j.|.|.|.d...
+00000d60: 0100 6400 5300 2903 4e7a 2441 7474 656d  ..d.S.).Nz$Attem
+00000d70: 7074 6564 2050 6174 6820 5472 6176 6572  pted Path Traver
+00000d80: 7361 6c20 696e 2054 6172 2046 696c 6572  sal in Tar Filer
+00000d90: 4e00 0000 2908 da0a 6765 746d 656d 6265  N...)...getmembe
+00000da0: 7273 720b 0000 0072 2300 0000 7244 0000  rsr....r#...rD..
+00000db0: 0072 0700 0000 724c 0000 0072 3200 0000  .r....rL...r2...
+00000dc0: da0a 6578 7472 6163 7461 6c6c 2906 da03  ..extractall)...
+00000dd0: 7461 7272 2300 0000 da07 6d65 6d62 6572  tarr#.....member
+00000de0: 7372 4f00 0000 da06 6d65 6d62 6572 5a0b  srO.....memberZ.
+00000df0: 6d65 6d62 6572 5f70 6174 6872 0f00 0000  member_pathr....
+00000e00: 720f 0000 0072 1000 0000 da13 7361 6665  r....r......safe
+00000e10: 5f74 6172 5f65 7874 7261 6374 616c 6c77  _tar_extractallw
+00000e20: 0000 0073 0a00 0000 0001 0c01 1001 0a01  ...s............
+00000e30: 0a02 7255 0000 0063 0100 0000 0000 0000  ..rU...c........
+00000e40: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000e50: 7320 0000 0064 017c 0076 0070 1e64 027c  s ...d.|.v.p.d.|
+00000e60: 0076 0070 1e64 037c 0076 0070 1e64 047c  .v.p.d.|.v.p.d.|
+00000e70: 0076 0053 0029 054e 7a0d 3a2f 2f6c 6f63  .v.S.).Nz.://loc
+00000e80: 616c 686f 7374 2f7a 0d3a 2f2f 6c6f 6361  alhost/z.://loca
+00000e90: 6c68 6f73 743a 7a0d 3a2f 2f31 3237 2e30  lhost:z.://127.0
+00000ea0: 2e30 2e31 2f7a 0d3a 2f2f 3132 372e 302e  .0.1/z.://127.0.
+00000eb0: 302e 313a 720f 0000 0072 3900 0000 720f  0.1:r....r9...r.
+00000ec0: 0000 0072 0f00 0000 7210 0000 00da 1069  ...r....r......i
+00000ed0: 735f 6c6f 6361 6c68 6f73 745f 7572 6c80  s_localhost_url.
+00000ee0: 0000 0073 0e00 0000 0002 0801 06ff 0202  ...s............
+00000ef0: 06fe 0203 06fc 7256 0000 0029 01da 1467  ......rV...)...g
+00000f00: 6574 5f70 6163 6b61 6765 5f72 6f6f 745f  et_package_root_
+00000f10: 6469 7263 0000 0000 0000 0000 0000 0000  dirc............
+00000f20: 0000 0000 0300 0000 4300 0000 730e 0000  ........C...s...
+00000f30: 0074 0074 0174 0283 016a 0383 0153 0072  .t.t.t...j...S.r
+00000f40: 1900 0000 2904 da03 7374 7272 0200 0000  ....)...strr....
+00000f50: da08 5f5f 6669 6c65 5f5f da06 7061 7265  ..__file__..pare
+00000f60: 6e74 720f 0000 0072 0f00 0000 720f 0000  ntr....r....r...
+00000f70: 0072 1000 0000 7257 0000 008d 0000 0073  .r....rW.......s
+00000f80: 0200 0000 0001 7257 0000 0063 0000 0000  ......rW...c....
+00000f90: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000fa0: 4300 0000 7310 0000 0074 006a 01a0 0274  C...s....t.j...t
+00000fb0: 0383 0064 01a1 0253 0029 024e da03 6269  ...d...S.).N..bi
+00000fc0: 6e29 0472 0b00 0000 7223 0000 0072 4400  n).r....r#...rD.
+00000fd0: 0000 7257 0000 0072 0f00 0000 720f 0000  ..rW...r....r...
+00000fe0: 0072 0f00 0000 7210 0000 00da 1367 6574  .r....r......get
+00000ff0: 5f70 6163 6b61 6765 5f62 696e 5f64 6972  _package_bin_dir
+00001000: 9100 0000 7302 0000 0000 0172 5c00 0000  ....s......r\...
+00001010: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
+00001020: 0004 0000 0043 0000 0073 2400 0000 7400  .....C...s$...t.
+00001030: 6a01 a002 6401 a101 7d00 7c00 7214 7c00  j...d...}.|.r.|.
+00001040: 5300 7400 6a03 a004 7405 8300 6402 a102  S.t.j...t...d...
+00001050: 5300 2903 4e5a 0d46 4c45 545f 5745 425f  S.).NZ.FLET_WEB_
+00001060: 5041 5448 da03 7765 6229 0672 0b00 0000  PATH..web).r....
+00001070: 7227 0000 0072 2800 0000 7223 0000 0072  r'...r(...r#...r
+00001080: 4400 0000 7257 0000 0029 015a 0c77 6562  D...rW...).Z.web
+00001090: 5f72 6f6f 745f 6469 7272 0f00 0000 720f  _root_dirr....r.
+000010a0: 0000 0072 1000 0000 da13 6765 745f 7061  ...r......get_pa
+000010b0: 636b 6167 655f 7765 625f 6469 7295 0000  ckage_web_dir...
+000010c0: 0073 0400 0000 0001 0c01 725e 0000 0063  .s........r^...c
+000010d0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+000010e0: 0300 0000 4300 0000 731e 0000 0074 00a0  ....C...s....t..
+000010f0: 00a1 007d 007c 00a0 0164 01a1 0101 007c  ...}.|...d.....|
+00001100: 00a0 02a1 0064 0219 0053 0029 034e 2902  .....d...S.).N).
+00001110: 722e 0000 0072 0100 0000 e901 0000 0029  r....r.........)
+00001120: 03da 0673 6f63 6b65 74da 0462 696e 64da  ...socket..bind.
+00001130: 0b67 6574 736f 636b 6e61 6d65 2901 da04  .getsockname)...
+00001140: 736f 636b 720f 0000 0072 0f00 0000 7210  sockr....r....r.
+00001150: 0000 00da 1167 6574 5f66 7265 655f 7463  .....get_free_tc
+00001160: 705f 706f 7274 9a00 0000 7306 0000 0000  p_port....s.....
+00001170: 0108 010a 0172 6400 0000 6300 0000 0000  .....rd...c.....
+00001180: 0000 0000 0000 0003 0000 0008 0000 0043  ...............C
+00001190: 0000 0073 7600 0000 7a4c 7400 a000 7400  ...sv...zLt...t.
+000011a0: 6a01 7400 6a02 a102 8f26 7d00 7c00 a003  j.t.j....&}.|...
+000011b0: 6401 a101 0100 7c00 a004 a100 6402 1900  d.....|.....d...
+000011c0: 7d01 5700 6400 0400 0400 8303 0100 6e10  }.W.d.........n.
+000011d0: 3100 733e 3000 0100 0100 0100 5900 0100  1.s>0.......Y...
+000011e0: 7c01 5700 5300 0400 7405 7970 0100 0100  |.W.S...t.yp....
+000011f0: 0100 7400 a006 a100 7d02 7400 a007 7c02  ..t.....}.t...|.
+00001200: a101 0600 5900 5300 3000 6400 5300 2903  ....Y.S.0.d.S.).
+00001210: 4e29 027a 0738 2e38 2e38 2e38 e950 0000  N).z.8.8.8.8.P..
+00001220: 0072 0100 0000 2908 7260 0000 00da 0741  .r....).r`.....A
+00001230: 465f 494e 4554 da0a 534f 434b 5f44 4752  F_INET..SOCK_DGR
+00001240: 414d da07 636f 6e6e 6563 7472 6200 0000  AM..connectrb...
+00001250: 7232 0000 00da 0b67 6574 686f 7374 6e61  r2.....gethostna
+00001260: 6d65 da0d 6765 7468 6f73 7462 796e 616d  me..gethostbynam
+00001270: 6529 03da 0173 5a08 6c6f 6361 6c5f 6970  e)...sZ.local_ip
+00001280: da08 686f 7374 6e61 6d65 720f 0000 0072  ..hostnamer....r
+00001290: 0f00 0000 7210 0000 00da 0c67 6574 5f6c  ....r......get_l
+000012a0: 6f63 616c 5f69 70a0 0000 0073 1000 0000  ocal_ip....s....
+000012b0: 0001 0201 1201 0a01 2a01 0601 0c01 0801  ........*.......
+000012c0: 726d 0000 0063 0000 0000 0000 0000 0000  rm...c..........
+000012d0: 0000 0100 0000 0400 0000 4300 0000 731e  ..........C...s.
+000012e0: 0000 0074 006a 01a0 0274 036a 0464 0119  ...t.j...t.j.d..
+000012f0: 00a1 017d 0074 006a 01a0 057c 00a1 0153  ...}.t.j...|...S
+00001300: 0029 024e 7201 0000 0029 0672 0b00 0000  .).Nr....).r....
+00001310: 7223 0000 00da 0764 6972 6e61 6d65 da03  r#.....dirname..
+00001320: 7379 73da 0461 7267 7672 4700 0000 2901  sys..argvrG...).
+00001330: da08 7061 7468 6e61 6d65 720f 0000 0072  ..pathnamer....r
+00001340: 0f00 0000 7210 0000 00da 1667 6574 5f63  ....r......get_c
+00001350: 7572 7265 6e74 5f73 6372 6970 745f 6469  urrent_script_di
+00001360: 72ab 0000 0073 0400 0000 0001 1201 7272  r....s........rr
+00001370: 0000 00e9 0000 0100 6302 0000 0000 0000  ........c.......
+00001380: 0000 0000 0005 0000 0008 0000 0043 0000  .............C..
+00001390: 0073 5600 0000 7400 a001 a100 7d02 7402  .sV...t.....}.t.
+000013a0: 7c00 6401 8302 8f2c 7d03 7c03 a003 7c01  |.d....,}.|...|.
+000013b0: a101 7d04 7c04 7324 7130 7c02 a004 7c04  ..}.|.s$q0|...|.
+000013c0: a101 0100 7114 5700 6400 0400 0400 8303  ....q.W.d.......
+000013d0: 0100 6e10 3100 7344 3000 0100 0100 0100  ..n.1.sD0.......
+000013e0: 5900 0100 7c02 a005 a100 5300 2902 4eda  Y...|.....S.).N.
+000013f0: 0272 6229 06da 0768 6173 686c 6962 da06  .rb)...hashlib..
+00001400: 7368 6132 3536 7225 0000 0072 2600 0000  sha256r%...r&...
+00001410: da06 7570 6461 7465 da09 6865 7864 6967  ..update..hexdig
+00001420: 6573 7429 0572 2300 0000 da09 626c 6f63  est).r#.....bloc
+00001430: 6b73 697a 65da 0168 da01 66da 0464 6174  ksize..h..f..dat
+00001440: 6172 0f00 0000 720f 0000 0072 1000 0000  ar....r....r....
+00001450: da13 6361 6c63 756c 6174 655f 6669 6c65  ..calculate_file
+00001460: 5f68 6173 68b0 0000 0073 0e00 0000 0001  _hash....s......
+00001470: 0801 0c02 0a01 0401 0201 2a01 727d 0000  ..........*.r}..
+00001480: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+00001490: 0000 0700 0000 4300 0000 7314 0000 0074  ......C...s....t
+000014a0: 006a 017c 007c 017c 0264 0164 0164 028d  .j.|.|.|.d.d.d..
+000014b0: 0553 0029 034e 5429 03da 0669 676e 6f72  .S.).NT)...ignor
+000014c0: 65da 0873 796d 6c69 6e6b 73da 0d64 6972  e..symlinks..dir
+000014d0: 735f 6578 6973 745f 6f6b 2902 da06 7368  s_exist_ok)...sh
+000014e0: 7574 696c da08 636f 7079 7472 6565 2903  util..copytree).
+000014f0: da03 7372 63da 0364 7374 727e 0000 0072  ..src..dstr~...r
+00001500: 0f00 0000 720f 0000 0072 1000 0000 da09  ....r....r......
+00001510: 636f 7079 5f74 7265 65bb 0000 0073 0200  copy_tree....s..
+00001520: 0000 0001 7285 0000 0063 0100 0000 0000  ....r....c......
+00001530: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00001540: 0000 7320 0000 0074 00a0 01a1 007d 017c  ..s ...t.....}.|
+00001550: 01a0 027c 00a0 0364 01a1 01a1 0101 007c  ...|...d.......|
+00001560: 01a0 04a1 0053 0029 024e 7a05 7574 662d  .....S.).Nz.utf-
+00001570: 3829 0572 7500 0000 da04 7368 6131 7277  8).ru.....sha1rw
+00001580: 0000 00da 0665 6e63 6f64 6572 7800 0000  .....encoderx...
+00001590: 2902 5a0c 696e 7075 745f 7374 7269 6e67  ).Z.input_string
+000015a0: 5a09 7368 6131 5f68 6173 6872 0f00 0000  Z.sha1_hashr....
+000015b0: 720f 0000 0072 1000 0000 7286 0000 00bf  r....r....r.....
+000015c0: 0000 0073 0600 0000 0001 0801 1001 7286  ...s..........r.
+000015d0: 0000 0029 014e 2902 724d 0000 004e 2901  ...).N).rM...N).
+000015e0: 7273 0000 0029 014e 292c 7275 0000 0072  rs...).N),ru...r
+000015f0: 0b00 0000 7281 0000 0072 6000 0000 726f  ....r....r`...ro
+00001600: 0000 00da 0770 6174 686c 6962 7202 0000  .....pathlibr...
+00001610: 00da 0f66 6c65 745f 636f 7265 2e74 7970  ...flet_core.typ
+00001620: 6573 7203 0000 005a 1766 6c65 745f 7275  esr....Z.flet_ru
+00001630: 6e74 696d 652e 7574 696c 732e 6f6e 6365  ntime.utils.once
+00001640: 7204 0000 005a 1e66 6c65 745f 7275 6e74  r....Z.flet_runt
+00001650: 696d 652e 7574 696c 732e 7061 7463 685f  ime.utils.patch_
+00001660: 696e 6465 7872 0500 0000 7206 0000 0072  indexr....r....r
+00001670: 5800 0000 7211 0000 0072 1500 0000 7217  X...r....r....r.
+00001680: 0000 0072 1800 0000 721a 0000 0072 1d00  ...r....r....r..
+00001690: 0000 7238 0000 0072 1f00 0000 7221 0000  ..r8...r....r!..
+000016a0: 0072 2b00 0000 722d 0000 0072 3300 0000  .r+...r-...r3...
+000016b0: 7237 0000 0072 3b00 0000 7246 0000 0072  r7...r;...rF...r
+000016c0: 4c00 0000 7255 0000 0072 5600 0000 5a0a  L...rU...rV...Z.
+000016d0: 666c 6574 2e75 7469 6c73 7257 0000 00da  flet.utilsrW....
+000016e0: 0b49 6d70 6f72 7445 7272 6f72 725c 0000  .ImportErrorr\..
+000016f0: 0072 5e00 0000 7264 0000 0072 6d00 0000  .r^...rd...rm...
+00001700: 7272 0000 0072 7d00 0000 7285 0000 0072  rr...r}...r....r
+00001710: 8600 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
+00001720: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
+00001730: 653e 0100 0000 734e 0000 0008 0108 0108  e>....sN........
+00001740: 0108 0108 010c 020c 010c 0110 030e 0508  ................
+00001750: 0408 0408 0408 0406 0108 0108 0308 0408  ................
+00001760: 0408 0c08 0408 0c08 0c08 060a 1108 0910  ................
+00001770: 0908 0902 0110 010e 020e 0408 0408 0508  ................
+00001780: 0608 0b08 050a 0b0a 04                   .........
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 347 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 5b01 0000  a........9)f[...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 5b01 0000  a........./f[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
 00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
 00000080: 6404 8400 5a04 6405 5300 2906 da04 4f6e  d...Z.d.S.)...On
 00000090: 6365 6301 0000 0000 0000 0000 0000 0001  cec.............
 000000a0: 0000 0002 0000 0043 0000 0073 1400 0000  .......C...s....
 000000b0: 7400 a001 a100 7c00 5f02 6401 7c00 5f03  t.....|._.d.|._.
 000000c0: 6400 5300 2902 4e46 2904 da07 6173 796e  d.S.).NF)...asyn
 000000d0: 6369 6fda 044c 6f63 6bda 055f 6c6f 636b  cio..Lock.._lock
 000000e0: da05 5f64 6f6e 6529 01da 0473 656c 66a9  .._done)...self.
-000000f0: 0072 0800 0000 fa5c 2f77 6f72 6b73 7061  .r.....\/workspa
+000000f0: 0072 0800 0000 fa63 2f77 6f72 6b73 7061  .r.....c/workspa
 00000100: 6365 732f 636f 6e74 7269 6266 6c65 742f  ces/contribflet/
-00000110: 666c 6574 2f73 646b 2f70 7974 686f 6e2f  flet/sdk/python/
-00000120: 7061 636b 6167 6573 2f66 6c65 742d 7275  packages/flet-ru
-00000130: 6e74 696d 652f 7372 632f 666c 6574 5f72  ntime/src/flet_r
-00000140: 756e 7469 6d65 2f75 7469 6c73 2f6f 6e63  untime/utils/onc
-00000150: 652e 7079 da08 5f5f 696e 6974 5f5f 0500  e.py..__init__..
-00000160: 0000 7304 0000 0000 010a 017a 0d4f 6e63  ..s........z.Onc
-00000170: 652e 5f5f 696e 6974 5f5f 6302 0000 0000  e.__init__c.....
-00000180: 0000 0000 0000 0004 0000 0009 0000 00cf  ................
-00000190: 0000 0073 6400 0000 7c00 6a00 7360 7c00  ...sd...|.j.s`|.
-000001a0: 6a01 3400 4900 6400 4800 9a36 0100 7c00  j.4.I.d.H..6..|.
-000001b0: 6a00 7336 7c01 7c02 6900 7c03 a401 8e01  j.s6|.|.i.|.....
-000001c0: 4900 6400 4800 0100 6401 7c00 5f00 5700  I.d.H...d.|._.W.
-000001d0: 6400 0400 0400 8303 4900 6400 4800 0100  d.......I.d.H...
-000001e0: 7160 3100 4900 6400 4800 7356 3000 0100  q`1.I.d.H.sV0...
-000001f0: 0100 0100 5900 0100 6400 5300 2902 4e54  ....Y...d.S.).NT
-00000200: 2902 7206 0000 0072 0500 0000 2904 7207  ).r....r....).r.
-00000210: 0000 00da 0466 756e 63da 0461 7267 73da  .....func..args.
-00000220: 066b 7761 7267 7372 0800 0000 7208 0000  .kwargsr....r...
-00000230: 0072 0900 0000 da02 646f 0900 0000 730a  .r......do....s.
-00000240: 0000 0000 0106 0110 0106 0114 017a 074f  .............z.O
-00000250: 6e63 652e 646f 4e29 05da 085f 5f6e 616d  nce.doN)...__nam
-00000260: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000270: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0a00  .__qualname__r..
-00000280: 0000 720e 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00000290: 0072 0800 0000 7209 0000 0072 0200 0000  .r....r....r....
-000002a0: 0400 0000 7304 0000 0008 0108 0472 0200  ....s........r..
-000002b0: 0000 2902 7203 0000 0072 0200 0000 7208  ..).r....r....r.
-000002c0: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-000002d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000002e0: 7302 0000 0008 03                        s......
+00000110: 666c 6574 636f 6e74 7269 622f 7364 6b2f  fletcontrib/sdk/
+00000120: 7079 7468 6f6e 2f70 6163 6b61 6765 732f  python/packages/
+00000130: 666c 6574 2d72 756e 7469 6d65 2f73 7263  flet-runtime/src
+00000140: 2f66 6c65 745f 7275 6e74 696d 652f 7574  /flet_runtime/ut
+00000150: 696c 732f 6f6e 6365 2e70 79da 085f 5f69  ils/once.py..__i
+00000160: 6e69 745f 5f05 0000 0073 0400 0000 0001  nit__....s......
+00000170: 0a01 7a0d 4f6e 6365 2e5f 5f69 6e69 745f  ..z.Once.__init_
+00000180: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
+00000190: 0000 0900 0000 cf00 0000 7364 0000 007c  ..........sd...|
+000001a0: 006a 0073 607c 006a 0134 0049 0064 0048  .j.s`|.j.4.I.d.H
+000001b0: 009a 3601 007c 006a 0073 367c 017c 0269  ..6..|.j.s6|.|.i
+000001c0: 007c 03a4 018e 0149 0064 0048 0001 0064  .|.....I.d.H...d
+000001d0: 017c 005f 0057 0064 0004 0004 0083 0349  .|._.W.d.......I
+000001e0: 0064 0048 0001 0071 6031 0049 0064 0048  .d.H...q`1.I.d.H
+000001f0: 0073 5630 0001 0001 0001 0059 0001 0064  .sV0.......Y...d
+00000200: 0053 0029 024e 5429 0272 0600 0000 7205  .S.).NT).r....r.
+00000210: 0000 0029 0472 0700 0000 da04 6675 6e63  ...).r......func
+00000220: da04 6172 6773 da06 6b77 6172 6773 7208  ..args..kwargsr.
+00000230: 0000 0072 0800 0000 7209 0000 00da 0264  ...r....r......d
+00000240: 6f09 0000 0073 0a00 0000 0001 0601 1001  o....s..........
+00000250: 0601 1401 7a07 4f6e 6365 2e64 6f4e 2905  ....z.Once.doN).
+00000260: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000270: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000280: 6d65 5f5f 720a 0000 0072 0e00 0000 7208  me__r....r....r.
+00000290: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
+000002a0: 0000 7202 0000 0004 0000 0073 0400 0000  ..r........s....
+000002b0: 0801 0804 7202 0000 0029 0272 0300 0000  ....r....).r....
+000002c0: 7202 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
+000002d0: 0800 0000 7209 0000 00da 083c 6d6f 6475  ....r......<modu
+000002e0: 6c65 3e01 0000 0073 0200 0000 0803       le>....s......
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:56:25 2024 UTC, .py size: 3202 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b939 2966 820c 0000  a........9)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 820c 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6401 6401 6405 6405 6406 6507  ..d.d.d.d.d.d.e.
 00000070: 6a08 6405 6407 6609 6509 6509 6505 6509  j.d.d.f.e.e.e.e.
@@ -108,63 +108,64 @@
 000006b0: 62da 0577 7269 7465 2910 7207 0000 0072  b..write).r....r
 000006c0: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
 000006d0: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
 000006e0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
 000006f0: 00da 0166 da05 696e 6465 78da 0b6d 6f64  ...f..index..mod
 00000700: 756c 655f 6e61 6d65 5a0b 7079 6f64 6964  ule_nameZ.pyodid
 00000710: 6543 6f64 65da 0862 6173 655f 7572 6ca9  eCode..base_url.
-00000720: 0072 2500 0000 fa63 2f77 6f72 6b73 7061  .r%....c/workspa
+00000720: 0072 2500 0000 fa6a 2f77 6f72 6b73 7061  .r%....j/workspa
 00000730: 6365 732f 636f 6e74 7269 6266 6c65 742f  ces/contribflet/
-00000740: 666c 6574 2f73 646b 2f70 7974 686f 6e2f  flet/sdk/python/
-00000750: 7061 636b 6167 6573 2f66 6c65 742d 7275  packages/flet-ru
-00000760: 6e74 696d 652f 7372 632f 666c 6574 5f72  ntime/src/flet_r
-00000770: 756e 7469 6d65 2f75 7469 6c73 2f70 6174  untime/utils/pat
-00000780: 6368 5f69 6e64 6578 2e70 79da 1070 6174  ch_index.py..pat
-00000790: 6368 5f69 6e64 6578 5f68 746d 6c09 0000  ch_index_html...
-000007a0: 0073 6e00 0000 000d 0c01 2602 0801 0a01  .sn.......&.....
-000007b0: 0202 0afe 0403 02fd 0807 0c01 1401 0401  ................
-000007c0: 0201 0cfe 0404 0401 0201 12fe 0404 0c02  ................
-000007d0: 0401 0e01 0401 0201 0401 14ff 02fe 0406  ................
-000007e0: 0601 0401 0201 0401 02ff 0203 02fb 0407  ................
-000007f0: 0601 0401 0201 0801 02fd 0405 0401 0201  ................
-00000800: 0801 02fd 0405 0601 0401 0201 0801 02fd  ................
-00000810: 0406 0c01 7227 0000 0029 04da 0d6d 616e  ....r'...)...man
-00000820: 6966 6573 745f 7061 7468 720a 0000 00da  ifest_pathr.....
-00000830: 0e61 7070 5f73 686f 7274 5f6e 616d 6572  .app_short_namer
-00000840: 0b00 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00000850: 0006 0000 0008 0000 0043 0000 0073 a600  .........C...s..
-00000860: 0000 7400 7c00 6401 8302 8f1e 7d04 7401  ..t.|.d.....}.t.
-00000870: a002 7c04 a003 a100 a101 7d05 5700 6400  ..|.......}.W.d.
-00000880: 0400 0400 8303 0100 6e10 3100 732e 3000  ........n.1.s.0.
-00000890: 0100 0100 0100 5900 0100 7c01 724c 7c01  ......Y...|.rL|.
-000008a0: 7c05 6402 3c00 7c01 7c05 6403 3c00 7c02  |.d.<.|.|.d.<.|.
-000008b0: 7258 7c02 7c05 6403 3c00 7c03 7264 7c03  rX|.|.d.<.|.rd|.
-000008c0: 7c05 6404 3c00 7400 7c00 6405 8302 8f24  |.d.<.t.|.d....$
-000008d0: 7d04 7c04 a004 7401 6a05 7c05 6406 6407  }.|...t.j.|.d.d.
-000008e0: 8d02 a101 0100 5700 6400 0400 0400 8303  ......W.d.......
-000008f0: 0100 6e10 3100 7398 3000 0100 0100 0100  ..n.1.s.0.......
-00000900: 5900 0100 6400 5300 2908 4e72 1200 0000  Y...d.S.).Nr....
-00000910: da04 6e61 6d65 5a0a 7368 6f72 745f 6e61  ..nameZ.short_na
-00000920: 6d65 da0b 6465 7363 7269 7074 696f 6e72  me..descriptionr
-00000930: 1400 0000 e902 0000 0029 01da 0669 6e64  .........)...ind
-00000940: 656e 7429 0672 1500 0000 da04 6a73 6f6e  ent).r......json
-00000950: da05 6c6f 6164 7372 1600 0000 7220 0000  ..loadsr....r ..
-00000960: 00da 0564 756d 7073 2906 7228 0000 0072  ...dumps).r(...r
-00000970: 0a00 0000 7229 0000 0072 0b00 0000 7221  ....r)...r....r!
-00000980: 0000 005a 086d 616e 6966 6573 7472 2500  ...Z.manifestr%.
-00000990: 0000 7225 0000 0072 2600 0000 da13 7061  ..r%...r&.....pa
-000009a0: 7463 685f 6d61 6e69 6665 7374 5f6a 736f  tch_manifest_jso
-000009b0: 6e54 0000 0073 1600 0000 0006 0c01 2c02  nT...s........,.
-000009c0: 0401 0801 0802 0401 0802 0401 0802 0c01  ................
-000009d0: 7231 0000 0029 034e 4e4e 290d 722e 0000  r1...).NNN).r...
-000009e0: 0072 1e00 0000 da07 7061 7468 6c69 6272  .r......pathlibr
-000009f0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-00000a00: 00da 0f66 6c65 745f 636f 7265 2e74 7970  ...flet_core.typ
-00000a10: 6573 7204 0000 00da 0441 5554 4f72 1800  esr......AUTOr..
-00000a20: 0000 da04 626f 6f6c 7227 0000 0072 3100  ....boolr'...r1.
-00000a30: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
-00000a40: 0072 2600 0000 da08 3c6d 6f64 756c 653e  .r&.....<module>
-00000a50: 0100 0000 7346 0000 0008 0108 010c 010c  ....sF..........
-00000a60: 020c 0602 0102 0102 0102 0102 0102 0104  ................
-00000a70: 0102 0102 f502 0102 0102 0106 0106 0106  ................
-00000a80: 0102 0102 0102 0102 0102 0102 f50c 4d00  ..............M.
-00000a90: 0100 0100 fc02 0102 0106 0106 0106 fc    ...............
+00000740: 666c 6574 636f 6e74 7269 622f 7364 6b2f  fletcontrib/sdk/
+00000750: 7079 7468 6f6e 2f70 6163 6b61 6765 732f  python/packages/
+00000760: 666c 6574 2d72 756e 7469 6d65 2f73 7263  flet-runtime/src
+00000770: 2f66 6c65 745f 7275 6e74 696d 652f 7574  /flet_runtime/ut
+00000780: 696c 732f 7061 7463 685f 696e 6465 782e  ils/patch_index.
+00000790: 7079 da10 7061 7463 685f 696e 6465 785f  py..patch_index_
+000007a0: 6874 6d6c 0900 0000 736e 0000 0000 0d0c  html....sn......
+000007b0: 0126 0208 010a 0102 020a fe04 0302 fd08  .&..............
+000007c0: 070c 0114 0104 0102 010c fe04 0404 0102  ................
+000007d0: 0112 fe04 040c 0204 010e 0104 0102 0104  ................
+000007e0: 0114 ff02 fe04 0606 0104 0102 0104 0102  ................
+000007f0: ff02 0302 fb04 0706 0104 0102 0108 0102  ................
+00000800: fd04 0504 0102 0108 0102 fd04 0506 0104  ................
+00000810: 0102 0108 0102 fd04 060c 0172 2700 0000  ...........r'...
+00000820: 2904 da0d 6d61 6e69 6665 7374 5f70 6174  )...manifest_pat
+00000830: 6872 0a00 0000 da0e 6170 705f 7368 6f72  hr......app_shor
+00000840: 745f 6e61 6d65 720b 0000 0063 0400 0000  t_namer....c....
+00000850: 0000 0000 0000 0000 0600 0000 0800 0000  ................
+00000860: 4300 0000 73a6 0000 0074 007c 0064 0183  C...s....t.|.d..
+00000870: 028f 1e7d 0474 01a0 027c 04a0 03a1 00a1  ...}.t...|......
+00000880: 017d 0557 0064 0004 0004 0083 0301 006e  .}.W.d.........n
+00000890: 1031 0073 2e30 0001 0001 0001 0059 0001  .1.s.0.......Y..
+000008a0: 007c 0172 4c7c 017c 0564 023c 007c 017c  .|.rL|.|.d.<.|.|
+000008b0: 0564 033c 007c 0272 587c 027c 0564 033c  .d.<.|.rX|.|.d.<
+000008c0: 007c 0372 647c 037c 0564 043c 0074 007c  .|.rd|.|.d.<.t.|
+000008d0: 0064 0583 028f 247d 047c 04a0 0474 016a  .d....$}.|...t.j
+000008e0: 057c 0564 0664 078d 02a1 0101 0057 0064  .|.d.d.......W.d
+000008f0: 0004 0004 0083 0301 006e 1031 0073 9830  .........n.1.s.0
+00000900: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00000910: 084e 7212 0000 00da 046e 616d 655a 0a73  .Nr......nameZ.s
+00000920: 686f 7274 5f6e 616d 65da 0b64 6573 6372  hort_name..descr
+00000930: 6970 7469 6f6e 7214 0000 00e9 0200 0000  iptionr.........
+00000940: 2901 da06 696e 6465 6e74 2906 7215 0000  )...indent).r...
+00000950: 00da 046a 736f 6eda 056c 6f61 6473 7216  ...json..loadsr.
+00000960: 0000 0072 2000 0000 da05 6475 6d70 7329  ...r .....dumps)
+00000970: 0672 2800 0000 720a 0000 0072 2900 0000  .r(...r....r)...
+00000980: 720b 0000 0072 2100 0000 5a08 6d61 6e69  r....r!...Z.mani
+00000990: 6665 7374 7225 0000 0072 2500 0000 7226  festr%...r%...r&
+000009a0: 0000 00da 1370 6174 6368 5f6d 616e 6966  .....patch_manif
+000009b0: 6573 745f 6a73 6f6e 5400 0000 7316 0000  est_jsonT...s...
+000009c0: 0000 060c 012c 0204 0108 0108 0204 0108  .....,..........
+000009d0: 0204 0108 020c 0172 3100 0000 2903 4e4e  .......r1...).NN
+000009e0: 4e29 0d72 2e00 0000 721e 0000 00da 0770  N).r....r......p
+000009f0: 6174 686c 6962 7202 0000 00da 0674 7970  athlibr......typ
+00000a00: 696e 6772 0300 0000 da0f 666c 6574 5f63  ingr......flet_c
+00000a10: 6f72 652e 7479 7065 7372 0400 0000 da04  ore.typesr......
+00000a20: 4155 544f 7218 0000 00da 0462 6f6f 6c72  AUTOr......boolr
+00000a30: 2700 0000 7231 0000 0072 2500 0000 7225  '...r1...r%...r%
+00000a40: 0000 0072 2500 0000 7226 0000 00da 083c  ...r%...r&.....<
+00000a50: 6d6f 6475 6c65 3e01 0000 0073 4600 0000  module>....sF...
+00000a60: 0801 0801 0c01 0c02 0c06 0201 0201 0201  ................
+00000a70: 0201 0201 0201 0401 0201 02f5 0201 0201  ................
+00000a80: 0201 0601 0601 0601 0201 0201 0201 0201  ................
+00000a90: 0201 02f5 0c4d 0001 0001 00fc 0201 0201  .....M..........
+00000aa0: 0601 0601 06fc                           ......
```

### Comparing `flet_contrib_runtime-2024.4.28.2241/src/flet_runtime/utils/patch_index.py` & `flet_contrib_runtime-2024.5.2.1633/src/flet_runtime/utils/patch_index.py`

 * *Files identical despite different names*

