# Comparing `tmp/umbrela-0.0.4-py3-none-any.whl.zip` & `tmp/umbrela-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16069 bytes, number of entries: 14
+Zip file size: 16844 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:11 umbrela/__init__.py
--rw-r--r--  2.0 unx     2713 b- defN 24-May-01 18:48 umbrela/gpt_judge.py
+-rw-r--r--  2.0 unx     2743 b- defN 24-May-01 22:34 umbrela/gpt_judge.py
 -rw-r--r--  2.0 unx      751 b- defN 24-Apr-30 23:41 umbrela/llm_judge.py
--rw-r--r--  2.0 unx     2443 b- defN 24-May-01 18:47 umbrela/osllm_judge.py
--rw-r--r--  2.0 unx     3380 b- defN 24-May-01 18:46 umbrela/vicuna_judge.py
--rw-r--r--  2.0 unx     1231 b- defN 24-May-01 01:05 umbrela/prompts/qrel_fewshot_bing.txt
+-rw-r--r--  2.0 unx     2466 b- defN 24-May-01 18:54 umbrela/osllm_judge.py
+-rw-r--r--  2.0 unx     3400 b- defN 24-May-01 18:54 umbrela/vicuna_judge.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-02 00:43 umbrela/prompts/qrel_fewshot_bing.txt
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:25 umbrela/utils/__init__.py
 -rw-r--r--  2.0 unx     1884 b- defN 24-May-01 01:04 umbrela/utils/common_utils.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-01 18:15 umbrela/utils/qrel_utils.py
--rw-r--r--  2.0 unx    10766 b- defN 24-May-01 18:49 umbrela-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    13073 b- defN 24-May-01 18:49 umbrela-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 18:49 umbrela-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-01 18:49 umbrela-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1115 b- defN 24-May-01 18:49 umbrela-0.0.4.dist-info/RECORD
-14 files, 40496 bytes uncompressed, 14221 bytes compressed:  64.9%
+-rw-r--r--  2.0 unx     3063 b- defN 24-May-02 00:45 umbrela/utils/qrel_utils.py
+-rw-r--r--  2.0 unx    10766 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14489 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1115 b- defN 24-May-02 00:46 umbrela-0.0.5.dist-info/RECORD
+14 files, 42111 bytes uncompressed, 14996 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: umbrela/utils/common_utils.py
 Comment: 
 
 Filename: umbrela/utils/qrel_utils.py
 Comment: 
 
-Filename: umbrela-0.0.4.dist-info/LICENSE
+Filename: umbrela-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: umbrela-0.0.4.dist-info/METADATA
+Filename: umbrela-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: umbrela-0.0.4.dist-info/WHEEL
+Filename: umbrela-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: umbrela-0.0.4.dist-info/top_level.txt
+Filename: umbrela-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: umbrela-0.0.4.dist-info/RECORD
+Filename: umbrela-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## umbrela/gpt_judge.py

```diff
@@ -9,17 +9,19 @@
 from umbrela.utils import common_utils
 
 
 class GPTJudge(LLMJudge):
     def __init__(
         self,
         qrel: str,
-        prompt_file=pkg_resources.resource_filename("umbrela", "prompts/qrel_fewshot_bing.txt"),
+        prompt_file: str = pkg_resources.resource_filename(
+            "umbrela", "prompts/qrel_fewshot_bing.txt"
+        ),
         few_shot_count: int = 2,
-        engine=""
+        engine="",
     ) -> None:
         model_name = engine if engine else "gpt"
         super().__init__(qrel, prompt_file, model_name, few_shot_count)
         self.create_openai_client()
 
     def create_openai_client(self):
         api_key = os.environ["OPEN_AI_API_KEY"]
```

## umbrela/osllm_judge.py

```diff
@@ -4,20 +4,23 @@
 import torch
 from tqdm import tqdm
 from transformers.generation import GenerationConfig
 
 from umbrela.llm_judge import LLMJudge
 from umbrela.utils import common_utils
 
+
 class OSLLMJudge(LLMJudge):
     def __init__(
         self,
         qrel: str,
         model_name: str,
-        prompt_file: str = pkg_resources.resource_filename("umbrela", "prompts/qrel_fewshot_bing.txt"),
+        prompt_file: str = pkg_resources.resource_filename(
+            "umbrela", "prompts/qrel_fewshot_bing.txt"
+        ),
         few_shot_count: int = 2,
         device: str = "cuda",
         num_gpus: int = 1,
     ) -> None:
         super().__init__(qrel, prompt_file, model_name, few_shot_count)
         self._device = device
         if self._device == "cuda":
```

