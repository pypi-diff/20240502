# Comparing `tmp/graph_validation_tests-0.0.8.tar.gz` & `tmp/graph_validation_tests-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_validation_tests-0.0.8.tar", max compression
+gzip compressed data, was "graph_validation_tests-0.0.9.tar", max compression
```

## Comparing `graph_validation_tests-0.0.8.tar` & `graph_validation_tests-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1070 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/LICENSE
--rw-r--r--   0        0        0    12012 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/README.md
--rw-r--r--   0        0        0    29085 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/translator/__init__.py
--rw-r--r--   0        0        0    36673 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/translator/registry/__init__.py
--rw-r--r--   0        0        0    10042 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/translator/trapi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/utils/__init__.py
--rw-r--r--   0        0        0      722 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/utils/asyncio.py
--rw-r--r--   0        0        0      113 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/utils/constants.py
--rw-r--r--   0        0        0      886 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/utils/http.py
--rw-r--r--   0        0        0     4267 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/utils/ontology_kp.py
--rw-r--r--   0        0        0    18148 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/graph_validation_test/utils/unit_test_templates.py
--rw-r--r--   0        0        0     8959 2024-04-19 22:49:43.140759 graph_validation_tests-0.0.8/one_hop_test/__init__.py
--rw-r--r--   0        0        0     3027 2024-04-19 22:49:56.756869 graph_validation_tests-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4851 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/standards_validation_test/__init__.py
--rw-r--r--   0        0        0     1292 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/__init__.py
--rw-r--r--   0        0        0     3611 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/test_graph_validation_test.py
--rw-r--r--   0        0        0     5764 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/test_unit_test_templates.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/translator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/translator/biolink/__init__.py
--rw-r--r--   0        0        0     1065 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/translator/biolink/test_ontology_kp.py
--rw-r--r--   0        0        0    18030 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/translator/trapi/__init__.py
--rw-r--r--   0        0        0     5061 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/graph_validation_test/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/__init__.py
--rw-r--r--   0        0        0     3383 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_one_hop_test.py
--rw-r--r--   0        0        0    25697 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2063 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/activate
--rw-r--r--   0        0        0     1027 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/activate.bat
--rw-r--r--   0        0        0      371 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/deactivate.bat
--rw-r--r--   0        0        0   108460 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pip.exe
--rw-r--r--   0        0        0   108460 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pip3.10.exe
--rw-r--r--   0        0        0   108460 2024-04-19 22:49:43.144759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pip3.exe
--rw-r--r--   0        0        0   268568 2024-04-19 22:49:43.148759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/python.exe
--rw-r--r--   0        0        0   257304 2024-04-19 22:49:43.148759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pythonw.exe
--rw-r--r--   0        0        0      164 2024-04-19 22:49:43.148759 graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/pyvenv.cfg
--rw-r--r--   0        0        0       70 2024-04-19 22:49:43.148759 graph_validation_tests-0.0.8/tests/scripts/one_hop_test.cmd
--rw-r--r--   0        0        0        0 2024-04-19 22:49:43.148759 graph_validation_tests-0.0.8/tests/standards_validation_test/__init__.py
--rw-r--r--   0        0        0     1720 2024-04-19 22:49:43.148759 graph_validation_tests-0.0.8/tests/standards_validation_test/test_standards_validation_test.py
--rw-r--r--   0        0        0    13987 1970-01-01 00:00:00.000000 graph_validation_tests-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-26 03:56:11.432092 graph_validation_tests-0.0.9/LICENSE
+-rw-r--r--   0        0        0    11881 2024-04-26 03:56:11.432092 graph_validation_tests-0.0.9/README.md
+-rw-r--r--   0        0        0    30115 2024-04-26 03:56:11.432092 graph_validation_tests-0.0.9/graph_validation_test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.432092 graph_validation_tests-0.0.9/graph_validation_test/translator/__init__.py
+-rw-r--r--   0        0        0    36673 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/translator/registry/__init__.py
+-rw-r--r--   0        0        0    10858 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/translator/trapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/utils/__init__.py
+-rw-r--r--   0        0        0      722 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/utils/asyncio.py
+-rw-r--r--   0        0        0      113 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/utils/constants.py
+-rw-r--r--   0        0        0      886 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/utils/http.py
+-rw-r--r--   0        0        0     4267 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/utils/ontology_kp.py
+-rw-r--r--   0        0        0    18148 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/graph_validation_test/utils/unit_test_templates.py
+-rw-r--r--   0        0        0     8959 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/one_hop_test/__init__.py
+-rw-r--r--   0        0        0     3002 2024-04-26 03:56:23.132114 graph_validation_tests-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4851 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/standards_validation_test/__init__.py
+-rw-r--r--   0        0        0     1292 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/__init__.py
+-rw-r--r--   0        0        0     4774 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/test_graph_validation_test.py
+-rw-r--r--   0        0        0     5764 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/test_unit_test_templates.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/translator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/translator/biolink/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/translator/biolink/test_ontology_kp.py
+-rw-r--r--   0        0        0    18029 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/translator/trapi/__init__.py
+-rw-r--r--   0        0        0     4886 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/graph_validation_test/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/one_hop_test/__init__.py
+-rw-r--r--   0        0        0     3007 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/one_hop_test/test_one_hop_test.py
+-rw-r--r--   0        0        0    25697 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2063 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/activate
+-rw-r--r--   0        0        0     1027 2024-04-26 03:56:11.436092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/activate.bat
+-rw-r--r--   0        0        0      371 2024-04-26 03:56:11.440092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/deactivate.bat
+-rw-r--r--   0        0        0   108460 2024-04-26 03:56:11.440092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pip.exe
+-rw-r--r--   0        0        0   108460 2024-04-26 03:56:11.440092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pip3.10.exe
+-rw-r--r--   0        0        0   108460 2024-04-26 03:56:11.440092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pip3.exe
+-rw-r--r--   0        0        0   268568 2024-04-26 03:56:11.440092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/python.exe
+-rw-r--r--   0        0        0   257304 2024-04-26 03:56:11.444092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pythonw.exe
+-rw-r--r--   0        0        0      164 2024-04-26 03:56:11.444092 graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/pyvenv.cfg
+-rw-r--r--   0        0        0       70 2024-04-26 03:56:11.444092 graph_validation_tests-0.0.9/tests/scripts/one_hop_test.cmd
+-rw-r--r--   0        0        0        0 2024-04-26 03:56:11.444092 graph_validation_tests-0.0.9/tests/standards_validation_test/__init__.py
+-rw-r--r--   0        0        0     1474 2024-04-26 03:56:11.444092 graph_validation_tests-0.0.9/tests/standards_validation_test/test_standards_validation_test.py
+-rw-r--r--   0        0        0    13857 1970-01-01 00:00:00.000000 graph_validation_tests-0.0.9/PKG-INFO
```

### Comparing `graph_validation_tests-0.0.8/LICENSE` & `graph_validation_tests-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/README.md` & `graph_validation_tests-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -202,59 +202,53 @@
 Note that the trapi_generation variables - defined in the **graph_validation_test.utils.unit_test_templates** module - are all simply Python functions returning TRAPI JSON messages to send to the target components. In principle, if one understands what those functions are doing, you could write your own methods to do other kinds of TRAPI queries whose output can then be validated against the specified TRAPI and Biolink Model releases.
 
 ### Sample Output
 
 This is a sample of what the JSON output from test runs currently looks like (this sample came from a OneHopTest run).
 
 ```json
-{
-    "pks": [
-        "arax",
-        "molepro"
-    ],
-    "results": [
-        [
-            {
-                "arax": {
-                    "by_subject": {
-                        "info": {},
-                        "skipped": {},
-                        "warning": {},
-                        "error": {
-                            "error.trapi.response.knowledge_graph.missing_expected_edge": {
-                                "global": {
-                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:has_side_effect]->(MONDO:0011426#biolink:Disease)": null
-                                }
+{    
+    "pks": {
+        "molepro": "molepro"
+    },
+    "results": {
+        "TestAsset_1-by_subject": {
+            "molepro": {
+                "status": "FAILED",
+                "messages": {
+                    "error": {
+                        "error.trapi.response.knowledge_graph.missing_expected_edge": {
+                            "global": {
+                                "TestAsset_1|(CHEBI:58579#biolink:SmallMolecule)-[biolink:is_active_metabolite_of]->(UniProtKB:Q9NQ88#biolink:Protein)": null
                             }
-                        },
-                        "critical": {}
+                        }
                     }
                 }
-            },
-"etc ...",
-            {
-                "molepro": {
-                    "by_subject": {
-                        "info": {},
-                        "skipped": {},
-                        "warning": {},
-                        "error": {
-                            "error.trapi.response.knowledge_graph.missing_expected_edge": {
-                                "global": {
-                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:has_side_effect]->(MONDO:0011426#biolink:Disease)": null
-                                }
+            }
+        },
+        "TestAsset_1-inverse_by_new_subject": {
+            "molepro": {
+                "status": "FAILED",
+                "messages": {
+                    "critical": {
+                        "critical.trapi.request.invalid": {
+                            "global": {
+                                "predicate 'biolink:is_active_metabolite_of'": [
+                                    {
+                                        "context": "inverse_by_new_subject",
+                                        "reason": "is an unknown or has no inverse?"
+                                    }
+                                ]
                             }
-                        },
-                        "critical": {}
+                        }
                     }
                 }
-            },
-etc...
-        ]
-    ]
+            }
+        },
+        # etc...
 }
 ```
 
 ## Releases
 
 A [full change log](CHANGELOG.md) is provided documenting each release, but we summarize key release limitations here:
```

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/__init__.py` & `graph_validation_tests-0.0.9/graph_validation_test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 """
 from typing import Dict, List, Optional, Tuple
 
 from argparse import ArgumentParser
 
 from reasoner_validator.biolink import BiolinkValidator
 from reasoner_validator.message import MESSAGES_BY_TARGET, MESSAGE_CATALOG, MESSAGES_BY_TEST
-from translator_testing_model.datamodel.pydanticmodel import (
-    TestAsset,
-    TestEnvEnum,
-    ComponentEnum,
-    TestCaseResultEnum
-)
+from translator_testing_model.datamodel.pydanticmodel import TestAsset, TestCaseResultEnum
 
 from graph_validation_test.translator.registry import (
     get_the_registry_data,
     extract_component_test_metadata_from_registry
 )
+from graph_validation_test.translator.trapi import get_available_components
 from graph_validation_test.utils.asyncio import gather
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class TestCaseRun(BiolinkValidator):
@@ -170,17 +166,18 @@
             runner_settings: Optional[List[str]] = None,
             **kwargs
     ):
         """
         GraphValidationTest constructor.
 
         :param test_asset: TestAsset, target test asset(s) being processed
-        :param component: Optional[str] = None, target component to be tested, (default: 'ars' assumed)
+        :param component: Optional[str] = None, target component to be tested,
+                          from ComponentEnum (default: 'ars' assumed)
         :param environment: Optional[str] = None, Translator execution environment for the test,
-                                            one of 'dev', 'ci', 'test' or 'prod' (default: 'ci' assumed)
+                            from TestEnvEnum, one of 'dev', 'ci', 'test' or 'prod' (default: 'ci' assumed)
         :param trapi_generators: Optional[List] = None, pointers to code functions that configure
                                  TRAPI query requests. e.g. see one_hop_test.unit_test_templates.
                                  May be empty for some types of tests with fixed TRAPI queries internally?
         :param trapi_version: Optional[str] = None, target TRAPI version (default: current release)
         :param biolink_version: Optional[str], target Biolink Model version (default: current release)
         :param runner_settings: Optional[List[str]], extra string directives to the Test Runner (default: None)
         :param kwargs: named arguments to pass on to BiolinkValidator parent class (if and as applicable)
@@ -269,20 +266,20 @@
         # TODO: unsure if one needs to limit concurrent requests here...
         await gather([test_case.run_test_case() for test_case in test_cases])  # , limit=num_concurrent_requests)
 
     FAILURE_MODES = ("error", "critical")
 
     def compute_status(self, tcr: TestCaseRun) -> Tuple[str, TestCaseResultEnum, Dict]:
         """
-        Method to construct components for a test case result based on
-        the failure mode assessment of non-empty validation messages.
+        Method to construct components for a test case result based on the failure mode
+        assessment of non-empty validation messages (which are also returned).
 
         :param tcr: TestCaseRun containing reasoner-validator style validation message from test execution.
         :return: Tuple[str, TestCaseResultEnum, Dict], where position 0 is the target,
-                 position 1 is the testcase status (passed/failed/skipped) and
+                 position 1 is the testcase TestCaseResultEnum status (PASSED|FAILED|SKIPPED) and
                  position 2 is a (possible empty) dictionary of non-empty validation messages
         """
         target: str = tcr.default_target
         test: str = tcr.default_test
         messages_by_target: MESSAGES_BY_TARGET = tcr.get_all_messages()
         if target in messages_by_target:
             messages_by_test: MESSAGES_BY_TEST = messages_by_target[target]
@@ -305,33 +302,34 @@
 
     def format_results(self, test_cases: List[TestCaseRun]) -> Dict:
         """
         This function normalizes and restructures TestCaseRun
         results for the upstream consumer of TestRunner results.
 
         :param test_cases: List[TestCaseRun], list of Test Case runs with results.
-
-        :return: Dict, of structured test message results for all TestCases,
+        :return: Dict, structured test PASSED/FAILED/SKIPPED status and message
+                       results for all TestCases, indexed by a "test_case_id"
+                       of format "<test_asset_id>-<test_name>" "test_name" as
                        specified by TRAPI generators of a given test run.
         """
         # Originally, the results == [tc.get_all_messages() for tc in test_cases], which gives
         # [
-        #    {
-        #        'molepro': {
+        #    {   # components are "ars", ARA or KP infores object references
+        #        '<component_id>': {
         #            'by_subject': {
         #                'info': {},
         #                'skipped': {},
         #                'warning': {},
         #                'error': {},
         #                'critical': {}
         #            }
         #        }
         #    },
         #    {
-        #        'molepro': {
+        #        '<component_id>': {
         #            'inverse_by_new_subject': {
         #                'info': {},
         #                'skipped': {},
         #                'warning': {},
         #                'error': {
         #                    'error.trapi.response.knowledge_graph.missing_expected_edge': {
         #                        'global': {
@@ -351,19 +349,26 @@
         # with the source test_asset as recorded within the test_case.test_run.test_asset property. Note that all the
         # test case message blocks have the same testing target component (although that doesn't have to be the case).
         #
         # We probably need to return something more like the following (using the source test asset information...):
         #
         # results == {
         #     "<test_case_id_1>": {
-        #         "molepro": <result_1>,
+        #         "<component_1>": {
+        #            "status: <PASSED|FAILED|SKIPPED>, # for result 1
+        #            "messages": <reasoner-validator formatted message partition>
+        #         }
+        #         "<component_2>": {
+        #            "status: <PASSED|FAILED|SKIPPED>, # for 'test_case_id_1' from 'component_2'
+        #            "messages": <reasoner-validator formatted message partition>
+        #         }
         #         etc...
         #     }
         #     "<test case id 2>": {
-        #         "molepro": <result 2>,
+        #         "<component_1>": <result 2>,
         #         etc...
         #     }
         #     etc...
         # ]
         # where the 'test_asset_id_#' is something sensible, probably composite of the test asset identifier and
         # the identifier of the test template method used to generate the TestCase-specific TRAPI query.
         #
@@ -373,32 +378,43 @@
         #
         # How should these messages be binned into test PASSED or FAILED? Should “PASSED” only be tolerant of
         # “information” messages? Are “skipped test” messages indicative of a failed test?
         #
         # Are “Warnings” to also be taken as an indication of a test failure? Could/should we give TestRunner
         # “stringency” indications which affect whether “skipped” and “warnings” are returned as “PASSED”?
         #
-        # The above <result_#> could be a 2-Tuple of (<PASSED|FAILED>, <pruned message catalog>) where the message
-        # catelog is a Python dictionary pruned of all empty reasoner-validator validation message partitions,
+        # The above <result_#> could be a dictionary of format:
+        #
+        # {
+        #     "status": "<PASSED|FAILED|SKIPPED>",
+        #     "messages": "<pruned message catalog>"
+        # }
+        #
+        # where the message catalog is a Python dictionary pruned of all empty reasoner-validator message partitions,
         # where the status of the test is determined by the aforementioned stringency rules, however coded.
         #
         results: Dict = dict()
         for tcr in test_cases:
             # TODO: not sure how robust this is: will the 'id' always be defined?
             test_asset_id: str = tcr.test_run.test_asset.id
             test_name: str = tcr.default_test
             test_case_id: str = f"{test_asset_id}-{test_name}"
             if test_case_id not in results:
                 results[test_case_id] = dict()
-            target: str
+            component: str
             status: TestCaseResultEnum
             messages: MESSAGE_CATALOG
-            target, status, messages = self.compute_status(tcr)
-            # TODO: we blissfully assume that targets only come up once for a given test_case_id
-            results[test_case_id][target] = (status, messages)
+            component, status, messages = self.compute_status(tcr)
+            # TODO: sanity check? we blissfully assume that a 'component'
+            #       is only reported once for a given 'test_case_id'
+            assert component not in results[test_case_id]
+            results[test_case_id][component] = {
+                "status": status,
+                "messages": messages
+            }
 
         return results
 
     async def process_test_run(self, **kwargs) -> Dict:
         """
         Applies a TestCase generator giving a specific subclass
         of TestCaseRun, wrapping queries defined by test-specific
@@ -429,16 +445,16 @@
             test_asset_id: str,
             subject_id: str,
             subject_category: str,
             predicate_id: str,
             object_id: str,
             object_category: str,
             trapi_generators: List,
-            environment: Optional[TestEnvEnum] = TestEnvEnum.ci,
-            components: Optional[List[ComponentEnum]] = None,
+            environment: Optional[str] = "ci",
+            components: Optional[List[str]] = None,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             runner_settings: Optional[List[str]] = None,
             **kwargs
     ) -> Dict[str, Dict]:
         """
         Run one or more Graph Validation tests, of specified category of test,
@@ -459,28 +475,28 @@
 
         - TRAPI JSON query generators for the TestCases using the specified TestAsset
         :param trapi_generators: List, pointers to code functions that
                                  configure an individual TRAPI query request.
                                  See one_hop_test.unit_test_templates.
 
         - Target endpoint(s) to be tested - one test report or report set generated per endpoint provided.
-        :param components: Optional[List[ComponentEnum]] = None, comma-delimited list of components to be tested
+        :param components: Optional[List[str]] = None, comma-delimited list of components to be tested
                            (Values specified in ComponentEnum in TranslatorTestingModel; default ['ars'])
         :param environment: Optional[str] = None, Target Translator execution environment for the test,
                             one of 'dev', 'ci', 'test' or 'prod' (default: 'ci')
 
         - Metadata globally configuring the test(s) to be run.
         :param trapi_version: Optional[str] = None, target TRAPI version (default: latest public release)
         :param biolink_version: Optional[str] = None, target Biolink Model version (default: Biolink toolkit release)
         :param runner_settings: Optional[List[str]] = None, extra string parameters to the Test Runner
         :param kwargs: Dict, optional extra named parameters to passed to TestCase TestRunner.
         :return: Dict { "pks": Dict[<target>, <pk>], "results": Dict[<test_case_id>, <test_case_results>] }
         """
         if not components:
-            components = [ComponentEnum('ars')]
+            components = ['ars']
 
         # TODO: (April 2024) short term limitation: can't test ARS endpoints, see the missing ARS code in
         #       the run_trapi_query() method of the graph_validation_test.translator.trapi package module.
         if 'ars' in components:
             logger.error("Default ARS testing is not yet supported by GraphValidationTests")
             return dict()
 
@@ -588,18 +604,19 @@
     #     --runner_settings 'inferred'
 
     parser = ArgumentParser(description=tool_name)
 
     parser.add_argument(
         "--components",
         type=str,
+        choices=get_available_components(),
         required=True,  # TODO: later, if and when implemented, the default could become 'ars' if unspecified...
-        help="Names Translator components to be tested taken from the Translator Testing Model 'ComponentEnum'; " +
+        help="Names Translator components to be tested, taken from the Translator Testing Model 'ComponentEnum'; " +
              "which may be a comma separated string of such names (e.g. 'arax,molepro')"
-             # "(Default: if unspecified, the test is run against the 'ars')",
+        # "(Default: if unspecified, the test is run against the 'ars')",
         # default=None
     )
 
     parser.add_argument(
         "--environment",
         type=str,
         choices=['dev', 'ci', 'test', 'prod'],
@@ -670,13 +687,14 @@
         nargs='+',
         help="Scalar settings for the TestRunner, e.g. 'inferred'",
         default=None
     )
 
     args = parser.parse_args()
 
-    # convert any comma-delimited string of components infores
-    # identifiers into the expected List of ComponentEnum entries
+    # convert any comma-delimited string of components
+    # ComponentEnum enumerated identifiers
+    # into the expected List of entries
     if "components" in args:
-        args["components"] = [ComponentEnum(entry) for entry in args["components"].split(",")]
+        args["components"] = [entry for entry in args["components"].split(",")]
 
     return args
```

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/translator/registry/__init__.py` & `graph_validation_tests-0.0.9/graph_validation_test/translator/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/translator/trapi/__init__.py` & `graph_validation_tests-0.0.9/graph_validation_test/translator/trapi/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Code to submit GraphValidation test queries to
 Translator components - ARS, ARA, KP - via TRAPI
 """
-from typing import Optional, Dict
+from typing import Optional, Dict, List
 from functools import lru_cache
 import requests
 
 from reasoner_validator.trapi import call_trapi
+
 from graph_validation_test.translator.registry import (
     DEPLOYMENT_TYPE_MAP,
     get_the_registry_data,
     get_component_endpoint_from_registry
 )
 
 from logging import getLogger
@@ -154,30 +155,58 @@
 
         except Exception as e:
             print(f"Cannot decode ARS PK '{response_id}' to a Translator Response, exception: {e}")
 
     return trapi_response
 
 
-def get_component_infores_object_id(component: str) -> str:
+# TODO: the ComponentEnum in the TranslatorTestingModel has the full list
+#       of available Translator components against their InfoRes but the
+#       Pydantic model does not yet publish thus the hacky patch here...
+_infores_obj_id_map = {
+    "ars": "ncats-ars",
+
+    # ARA's
+    "arax": "arax",
+    "explanatory": "explanatory-agent",
+    "improving": "improving-agent",
+    "aragorn": "aragorn",
+    "bte": "biothings-explorer",
+    "unsecret": "unsecret-agent",
+
+    # KP's
+    "rtxkg2": "rtx-kg2",
+    "icees": "icees-kg",
+    "cam": "cam-kp",
+    "spoke": "spoke",
+    "molepro": "molepro",
+    "genetics": "genetics-data-provider",
+    "textmining": "textmining-kp",
+    "cohd": "cohd",
+    "openpredict": "openpredict",
+    "collaboratory": "knowledge-collaboratory",
+    "connections": "connections-hypothesis"
+}
+
+
+def get_available_components() -> List[str]:
+    return list(_infores_obj_id_map.keys())
+
+
+def get_component_infores_object_id(component: str) -> Optional[str]:
     """
     Returns the InfoRes object identifier of a given component.
     :param component: str, acronym of the component
     :return: infores reference identifier of the component
     """
     # TODO: can I resolve here whether a given component
     #       is an ARA or a KP, and return this to the caller?
-    assert component
-    infores_map = {
-        "arax": "arax",
-        "aragorn": "aragorn",
-        "bte": "biothings-explorer",
-        "improving": "improving-agent",
-    }
-    return infores_map.setdefault(component, component)
+    if component not in _infores_obj_id_map.keys():
+        return None
+    return _infores_obj_id_map[component]
 
 
 @lru_cache()
 def resolve_component_endpoint(
         component: Optional[str],
         environment: Optional[str],
         target_trapi_version: Optional[str],
```

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/utils/asyncio.py` & `graph_validation_tests-0.0.9/graph_validation_test/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/utils/http.py` & `graph_validation_tests-0.0.9/graph_validation_test/utils/http.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/utils/ontology_kp.py` & `graph_validation_tests-0.0.9/graph_validation_test/utils/ontology_kp.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/graph_validation_test/utils/unit_test_templates.py` & `graph_validation_tests-0.0.9/graph_validation_test/utils/unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/one_hop_test/__init__.py` & `graph_validation_tests-0.0.9/one_hop_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/pyproject.toml` & `graph_validation_tests-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graph-validation-tests"
-version = "0.0.8"
+version = "0.0.9"
 description = "Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Chris Bizon <bizon.renci.org>",
     "Tim Putnam <tim@tislab>"
 ]
 maintainers = ["Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
@@ -43,23 +43,23 @@
 ]
 
 include = [
     { path = "tests" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.10,<3.12"
 deepdiff = "^6.7.1"
 
 #reasoner-validator = { git = "https://github.com/NCATSTranslator/reasoner-validator.git", branch = "graph-validation-test-revisions" }
-reasoner-validator = "^4.0.1"
+reasoner-validator = "^4.0.2"
 
 #translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", rev = "ef5d68e" }
-#translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", branch = "fix-TestCaseResultEnum-values" }
-translator-testing-model = "^0.2.7"
+#translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", branch = "main" }
+translator-testing-model = "^0.3.1"
 
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.3"
 fastapi = "*"
 httpx = "^0.27.0"
 tqdm = "^4.66.2"
 
@@ -95,8 +95,7 @@
 log_cli_level = "INFO"
 log_cli_format = "%(message)s"
 
 log_file = "pytest.log"
 log_file_level = "INFO"
 log_file_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_file_date_format = "%Y-%m-%d %H:%M:%S"
-
```

### Comparing `graph_validation_tests-0.0.8/standards_validation_test/__init__.py` & `graph_validation_tests-0.0.9/standards_validation_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/__init__.py` & `graph_validation_tests-0.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/graph_validation_test/test_graph_validation_test.py` & `graph_validation_tests-0.0.9/tests/graph_validation_test/test_graph_validation_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Unit tests for pieces of the GraphValidationTests code
 """
