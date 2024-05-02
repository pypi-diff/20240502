# Comparing `tmp/lense-0.0.8-py3-none-any.whl.zip` & `tmp/lense-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9977 bytes, number of entries: 14
+Zip file size: 9974 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-22 06:00 lense/__init__.py
--rw-rw-rw-  2.0 fat     6484 b- defN 24-Apr-23 08:07 lense/app.py
+-rw-rw-rw-  2.0 fat     6482 b- defN 24-Apr-23 08:10 lense/app.py
 -rw-rw-rw-  2.0 fat     3290 b- defN 24-Apr-22 07:32 lense/backend/SQL_engine.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-22 06:59 lense/backend/__init__.py
 -rw-rw-rw-  2.0 fat     1173 b- defN 24-Apr-22 07:20 lense/backend/cglense.py
 -rw-rw-rw-  2.0 fat     5836 b- defN 24-Apr-22 07:22 lense/backend/csv_engine.py
 -rw-rw-rw-  2.0 fat     4694 b- defN 24-Apr-22 07:24 lense/backend/error_handling.py
 -rw-rw-rw-  2.0 fat     1064 b- defN 24-Apr-23 07:54 lense/backend/loader.py
 -rw-rw-rw-  2.0 fat     2464 b- defN 24-Apr-22 07:28 lense/backend/qna_engine.py
 -rw-rw-rw-  2.0 fat     3336 b- defN 24-Apr-22 07:31 lense/backend/replace_file.py
--rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-23 08:07 lense-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 08:07 lense-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 08:07 lense-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1095 b- defN 24-Apr-23 08:07 lense-0.0.8.dist-info/RECORD
-14 files, 30486 bytes uncompressed, 8167 bytes compressed:  73.2%
+-rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-23 08:11 lense-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 08:11 lense-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 08:11 lense-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1095 b- defN 24-Apr-23 08:11 lense-0.0.9.dist-info/RECORD
+14 files, 30484 bytes uncompressed, 8164 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: lense/backend/qna_engine.py
 Comment: 
 
 Filename: lense/backend/replace_file.py
 Comment: 
 
-Filename: lense-0.0.8.dist-info/METADATA
+Filename: lense-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: lense-0.0.8.dist-info/WHEEL
+Filename: lense-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: lense-0.0.8.dist-info/top_level.txt
+Filename: lense-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: lense-0.0.8.dist-info/RECORD
+Filename: lense-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lense/app.py

```diff
@@ -193,9 +193,9 @@
         return {"result": result}
     
     except Exception as e:
         return {"error": str(e)}
     
 
 def start():
-    app.mount("/", StaticFiles(directory="/my_frontend", html=True), name="/my_frontend")
+    app.mount("/", StaticFiles(directory="my_frontend", html=True), name="my_frontend")
     uvicorn.run("lense.app:app", reload=False, host="127.0.0.1", port=9009,workers=1)
```

## Comparing `lense-0.0.8.dist-info/METADATA` & `lense-0.0.9.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lense
-Version: 0.0.8
+Version: 0.0.9
 Requires-Dist: pandas ==2.2.2
 Requires-Dist: PyPDF2 ==3.0.1
 Requires-Dist: python-docx ==1.1.0
 Requires-Dist: python-pptx ==0.6.23
 Requires-Dist: llama-index ==0.10.29
 Requires-Dist: llama-index.llms.azure-openai ==0.1.5
 Requires-Dist: llama-index.embeddings.azure-openai ==0.1.6
```

## Comparing `lense-0.0.8.dist-info/RECORD` & `lense-0.0.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 lense/__init__.py,sha256=5rivs2U5ia9uXArxLc1H8FyzIZXtDjxp_vsZsUEDo60,22
-lense/app.py,sha256=h9ciVFJXkMiEcg31G25pXfCp9umGs_-NpB-o1kUvJDM,6484
+lense/app.py,sha256=kyOJ8C4cgqqUiBWMO29QKB2oRaMhul_TuXtVvVZSpvI,6482
 lense/backend/SQL_engine.py,sha256=Gzs7MM3n-xACgZ6sAUbRZxdecvcP819YBFNhiNy8020,3290
 lense/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lense/backend/cglense.py,sha256=nba7Qa0B64U1RzhFenAOiFfarNS5qYSt0IPeqpHhSWA,1173
 lense/backend/csv_engine.py,sha256=id-MVVsjD2KZlB8Q0gvols1db2Ot5t7K1HemEDx_gN8,5836
 lense/backend/error_handling.py,sha256=HjB1eD-2jwhC7-rwvUc6CtYICjinKnMKop4DheUQOM4,4694
 lense/backend/loader.py,sha256=c0v_AKf9Qu4O_IzKqNF-EQNYu6PcUN2HTtfVwGxb8NI,1064
 lense/backend/qna_engine.py,sha256=VZkoMp-jqitYdWOsoctmeN1ApBE5cxyGJ2IHI6Wz994,2464
 lense/backend/replace_file.py,sha256=-DzKIrFXiKwhMZAPW7GSfDIhV9FGB7yhOqp3OqlS7eE,3336
-lense-0.0.8.dist-info/METADATA,sha256=12p_0SewF7AEJZVWpY4SRh_L-_HJRDPZpG5tUhRxZ78,930
-lense-0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-lense-0.0.8.dist-info/top_level.txt,sha256=iyP2ZFtpvgpecDSV53lznPmRGjO3FUFAnNUkUTRbxIg,6
-lense-0.0.8.dist-info/RECORD,,
+lense-0.0.9.dist-info/METADATA,sha256=js2RRSdVJWJ7_rKbx1PH2Bw9W3vqpkw7e93V6UXo598,930
+lense-0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+lense-0.0.9.dist-info/top_level.txt,sha256=iyP2ZFtpvgpecDSV53lznPmRGjO3FUFAnNUkUTRbxIg,6
+lense-0.0.9.dist-info/RECORD,,
```

