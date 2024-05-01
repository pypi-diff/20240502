# Comparing `tmp/edsl-0.1.8.tar.gz` & `tmp/edsl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsl-0.1.8.tar", max compression
+gzip compressed data, was "edsl-0.1.9.tar", max compression
```

## Comparing `edsl-0.1.8.tar` & `edsl-0.1.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     1111 2024-01-03 15:37:34.845191 edsl-0.1.8/LICENSE
--rw-r--r--   0        0        0     1051 2024-01-03 23:43:34.410352 edsl-0.1.8/README.md
--rw-r--r--   0        0        0     1530 2024-01-23 17:40:22.731315 edsl-0.1.8/edsl/Base.py
--rw-r--r--   0        0        0      495 2024-01-14 16:45:53.358228 edsl-0.1.8/edsl/__init__.py
--rw-r--r--   0        0        0     7959 2024-01-25 16:52:45.873529 edsl-0.1.8/edsl/agents/Agent.py
--rw-r--r--   0        0        0     1417 2024-01-18 23:19:35.876212 edsl-0.1.8/edsl/agents/AgentList.py
--rw-r--r--   0        0        0      689 2024-01-08 00:00:52.087576 edsl-0.1.8/edsl/agents/AgentListExportMixin.py
--rw-r--r--   0        0        0     8210 2024-01-25 16:52:45.873915 edsl-0.1.8/edsl/agents/Invigilator.py
--rw-r--r--   0        0        0       80 2024-01-03 15:37:34.845970 edsl-0.1.8/edsl/agents/__init__.py
--rw-r--r--   0        0        0     1420 2024-01-11 02:23:05.539848 edsl-0.1.8/edsl/agents/descriptors.py
--rw-r--r--   0        0        0       79 2024-01-03 15:37:34.846080 edsl-0.1.8/edsl/api/__init__.py
--rw-r--r--   0        0        0     2837 2024-01-04 17:00:43.494395 edsl-0.1.8/edsl/api/client.py
--rw-r--r--   0        0        0      339 2024-01-03 15:37:34.846218 edsl-0.1.8/edsl/api/jobs.py
--rw-r--r--   0        0        0      763 2024-01-03 15:37:34.846281 edsl-0.1.8/edsl/api/results.py
--rw-r--r--   0        0        0     5974 2024-01-24 21:25:06.567195 edsl-0.1.8/edsl/config.py
--rw-r--r--   0        0        0     1491 2024-01-03 15:37:34.846508 edsl-0.1.8/edsl/data/Database.py
--rw-r--r--   0        0        0      146 2024-01-03 15:37:34.846606 edsl-0.1.8/edsl/data/__init__.py
--rw-r--r--   0        0        0     3057 2024-01-09 17:15:38.961585 edsl-0.1.8/edsl/data/crud.py
--rw-r--r--   0        0        0     1103 2024-01-09 17:15:38.962209 edsl-0.1.8/edsl/data/orm.py
--rw-r--r--   0        0        0      205 2024-01-25 16:52:45.874054 edsl-0.1.8/edsl/data_transfer_models.py
--rw-r--r--   0        0        0     1102 2024-01-23 17:40:22.733076 edsl-0.1.8/edsl/enums.py
--rw-r--r--   0        0        0     1245 2024-01-18 23:19:17.965620 edsl-0.1.8/edsl/exceptions/__init__.py
--rw-r--r--   0        0        0      269 2024-01-03 15:37:34.847002 edsl-0.1.8/edsl/exceptions/agents.py
--rw-r--r--   0        0        0      351 2024-01-03 15:37:34.847083 edsl-0.1.8/edsl/exceptions/configuration.py
--rw-r--r--   0        0        0      152 2024-01-03 15:37:34.847160 edsl-0.1.8/edsl/exceptions/data.py
--rw-r--r--   0        0        0       81 2024-01-03 15:37:34.847239 edsl-0.1.8/edsl/exceptions/jobs.py
--rw-r--r--   0        0        0      351 2024-01-03 15:37:34.847316 edsl-0.1.8/edsl/exceptions/language_models.py
--rw-r--r--   0        0        0      247 2024-01-23 17:40:22.733654 edsl-0.1.8/edsl/exceptions/prompts.py
--rw-r--r--   0        0        0      534 2024-01-23 17:40:22.734108 edsl-0.1.8/edsl/exceptions/questions.py
--rw-r--r--   0        0        0      273 2024-01-09 17:15:38.963320 edsl-0.1.8/edsl/exceptions/results.py
--rw-r--r--   0        0        0      557 2024-01-03 15:37:34.847470 edsl-0.1.8/edsl/exceptions/surveys.py
--rw-r--r--   0        0        0      767 2024-01-13 23:05:38.398521 edsl-0.1.8/edsl/jobs/Answers.py
--rw-r--r--   0        0        0    10644 2024-01-27 02:26:29.139483 edsl-0.1.8/edsl/jobs/Interview.py
--rw-r--r--   0        0        0     9858 2024-01-25 16:52:45.874819 edsl-0.1.8/edsl/jobs/Jobs.py
--rw-r--r--   0        0        0     1805 2024-01-14 16:45:53.361075 edsl-0.1.8/edsl/jobs/JobsRunner.py
--rw-r--r--   0        0        0       32 2024-01-03 15:37:34.848276 edsl-0.1.8/edsl/jobs/__init__.py
--rw-r--r--   0        0        0     1333 2024-01-19 05:38:55.854396 edsl-0.1.8/edsl/jobs/base.py
--rw-r--r--   0        0        0     2755 2024-01-20 21:45:06.002110 edsl-0.1.8/edsl/jobs/runners/JobsRunnerAsyncio.py
--rw-r--r--   0        0        0      483 2024-01-14 16:45:53.363075 edsl-0.1.8/edsl/jobs/runners/JobsRunnerDryRun.py
--rw-r--r--   0        0        0     1684 2024-01-14 16:45:53.363647 edsl-0.1.8/edsl/jobs/runners/JobsRunnerStreaming.py
--rw-r--r--   0        0        0     2392 2024-01-23 17:40:22.734417 edsl-0.1.8/edsl/language_models/DeepInfra.py
--rw-r--r--   0        0        0    18818 2024-01-25 16:52:45.875233 edsl-0.1.8/edsl/language_models/LanguageModel.py
--rw-r--r--   0        0        0     2209 2024-01-23 17:40:22.735250 edsl-0.1.8/edsl/language_models/OpenAI.py
--rw-r--r--   0        0        0      419 2024-01-20 21:45:06.003037 edsl-0.1.8/edsl/language_models/__init__.py
--rw-r--r--   0        0        0     2319 2024-01-23 17:40:22.735781 edsl-0.1.8/edsl/language_models/model_interfaces/GeminiPro.py
--rw-r--r--   0        0        0      265 2024-01-23 17:40:22.736203 edsl-0.1.8/edsl/language_models/model_interfaces/LanguageModelOpenAIFour.py
--rw-r--r--   0        0        0      293 2024-01-23 17:40:22.736715 edsl-0.1.8/edsl/language_models/model_interfaces/LanguageModelOpenAIThreeFiveTurbo.py
--rw-r--r--   0        0        0      775 2024-01-23 17:40:22.737069 edsl-0.1.8/edsl/language_models/model_interfaces/LlamaTwo13B.py
--rw-r--r--   0        0        0      775 2024-01-23 17:40:22.737368 edsl-0.1.8/edsl/language_models/model_interfaces/LlamaTwo70B.py
--rw-r--r--   0        0        0      801 2024-01-23 17:40:22.737670 edsl-0.1.8/edsl/language_models/model_interfaces/Mixtral8x7B.py
--rw-r--r--   0        0        0        0 2024-01-20 21:45:06.003594 edsl-0.1.8/edsl/language_models/model_interfaces/__init__.py
--rw-r--r--   0        0        0     2597 2024-01-23 17:40:22.738142 edsl-0.1.8/edsl/language_models/registry.py
--rw-r--r--   0        0        0     2924 2024-01-23 17:40:22.738968 edsl-0.1.8/edsl/language_models/repair.py
--rw-r--r--   0        0        0      373 2024-01-03 15:37:34.848744 edsl-0.1.8/edsl/language_models/schemas.py
--rw-r--r--   0        0        0     3331 2024-01-23 17:40:22.739473 edsl-0.1.8/edsl/language_models/unused/ReplicateBase.py
--rw-r--r--   0        0        0     5232 2024-01-24 21:45:30.268871 edsl-0.1.8/edsl/prompts/Prompt.py
--rw-r--r--   0        0        0      200 2024-01-18 23:19:35.880541 edsl-0.1.8/edsl/prompts/QuestionInstructionsBase.py
--rw-r--r--   0        0        0       85 2024-01-18 23:19:35.880936 edsl-0.1.8/edsl/prompts/__init__.py
--rw-r--r--   0        0        0      846 2024-01-24 21:45:30.269340 edsl-0.1.8/edsl/prompts/library/agent_instructions.py
--rw-r--r--   0        0        0      430 2024-01-24 21:45:30.269578 edsl-0.1.8/edsl/prompts/library/agent_persona.py
--rw-r--r--   0        0        0     1112 2024-01-19 19:50:28.035229 edsl-0.1.8/edsl/prompts/library/question_budget.py
--rw-r--r--   0        0        0     1364 2024-01-18 23:19:35.881471 edsl-0.1.8/edsl/prompts/library/question_checkbox.py
--rw-r--r--   0        0        0      711 2024-01-18 23:19:35.881630 edsl-0.1.8/edsl/prompts/library/question_extract.py
--rw-r--r--   0        0        0      442 2024-01-18 23:19:35.881911 edsl-0.1.8/edsl/prompts/library/question_freetext.py
--rw-r--r--   0        0        0      704 2024-01-18 23:19:35.882074 edsl-0.1.8/edsl/prompts/library/question_linear_scale.py
--rw-r--r--   0        0        0      638 2024-01-18 23:19:35.882246 edsl-0.1.8/edsl/prompts/library/question_list.py
--rw-r--r--   0        0        0     1424 2024-01-18 23:19:35.882420 edsl-0.1.8/edsl/prompts/library/question_multiple_choice.py
--rw-r--r--   0        0        0     1388 2024-01-18 23:19:35.882588 edsl-0.1.8/edsl/prompts/library/question_numerical.py
--rw-r--r--   0        0        0      824 2024-01-18 23:19:35.882770 edsl-0.1.8/edsl/prompts/library/question_rank.py
--rw-r--r--   0        0        0      843 2024-01-24 21:45:30.270265 edsl-0.1.8/edsl/prompts/prompt_config.py
--rw-r--r--   0        0        0     7651 2024-01-23 17:40:22.741094 edsl-0.1.8/edsl/prompts/registry.py
--rw-r--r--   0        0        0    10746 2024-01-17 22:50:54.115721 edsl-0.1.8/edsl/questions/AnswerValidatorMixin.py
--rw-r--r--   0        0        0     7671 2024-01-23 17:40:22.741503 edsl-0.1.8/edsl/questions/Question.py
--rw-r--r--   0        0        0     4659 2024-01-19 19:50:28.036746 edsl-0.1.8/edsl/questions/QuestionBudget.py
--rw-r--r--   0        0        0     5110 2024-01-17 22:50:54.116498 edsl-0.1.8/edsl/questions/QuestionCheckBox.py
--rw-r--r--   0        0        0     3229 2024-01-19 19:50:28.037358 edsl-0.1.8/edsl/questions/QuestionExtract.py
--rw-r--r--   0        0        0     3041 2024-01-17 22:50:54.117003 edsl-0.1.8/edsl/questions/QuestionFreeText.py
--rw-r--r--   0        0        0     2842 2024-01-17 22:50:54.117248 edsl-0.1.8/edsl/questions/QuestionFunctional.py
--rw-r--r--   0        0        0     3349 2024-01-17 22:50:54.117495 edsl-0.1.8/edsl/questions/QuestionList.py
--rw-r--r--   0        0        0     3678 2024-01-17 22:50:54.117828 edsl-0.1.8/edsl/questions/QuestionMultipleChoice.py
--rw-r--r--   0        0        0     3176 2024-01-17 22:50:54.118137 edsl-0.1.8/edsl/questions/QuestionNumerical.py
--rw-r--r--   0        0        0     4170 2024-01-17 22:50:54.118434 edsl-0.1.8/edsl/questions/QuestionRank.py
--rw-r--r--   0        0        0     1074 2024-01-12 21:55:58.392318 edsl-0.1.8/edsl/questions/__init__.py
--rw-r--r--   0        0        0     3087 2024-01-04 17:08:52.176616 edsl-0.1.8/edsl/questions/compose_questions.py
--rw-r--r--   0        0        0     2535 2024-01-17 22:50:54.118745 edsl-0.1.8/edsl/questions/derived/QuestionLikertFive.py
--rw-r--r--   0        0        0     2787 2024-01-17 22:50:54.119037 edsl-0.1.8/edsl/questions/derived/QuestionLinearScale.py
--rw-r--r--   0        0        0     3049 2024-01-17 22:50:54.119305 edsl-0.1.8/edsl/questions/derived/QuestionTopK.py
--rw-r--r--   0        0        0     2308 2024-01-17 22:50:54.119622 edsl-0.1.8/edsl/questions/derived/QuestionYesNo.py
--rw-r--r--   0        0        0        0 2024-01-03 15:37:34.850375 edsl-0.1.8/edsl/questions/derived/__init__.py
--rw-r--r--   0        0        0    12187 2024-01-18 23:19:35.883698 edsl-0.1.8/edsl/questions/descriptors.py
--rw-r--r--   0        0        0     3445 2024-01-18 23:19:17.967746 edsl-0.1.8/edsl/questions/question_registry.py
--rw-r--r--   0        0        0      246 2024-01-12 21:55:58.396865 edsl-0.1.8/edsl/questions/settings.py
--rw-r--r--   0        0        0     3276 2024-01-03 15:37:34.851630 edsl-0.1.8/edsl/report/InputOutputDataTypes.py
--rw-r--r--   0        0        0     1024 2024-01-17 23:32:25.039981 edsl-0.1.8/edsl/report/RegressionMixin.py
--rw-r--r--   0        0        0    39798 2024-01-17 23:32:25.050563 edsl-0.1.8/edsl/report/ReportOutputs.py
--rw-r--r--   0        0        0     3301 2024-01-17 23:32:25.050896 edsl-0.1.8/edsl/report/ResultsFetchMixin.py
--rw-r--r--   0        0        0      671 2024-01-17 23:32:25.040238 edsl-0.1.8/edsl/report/ResultsOutputMixin.py
--rw-r--r--   0        0        0        0 2024-01-03 15:37:34.851820 edsl-0.1.8/edsl/report/__init__.py
--rw-r--r--   0        0        0   311272 2024-01-03 15:37:34.852270 edsl-0.1.8/edsl/report/demo.ipynb
--rw-r--r--   0        0        0     2036 2024-01-09 17:15:38.968079 edsl-0.1.8/edsl/results/Dataset.py
--rw-r--r--   0        0        0     5415 2024-01-18 23:19:35.884148 edsl-0.1.8/edsl/results/Result.py
--rw-r--r--   0        0        0    15288 2024-01-18 23:19:35.884774 edsl-0.1.8/edsl/results/Results.py
--rw-r--r--   0        0        0     4543 2024-01-26 21:21:24.498261 edsl-0.1.8/edsl/results/ResultsExportMixin.py
--rw-r--r--   0        0        0       80 2024-01-03 15:37:34.852914 edsl-0.1.8/edsl/results/__init__.py
--rw-r--r--   0        0        0     4076 2024-01-13 16:43:04.406628 edsl-0.1.8/edsl/scenarios/Scenario.py
--rw-r--r--   0        0        0     2256 2024-01-13 16:43:04.407036 edsl-0.1.8/edsl/scenarios/ScenarioList.py
--rw-r--r--   0        0        0       45 2024-01-03 15:37:34.853172 edsl-0.1.8/edsl/scenarios/__init__.py
--rw-r--r--   0        0        0     1965 2024-01-26 21:21:24.498857 edsl-0.1.8/edsl/surveys/DAG.py
--rw-r--r--   0        0        0      745 2024-01-12 21:58:43.442258 edsl-0.1.8/edsl/surveys/Memory.py
--rw-r--r--   0        0        0     4832 2024-01-26 21:21:24.499380 edsl-0.1.8/edsl/surveys/MemoryPlan.py
--rw-r--r--   0        0        0     7048 2024-01-26 21:21:24.499976 edsl-0.1.8/edsl/surveys/Rule.py
--rw-r--r--   0        0        0     7678 2024-01-26 21:21:24.500556 edsl-0.1.8/edsl/surveys/RuleCollection.py
--rw-r--r--   0        0        0    18990 2024-01-26 21:21:24.501124 edsl-0.1.8/edsl/surveys/Survey.py
--rw-r--r--   0        0        0     2828 2024-01-08 00:00:52.088759 edsl-0.1.8/edsl/surveys/SurveyExportMixin.py
--rw-r--r--   0        0        0      129 2024-01-13 23:05:38.400739 edsl-0.1.8/edsl/surveys/__init__.py
--rw-r--r--   0        0        0      310 2024-01-12 21:55:58.398332 edsl-0.1.8/edsl/surveys/base.py
--rw-r--r--   0        0        0     1634 2024-01-12 21:55:58.399015 edsl-0.1.8/edsl/surveys/descriptors.py
--rw-r--r--   0        0        0     3032 2024-01-03 15:37:34.853757 edsl-0.1.8/edsl/trackers/Tracker.py
--rw-r--r--   0        0        0     6602 2024-01-03 15:37:34.853876 edsl-0.1.8/edsl/trackers/TrackerAPI.py
--rw-r--r--   0        0        0     2406 2024-01-03 15:37:34.853944 edsl-0.1.8/edsl/trackers/TrackerTasks.py
--rw-r--r--   0        0        0        0 2024-01-03 15:37:34.853970 edsl-0.1.8/edsl/trackers/__init__.py
--rw-r--r--   0        0        0      470 2024-01-17 23:32:25.052089 edsl-0.1.8/edsl/utilities/__init__.py
--rw-r--r--   0        0        0      730 2024-01-03 15:37:34.854146 edsl-0.1.8/edsl/utilities/ast_utilities.py
--rw-r--r--   0        0        0      122 2024-01-09 17:15:38.972776 edsl-0.1.8/edsl/utilities/data/Registry.py
--rw-r--r--   0        0        0       62 2024-01-09 17:15:38.973272 edsl-0.1.8/edsl/utilities/data/__init__.py
--rw-r--r--   0        0        0   250944 2024-01-03 15:37:34.854670 edsl-0.1.8/edsl/utilities/data/scooter_results.json
--rw-r--r--   0        0        0     1134 2024-01-20 21:45:06.005131 edsl-0.1.8/edsl/utilities/decorators.py
--rw-r--r--   0        0        0    11997 2024-01-26 21:21:24.501822 edsl-0.1.8/edsl/utilities/interface.py
--rw-r--r--   0        0        0     7152 2024-01-11 02:23:05.551425 edsl-0.1.8/edsl/utilities/utilities.py
--rw-r--r--   0        0        0     1953 2024-01-27 02:26:29.139900 edsl-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 edsl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-01-03 15:37:34.845191 edsl-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1051 2024-01-03 23:43:34.410352 edsl-0.1.9/README.md
+-rw-r--r--   0        0        0     2018 2024-01-27 21:34:57.543104 edsl-0.1.9/edsl/Base.py
+-rw-r--r--   0        0        0      495 2024-01-14 16:45:53.358228 edsl-0.1.9/edsl/__init__.py
+-rw-r--r--   0        0        0    10855 2024-01-27 21:34:57.543510 edsl-0.1.9/edsl/agents/Agent.py
+-rw-r--r--   0        0        0     1417 2024-01-18 23:19:35.876212 edsl-0.1.9/edsl/agents/AgentList.py
+-rw-r--r--   0        0        0      689 2024-01-08 00:00:52.087576 edsl-0.1.9/edsl/agents/AgentListExportMixin.py
+-rw-r--r--   0        0        0     8211 2024-01-27 21:34:57.543861 edsl-0.1.9/edsl/agents/Invigilator.py
+-rw-r--r--   0        0        0       80 2024-01-03 15:37:34.845970 edsl-0.1.9/edsl/agents/__init__.py
+-rw-r--r--   0        0        0     1420 2024-01-11 02:23:05.539848 edsl-0.1.9/edsl/agents/descriptors.py
+-rw-r--r--   0        0        0       79 2024-01-03 15:37:34.846080 edsl-0.1.9/edsl/api/__init__.py
+-rw-r--r--   0        0        0     2837 2024-01-04 17:00:43.494395 edsl-0.1.9/edsl/api/client.py
+-rw-r--r--   0        0        0      339 2024-01-03 15:37:34.846218 edsl-0.1.9/edsl/api/jobs.py
+-rw-r--r--   0        0        0      763 2024-01-03 15:37:34.846281 edsl-0.1.9/edsl/api/results.py
+-rw-r--r--   0        0        0     5974 2024-01-24 21:25:06.567195 edsl-0.1.9/edsl/config.py
+-rw-r--r--   0        0        0     1491 2024-01-03 15:37:34.846508 edsl-0.1.9/edsl/data/Database.py
+-rw-r--r--   0        0        0      146 2024-01-03 15:37:34.846606 edsl-0.1.9/edsl/data/__init__.py
+-rw-r--r--   0        0        0     3057 2024-01-09 17:15:38.961585 edsl-0.1.9/edsl/data/crud.py
+-rw-r--r--   0        0        0     1103 2024-01-09 17:15:38.962209 edsl-0.1.9/edsl/data/orm.py
+-rw-r--r--   0        0        0      205 2024-01-25 16:52:45.874054 edsl-0.1.9/edsl/data_transfer_models.py
+-rw-r--r--   0        0        0     1102 2024-01-23 17:40:22.733076 edsl-0.1.9/edsl/enums.py
+-rw-r--r--   0        0        0     1245 2024-01-18 23:19:17.965620 edsl-0.1.9/edsl/exceptions/__init__.py
+-rw-r--r--   0        0        0      394 2024-01-27 21:34:57.544146 edsl-0.1.9/edsl/exceptions/agents.py
+-rw-r--r--   0        0        0      351 2024-01-03 15:37:34.847083 edsl-0.1.9/edsl/exceptions/configuration.py
+-rw-r--r--   0        0        0      152 2024-01-03 15:37:34.847160 edsl-0.1.9/edsl/exceptions/data.py
+-rw-r--r--   0        0        0       81 2024-01-03 15:37:34.847239 edsl-0.1.9/edsl/exceptions/jobs.py
+-rw-r--r--   0        0        0      351 2024-01-03 15:37:34.847316 edsl-0.1.9/edsl/exceptions/language_models.py
+-rw-r--r--   0        0        0      247 2024-01-23 17:40:22.733654 edsl-0.1.9/edsl/exceptions/prompts.py
+-rw-r--r--   0        0        0      534 2024-01-23 17:40:22.734108 edsl-0.1.9/edsl/exceptions/questions.py
+-rw-r--r--   0        0        0      273 2024-01-09 17:15:38.963320 edsl-0.1.9/edsl/exceptions/results.py
+-rw-r--r--   0        0        0      557 2024-01-03 15:37:34.847470 edsl-0.1.9/edsl/exceptions/surveys.py
+-rw-r--r--   0        0        0      767 2024-01-13 23:05:38.398521 edsl-0.1.9/edsl/jobs/Answers.py
+-rw-r--r--   0        0        0    10644 2024-01-27 02:26:29.139483 edsl-0.1.9/edsl/jobs/Interview.py
+-rw-r--r--   0        0        0    10873 2024-01-27 21:34:57.544685 edsl-0.1.9/edsl/jobs/Jobs.py
+-rw-r--r--   0        0        0     1805 2024-01-14 16:45:53.361075 edsl-0.1.9/edsl/jobs/JobsRunner.py
+-rw-r--r--   0        0        0       32 2024-01-03 15:37:34.848276 edsl-0.1.9/edsl/jobs/__init__.py
+-rw-r--r--   0        0        0     1333 2024-01-19 05:38:55.854396 edsl-0.1.9/edsl/jobs/base.py
+-rw-r--r--   0        0        0     2755 2024-01-20 21:45:06.002110 edsl-0.1.9/edsl/jobs/runners/JobsRunnerAsyncio.py
+-rw-r--r--   0        0        0      483 2024-01-14 16:45:53.363075 edsl-0.1.9/edsl/jobs/runners/JobsRunnerDryRun.py
+-rw-r--r--   0        0        0     1684 2024-01-14 16:45:53.363647 edsl-0.1.9/edsl/jobs/runners/JobsRunnerStreaming.py
+-rw-r--r--   0        0        0     2392 2024-01-23 17:40:22.734417 edsl-0.1.9/edsl/language_models/DeepInfra.py
+-rw-r--r--   0        0        0    18818 2024-01-25 16:52:45.875233 edsl-0.1.9/edsl/language_models/LanguageModel.py
+-rw-r--r--   0        0        0     2209 2024-01-23 17:40:22.735250 edsl-0.1.9/edsl/language_models/OpenAI.py
+-rw-r--r--   0        0        0      419 2024-01-20 21:45:06.003037 edsl-0.1.9/edsl/language_models/__init__.py
+-rw-r--r--   0        0        0     2319 2024-01-23 17:40:22.735781 edsl-0.1.9/edsl/language_models/model_interfaces/GeminiPro.py
+-rw-r--r--   0        0        0      265 2024-01-23 17:40:22.736203 edsl-0.1.9/edsl/language_models/model_interfaces/LanguageModelOpenAIFour.py
+-rw-r--r--   0        0        0      293 2024-01-23 17:40:22.736715 edsl-0.1.9/edsl/language_models/model_interfaces/LanguageModelOpenAIThreeFiveTurbo.py
+-rw-r--r--   0        0        0      775 2024-01-23 17:40:22.737069 edsl-0.1.9/edsl/language_models/model_interfaces/LlamaTwo13B.py
+-rw-r--r--   0        0        0      775 2024-01-23 17:40:22.737368 edsl-0.1.9/edsl/language_models/model_interfaces/LlamaTwo70B.py
+-rw-r--r--   0        0        0      801 2024-01-23 17:40:22.737670 edsl-0.1.9/edsl/language_models/model_interfaces/Mixtral8x7B.py
+-rw-r--r--   0        0        0        0 2024-01-20 21:45:06.003594 edsl-0.1.9/edsl/language_models/model_interfaces/__init__.py
+-rw-r--r--   0        0        0     2597 2024-01-23 17:40:22.738142 edsl-0.1.9/edsl/language_models/registry.py
+-rw-r--r--   0        0        0     2924 2024-01-23 17:40:22.738968 edsl-0.1.9/edsl/language_models/repair.py
+-rw-r--r--   0        0        0      373 2024-01-03 15:37:34.848744 edsl-0.1.9/edsl/language_models/schemas.py
+-rw-r--r--   0        0        0     3331 2024-01-23 17:40:22.739473 edsl-0.1.9/edsl/language_models/unused/ReplicateBase.py
+-rw-r--r--   0        0        0     5232 2024-01-24 21:45:30.268871 edsl-0.1.9/edsl/prompts/Prompt.py
+-rw-r--r--   0        0        0      200 2024-01-18 23:19:35.880541 edsl-0.1.9/edsl/prompts/QuestionInstructionsBase.py
+-rw-r--r--   0        0        0       85 2024-01-18 23:19:35.880936 edsl-0.1.9/edsl/prompts/__init__.py
+-rw-r--r--   0        0        0      846 2024-01-24 21:45:30.269340 edsl-0.1.9/edsl/prompts/library/agent_instructions.py
+-rw-r--r--   0        0        0      430 2024-01-24 21:45:30.269578 edsl-0.1.9/edsl/prompts/library/agent_persona.py
+-rw-r--r--   0        0        0     1112 2024-01-19 19:50:28.035229 edsl-0.1.9/edsl/prompts/library/question_budget.py
+-rw-r--r--   0        0        0     1364 2024-01-18 23:19:35.881471 edsl-0.1.9/edsl/prompts/library/question_checkbox.py
+-rw-r--r--   0        0        0      711 2024-01-18 23:19:35.881630 edsl-0.1.9/edsl/prompts/library/question_extract.py
+-rw-r--r--   0        0        0      442 2024-01-18 23:19:35.881911 edsl-0.1.9/edsl/prompts/library/question_freetext.py
+-rw-r--r--   0        0        0      704 2024-01-18 23:19:35.882074 edsl-0.1.9/edsl/prompts/library/question_linear_scale.py
+-rw-r--r--   0        0        0      638 2024-01-18 23:19:35.882246 edsl-0.1.9/edsl/prompts/library/question_list.py
+-rw-r--r--   0        0        0     1424 2024-01-18 23:19:35.882420 edsl-0.1.9/edsl/prompts/library/question_multiple_choice.py
+-rw-r--r--   0        0        0     1388 2024-01-18 23:19:35.882588 edsl-0.1.9/edsl/prompts/library/question_numerical.py
+-rw-r--r--   0        0        0      824 2024-01-18 23:19:35.882770 edsl-0.1.9/edsl/prompts/library/question_rank.py
+-rw-r--r--   0        0        0      843 2024-01-24 21:45:30.270265 edsl-0.1.9/edsl/prompts/prompt_config.py
+-rw-r--r--   0        0        0     7651 2024-01-23 17:40:22.741094 edsl-0.1.9/edsl/prompts/registry.py
+-rw-r--r--   0        0        0    10746 2024-01-17 22:50:54.115721 edsl-0.1.9/edsl/questions/AnswerValidatorMixin.py
+-rw-r--r--   0        0        0     7671 2024-01-23 17:40:22.741503 edsl-0.1.9/edsl/questions/Question.py
+-rw-r--r--   0        0        0     4659 2024-01-19 19:50:28.036746 edsl-0.1.9/edsl/questions/QuestionBudget.py
+-rw-r--r--   0        0        0     5110 2024-01-17 22:50:54.116498 edsl-0.1.9/edsl/questions/QuestionCheckBox.py
+-rw-r--r--   0        0        0     3229 2024-01-19 19:50:28.037358 edsl-0.1.9/edsl/questions/QuestionExtract.py
+-rw-r--r--   0        0        0     3041 2024-01-17 22:50:54.117003 edsl-0.1.9/edsl/questions/QuestionFreeText.py
+-rw-r--r--   0        0        0     2842 2024-01-17 22:50:54.117248 edsl-0.1.9/edsl/questions/QuestionFunctional.py
+-rw-r--r--   0        0        0     3349 2024-01-17 22:50:54.117495 edsl-0.1.9/edsl/questions/QuestionList.py
+-rw-r--r--   0        0        0     3678 2024-01-17 22:50:54.117828 edsl-0.1.9/edsl/questions/QuestionMultipleChoice.py
+-rw-r--r--   0        0        0     3176 2024-01-17 22:50:54.118137 edsl-0.1.9/edsl/questions/QuestionNumerical.py
+-rw-r--r--   0        0        0     4170 2024-01-17 22:50:54.118434 edsl-0.1.9/edsl/questions/QuestionRank.py
+-rw-r--r--   0        0        0     1074 2024-01-12 21:55:58.392318 edsl-0.1.9/edsl/questions/__init__.py
+-rw-r--r--   0        0        0     3087 2024-01-04 17:08:52.176616 edsl-0.1.9/edsl/questions/compose_questions.py
+-rw-r--r--   0        0        0     2535 2024-01-17 22:50:54.118745 edsl-0.1.9/edsl/questions/derived/QuestionLikertFive.py
+-rw-r--r--   0        0        0     2787 2024-01-17 22:50:54.119037 edsl-0.1.9/edsl/questions/derived/QuestionLinearScale.py
+-rw-r--r--   0        0        0     3049 2024-01-17 22:50:54.119305 edsl-0.1.9/edsl/questions/derived/QuestionTopK.py
+-rw-r--r--   0        0        0     2308 2024-01-17 22:50:54.119622 edsl-0.1.9/edsl/questions/derived/QuestionYesNo.py
+-rw-r--r--   0        0        0        0 2024-01-03 15:37:34.850375 edsl-0.1.9/edsl/questions/derived/__init__.py
+-rw-r--r--   0        0        0    12256 2024-01-27 21:34:57.545050 edsl-0.1.9/edsl/questions/descriptors.py
+-rw-r--r--   0        0        0     3445 2024-01-18 23:19:17.967746 edsl-0.1.9/edsl/questions/question_registry.py
+-rw-r--r--   0        0        0      246 2024-01-12 21:55:58.396865 edsl-0.1.9/edsl/questions/settings.py
+-rw-r--r--   0        0        0     3276 2024-01-03 15:37:34.851630 edsl-0.1.9/edsl/report/InputOutputDataTypes.py
+-rw-r--r--   0        0        0     1024 2024-01-17 23:32:25.039981 edsl-0.1.9/edsl/report/RegressionMixin.py
+-rw-r--r--   0        0        0    39798 2024-01-17 23:32:25.050563 edsl-0.1.9/edsl/report/ReportOutputs.py
+-rw-r--r--   0        0        0     3464 2024-01-27 21:34:57.545324 edsl-0.1.9/edsl/report/ResultsFetchMixin.py
+-rw-r--r--   0        0        0      671 2024-01-17 23:32:25.040238 edsl-0.1.9/edsl/report/ResultsOutputMixin.py
+-rw-r--r--   0        0        0        0 2024-01-03 15:37:34.851820 edsl-0.1.9/edsl/report/__init__.py
+-rw-r--r--   0        0        0   311272 2024-01-03 15:37:34.852270 edsl-0.1.9/edsl/report/demo.ipynb
+-rw-r--r--   0        0        0     2036 2024-01-09 17:15:38.968079 edsl-0.1.9/edsl/results/Dataset.py
+-rw-r--r--   0        0        0     5415 2024-01-18 23:19:35.884148 edsl-0.1.9/edsl/results/Result.py
+-rw-r--r--   0        0        0    15629 2024-01-27 21:34:57.545674 edsl-0.1.9/edsl/results/Results.py
+-rw-r--r--   0        0        0     4477 2024-01-27 21:34:57.546102 edsl-0.1.9/edsl/results/ResultsExportMixin.py
+-rw-r--r--   0        0        0       80 2024-01-03 15:37:34.852914 edsl-0.1.9/edsl/results/__init__.py
+-rw-r--r--   0        0        0     4076 2024-01-13 16:43:04.406628 edsl-0.1.9/edsl/scenarios/Scenario.py
+-rw-r--r--   0        0        0     2256 2024-01-13 16:43:04.407036 edsl-0.1.9/edsl/scenarios/ScenarioList.py
+-rw-r--r--   0        0        0       45 2024-01-03 15:37:34.853172 edsl-0.1.9/edsl/scenarios/__init__.py
+-rw-r--r--   0        0        0     1965 2024-01-26 21:21:24.498857 edsl-0.1.9/edsl/surveys/DAG.py
+-rw-r--r--   0        0        0      745 2024-01-12 21:58:43.442258 edsl-0.1.9/edsl/surveys/Memory.py
+-rw-r--r--   0        0        0     4832 2024-01-26 21:21:24.499380 edsl-0.1.9/edsl/surveys/MemoryPlan.py
+-rw-r--r--   0        0        0     7012 2024-01-27 21:34:57.546478 edsl-0.1.9/edsl/surveys/Rule.py
+-rw-r--r--   0        0        0     7651 2024-01-27 21:34:57.546840 edsl-0.1.9/edsl/surveys/RuleCollection.py
+-rw-r--r--   0        0        0    19465 2024-01-27 21:34:57.547354 edsl-0.1.9/edsl/surveys/Survey.py
+-rw-r--r--   0        0        0     2828 2024-01-08 00:00:52.088759 edsl-0.1.9/edsl/surveys/SurveyExportMixin.py
+-rw-r--r--   0        0        0      129 2024-01-13 23:05:38.400739 edsl-0.1.9/edsl/surveys/__init__.py
+-rw-r--r--   0        0        0      633 2024-01-27 21:34:57.547789 edsl-0.1.9/edsl/surveys/base.py
+-rw-r--r--   0        0        0     1634 2024-01-12 21:55:58.399015 edsl-0.1.9/edsl/surveys/descriptors.py
+-rw-r--r--   0        0        0     3032 2024-01-03 15:37:34.853757 edsl-0.1.9/edsl/trackers/Tracker.py
+-rw-r--r--   0        0        0     6602 2024-01-03 15:37:34.853876 edsl-0.1.9/edsl/trackers/TrackerAPI.py
+-rw-r--r--   0        0        0     2406 2024-01-03 15:37:34.853944 edsl-0.1.9/edsl/trackers/TrackerTasks.py
+-rw-r--r--   0        0        0        0 2024-01-03 15:37:34.853970 edsl-0.1.9/edsl/trackers/__init__.py
+-rw-r--r--   0        0        0      470 2024-01-17 23:32:25.052089 edsl-0.1.9/edsl/utilities/__init__.py
+-rw-r--r--   0        0        0      730 2024-01-03 15:37:34.854146 edsl-0.1.9/edsl/utilities/ast_utilities.py
+-rw-r--r--   0        0        0      122 2024-01-09 17:15:38.972776 edsl-0.1.9/edsl/utilities/data/Registry.py
+-rw-r--r--   0        0        0       62 2024-01-09 17:15:38.973272 edsl-0.1.9/edsl/utilities/data/__init__.py
+-rw-r--r--   0        0        0   250944 2024-01-03 15:37:34.854670 edsl-0.1.9/edsl/utilities/data/scooter_results.json
+-rw-r--r--   0        0        0     1134 2024-01-20 21:45:06.005131 edsl-0.1.9/edsl/utilities/decorators.py
+-rw-r--r--   0        0        0    11997 2024-01-26 21:21:24.501822 edsl-0.1.9/edsl/utilities/interface.py
+-rw-r--r--   0        0        0     7152 2024-01-11 02:23:05.551425 edsl-0.1.9/edsl/utilities/utilities.py
+-rw-r--r--   0        0        0     1734 2024-01-27 21:34:57.549677 edsl-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 edsl-0.1.9/PKG-INFO
```

### Comparing `edsl-0.1.8/LICENSE` & `edsl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/README.md` & `edsl-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/agents/Agent.py` & `edsl-0.1.9/edsl/agents/Agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from __future__ import annotations
 import copy