+from typing import List, Dict
 from translator_testing_model.datamodel.pydanticmodel import TestAsset
 from graph_validation_test import TestCaseRun, GraphValidationTest
 from graph_validation_test.utils.unit_test_templates import by_subject, by_object
 from tests import DEFAULT_TRAPI_VERSION, DEFAULT_BMT
 
 import logging
 logger = logging.getLogger(__name__)
@@ -95,7 +96,38 @@
     info = tcr.get_info()
     assert len(info) == 1
     assert "info.compliant" in info
     tcr.report(code="skipped.test", identifier="Non-standards compliant input?")
     skipped = tcr.get_skipped()
     assert len(skipped) == 1
     assert "skipped.test" in skipped
+
+
+def test_format_results():
+    test_asset_id: str = "TestAsset_1"
+    test_asset: TestAsset = TestAsset(id=test_asset_id)
+    gvt: GraphValidationTest = GraphValidationTest(
+        test_asset=test_asset
+    )
+    tcr_1: TestCaseRun = TestCaseRun(
+        test_run=gvt,
+        test=by_subject
+    )
+    tcr_2: TestCaseRun = TestCaseRun(
+        test_run=gvt,
+        test=by_object
+    )
+    test_cases: List[TestCaseRun] = [
+        tcr_1,
+        tcr_2
+    ]
+    formatted_output: Dict = gvt.format_results(test_cases)
+    assert formatted_output
+    by_subject_test_case_id: str = f"{test_asset_id}-by_subject"
+    assert formatted_output[by_subject_test_case_id]
+    by_object_test_case_id: str = f"{test_asset_id}-by_object"
+    assert formatted_output[by_object_test_case_id]
+    assert "ars" in formatted_output[by_object_test_case_id]
+    assert formatted_output[by_object_test_case_id]["ars"]
+    assert "status" in formatted_output[by_object_test_case_id]["ars"]
+    assert formatted_output[by_object_test_case_id]["ars"]["status"] == "SKIPPED"
+    assert not formatted_output[by_object_test_case_id]["ars"]["messages"]
```

### Comparing `graph_validation_tests-0.0.8/tests/graph_validation_test/test_unit_test_templates.py` & `graph_validation_tests-0.0.9/tests/graph_validation_test/test_unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/graph_validation_test/translator/biolink/test_ontology_kp.py` & `graph_validation_tests-0.0.9/tests/graph_validation_test/translator/biolink/test_ontology_kp.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/graph_validation_test/translator/test_translator_smartapi_registry.py` & `graph_validation_tests-0.0.9/tests/graph_validation_test/translator/test_translator_smartapi_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,15 +476,15 @@
         assert not resource_metadata
 
 
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
-        ("aragorn", "ci", "https://aragorn.ci.transltr.io/aragorn"),
+        ("aragorn", "prod", "https://aragorn.transltr.io/aragorn"),
         ("biothings-explorer", "test", "https://bte.test.transltr.io/v1"),
         ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
         ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None)
     ]
 )
 def test_get_component_endpoint_from_registry(
```

### Comparing `graph_validation_tests-0.0.8/tests/graph_validation_test/translator/trapi/test_trapi.py` & `graph_validation_tests-0.0.9/tests/graph_validation_test/translator/trapi/test_trapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 )
 
 pytest_plugins = ('pytest_asyncio',)
 
 TRAPI_TEST_ENDPOINT = "https://molepro-trapi.transltr.io/molepro/trapi/v1.4"
 
 
