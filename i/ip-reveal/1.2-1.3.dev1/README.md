# Comparing `tmp/ip-reveal-1.2.tar.gz` & `tmp/ip_reveal-1.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip-reveal-1.2.tar", max compression
+gzip compressed data, was "ip_reveal-1.3.dev1.tar", max compression
```

## Comparing `ip-reveal-1.2.tar` & `ip_reveal-1.3.dev1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0      184 2021-08-17 01:02:00.380663 ip-reveal-1.2/ip_reveal/.idea/.gitignore
--rw-r--r--   0        0        0      179 2021-08-17 01:02:00.381678 ip-reveal-1.2/ip_reveal/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      613 2021-08-17 01:02:00.382676 ip-reveal-1.2/ip_reveal/.idea/ip_reveal.iml
--rw-r--r--   0        0        0      200 2021-08-17 01:02:00.383672 ip-reveal-1.2/ip_reveal/.idea/misc.xml
--rw-r--r--   0        0        0      277 2021-08-17 01:02:00.383672 ip-reveal-1.2/ip_reveal/.idea/modules.xml
--rw-r--r--   0        0        0      191 2021-08-17 01:02:00.384672 ip-reveal-1.2/ip_reveal/.idea/vcs.xml
--rw-r--r--   0        0        0    17118 2021-10-21 21:21:24.154779 ip-reveal-1.2/ip_reveal/__init__.py
--rw-r--r--   0        0        0        0 2021-08-17 01:02:00.388677 ip-reveal-1.2/ip_reveal/assets/__init__.py
--rw-r--r--   0        0        0     1291 2021-10-21 21:21:24.170784 ip-reveal-1.2/ip_reveal/assets/sounds/__init__.py
--rw-r--r--   0        0        0      298 2021-10-21 21:21:24.172783 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/__init__.py
--rw-r--r--   0        0        0   130054 2021-10-21 21:20:39.970848 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/blip_pulse.wav
--rw-r--r--   0        0        0   437762 2021-10-21 21:20:39.983756 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/low_pulse.wav
--rw-r--r--   0        0        0    25817 2021-08-17 01:02:00.391688 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/o-pulse-alert.mp3
--rw-r--r--   0        0        0   285788 2021-08-17 01:02:00.394682 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/o-pulse-alert.wav
--rw-r--r--   0        0        0   285788 2021-10-21 21:20:39.991758 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/o-pulse.wav
--rw-r--r--   0        0        0   748424 2021-10-21 21:20:40.014588 ip-reveal-1.2/ip_reveal/assets/sounds/alerts/scifi_pulse.wav
--rw-r--r--   0        0        0        0 2021-10-21 21:20:39.504814 ip-reveal-1.2/ip_reveal/assets/ui_elements/__init__.py
--rw-r--r--   0        0        0      114 2021-08-17 01:02:00.396686 ip-reveal-1.2/ip_reveal/assets/ui_elements/backgrounds/__init__.py
--rw-r--r--   0        0        0  1691683 2021-08-17 01:02:00.412232 ip-reveal-1.2/ip_reveal/assets/ui_elements/backgrounds/neon_dark.png
--rw-r--r--   0        0        0      890 2021-08-17 01:02:00.413227 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/2897337-48.png
--rw-r--r--   0        0        0    13768 2021-10-21 21:20:39.506815 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/__init__.py
--rw-r--r--   0        0        0     2887 2021-08-17 01:02:00.415227 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/alerts/__init__.py
--rw-r--r--   0        0        0     1912 2021-08-17 01:02:00.416226 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/alerts/icons8-warning-shield-40.png
--rw-r--r--   0        0        0     6425 2021-10-21 21:21:24.191780 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_apply_en_unsel_48x48.png
--rw-r--r--   0        0        0     1978 2021-08-17 01:02:00.416226 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main-48.png
--rw-r--r--   0        0        0     1150 2021-08-17 01:02:00.417228 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main_16x16.ico
--rw-r--r--   0        0        0     2462 2021-08-17 01:02:00.418229 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main_24x24.ico
--rw-r--r--   0        0        0     4286 2021-08-17 01:02:00.419228 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main_32x32.ico
--rw-r--r--   0        0        0    10462 2021-08-17 01:02:00.419228 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_quit_50x50.ico
--rw-r--r--   0        0        0    35022 2021-08-17 01:02:00.420247 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_quit_92x92.ico
--rw-r--r--   0        0        0    10462 2021-08-17 01:02:00.421263 ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_refresh_50x50.ico
--rw-r--r--   0        0        0      466 2021-08-17 01:02:00.422262 ip-reveal-1.2/ip_reveal/assets/ui_elements/themes/__init__.py
--rw-r--r--   0        0        0     1505 2021-10-21 21:21:24.207778 ip-reveal-1.2/ip_reveal/config/__init__.py
--rw-r--r--   0        0        0     2245 2021-10-21 21:20:40.017589 ip-reveal-1.2/ip_reveal/config/arguments/__init__.py
--rw-r--r--   0        0        0     1096 2021-10-21 21:20:40.018581 ip-reveal-1.2/ip_reveal/config/errors.py
--rw-r--r--   0        0        0      241 2021-10-21 21:20:40.021581 ip-reveal-1.2/ip_reveal/gui/__init__.py
--rw-r--r--   0        0        0     1024 2021-10-21 21:21:24.225778 ip-reveal-1.2/ip_reveal/gui/windows/.test.py.swp
--rw-r--r--   0        0        0        0 2021-10-21 21:21:24.225778 ip-reveal-1.2/ip_reveal/gui/windows/__init__.py
--rw-r--r--   0        0        0      129 2021-10-21 21:21:24.227783 ip-reveal-1.2/ip_reveal/gui/windows/backgrounds/__init__.py
--rw-r--r--   0        0        0     1990 2021-10-21 21:21:24.245780 ip-reveal-1.2/ip_reveal/gui/windows/preferences.py
--rw-r--r--   0        0        0     1268 2021-10-21 21:21:24.262780 ip-reveal-1.2/ip_reveal/popups/__init__.py
--rw-r--r--   0        0        0     1494 2021-08-17 01:02:00.427263 ip-reveal-1.2/ip_reveal/popups/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0     2396 2021-08-17 01:02:00.428264 ip-reveal-1.2/ip_reveal/timers/__init__.py
--rw-r--r--   0        0        0     2361 2021-08-17 01:02:00.429264 ip-reveal-1.2/ip_reveal/timers/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      373 2021-08-17 01:02:00.000000 ip-reveal-1.2/ip_reveal/tools/__init__.py
--rw-r--r--   0        0        0      546 2021-08-17 01:02:00.431546 ip-reveal-1.2/ip_reveal/tools/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0     1176 2021-10-21 21:20:40.023580 ip-reveal-1.2/ip_reveal/tools/arguments/__init__.py
--rw-r--r--   0        0        0        0 2021-10-21 21:20:40.023580 ip-reveal-1.2/ip_reveal/tools/logging/__init__.py
--rw-r--r--   0        0        0      713 2021-10-21 21:20:40.025580 ip-reveal-1.2/ip_reveal/tools/network/__init__.py
--rw-r--r--   0        0        0      324 2021-10-21 21:20:40.027580 ip-reveal-1.2/ip_reveal/version/__init__.py
--rw-r--r--   0        0        0      506 2021-10-21 21:20:40.026580 ip-reveal-1.2/ip_reveal/version/VERSION
--rw-r--r--   0        0        0      786 2021-10-21 21:21:24.298779 ip-reveal-1.2/pyproject.toml
--rw-r--r--   0        0        0     1662 2021-10-22 02:34:58.403914 ip-reveal-1.2/setup.py
--rw-r--r--   0        0        0      883 2021-10-22 02:34:58.403914 ip-reveal-1.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2023-12-07 01:44:58.603575 ip_reveal-1.3.dev1/ip_reveal/.idea/.gitignore
+-rw-r--r--   0        0        0      174 2023-12-07 01:44:58.604571 ip_reveal-1.3.dev1/ip_reveal/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      599 2023-12-07 01:44:58.604571 ip_reveal-1.3.dev1/ip_reveal/.idea/ip_reveal.iml
+-rw-r--r--   0        0        0      197 2023-12-07 01:44:58.605566 ip_reveal-1.3.dev1/ip_reveal/.idea/misc.xml
+-rw-r--r--   0        0        0      270 2023-12-07 01:44:58.605566 ip_reveal-1.3.dev1/ip_reveal/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2023-12-07 01:44:58.606565 ip_reveal-1.3.dev1/ip_reveal/.idea/vcs.xml
+-rw-r--r--   0        0        0      353 2023-12-07 05:46:24.192214 ip_reveal-1.3.dev1/ip_reveal/__about__.py
+-rw-r--r--   0        0        0    17379 2023-12-07 01:44:58.607559 ip_reveal-1.3.dev1/ip_reveal/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:44:58.609552 ip_reveal-1.3.dev1/ip_reveal/assets/__init__.py
+-rw-r--r--   0        0        0     1242 2023-12-07 01:44:58.609552 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/__init__.py
+-rw-r--r--   0        0        0      287 2023-12-07 01:44:58.609552 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/__init__.py
+-rw-r--r--   0        0        0   130054 2023-12-07 01:44:58.611547 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/blip_pulse.wav
+-rw-r--r--   0        0        0   437762 2023-12-07 01:44:58.615602 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/low_pulse.wav
+-rw-r--r--   0        0        0    25817 2023-12-07 01:44:58.616719 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/o-pulse-alert.mp3
+-rw-r--r--   0        0        0   285788 2023-12-07 01:44:58.618794 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/o-pulse-alert.wav
+-rw-r--r--   0        0        0   285788 2023-12-07 01:44:58.620925 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/o-pulse.wav
+-rw-r--r--   0        0        0   748424 2023-12-07 01:44:58.625203 ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/scifi_pulse.wav
+-rw-r--r--   0        0        0        0 2023-12-07 01:44:58.626376 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-07 01:44:58.627463 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/backgrounds/__init__.py
+-rw-r--r--   0        0        0  1691683 2023-12-07 01:44:58.638609 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/backgrounds/neon_dark.png
+-rw-r--r--   0        0        0      890 2023-12-07 01:44:58.639607 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/2897337-48.png
+-rw-r--r--   0        0        0    13750 2023-12-07 01:44:58.640602 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/__init__.py
+-rw-r--r--   0        0        0     2875 2023-12-07 01:44:58.640602 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/alerts/__init__.py
+-rw-r--r--   0        0        0     1912 2023-12-07 01:44:58.641599 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/alerts/icons8-warning-shield-40.png
+-rw-r--r--   0        0        0     6425 2023-12-07 01:44:58.641599 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_apply_en_unsel_48x48.png
+-rw-r--r--   0        0        0     1978 2023-12-07 01:44:58.641599 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main-48.png
+-rw-r--r--   0        0        0     1150 2023-12-07 01:44:58.641599 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main_16x16.ico
+-rw-r--r--   0        0        0     2462 2023-12-07 01:44:58.642595 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main_24x24.ico
+-rw-r--r--   0        0        0     4286 2023-12-07 01:44:58.642595 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main_32x32.ico
+-rw-r--r--   0        0        0    10462 2023-12-07 01:44:58.642595 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_quit_50x50.ico
+-rw-r--r--   0        0        0    35022 2023-12-07 01:44:58.643592 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_quit_92x92.ico
+-rw-r--r--   0        0        0    10462 2023-12-07 01:44:58.644590 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_refresh_50x50.ico
+-rw-r--r--   0        0        0      442 2023-12-07 01:44:58.644590 ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/themes/__init__.py
+-rw-r--r--   0        0        0     1452 2023-12-07 01:44:58.644590 ip_reveal-1.3.dev1/ip_reveal/config/__init__.py
+-rw-r--r--   0        0        0     3941 2023-12-07 05:49:55.055647 ip_reveal-1.3.dev1/ip_reveal/config/arguments/__init__.py
+-rw-r--r--   0        0        0      311 2023-12-07 05:49:57.966273 ip_reveal-1.3.dev1/ip_reveal/config/arguments/app.log
+-rw-r--r--   0        0        0      997 2023-12-07 01:44:58.645982 ip_reveal-1.3.dev1/ip_reveal/config/errors.py
+-rw-r--r--   0        0        0      231 2023-12-07 01:44:58.645982 ip_reveal-1.3.dev1/ip_reveal/gui/__init__.py
+-rw-r--r--   0        0        0     1024 2023-12-07 01:44:58.646986 ip_reveal-1.3.dev1/ip_reveal/gui/windows/.test.py.swp
+-rw-r--r--   0        0        0        0 2023-12-07 01:44:58.646986 ip_reveal-1.3.dev1/ip_reveal/gui/windows/__init__.py
+-rw-r--r--   0        0        0      123 2023-12-07 01:44:58.647998 ip_reveal-1.3.dev1/ip_reveal/gui/windows/backgrounds/__init__.py
+-rw-r--r--   0        0        0     1775 2023-12-07 01:44:58.647998 ip_reveal-1.3.dev1/ip_reveal/gui/windows/preferences.py
+-rw-r--r--   0        0        0     1207 2023-12-07 01:44:58.649121 ip_reveal-1.3.dev1/ip_reveal/popups/__init__.py
+-rw-r--r--   0        0        0     1494 2023-12-07 01:44:58.650148 ip_reveal-1.3.dev1/ip_reveal/popups/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     4017 2023-12-07 05:14:14.433738 ip_reveal-1.3.dev1/ip_reveal/timers/__init__.py
+-rw-r--r--   0        0        0     2361 2023-12-07 01:44:58.652264 ip_reveal-1.3.dev1/ip_reveal/timers/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      356 2023-12-07 01:44:58.652264 ip_reveal-1.3.dev1/ip_reveal/tools/__init__.py
+-rw-r--r--   0        0        0      546 2023-12-07 01:44:58.653351 ip_reveal-1.3.dev1/ip_reveal/tools/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     1052 2023-12-07 01:44:58.654504 ip_reveal-1.3.dev1/ip_reveal/tools/arguments/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:44:58.654504 ip_reveal-1.3.dev1/ip_reveal/tools/logging/__init__.py
+-rw-r--r--   0        0        0      683 2023-12-07 01:44:58.654504 ip_reveal-1.3.dev1/ip_reveal/tools/network/__init__.py
+-rw-r--r--   0        0        0      307 2023-12-07 01:44:58.655543 ip_reveal-1.3.dev1/ip_reveal/version/__init__.py
+-rw-r--r--   0        0        0      951 2023-12-07 05:24:09.616956 ip_reveal-1.3.dev1/ip_reveal/version/VERSION
+-rw-r--r--   0        0        0      770 2024-01-06 19:07:47.433784 ip_reveal-1.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 ip_reveal-1.3.dev1/PKG-INFO
```

### Comparing `ip-reveal-1.2/ip_reveal/.idea/ip_reveal.iml` & `ip_reveal-1.3.dev1/ip_reveal/.idea/ip_reveal.iml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c6d 6f64 756c 6520  F-8"?>..<module 
-00000030: 7479 7065 3d22 5059 5448 4f4e 5f4d 4f44  type="PYTHON_MOD
-00000040: 554c 4522 2076 6572 7369 6f6e 3d22 3422  ULE" version="4"
-00000050: 3e0d 0a20 203c 636f 6d70 6f6e 656e 7420  >..  <component 
-00000060: 6e61 6d65 3d22 4e65 774d 6f64 756c 6552  name="NewModuleR
-00000070: 6f6f 744d 616e 6167 6572 223e 0d0a 2020  ootManager">..  
-00000080: 2020 3c63 6f6e 7465 6e74 2075 726c 3d22    <content url="
-00000090: 6669 6c65 3a2f 2f24 4d4f 4455 4c45 5f44  file://$MODULE_D
-000000a0: 4952 2422 202f 3e0d 0a20 2020 203c 6f72  IR$" />..    <or
-000000b0: 6465 7245 6e74 7279 2074 7970 653d 226a  derEntry type="j
-000000c0: 646b 2220 6a64 6b4e 616d 653d 2250 7974  dk" jdkName="Pyt
-000000d0: 686f 6e20 332e 3620 2869 702d 7265 7665  hon 3.6 (ip-reve
-000000e0: 616c 2922 206a 646b 5479 7065 3d22 5079  al)" jdkType="Py
-000000f0: 7468 6f6e 2053 444b 2220 2f3e 0d0a 2020  thon SDK" />..  
-00000100: 2020 3c6f 7264 6572 456e 7472 7920 7479    <orderEntry ty
-00000110: 7065 3d22 736f 7572 6365 466f 6c64 6572  pe="sourceFolder
-00000120: 2220 666f 7254 6573 7473 3d22 6661 6c73  " forTests="fals
-00000130: 6522 202f 3e0d 0a20 203c 2f63 6f6d 706f  e" />..  </compo
-00000140: 6e65 6e74 3e0d 0a20 203c 636f 6d70 6f6e  nent>..  <compon
-00000150: 656e 7420 6e61 6d65 3d22 5079 446f 6375  ent name="PyDocu
-00000160: 6d65 6e74 6174 696f 6e53 6574 7469 6e67  mentationSetting
-00000170: 7322 3e0d 0a20 2020 203c 6f70 7469 6f6e  s">..    <option
-00000180: 206e 616d 653d 2266 6f72 6d61 7422 2076   name="format" v
-00000190: 616c 7565 3d22 474f 4f47 4c45 2220 2f3e  alue="GOOGLE" />
-000001a0: 0d0a 2020 2020 3c6f 7074 696f 6e20 6e61  ..    <option na
-000001b0: 6d65 3d22 6d79 446f 6353 7472 696e 6746  me="myDocStringF
-000001c0: 6f72 6d61 7422 2076 616c 7565 3d22 476f  ormat" value="Go
-000001d0: 6f67 6c65 2220 2f3e 0d0a 2020 3c2f 636f  ogle" />..  </co
-000001e0: 6d70 6f6e 656e 743e 0d0a 2020 3c63 6f6d  mponent>..  <com
-000001f0: 706f 6e65 6e74 206e 616d 653d 2254 6573  ponent name="Tes
-00000200: 7452 756e 6e65 7253 6572 7669 6365 223e  tRunnerService">
-00000210: 0d0a 2020 2020 3c6f 7074 696f 6e20 6e61  ..    <option na
-00000220: 6d65 3d22 5052 4f4a 4543 545f 5445 5354  me="PROJECT_TEST
-00000230: 5f52 554e 4e45 5222 2076 616c 7565 3d22  _RUNNER" value="
-00000240: 7079 7465 7374 2220 2f3e 0d0a 2020 3c2f  pytest" />..  </
-00000250: 636f 6d70 6f6e 656e 743e 0d0a 3c2f 6d6f  component>..</mo
-00000260: 6475 6c65 3e                             dule>
+00000020: 462d 3822 3f3e 0a3c 6d6f 6475 6c65 2074  F-8"?>.<module t
+00000030: 7970 653d 2250 5954 484f 4e5f 4d4f 4455  ype="PYTHON_MODU
+00000040: 4c45 2220 7665 7273 696f 6e3d 2234 223e  LE" version="4">
+00000050: 0a20 203c 636f 6d70 6f6e 656e 7420 6e61  .  <component na
+00000060: 6d65 3d22 4e65 774d 6f64 756c 6552 6f6f  me="NewModuleRoo
+00000070: 744d 616e 6167 6572 223e 0a20 2020 203c  tManager">.    <
+00000080: 636f 6e74 656e 7420 7572 6c3d 2266 696c  content url="fil
+00000090: 653a 2f2f 244d 4f44 554c 455f 4449 5224  e://$MODULE_DIR$
+000000a0: 2220 2f3e 0a20 2020 203c 6f72 6465 7245  " />.    <orderE
+000000b0: 6e74 7279 2074 7970 653d 226a 646b 2220  ntry type="jdk" 
+000000c0: 6a64 6b4e 616d 653d 2250 7974 686f 6e20  jdkName="Python 
+000000d0: 332e 3620 2869 702d 7265 7665 616c 2922  3.6 (ip-reveal)"
+000000e0: 206a 646b 5479 7065 3d22 5079 7468 6f6e   jdkType="Python
+000000f0: 2053 444b 2220 2f3e 0a20 2020 203c 6f72   SDK" />.    <or
+00000100: 6465 7245 6e74 7279 2074 7970 653d 2273  derEntry type="s
+00000110: 6f75 7263 6546 6f6c 6465 7222 2066 6f72  ourceFolder" for
+00000120: 5465 7374 733d 2266 616c 7365 2220 2f3e  Tests="false" />
+00000130: 0a20 203c 2f63 6f6d 706f 6e65 6e74 3e0a  .  </component>.
+00000140: 2020 3c63 6f6d 706f 6e65 6e74 206e 616d    <component nam
+00000150: 653d 2250 7944 6f63 756d 656e 7461 7469  e="PyDocumentati
+00000160: 6f6e 5365 7474 696e 6773 223e 0a20 2020  onSettings">.   
+00000170: 203c 6f70 7469 6f6e 206e 616d 653d 2266   <option name="f
+00000180: 6f72 6d61 7422 2076 616c 7565 3d22 474f  ormat" value="GO
+00000190: 4f47 4c45 2220 2f3e 0a20 2020 203c 6f70  OGLE" />.    <op
+000001a0: 7469 6f6e 206e 616d 653d 226d 7944 6f63  tion name="myDoc
+000001b0: 5374 7269 6e67 466f 726d 6174 2220 7661  StringFormat" va
+000001c0: 6c75 653d 2247 6f6f 676c 6522 202f 3e0a  lue="Google" />.
+000001d0: 2020 3c2f 636f 6d70 6f6e 656e 743e 0a20    </component>. 
+000001e0: 203c 636f 6d70 6f6e 656e 7420 6e61 6d65   <component name
+000001f0: 3d22 5465 7374 5275 6e6e 6572 5365 7276  ="TestRunnerServ
+00000200: 6963 6522 3e0a 2020 2020 3c6f 7074 696f  ice">.    <optio
+00000210: 6e20 6e61 6d65 3d22 5052 4f4a 4543 545f  n name="PROJECT_
+00000220: 5445 5354 5f52 554e 4e45 5222 2076 616c  TEST_RUNNER" val
+00000230: 7565 3d22 7079 7465 7374 2220 2f3e 0a20  ue="pytest" />. 
+00000240: 203c 2f63 6f6d 706f 6e65 6e74 3e0a 3c2f   </component>.</
+00000250: 6d6f 6475 6c65 3e                        module>
```

### Comparing `ip-reveal-1.2/ip_reveal/__init__.py` & `ip_reveal-1.3.dev1/ip_reveal/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,510 +1,563 @@
-import socket
-import sys
-from argparse import ArgumentParser
-from platform import node
-from socket import gaierror
-from urllib.error import URLError
-
-try:
-    import PySimpleGUIQt as Qt
-except ImportError:
-    try:
-        shell = get_ipython().__class__.__name__
-        Qt = pyqt5
-    except:
-        raise
-
-
-from inspy_logger import LEVELS as LOG_LEVELS, getLogger
-from inspy_logger import InspyLogger
-from inspyred_print import Color, Format
-from requests import get
-from requests.exceptions import ConnectionError
-from urllib3.exceptions import MaxRetryError
-from threading import Thread
-
-from ip_reveal.assets.ui_elements.backgrounds import NEON_DARK_FP
-from ip_reveal.assets.ui_elements.icons import app_main_24x24
-from ip_reveal.assets.ui_elements.icons import app_quit_50x50_fp
-from ip_reveal.assets.ui_elements.icons import app_refresh_50x50_fp
-
-from ip_reveal import config
-
-#import ip_reveal.timers as timer
-import humanize
-from inspyre_toolbox.live_timer import Timer
-from ip_reveal.tools import commify
-
-quit_icon = app_quit_50x50_fp
-refresh_icon = app_refresh_50x50_fp
-
-end = Format().end_mod
-color = Color()
-red = color.red
-
-update_window_timer = None
-
-timer = Timer()
-timer.start()
-
-cached_ext_ip = None
-ip_hist = []
-
-inet_down = False
-log_device = None
-args = None
-config = config
-
-def get_hostname():
-    """
-    get_hostname
-
-    Fetch the system's apparent hostname and return it to the caller
-
-    Returns:
-        str: The system's apparent hostname contained within a string.
-    """
-
-    # Prepare the logger
-    _log = getLogger(log_name + '.get_hostname')
-    _debug = _log.debug
-
-    # Fetch the hostname from platform.node
-    hostname = node()
-    _debug(f'Checked hostname and found it is: {hostname}')
-
-    # Return this to the caller
-    return hostname
-
-
-def push_notification(old_ip, new_ip):
-    """
-    
-    Push a notification through the GUI with a sound.
-    
-    
-    Args:
-        old_ip (str):
-            The IP that was held previously.
-        
-        new_ip (str):
-            The new - currently held - IP address
-            
-
-    Returns:
-        None
-
-    """
-    from ip_reveal.popups import ip_change_notify
-
-    ip_change_notify(old_ip, new_ip)
-    
-
-def get_external():
-    """
-    get_external
-
-    Fetch the system's apparent hostname and return it to the caller in the form of a string.
-
-    Returns:
-        str: The system's apparent external IP-Address in the form of a string.
-    """
-    global cached_ext_ip, inet_down, ip_hist
-
-    # Prepare the logger
-    _log = getLogger(log_name + '.get_external')
-    _debug = _log.debug
-
-    # Try contacting IPIFY.org with a basic request and read the returned text.
-    #
-    # If we are unable to connect to this outside service, it's likely that Internet connection has dropped. There
-    # are - however, instances where this service is down, and for these reasons we want to have at least one
-    # alternative to control for failure on a Singular -free- AI API.
-
-    # Fetch the external IP-Address from IPIFY.org
-    try:
-        external = get('https://api.ipify.org').text
-        _debug(f'Checked external IP and found it is: {external}')
-
-    # Catch the "ConnectionError" exception that is raised when the "requests" package is unable to reach
-    # "IPIFY.org", simply reporting this occurred (if the logger is listening) before (maybe first; attempt connection
-    # to another service?)
-    except (ConnectionError, MaxRetryError, gaierror, URLError) as e:
-        if not inet_down:
-            _log.warning("Unable to establish an internet connection.")
-            inet_down = True
-        external = None
-
-    if external is not None:
-
-        if not cached_ext_ip:
-            cached_ext_ip = external
-            if not cached_ext_ip == external:
-                push_notification(cached_ext_ip, external)
-                cached_ext_ip = external
-
-    else:
-        return False
-
-    if len(ip_hist) == 0:
-        _debug("Added first IP to history list.")
-        ip_hist.append(external)
-        _debug(f"IP History: {ip_hist}")
-
-    # Return the text result we get from the API to the caller.
-    return external
-
-
-def get_internal():
-    """
-    get_internal
-
-    Fetch the system's local IP-Address and return it to the caller in the form of a string.
-
-    Returns:
-        str: The system's local IP-Address contained within a string.
-    """
-
-    # Set up a logger
-    _log = getLogger(log_name + '.get_internal')
-
-    # Alias the debug entry call
-    _debug = _log.debug
-
-    # Start a socket
-    s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-
-    # Attempt a connection to an arbitrary host
-    try:
-        # doesn't even have to be reachable
-        s.connect(('10.255.255.255', 1))
-
-        # Fetch our IP from this socket's metadata
-        IP = s.getsockname()[0]
-
-    # Should we raise an exception we won't bother handling it, we'll just return the loopback address to the caller.
-    except Exception:
-        IP = '127.0.0.1'
-
-    # No matter the result, let's remember to close the socket.
-    finally:
-        s.close()
-
-    # Announce that we've found an IP
-    _debug(f'Checked internal IP and found: {IP}')
-
-    # Return a string containing the result to the caller.
-    return IP
-
-
-def update_window(values=None):
-    global log_device, args
-    from ip_reveal.popups import ip_change_notify
-    """
-
-    A function that handles the following processes for updating the IP Reveal window:
-
-      * Updating all relevant fields
-      * Resetting accumulators
-      * Incrementing refresh stats (if opted in)
-      * Fetching the information for external and internal IP addresses
-      * Calls a refresh on the timer.
-
-    NOTE:
-        It is not advisable to utilize this function in a loop without limiting how often it's run. You could end up
-        DoSing yourself or others.
-
-    Returns:
-        None
-
-    """
-    global acc, refresh_num, timer, cached_ext_ip, ip_hist
-
-    # Start the logger for this operation
-    _log = getLogger(log_name + '.update_window')
-
-    # If set to do so; spit out some debug data
-    u_debug = _log.debug
-    u_debug('TIMEOUT - Refreshing window...')
-    u_debug(f'acc = {str(acc)}')
-
-    # Reset the frame accumulator
-    acc = 0
-
-    # Spit out some more useful info, if allowed.
-    u_debug(f'Reset acc accumulator new value: {str(acc)}')
-    u_debug(f'Incrementing refresh count...')
-
-    # For stats purposes only; increment our count of window refreshes.
-    refresh_num += 1
-
-    # Grab our fresh data for diplaying to the window
-    ip = get_external()
-
-    if not ip:
-        ip = "Offline"
-
-    local_ip = get_internal()
-    hostname = get_hostname()
-
-    # Call a 'refresh()' on our timer object. This will start another cycle to keep track of. This allows the timer
-    # routine to always track the time since last data fetching
-    timer.reset()
-
-    if ip == "Offline":
-        t_color = "red"
-    else:
-        t_color = "green"
-
-    # Update the relevant fields with our fresh data
-    window['EXTIP_OUT'].update(ip, text_color=t_color)
-    window['INTIP_OUT'].update(local_ip)
-    window['HOSTNAME_OUT'].update(hostname)
-    window['TIME_SINCE_Q_OUT'].update("Just now...")
-
-    # Make some notes in the debug log that might be useful
-    u_debug(f'Updated window with new values: {values}')
-    u_debug(f'This was refresh number {refresh_num}')
-
-    if not ip == cached_ext_ip:
-        ip_change_notify(cached_ext_ip, ip, args.mute_all)
-        cached_ext_ip = ip
-        ip_hist.append(ip)
-
-
-def safe_exit(win, exit_reason):
-    _log = getLogger(log_name + '.safe_exit')
-    
-    tmp_hist = []
-    for ip in ip_hist:
-        if ip not in tmp_hist:
-            tmp_hist.append(ip)
-
-    _log.info(f"During operation you switched IP addresses {len(ip_hist) - 1} times.")
-    _log.info(f"Held IP addresses: {tmp_hist}")
-    _log.info(f"Exiting safely. Reason: {exit_reason}")
-    _log.info(f"The IP address was refreshed {refresh_num} times")
-    _log.info(f"Window underwent {total_acc} cycles")
-    print(timer.start_time)
-
-    win.close()
-    sys.exit()
-
-
-# Set up a name for our logging device
-log_name = "IPReveal"
-
-# Declare a variable named 'acc' for our accumulator and set it at int(0)
-acc = 0
-
-# For statistics tracking; declare a variable called 'refresh_num' and start it at 0
-refresh_num = 0
-
-# ...and one that will hold our total cycle count
-total_acc = 0
-
-# Set up a placeholder variable for our window object
-window = None
-
-# Set up two variables that will act as caches for the external and internal IPs
-cached_ext_ip = None
-cached_int_ip = None
-
-acc2 = 0
-
-def main():
-    global total_acc, acc, refresh_num, window, log_device, args
-
-    # Timer text
-    t_text = "Just now..."
-
-    # Qt.theme('DarkBlue3')
-
-    parser = ArgumentParser(
-        'ip-reveal', description='A program that will show you your external IP address.')
-
-    parser.add_argument('-l', '--log-level',
-                        nargs='?',
-                        choices=LOG_LEVELS,
-                        default='info'
-                        )
-
-    # Argument to mute sounds
-    parser.add_argument('-m', '--mute-all',
-                        action='store_true',
-                        required=False,
-                        help="Starts the program with all program audio muted.",
-                        default=False
-                        )
-    
-    # Argument to implicitly set the refresh rate
-    parser.add_argument('-r', '--refresh-interval',
-                        type=int,
-                        default=30,
-                        help='Specify the number of seconds you want to have pass before IP-Reveal refreshes your IP '
-                             'information. (Defaults to 30)',
-                        action='store')
-
-    parser.add_argument('-V', '--version', action='version', version='1.2'
-                        )
-
-    sub_parsers = parser.add_subparsers(
-        dest='subcommands', help='The sub-commands for IP Reveal')
-
-    ext_ip_parse = sub_parsers.add_parser('get-external',
-                                          help='Return the external IP to the command-line and nothing else.')
-    host_parse = sub_parsers.add_parser(
-        'get-host', help='Return the hostname to the command-line and nothing else.')
-    local_parse = sub_parsers.add_parser('get-local',
-                                         help='Return the local IP-Address to the command-line and nothing '
-                                              'else.')
-    test_audio_parse = sub_parsers.add_parser('test-audio',
-                                              help="To ensure you get notifications you can test IP-Reveal's audio "
-                                                   "engine with this command.")
-    test_audio_parse.add_argument('-c', '--countdown',
-                                  action='store',
-                                  type=int,
-                                  default=3,
-                                  help="Enter the number to countdown from before starting the test.")
-    test_audio_parse.add_argument('-f', '--full',
-                                  help='Run the full range of audio tests provided by the audio engine',
-                                  action='store_true',
-                                  default=False)
-
-    args = parser.parse_args()
-    
-    config.args = args
-
-    # Set up the logging device
-    log_device = InspyLogger(log_name, args.log_level).device
-
-    # Start the logging device
-    log = log_device.start(mute=args.subcommands)
-    debug = log.debug
-
-    # Announce that we did that
-    debug('Started my logger!')
-    log = getLogger(log_name + '.Main')
-    # Alias the log.debug signature for ease-of-use
-    debug = log.debug
-
-    # See if we got one of the subcommands assigned.
-    if args.subcommands == 'get-external':
-        print(get_external())
-        exit()
-    elif args.subcommands == 'get-host':
-        print(get_hostname())
-        exit()
-    elif args.subcommands == 'get-local':
-        print(get_internal())
-        exit()
-    elif args.subcommands == 'test-audio':
-        from ip_reveal.assets.sounds import run_audio_test
-        run_audio_test(args.countdown, args.full, args.log_level)
-        exit()
-
-    status_bar_layout = [
-
-    ]
-
-    bg_color = "340245"
-    size = (220, 50)
-    alpha = 1
-    if alpha >= 1:
-        text_background_color = "pink"
-    else:
-        text_background_color = "white"
-
-    layout = [
-        [
-            Qt.Text('External IP:', background_color=text_background_color, text_color="black", relief=Qt.RELIEF_GROOVE,
-                    size_px=size, auto_size_text=True, justification='center'),
-            Qt.Text(get_external(), relief=Qt.RELIEF_SUNKEN, key='EXTIP_OUT', background_color=text_background_color,
-                    text_color="black", size_px=size, auto_size_text=True, justification='center'),
-        ],
-
-        [
-            Qt.Text('Internal IP:', background_color=text_background_color, text_color="black", relief=Qt.RELIEF_GROOVE,
-                    size_px=size, auto_size_text=True, justification='center'),
-            Qt.Text(get_internal(), key='INTIP_OUT', relief=Qt.RELIEF_SUNKEN, background_color=text_background_color,
-                    text_color="black", size_px=size, auto_size_text=True, justification='center')
-        ],
-        [
-            Qt.Text('Hostname:', background_color=text_background_color, text_color="black", relief=Qt.RELIEF_GROOVE,
-                    size_px=size, auto_size_text=True, justification='center'),
-            Qt.Text(get_hostname(), key='HOSTNAME_OUT', relief=Qt.RELIEF_SUNKEN, background_color=text_background_color,
-                    text_color="black", size_px=size, auto_size_text=True, justification='center')
-        ],
-        [
-            Qt.Text(f"Last checked", background_color=text_background_color, text_color="black",
-                    relief=Qt.RELIEF_GROOVE, size_px=size, auto_size_text=True, justification='center'),
-            Qt.Text(t_text, key="TIME_SINCE_Q_OUT", relief=Qt.RELIEF_SUNKEN, background_color=text_background_color,
-                    text_color="black", size_px=size, auto_size_text=True, justification='center')
-        ],
-        [
-            Qt.Button('', key='MAIN_CLOSE_BUTTON',
-                      image_filename=app_quit_50x50_fp,
-                      image_size=(50, 50),
-                      button_color=(None, "#ff0000"),
-                      tooltip="Quit IP Reveal"),
-            Qt.Button('', key='MAIN_REFRESH_BUTTON',
-                      image_filename=app_refresh_50x50_fp,
-                      image_size=(50, 50),
-                      button_color=(None, "#ff0000"),
-                      tooltip="Refresh")
-        ],
-    ]
-
-    # Assemble the above widget into a window.
-    window = Qt.Window('IP-Reveal by Inspyre Softworks', layout=layout,
-                       background_image=NEON_DARK_FP,
-                       icon=app_main_24x24,
-                       size=(300, 400),
-                       alpha_channel=alpha,
-                       grab_anywhere=True,
-                       background_color="white"
-                       )
-    
-
-    # Start our main GUI loop.
-    while True:
-        event, values = window.read(timeout=100)
-
-        # Set up a child logger that will log window events.
-        w_log = getLogger(log_name + '.MainWindow')
-        w_debug = w_log.debug
-
-        # Increment the cycle count
-        acc += 1
-        total_acc += 1
-
-        t = int(timer.get_elapsed(seconds=True))
-        t_text = humanize.naturaldelta(t)
-
-        window['TIME_SINCE_Q_OUT'].update(f"{t_text} ago...")
-
-        # If the accumulator is at 325 counts, alert the user, update the window, and reset the accumulator
-        if t == args.refresh_interval:
-            w_debug('Calling function to update the window...')
-
-            window['TIME_SINCE_Q_OUT'].update('Refreshing...')
-            update_win = Thread(target=update_window)
-
-            update_win.start()
-            w_debug('Updated window!')
-
-        # If the 'Close' button is pressed: we exit.
-        if event is None or event == 'MAIN_CLOSE_BUTTON':
-            e_reason = f"It seems the user closed the window, received {values}"
-            if event == 'MAIN_CLOSE_BUTTON':
-                e_reason = 'The close button was pressed'
-            safe_exit(window, exit_reason=e_reason)
-
-            w_log.info("User initiated closing")
-
-            break
-
-        if event == 'MAIN_REFRESH_BUTTON':
-            w_debug('Calling a refresh on the window')
-            update_window()
-            w_debug('All seems well!')
+import socket
+import sys
+from argparse import ArgumentParser
+from platform import node
+from socket import gaierror
+from urllib.error import URLError
+
+try:
+    import PySimpleGUIQt as Qt
+except ImportError:
+    try:
+        shell = get_ipython().__class__.__name__
+        Qt = pyqt5
+    except:
+        raise
+
+
+from inspy_logger import LEVELS as LOG_LEVELS, getLogger
+from inspy_logger import InspyLogger
+from inspyred_print import Color, Format
+from requests import get
+from requests.exceptions import ConnectionError
+from urllib3.exceptions import MaxRetryError
+from threading import Thread
+
+from ip_reveal.assets.ui_elements.backgrounds import NEON_DARK_FP
+from ip_reveal.assets.ui_elements.icons import app_main_24x24
+from ip_reveal.assets.ui_elements.icons import app_quit_50x50_fp
+from ip_reveal.assets.ui_elements.icons import app_refresh_50x50_fp
+
+from ip_reveal import config
+
+#import ip_reveal.timers as timer
+import humanize
+from inspyre_toolbox.live_timer import Timer
+from ip_reveal.tools import commify
+
+quit_icon = app_quit_50x50_fp
+refresh_icon = app_refresh_50x50_fp
+
+end = Format().end_mod
+color = Color()
+red = color.red
+
+update_window_timer = None
+
+timer = Timer()
+timer.start()
+
+cached_ext_ip = None
+ip_hist = []
+
+inet_down = False
+log_device = None
+args = None
+config = config
+
+def get_hostname():
+    """
+    get_hostname
+
+    Fetch the system's apparent hostname and return it to the caller
+
+    Returns:
+        str: The system's apparent hostname contained within a string.
+    """
+
+    # Prepare the logger
+    _log = getLogger(log_name + '.get_hostname')
+    _debug = _log.debug
+
+    # Fetch the hostname from platform.node
+    hostname = node()
+    _debug(f'Checked hostname and found it is: {hostname}')
+
+    # Return this to the caller
+    return hostname
+
+
+def push_notification(old_ip, new_ip):
+    """
+    
+    Push a notification through the GUI with a sound.
+    
+    
+    Args:
+        old_ip (str):
+            The IP that was held previously.
+        
+        new_ip (str):
+            The new - currently held - IP address
+            
+
+    Returns:
+        None
+
+    """
+    from ip_reveal.popups import ip_change_notify
+
+    ip_change_notify(old_ip, new_ip)
+    
+
+def get_external():
+    """
+    get_external
+
+    Fetch the system's apparent hostname and return it to the caller in the form of a string.
+
+    Returns:
+        str: The system's apparent external IP-Address in the form of a string.
+    """
+    global cached_ext_ip, inet_down, ip_hist
+
+    # Prepare the logger
+    _log = getLogger(log_name + '.get_external')
+    _debug = _log.debug
+
+    # Try contacting IPIFY.org with a basic request and read the returned text.
+    #
+    # If we are unable to connect to this outside service, it's likely that Internet connection has dropped. There
+    # are - however, instances where this service is down, and for these reasons we want to have at least one
+    # alternative to control for failure on a Singular -free- AI API.
+
+    # Fetch the external IP-Address from IPIFY.org
+    try:
+        external = get('https://api.ipify.org').text
+        _debug(f'Checked external IP and found it is: {external}')
+
+    # Catch the "ConnectionError" exception that is raised when the "requests" package is unable to reach
+    # "IPIFY.org", simply reporting this occurred (if the logger is listening) before (maybe first; attempt connection
+    # to another service?)
+    except (ConnectionError, MaxRetryError, gaierror, URLError) as e:
+        if not inet_down:
+            _log.warning("Unable to establish an internet connection.")
+            inet_down = True
+        external = None
+
+    if external is None:
+        return False
+
+    if not cached_ext_ip:
+        cached_ext_ip = external
+        if cached_ext_ip != external:
+            push_notification(cached_ext_ip, external)
+            cached_ext_ip = external
+
+    if len(ip_hist) == 0:
+        _debug("Added first IP to history list.")
+        ip_hist.append(external)
+        _debug(f"IP History: {ip_hist}")
+
+    # Return the text result we get from the API to the caller.
+    return external
+
+
+def get_internal():
+    """
+    get_internal
+
+    Fetch the system's local IP-Address and return it to the caller in the form of a string.
+
+    Returns:
+        str: The system's local IP-Address contained within a string.
+    """
+
+    # Set up a logger
+    _log = getLogger(log_name + '.get_internal')
+
+    # Alias the debug entry call
+    _debug = _log.debug
+
+    # Start a socket
+    s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+
+    # Attempt a connection to an arbitrary host
+    try:
+        # doesn't even have to be reachable
+        s.connect(('10.255.255.255', 1))
+
+        # Fetch our IP from this socket's metadata
+        IP = s.getsockname()[0]
+
+    # Should we raise an exception we won't bother handling it, we'll just return the loopback address to the caller.
+    except Exception:
+        IP = '127.0.0.1'
+
+    # No matter the result, let's remember to close the socket.
+    finally:
+        s.close()
+
+    # Announce that we've found an IP
+    _debug(f'Checked internal IP and found: {IP}')
+
+    # Return a string containing the result to the caller.
+    return IP
+
+
+def update_window(values=None):
+    global log_device, args
+    from ip_reveal.popups import ip_change_notify
+    """
+
+    A function that handles the following processes for updating the IP Reveal window:
+
+      * Updating all relevant fields
+      * Resetting accumulators
+      * Incrementing refresh stats (if opted in)
+      * Fetching the information for external and internal IP addresses
+      * Calls a refresh on the timer.
+
+    NOTE:
+        It is not advisable to utilize this function in a loop without limiting how often it's run. You could end up
+        DoSing yourself or others.
+
+    Returns:
+        None
+
+    """
+    global acc, refresh_num, timer, cached_ext_ip, ip_hist
+
+    # Start the logger for this operation
+    _log = getLogger(log_name + '.update_window')
+
+    # If set to do so; spit out some debug data
+    u_debug = _log.debug
+    u_debug('TIMEOUT - Refreshing window...')
+    u_debug(f'acc = {acc}')
+
+    # Spit out some more useful info, if allowed.
+    u_debug('Reset acc accumulator new value: 0')
+    u_debug('Incrementing refresh count...')
+
+    # For stats purposes only; increment our count of window refreshes.
+    refresh_num += 1
+
+    # Grab our fresh data for diplaying to the window
+    ip = get_external()
+
+    if not ip:
+        ip = "Offline"
+
+    local_ip = get_internal()
+    hostname = get_hostname()
+
+    # Call a 'refresh()' on our timer object. This will start another cycle to keep track of. This allows the timer
+    # routine to always track the time since last data fetching
+    timer.reset()
+
+    t_color = "red" if ip == "Offline" else "green"
+    # Update the relevant fields with our fresh data
+    window['EXTIP_OUT'].update(ip, text_color=t_color)
+    window['INTIP_OUT'].update(local_ip)
+    window['HOSTNAME_OUT'].update(hostname)
+    window['TIME_SINCE_Q_OUT'].update("Just now...")
+
+    # Make some notes in the debug log that might be useful
+    u_debug(f'Updated window with new values: {values}')
+    u_debug(f'This was refresh number {refresh_num}')
+
+    if ip != cached_ext_ip:
+        ip_change_notify(cached_ext_ip, ip, args.mute_all)
+        cached_ext_ip = ip
+        ip_hist.append(ip)
+
+
+def safe_exit(win, exit_reason):
+    _log = getLogger(log_name + '.safe_exit')
+    
+    tmp_hist = []
+    for ip in ip_hist:
+        if ip not in tmp_hist:
+            tmp_hist.append(ip)
+
+    _log.info(f"During operation you switched IP addresses {len(ip_hist) - 1} times.")
+    _log.info(f"Held IP addresses: {tmp_hist}")
+    _log.info(f"Exiting safely. Reason: {exit_reason}")
+    _log.info(f"The IP address was refreshed {refresh_num} times")
+    _log.info(f"Window underwent {total_acc} cycles")
+    print(timer.start_time)
+
+    win.close()
+    sys.exit()
+
+
+# Set up a name for our logging device
+log_name = "IPReveal"
+
+# Declare a variable named 'acc' for our accumulator and set it at int(0)
+acc = 0
+
+# For statistics tracking; declare a variable called 'refresh_num' and start it at 0
+refresh_num = 0
+
+# ...and one that will hold our total cycle count
+total_acc = 0
+
+# Set up a placeholder variable for our window object
+window = None
+
+# Set up two variables that will act as caches for the external and internal IPs
+cached_ext_ip = None
+cached_int_ip = None
+
+acc2 = 0
+
+def main():
+    global total_acc, acc, refresh_num, window, log_device, args
+
+    # Timer text
+    t_text = "Just now..."
+
+    # Qt.theme('DarkBlue3')
+
+    parser = ArgumentParser(
+        'ip-reveal', description='A program that will show you your external IP address.')
+
+    parser.add_argument('-l', '--log-level',
+                        nargs='?',
+                        choices=LOG_LEVELS,
+                        default='info'
+                        )
+
+    # Argument to mute sounds
+    parser.add_argument('-m', '--mute-all',
+                        action='store_true',
+                        required=False,
+                        help="Starts the program with all program audio muted.",
+                        default=False
+                        )
+
+    # Argument to implicitly set the refresh rate
+    parser.add_argument('-r', '--refresh-interval',
+                        type=int,
+                        default=30,
+                        help='Specify the number of seconds you want to have pass before IP-Reveal refreshes your IP '
+                             'information. (Defaults to 30)',
+                        action='store')
+
+    parser.add_argument('-V', '--version', action='version', version='1.2'
+                        )
+
+    sub_parsers = parser.add_subparsers(
+        dest='subcommands', help='The sub-commands for IP Reveal')
+
+    ext_ip_parse = sub_parsers.add_parser('get-external',
+                                          help='Return the external IP to the command-line and nothing else.')
+    host_parse = sub_parsers.add_parser(
+        'get-host', help='Return the hostname to the command-line and nothing else.')
+    local_parse = sub_parsers.add_parser('get-local',
+                                         help='Return the local IP-Address to the command-line and nothing '
+                                              'else.')
+    test_audio_parse = sub_parsers.add_parser('test-audio',
+                                              help="To ensure you get notifications you can test IP-Reveal's audio "
+                                                   "engine with this command.")
+    test_audio_parse.add_argument('-c', '--countdown',
+                                  action='store',
+                                  type=int,
+                                  default=3,
+                                  help="Enter the number to countdown from before starting the test.")
+    test_audio_parse.add_argument('-f', '--full',
+                                  help='Run the full range of audio tests provided by the audio engine',
+                                  action='store_true',
+                                  default=False)
+
+    args = parser.parse_args()
+
+    config.args = args
+
+    # Set up the logging device
+    log_device = InspyLogger(log_name, args.log_level).device
+
+    # Start the logging device
+    log = log_device.start(mute=args.subcommands)
+    debug = log.debug
+
+    # Announce that we did that
+    debug('Started my logger!')
+    log = getLogger(log_name + '.Main')
+    # Alias the log.debug signature for ease-of-use
+    debug = log.debug
+
+    # See if we got one of the subcommands assigned.
+    if args.subcommands == 'get-external':
+        print(get_external())
+        exit()
+    elif args.subcommands == 'get-host':
+        print(get_hostname())
+        exit()
+    elif args.subcommands == 'get-local':
+        print(get_internal())
+        exit()
+    elif args.subcommands == 'test-audio':
+        from ip_reveal.assets.sounds import run_audio_test
+        run_audio_test(args.countdown, args.full, args.log_level)
+        exit()
+
+    status_bar_layout = [
+
+    ]
+
+    bg_color = "340245"
+    size = (220, 50)
+    alpha = 1
+    text_background_color = "pink" if alpha >= 1 else "white"
+    layout = [
+        [
+            Qt.Text(
+                'External IP:',
+                background_color=text_background_color,
+                text_color="black",
+                relief=Qt.RELIEF_GROOVE,
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+            Qt.Text(
+                get_external(),
+                relief=Qt.RELIEF_SUNKEN,
+                key='EXTIP_OUT',
+                background_color=text_background_color,
+                text_color="black",
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+        ],
+        [
+            Qt.Text(
+                'Internal IP:',
+                background_color=text_background_color,
+                text_color="black",
+                relief=Qt.RELIEF_GROOVE,
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+            Qt.Text(
+                get_internal(),
+                key='INTIP_OUT',
+                relief=Qt.RELIEF_SUNKEN,
+                background_color=text_background_color,
+                text_color="black",
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+        ],
+        [
+            Qt.Text(
+                'Hostname:',
+                background_color=text_background_color,
+                text_color="black",
+                relief=Qt.RELIEF_GROOVE,
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+            Qt.Text(
+                get_hostname(),
+                key='HOSTNAME_OUT',
+                relief=Qt.RELIEF_SUNKEN,
+                background_color=text_background_color,
+                text_color="black",
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+        ],
+        [
+            Qt.Text(
+                'Last checked',
+                background_color=text_background_color,
+                text_color="black",
+                relief=Qt.RELIEF_GROOVE,
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+            Qt.Text(
+                t_text,
+                key="TIME_SINCE_Q_OUT",
+                relief=Qt.RELIEF_SUNKEN,
+                background_color=text_background_color,
+                text_color="black",
+                size_px=size,
+                auto_size_text=True,
+                justification='center',
+            ),
+        ],
+        [
+            Qt.Button(
+                '',
+                key='MAIN_CLOSE_BUTTON',
+                image_filename=app_quit_50x50_fp,
+                image_size=(50, 50),
+                button_color=(None, "#ff0000"),
+                tooltip="Quit IP Reveal",
+            ),
+            Qt.Button(
+                '',
+                key='MAIN_REFRESH_BUTTON',
+                image_filename=app_refresh_50x50_fp,
+                image_size=(50, 50),
+                button_color=(None, "#ff0000"),
+                tooltip="Refresh",
+            ),
+        ],
+    ]
+
+
+    # Assemble the above widget into a window.
+    window = Qt.Window('IP-Reveal by Inspyre Softworks', layout=layout,
+                       background_image=NEON_DARK_FP,
+                       icon=app_main_24x24,
+                       size=(300, 400),
+                       alpha_channel=alpha,
+                       grab_anywhere=True,
+                       background_color="white"
+                       )
+
+
+    # Start our main GUI loop.
+    while True:
+        event, values = window.read(timeout=100)
+
+        # Set up a child logger that will log window events.
+        w_log = getLogger(log_name + '.MainWindow')
+        w_debug = w_log.debug
+
+        # Increment the cycle count
+        acc += 1
+        total_acc += 1
+
+        t = int(timer.get_elapsed(seconds=True))
+        t_text = humanize.naturaldelta(t)
+
+        window['TIME_SINCE_Q_OUT'].update(f"{t_text} ago...")
+
+        # If the accumulator is at 325 counts, alert the user, update the window, and reset the accumulator
+        if t == args.refresh_interval:
+            w_debug('Calling function to update the window...')
+
+            window['TIME_SINCE_Q_OUT'].update('Refreshing...')
+            update_win = Thread(target=update_window)
+
+            update_win.start()
+            w_debug('Updated window!')
+
+        # If the 'Close' button is pressed: we exit.
+        if event is None or event == 'MAIN_CLOSE_BUTTON':
+            e_reason = f"It seems the user closed the window, received {values}"
+            if event == 'MAIN_CLOSE_BUTTON':
+                e_reason = 'The close button was pressed'
+            safe_exit(window, exit_reason=e_reason)
+
+            w_log.info("User initiated closing")
+
+            break
+
+        if event == 'MAIN_REFRESH_BUTTON':
+            w_debug('Calling a refresh on the window')
+            update_window()
+            w_debug('All seems well!')
```

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/__init__.py` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from ip_reveal.assets.sounds import alerts
-
-
-def run_audio_test(countdown=3, full=False, log_level='debug'):
-    """
-    
-    Run a left-right channel audio-test to ensure 'simpleaudio' is working correctly.
-    
-    Returns:
-        None
-
-    """
-    from inspy_logger import InspyLogger
-    
-    isl = InspyLogger('IP-Reveal.assets.sounds.run_audio_test', log_level)
-    log = isl.device.start()
-    
-    log.debug('Importing "simpleaudio"...')
-    
-    from simpleaudio.functionchecks import LeftRightCheck as LRC, run_all
-    
-    log.debug('Done!')
-    log.debug('Determining test type....')
-    log.debug(f'Full test: | {full}')
-    log.debug(f'Countdown: | {countdown}')
-    
-    if not full:
-        LRC.run(countdown=countdown)
-    else:
-        run_all(countdown=countdown)
-    
-
-class Alerts(object):
-    
-    import simpleaudio as sa
-    from ip_reveal.config import args
-    
-    def __init__(self):
-        """
-        Initialize an "Alerts" class that contains sounds for alerts.
-        """
-        self.asset_fp = alerts.ALERT_AUDIO_FP
-        self.o_pulse_fp = alerts.O_PULSE_FP
-        self.sound = self.sa.WaveObject.from_wave_file(self.o_pulse_fp)
-        
-        
-        
-    def play(self):
-        self.sound.play()
+from ip_reveal.assets.sounds import alerts
+
+
+def run_audio_test(countdown=3, full=False, log_level='debug'):
+    """
+    
+    Run a left-right channel audio-test to ensure 'simpleaudio' is working correctly.
+    
+    Returns:
+        None
+
+    """
+    from inspy_logger import InspyLogger
+    
+    isl = InspyLogger('IP-Reveal.assets.sounds.run_audio_test', log_level)
+    log = isl.device.start()
+    
+    log.debug('Importing "simpleaudio"...')
+    
+    from simpleaudio.functionchecks import LeftRightCheck as LRC, run_all
+    
+    log.debug('Done!')
+    log.debug('Determining test type....')
+    log.debug(f'Full test: | {full}')
+    log.debug(f'Countdown: | {countdown}')
+    
+    if not full:
+        LRC.run(countdown=countdown)
+    else:
+        run_all(countdown=countdown)
+    
+
+class Alerts(object):
+    
+    import simpleaudio as sa
+    from ip_reveal.config import args
+    
+    def __init__(self):
+        """
+        Initialize an "Alerts" class that contains sounds for alerts.
+        """
+        self.asset_fp = alerts.ALERT_AUDIO_FP
+        self.o_pulse_fp = alerts.O_PULSE_FP
+        self.sound = self.sa.WaveObject.from_wave_file(self.o_pulse_fp)
+        
+        
+        
+    def play(self):
+        self.sound.play()
```

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/alerts/blip_pulse.wav` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/blip_pulse.wav`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/alerts/low_pulse.wav` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/low_pulse.wav`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/alerts/o-pulse-alert.mp3` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/o-pulse-alert.mp3`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/alerts/o-pulse-alert.wav` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/o-pulse-alert.wav`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/alerts/o-pulse.wav` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/o-pulse.wav`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/sounds/alerts/scifi_pulse.wav` & `ip_reveal-1.3.dev1/ip_reveal/assets/sounds/alerts/scifi_pulse.wav`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/backgrounds/neon_dark.png` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/backgrounds/neon_dark.png`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/2897337-48.png` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/2897337-48.png`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/__init__.py` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/__init__.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from pathlib import Path
-
-# Get the directory we're currently in which contains the icons
-cwd = str(Path(__file__).parent.absolute())
-
-# Where do we keep our icon files?
-ICON_DIR = cwd + '/assets/ui_elements/icons'
-
-# Our list of icons
-# ToDo:
-#   * Enable end-user to choose themes which change the icons as well as other window elements.
-app_main_48 = b'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'
-app_main_32x32 = b'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ADUAAAALAAAAC0kVADVeGgA0XhoANFkaADSedgs3AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA//////////////////////AD/A/wA/wP8AP8D/AH9A/zwAPP84ABz/MAAM/yAABP8AAAD/AgBA/AAAADwAAAA8AAAAPAAAAD8CAED/AAAA/yAABP8wAAz/OAAc/zwAPP8C/gD/A/wA/wP8AP8D/AD/////////////////////8='
-app_main_24x24 = b'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'
-app_main_16x16 = b'AAABAAEAEBAAAAEAIABoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAYFRABAAAAAAAAAAAAAAAAFQcFrxcTDaZKQi6AAAAAgAAAAIQAAAAAAAAAAAAAAAAAAAAABwUDhAYGBaZDPC2vAAAAAAAAAAAAAAAAAAAAAEwPC/9MMCCukIBUgAAAAHoAAAByAAAAAAAAAAAAAAAAAAAAACEfGoQqKSWuZ1xE/wAAAAAAAAAAAAAAAAAAAABfOwD5/6UADQAAAAgkHxF+PjIx/2IwOP9jMjn/IBAS/xITEIYaHRcIAAAADT83J/kAAAAAAAAAAAAAAAAAAAAAe0kA+FMrACczLBzwjHtN/zMwK8GUSVT0oVBc9CUQFMFERDv/YF9T8A4SDyc4NS74AAAAAAAAAAAAAAAAAAAAAGE5AP8gGQ3/t6Fm3BEOBUlANjH/RiMmzzsfIs8mEA3/LzQuSWNgWNxMQjn/OTQp/wAAAAAAAAAAAAAAEkgqALV6SAD/OSoV/2RTN+YAAADqgHpl/hoDAc4WBQPOAAAA/mpgTuoSDgnmMSwm/ykkGf9MRDC1XlQ6EgAAABJwQwC1YjoA/z4vGf9vWTzmAAAA6pGJcP4uBwTOKgoIzgAAAP5zWDbqCQYD5kA8OP9KQzL/kYFatZ2NYhIAAAAAAAAAACwlGv8MCQb/UE9B3AAAAEkpKCL/PkI2zzoNCs8pGRf/aFIzSTMnF9wwLCn/c10q/wAAAAAAAAAAAAAAAAAAAABHOif4QDEgJzU1LPBPT0H/ODcwwYiPdvRzGRL0EgwLwQcHB/9LQznwFQcEJ6d5APgAAAAAAAAAAAAAAAAAAAAASz0p+f3Miw0AAAAIMzQphmBcUf9mX1P/RBEJ/08vIP9UVFF+////CAAAAA2dcgD5AAAAAAAAAAAAAAAAAAAAAAYHBv8gHxuuREM6hAAAAAAAAAAAAAAAAAAAAAAAAAByAAAAeh4JAIAnCQCuaUwB/wAAAAAAAAAAAAAAAAAAAAAvLymvV1ZLpoSDcoQAAAAAAAAAAAAAAAAAAAAAAAAAhAAAAIBAEgCAdCAApmhDBq8AAAAAAAAAAAAAAAAoKCMBAAAAAAAAAAAAAAAAdHNkAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAeVQHAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA//8AAL/9AADB4wAAweMAAMADAADAAwAAwAMAAAAAAAAAAAAAwAMAAMADAADAAwAAx4MAAMeDAAC//QAA//8AAA=='
-app_quit_92x92_fp = cwd + "/neon_quit_92x92.ico"
-app_quit_50x50_fp = cwd + "/neon_quit_50x50.ico"
-app_refresh_50x50_fp = cwd + "/neon_refresh_50x50.ico"
+from pathlib import Path
+
+# Get the directory we're currently in which contains the icons
+cwd = str(Path(__file__).parent.absolute())
+
+# Where do we keep our icon files?
+ICON_DIR = cwd + '/assets/ui_elements/icons'
+
+# Our list of icons
+# ToDo:
+#   * Enable end-user to choose themes which change the icons as well as other window elements.
+app_main_48 = b'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'
+app_main_32x32 = b'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ADUAAAALAAAAC0kVADVeGgA0XhoANFkaADSedgs3AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA//////////////////////AD/A/wA/wP8AP8D/AH9A/zwAPP84ABz/MAAM/yAABP8AAAD/AgBA/AAAADwAAAA8AAAAPAAAAD8CAED/AAAA/yAABP8wAAz/OAAc/zwAPP8C/gD/A/wA/wP8AP8D/AD/////////////////////8='
+app_main_24x24 = b'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'
+app_main_16x16 = b'AAABAAEAEBAAAAEAIABoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAYFRABAAAAAAAAAAAAAAAAFQcFrxcTDaZKQi6AAAAAgAAAAIQAAAAAAAAAAAAAAAAAAAAABwUDhAYGBaZDPC2vAAAAAAAAAAAAAAAAAAAAAEwPC/9MMCCukIBUgAAAAHoAAAByAAAAAAAAAAAAAAAAAAAAACEfGoQqKSWuZ1xE/wAAAAAAAAAAAAAAAAAAAABfOwD5/6UADQAAAAgkHxF+PjIx/2IwOP9jMjn/IBAS/xITEIYaHRcIAAAADT83J/kAAAAAAAAAAAAAAAAAAAAAe0kA+FMrACczLBzwjHtN/zMwK8GUSVT0oVBc9CUQFMFERDv/YF9T8A4SDyc4NS74AAAAAAAAAAAAAAAAAAAAAGE5AP8gGQ3/t6Fm3BEOBUlANjH/RiMmzzsfIs8mEA3/LzQuSWNgWNxMQjn/OTQp/wAAAAAAAAAAAAAAEkgqALV6SAD/OSoV/2RTN+YAAADqgHpl/hoDAc4WBQPOAAAA/mpgTuoSDgnmMSwm/ykkGf9MRDC1XlQ6EgAAABJwQwC1YjoA/z4vGf9vWTzmAAAA6pGJcP4uBwTOKgoIzgAAAP5zWDbqCQYD5kA8OP9KQzL/kYFatZ2NYhIAAAAAAAAAACwlGv8MCQb/UE9B3AAAAEkpKCL/PkI2zzoNCs8pGRf/aFIzSTMnF9wwLCn/c10q/wAAAAAAAAAAAAAAAAAAAABHOif4QDEgJzU1LPBPT0H/ODcwwYiPdvRzGRL0EgwLwQcHB/9LQznwFQcEJ6d5APgAAAAAAAAAAAAAAAAAAAAASz0p+f3Miw0AAAAIMzQphmBcUf9mX1P/RBEJ/08vIP9UVFF+////CAAAAA2dcgD5AAAAAAAAAAAAAAAAAAAAAAYHBv8gHxuuREM6hAAAAAAAAAAAAAAAAAAAAAAAAAByAAAAeh4JAIAnCQCuaUwB/wAAAAAAAAAAAAAAAAAAAAAvLymvV1ZLpoSDcoQAAAAAAAAAAAAAAAAAAAAAAAAAhAAAAIBAEgCAdCAApmhDBq8AAAAAAAAAAAAAAAAoKCMBAAAAAAAAAAAAAAAAdHNkAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAeVQHAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA//8AAL/9AADB4wAAweMAAMADAADAAwAAwAMAAAAAAAAAAAAAwAMAAMADAADAAwAAx4MAAMeDAAC//QAA//8AAA=='
+app_quit_92x92_fp = cwd + "/neon_quit_92x92.ico"
+app_quit_50x50_fp = cwd + "/neon_quit_50x50.ico"
+app_refresh_50x50_fp = cwd + "/neon_refresh_50x50.ico"
```

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/alerts/__init__.py` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/alerts/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-icons_alert_shield = b'iVBORw0KGgoAAAANSUhEUgAAACgAAAAoCAYAAACM/rhtAAAABmJLR0QA/wD/AP' \
-                     b'+gvaeTAAAHLUlEQVRYhc2Ya4xVVxWAv7X3Oee+ZoZHsUUepRZqxCYlmrTUpI0xplLTNrX+MMaYkgFjkUctDKXGX' \
-                     b'/PLxhLAyEMxoUBStbU2aRNMajVRU5NSqA2QUkoZOzAgw2Ng7nDnvs5jL3/MDN6Ze+cFpLh+7XP22mt9Z' \
-                     b'+21V9bZ8H8ucqMMbV69+3sKWwAV5Zl121tfvhF2rxvw5xt2NXtluxnV1i/47riJojnHNJ1D3K4oq' \
-                     b'+ufe2F54aYBblyz5xHjdJtvyH49HedmWpcr9Ja4ZHx9x2YLVeSSOFau29H65qcGuPOHO' \
-                     b'/1CKnhMlJ8C99zhadcDqWh+rzO8E1qS2PElV2KKSzjiN/WfVC' \
-                     b'+jhvfFmedzUWXfU795KrqhgNtW7b2latxdorpQkSXAwwLpWdad' \
-                     b'+Eo6WZAWTR8OLUdDy3zPEYUxXSZgQVJloVaoIhzzspdO4bUARYU3Rfgz8FHKmROrty' \
-                     b'+9NCnAzat2f1eF9cBMYCqQAzBwYbrR7s' \
-                     b'/7Se4Oz93pCeZkbPhXaAG4P0iY6zkKvSXOis9hm0ER7nZlbnchsQjnTVDpMkG+B5uOBmwDFIE8cA50Y9u2Za' \
-                     b'+MCvj8j347LbBh9zzffTTLupY0ZJpFp0wxmrGDmnkndMWG45GlqvBFP' \
-                     b'+GeVII3aKPQWwIgQfjYpDhu0wQ45iUh8zSkSd3gPPSLpWJMHBqTXMTv78RrNh63rf1Fa36IyasFtH44A0dqcRAvygqUnNCVCJ2J4YoTLjqh5IQWURb6MXf5Skq04dZYlIWuwnxXpcsGnDQBHaR4LO4jLx4XxCOFY7aLvCBRb4ZEqU6vhcjxmcGI1gNKaPvwEiIVEKXHCcciS06UFgOLfMcs62g2DaAEgsWfo6kc0v+PEzCoEqAsSKosoEqMYICiGM4aj1AM6UT5rEaEg5sZSHyl1uwwwOLMdL65p0g4+Hy757jdcw0jNFLM9CZSX11ACqh8eI74Qn358wap57qQuS4cNjd0tPN9Xt8wu7UP7e3fCUU0Dhvv2tjikqtDTZIxFBvLQHTVte9prYwKCGBUSqFOoDzKcB2t1ACW40kDRiJYJBz5vh5QtH88QC+VxgapYZBajQbyTsFVJlWLAYgxGChPAJC+Mc2LDGTSyG9wikYxrhqBm3yOhICg/eMCJsjFyljnQpUkrJJUq6AjQCoxOkb0Uk1ZjK1zOQhoULg4LqBT01HQUYpbDWQdHKCVCFdqDOinA7ItOXLTWhpCFsUQiRwdF1BJOvucmXwSMZB7rlyX54gxpLIZRAQv8PEz6XpAY9Qpn4x87418oWqOXAGjXEOrU4nRsL7EqHP0X+6jafoUqqUyUWX4RyjQrwY1HBm5tn6LY7PfqXo9bvKtooYxGo5eYor5Qh0cwGXxiEUkUbd/XMBnf/3kBYN2nIknDxh/eI7yoTOjzqtrfPrOiY+Hnnlu2/Kz4wICOHilK7HFyQImp/NUT16e7DK6recS5KVGcw0BjZM/9iaSu9xgm0WkYW5KJiC74gFu+8lD2Ob6QzCa5MWjD2tE9dUJA67d0XpI0Hc/CE21bkGQRoKgflFgMRkfk/GRjD9hwA4bYODQ2u3L3m80X3eKh0SRTZ2J97t71ZGpKYtJWOFqL1Wr31em9NIBSoWwYSfTSCpiOC2BS0RfGE2ncVkHCjNOvYbqB+9VR+SiaiO+AfjuK4SnJ56DR01aFTr6b+lquL1jAra3tzunbPh3bLLnEkNSk3nDxjW8jv+NdaTeiHGPeHQaX3D8uL29fdTaZEebAHjr4BufLLnvWwu7E5l7ODLpOVbJGNhX9kkLTDXK36oeZYVbrXKgaulOLDM1psOkOGFTzHUR/zE+B70sd7qQvFj+4jfTY4IwRF5v2976s7EYRo3gkIifrCyrFCOVq11v7GDok+Oa6MRAPNiCJTLQhA5EDBId0hFihIJKXsNwxbj+x1MA2Lxm94Oq8td7g7h6d5A09zjDFOPwgV4nZERJCxScUOwrk8NRFaGCYYomxCIUsEzTmA6T1iM2HSfwjWe3tf79hgACbFr94veBvQ+mk+J8zzWPpjf029lITptAD5osaljWtrV1z0T8jpmDtfLWgTeOLFn8RP50ZB7NGL0yw2rDahyO0g+esil30GYRIxvatrb+aqJ+Jww4APn6uw/d9/jZM4n37QTOz7JaF8lGgMdsJjlsUoKyum1b6y8n4/Oabrc2r9z9MKKvzvG072uZeHbtSavdYgcc8nJhpwSI6tJruTO85uu3TWt2LRK1+6ZaJ99MR7MDGQ4Yi7Dfy5bP45fVucfX71j+z2vxc133g5tX7J2tnvtTWnTmo5n41iajUugtUcbwtp8rFfDOovJI2/alH1+rj+u+Yd3yzO6pGvOahS8vycR+pVDJvm1z5VDkPfGTJ9Zt+cHk+68bCQjQ3v6HoPlicSfCkwAov/dNYfnTW5+u64Zuqmxc9eLiTWt233+zOT5V+S8B3z5ULV+fGgAAAABJRU5ErkJggg== '
+icons_alert_shield = b'iVBORw0KGgoAAAANSUhEUgAAACgAAAAoCAYAAACM/rhtAAAABmJLR0QA/wD/AP' \
+                     b'+gvaeTAAAHLUlEQVRYhc2Ya4xVVxWAv7X3Oee+ZoZHsUUepRZqxCYlmrTUpI0xplLTNrX+MMaYkgFjkUctDKXGX' \
+                     b'/PLxhLAyEMxoUBStbU2aRNMajVRU5NSqA2QUkoZOzAgw2Ng7nDnvs5jL3/MDN6Ze+cFpLh+7XP22mt9Z' \
+                     b'+21V9bZ8H8ucqMMbV69+3sKWwAV5Zl121tfvhF2rxvw5xt2NXtluxnV1i/47riJojnHNJ1D3K4oq' \
+                     b'+ufe2F54aYBblyz5xHjdJtvyH49HedmWpcr9Ja4ZHx9x2YLVeSSOFau29H65qcGuPOHO' \
+                     b'/1CKnhMlJ8C99zhadcDqWh+rzO8E1qS2PElV2KKSzjiN/WfVC' \
+                     b'+jhvfFmedzUWXfU795KrqhgNtW7b2latxdorpQkSXAwwLpWdad' \
+                     b'+Eo6WZAWTR8OLUdDy3zPEYUxXSZgQVJloVaoIhzzspdO4bUARYU3Rfgz8FHKmROrty' \
+                     b'+9NCnAzat2f1eF9cBMYCqQAzBwYbrR7s' \
+                     b'/7Se4Oz93pCeZkbPhXaAG4P0iY6zkKvSXOis9hm0ER7nZlbnchsQjnTVDpMkG+B5uOBmwDFIE8cA50Y9u2Za' \
+                     b'+MCvj8j347LbBh9zzffTTLupY0ZJpFp0wxmrGDmnkndMWG45GlqvBFP' \
+                     b'+GeVII3aKPQWwIgQfjYpDhu0wQ45iUh8zSkSd3gPPSLpWJMHBqTXMTv78RrNh63rf1Fa36IyasFtH44A0dqcRAvygqUnNCVCJ2J4YoTLjqh5IQWURb6MXf5Skq04dZYlIWuwnxXpcsGnDQBHaR4LO4jLx4XxCOFY7aLvCBRb4ZEqU6vhcjxmcGI1gNKaPvwEiIVEKXHCcciS06UFgOLfMcs62g2DaAEgsWfo6kc0v+PEzCoEqAsSKosoEqMYICiGM4aj1AM6UT5rEaEg5sZSHyl1uwwwOLMdL65p0g4+Hy757jdcw0jNFLM9CZSX11ACqh8eI74Qn358wap57qQuS4cNjd0tPN9Xt8wu7UP7e3fCUU0Dhvv2tjikqtDTZIxFBvLQHTVte9prYwKCGBUSqFOoDzKcB2t1ACW40kDRiJYJBz5vh5QtH88QC+VxgapYZBajQbyTsFVJlWLAYgxGChPAJC+Mc2LDGTSyG9wikYxrhqBm3yOhICg/eMCJsjFyljnQpUkrJJUq6AjQCoxOkb0Uk1ZjK1zOQhoULg4LqBT01HQUYpbDWQdHKCVCFdqDOinA7ItOXLTWhpCFsUQiRwdF1BJOvucmXwSMZB7rlyX54gxpLIZRAQv8PEz6XpAY9Qpn4x87418oWqOXAGjXEOrU4nRsL7EqHP0X+6jafoUqqUyUWX4RyjQrwY1HBm5tn6LY7PfqXo9bvKtooYxGo5eYor5Qh0cwGXxiEUkUbd/XMBnf/3kBYN2nIknDxh/eI7yoTOjzqtrfPrOiY+Hnnlu2/Kz4wICOHilK7HFyQImp/NUT16e7DK6recS5KVGcw0BjZM/9iaSu9xgm0WkYW5KJiC74gFu+8lD2Ob6QzCa5MWjD2tE9dUJA67d0XpI0Hc/CE21bkGQRoKgflFgMRkfk/GRjD9hwA4bYODQ2u3L3m80X3eKh0SRTZ2J97t71ZGpKYtJWOFqL1Wr31em9NIBSoWwYSfTSCpiOC2BS0RfGE2ncVkHCjNOvYbqB+9VR+SiaiO+AfjuK4SnJ56DR01aFTr6b+lquL1jAra3tzunbPh3bLLnEkNSk3nDxjW8jv+NdaTeiHGPeHQaX3D8uL29fdTaZEebAHjr4BufLLnvWwu7E5l7ODLpOVbJGNhX9kkLTDXK36oeZYVbrXKgaulOLDM1psOkOGFTzHUR/zE+B70sd7qQvFj+4jfTY4IwRF5v2976s7EYRo3gkIifrCyrFCOVq11v7GDok+Oa6MRAPNiCJTLQhA5EDBId0hFihIJKXsNwxbj+x1MA2Lxm94Oq8td7g7h6d5A09zjDFOPwgV4nZERJCxScUOwrk8NRFaGCYYomxCIUsEzTmA6T1iM2HSfwjWe3tf79hgACbFr94veBvQ+mk+J8zzWPpjf029lITptAD5osaljWtrV1z0T8jpmDtfLWgTeOLFn8RP50ZB7NGL0yw2rDahyO0g+esil30GYRIxvatrb+aqJ+Jww4APn6uw/d9/jZM4n37QTOz7JaF8lGgMdsJjlsUoKyum1b6y8n4/Oabrc2r9z9MKKvzvG072uZeHbtSavdYgcc8nJhpwSI6tJruTO85uu3TWt2LRK1+6ZaJ99MR7MDGQ4Yi7Dfy5bP45fVucfX71j+z2vxc133g5tX7J2tnvtTWnTmo5n41iajUugtUcbwtp8rFfDOovJI2/alH1+rj+u+Yd3yzO6pGvOahS8vycR+pVDJvm1z5VDkPfGTJ9Zt+cHk+68bCQjQ3v6HoPlicSfCkwAov/dNYfnTW5+u64Zuqmxc9eLiTWt233+zOT5V+S8B3z5ULV+fGgAAAABJRU5ErkJggg== '
```

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/alerts/icons8-warning-shield-40.png` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/alerts/icons8-warning-shield-40.png`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_apply_en_unsel_48x48.png` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_apply_en_unsel_48x48.png`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main-48.png` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main-48.png`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main_16x16.ico` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main_16x16.ico`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main_24x24.ico` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main_24x24.ico`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_main_32x32.ico` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_main_32x32.ico`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_quit_50x50.ico` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_quit_50x50.ico`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_quit_92x92.ico` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_quit_92x92.ico`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/assets/ui_elements/icons/neon_refresh_50x50.ico` & `ip_reveal-1.3.dev1/ip_reveal/assets/ui_elements/icons/neon_refresh_50x50.ico`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/config/errors.py` & `ip_reveal-1.3.dev1/ip_reveal/config/errors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-
-class NoStoredConfigError(Exception):
-    """
-    
-    Raised when the program is unable to find a stored config-file or flag-file.
-    
-    
-    """
-    def __init__(self, message:str=None, no_print=False, logger=None):
-        """
-        
-        Raised when the program has tried and been unable to find a config file, nor a valid flag file in the given
-        locations.
-        
-        Args:
-            message(str): A message to be delivered upon raising of this exception. (*Default* Was unable to find a
-                          valid config file, nor was I able to find a valid flag file in this location):
-            no_print(bool): Do not do any printing on initialization, let the caller handle it.
-        """
-        msg = "Was unable to find a valid config file, nor was I able to find a valid flag file in this location"
-        if message is not None:
-            self.message = msg + f' {message}'
-        else:
-            self.message = msg
-            
-        self.msg = self.message
-        
-        if not no_print:
-            print()
+
+class NoStoredConfigError(Exception):
+    """
+    
+    Raised when the program is unable to find a stored config-file or flag-file.
+    
+    
+    """
+    def __init__(self, message:str=None, no_print=False, logger=None):
+        """
+        
+        Raised when the program has tried and been unable to find a config file, nor a valid flag file in the given
+        locations.
+        
+        Args:
+            message(str): A message to be delivered upon raising of this exception. (*Default* Was unable to find a
+                          valid config file, nor was I able to find a valid flag file in this location):
+            no_print(bool): Do not do any printing on initialization, let the caller handle it.
+        """
+        msg = "Was unable to find a valid config file, nor was I able to find a valid flag file in this location"
+        self.message = msg + f' {message}' if message is not None else msg
+        self.msg = self.message
+
+        if not no_print:
+            print()
```

### Comparing `ip-reveal-1.2/ip_reveal/gui/windows/.test.py.swp` & `ip_reveal-1.3.dev1/ip_reveal/gui/windows/.test.py.swp`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/gui/windows/preferences.py` & `ip_reveal-1.3.dev1/ip_reveal/gui/windows/preferences.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,56 @@
-import PySimpleGUIQt as psg
-
-
-class Window(object):
-    
-    active = False
-    
-    tab1_layout = [
-            [psg.Checkbox('Enable SecureKill', enable_events=True, key='SECURE_KILL_CHECK')],
-            [psg.Text('Name of program to kill:', visible=False, key='SECURE_KILL_PROG_LABEL', size=(175,30)),
-             psg.InputText(visible=False, key='SECURE_KILL_PROG', size=(175,30))]
-            ]
-    
-    layout = [
-            [
-                    psg.TabGroup([[psg.Tab('SecureKill', tab1_layout, tooltip='Kill a program if your IP changes.',)]])
-                    ],
-            [
-                    psg.Button('Save and Exit', disabled=True, key='SAVE_BUTTON'),
-                    psg.Button('Exit', key='EXIT_BUTTON')
-                    ]
-            
-            ]
-    
-    win = psg.Window('Preferences', layout=layout, size=(400,200))
-    
-    running = False
-    
-    def run(self):
-        self.running = True
-        vals_last_save = None
-        while self.running:
-            event, values = self.win.read(100)
-            
-            if vals_last_save is None:
-                vals_last_save = values
-                
-            vals_differ = (vals_last_save != values)
-            
-            if vals_differ:
-                save_button_color = 'green'
-            else:
-                save_button_color = 'red'
-            
-            self.win['SAVE_BUTTON'].update(disabled=not vals_differ, button_color=('black', save_button_color))
-            
-            cbox_now = values['SECURE_KILL_CHECK']
-            
-            self.win['SECURE_KILL_PROG_LABEL'].update(visible=cbox_now)
-            self.win['SECURE_KILL_PROG'].update(visible=cbox_now)
-            
-            if event is None:
-                self.running = False
-                self.win.close()
-            if event == 'EXIT_BUTTON':
-                self.running = False
-                self.win.close
-
-win = Window()
-win.run()
+import PySimpleGUIQt as psg
+
+
+class Window(object):
+    
+    active = False
+    
+    tab1_layout = [
+            [psg.Checkbox('Enable SecureKill', enable_events=True, key='SECURE_KILL_CHECK')],
+            [psg.Text('Name of program to kill:', visible=False, key='SECURE_KILL_PROG_LABEL', size=(175,30)),
+             psg.InputText(visible=False, key='SECURE_KILL_PROG', size=(175,30))]
+            ]
+    
+    layout = [
+            [
+                    psg.TabGroup([[psg.Tab('SecureKill', tab1_layout, tooltip='Kill a program if your IP changes.',)]])
+                    ],
+            [
+                    psg.Button('Save and Exit', disabled=True, key='SAVE_BUTTON'),
+                    psg.Button('Exit', key='EXIT_BUTTON')
+                    ]
+            
+            ]
+    
+    win = psg.Window('Preferences', layout=layout, size=(400,200))
+    
+    running = False
+    
+    def run(self):
+        self.running = True
+        vals_last_save = None
+        while self.running:
+            event, values = self.win.read(100)
+
+            if vals_last_save is None:
+                vals_last_save = values
+
+            vals_differ = (vals_last_save != values)
+
+            save_button_color = 'green' if vals_differ else 'red'
+            self.win['SAVE_BUTTON'].update(disabled=not vals_differ, button_color=('black', save_button_color))
+
+            cbox_now = values['SECURE_KILL_CHECK']
+
+            self.win['SECURE_KILL_PROG_LABEL'].update(visible=cbox_now)
+            self.win['SECURE_KILL_PROG'].update(visible=cbox_now)
+
+            if event is None:
+                self.running = False
+                self.win.close()
+            if event == 'EXIT_BUTTON':
+                self.running = False
+                self.win.close
+
+win = Window()
+win.run()
```

### Comparing `ip-reveal-1.2/ip_reveal/popups/__init__.py` & `ip_reveal-1.3.dev1/ip_reveal/popups/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-import PySimpleGUI as Gui
-from ip_reveal.assets.ui_elements.icons.alerts import icons_alert_shield
-from ip_reveal.assets.sounds import Alerts
-from threading import Thread
-from pypattyrn.behavioral.null import Null
-from ip_reveal.config import args
-
-GUI = Gui
-
-
-if args.mute_all:
-    bell = Null()
-else:
-    bell = Alerts()
-
-
-def notify(msg, duration=7000, alpha=.8, location=(750, 450), icon=icons_alert_shield):
-    bell.play()
-    GUI.popup_notify(msg, display_duration_in_ms=duration, alpha=alpha,
-                     location=location, icon=icon)
-
-
-def ip_change_notify(old, new, muted=False, log_device=None):
-    """
-
-    Play and alert sound and produce a notification in the center of the screen alerting the user that their external IP
-    address has changed
-
-    Args:
-
-        old (str): The old IP Address, as recorded.
-
-        new (str): The new IP Address that the machine now has, as recorded.
-        
-        muted (bool): Is the sound for the program muted? If bool(True); does not produce noise with notification.
-        
-
-    Returns:
-        None
-
-    """
-    message = f'Your external IP address has changed from {old} to {new}'
-    notif = Thread(target=notify, args=(message,))
-    notif.start()
+import PySimpleGUI as Gui
+from ip_reveal.assets.ui_elements.icons.alerts import icons_alert_shield
+from ip_reveal.assets.sounds import Alerts
+from threading import Thread
+from pypattyrn.behavioral.null import Null
+from ip_reveal.config import args
+
+GUI = Gui
+
+
+bell = Null() if args.mute_all else Alerts()
+
+
+def notify(msg, duration=7000, alpha=.8, location=(750, 450), icon=icons_alert_shield):
+    bell.play()
+    GUI.popup_notify(msg, display_duration_in_ms=duration, alpha=alpha,
+                     location=location, icon=icon)
+
+
+def ip_change_notify(old, new, muted=False, log_device=None):
+    """
+
+    Play and alert sound and produce a notification in the center of the screen alerting the user that their external IP
+    address has changed
+
+    Args:
+
+        old (str): The old IP Address, as recorded.
+
+        new (str): The new IP Address that the machine now has, as recorded.
+        
+        muted (bool): Is the sound for the program muted? If bool(True); does not produce noise with notification.
+        
+
+    Returns:
+        None
+
+    """
+    message = f'Your external IP address has changed from {old} to {new}'
+    notif = Thread(target=notify, args=(message,))
+    notif.start()
```

### Comparing `ip-reveal-1.2/ip_reveal/popups/__pycache__/__init__.cpython-36.pyc` & `ip_reveal-1.3.dev1/ip_reveal/popups/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/timers/__pycache__/__init__.cpython-36.pyc` & `ip_reveal-1.3.dev1/ip_reveal/timers/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/tools/__pycache__/__init__.cpython-36.pyc` & `ip_reveal-1.3.dev1/ip_reveal/tools/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ip-reveal-1.2/ip_reveal/tools/arguments/__init__.py` & `ip_reveal-1.3.dev1/ip_reveal/tools/arguments/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-from argparse import ArgumentParser
-
-
-def super():
-    pass
-
-
-class ArgParser(ArgumentParser):
-
-    def __init__(self):
-        """
-
-        Instantiate an argument parser.
-
-        """
-        super().__init__(help="Use this option if you'd like the most output from the program into the console you "
-                               "can get")
-
-        self.add_argument("--no-alerts", required=False, action='store_true', default=False,
-                          help="If you use this flag it will set")
-
-        self.add_argument('--mode', required=False, help='Not used')
-
-        self.add_argument('--port', required=False, action='store', default=None, help='Not used')
-
-
-def run():
-    """
-
-    The main driver for the arguments package, this will call on the ArgParser class and parse our arguments for us
-
-    Returns:
-        ArgsParser (object): A parsed ArgParser object which will have the namespace for the program's options.
-
-    """
-
-    # Instantiate our argument parser
-    parser = ArgParser()
-
-    # Parse the arguments that were received on session start
-    args = parser.parse_args()
-
-    return args
-
-run()
+from argparse import ArgumentParser
+
+
+def super():
+    pass
+
+
+class ArgParser(ArgumentParser):
+
+    def __init__(self):
+        """
+
+        Instantiate an argument parser.
+
+        """
+        super().__init__(help="Use this option if you'd like the most output from the program into the console you "
+                               "can get")
+
+        self.add_argument("--no-alerts", required=False, action='store_true', default=False,
+                          help="If you use this flag it will set")
+
+        self.add_argument('--mode', required=False, help='Not used')
+
+        self.add_argument('--port', required=False, action='store', default=None, help='Not used')
+
+
+def run():
+    """
+
+    The main driver for the arguments package, this will call on the ArgParser class and parse our arguments for us
+
+    Returns:
+        ArgsParser (object): A parsed ArgParser object which will have the namespace for the program's options.
+
+    """
+
+    # Instantiate our argument parser
+    parser = ArgParser()
+
+    return parser.parse_args()
+
+run()
```

### Comparing `ip-reveal-1.2/pyproject.toml` & `ip_reveal-1.3.dev1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[tool.poetry]
-name = "ip-reveal"
-version = "1.2"
-description = "A GUI-based widget that checks your IP address periodically, sending notifications if it changes."
-authors = ["Taylor B. <tayjaybabee@gmail.com>"]
-license = "WTFPL"
-
-[tool.poetry.dependencies]
-humanize = "^3.1.0"
-inspy_logger = "2.1a14"
-inspyred_print = "^1.0"
-PySimpleGUI = "^4.30.0"
-PySimpleGUIQt = "^0.35.0"
-python = "^3.7"
-requests = "^2.25.0"
-simpleaudio = "^1.0.4"
-pypattyrn = "^1.2"
-inspyre-toolbox = "1.0a7"
-
-
-
-[tool.poetry.dev-dependencies]
-Sphinx = "^3.4.1"
-changelog-generator = "^0.2.4"
-pre-commit = "^2.15.0"
-recommonmark = "^0.7.1"
-
-[tool.poetry.scripts]
-ip-reveal = 'ip_reveal:main'
-
-[build-system]
-requires = ["poetry-core>=0.12"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "ip-reveal"
+version = "1.3-dev1"
+description = "A GUI-based widget that checks your IP address periodically, sending notifications if it changes."
+authors = ["Taylor B. <tayjaybabee@gmail.com>"]
+license = "WTFPL"
+
+[tool.poetry.dependencies]
+humanize = "^4.4.0"
+inspy_logger = "3.0.2-dev.1"
+inspyred_print = "^1.0"
+PySimpleGUI = "^4.30.0"
+PySimpleGUIQt = "^0.35.0"
+python = ">=3.9,<4.0"
+requests = "^2.25.0"
+simpleaudio = "^1.0.4"
+pypattyrn = "^1.2"
+inspyre-toolbox = "^1.3.2"
+
+
+
+[tool.poetry.dev-dependencies]
+Sphinx = "^3.4.1"
+changelog-generator = "^0.2.4"
+pre-commit = "^2.15.0"
+recommonmark = "^0.7.1"
+
+[tool.poetry.scripts]
+ip-reveal = 'ip_reveal:main'
+
+[build-system]
+requires = ["poetry-core>=0.12"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `ip-reveal-1.2/PKG-INFO` & `ip_reveal-1.3.dev1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ip-reveal
-Version: 1.2
+Version: 1.3.dev1
 Summary: A GUI-based widget that checks your IP address periodically, sending notifications if it changes.
 License: WTFPL
 Author: Taylor B.
 Author-email: tayjaybabee@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PySimpleGUI (>=4.30.0,<5.0.0)
 Requires-Dist: PySimpleGUIQt (>=0.35.0,<0.36.0)
-Requires-Dist: humanize (>=3.1.0,<4.0.0)
-Requires-Dist: inspy_logger (==2.1a14)
-Requires-Dist: inspyre-toolbox (==1.0a7)
+Requires-Dist: humanize (>=4.4.0,<5.0.0)
+Requires-Dist: inspy_logger (==3.0.2-dev.1)
+Requires-Dist: inspyre-toolbox (>=1.3.2,<2.0.0)
 Requires-Dist: inspyred_print (>=1.0,<2.0)
 Requires-Dist: pypattyrn (>=1.2,<2.0)
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: simpleaudio (>=1.0.4,<2.0.0)
```