+import inspect
+import types
 from typing import Any, Callable, Optional, Union, Dict
 
 from edsl.Base import Base
 
-from edsl.exceptions import AgentCombinationError
+from edsl.exceptions.agents import (
+    AgentCombinationError,
+    AgentDirectAnswerFunctionError,
+    AgentDynamicTraitsFunctionError,
+)
 
 from edsl.agents.Invigilator import (
     InvigilatorDebug,
     InvigilatorHuman,
     InvigilatorFunctional,
     InvigilatorAI,
 )
 
-from edsl.language_models import LanguageModel, LanguageModelOpenAIThreeFiveTurbo
+# from edsl.language_models import LanguageModel, LanguageModelOpenAIThreeFiveTurbo
+from edsl.language_models.registry import Model
 from edsl.scenarios import Scenario
 from edsl.utilities import (
     dict_to_html,
     print_dict_as_html_table,
     print_dict_with_rich,
 )
 
@@ -29,31 +36,86 @@
 
 from edsl.utilities.decorators import sync_wrapper
 
 from edsl.data_transfer_models import AgentResponseDict
 
 
 class Agent(Base):
-    """An agent answers questions."""
+    """An agent that can answer questions.
+
+    Parameters
+    ----------
+    traits : dict, optional - A dictionary of traits that the agent has. The keys need to be
+    valid python variable names. The values can be any python object that has a valid __str__ method.
+    codebook : dict, optional - A codebook mapping trait keys to trait descriptions.
+    instruction : str, optional - Instructions for the agent.
+
+    dynamic_traits_function : Callable, optional - A function that returns a dictionary of traits.
+
+    """
 
     default_instruction = """You are answering questions as if you were a human. Do not break character."""
 
     traits = TraitsDescriptor()
     codebook = CodebookDescriptor()
     instruction = InstructionDescriptor()
 
     def __init__(
         self,
         traits: dict = None,
         codebook: dict = None,
         instruction: str = None,
+        dynamic_traits_function: Callable = None,
     ):