-def test_empty_get_component_infores_object_id():
-    with pytest.raises(AssertionError):
-        assert get_component_infores_object_id(component="")
-
-
 @pytest.mark.parametrize(
     "component,infores",
     [
         ("arax", "arax"),
         ("aragorn", "aragorn"),
         ("bte", "biothings-explorer"),
         ("improving", "improving-agent"),
@@ -42,17 +37,17 @@
     "component,environment,result",
     [
         (None, None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", "non-environment", None),
         ("ars", "test", f"https://ars.test.transltr.io/ars/api/"),
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
-        ("aragorn", "ci", "https://aragorn.ci.transltr.io/aragorn"),
-        ("biothings-explorer", "test", "https://bte.test.transltr.io/v1"),
-        ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
+        ("aragorn", "prod", "https://aragorn.transltr.io/aragorn"),
+        ("bte", "test", "https://bte.test.transltr.io/v1"),
+        ("improving", "test", "https://ia.test.transltr.io/api/v1.4/"),
         ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None),
         ("arax", "non-environment", None),
     ]
 )
 def test_resolve_component_endpoint(
         component: Optional[str],
```

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_one_hop_test.py` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_one_hop_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 """
 Unit tests for One Hop Test code validation
 """
 from sys import stdout, stderr
-from typing import List, Dict
+from typing import Dict
 from json import dump
 import subprocess
 import pytest
 
-from translator_testing_model.datamodel.pydanticmodel import (
-    TestEnvEnum,
-    ComponentEnum
-)
 from graph_validation_test.utils.unit_test_templates import (
     by_subject,
     inverse_by_new_subject,
     by_object,
     raise_subject_entity,
     raise_object_entity,
     raise_object_by_subject,
@@ -34,19 +30,16 @@
         raise_object_entity,
         raise_object_by_subject,
         raise_predicate_by_subject
     ]
     results: Dict = await OneHopTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.prod,
-        components=[
-            ComponentEnum("arax"),
-            ComponentEnum("molepro")
-        ]
+        environment="prod",
+        components=["arax", "molepro"]
     )
     dump(results, stderr, indent=4)
 
 
 # ARS tests not yet supported so yes... results will
 # always be empty, with a logger message to inform why
 @pytest.mark.asyncio
@@ -59,42 +52,36 @@
         raise_object_entity,
         raise_object_by_subject,
         raise_predicate_by_subject
     ]
     results: Dict = await OneHopTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.prod