## umbrela/vicuna_judge.py

```diff
@@ -10,15 +10,17 @@
 from umbrela.utils import common_utils
 
 
 class VicunaJudge(LLMJudge):
     def __init__(
         self,
         qrel: str,
-        prompt_file: str = pkg_resources.resource_filename(__name__, "prompts/qrel_fewshot_bing.txt"),
+        prompt_file: str = pkg_resources.resource_filename(
+            __name__, "prompts/qrel_fewshot_bing.txt"
+        ),
         few_shot_count: int = 2,
         device: str = "cuda",
         num_gpus: int = 1,
     ) -> None:
         super().__init__(qrel, prompt_file, "lmsys/vicuna-7b-v1.5-16k", few_shot_count)
         self._device = device
         if self._device == "cuda":
@@ -91,12 +93,12 @@
 
                 outputs.append(
                     tokenizer.decode(output_ids, skip_special_tokens=True).strip()
                 )
 
         return outputs
 
-    def judge(self, request_dict, max_new_tokens = 100):
+    def judge(self, request_dict, max_new_tokens=100):
         outputs = self.predict_with_llm(request_dict, max_new_tokens)
         return common_utils.prepare_judgments(
             outputs, self.query_passage, self.prompts, self.model_name
         )
```

## umbrela/prompts/qrel_fewshot_bing.txt

```diff
@@ -1,13 +1,17 @@
 Given a query and a passage, you must provide a score on an integer scale of 0 to 3 with the following meanings:
 0 = represent that the passage has nothing to do with the query, 
 1 = represents that the passage seems related to the query but does not answer it, 
 2 = represents that the passage has some answer for the query, but the answer may be a bit unclear, or hidden amongst extraneous information and 
 3 = represents that the passage is dedicated to the query and contains the exact answer.
 
+Following are some of the examples of relevance categorizations for different categories:
+
+{examples}
+
 Assume that you are writing a report on the subject of the topic. If you would use any of the information contained in the passage in such a report, mark it 1. If the passage is primarily about the topic mark it 3, or contains vital information about the topic, mark it 2. Otherwise, mark it 0.
 
 Query: {query}
 Passage: {passage}
 
 Split this problem into steps:
 Consider the underlying intent of the search.
```

## umbrela/utils/qrel_utils.py

```diff
@@ -48,20 +48,21 @@
         if qrel in ["dl19-passage", "dl20-passage"]:
             passage = json.loads(index_reader.doc_raw(str(example[1]))).get(
                 "contents", ""
             )
         else:
             passage = get_passage(example[1])
 
+        res_json = {"O": qrel_data[example[0]][example[1]]}
         prompt_examples += f"""
                 ###
 
                 Query: {query}
                 Passage: {passage}
-                Relevance category: {qrel_data[example[0]][example[1]]}
+                Output: {res_json}
                 """
     return prompt_examples
 
 
 def get_query_mappings(qrel):
     # Query mappings
     topic_mapping = {
```

## Comparing `umbrela-0.0.4.dist-info/LICENSE` & `umbrela-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `umbrela-0.0.4.dist-info/METADATA` & `umbrela-0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbrela
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Package for generating query-passage relevance assessment labels.
 Author-email: Shivani Upadhyay <sjupadhyay@uwaterloo.ca>, Ronak Pradeep <rpradeep@uwaterloo.ca>, Jimmy Lin <jimmylin@uwaterloo.ca>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -197,16 +197,72 @@
 Project-URL: Homepage, https://github.com/castorini/umbrela
 Keywords: LLM,evaluation,information retrieval
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasets ==2.19.0
-Requires-Dist: fschat ==0.2.36
-Requires-Dist: openai ==1.24.1
-Requires-Dist: pyserini ==0.35.0
-Requires-Dist: torch ==2.2.2
-Requires-Dist: tqdm ==4.66.2
-Requires-Dist: transformers ==4.40.1
+Requires-Dist: datasets >=2.19.0
+Requires-Dist: fschat >=0.2.36
+Requires-Dist: openai >=1.24.1
+Requires-Dist: pyserini >=0.35.0
+Requires-Dist: torch >=2.2.2
+Requires-Dist: tqdm >=4.66.2
+Requires-Dist: transformers >=4.40.1
 
 # umBRELA