-        self.traits = traits or dict()
+        self._traits = traits or dict()
         self.codebook = codebook or dict()
         self.instruction = instruction or self.default_instruction
+        self.dynamic_traits_function = dynamic_traits_function
+        self._check_dynamic_traits_function()
+        self.current_question = None
+
+    def _check_dynamic_traits_function(self):
+        if self.dynamic_traits_function:
+            sig = inspect.signature(self.dynamic_traits_function)
+            if "question" in sig.parameters:
+                if len(sig.parameters) > 1:
+                    raise AgentDynamicTraitsFunctionError(
+                        f"The dynamic traits function {self.dynamic_traits_function} has too many parameters. It should only have one parameter: 'question'."
+                    )
+            else:
+                if len(sig.parameters) > 0:
+                    raise AgentDynamicTraitsFunctionError(
+                        f"""The dynamic traits function {self.dynamic_traits_function} has too many parameters. It should have no parameters or 
+                        just a single parameter: 'question'."""
+                    )
+
+    @property
+    def traits(self):
+        if self.dynamic_traits_function:
+            sig = inspect.signature(self.dynamic_traits_function)
+            if "question" in sig.parameters:
+                return self.dynamic_traits_function(question=self.current_question)
+            else:
+                return self.dynamic_traits_function()
+        else:
+            return self._traits
+
+    def add_direct_question_answering_method(self, method: Callable):
+        """Adds a method to the agent that can answer a particular question type."""
+        if hasattr(self, "answer_question_directly"):
+            print("Warning: overwriting existing answer_question_directly method")
+
+        signature = inspect.signature(method)
+        for argument in ["question", "scenario", "self"]:
+            if argument not in signature.parameters:
+                raise AgentDirectAnswerFunctionError(
+                    f"The method {method} does not have a '{argument}' parameter."
+                )
+        bound_method = types.MethodType(method, self)
+        setattr(self, "answer_question_directly", bound_method)
 
     async def async_answer_question(
         self,
         question: Question,
         scenario: Optional[Scenario] = None,
         model: Optional[LanguageModel] = None,
         debug: bool = False,
@@ -61,15 +123,17 @@
         current_answers: Optional[dict] = None,
     ):
         """
         This is a function where an agent returns an answer to a particular question.
         However, there are several different ways an agent can answer a question, so the
         actual functionality is delegated to an Invigilator object.
         """
