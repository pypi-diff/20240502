# Comparing `tmp/paifulogger-0.4.0.2.tar.gz` & `tmp/paifulogger-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paifulogger-0.4.0.2.tar", last modified: Sat Apr 20 12:41:46 2024, max compression
+gzip compressed data, was "paifulogger-0.4.1.tar", last modified: Thu May  2 16:07:24 2024, max compression
```

## Comparing `paifulogger-0.4.0.2.tar` & `paifulogger-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/PaifuLogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 12:41:46.000000 paifulogger-0.4.0.2/PaifuLogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.872611 paifulogger-0.4.0.2/paifulogger/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/paifulogger/localizations/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/localizations/zh_tw.json
--rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/paifu_dl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/paifulogger/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/Paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/get_paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/log_into_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/log_into_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/log_into_xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/
--rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/src/url_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/paifulogger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/pub_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/pub_tools/pub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:46.876611 paifulogger-0.4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-20 12:41:40.000000 paifulogger-0.4.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.263487 paifulogger-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 16:07:19.000000 paifulogger-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-02 16:07:24.263487 paifulogger-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.263487 paifulogger-0.4.1/PaifuLogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-02 16:07:24.000000 paifulogger-0.4.1/PaifuLogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-02 16:07:24.000000 paifulogger-0.4.1/PaifuLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:07:24.000000 paifulogger-0.4.1/PaifuLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 16:07:24.000000 paifulogger-0.4.1/PaifuLogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 16:07:24.000000 paifulogger-0.4.1/PaifuLogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 16:07:24.000000 paifulogger-0.4.1/PaifuLogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-02 16:07:19.000000 paifulogger-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.259487 paifulogger-0.4.1/paifulogger/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.259487 paifulogger-0.4.1/paifulogger/localizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/localizations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/localizations/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/localizations/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/localizations/zh_tw.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/paifu_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.263487 paifulogger-0.4.1/paifulogger/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/Paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/Paifu.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/get_paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/log_into_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/log_into_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/log_into_xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.263487 paifulogger-0.4.1/paifulogger/src/mjlog2mjai/
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-05-02 16:07:20.000000 paifulogger-0.4.1/paifulogger/src/mjlog2mjai/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-02 16:07:20.000000 paifulogger-0.4.1/paifulogger/src/mjlog2mjai/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/src/url_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 16:07:19.000000 paifulogger-0.4.1/paifulogger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.263487 paifulogger-0.4.1/pub_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 16:07:19.000000 paifulogger-0.4.1/pub_tools/pub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 16:07:19.000000 paifulogger-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:07:24.263487 paifulogger-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:24.263487 paifulogger-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:07:19.000000 paifulogger-0.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-02 16:07:19.000000 paifulogger-0.4.1/test/test.py
```

### Comparing `paifulogger-0.4.0.2/LICENSE` & `paifulogger-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/PKG-INFO` & `paifulogger-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.4.0.2
+Version: 0.4.1
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
         Copyright (c) 2023-2024 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -42,15 +42,15 @@
 
 Logging tenhou paifu into excel, csv or html file with some key information.
 
 ![Generated by DALL·E](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/paifulogger.png)
 
 If you like this project, please leave a star. It will be a great encouragement for me. And if you have any suggestions, please feel free to create an issue.
 