+
+## 📟 Instructions
+
+### Create Conda Environment
+
+```bash
+conda create -n umbrela python=3.10
+conda activate umbrela
+```
+
+### If you do not already have JDK 21 installed, install via conda:
+```bash
+conda install -c conda-forge openjdk=21 maven -y
+```
+
+### Install following dependencies for retrieval:
+```bash
+conda install -c pytorch faiss-cpu pytorch -y
+```
+
+### Install Dependencies
+```bash
+pip install -r requirements.txt
+```
+
+### Judgment generation snippet
+
+#### Setting up the model jugde:
+```python
+from umbrela.vicuna_judge import VicunaJudge
+
+judge_vicuna = OSLLMJudge("dl19-passage", "lmsys/vicuna-7b-v1.5")
+```
+
+#### Passing qrel-passages for evaluations:
+```python
+input_dict = {
+    "query": {"text": "how long is life cycle of flea", "qid": "264014"},
+    "candidates": [
+        {
+            "doc": {
+                "segment": "The life cycle of a flea can last anywhere from 20 days to an entire year. It depends on how long the flea remains in the dormant stage (eggs, larvae, pupa). Outside influences, such as weather, affect the flea cycle. A female flea can lay around 20 to 25 eggs in one day."
+            },
+            "docid": "4834547",
+            "score": 14.971799850463867,
+        },
+    ]
+}
+
+judgments = judge_vicuna.judge(input_dict)
+```
+
+
+## 🙏 Acknowledgments
+
+This research is supported in part by the Natural Sciences and Engineering Research Council (NSERC) of Canada.
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `umbrela-0.0.4.dist-info/RECORD` & `umbrela-0.0.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 umbrela/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-umbrela/gpt_judge.py,sha256=mU-95tMDVf-2GIARUFX7ot1TidbvQxi-F7epxFVHL7s,2713
+umbrela/gpt_judge.py,sha256=gJr6K_loYqBkaL1HK74hZVpj2tml_ZUHIEilXvKytkM,2743
 umbrela/llm_judge.py,sha256=7uC-GFZvw_vQom4jekvc_Z5NYNH8CJLoVGgL8LLosu0,751
-umbrela/osllm_judge.py,sha256=tc31-unseNSiQQWvH65z5T9AWMtmp35uAsJb1U3k690,2443
-umbrela/vicuna_judge.py,sha256=dOzzHSjcg8r7tnXy10Pma2pvbWQ0k_taF5y9VxqsZNY,3380
-umbrela/prompts/qrel_fewshot_bing.txt,sha256=9Z1aw7tOHhbAuaLuUf5mjusxFNdNSZJaZzYIbCCLHuk,1231
+umbrela/osllm_judge.py,sha256=EcuR9N60vCc0ySrh56BxQ1BGDyFglepJwp2aQtJ5VZc,2466
+umbrela/vicuna_judge.py,sha256=J7t16ut6tHTMEQea4I_bZiQZhisp9eWtdqZSalbluGU,3400
+umbrela/prompts/qrel_fewshot_bing.txt,sha256=N_HM-Sa6ntPPwfnS1sM7qAobS5rEDcRe0JgeVaT1xV4,1334
 umbrela/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 umbrela/utils/common_utils.py,sha256=6AdK9cKsYZ773yTeUb8X_aQfoPi8cMTyxxfuAtBFH_M,1884
-umbrela/utils/qrel_utils.py,sha256=JeGZiVbUaZCY-l98T9ASPf6BWTZK9H2aIsNU3aaYaFk,3040
-umbrela-0.0.4.dist-info/LICENSE,sha256=5xLBDUMjnrK1STpg2CvThfuHUKCCFxoSozCIGAx56Pk,10766
-umbrela-0.0.4.dist-info/METADATA,sha256=Rl3bZB8l5crzt-baoEtYfCbJG8i4FquZ2kF7HG_oT3k,13073
-umbrela-0.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-umbrela-0.0.4.dist-info/top_level.txt,sha256=E6ASKK6PNcJWJAC6mYtbt91P5fKJrAkJtRoGthCaYUI,8
-umbrela-0.0.4.dist-info/RECORD,,
+umbrela/utils/qrel_utils.py,sha256=5o2VAUqwoTLiIzNDRRhoIxR1Ad-rKpPEF6sovVFwtEk,3063
+umbrela-0.0.5.dist-info/LICENSE,sha256=5xLBDUMjnrK1STpg2CvThfuHUKCCFxoSozCIGAx56Pk,10766
+umbrela-0.0.5.dist-info/METADATA,sha256=fYmuNM9_3BVvpQ8jENCIXrBtE-lVMY3RJ-p1DxQ4uYE,14489
+umbrela-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+umbrela-0.0.5.dist-info/top_level.txt,sha256=E6ASKK6PNcJWJAC6mYtbt91P5fKJrAkJtRoGthCaYUI,8
+umbrela-0.0.5.dist-info/RECORD,,
```

