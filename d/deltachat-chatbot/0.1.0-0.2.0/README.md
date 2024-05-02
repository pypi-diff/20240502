# Comparing `tmp/deltachat_chatbot-0.1.0-py3-none-any.whl.zip` & `tmp/deltachat_chatbot-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19316 bytes, number of entries: 10
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-28 01:16 deltachat_chatbot/__init__.py
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-28 01:16 deltachat_chatbot/__main__.py
--rw-r--r--  2.0 unx     7181 b- defN 24-Apr-28 01:16 deltachat_chatbot/gpt4all.py
--rw-r--r--  2.0 unx     5756 b- defN 24-Apr-28 01:16 deltachat_chatbot/hooks.py
--rw-r--r--  2.0 unx    35141 b- defN 24-Apr-28 01:16 deltachat_chatbot-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1529 b- defN 24-Apr-28 01:16 deltachat_chatbot-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 01:16 deltachat_chatbot-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 24-Apr-28 01:16 deltachat_chatbot-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-28 01:16 deltachat_chatbot-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      879 b- defN 24-Apr-28 01:16 deltachat_chatbot-0.1.0.dist-info/RECORD
-10 files, 50877 bytes uncompressed, 17792 bytes compressed:  65.0%
+Zip file size: 19318 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      165 b- defN 24-May-02 12:16 deltachat_chatbot/__init__.py
+-rw-r--r--  2.0 unx       65 b- defN 24-May-02 12:16 deltachat_chatbot/__main__.py
+-rw-r--r--  2.0 unx     7181 b- defN 24-May-02 12:16 deltachat_chatbot/gpt4all.py
+-rw-r--r--  2.0 unx     5756 b- defN 24-May-02 12:16 deltachat_chatbot/hooks.py
+-rw-r--r--  2.0 unx    35141 b- defN 24-May-02 12:16 deltachat_chatbot-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1529 b- defN 24-May-02 12:16 deltachat_chatbot-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 12:16 deltachat_chatbot-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 24-May-02 12:16 deltachat_chatbot-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-May-02 12:16 deltachat_chatbot-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      879 b- defN 24-May-02 12:16 deltachat_chatbot-0.2.0.dist-info/RECORD
+10 files, 50877 bytes uncompressed, 17794 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: deltachat_chatbot/gpt4all.py
 Comment: 
 
 Filename: deltachat_chatbot/hooks.py
 Comment: 
 
-Filename: deltachat_chatbot-0.1.0.dist-info/LICENSE
+Filename: deltachat_chatbot-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: deltachat_chatbot-0.1.0.dist-info/METADATA
+Filename: deltachat_chatbot-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: deltachat_chatbot-0.1.0.dist-info/WHEEL
+Filename: deltachat_chatbot-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: deltachat_chatbot-0.1.0.dist-info/entry_points.txt
+Filename: deltachat_chatbot-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: deltachat_chatbot-0.1.0.dist-info/top_level.txt
+Filename: deltachat_chatbot-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: deltachat_chatbot-0.1.0.dist-info/RECORD
+Filename: deltachat_chatbot-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deltachat_chatbot/hooks.py

```diff
@@ -31,15 +31,15 @@
     help="gpt4all model to use (default: %(default)s)",
     default="mistral-7b-openorca.gguf2.Q4_0.gguf",
 )
 cli.add_generic_option("--system-prompt", help="an initial instruction for the model")
 cli.add_generic_option(
     "--max-tokens",
     help="the maximum number of tokens to generate (default: %(default)s)",
-    default=200,
+    default=500,
     type=int,
 )
 cli.add_generic_option(
     "--history",
     help="the maximum number replies to rember (default: %(default)s)",
     default=20,
     type=int,
```

## Comparing `deltachat_chatbot-0.1.0.dist-info/LICENSE` & `deltachat_chatbot-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `deltachat_chatbot-0.1.0.dist-info/METADATA` & `deltachat_chatbot-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-chatbot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Conversational chat-bot for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/chatbot
 Keywords: deltachat,bot,chatbot,ai
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

## Comparing `deltachat_chatbot-0.1.0.dist-info/RECORD` & `deltachat_chatbot-0.2.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 deltachat_chatbot/__init__.py,sha256=-zJcWqNBNBqxfEQK0q7E7VIMwB1ibTJqLG4Eh7qdvXQ,165
 deltachat_chatbot/__main__.py,sha256=M7jcIQ0wYwLot7bzOqMQUEJv_190nXbdctI6hrTINbA,65
 deltachat_chatbot/gpt4all.py,sha256=DxcIhufBsXYlhsy5DfhxSKSXk2wAxn1rNC9-037ix7A,7181
-deltachat_chatbot/hooks.py,sha256=26T8dXRspiI9J2y9MhXel-fVDhJIJnJsPo6QIvpkyF4,5756
-deltachat_chatbot-0.1.0.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-deltachat_chatbot-0.1.0.dist-info/METADATA,sha256=z0x2fPIH8yp5W63vAj3R6lBKNO9QIWxL_qoqdpWEX0g,1529
-deltachat_chatbot-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-deltachat_chatbot-0.1.0.dist-info/entry_points.txt,sha256=sgZrTGKlpH07JDqLMlMDmURt2Lx0AovKcolhBys1pBY,51
-deltachat_chatbot-0.1.0.dist-info/top_level.txt,sha256=7asdSweUDlMasQ6vv7YcSyW24nptcaLgrNcqUGe87Vc,18
-deltachat_chatbot-0.1.0.dist-info/RECORD,,
+deltachat_chatbot/hooks.py,sha256=49Lk3q6fHWcOQdYwKAgCMbVm3DO4m4lGGtURU37A5D8,5756
+deltachat_chatbot-0.2.0.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+deltachat_chatbot-0.2.0.dist-info/METADATA,sha256=mPnjpk5Zb_7vOIg3umRjfCs1Km5-mnac6xCzsfTUb4k,1529
+deltachat_chatbot-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+deltachat_chatbot-0.2.0.dist-info/entry_points.txt,sha256=sgZrTGKlpH07JDqLMlMDmURt2Lx0AovKcolhBys1pBY,51
+deltachat_chatbot-0.2.0.dist-info/top_level.txt,sha256=7asdSweUDlMasQ6vv7YcSyW24nptcaLgrNcqUGe87Vc,18
+deltachat_chatbot-0.2.0.dist-info/RECORD,,
```