+        environment="prod"
     )
     assert not results
 
 
 @pytest.mark.asyncio
 async def test_run_one_hop_tests():
     results: Dict = await run_one_hop_tests(
         **SAMPLE_TEST_INPUT_1,
-        environment=TestEnvEnum.prod,
-        components=[
-            ComponentEnum("arax"),
-            ComponentEnum("molepro")
-        ]
+        environment="prod",
+        components=["arax", "molepro"]
     )
     assert results
     dump(results, stderr, indent=4)
 
 
 @pytest.mark.asyncio
 async def test_run_one_hop_tests_with_runner_parameters():
     results: Dict = await run_one_hop_tests(
         **SAMPLE_TEST_INPUT_1,
-        environment=TestEnvEnum.prod,
-        components=[
-            ComponentEnum("arax"),
-            ComponentEnum("molepro")
-        ],
+        environment="prod",
+        components=["arax", "molepro"],
         strict_validation=True
     )
     assert results
     dump(results, stderr, indent=4)
 
 
 # subprocess.run(
@@ -105,14 +92,13 @@
 # )
 @pytest.mark.skip("Not yet fully implemented")
 def test_one_hop_cli():
     # command: List = ["python", "-m", "one_hop_test.__init__"]
     # args: Dict = SAMPLE_TEST_INPUT_1.copy()
     # args["components"] = "arax,molepro"
     # [command.extend([f"--{flag}", value]) for flag, value in args.items()]