-        model = model or LanguageModelOpenAIThreeFiveTurbo(use_cache=True)
+        self.current_question = question
+        # model = model or LanguageModelOpenAIThreeFiveTurbo(use_cache=True)
+        model = model or Model("gpt-3.5-turbo", use_cache=True)
         scenario = scenario or Scenario()
         invigilator = self._create_invigilator(
             question, scenario, model, debug, memory_plan, current_answers
         )
         response: AgentResponseDict = await invigilator.async_answer_question()
         return response
 
@@ -80,15 +144,15 @@
         question: Question,
         scenario: Optional[Scenario] = None,
         model: Optional[LanguageModel] = None,
         debug: bool = False,
         memory_plan: Optional[MemoryPlan] = None,
         current_answers: Optional[dict] = None,
     ):
-        model = model or LanguageModelOpenAIThreeFiveTurbo(use_cache=True)
+        model = model or Model("gpt-3.5-turbo", use_cache=True)
         scenario = scenario or Scenario()
 
         if debug:
             # use the question's simulate_answer method
             invigilator_class = InvigilatorDebug
         elif hasattr(question, "answer_question_directly"):
             # it is a functional question and the answer only depends on the agent's traits & the scenario
```

### Comparing `edsl-0.1.8/edsl/agents/AgentList.py` & `edsl-0.1.9/edsl/agents/AgentList.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/agents/AgentListExportMixin.py` & `edsl-0.1.9/edsl/agents/AgentListExportMixin.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/agents/Invigilator.py` & `edsl-0.1.9/edsl/agents/Invigilator.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     def get_prompts(self) -> Dict[str, Prompt]:
         return {"user_prompt": Prompt("NA"), "system_prompt": Prompt("NA")}
 
 
 class InvigilatorHuman(InvigilatorBase):
     async def async_answer_question(self) -> AgentResponseDict:
-        answer = self.agent.answer_question_directly(self.question.question_name)
+        answer = self.agent.answer_question_directly(self.question, self.scenario)
         response = {"answer": answer}
         response = self.question.validate_response(response)
         response["comment"] = "This is a real survey response from a human."
         response["prompts"] = self.get_prompts()
         return AgentResponseDict(**response)
 
     def get_prompts(self) -> Dict[str, Prompt]:
```

### Comparing `edsl-0.1.8/edsl/agents/descriptors.py` & `edsl-0.1.9/edsl/agents/descriptors.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/api/client.py` & `edsl-0.1.9/edsl/api/client.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/api/results.py` & `edsl-0.1.9/edsl/api/results.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/config.py` & `edsl-0.1.9/edsl/config.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/data/Database.py` & `edsl-0.1.9/edsl/data/Database.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/data/crud.py` & `edsl-0.1.9/edsl/data/crud.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/data/orm.py` & `edsl-0.1.9/edsl/data/orm.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/enums.py` & `edsl-0.1.9/edsl/enums.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/exceptions/__init__.py` & `edsl-0.1.9/edsl/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/exceptions/questions.py` & `edsl-0.1.9/edsl/exceptions/questions.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/exceptions/surveys.py` & `edsl-0.1.9/edsl/exceptions/surveys.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/jobs/Answers.py` & `edsl-0.1.9/edsl/jobs/Answers.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/jobs/Interview.py` & `edsl-0.1.9/edsl/jobs/Interview.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/jobs/Jobs.py` & `edsl-0.1.9/edsl/jobs/Jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -237,29 +237,54 @@
     #######################
     # Example methods
     #######################
     @classmethod
     def example(cls) -> Jobs:
         from edsl.questions import QuestionMultipleChoice
 