-[Downloads](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest) | [中文說明](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh.md) | [日本語](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_ja.md)
+[Downloads](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest) | [繁體中文](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh_TW.md) | [简体中文](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh.md) | [日本語](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_ja.md)
 
 ## Requirements
 
 * Python 3.10 or later
 
 Since CLI-0.3.8, the project is only compatible with Python 3.10 or later.
 For Python 3.9 or earlier users, please use [CLI-0.3.7.1](https://github.com/Jim137/Tenhou-Paifu-Logger/tree/CLI-0.3.7.1) which is the last version that supports Python 3.9 or earlier.
@@ -88,31 +88,31 @@
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard. And run by
 >>
 >> ```shell
 >> plog -l [language] -o [output directory] [paifu URLs]
 >> ```
 >> ```shell
->> paifulogger plog -l [language] -o [output directory] [paifu URLs]
+>> paifu plog -l [language] -o [output directory] [paifu URLs]
 >> ```
 
 2. Once `Please enter the URL of match:` appears, paste the URL and press Enter.\
 Note: In the latest version, you can input multiple URLs at once, separated by whatever you like. If you are lazy, you can just paste w/o anything.
 3. After `Match of {paifu name} has been recorded` appears, the paifu has been successfully logged.
 
 ### Inline
 
 You can manually log the paifu by the following code.
 
 ```python
-from paifulogger import get_paifu, localized_str, log_paifu, main_path
+from paifulogger import get_paifu, localized_str, log_paifu
 from paifulogger.log import _get_log_func
 
 url = "Your paifu URL"
-local_lang = localized_str("en", main_path) # Localization
+local_lang = localized_str("en") # Localization
 log_formats = _get_log_func(["csv", "html"]) # Log into csv and html file.
 output = "./" # Output directory
 mjai = False # Whether have output in mjai format
 
 # Log the paifu into the file.
 log_paifu(
     url,
@@ -139,14 +139,16 @@
   * [x] Traditional Chinese: zh_tw
   * [x] Simplified Chinese: zh
   * [x] Japanese (ChatGPT): ja
 * [x] Support config file. Placing `config.json` in the same directory as the execution enables local configuration. For global configuration, place it in the following directories:
   * Windows: `%localappdata%\Jim137\paifulogger\config.json`
   * macOS: `/Users/{UserName}/Library/Application Support/paifulogger/config.json`
   * Linux: `~/.local/share/paifulogger/config.json`
+* [x] Support logging from Tenhou client(*.mjlog). (-c, --from-client DIR_TO_MJLOG)\
+Note: Tpyically, the saved directory is `{Documents}/My Tenhou/log/` on Windows.
 
 ## Information logged
 
 * Game time
 * Placing
 * URL (for future use)
 * Rate before the game
```

### Comparing `paifulogger-0.4.0.2/PaifuLogger.egg-info/PKG-INFO` & `paifulogger-0.4.1/PaifuLogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.4.0.2
+Version: 0.4.1
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
         Copyright (c) 2023-2024 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -42,15 +42,15 @@
 
 Logging tenhou paifu into excel, csv or html file with some key information.
 
 ![Generated by DALL·E](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/paifulogger.png)
 
 If you like this project, please leave a star. It will be a great encouragement for me. And if you have any suggestions, please feel free to create an issue.
 
-[Downloads](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest) | [中文說明](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh.md) | [日本語](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_ja.md)
+[Downloads](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest) | [繁體中文](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh_TW.md) | [简体中文](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh.md) | [日本語](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_ja.md)
 
 ## Requirements
 
 * Python 3.10 or later
 
 Since CLI-0.3.8, the project is only compatible with Python 3.10 or later.
 For Python 3.9 or earlier users, please use [CLI-0.3.7.1](https://github.com/Jim137/Tenhou-Paifu-Logger/tree/CLI-0.3.7.1) which is the last version that supports Python 3.9 or earlier.
@@ -88,31 +88,31 @@
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard. And run by
 >>
 >> ```shell
 >> plog -l [language] -o [output directory] [paifu URLs]
 >> ```
 >> ```shell
->> paifulogger plog -l [language] -o [output directory] [paifu URLs]
+>> paifu plog -l [language] -o [output directory] [paifu URLs]
 >> ```
 
 2. Once `Please enter the URL of match:` appears, paste the URL and press Enter.\
 Note: In the latest version, you can input multiple URLs at once, separated by whatever you like. If you are lazy, you can just paste w/o anything.
 3. After `Match of {paifu name} has been recorded` appears, the paifu has been successfully logged.
 
 ### Inline
 
 You can manually log the paifu by the following code.
 
 ```python
-from paifulogger import get_paifu, localized_str, log_paifu, main_path
+from paifulogger import get_paifu, localized_str, log_paifu
 from paifulogger.log import _get_log_func
 
 url = "Your paifu URL"
-local_lang = localized_str("en", main_path) # Localization
+local_lang = localized_str("en") # Localization
 log_formats = _get_log_func(["csv", "html"]) # Log into csv and html file.
 output = "./" # Output directory
 mjai = False # Whether have output in mjai format
 
 # Log the paifu into the file.
 log_paifu(
     url,
@@ -139,14 +139,16 @@
   * [x] Traditional Chinese: zh_tw
   * [x] Simplified Chinese: zh
   * [x] Japanese (ChatGPT): ja
 * [x] Support config file. Placing `config.json` in the same directory as the execution enables local configuration. For global configuration, place it in the following directories:
   * Windows: `%localappdata%\Jim137\paifulogger\config.json`
   * macOS: `/Users/{UserName}/Library/Application Support/paifulogger/config.json`
   * Linux: `~/.local/share/paifulogger/config.json`
+* [x] Support logging from Tenhou client(*.mjlog). (-c, --from-client DIR_TO_MJLOG)\
+Note: Tpyically, the saved directory is `{Documents}/My Tenhou/log/` on Windows.
 
 ## Information logged
 
 * Game time
 * Placing
 * URL (for future use)
 * Rate before the game
```

### Comparing `paifulogger-0.4.0.2/PaifuLogger.egg-info/SOURCES.txt` & `paifulogger-0.4.1/PaifuLogger.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 paifulogger/paifu_dl.py
 paifulogger/version.py
 paifulogger/localizations/en.json
 paifulogger/localizations/ja.json
 paifulogger/localizations/zh.json
 paifulogger/localizations/zh_tw.json
 paifulogger/src/Paifu.py
+paifulogger/src/Paifu.pyi
 paifulogger/src/__init__.py
 paifulogger/src/config.py
 paifulogger/src/get_paifu.py
 paifulogger/src/i18n.py
+paifulogger/src/i18n.pyi
 paifulogger/src/log_into_csv.py
 paifulogger/src/log_into_html.py
 paifulogger/src/log_into_xlsx.py
 paifulogger/src/url_log.py
 paifulogger/src/mjlog2mjai/parse.py
 paifulogger/src/mjlog2mjai/test.py
 pub_tools/pub.py
```

### Comparing `paifulogger-0.4.0.2/README.md` & `paifulogger-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Logging tenhou paifu into excel, csv or html file with some key information.
 
 ![Generated by DALL·E](https://github.com/Jim137/Tenhou-Paifu-Logger/raw/master/READMEs/image/paifulogger.png)
 
 If you like this project, please leave a star. It will be a great encouragement for me. And if you have any suggestions, please feel free to create an issue.
 
-[Downloads](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest) | [中文說明](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh.md) | [日本語](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_ja.md)
+[Downloads](https://github.com/Jim137/Tenhou-Paifu-Logger/releases/latest) | [繁體中文](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh_TW.md) | [简体中文](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_zh.md) | [日本語](https://github.com/Jim137/Tenhou-Paifu-Logger/blob/master/READMEs/README_ja.md)
 
 ## Requirements
 
 * Python 3.10 or later
 
 Since CLI-0.3.8, the project is only compatible with Python 3.10 or later.
 For Python 3.9 or earlier users, please use [CLI-0.3.7.1](https://github.com/Jim137/Tenhou-Paifu-Logger/tree/CLI-0.3.7.1) which is the last version that supports Python 3.9 or earlier.
@@ -58,31 +58,31 @@
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard. And run by
 >>
 >> ```shell
 >> plog -l [language] -o [output directory] [paifu URLs]
 >> ```
 >> ```shell
->> paifulogger plog -l [language] -o [output directory] [paifu URLs]
+>> paifu plog -l [language] -o [output directory] [paifu URLs]
 >> ```
 
 2. Once `Please enter the URL of match:` appears, paste the URL and press Enter.\
 Note: In the latest version, you can input multiple URLs at once, separated by whatever you like. If you are lazy, you can just paste w/o anything.
 3. After `Match of {paifu name} has been recorded` appears, the paifu has been successfully logged.
 
 ### Inline
 
 You can manually log the paifu by the following code.
 
 ```python
-from paifulogger import get_paifu, localized_str, log_paifu, main_path
+from paifulogger import get_paifu, localized_str, log_paifu
 from paifulogger.log import _get_log_func
 
 url = "Your paifu URL"
-local_lang = localized_str("en", main_path) # Localization
+local_lang = localized_str("en") # Localization
 log_formats = _get_log_func(["csv", "html"]) # Log into csv and html file.
 output = "./" # Output directory
 mjai = False # Whether have output in mjai format
 
 # Log the paifu into the file.
 log_paifu(
     url,
@@ -109,14 +109,16 @@
   * [x] Traditional Chinese: zh_tw
   * [x] Simplified Chinese: zh
   * [x] Japanese (ChatGPT): ja
 * [x] Support config file. Placing `config.json` in the same directory as the execution enables local configuration. For global configuration, place it in the following directories:
   * Windows: `%localappdata%\Jim137\paifulogger\config.json`
   * macOS: `/Users/{UserName}/Library/Application Support/paifulogger/config.json`
   * Linux: `~/.local/share/paifulogger/config.json`
+* [x] Support logging from Tenhou client(*.mjlog). (-c, --from-client DIR_TO_MJLOG)\
+Note: Tpyically, the saved directory is `{Documents}/My Tenhou/log/` on Windows.
 
 ## Information logged
 
 * Game time
 * Placing
 * URL (for future use)
 * Rate before the game
```

### Comparing `paifulogger-0.4.0.2/paifulogger/localizations/en.json` & `paifulogger-0.4.1/paifulogger/localizations/en.json`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/paifulogger/localizations/ja.json` & `paifulogger-0.4.1/paifulogger/localizations/ja.json`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/paifulogger/localizations/zh.json` & `paifulogger-0.4.1/paifulogger/localizations/zh.json`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/paifulogger/localizations/zh_tw.json` & `paifulogger-0.4.1/paifulogger/localizations/zh_tw.json`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/paifulogger/log.py` & `paifulogger-0.4.1/paifulogger/log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,182 +1,243 @@
 import argparse
 import json
-import urllib.request
 import os
 import re
 import sys
+import urllib.request
 import warnings
 from typing import Callable
 
-from pandas import HDFStore, DataFrame
+from pandas import DataFrame, HDFStore
 
+from . import __version__, main_path
 from .src.config import config_path
-from .src.get_paifu import get_paifu
-from .src.i18n import localized_str, LocalStr
+from .src.get_paifu import get_paifu, get_paifu_from_client_log, save_mjai
+from .src.i18n import LocalStr, localized_str
 from .src.log_into_csv import log_into_csv
-from .src.log_into_xlsx import log_into_xlsx
 from .src.log_into_html import log_into_html
-from .src.url_log import url_log, check_duplicate
-
+from .src.log_into_xlsx import log_into_xlsx
+from .src.Paifu import Paifu
+from .src.url_log import check_duplicate, url_log
 
-url_reg = r"https?://tenhou\.net/\d/\?log=\d{10}gm-\w{4}-\w{4}-\w{8}&tw=\d"
+REG_URL = r"https?://tenhou\.net/\d/\?log=\d{10}gm-\w{4}-\w{4}-\w{8}&tw=\d"
 avaiable_formats = ["xlsx", "html", "csv"]
 
 
 def remove_old_paifu(paifu_str: str, formats: list[str], output: str) -> None:
     """
     Remove old paifu files.
 
-    Args:
-        paifu_str: str
-            The name of the paifu file.
-        formats: list
-            The formats of the paifu file.
-        output: str
-            The output directory.
-
-    Returns:
-        None
-
-    ---
-
-    Examples:
-        >>> remove_old_paifu("paifu", ["xlsx", "html", "csv"], "./")
-        paifu.xlsx has been removed.
-        paifu.html has been removed.
-        paifu.csv has been removed.
+    Parameters
+    ----------
+    paifu_str : str
+        The name of the paifu file.
+    formats : list
+        The formats of the paifu file.
+    output : str
+        The output directory.
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> remove_old_paifu("paifu", ["xlsx", "html", "csv"], "./")
+    paifu.xlsx has been removed.
+    paifu.html has been removed.
+    paifu.csv has been removed.
     """
 
     for format in formats:
         if os.path.exists(f"{output}/{paifu_str}.{format}"):
             os.remove(f"{output}/{paifu_str}.{format}")
             print(f"{paifu_str}.{format} has been removed.")
     return None
 
 
 def _get_lang(lang: str | None = None) -> LocalStr:
     """
     Get the localized string.
 
     If not given, use English.
+
+    Parameters
+    ----------
+    lang : str
+        The language of the program.
+
+    Returns
+    -------
+    LocalStr
+        The localized string.
     """
 
-    if lang:
-        _lang = lang
-    else:
-        _lang = "en"
-    main_path = os.path.dirname(os.path.abspath(__file__))
-    local_lang = localized_str(_lang, main_path)
-    return local_lang
+    return localized_str(lang, main_path) if lang else localized_str("en", main_path)
 
 
 def _get_output(output: str = "./") -> str:
     """
     Get output directory from args.output.
 
     If not given, use current directory "./".
+
+    Parameters
+    ----------
+    output : str
+        The output directory.
+
+    Returns
+    -------
+    str
+        The absolute path of the output directory.
     """
 
-    if output:
-        _output = os.path.abspath(output)
-    else:
-        _output = os.path.abspath("./")
-    return _output
+    return os.path.abspath(output) if output else os.path.abspath("./")
 
 
 def _get_urls(
     url: list[str] | None = None,
-    local_lang: LocalStr = localized_str(
-        "en", os.path.dirname(os.path.abspath(__file__))
-    ),
+    local_lang: LocalStr = localized_str("en"),
     output: str = os.path.abspath("./"),
     remake: bool = False,
 ) -> list[str]:
     """
     Get urls from input or url.
 
     If remake, get urls from url_log.h5
     Else if not given url, get urls from input.
 
-    Note:
-        `re.findall(url_reg, _url)` will return a list of urls that match the regular expression.
+    Parameters
+    ----------
+    url : list[str]
+        The urls of the paifu files.
+    local_lang : LocalStr
+        The localized string.
+    output : str
+        The output directory.
+    remake : bool
+        Remake the log file from url_log.h5.
+
+    Returns
+    -------
+    list[str]
+        The list of urls.
+
+    Note
+    ----
+    `re.findall(REG_URL, _url)` will return a list of urls that match the regular expression.
     """
 
     urls = []
     if remake:
         with HDFStore(f"{output}/{local_lang.paifu}/url_log.h5") as store:
-            ############################################################
+            # ===============================================================
             # Special case: if "url" not in store, add it.
             # It will be deprecated in the future.
             if "url" not in store:
                 store["url"] = DataFrame(columns=["url"])
                 warnings.warn(
-                    """The url_log.h5 you used is deprecated. 
+                    """The url_log.h5 you used is deprecated.
                     You have to manually copy all urls and delete url_log.h5,
-                    then run and paste the urls to the program. 
+                    then run and paste the urls to the program.
                     The new url_log.h5 will be automatically created.
                     """,
                     DeprecationWarning,
                 )
-            ############################################################
+            # ===============================================================
             urlstore = store["url"]["url"].values
             for _url in urlstore:
-                if not re.match(url_reg, _url):
+                if not re.match(REG_URL, _url):
                     urls.append("https://" + _url)
                     continue
                 urls.append(_url)
     elif not url:
-        for _url in re.findall(url_reg, input(local_lang.hint_input)):
+        for _url in re.findall(REG_URL, input(local_lang.hint_input)):
             urls.append(_url)
     else:
         for _url in url:
-            urls.extend(re.findall(url_reg, _url))
+            urls.extend(re.findall(REG_URL, _url))
     return urls
 
 
 def _get_formats(format: list[str] | None = None) -> list:
     """
     Get formats from `args.format`.
 
     If not given, return ["csv"].
+
+    Parameters
+    ----------
+    format : list
+        The formats of the output file.
+
+    Returns
+    -------
+    list
+        The formats of the output file.
     """
 
-    if format:
-        formats = format
-    else:
-        formats = ["csv"]
-    return formats
+    return format if format else ["csv"]
 
 
 def _remake_log(
     local_lang: LocalStr, output: str, formats: list[str], all_formats: bool = False
 ) -> None:
     """
     Remake the log file from url_log.h5 (past logging log), and remove old paifu files.
+
+    Parameters
+    ----------
+    local_lang : LocalStr
+        The localized string.
+    output : str
+        The output directory to remove.
+    formats : list
+        The formats of the output file.
+    all_formats : bool
+        Remove all formats.
     """
 
     paifu_str3 = local_lang.paifu + "/" + local_lang.sanma + local_lang.paifu
     paifu_str4 = local_lang.paifu + "/" + local_lang.yonma + local_lang.paifu
     try:
         if all_formats:
             remove_old_paifu(paifu_str3, avaiable_formats, output)
-            remove_old_paifu(paifu_str4, avaiable_formats, output)
         else:
             remove_old_paifu(paifu_str3, formats, output)
+    except OSError:
+        pass
+    try:
+        if all_formats:
+            remove_old_paifu(paifu_str4, avaiable_formats, output)
+        else:
             remove_old_paifu(paifu_str4, formats, output)
     except OSError:
         pass
     return None
 
 
 def _get_log_func(formats: list[str], all_formats: bool = False) -> list[Callable]:
     """
     Parse the formats and return the corresponding log functions.
 
     If `all_formats`, return all log functions.
+
+    Parameters
+    ----------
+    formats : list
+        The formats of the output file.
+    all_formats : bool
+        Output all formats.
+
+    Returns
+    -------
+    list
+        The list of log functions.
     """
 
     assert formats, "No format is given."
 
     if all_formats:
         log_formats = [
             log_into_xlsx,
@@ -190,55 +251,117 @@
         if "html" in formats:
             log_formats.append(log_into_html)
         if "csv" in formats:
             log_formats.append(log_into_csv)
     return log_formats
 
 
+def log_paifu_from_local(
+    paifus: list[Paifu],
+    *,
+    log_formats: list[Callable] = [log_into_csv],
+    local_lang: LocalStr = localized_str("en", main_path),
+    output: str = os.path.abspath("./"),
+    ignore_duplicated: bool = False,
+    mjai: bool = False,
+):
+    """
+    Log paifu files from local.
+
+    Parameters
+    ----------
+    paifus : list[Paifu]
+        The list of paifu files.
+    log_formats : list
+        The log functions.
+    local_lang : LocalStr
+        The localized string.
+    output : str
+        The output directory.
+    ignore_duplicated : bool
+        Ignore duplicated urls.
+    mjai : bool
+        Output MJAI format paifu.
+
+    Returns
+    -------
+    int
+        The return code.
+    """
+
+    retcode = 0
+    for paifu in paifus:
+        try:
+            if mjai:
+                save_mjai(paifu, output, paifu.name, local_lang)
+            if check_duplicate(paifu.url, local_lang, output) and not ignore_duplicated:
+                print(local_lang.hint_duplicate, paifu.url)
+                continue
+            for log_into_format in log_formats:
+                log_into_format(paifu, local_lang, output)
+            url_log(paifu.url, local_lang, output)
+        except OSError:
+            print(local_lang.hint_url, paifu.url)
+            retcode = 1
+        except ValueError:
+            print(local_lang.hint_tw, paifu.url)
+            retcode = 1
+        except KeyError:
+            print(
+                """Please remake the log file by `plog -f [format] -l [lang] -o [output] -r` first,
+                  or `python -m paifulogger plog -f [format] -l [lang] -o [output] -r` manually."""
+            )
+            return 1
+    return retcode
+
+
 def log_paifu(
     *urls: list[str] | str,
     log_formats: list[Callable] = [log_into_csv],
-    local_lang: LocalStr = LocalStr("en", os.path.dirname(os.path.abspath(__file__))),
+    local_lang: LocalStr = localized_str("en", main_path),
     output: str = os.path.abspath("./"),
     remake: bool = False,
     ignore_duplicated: bool = False,
     mjai: bool = False,
 ) -> int:
     """
     Log paifu files.
 
-    Args:
-        urls: list[str]
-            The urls of the paifu files.
-        log_formats: list
-            The list of log functions.
-        local_lang: LocalStr
-            The localized string.
-        output: str
-            The output directory.
-        remake: bool
-            Remake the log file from url_log.h5.
-        ignore_duplicated: bool
-            Ignore duplicated urls.
-        mjai: bool
-            Output MJAI format paifu.
-
-    Returns:
-        int
+    Parameters
+    ----------
+    urls : list
+        The urls of the paifu files.
+    log_formats : list
+        The log functions.
+    local_lang : LocalStr
+        The localized string.
+    output : str
+        The output directory.
+    remake : bool
+        Remake the log file from url_log.h5.
+    ignore_duplicated : bool
+        Ignore duplicated urls.
+    mjai : bool
+        Output MJAI format paifu.
+
+    Returns
+    -------
+    int
+        The return code.
     """
 
-    retCode = 0
+    retcode = 0
     _urls: list[str] = []
     for url in urls:
         if isinstance(url, list):
             _urls.extend(url)
         else:
             _urls.append(url)
     for url in _urls:
-        if not re.match(url_reg, url):
+        if not re.match(REG_URL, url):
             print(local_lang.hint_url, url)
             continue
         if remake:
             pass
         elif check_duplicate(url, local_lang, output) and not ignore_duplicated:
             print(local_lang.hint_duplicate, url)
             continue
@@ -248,52 +371,71 @@
                 log_into_format(paifu, local_lang, output)
             if remake:
                 pass
             else:
                 url_log(url, local_lang, output)
         except urllib.error.URLError:
             print(local_lang.hint_url, url)
-            retCode = 1
+            retcode = 1
         except OSError:
             print(local_lang.hint_url, url)
-            retCode = 1
+            retcode = 1
         except ValueError:
             print(local_lang.hint_tw, url)
-            retCode = 1
+            retcode = 1
         except KeyError:
             print(
                 """Please remake the log file by `plog -f [format] -l [lang] -o [output] -r`,
-                  or `python -m plog -f [format] -l [lang] -o [output] -r` manually."""
+                  or `python -m paifulogger plog -f [format] -l [lang] -o [output] -r` manually."""
             )
             return 1
-    return retCode
+    return retcode
 
 
 def log(args: argparse.Namespace) -> int:
     """
     Parse the arguments and log paifu files.
-    """
 
-    # get version and exit
-    if args.version:
-        from .version import __version__
-
-        print("Tenhou-Paifu-Logger", __version__)
-        return 0
+    Parameters
+    ----------
+    args : argparse.Namespace
+        The arguments from the command line.
+
+    Returns
+    -------
+    int
+        The return code.
+    """
 
     local_lang = _get_lang(args.lang)
     output = _get_output(args.output)
-    urls = _get_urls(args.url, local_lang, output, args.remake)
     formats = _get_formats(args.format)
 
     # if remake, remove old files
     if args.remake:
         _remake_log(local_lang, output, formats, args.all_formats)
 
     log_formats = _get_log_func(formats, args.all_formats)
+
+    if args.from_client:
+        paifus = get_paifu_from_client_log(args.from_client)
+        if not paifus:
+            print("No paifu files found.")
+            return 0
+        print(f"Found {len(paifus)} paifu files.")
+        return log_paifu_from_local(
+            paifus,
+            log_formats=log_formats,
+            local_lang=local_lang,
+            output=output,
+            ignore_duplicated=args.ignore_duplicated,
+            mjai=args.mjai,
+        )
+
+    urls = _get_urls(args.url, local_lang, output, args.remake)
     return log_paifu(
         urls,
         log_formats=log_formats,
         local_lang=local_lang,
         output=output,
         remake=args.remake,
         ignore_duplicated=args.ignore_duplicated,
@@ -303,35 +445,40 @@
 
 def log_parser(
     config_path: str | None = None, parser: argparse.ArgumentParser | None = None
 ) -> argparse.Namespace:
     """
     Parse the arguments from the command line.
 
-    Args:
-        config_path: str
-            The path of the config file.
-
-    Returns:
-        argparse.Namespace
+    Parameters
+    ----------
+    config_path : str
+        The path of the config file.
+    parser : argparse.ArgumentParser
+        The argument parser.
+
+    Returns
+    -------
+    argparse.Namespace
+        The arguments from the command line.
     """
 
     config = {}
     if config_path and os.path.exists(f"{config_path}/config.json"):
         with open(f"{config_path}/config.json", "r") as f:
             config = json.load(f)
 
     if parser is None:
-        parser = argparse.ArgumentParser(description="Paifu Logger")
+        parser = argparse.ArgumentParser(description="Paifu Logger", prog="PaifuLogger")
     parser.add_argument("url", nargs="*", help="URL of the match.")
     parser.add_argument(
         "-l",
         "--lang",
         type=str,
-        help="""Language of the program and output files. Default is English. 
+        help="""Language of the program and output files. Default is English.
         Available languages: English(en), 繁體中文(zh_tw), 简体中文(zh), 日本語(ja).""",
         default=config.get("lang", None),
     )
     parser.add_argument(
         "-f",
         "--format",
         action="append",
@@ -347,37 +494,46 @@
         help="Output all formats.",
         default=config.get("all_formats", False),
     )
     parser.add_argument(
         "-r",
         "--remake",
         action="store_true",
-        help="""Remake the log file from url_log.h5 (past logging log). 
-        Use this when the program is updated, changing format or language of the log file, or the log file is missing. 
+        help="""Remake the log file from url_log.h5 (past logging log).
+        Use this when the program is updated, changing format or language of the log file, or the log file is missing.
         Note that this will overwrite the log file.""",
     )
     parser.add_argument(
         "-o",
         "--output",
         type=str,
         help="Output directory. Default is './'.",
         default=config.get("output", None),
     )
     parser.add_argument(
         "-v",
         "--version",
-        action="store_true",
-        help="Show version of the program. If this is used, all other arguments will be ignored and the program will be closed.",
+        action="version",
+        help="""Show version of the program.
+        If this is used, all other arguments will be ignored and the program will be closed.""",
+        version=f"%(prog)s {__version__}",
     )
     parser.add_argument(
         "--mjai",
         action="store_true",
         help="Output MJAI format paifu.",
         default=config.get("mjai", False),
     )
+    parser.add_argument(
+        "-c",
+        "--from-client",
+        nargs="+",
+        help="Log client saved paifu (*.mjlog) from given directory.",
+        type=str,
+    )
     # Args for Debugging
     parser.add_argument(
         "--ignore-duplicated",
         action="store_true",
         help=argparse.SUPPRESS,
         default=config.get("ignore_duplicated", False),
     )
```

### Comparing `paifulogger-0.4.0.2/paifulogger/src/Paifu.py` & `paifulogger-0.4.1/paifulogger/src/Paifu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import re
 import xml.etree.ElementTree as ET
+from datetime import datetime
 
 
 class Paifu:
     def __init__(self, url: str, root: ET.Element):
         self.url = url
+        self.name = url.split("=")[1] + "=" + url.split("=")[2]
+        self.time = datetime.strptime(re.findall(r"\d{10}", self.url)[0], "%Y%m%d%H")
         self.ban = int(url[-1])
         self.root = root
 
         if gtype := root[1].get("type"):
             self.go_type = int(gtype)
         if owari := root[-1].get("owari"):
             self.owari = owari.split(",")
@@ -19,17 +23,16 @@
         self.plc = self.get_place(self.ban)
         self.rate_change = self.get_rate_change()
 
     def go_type_distinguish(self):
         """
         Distinguish the type of the game. And set the go_str and player_num.
 
-        ---
-
-        Examples:
+        Examples
+        --------
             三鳳南喰赤速 (go_type = 127) -> go_str = '三南喰赤速', player_num = 3
 
         """
 
         self.go_str = ""
         if self.go_type & 1:
             # PVP
@@ -61,25 +64,33 @@
         if not self.go_type & 2:
             self.go_str += "赤"
 
         if self.go_type & 64:
             self.go_str += "速"
 
     def _rounds(self):
+        """
+        Get rounds of the game.
+        """
         self.rounds = [[] for _ in range(self.get_round_num() + 1)]
         round_idx = -1
         for el in self.root:
             # Each element has tag: str, attrib: dict, text, tail attributes
             if el.tag == "INIT":
                 round_idx += 1
             self.rounds[round_idx].append(el)
 
-    def get_place(self, ban):
+    def get_place(self, ban) -> int:
         """
         Return the placing and rate before match
+
+        Parameters
+        ----------
+        ban: int
+            The player's seat number.
         """
         o0, s0, o1, s1, o2, s2, o3, s3 = self.owari
 
         if self.player_num == 4:
             sp = [float(s0), float(s1), float(s2), float(s3)]
             placing = [1, 1, 1, 1]
             for i in range(4):
@@ -91,51 +102,85 @@
             placing = [1, 1, 1]
             for i in range(3):
                 for j in range(3):
                     if sp[i] < sp[j]:
                         placing[i] += 1
         return placing[ban]
 
-    def get_rate_change(self):
+    def get_rate_change(self) -> float:
         """
         Return the rate change after match.
 
-        Note: Since the rate change has a correction of number of played games. We assumed that player has played over 400 games,
-        which the correction is fixed to 0.2.
+        Returns
+        -------
+        float
+            The rate change after match.
+
+        Note
+        ----
+        Since the rate change has a correction of number of played games.
+        We assumed that player has played over 400 games, which the correction is fixed to 0.2.
         """
 
         if self.player_num == 4:
             dr_result = (30, 10, -10, -30)
             corr = (sum([float(r) for r in self.r]) / 4 - float(self.r[self.ban])) / 40
             return 0.2 * (dr_result[self.plc - 1] + corr)
         else:
-            dr_result = (30, 0, -30)
+            dr_result = (30, 0, -30, 0)
             corr = (sum([float(r) for r in self.r]) / 3 - float(self.r[self.ban])) / 40
+            if self.plc == 4:
+                assert False, "Sanma has no 4th place."
             return 0.2 * (dr_result[self.plc - 1] + corr)
 
     def get_round_num(self) -> int:
         """
-        Return the total number of rounds
+        Return the total number of rounds.
+
+        Returns
+        -------
+        int
+            The total number of rounds
         """
         return len(self.root.findall("INIT"))
 
     def get_deal_in_num(self, ban) -> int:
         """
-        Return the number of deal-in
+        Return number of deal-ins.
+
+        Parameters
+        ----------
+        ban: int
+            The player's seat number.
+
+        Returns
+        -------
+        int
+            The number of deal-in
         """
         agaris = self.root.findall("AGARI")
         count = 0
         for agari in agaris:
             if agari.get("fromWho") == str(ban) and agari.get("who") != str(ban):
                 count += 1
         return count
 
     def get_win_num(self, ban) -> int:
         """
-        Return the number of win
+        Return number of wins.
+
+        Parameters
+        ----------
+        ban: int
+            The player's seat number.
+
+        Returns
+        -------
+        int
+            The number of wins
         """
         agaris = self.root.findall("AGARI")
         count = 0
         for agari in agaris:
             if agari.get("who") == str(ban):
                 count += 1
         return count
```

### Comparing `paifulogger-0.4.0.2/paifulogger/src/i18n.py` & `paifulogger-0.4.1/paifulogger/src/i18n.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 
+from .. import main_path
+
 
 class LocalStr:
     def __init__(self, lang: str = "en", main_path: str = "./"):
         self.lang = lang
         self.main_path = main_path
         pass
 
@@ -18,18 +20,35 @@
         "If the attribute is not loaded, return the value in English."
 
         with open(f"{self.main_path}/localizations/en.json") as f:
             data = json.load(f)
         return data[name]
 
 
-def localized_str(lang: str, main_path: str) -> LocalStr:
+def localized_str(lang: str, main_path: str = main_path) -> LocalStr:
+    """
+    Get the localized string.
+
+    Parameters
+    ----------
+    lang: str
+        The language.
+    main_path: str
+        The main path.
+
+    Returns
+    -------
+    LocalStr
+        The localized string.
+    """
+
     localized = LocalStr(lang, main_path)
     try:
         with open(f"{main_path}/localizations/{lang}.json", encoding="utf-8") as f:
             data = json.load(f)
             localized.load_data(data)
     except FileNotFoundError:
+        print(f"Cannot find {lang}.json. Using English instead.")
         with open(f"{main_path}/localizations/en.json") as f:
             data = json.load(f)
             localized.load_data(data)
     return localized
```

### Comparing `paifulogger-0.4.0.2/paifulogger/src/log_into_csv.py` & `paifulogger-0.4.1/paifulogger/src/log_into_csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import csv
-import re
 import os.path
-from datetime import datetime
+import re
 
 import pandas as pd
 
 from .i18n import LocalStr
 from .Paifu import Paifu
 
 
 def log_into_csv(paifu: Paifu, local_lang: LocalStr, output: str):
+    """
+    Log the paifu data into csv file.
+
+    Parameters
+    ----------
+    paifu: Paifu
+        The paifu data.
+    local_lang: LocalStr
+        The localized string.
+    output: str
+        The output directory.
+    """
+
     if paifu.player_num == 3:
         paifu_str = local_lang.sanma + local_lang.paifu
     else:
         paifu_str = local_lang.yonma + local_lang.paifu
     path = f"{output}/{local_lang.paifu}/{paifu_str}.csv"
     if os.path.isfile(path):
         csvfile = open(path, "a+", encoding="utf-8")
@@ -42,15 +54,15 @@
         except pd.errors.EmptyDataError:
             # If the csv file is empty, create a new DataFrame
             df = pd.DataFrame(columns=["id", "date", "plc", "paifu", "preR", "r_change", "round_num", "win", "deal_in"])
         # Append new paifu data to the csv file
         writer.writerow(
             [
                 df.shape[0],
-                datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H"),
+                paifu.time,
                 paifu.get_place(paifu.ban),
                 paifu.url,
                 float(paifu.r[paifu.ban]),
                 paifu.rate_change,
                 paifu.get_round_num(),
                 paifu.get_win_num(paifu.ban),
                 paifu.get_deal_in_num(paifu.ban),
```

### Comparing `paifulogger-0.4.0.2/paifulogger/src/log_into_html.py` & `paifulogger-0.4.1/paifulogger/src/log_into_html.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import io
 import re
-from datetime import datetime
 
 import pandas as pd
 
 from .i18n import LocalStr
 from .Paifu import Paifu
 
 
@@ -23,17 +22,37 @@
             self.replay = ""
         else:
             self.replay = html_str.split("</body>")[1].split("</html>")[0]
         self.end = "</body></html>"
         pass
 
     def __repr__(self) -> str:
+        """
+        Return the html string.
+
+        Returns
+        -------
+        str
+            The html string.
+        """
+
         return self.logged + self.new_log + self.end_table + self.replay + self.end
 
     def create_html(self, paifu_str, local_lang: LocalStr) -> None:
+        """
+        Create the html file.
+
+        Parameters
+        ----------
+        paifu_str: str
+            The paifu string.
+        local_lang: LocalStr
+            The localized string.
+        """
+
         self.logged += f"""<!DOCTYPE html>
         <html lang={local_lang.lang}>
         <head>
             <meta charset="utf-8">
             <title>{paifu_str}</title>
             <style>
                 table {{
@@ -76,32 +95,50 @@
                         <th>{local_lang.deal_in}</th>
                     </tr>
                 </thead>
                 <tbody>
         """
 
     def log_into_table(self, paifu: Paifu) -> None:
-        time_str = datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H")
+        """
+        Log the paifu data into the html table.
+        
+        Parameters
+        ----------
+        paifu: Paifu
+            The paifu data.
+        """
+
         self.new_log += f"""
                     <tr>
-                        <td>{time_str}</td>
+                        <td>{paifu.time}</td>
                         <td>{paifu.get_place(paifu.ban)}</td>
                         <td><a href="{paifu.url}">{paifu.url}</a></td>
                         <td><textarea id="persisted-text"></textarea></td>
                         <td>{paifu.r[paifu.ban]}</td>
                         <td>{paifu.rate_change:.03f}</td>
                         <td>{paifu.get_round_num()}</td>
                         <td>{paifu.get_win_num(paifu.ban)}</td>
                         <td>{paifu.get_deal_in_num(paifu.ban)}</td>
                     </tr>
         """
 
     def _retrieve(self, local_lang: LocalStr) -> tuple[int, float, float, float]:
         """
         Retrieve the data from the html table.
+
+        Parameters
+        ----------
+        local_lang: LocalStr
+            The localized string.
+
+        Returns
+        -------
+        tuple[int, float, float, float]
+            The number of logged data, the average place, the win rate, and the deal-in rate.
         """
 
         pseudo_html = (
             self.logged
             + self.new_log
             + """
                 </tbody>
@@ -116,26 +153,48 @@
         win_rate = df[f"{local_lang.win}"].sum() / df[f"{local_lang.round_num}"].sum()
         deal_in_rate = (
             df[f"{local_lang.deal_in}"].sum() / df[f"{local_lang.round_num}"].sum()
         )
         return logged_num, avg_plc, win_rate, deal_in_rate
 
     def end_of_table(self, local_lang: LocalStr) -> None:
+        """
+        The end of the table.
+
+        Parameters
+        ----------
+        local_lang: LocalStr
+            The localized string.
+        """
+
         logged_num, avg_plc, win_rate, deal_in_rate = self._retrieve(local_lang)
         self.end_table += f"""
-                </tbody>  
+                </tbody>
             </table>
             <p>{local_lang.log_num} = {logged_num}</p>
             <p>{local_lang.avg_plc} = {avg_plc:.2}</p>
             <p>{local_lang.win_rate} = {win_rate:.3%}</p>
             <p>{local_lang.deal_in_rate} = {deal_in_rate:.3%}</p>
         """
 
 
 def log_into_html(paifu: Paifu, local_lang: LocalStr, output: str):
+    """
+    Log the paifu data into html file.
+
+    Parameters
+    ----------
+    paifu: Paifu
+        The paifu data.
+    local_lang: LocalStr
+        The localized string.
+    output: str
+        The output directory.
+    """
+
     if paifu.player_num == 3:
         paifu_str = local_lang.sanma + local_lang.paifu
     else:
         paifu_str = local_lang.yonma + local_lang.paifu
     path = f"{output}/{local_lang.paifu}/{paifu_str}.html"
     try:
         with open(path, "r", encoding="utf-8") as f:
```

### Comparing `paifulogger-0.4.0.2/paifulogger/src/log_into_xlsx.py` & `paifulogger-0.4.1/paifulogger/src/log_into_xlsx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import re
-from datetime import datetime
 from typing import cast
 
 import openpyxl as xl
 from openpyxl.worksheet.worksheet import Worksheet
 
 from .i18n import LocalStr
 from .Paifu import Paifu
 
 
 def log_into_xlsx(paifu: Paifu, local_lang: LocalStr, output: str):
+    """
+    Log the paifu data into xlsx file.
+
+    Parameters
+    ----------
+    paifu: Paifu
+        The paifu data.
+    local_lang: LocalStr
+        The localized string.
+    output: str
+        The output directory.
+    """
+
     try:
         if paifu.player_num == 3:
             paifu_str = local_lang.sanma + local_lang.paifu
         else:
             paifu_str = local_lang.yonma + local_lang.paifu
         path = f"{output}/{local_lang.paifu}/{paifu_str}.xlsx"
         wb = xl.load_workbook(path)
@@ -42,15 +54,15 @@
         # set column width
         sheet.column_dimensions["A"].width = 20
         sheet.column_dimensions["C"].width = 71
         sheet.column_dimensions["E"].width = local_lang.excelE
     # Append new paifu data to the sheet
     sheet.append(
         [
-            datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H"),
+            paifu.time,
             paifu.get_place(paifu.ban),
             paifu.url,
             "",
             float(paifu.r[paifu.ban]),
             paifu.rate_change,
             paifu.get_round_num(),
             paifu.get_win_num(paifu.ban),
```

### Comparing `paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/parse.py` & `paifulogger-0.4.1/paifulogger/src/mjlog2mjai/parse.py`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/paifulogger/src/mjlog2mjai/test.py` & `paifulogger-0.4.1/paifulogger/src/mjlog2mjai/test.py`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/paifulogger/src/url_log.py` & `paifulogger-0.4.1/paifulogger/src/url_log.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,26 +20,57 @@
 
 import pandas as pd
 
 from .i18n import LocalStr
 
 
 def check_duplicate(url, local_lang: LocalStr, output: str) -> bool:
+    """
+    Check if the given URL is already in the log file.
+
+    Parameters
+    ----------
+    url: str
+        The URL to check.
+    local_lang: LocalStr
+        The language settings.
+    output: str
+        The output directory.
+
+    Returns
+    -------
+    bool
+        True if the URL is duplicated, False otherwise.
+    """
+
     path = f"{output}/{local_lang.paifu}"
     if not os.path.isdir(path):
         os.makedirs(path)
     store = pd.HDFStore(f"{path}/url_log.h5")
     if "url" not in store:
         store["url"] = pd.DataFrame(columns=["url"])
     duplicated = url.split("//")[1] in store["url"]["url"].values
     store.close()
     return duplicated
 
 
 def url_log(url, local_lang: LocalStr, output: str) -> None:
+    """
+    Logs the given URL to the log file.
+
+    Parameters
+    ----------
+    url: str
+        The URL to log.
+    local_lang: LocalStr
+        The language settings.
+    output: str
+        The output directory.
+    """
+
     path = f"{output}/{local_lang.paifu}"
     if not os.path.isdir(path):
         os.makedirs(path)
     store = pd.HDFStore(f"{path}/url_log.h5")
     if "url" not in store:
         store["url"] = pd.DataFrame(columns=["url"])
     if url.split("//")[1] in store["url"]["url"].values:
```

### Comparing `paifulogger-0.4.0.2/pub_tools/pub.py` & `paifulogger-0.4.1/pub_tools/pub.py`

 * *Files identical despite different names*

### Comparing `paifulogger-0.4.0.2/pyproject.toml` & `paifulogger-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PaifuLogger"
-version = "0.4.0.2"
+version = "0.4.1"
 description = "Logging tenhou paifu into excel or html file with some key information."
 readme = "README.md"
 authors = [{ name = "Jim137", email = "jim@mail.jim137.eu.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
```

### Comparing `paifulogger-0.4.0.2/test/test.py` & `paifulogger-0.4.1/test/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,41 +3,38 @@
 import sys
 import unittest
 
 sys.path.append(os.getcwd())
 
 from paifulogger import log, paifu_dl
 
-
 ATTR = [
     "url",
     "lang",
     "format",
     "all-formats",
     "remake",
     "output",
-    "version",
     "mjai",
     "ignore-duplicated",
+    "from-client",
 ]
 
 
 class Test(unittest.TestCase):
     def test_0(self):
-        parser = argparse.ArgumentParser()
-        args = parser.parse_args()
-
-        for attr in ATTR:
-            setattr(args, attr.replace("-", "_"), None)
-
-        args.version = True
-
-        self.assertEqual(log(args), 0)
+        """
+        Version test
+        """
+        self.assertEqual(os.system("python3 -m paifulogger -v"), 0)
 
     def test_1(self):
+        """
+        Normal test
+        """
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.url = [
@@ -52,14 +49,17 @@
         args.all_formats = True
         args.ignore_duplicated = True
         args.output = "./test/"
 
         self.assertEqual(log(args), 0)
 
     def test_2(self):
+        """
+        i18n test
+        """
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.url = [
@@ -75,35 +75,56 @@
         args.ignore_duplicated = True
         args.output = "./test/"
         args.lang = "zh_tw"
 
         self.assertEqual(log(args), 0)
 
     def test_3(self):
+        """
+        pdl test
+        """
         urls = [
             # yonma tests
             "https://tenhou.net/3/?log=2022052501gm-00c1-0000-f71e7910&tw=1",
             "https://tenhou.net/0/?log=2023051123gm-0001-0000-b3720f99&tw=2",
             "http://tenhou.net/0/?log=2023051216gm-0001-0000-5fd022cc&tw=1",
             # sanma tests
             "https://tenhou.net/0/?log=2023050200gm-0099-0000-50c65fbf&tw=2",
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
 
         self.assertEqual(paifu_dl(urls, output="./test/"), 0)
 
     def test_4(self):
+        """
+        Remake test
+        """
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.all_formats = True
         args.output = "./test/"
         args.remake = True
 
         self.assertEqual(log(args), 0)
 
+    def test_5(self):
+        """
+        Log from client test
+        """
+        parser = argparse.ArgumentParser()
+        args = parser.parse_args()
+
+        for attr in ATTR:
+            setattr(args, attr.replace("-", "_"), None)
+
+        args.from_client = "./test/test_data/"
+        args.ignore_duplicated = True
+
+        self.assertEqual(log(args), 0)
+
 
 if __name__ == "__main__":
     unittest.main()
```

