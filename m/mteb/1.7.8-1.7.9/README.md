# Comparing `tmp/mteb-1.7.8.tar.gz` & `tmp/mteb-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.7.8.tar", last modified: Tue Apr 23 07:19:43 2024, max compression
+gzip compressed data, was "mteb-1.7.9.tar", last modified: Tue Apr 23 07:43:09 2024, max compression
```

## Comparing `mteb-1.7.8.tar` & `mteb-1.7.9.tar`

### file list

```diff
@@ -1,764 +1,772 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.336239 mteb-1.7.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-23 07:19:39.000000 mteb-1.7.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23583 2024-04-23 07:19:43.336239 mteb-1.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2024-04-23 07:19:39.000000 mteb-1.7.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.200239 mteb-1.7.8/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.216239 mteb-1.7.8/docs/mmteb/
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-23 07:19:39.000000 mteb-1.7.8/docs/mmteb/create_points_table.py
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-23 07:19:39.000000 mteb-1.7.8/docs/mmteb/validate_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.216239 mteb-1.7.8/mteb/
--rw-r--r--   0 root         (0) root         (0)     2273 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.224238 mteb-1.7.8/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     2284 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5876 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2384 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)    24826 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskInstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1013 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     9793 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7082 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/iso_15924_to_script.json
--rw-r--r--   0 root         (0) root         (0)   193114 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/iso_639_3_to_language.json
--rw-r--r--   0 root         (0) root         (0)      541 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/abstasks/languages.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.224238 mteb-1.7.8/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13004 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.224238 mteb-1.7.8/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5840 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8927 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)      789 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     7126 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9554 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    13983 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      820 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.228239 mteb-1.7.8/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.228239 mteb-1.7.8/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      567 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.228239 mteb-1.7.8/mteb/tasks/BitextMining/dan/
--rw-r--r--   0 root         (0) root         (0)     1443 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.228239 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     3552 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1423 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.228239 mteb-1.7.8/mteb/tasks/BitextMining/vie/
--rw-r--r--   0 root         (0) root         (0)     2889 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/BitextMining/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.228239 mteb-1.7.8/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     3114 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/ara/
--rw-r--r--   0 root         (0) root         (0)     1725 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1913 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ara/TweetEmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)     3161 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ara/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/bam/
--rw-r--r--   0 root         (0) root         (0)     1969 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/bam/BambaraSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/bam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/ben/
--rw-r--r--   0 root         (0) root         (0)     1793 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ben/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/bul/
--rw-r--r--   0 root         (0) root         (0)     2031 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1947 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/bul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/ces/
--rw-r--r--   0 root         (0) root         (0)     1704 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/dan/
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2502 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.232239 mteb-1.7.8/mteb/tasks/Classification/ell/
--rw-r--r--   0 root         (0) root         (0)     2172 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ell/GreekSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/eng/
--rw-r--r--   0 root         (0) root         (0)     1041 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/est/
--rw-r--r--   0 root         (0) root         (0)     2407 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/est/estonian_valence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/fas/
--rw-r--r--   0 root         (0) root         (0)     1874 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/fas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/fil/
--rw-r--r--   0 root         (0) root         (0)     2085 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/fil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/fra/
--rw-r--r--   0 root         (0) root         (0)     1905 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/guj/
--rw-r--r--   0 root         (0) root         (0)     1285 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/guj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/hin/
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/hin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.236239 mteb-1.7.8/mteb/tasks/Classification/hrv/
--rw-r--r--   0 root         (0) root         (0)     2028 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/hrv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.240239 mteb-1.7.8/mteb/tasks/Classification/ind/
--rw-r--r--   0 root         (0) root         (0)     2881 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ind/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.240239 mteb-1.7.8/mteb/tasks/Classification/ita/
--rw-r--r--   0 root         (0) root         (0)     4105 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ita/ItaHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ita/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.240239 mteb-1.7.8/mteb/tasks/Classification/jpn/
--rw-r--r--   0 root         (0) root         (0)     3550 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/jpn/WRIMEClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.240239 mteb-1.7.8/mteb/tasks/Classification/kur/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/kur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.240239 mteb-1.7.8/mteb/tasks/Classification/mkd/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/mkd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.240239 mteb-1.7.8/mteb/tasks/Classification/mlt/
--rw-r--r--   0 root         (0) root         (0)     2023 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/mlt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1575 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6099 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)     3358 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/ToxicChatClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/nld/
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/nld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/nob/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/nob/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/nob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/pol/
--rw-r--r--   0 root         (0) root         (0)     4922 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/pol/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/ron/
--rw-r--r--   0 root         (0) root         (0)     1587 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ron/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/slk/
--rw-r--r--   0 root         (0) root         (0)     2078 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/slk/SlovakSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/slk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/ssw/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/ssw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/swe/
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/swe/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/swe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/tur/
--rw-r--r--   0 root         (0) root         (0)     1518 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/tur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.244239 mteb-1.7.8/mteb/tasks/Classification/uig/
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/uig/UyghurSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/uig/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.248239 mteb-1.7.8/mteb/tasks/Classification/vie/
--rw-r--r--   0 root         (0) root         (0)     3368 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.248239 mteb-1.7.8/mteb/tasks/Classification/zho/
--rw-r--r--   0 root         (0) root         (0)     6571 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/zho/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)     1729 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.248239 mteb-1.7.8/mteb/tasks/Classification/zul/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Classification/zul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.248239 mteb-1.7.8/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1319 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.248239 mteb-1.7.8/mteb/tasks/Clustering/deu/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.252239 mteb-1.7.8/mteb/tasks/Clustering/eng/
--rw-r--r--   0 root         (0) root         (0)     1101 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.252239 mteb-1.7.8/mteb/tasks/Clustering/fra/
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1607 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     2406 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.252239 mteb-1.7.8/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2687 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.252239 mteb-1.7.8/mteb/tasks/Clustering/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3442 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/nob/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/nob/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.252239 mteb-1.7.8/mteb/tasks/Clustering/pol/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/pol/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.252239 mteb-1.7.8/mteb/tasks/Clustering/rom/
--rw-r--r--   0 root         (0) root         (0)     1089 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/Clustering/spa/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/Clustering/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3917 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/swe/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/Clustering/zho/
--rw-r--r--   0 root         (0) root         (0)     3639 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/zho/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Clustering/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/InstructionRetrieval/
--rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/InstructionRetrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1548 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1555 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/PairClassification/deu/
--rw-r--r--   0 root         (0) root         (0)     2862 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/PairClassification/eng/
--rw-r--r--   0 root         (0) root         (0)     1152 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2780 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.256239 mteb-1.7.8/mteb/tasks/PairClassification/pol/
--rw-r--r--   0 root         (0) root         (0)     3577 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/pol/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/PairClassification/zho/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/PairClassification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Reranking/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/eng/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/eng/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Reranking/fra/
--rw-r--r--   0 root         (0) root         (0)     1195 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/fra/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/fra/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Reranking/zho/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/zho/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Reranking/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Retrieval/code/
--rw-r--r--   0 root         (0) root         (0)     3377 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.260239 mteb-1.7.8/mteb/tasks/Retrieval/dan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/dan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/dan/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2574 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/dan/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.264239 mteb-1.7.8/mteb/tasks/Retrieval/deu/
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2891 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.272239 mteb-1.7.8/mteb/tasks/Retrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.272239 mteb-1.7.8/mteb/tasks/Retrieval/est/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/est/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/est/estqa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.272239 mteb-1.7.8/mteb/tasks/Retrieval/fra/
--rw-r--r--   0 root         (0) root         (0)     2144 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2475 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3184 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2148 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.272239 mteb-1.7.8/mteb/tasks/Retrieval/hun/
--rw-r--r--   0 root         (0) root         (0)     2589 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/hun/HunSum2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.272239 mteb-1.7.8/mteb/tasks/Retrieval/jpn/
--rw-r--r--   0 root         (0) root         (0)     2853 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.272239 mteb-1.7.8/mteb/tasks/Retrieval/kor/
--rw-r--r--   0 root         (0) root         (0)      906 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/kor/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.276239 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3277 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3731 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3771 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3145 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.276239 mteb-1.7.8/mteb/tasks/Retrieval/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/nob/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/nob/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.276239 mteb-1.7.8/mteb/tasks/Retrieval/pol/
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.280239 mteb-1.7.8/mteb/tasks/Retrieval/spa/
--rw-r--r--   0 root         (0) root         (0)     2125 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.280239 mteb-1.7.8/mteb/tasks/Retrieval/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.280239 mteb-1.7.8/mteb/tasks/Retrieval/vie/
--rw-r--r--   0 root         (0) root         (0)     3798 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.280239 mteb-1.7.8/mteb/tasks/Retrieval/zho/
--rw-r--r--   0 root         (0) root         (0)    10384 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Retrieval/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.280239 mteb-1.7.8/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.280239 mteb-1.7.8/mteb/tasks/STS/deu/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/eng/
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/fra/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/fra/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/jpn/
--rw-r--r--   0 root         (0) root         (0)     3034 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/jpn/JSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/kor/
--rw-r--r--   0 root         (0) root         (0)     2504 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/kor/KlueSTS.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/kor/KorSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/pol/
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/pol/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/ron/
--rw-r--r--   0 root         (0) root         (0)     1896 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/ron/RonSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/spa/
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/spa/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/STS/zho/
--rw-r--r--   0 root         (0) root         (0)     7122 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/zho/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/STS/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.284239 mteb-1.7.8/mteb/tasks/Summarization/eng/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Summarization/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.288239 mteb-1.7.8/mteb/tasks/Summarization/fra/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/Summarization/fra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      288 2024-04-23 07:19:39.000000 mteb-1.7.8/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.336239 mteb-1.7.8/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23583 2024-04-23 07:19:43.000000 mteb-1.7.8/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35941 2024-04-23 07:19:43.000000 mteb-1.7.8/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:19:43.000000 mteb-1.7.8/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 07:19:43.000000 mteb-1.7.8/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-23 07:19:43.000000 mteb-1.7.8/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-23 07:19:43.000000 mteb-1.7.8/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2728 2024-04-23 07:19:40.000000 mteb-1.7.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.212239 mteb-1.7.8/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.288239 mteb-1.7.8/results/GritLM__GritLM-7B/
--rw-r--r--   0 root         (0) root         (0)     2342 2024-04-23 07:19:39.000000 mteb-1.7.8/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2381 2024-04-23 07:19:39.000000 mteb-1.7.8/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2384 2024-04-23 07:19:39.000000 mteb-1.7.8/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.212239 mteb-1.7.8/results/dangvantuan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.292239 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      250 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      675 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
--rw-r--r--   0 root         (0) root         (0)      676 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
--rw-r--r--   0 root         (0) root         (0)      332 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      335 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
--rw-r--r--   0 root         (0) root         (0)     1242 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2992 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)     2801 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      820 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/SICKFr.json
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/STS22.json
--rw-r--r--   0 root         (0) root         (0)      921 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1245 2024-04-23 07:19:39.000000 mteb-1.7.8/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.212239 mteb-1.7.8/results/intfloat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.292239 mteb-1.7.8/results/intfloat/multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat/multilingual-e5-small/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat/multilingual-e5-small/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat/multilingual-e5-small/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat/multilingual-e5-small/SlovakSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.292239 mteb-1.7.8/results/intfloat__e5-small/
--rw-r--r--   0 root         (0) root         (0)      439 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__e5-small/TurkishProductSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.292239 mteb-1.7.8/results/intfloat__e5-small-v2/
--rw-r--r--   0 root         (0) root         (0)     2512 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2540 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2550 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.296239 mteb-1.7.8/results/intfloat__multilingual-e5-base/
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      733 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-base/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.308239 mteb-1.7.8/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/BambaraSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2105 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/GermanDPR.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1289 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/ItaHateClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1163 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7814 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7703 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3386 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3392 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      403 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      304 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1116 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1028 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)     2184 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-04-23 07:19:39.000000 mteb-1.7.8/results/intfloat__multilingual-e5-small/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.308239 mteb-1.7.8/results/sentence-transformers/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers/ToxicChatClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.308239 mteb-1.7.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SlovakSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.312239 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1014 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      302 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/model.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.328239 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      759 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      746 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
--rw-r--r--   0 root         (0) root         (0)      610 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1317 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaHateClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7839 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7915 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1152 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      736 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3382 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3376 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)    16669 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)    18247 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      741 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      294 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
--rw-r--r--   0 root         (0) root         (0)     2186 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 07:19:39.000000 mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.328239 mteb-1.7.8/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.328239 mteb-1.7.8/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.328239 mteb-1.7.8/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.328239 mteb-1.7.8/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.328239 mteb-1.7.8/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5924 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2133 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/medicalqaretrieval/
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/medicalqaretrieval/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2435 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/mteb_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.216239 mteb-1.7.8/scripts/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.332239 mteb-1.7.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1008 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-23 07:19:39.000000 mteb-1.7.8/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:19:43.336239 mteb-1.7.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:19:43.336239 mteb-1.7.8/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1418 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2404 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_all_abstasks.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_mteb.py
--rw-r--r--   0 root         (0) root         (0)      278 2024-04-23 07:19:39.000000 mteb-1.7.8/tests/test_retrieval_abstask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.191770 mteb-1.7.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-23 07:43:04.000000 mteb-1.7.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23583 2024-04-23 07:43:09.187770 mteb-1.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2024-04-23 07:43:04.000000 mteb-1.7.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.043770 mteb-1.7.9/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.063770 mteb-1.7.9/docs/mmteb/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-23 07:43:04.000000 mteb-1.7.9/docs/mmteb/create_points_table.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-23 07:43:04.000000 mteb-1.7.9/docs/mmteb/validate_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.063770 mteb-1.7.9/mteb/
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.067770 mteb-1.7.9/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)    24826 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskInstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     9810 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/iso_15924_to_script.json
+-rw-r--r--   0 root         (0) root         (0)   193114 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/iso_639_3_to_language.json
+-rw-r--r--   0 root         (0) root         (0)      541 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/languages.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13004 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8927 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)      789 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    13983 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      820 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/tasks/BitextMining/dan/
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5709 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/BitextMining/vie/
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     3171 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/ara/
+-rw-r--r--   0 root         (0) root         (0)     1725 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/TweetEmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/bam/
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bam/BambaraSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/ben/
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ben/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/bul/
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/ces/
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/dan/
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/ell/
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ell/GreekSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/est/
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/est/estonian_valence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/fas/
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/fil/
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/fra/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/guj/
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/guj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/hin/
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/hrv/
+-rw-r--r--   0 root         (0) root         (0)     2028 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hrv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/ind/
+-rw-r--r--   0 root         (0) root         (0)     2881 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/ita/
+-rw-r--r--   0 root         (0) root         (0)     4105 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ita/ItaHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ita/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3550 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/jpn/WRIMEClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/kur/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/kur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/mkd/
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mkd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/mlt/
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mlt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/ToxicChatClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/nld/
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/nob/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nob/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/pol/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/pol/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/ron/
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/slk/
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/slk/SlovakSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/slk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/ssw/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ssw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/swe/
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/swe/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/swe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/tur/
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/uig/
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/uig/UyghurSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/uig/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/vie/
+-rw-r--r--   0 root         (0) root         (0)     3368 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Classification/zho/
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zho/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Classification/zul/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1319 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Clustering/deu/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/eng/
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/fra/
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/nob/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/nob/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/pol/
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/pol/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/rom/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/spa/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3917 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/swe/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/zho/
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/zho/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/InstructionRetrieval/
+-rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/PairClassification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/pol/
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/pol/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/zho/
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/Reranking/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/Reranking/fra/
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/fra/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/fra/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Reranking/zho/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/zho/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/code/
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/dan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/deu/
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.119770 mteb-1.7.9/mteb/tasks/Retrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.119770 mteb-1.7.9/mteb/tasks/Retrieval/est/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/est/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/est/estqa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/fra/
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/hun/
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/hun/HunSum2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/jpn/
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/kor/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/kor/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/nob/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/nob/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/pol/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/spa/
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/vie/
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/zho/
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      708 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/deu/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/eng/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/fin/
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fin/FinParaSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/fra/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fra/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/jpn/JSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/kor/
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/kor/KlueSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/kor/KorSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/pol/
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/pol/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/ron/
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/ron/RonSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/spa/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/spa/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/zho/
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/zho/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/Summarization/eng/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/Summarization/fra/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/fra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      288 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23583 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    36394 2024-04-23 07:43:09.000000 mteb-1.7.9/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-23 07:43:05.000000 mteb-1.7.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.059770 mteb-1.7.9/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/results/GritLM__GritLM-7B/
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-23 07:43:04.000000 mteb-1.7.9/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-04-23 07:43:04.000000 mteb-1.7.9/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.059770 mteb-1.7.9/results/dangvantuan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
+-rw-r--r--   0 root         (0) root         (0)      332 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      820 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SICKFr.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/STS22.json
+-rw-r--r--   0 root         (0) root         (0)      921 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.059770 mteb-1.7.9/results/intfloat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/intfloat/multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/SlovakSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/intfloat__e5-small/
+-rw-r--r--   0 root         (0) root         (0)      439 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small/TurkishProductSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/intfloat__e5-small-v2/
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.147770 mteb-1.7.9/results/intfloat__multilingual-e5-base/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.159770 mteb-1.7.9/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      827 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/GermanDPR.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/ItaHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7814 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7703 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      403 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)      298 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      304 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.159770 mteb-1.7.9/results/sentence-transformers/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/ToxicChatClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.163770 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SlovakSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.163770 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      302 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/model.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.179770 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      762 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      759 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      746 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
+-rw-r--r--   0 root         (0) root         (0)      610 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7839 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7915 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      736 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)    16669 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)    18247 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      741 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      294 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/medicalqaretrieval/
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/medicalqaretrieval/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/mteb_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.063770 mteb-1.7.9/scripts/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:43:09.191770 mteb-1.7.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_all_abstasks.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_mteb.py
+-rw-r--r--   0 root         (0) root         (0)      278 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_retrieval_abstask.py
```

### Comparing `mteb-1.7.8/LICENSE` & `mteb-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/PKG-INFO` & `mteb-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.7.8
+Version: 1.7.9
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.7.8/README.md` & `mteb-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/docs/mmteb/create_points_table.py` & `mteb-1.7.9/docs/mmteb/create_points_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/docs/mmteb/validate_points.py` & `mteb-1.7.9/docs/mmteb/validate_points.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/__init__.py` & `mteb-1.7.9/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTask.py` & `mteb-1.7.9/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskInstructionRetrieval.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskInstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.7.9/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/CrosslingualTask.py` & `mteb-1.7.9/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/LangMapping.py` & `mteb-1.7.9/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/MultilingualTask.py` & `mteb-1.7.9/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/TaskMetadata.py` & `mteb-1.7.9/mteb/abstasks/TaskMetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     "News",
     "Non-fiction",
     "Poetry",
     "Religious",
     "Reviews",
     "Social",
     "Spoken",