-    # results = check_output(command)
     # results = check_output(["dir"])
     # results = check_output([
     #     "python", "-m", "venv", "--clear", "test_venv", ";",
     #     ".", "test_venv/bin/activate"
     # ])
     subprocess.run("one_hop_test", stdout=stdout, shell=True, cwd=SCRIPTS_DIR)
```

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/Activate.ps1` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/activate` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/activate.bat` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pip.exe` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pip3.10.exe` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pip3.10.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pip3.exe` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/python.exe` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/one_hop_test/test_venv/Scripts/pythonw.exe` & `graph_validation_tests-0.0.9/tests/one_hop_test/test_venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.8/tests/standards_validation_test/test_standards_validation_test.py` & `graph_validation_tests-0.0.9/tests/standards_validation_test/test_standards_validation_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,34 +2,30 @@
 Unit tests for Standards Validation Test code validation
 """
 from sys import stderr
 from typing import Dict
 from json import dump
 import pytest
 
-from translator_testing_model.datamodel.pydanticmodel import TestEnvEnum, ComponentEnum
 from graph_validation_test.utils.unit_test_templates import by_subject, by_object
 from standards_validation_test import StandardsValidationTest, run_standards_validation_tests
 from tests import SAMPLE_TEST_INPUT_1
 
 
 @pytest.mark.asyncio
 async def test_standards_validation_test():
     trapi_generators = [
         by_subject,
         by_object
     ]
     results: Dict = await StandardsValidationTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.prod,
-        components=[
-            ComponentEnum("arax"),
-            ComponentEnum("molepro")
-        ]
+        environment="prod",
+        components=["arax", "molepro"]
     )
     dump(results, stderr, indent=4)
 
 
 # ARS tests not yet supported so yes... results will
 # always be empty, with a logger message to inform why
 @pytest.mark.asyncio
@@ -37,24 +33,21 @@
     trapi_generators = [
         by_subject,
         by_object
     ]
     results: Dict = await StandardsValidationTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.prod
+        environment="prod"
     )
     assert not results
 
 
 @pytest.mark.asyncio
 async def test_run_standards_validation_tests():
     results: Dict = await run_standards_validation_tests(
         **SAMPLE_TEST_INPUT_1,
-        environment=TestEnvEnum.prod,
-        components=[
-            ComponentEnum("arax"),
-            ComponentEnum("molepro")
-        ]
+        environment="prod",
+        components=["arax", "molepro"]
     )
     assert results
     dump(results, stderr, indent=4)
```

### Comparing `graph_validation_tests-0.0.8/PKG-INFO` & `graph_validation_tests-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: graph-validation-tests
-Version: 0.0.8
+Version: 0.0.9
 Summary: Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation
 Home-page: https://github.com/TranslatorSRI
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
 Maintainer-email: richard.bruskiewich@delphinai.com
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
 Requires-Dist: fastapi
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.3,<0.24.0)
-Requires-Dist: reasoner-validator (>=4.0.1,<5.0.0)
+Requires-Dist: reasoner-validator (>=4.0.2,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
-Requires-Dist: translator-testing-model (>=0.2.7,<0.3.0)
+Requires-Dist: translator-testing-model (>=0.3.1,<0.4.0)
 Project-URL: Bug Tracker, https://github.com/TranslatorSRI/GraphValidationTests/issues
 Project-URL: Change Log, https://github.com/TranslatorSRI/GraphValidationTests/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/TranslatorSRI/GraphValidationTests/blob/main/README.md
 Project-URL: Repository, https://github.com/TranslatorSRI/GraphValidationTests
 Description-Content-Type: text/markdown
 
 # Graph Validation Tests
@@ -242,59 +242,53 @@
 Note that the trapi_generation variables - defined in the **graph_validation_test.utils.unit_test_templates** module - are all simply Python functions returning TRAPI JSON messages to send to the target components. In principle, if one understands what those functions are doing, you could write your own methods to do other kinds of TRAPI queries whose output can then be validated against the specified TRAPI and Biolink Model releases.
 
 ### Sample Output
 
 This is a sample of what the JSON output from test runs currently looks like (this sample came from a OneHopTest run).
 
 ```json
-{
-    "pks": [
-        "arax",
-        "molepro"
-    ],
-    "results": [
-        [
-            {
-                "arax": {
-                    "by_subject": {
-                        "info": {},
-                        "skipped": {},
-                        "warning": {},
-                        "error": {
-                            "error.trapi.response.knowledge_graph.missing_expected_edge": {
-                                "global": {
-                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:has_side_effect]->(MONDO:0011426#biolink:Disease)": null
-                                }
+{    
+    "pks": {
+        "molepro": "molepro"
+    },
+    "results": {
+        "TestAsset_1-by_subject": {
+            "molepro": {
+                "status": "FAILED",
+                "messages": {
+                    "error": {
+                        "error.trapi.response.knowledge_graph.missing_expected_edge": {
+                            "global": {
+                                "TestAsset_1|(CHEBI:58579#biolink:SmallMolecule)-[biolink:is_active_metabolite_of]->(UniProtKB:Q9NQ88#biolink:Protein)": null
                             }
-                        },
-                        "critical": {}
+                        }
                     }
                 }
-            },
-"etc ...",
-            {
-                "molepro": {
-                    "by_subject": {
-                        "info": {},
-                        "skipped": {},
-                        "warning": {},
-                        "error": {
-                            "error.trapi.response.knowledge_graph.missing_expected_edge": {
-                                "global": {
-                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:has_side_effect]->(MONDO:0011426#biolink:Disease)": null
-                                }
+            }
+        },
+        "TestAsset_1-inverse_by_new_subject": {
+            "molepro": {
+                "status": "FAILED",
+                "messages": {
+                    "critical": {
+                        "critical.trapi.request.invalid": {
+                            "global": {
+                                "predicate 'biolink:is_active_metabolite_of'": [
+                                    {
+                                        "context": "inverse_by_new_subject",
+                                        "reason": "is an unknown or has no inverse?"
+                                    }
+                                ]
                             }
-                        },
-                        "critical": {}
+                        }
                     }
                 }
-            },
-etc...
-        ]
-    ]
+            }
+        },
+        # etc...
 }
 ```
 
 ## Releases
 
 A [full change log](CHANGELOG.md) is provided documenting each release, but we summarize key release limitations here:
```