+        from edsl import Agent
+
+        # (status, question, period)
+        agent_answers = {
+            ("Joyful", "how_feeling", "morning"): "OK",
+            ("Joyful", "how_feeling", "afternoon"): "Great",
+            ("Joyful", "how_feeling_yesterday", "morning"): "Great",
+            ("Joyful", "how_feeling_yesterday", "afternoon"): "Good",
+            ("Sad", "how_feeling", "morning"): "Terrible",
+            ("Sad", "how_feeling", "afternoon"): "OK",
+            ("Sad", "how_feeling_yesterday", "morning"): "OK",
+            ("Sad", "how_feeling_yesterday", "afternoon"): "Terrible",
+        }
+
+        def answer_question_directly(self, question, scenario):
+            return agent_answers[
+                (self.traits["status"], question.question_name, scenario["period"])
+            ]
+
+        sad_agent = Agent({"status": "Sad"})
+        joy_agent = Agent({"status": "Joyful"})
+
+        sad_agent.add_direct_question_answering_method(answer_question_directly)
+        joy_agent.add_direct_question_answering_method(answer_question_directly)
+
         q1 = QuestionMultipleChoice(
             question_text="How are you this {{ period }}?",
             question_options=["Good", "Great", "OK", "Terrible"],
             question_name="how_feeling",
         )
         q2 = QuestionMultipleChoice(
             question_text="How were you feeling yesterday {{ period }}?",
             question_options=["Good", "Great", "OK", "Terrible"],
             question_name="how_feeling_yesterday",
         )
         base_survey = Survey(questions=[q1, q2])
 
         job = base_survey.by(
             Scenario({"period": "morning"}), Scenario({"period": "afternoon"})
-        ).by(Agent({"status": "Super duper unhappy"}), Agent({"status": "Joyful"}))
+        ).by(joy_agent, sad_agent)
 
         return job
 
 
 def main():
     from edsl.jobs import Jobs
```

### Comparing `edsl-0.1.8/edsl/jobs/JobsRunner.py` & `edsl-0.1.9/edsl/jobs/JobsRunner.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/jobs/base.py` & `edsl-0.1.9/edsl/jobs/base.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/jobs/runners/JobsRunnerAsyncio.py` & `edsl-0.1.9/edsl/jobs/runners/JobsRunnerAsyncio.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/jobs/runners/JobsRunnerStreaming.py` & `edsl-0.1.9/edsl/jobs/runners/JobsRunnerStreaming.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/DeepInfra.py` & `edsl-0.1.9/edsl/language_models/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/LanguageModel.py` & `edsl-0.1.9/edsl/language_models/LanguageModel.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/OpenAI.py` & `edsl-0.1.9/edsl/language_models/OpenAI.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/model_interfaces/GeminiPro.py` & `edsl-0.1.9/edsl/language_models/model_interfaces/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/model_interfaces/LlamaTwo13B.py` & `edsl-0.1.9/edsl/language_models/model_interfaces/LlamaTwo13B.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/model_interfaces/LlamaTwo70B.py` & `edsl-0.1.9/edsl/language_models/model_interfaces/LlamaTwo70B.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/model_interfaces/Mixtral8x7B.py` & `edsl-0.1.9/edsl/language_models/model_interfaces/Mixtral8x7B.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/registry.py` & `edsl-0.1.9/edsl/language_models/registry.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/repair.py` & `edsl-0.1.9/edsl/language_models/repair.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/language_models/unused/ReplicateBase.py` & `edsl-0.1.9/edsl/language_models/unused/ReplicateBase.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/Prompt.py` & `edsl-0.1.9/edsl/prompts/Prompt.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/agent_instructions.py` & `edsl-0.1.9/edsl/prompts/library/agent_instructions.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_budget.py` & `edsl-0.1.9/edsl/prompts/library/question_budget.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_checkbox.py` & `edsl-0.1.9/edsl/prompts/library/question_checkbox.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_extract.py` & `edsl-0.1.9/edsl/prompts/library/question_extract.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_linear_scale.py` & `edsl-0.1.9/edsl/prompts/library/question_linear_scale.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_list.py` & `edsl-0.1.9/edsl/prompts/library/question_list.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_multiple_choice.py` & `edsl-0.1.9/edsl/prompts/library/question_multiple_choice.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_numerical.py` & `edsl-0.1.9/edsl/prompts/library/question_numerical.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/library/question_rank.py` & `edsl-0.1.9/edsl/prompts/library/question_rank.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/prompt_config.py` & `edsl-0.1.9/edsl/prompts/prompt_config.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/prompts/registry.py` & `edsl-0.1.9/edsl/prompts/registry.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/AnswerValidatorMixin.py` & `edsl-0.1.9/edsl/questions/AnswerValidatorMixin.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/Question.py` & `edsl-0.1.9/edsl/questions/Question.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionBudget.py` & `edsl-0.1.9/edsl/questions/QuestionBudget.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionCheckBox.py` & `edsl-0.1.9/edsl/questions/QuestionCheckBox.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionExtract.py` & `edsl-0.1.9/edsl/questions/QuestionExtract.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionFreeText.py` & `edsl-0.1.9/edsl/questions/QuestionFreeText.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionFunctional.py` & `edsl-0.1.9/edsl/questions/QuestionFunctional.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionList.py` & `edsl-0.1.9/edsl/questions/QuestionList.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionMultipleChoice.py` & `edsl-0.1.9/edsl/questions/QuestionMultipleChoice.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionNumerical.py` & `edsl-0.1.9/edsl/questions/QuestionNumerical.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/QuestionRank.py` & `edsl-0.1.9/edsl/questions/QuestionRank.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/__init__.py` & `edsl-0.1.9/edsl/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/compose_questions.py` & `edsl-0.1.9/edsl/questions/compose_questions.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/derived/QuestionLikertFive.py` & `edsl-0.1.9/edsl/questions/derived/QuestionLikertFive.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/derived/QuestionLinearScale.py` & `edsl-0.1.9/edsl/questions/derived/QuestionLinearScale.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/derived/QuestionTopK.py` & `edsl-0.1.9/edsl/questions/derived/QuestionTopK.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/derived/QuestionYesNo.py` & `edsl-0.1.9/edsl/questions/derived/QuestionYesNo.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/questions/descriptors.py` & `edsl-0.1.9/edsl/questions/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     @abstractmethod
     def validate(self, value: Any) -> None:
         """Validates the value. If it is invalid, raises an exception. If it is valid, does nothing."""
         pass
 
     def __get__(self, instance, owner):
         """"""
