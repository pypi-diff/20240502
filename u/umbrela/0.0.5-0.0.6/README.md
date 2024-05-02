# Comparing `tmp/umbrela-0.0.5-py3-none-any.whl.zip` & `tmp/umbrela-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16844 bytes, number of entries: 14
+Zip file size: 16842 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:11 umbrela/__init__.py
 -rw-r--r--  2.0 unx     2743 b- defN 24-May-01 22:34 umbrela/gpt_judge.py
 -rw-r--r--  2.0 unx      751 b- defN 24-Apr-30 23:41 umbrela/llm_judge.py
 -rw-r--r--  2.0 unx     2466 b- defN 24-May-01 18:54 umbrela/osllm_judge.py
 -rw-r--r--  2.0 unx     3400 b- defN 24-May-01 18:54 umbrela/vicuna_judge.py
 -rw-r--r--  2.0 unx     1334 b- defN 24-May-02 00:43 umbrela/prompts/qrel_fewshot_bing.txt
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:25 umbrela/utils/__init__.py
 -rw-r--r--  2.0 unx     1884 b- defN 24-May-01 01:04 umbrela/utils/common_utils.py
--rw-r--r--  2.0 unx     3063 b- defN 24-May-02 00:45 umbrela/utils/qrel_utils.py
--rw-r--r--  2.0 unx    10766 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    14489 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1115 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/RECORD
-14 files, 42111 bytes uncompressed, 14996 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     3068 b- defN 24-May-02 00:55 umbrela/utils/qrel_utils.py
+-rw-r--r--  2.0 unx    10766 b- defN 24-May-02 00:56 umbrela-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14488 b- defN 24-May-02 00:56 umbrela-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 00:56 umbrela-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-02 00:56 umbrela-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1115 b- defN 24-May-02 00:56 umbrela-0.0.6.dist-info/RECORD
+14 files, 42115 bytes uncompressed, 14994 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: umbrela/utils/common_utils.py
 Comment: 
 
 Filename: umbrela/utils/qrel_utils.py
 Comment: 
 
-Filename: umbrela-0.0.5.dist-info/LICENSE
+Filename: umbrela-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: umbrela-0.0.5.dist-info/METADATA
+Filename: umbrela-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: umbrela-0.0.5.dist-info/WHEEL
+Filename: umbrela-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: umbrela-0.0.5.dist-info/top_level.txt
+Filename: umbrela-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: umbrela-0.0.5.dist-info/RECORD
+Filename: umbrela-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## umbrela/utils/qrel_utils.py

```diff
@@ -48,15 +48,15 @@
         if qrel in ["dl19-passage", "dl20-passage"]:
             passage = json.loads(index_reader.doc_raw(str(example[1]))).get(
                 "contents", ""
             )
         else:
             passage = get_passage(example[1])
 
-        res_json = {"O": qrel_data[example[0]][example[1]]}
+        res_json = {"O": int(qrel_data[example[0]][example[1]])}
         prompt_examples += f"""
                 ###
 
                 Query: {query}
                 Passage: {passage}
                 Output: {res_json}
                 """
```

## Comparing `umbrela-0.0.5.dist-info/LICENSE` & `umbrela-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `umbrela-0.0.5.dist-info/METADATA` & `umbrela-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbrela
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Package for generating query-passage relevance assessment labels.
 Author-email: Shivani Upadhyay <sjupadhyay@uwaterloo.ca>, Ronak Pradeep <rpradeep@uwaterloo.ca>, Jimmy Lin <jimmylin@uwaterloo.ca>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,15 +235,15 @@
 pip install -r requirements.txt
 ```
 
 ### Judgment generation snippet
 
 #### Setting up the model jugde:
 ```python
-from umbrela.vicuna_judge import VicunaJudge
+from umbrela.vicuna_judge import OSLLMJudge
 
 judge_vicuna = OSLLMJudge("dl19-passage", "lmsys/vicuna-7b-v1.5")
 ```
 
 #### Passing qrel-passages for evaluations:
 ```python
 input_dict = {
```

## Comparing `umbrela-0.0.5.dist-info/RECORD` & `umbrela-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 umbrela/gpt_judge.py,sha256=gJr6K_loYqBkaL1HK74hZVpj2tml_ZUHIEilXvKytkM,2743
 umbrela/llm_judge.py,sha256=7uC-GFZvw_vQom4jekvc_Z5NYNH8CJLoVGgL8LLosu0,751
 umbrela/osllm_judge.py,sha256=EcuR9N60vCc0ySrh56BxQ1BGDyFglepJwp2aQtJ5VZc,2466
 umbrela/vicuna_judge.py,sha256=J7t16ut6tHTMEQea4I_bZiQZhisp9eWtdqZSalbluGU,3400
 umbrela/prompts/qrel_fewshot_bing.txt,sha256=N_HM-Sa6ntPPwfnS1sM7qAobS5rEDcRe0JgeVaT1xV4,1334
 umbrela/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 umbrela/utils/common_utils.py,sha256=6AdK9cKsYZ773yTeUb8X_aQfoPi8cMTyxxfuAtBFH_M,1884
-umbrela/utils/qrel_utils.py,sha256=5o2VAUqwoTLiIzNDRRhoIxR1Ad-rKpPEF6sovVFwtEk,3063
-umbrela-0.0.5.dist-info/LICENSE,sha256=5xLBDUMjnrK1STpg2CvThfuHUKCCFxoSozCIGAx56Pk,10766
-umbrela-0.0.5.dist-info/METADATA,sha256=fYmuNM9_3BVvpQ8jENCIXrBtE-lVMY3RJ-p1DxQ4uYE,14489
-umbrela-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-umbrela-0.0.5.dist-info/top_level.txt,sha256=E6ASKK6PNcJWJAC6mYtbt91P5fKJrAkJtRoGthCaYUI,8
-umbrela-0.0.5.dist-info/RECORD,,
+umbrela/utils/qrel_utils.py,sha256=AF2t2tnm1YGRVM8Ey1vmhxQtQJnMXf8KNJVHj7PchzM,3068
+umbrela-0.0.6.dist-info/LICENSE,sha256=5xLBDUMjnrK1STpg2CvThfuHUKCCFxoSozCIGAx56Pk,10766
+umbrela-0.0.6.dist-info/METADATA,sha256=DaAo1OxWcNfdbXfmrbowaiH4GBIW5_U-RYHaQ1O5hAs,14488
+umbrela-0.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+umbrela-0.0.6.dist-info/top_level.txt,sha256=E6ASKK6PNcJWJAC6mYtbt91P5fKJrAkJtRoGthCaYUI,8
+umbrela-0.0.6.dist-info/RECORD,,
```