+    "Subtitles",
     "Web",
     "Programming",
 ]
 
 TEXT_CREATION_METHOD = Literal[
     "found",
     "created",
```

### Comparing `mteb-1.7.8/mteb/abstasks/iso_15924_to_script.json` & `mteb-1.7.9/mteb/abstasks/iso_15924_to_script.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/iso_639_3_to_language.json` & `mteb-1.7.9/mteb/abstasks/iso_639_3_to_language.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/abstasks/languages.py` & `mteb-1.7.9/mteb/abstasks/languages.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/cmd.py` & `mteb-1.7.9/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/MTEB.py` & `mteb-1.7.9/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.7.9/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/evaluation/evaluators/utils.py` & `mteb-1.7.9/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/logging.py` & `mteb-1.7.9/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/__init__.py` & `mteb-1.7.9/mteb/tasks/BitextMining/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py` & `mteb-1.7.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/__init__.py` & `mteb-1.7.9/mteb/tasks/Classification/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .ita.ItalianLinguistAcceptabilityClassification import *
 from .jpn.WRIMEClassification import *
 from .kur.KurdishSentimentClassification import *
 from .mkd.MacedonianTweetSentimentClassification import *
 from .mlt.MalteseSentimentClassification import *
 from .multilingual.AmazonCounterfactualClassification import *
 from .multilingual.AmazonReviewsClassification import *
+from .multilingual.IndicSentimentClassification import *
 from .multilingual.MasakhaNEWSClassification import *
 from .multilingual.MassiveIntentClassification import *
 from .multilingual.MassiveScenarioClassification import *
 from .multilingual.MTOPDomainClassification import *
 from .multilingual.MTOPIntentClassification import *
 from .multilingual.NordicLangClassification import *
 from .multilingual.ScalaClassification import *
```

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ara/TweetEmotionClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ara/TweetEmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ara/TweetSarcasmClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ara/TweetSarcasmClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/bam/BambaraSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/bam/BambaraSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py` & `mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/dan/DKHateClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/dan/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/dan/DalajClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/dan/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/dan/LccSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/dan/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ell/GreekSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ell/GreekSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/Banking77Classification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/EmotionClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/ImdbClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/NewsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/est/estonian_valence.py` & `mteb-1.7.9/mteb/tasks/Classification/est/estonian_valence.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/guj/GujaratiNewsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/guj/GujaratiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ita/ItaHateClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ita/ItaHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/jpn/WRIMEClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/jpn/WRIMEClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/kur/KurdishSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/kur/KurdishSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/multilingual/ToxicChatClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/multilingual/ToxicChatClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/nob/NoRecClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/nob/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/pol/PolishClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/pol/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ron/RomanianSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ron/RomanianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/slk/SlovakSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/slk/SlovakSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/swe/SweRecClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/swe/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/uig/UyghurSentimentClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/uig/UyghurSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/zho/CMTEBClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/zho/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py` & `mteb-1.7.9/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/__init__.py` & `mteb-1.7.9/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/BigPatentClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/RedditClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/nob/snl_clustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/nob/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/nob/vg_clustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/nob/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/pol/PolishClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/pol/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/rom/RomaniBibleClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/rom/RomaniBibleClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py` & `mteb-1.7.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py` & `mteb-1.7.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/swe/swedn_clustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/swe/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Clustering/zho/CMTEBClustering.py` & `mteb-1.7.9/mteb/tasks/Clustering/zho/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py` & `mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py` & `mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py` & `mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py` & `mteb-1.7.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py` & `mteb-1.7.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py` & `mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py` & `mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.7.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.7.9/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/pol/PolishPC.py` & `mteb-1.7.9/mteb/tasks/PairClassification/pol/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py` & `mteb-1.7.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py` & `mteb-1.7.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/eng/MindSmallReranking.py` & `mteb-1.7.9/mteb/tasks/Reranking/eng/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/eng/SciDocsReranking.py` & `mteb-1.7.9/mteb/tasks/Reranking/eng/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py` & `mteb-1.7.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/fra/AlloprofReranking.py` & `mteb-1.7.9/mteb/tasks/Reranking/fra/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/fra/SyntecReranking.py` & `mteb-1.7.9/mteb/tasks/Reranking/fra/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.7.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Reranking/zho/CMTEBReranking.py` & `mteb-1.7.9/mteb/tasks/Reranking/zho/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/__init__.py` & `mteb-1.7.9/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/dan/dan_fever.py` & `mteb-1.7.9/mteb/tasks/Retrieval/dan/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/dan/twitterhjerne.py` & `mteb-1.7.9/mteb/tasks/Retrieval/dan/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/NQRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/est/estqa.py` & `mteb-1.7.9/mteb/tasks/Retrieval/est/estqa.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/fra/FQuADRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/fra/FQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/hun/HunSum2.py` & `mteb-1.7.9/mteb/tasks/Retrieval/hun/HunSum2.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/kor/KoMiracl.py` & `mteb-1.7.9/mteb/tasks/Retrieval/kor/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py` & `mteb-1.7.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/nob/norquad.py` & `mteb-1.7.9/mteb/tasks/Retrieval/nob/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/nob/snl_retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/nob/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py` & `mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py` & `mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py` & `mteb-1.7.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/__init__.py` & `mteb-1.7.9/mteb/tasks/STS/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .eng.SickrSTS import *
 from .eng.STS12STS import *
 from .eng.STS13STS import *
 from .eng.STS14STS import *
 from .eng.STS15STS import *
 from .eng.STS16STS import *
 from .eng.STSBenchmarkSTS import *
+from .fin.FinParaSTS import *
 from .fra.SickFrSTS import *
 from .jpn.JSTS import *
 from .kor.KlueSTS import *
 from .kor.KorSTS import *
 from .multilingual.STS17CrosslingualSTS import *
 from .multilingual.STS22CrosslingualSTS import *
 from .multilingual.STSBenchmarkMultilingualSTS import *
```

### Comparing `mteb-1.7.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py` & `mteb-1.7.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/BiossesSTS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/STS12STS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/STS13STS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/STS14STS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/STS15STS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/STS16STS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/eng/SickrSTS.py` & `mteb-1.7.9/mteb/tasks/STS/eng/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/fra/SickFrSTS.py` & `mteb-1.7.9/mteb/tasks/STS/fra/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/jpn/JSTS.py` & `mteb-1.7.9/mteb/tasks/STS/jpn/JSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/kor/KlueSTS.py` & `mteb-1.7.9/mteb/tasks/STS/kor/KlueSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/kor/KorSTS.py` & `mteb-1.7.9/mteb/tasks/STS/kor/KorSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.7.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.7.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.7.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/pol/PolishSTS.py` & `mteb-1.7.9/mteb/tasks/STS/pol/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/ron/RonSTS.py` & `mteb-1.7.9/mteb/tasks/STS/ron/RonSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/spa/STSES.py` & `mteb-1.7.9/mteb/tasks/STS/spa/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/STS/zho/CMTEBSTS.py` & `mteb-1.7.9/mteb/tasks/STS/zho/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py` & `mteb-1.7.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py` & `mteb-1.7.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/mteb.egg-info/PKG-INFO` & `mteb-1.7.9/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.7.8
+Version: 1.7.9
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.7.8/mteb.egg-info/SOURCES.txt` & `mteb-1.7.9/mteb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 mteb/tasks/Classification/kur/__init__.py
 mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
 mteb/tasks/Classification/mkd/__init__.py
 mteb/tasks/Classification/mlt/MalteseSentimentClassification.py
 mteb/tasks/Classification/mlt/__init__.py
 mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
 mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
 mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
 mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
 mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
 mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
 mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
 mteb/tasks/Classification/multilingual/NordicLangClassification.py
 mteb/tasks/Classification/multilingual/ScalaClassification.py
@@ -340,14 +341,16 @@
 mteb/tasks/STS/eng/STS13STS.py
 mteb/tasks/STS/eng/STS14STS.py
 mteb/tasks/STS/eng/STS15STS.py
 mteb/tasks/STS/eng/STS16STS.py
 mteb/tasks/STS/eng/STSBenchmarkSTS.py
 mteb/tasks/STS/eng/SickrSTS.py
 mteb/tasks/STS/eng/__init__.py
+mteb/tasks/STS/fin/FinParaSTS.py
+mteb/tasks/STS/fin/__init__.py
 mteb/tasks/STS/fra/SickFrSTS.py
 mteb/tasks/STS/fra/__init__.py
 mteb/tasks/STS/jpn/JSTS.py
 mteb/tasks/STS/kor/KlueSTS.py
 mteb/tasks/STS/kor/KorSTS.py
 mteb/tasks/STS/kor/__init__.py
 mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
@@ -424,21 +427,23 @@
 results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
 results/intfloat__multilingual-e5-small/DanFEVER.json
 results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
 results/intfloat__multilingual-e5-small/EstQA.json
 results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
 results/intfloat__multilingual-e5-small/FQuADRetrieval.json
 results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
+results/intfloat__multilingual-e5-small/FinParaSTS.json
 results/intfloat__multilingual-e5-small/GermanDPR.json
 results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
 results/intfloat__multilingual-e5-small/GreekSentimentClassification.json
 results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
 results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
 results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
 results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
+results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
 results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
 results/intfloat__multilingual-e5-small/ItaHateClassification.json
 results/intfloat__multilingual-e5-small/Itacola.json
 results/intfloat__multilingual-e5-small/JSTS.json
 results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
 results/intfloat__multilingual-e5-small/KLUE-STS.json
 results/intfloat__multilingual-e5-small/KorSTS.json
@@ -516,22 +521,24 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaHateClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
```

### Comparing `mteb-1.7.8/pyproject.toml` & `mteb-1.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.7.8"
+version = "1.7.9"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.7.8/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json` & `mteb-1.7.9/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/GritLM__GritLM-7B/News21InstructionRetrieval.json` & `mteb-1.7.9/results/GritLM__GritLM-7B/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json` & `mteb-1.7.9/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/PawsX.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/SICKFr.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SICKFr.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json` & `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json` & `mteb-1.7.9/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__e5-small-v2/News21InstructionRetrieval.json` & `mteb-1.7.9/results/intfloat__e5-small-v2/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json` & `mteb-1.7.9/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/DanFEVER.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/EstQA.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/FQuADRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/GermanDPR.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/GermanDPR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/SyntecRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json` & `mteb-1.7.9/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MalteseSentimentClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MalteseSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json` & `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/amazon_polarity/create_data.py` & `mteb-1.7.9/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.7.9/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/arxiv/script_clustering.py` & `mteb-1.7.9/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/arxiv/script_raw.py` & `mteb-1.7.9/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/biorxiv/script_clustering.py` & `mteb-1.7.9/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/biorxiv/script_raw.py` & `mteb-1.7.9/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/bucc/create_data.py` & `mteb-1.7.9/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/create_task_table.py` & `mteb-1.7.9/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/germanquad/process_data.py` & `mteb-1.7.9/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/hal/create_data.py` & `mteb-1.7.9/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/imdb/create_data.py` & `mteb-1.7.9/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/medicalqaretrieval/create_data.py` & `mteb-1.7.9/scripts/data/medicalqaretrieval/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/medrxiv/script_clustering.py` & `mteb-1.7.9/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/medrxiv/script_raw.py` & `mteb-1.7.9/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/mind/prepare_data.py` & `mteb-1.7.9/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/redditp2p/script_clustering.py` & `mteb-1.7.9/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.7.9/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.7.9/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/summeval_fr/create_data.py` & `mteb-1.7.9/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.7.9/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/merge_cqadupstack.py` & `mteb-1.7.9/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/mteb_meta.py` & `mteb-1.7.9/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_chinese.py` & `mteb-1.7.9/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_english.py` & `mteb-1.7.9/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_french.py` & `mteb-1.7.9/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_german.py` & `mteb-1.7.9/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_korean.py` & `mteb-1.7.9/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_law.py` & `mteb-1.7.9/scripts/run_mteb_law.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/scripts/run_mteb_polish.py` & `mteb-1.7.9/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_ClusteringEvaluator.py` & `mteb-1.7.9/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_InstructionRetrievalEvaluator.py` & `mteb-1.7.9/tests/test_InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_PairClassificationEvaluator.py` & `mteb-1.7.9/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_RerankingEvaluator.py` & `mteb-1.7.9/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_RetrievalEvaluator.py` & `mteb-1.7.9/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_TaskMetadata.py` & `mteb-1.7.9/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_all_abstasks.py` & `mteb-1.7.9/tests/test_all_abstasks.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.8/tests/test_mteb.py` & `mteb-1.7.9/tests/test_mteb.py`

 * *Files identical despite different names*