+        if self.name not in instance.__dict__:
+            return {}
         return instance.__dict__[self.name]
 
     def __set__(self, instance, value: Any) -> None:
         self.validate(value, instance)
         instance.__dict__[self.name] = value
         if self.name == "_instructions":
             instructions = value
```

### Comparing `edsl-0.1.8/edsl/questions/question_registry.py` & `edsl-0.1.9/edsl/questions/question_registry.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/report/InputOutputDataTypes.py` & `edsl-0.1.9/edsl/report/InputOutputDataTypes.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/report/RegressionMixin.py` & `edsl-0.1.9/edsl/report/RegressionMixin.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/report/ReportOutputs.py` & `edsl-0.1.9/edsl/report/ReportOutputs.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/report/ResultsFetchMixin.py` & `edsl-0.1.9/edsl/report/ResultsFetchMixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,22 @@
     def _fetch_answer_data(self, key, element_data_class):
         """Extracts data from a results object and returns in in the corresponding element_data_class."""
         question = self.survey.get_question(key)
         question_type = question.question_type
         options = getattr(question, "question_options", None)
         responses = self._fetch_list("answer", key)
 
+        if hasattr(question, "short_names_dict"):
+            short_names_dict = getattr(question, "short_names_dict", {})
+        else:
+            short_names_dict = {}
+
         data = {
             "text": question.question_text,
-            "short_names_dict": question.short_names_dict,
+            "short_names_dict": short_names_dict,
         }
 
         if element_data_class == CategoricalData:
             if question_type in ["checkbox"]:
                 data["responses"] = [
                     str(r) for r in list(chain.from_iterable(responses))
                 ]
```

### Comparing `edsl-0.1.8/edsl/report/ResultsOutputMixin.py` & `edsl-0.1.9/edsl/report/ResultsOutputMixin.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/report/demo.ipynb` & `edsl-0.1.9/edsl/report/demo.ipynb`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/results/Dataset.py` & `edsl-0.1.9/edsl/results/Dataset.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/results/Result.py` & `edsl-0.1.9/edsl/results/Result.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/results/Results.py` & `edsl-0.1.9/edsl/results/Results.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,29 @@
     ):
         super().__init__(data)
         self.survey = survey
         self.created_columns = created_columns or []
         self._job_uuid = job_uuid
         self._total_results = total_results
 
+        if hasattr(self, "add_output_functions"):
+            self.add_output_functions()
+
     ######################
     # Streaming methods
     ######################
+
+    def __getitem__(self, i):
+        if isinstance(i, slice):
+            # Return a sliced view of the list
+            return self.__class__(survey=self.survey, data=self.data[i])
+        else:
+            # Return a single item
+            return self.data[i]
+
     def _update_results(self) -> None:
         if self._job_uuid and len(self.data) < self._total_results:
             results = [
                 Result(
                     agent=Agent.from_dict(json.loads(r.agent)),
                     scenario=Scenario.from_dict(json.loads(r.scenario)),
                     model=LanguageModel.from_dict(json.loads(r.model)),
@@ -400,15 +412,15 @@
         """
         Returns an example Results object
         - debug: if False, uses actual API calls
         """
         from edsl.jobs import Jobs
 
         job = Jobs.example()
-        results = job.run(n=1, debug=debug)
+        results = job.run()
         return results
 
 
 def main():  # pragma: no cover
     """Calls the OpenAI API credits"""
     from edsl.results.Results import Results
```

### Comparing `edsl-0.1.8/edsl/results/ResultsExportMixin.py` & `edsl-0.1.9/edsl/results/ResultsExportMixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,28 +61,27 @@
         html=False,
         interactive=False,
         split_at_dot=True,
     ):
         if pretty_labels is None:
             pretty_labels = {}
 
+        new_data = []
+        for entry in self:
+            key, list_of_values = list(entry.items())[0]
+            new_data.append({pretty_labels.get(key, key): list_of_values})
         else:
-            new_data = []
-            for entry in self:
-                key, list_of_values = list(entry.items())[0]
-                new_data.append({pretty_labels.get(key, key): list_of_values})
+            if not html:
+                print_list_of_dicts_with_rich(
+                    new_data, filename=filename, split_at_dot=split_at_dot
+                )
             else:
-                if not html:
-                    print_list_of_dicts_with_rich(
-                        new_data, filename=filename, split_at_dot=split_at_dot
-                    )
-                else:
-                    print_list_of_dicts_as_html_table(
-                        new_data, filename=None, interactive=interactive
-                    )
+                print_list_of_dicts_as_html_table(
+                    new_data, filename=None, interactive=interactive
+                )
 
     @convert_decorator
     def to_csv(self, filename: str = None, remove_prefix=False, download_link=False):
         """
         >>> r = create_example_results()
         >>> r.select('how_feeling').to_csv()
         'result.how_feeling\\r\\nBad\\r\\nBad\\r\\nGreat\\r\\nGreat\\r\\n'
```

### Comparing `edsl-0.1.8/edsl/scenarios/Scenario.py` & `edsl-0.1.9/edsl/scenarios/Scenario.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/scenarios/ScenarioList.py` & `edsl-0.1.9/edsl/scenarios/ScenarioList.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/surveys/DAG.py` & `edsl-0.1.9/edsl/surveys/DAG.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/surveys/Memory.py` & `edsl-0.1.9/edsl/surveys/Memory.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/surveys/MemoryPlan.py` & `edsl-0.1.9/edsl/surveys/MemoryPlan.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/surveys/Rule.py` & `edsl-0.1.9/edsl/surveys/Rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,27 +56,27 @@
     This would be a lot of work.
     """
 
     def __init__(
         self,
         current_q: int,
         expression: str,
-        next_q: Union[int, EndOfSurvey],
+        next_q: Union[int, EndOfSurvey.__class__],
         question_name_to_index: dict[str, int],
         priority: int,
     ):
         """Questions are represented by int indices."""
 
         self.current_q = current_q
         self.expression = expression
         self.next_q = next_q
         self.priority = priority
         self.question_name_to_index = question_name_to_index
 
-        if not isinstance(next_q, EndOfSurvey) and current_q > next_q:
+        if not next_q == EndOfSurvey and current_q > next_q:
             raise SurveyRuleSendsYouBackwardsError
 
         # get the AST for the expression - used to extract
         # the variables referenced in the expression
         try:
             self.ast_tree = ast.parse(self.expression)
         except SyntaxError:
@@ -103,25 +103,23 @@
             if max(self.named_questions_by_index) > self.current_q:
                 raise SurveyRuleRefersToFutureStateError
 
     def to_dict(self):
         return {
             "current_q": self.current_q,
             "expression": self.expression,
-            "next_q": "EndOfSurvey"
-            if isinstance(self.next_q, EndOfSurvey)
-            else self.next_q,
+            "next_q": "EndOfSurvey" if self.next_q == EndOfSurvey else self.next_q,
             "priority": self.priority,
             "question_name_to_index": self.question_name_to_index,
         }
 
     @classmethod
     def from_dict(self, rule_dict):
         if rule_dict["next_q"] == "EndOfSurvey":
-            rule_dict["next_q"] = EndOfSurvey()
+            rule_dict["next_q"] = EndOfSurvey
 
         return Rule(
             current_q=rule_dict["current_q"],
             expression=rule_dict["expression"],
             next_q=rule_dict["next_q"],
             priority=rule_dict["priority"],
             question_name_to_index=rule_dict["question_name_to_index"],
```

### Comparing `edsl-0.1.8/edsl/surveys/RuleCollection.py` & `edsl-0.1.9/edsl/surveys/RuleCollection.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     def __init__(self, num_questions: int = None, rules: List[Rule] = None):
         super().__init__(rules or [])
         self.num_questions = num_questions
 
     def __repr__(self):
         """
         >>> rule_collection = RuleCollection.example()
-        >>> rule_collection == eval(repr(rule_collection))
-        True
+        >>> _ = eval(repr(rule_collection))
         """
         return f"RuleCollection(rules={self.data}, num_questions={self.num_questions})"
 
     def to_dict(self):
         return {
             "rules": [rule.to_dict() for rule in self],
             "num_questions": self.num_questions,
@@ -123,25 +122,25 @@
         """Returns a list of all question indices between start_q and end_q
         >>> rule_collection = RuleCollection(num_questions=5)
         >>> rule_collection.keys_between(1, 3)
         [2, 3]
         >>> rule_collection.keys_between(1, 4)
         [2, 3, 4]
         >>> rule_collection.keys_between(1, EndOfSurvey, right_inclusive=False)
-        [2, 3, 4]
+        [2, 3]
         """
 
         # If it's the end of the survey, all questions between the start_q and the end of the survey
         # now depend on the start_q
         if end_q == EndOfSurvey:
             if self.num_questions is None:
                 raise ValueError(
                     "Cannot determine DAG when EndOfSurvey and when num_questions is not known"
                 )
-            end_q = self.num_questions
+            end_q = self.num_questions - 1
 
         question_range = list(range(start_q + 1, end_q + int(right_inclusive)))
 
         return question_range
 
     @property
     def dag(self) -> dict:
```

### Comparing `edsl-0.1.8/edsl/surveys/Survey.py` & `edsl-0.1.9/edsl/surveys/Survey.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,22 +191,22 @@
 
         self.memory_plan.add_memory_collection(
             focal_question=focal_question_name, prior_questions=prior_question_names
         )
 
     def add_stop_rule(self, question: Question, expression: str) -> Survey:
         """Adds a rule that stops the survey."""
-        self.add_rule(question, expression, EndOfSurvey())
+        self.add_rule(question, expression, EndOfSurvey)
         return self
 
     def _get_question_index(self, q):
         """Returns the index of the question or EndOfSurvey object. It can handle it if the user
         passes in the question name, the question object, or the EndOfSurvey object."""
-        if isinstance(q, EndOfSurvey):
-            return EndOfSurvey()
+        if q == EndOfSurvey:
+            return EndOfSurvey
         else:
             question_name = q if isinstance(q, str) else q.question_name
             if question_name not in self.question_name_to_index:
                 raise ValueError(
                     f"""Question name {question_name} not found in survey. The current question names are {self.question_name_to_index}."""
                 )
             return self.question_name_to_index[question_name]
@@ -271,15 +271,15 @@
 
     def first_question(self) -> Question:
         "Returns the first question in the survey"
         return self.questions[0]
 
     def next_question(
         self, current_question: "Question", answers: dict
-    ) -> Union[Question, EndOfSurvey]:
+    ) -> Union[Question, EndOfSurvey.__class__]:
         """
         Returns the next question in a survey.
         - If called with no arguments, it returns the first question in the survey.
         - If no answers are provided for a question with a rule, the next question is returned. If answers are provided, the next question is determined by the rules and the answers.
         - If the next question is the last question in the survey, an EndOfSurvey object is returned.
         """
         if isinstance(current_question, str):
@@ -292,19 +292,19 @@
         next_question_object = self.rule_collection.next_question(
             question_index, answers
         )
 
         if next_question_object.num_rules_found == 0:
             raise SurveyHasNoRulesError
 
-        if isinstance(next_question_object.next_q, EndOfSurvey):
-            return EndOfSurvey()
+        if next_question_object.next_q == EndOfSurvey:
+            return EndOfSurvey
         else:
             if next_question_object.next_q >= len(self.questions):
-                return EndOfSurvey()
+                return EndOfSurvey
             else:
                 return self.questions[next_question_object.next_q]
 
     def gen_path_through_survey(self) -> Generator[Question, dict, None]:
         """
         Generates a coroutine that can be used to conduct an Interview.
         - The coroutine is a generator that yields a question and receives answers.
@@ -313,15 +313,15 @@
 
         E.g., in Interview.py
 
         path_through_survey = self.survey.gen_path_through_survey()
         question = path_through_survey.send({question.question_name: answer})
         """
         question = self.first_question()
-        while not isinstance(question, EndOfSurvey):
+        while not question == EndOfSurvey:
             self.answers = yield question
             question = self.next_question(question, self.answers)
 
     @property
     def scenario_attributes(self) -> list[str]:
         """Returns a list of attributes that admissible Scenarios should have"""
         temp = []
@@ -331,21 +331,36 @@
             matches = re.findall(r"\{\{(.+?)\}\}", question_text)
             # remove whitespace
             matches = [match.strip() for match in matches]
             # add them to the temp list
             temp.extend(matches)
         return temp
 
-    def textify(self, d: DAG) -> DAG:
-        return {
-            self.questions[key].question_name: {
-                self.questions[index].question_name for index in value
-            }
-            for key, value in d.items()
-        }
+    def textify(self, index_dag: DAG) -> DAG:
+        """Converts the DAG of question indices to a DAG of question names
+        >>> s = Survey.example()
+        >>> d = s.dag()
+        >>> d
+        {1: {0}, 2: {0}}
+        >>> s.textify(d)
+        {'q1': {'q0'}, 'q2': {'q0'}}
+        """
+
+        def get_name(index):
+            return self.questions[index].question_name
+
+        try:
+            text_dag = {}
+            for child_index, parent_indices in index_dag.items():
+                parent_names = {get_name(index) for index in parent_indices}
+                child_name = get_name(child_index)
+                text_dag[child_name] = parent_names
+            return text_dag
+        except IndexError:
+            breakpoint()
 
     def dag(self, textify=False) -> DAG:
         """Returns the DAG of the survey, which reflects both skip-logic and memory."""
         memory_dag = self.memory_plan.dag
         rule_dag = self.rule_collection.dag
         if textify:
             memory_dag = DAG(self.textify(memory_dag))
```

### Comparing `edsl-0.1.8/edsl/surveys/SurveyExportMixin.py` & `edsl-0.1.9/edsl/surveys/SurveyExportMixin.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/surveys/descriptors.py` & `edsl-0.1.9/edsl/surveys/descriptors.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/trackers/Tracker.py` & `edsl-0.1.9/edsl/trackers/Tracker.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/trackers/TrackerAPI.py` & `edsl-0.1.9/edsl/trackers/TrackerAPI.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/trackers/TrackerTasks.py` & `edsl-0.1.9/edsl/trackers/TrackerTasks.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/utilities/ast_utilities.py` & `edsl-0.1.9/edsl/utilities/ast_utilities.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/utilities/data/scooter_results.json` & `edsl-0.1.9/edsl/utilities/data/scooter_results.json`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/utilities/decorators.py` & `edsl-0.1.9/edsl/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/utilities/interface.py` & `edsl-0.1.9/edsl/utilities/interface.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/edsl/utilities/utilities.py` & `edsl-0.1.9/edsl/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `edsl-0.1.8/pyproject.toml` & `edsl-0.1.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 documentation = "https://www.goemeritus.com/getting-started/"
 homepage = "https://www.goemeritus.com/"
 keywords = ["LLM", "social science", "surveys", "user research"]
 license = "MIT"
 name = "edsl"
 packages = [{include = "edsl"}]
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = "^3.9.1"
 numpy = "^1.22"
 sqlalchemy = "^2.0.23"
 python-dotenv = "^1.0.0"
 openai = "^1.4.0"
@@ -35,26 +35,18 @@
 jupyter = "^1.0.0"
 pandas = "^2.1.4"
 tenacity = "^8.2.3"
 python-docx = "^1.1.0"
 pillow = ">=9.4.0"
 nest-asyncio = "^1.5.9"
 aiohttp = "^3.9.1"
-markdown2 = {optional = true, version = "^2.4.11"}
-seaborn = {optional = true, version = "^0.13.0"}
-statsmodels = {optional = true, version = "^0.13.5"}
-wordcloud = {optional = true, version = "^1.9.3"}
-
-[tool.poetry.extras]
-report = [
-    "markdown2",
-    "seaborn",
-    "statsmodels",
-    "wordcloud",
-]
+markdown2 = "^2.4.11"
+seaborn = "^0.13.0"
+statsmodels = "^0.13.5"
+wordcloud = "^1.9.3"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^23.12.0"}
 coverage = "^7.3.3"
 mypy = "^1.7.1"
 pre-commit = "^3.6.0"
 pytest = "^7.4.3"
```

### Comparing `edsl-0.1.8/PKG-INFO` & `edsl-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsl
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create and analyze LLM-based surveys
 Home-page: https://www.goemeritus.com/
 License: MIT
 Keywords: LLM,social science,surveys,user research
 Author: Apostolos Filippas
 Author-email: apostolos@goemeritus.com
 Requires-Python: >=3.9.1,<4.0.0
@@ -12,33 +12,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: report
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: markdown2 (>=2.4.11,<3.0.0) ; extra == "report"
+Requires-Dist: markdown2 (>=2.4.11,<3.0.0)
 Requires-Dist: nest-asyncio (>=1.5.9,<2.0.0)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: openai (>=1.4.0,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pillow (>=9.4.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: seaborn (>=0.13.0,<0.14.0) ; extra == "report"
+Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: simpleeval (>=0.9.13,<0.10.0)
 Requires-Dist: sqlalchemy (>=2.0.23,<3.0.0)
-Requires-Dist: statsmodels (>=0.13.5,<0.14.0) ; extra == "report"
+Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: wordcloud (>=1.9.3,<2.0.0) ; extra == "report"
+Requires-Dist: wordcloud (>=1.9.3,<2.0.0)
 Project-URL: Documentation, https://www.goemeritus.com/getting-started/
 Description-Content-Type: text/markdown
 
 # Emeritus Domain-Specific Language 
 <p align="center">
   <img src="https://github.com/goemeritus/edsl-public/blob/main/static/logo.png?raw=true" alt="edsl.png" width="100"/>
 </p>
```

