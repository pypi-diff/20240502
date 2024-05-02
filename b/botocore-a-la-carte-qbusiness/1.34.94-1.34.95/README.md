# Comparing `tmp/botocore-a-la-carte-qbusiness-1.34.94.tar.gz` & `tmp/botocore-a-la-carte-qbusiness-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-qbusiness-1.34.94.tar", last modified: Tue Apr 30 01:01:40 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-qbusiness-1.34.95.tar", last modified: Wed May  1 01:06:33 2024, max compression
```

## Comparing `botocore-a-la-carte-qbusiness-1.34.94.tar` & `botocore-a-la-carte-qbusiness-1.34.95.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:40.431318 botocore-a-la-carte-qbusiness-1.34.94/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-30 01:01:40.000000 botocore-a-la-carte-qbusiness-1.34.94/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-30 01:01:40.431318 botocore-a-la-carte-qbusiness-1.34.94/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:40.427318 botocore-a-la-carte-qbusiness-1.34.94/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:40.427318 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:40.427318 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:40.431318 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-30 01:01:14.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-30 01:01:14.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-30 01:01:14.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (127)   238125 2024-04-30 01:01:14.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:40.431318 botocore-a-la-carte-qbusiness-1.34.94/botocore_a_la_carte_qbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-30 01:01:40.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore_a_la_carte_qbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 01:01:40.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore_a_la_carte_qbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:01:40.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore_a_la_carte_qbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 01:01:40.000000 botocore-a-la-carte-qbusiness-1.34.94/botocore_a_la_carte_qbusiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:01:40.431318 botocore-a-la-carte-qbusiness-1.34.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-30 01:01:40.000000 botocore-a-la-carte-qbusiness-1.34.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.384765 botocore-a-la-carte-qbusiness-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-01 01:06:33.000000 botocore-a-la-carte-qbusiness-1.34.95/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 01:06:33.384765 botocore-a-la-carte-qbusiness-1.34.95/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.380764 botocore-a-la-carte-qbusiness-1.34.95/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.380764 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.380764 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.384765 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-05-01 01:06:02.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-01 01:06:02.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 01:06:02.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (127)   261247 2024-05-01 01:06:02.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 01:06:02.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.384765 botocore-a-la-carte-qbusiness-1.34.95/botocore_a_la_carte_qbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 01:06:33.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore_a_la_carte_qbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-01 01:06:33.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore_a_la_carte_qbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:06:33.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore_a_la_carte_qbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 01:06:33.000000 botocore-a-la-carte-qbusiness-1.34.95/botocore_a_la_carte_qbusiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:06:33.384765 botocore-a-la-carte-qbusiness-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-01 01:06:33.000000 botocore-a-la-carte-qbusiness-1.34.95/setup.py
```

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/LICENSE.txt` & `botocore-a-la-carte-qbusiness-1.34.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/PKG-INFO` & `botocore-a-la-carte-qbusiness-1.34.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-qbusiness
-Version: 1.34.94
+Version: 1.34.95
 Summary: qbusiness data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/endpoint-rule-set-1.json` & `botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/paginators-1.json` & `botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/botocore/data/qbusiness/2023-11-27/service-2.json` & `botocore-a-la-carte-qbusiness-1.34.95/botocore/data/qbusiness/2023-11-27/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8620520615886157%*

 * *Differences: {"'documentation'": "'<p>This is the <i>Amazon Q Business</i> API Reference. Amazon Q Business is "*

 * *                    'a fully managed, generative-AI powered enterprise chat assistant that you can '*

 * *                    'deploy within your organization. Amazon Q Business enhances employee '*

 * *                    'productivity by supporting key tasks such as question-answering, knowledge '*

 * *                    'discovery, writing email messages, summarizing text, drafting document '*

 * *                    'outlin […]*

```diff
@@ -1,14 +1,19 @@
 {
-    "documentation": "<note> <p>Amazon Q is in preview release and is subject to change.</p> </note> <p>This is the <i>Amazon Q Business</i> API Reference. Amazon Q Business is a fully managed, generative-AI powered enterprise chat assistant that you can deploy within your organization. Amazon Q Business enhances employee productivity by supporting key tasks such as question-answering, knowledge discovery, writing email messages, summarizing text, drafting document outlines, and brainstorming ideas. Users ask questions of Amazon Q Business and get answers that are presented in a conversational manner. For an introduction to the service, see the <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/what-is.html\"> <i>Amazon Q Business User Guide</i> </a>.</p> <p>For an overview of the Amazon Q Business APIs, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/api-ref.html#api-overview\">Overview of Amazon Q Business API operations</a>.</p> <p>For information about the IAM access control permissions you need to use this API, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/iam-roles.html\">IAM roles for Amazon Q Business</a> in the <i>Amazon Q Business User Guide</i>.</p> <p>You can use the following AWS SDKs to access Amazon Q Business APIs:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-cpp\">AWS SDK for C++</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-go\">AWS SDK for Go</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-java\">AWS SDK for Java</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-javascript\">AWS SDK for JavaScript</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-net\">AWS SDK for .NET</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/pythonsdk\">AWS SDK for Python (Boto3)</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-ruby\">AWS SDK for Ruby</a> </p> </li> </ul> <p>The following resources provide additional information about using the Amazon Q Business API:</p> <ul> <li> <p> <i> <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/setting-up.html\">Setting up for Amazon Q Business</a> </i> </p> </li> <li> <p> <i> <a href=\"https://awscli.amazonaws.com/v2/documentation/api/latest/reference/qbusiness/index.html\">Amazon Q Business CLI Reference</a> </i> </p> </li> <li> <p> <i> <a href=\"https://docs.aws.amazon.com/general/latest/gr/amazonq.html\">Amazon Web Services General Reference</a> </i> </p> </li> </ul>",
+    "documentation": "<p>This is the <i>Amazon Q Business</i> API Reference. Amazon Q Business is a fully managed, generative-AI powered enterprise chat assistant that you can deploy within your organization. Amazon Q Business enhances employee productivity by supporting key tasks such as question-answering, knowledge discovery, writing email messages, summarizing text, drafting document outlines, and brainstorming ideas. Users ask questions of Amazon Q Business and get answers that are presented in a conversational manner. For an introduction to the service, see the <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/what-is.html\"> <i>Amazon Q Business User Guide</i> </a>.</p> <p>For an overview of the Amazon Q Business APIs, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/api-ref.html#api-overview\">Overview of Amazon Q Business API operations</a>.</p> <p>For information about the IAM access control permissions you need to use this API, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/iam-roles.html\">IAM roles for Amazon Q Business</a> in the <i>Amazon Q Business User Guide</i>.</p> <p>You can use the following AWS SDKs to access Amazon Q Business APIs:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-cpp\">AWS SDK for C++</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-go\">AWS SDK for Go</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-java\">AWS SDK for Java</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-javascript\">AWS SDK for JavaScript</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-net\">AWS SDK for .NET</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/pythonsdk\">AWS SDK for Python (Boto3)</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sdk-for-ruby\">AWS SDK for Ruby</a> </p> </li> </ul> <p>The following resources provide additional information about using the Amazon Q Business API:</p> <ul> <li> <p> <i> <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/setting-up.html\">Setting up for Amazon Q Business</a> </i> </p> </li> <li> <p> <i> <a href=\"https://awscli.amazonaws.com/v2/documentation/api/latest/reference/qbusiness/index.html\">Amazon Q Business CLI Reference</a> </i> </p> </li> <li> <p> <i> <a href=\"https://docs.aws.amazon.com/general/latest/gr/amazonq.html\">Amazon Web Services General Reference</a> </i> </p> </li> </ul>",
     "metadata": {
         "apiVersion": "2023-11-27",
         "endpointPrefix": "qbusiness",
-        "jsonVersion": "1.1",
         "protocol": "rest-json",
+        "protocolSettings": {
+            "h2": "eventstream"
+        },
+        "protocols": [
+            "rest-json"
+        ],
         "serviceFullName": "QBusiness",
         "serviceId": "QBusiness",
         "signatureVersion": "v4",
         "signingName": "qbusiness",
         "uid": "qbusiness-2023-11-27"
     },
     "operations": {
@@ -81,14 +86,52 @@
                 "shape": "BatchPutDocumentRequest"
             },
             "name": "BatchPutDocument",
             "output": {
                 "shape": "BatchPutDocumentResponse"
             }
         },
+        "Chat": {
+            "documentation": "<p>Starts or continues a streaming Amazon Q Business conversation.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "LicenseNotFoundException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/applications/{applicationId}/conversations",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ChatInput"
+            },
+            "name": "Chat",
+            "output": {
+                "shape": "ChatOutput"
+            }
+        },
         "ChatSync": {
             "documentation": "<p>Starts or continues a non-streaming Amazon Q Business conversation.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -120,15 +163,15 @@
             },
             "name": "ChatSync",
             "output": {
                 "shape": "ChatSyncOutput"
             }
         },
         "CreateApplication": {
-            "documentation": "<p>Creates an Amazon Q Business application.</p>",
+            "documentation": "<p>Creates an Amazon Q Business application.</p> <note> <p>There are new tiers for Amazon Q Business. Not all features in Amazon Q Business Pro are also available in Amazon Q Business Lite. For information on what's included in Amazon Q Business Lite and what's included in Amazon Q Business Pro, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/what-is.html#tiers\">Amazon Q Business tiers</a>. You must use the Amazon Q Business console to assign subscription tiers to users.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "InternalServerException"
                 },
@@ -1939,14 +1982,35 @@
             "name": "UpdateWebExperience",
             "output": {
                 "shape": "UpdateWebExperienceResponse"
             }
         }
     },
     "shapes": {
+        "APISchema": {
+            "documentation": "<p>Contains details about the OpenAPI schema for a custom plugin. For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/custom-plugin.html#plugins-api-schema\">custom plugin OpenAPI schemas</a>. You can either include the schema directly in the payload field or you can upload it to an S3 bucket and specify the S3 bucket location in the <code>s3</code> field. </p>",
+            "members": {
+                "payload": {
+                    "documentation": "<p>The JSON or YAML-formatted payload defining the OpenAPI schema for a custom plugin. </p>",
+                    "shape": "Payload"
+                },
+                "s3": {
+                    "documentation": "<p>Contains details about the S3 object containing the OpenAPI schema for a custom plugin. The schema could be in either JSON or YAML format.</p>",
+                    "shape": "S3"
+                }
+            },
+            "type": "structure",
+            "union": true
+        },
+        "APISchemaType": {
+            "enum": [
+                "OPEN_API_V3"
+            ],
+            "type": "string"
+        },
         "AccessConfiguration": {
             "documentation": "<p>Used to configure access permissions for a document.</p>",
             "members": {
                 "accessControls": {
                     "documentation": "<p>A list of <code>AccessControlList</code> objects.</p>",
                     "shape": "AccessControls"
                 },
@@ -2013,17 +2077,41 @@
                 },
                 "pluginId": {
                     "documentation": "<p>The identifier of the plugin the action is attached to.</p>",
                     "shape": "PluginId"
                 }
             },
             "required": [
+                "pluginId",
                 "payload",
-                "payloadFieldNameSeparator",
-                "pluginId"
+                "payloadFieldNameSeparator"
+            ],
+            "type": "structure"
+        },
+        "ActionExecutionEvent": {
+            "documentation": "<p>A request from an end user signalling an intent to perform an Amazon Q Business plugin action during a streaming chat.</p>",
+            "event": true,
+            "members": {
+                "payload": {
+                    "documentation": "<p>A mapping of field names to the field values in input that an end user provides to Amazon Q Business requests to perform their plugin action. </p>",
+                    "shape": "ActionExecutionPayload"
+                },
+                "payloadFieldNameSeparator": {
+                    "documentation": "<p>A string used to retain information about the hierarchical contexts within a action execution event payload.</p>",
+                    "shape": "ActionPayloadFieldNameSeparator"
+                },
+                "pluginId": {
+                    "documentation": "<p>The identifier of the plugin for which the action is being requested.</p>",
+                    "shape": "PluginId"
+                }
+            },
+            "required": [
+                "pluginId",
+                "payload",
+                "payloadFieldNameSeparator"
             ],
             "type": "structure"
         },
         "ActionExecutionPayload": {
             "key": {
                 "shape": "ActionPayloadFieldKey"
             },
@@ -2086,30 +2174,73 @@
                 "pluginType": {
                     "documentation": "<p>The type of plugin.</p>",
                     "shape": "PluginType"
                 }
             },
             "type": "structure"
         },
+        "ActionReviewEvent": {
+            "documentation": "<p>An output event that Amazon Q Business returns to an user who wants to perform a plugin action during a streaming chat conversation. It contains information about the selected action with a list of possible user input fields, some pre-populated by Amazon Q Business. </p>",
+            "event": true,
+            "members": {
+                "conversationId": {
+                    "documentation": "<p>The identifier of the conversation with which the action review event is associated.</p>",
+                    "shape": "ConversationId"
+                },
+                "payload": {
+                    "documentation": "<p>Field values that an end user needs to provide to Amazon Q Business for Amazon Q Business to perform the requested plugin action.</p>",
+                    "shape": "ActionReviewPayload"
+                },
+                "payloadFieldNameSeparator": {
+                    "documentation": "<p>A string used to retain information about the hierarchical contexts within an action review event payload.</p>",
+                    "shape": "ActionPayloadFieldNameSeparator"
+                },
+                "pluginId": {
+                    "documentation": "<p>The identifier of the plugin associated with the action review event.</p>",
+                    "shape": "PluginId"
+                },
+                "pluginType": {
+                    "documentation": "<p>The type of plugin.</p>",
+                    "shape": "PluginType"
+                },
+                "systemMessageId": {
+                    "documentation": "<p>The identifier of an Amazon Q Business AI generated associated with the action review event.</p>",
+                    "shape": "MessageId"
+                },
+                "userMessageId": {
+                    "documentation": "<p>The identifier of the conversation with which the plugin action is associated.</p>",
+                    "shape": "MessageId"
+                }
+            },
+            "type": "structure"
+        },
         "ActionReviewPayload": {
             "key": {
                 "shape": "ActionPayloadFieldKey"
             },
             "type": "map",
             "value": {
                 "shape": "ActionReviewPayloadField"
             }
         },
         "ActionReviewPayloadField": {
             "documentation": "<p>A user input field in an plugin action review payload.</p>",
             "members": {
+                "allowedFormat": {
+                    "documentation": "<p>The expected data format for the action review input field value. For example, in PTO request, <code>from</code> and <code>to</code> would be of <code>datetime</code> allowed format. </p>",
+                    "shape": "String"
+                },
                 "allowedValues": {
                     "documentation": "<p>Information about the field values that an end user can use to provide to Amazon Q Business for Amazon Q Business to perform the requested plugin action.</p>",
                     "shape": "ActionReviewPayloadFieldAllowedValues"
                 },
+                "displayDescription": {
+                    "documentation": "<p>The field level description of each action review input field. This could be an explanation of the field. In the Amazon Q Business web experience, these descriptions could be used to display as tool tips to help users understand the field. </p>",
+                    "shape": "String"
+                },
                 "displayName": {
                     "documentation": "<p> The name of the field. </p>",
                     "shape": "String"
                 },
                 "displayOrder": {
                     "documentation": "<p>The display order of fields in a payload.</p>",
                     "shape": "Integer"
@@ -2179,27 +2310,27 @@
                 }
             },
             "type": "structure"
         },
         "ApplicationArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "ApplicationId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "ApplicationName": {
             "max": 1000,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "ApplicationStatus": {
             "enum": [
                 "CREATING",
                 "ACTIVE",
                 "DELETING",
@@ -2246,23 +2377,33 @@
                 },
                 "name": {
                     "documentation": "<p>The name of the file.</p>",
                     "shape": "AttachmentName"
                 }
             },
             "required": [
-                "data",
-                "name"
+                "name",
+                "data"
             ],
             "type": "structure"
         },
+        "AttachmentInputEvent": {
+            "documentation": "<p>A file input event activated by a end user request to upload files into their web experience chat.</p>",
+            "event": true,
+            "members": {
+                "attachment": {
+                    "shape": "AttachmentInput"
+                }
+            },
+            "type": "structure"
+        },
         "AttachmentName": {
             "max": 1000,
             "min": 1,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "AttachmentOutput": {
             "documentation": "<p>The details of a file uploaded during chat.</p>",
             "members": {
                 "error": {
                     "documentation": "<p>An error associated with a file uploaded during chat.</p>",
@@ -2382,29 +2523,102 @@
         },
         "AttributeValueOperator": {
             "enum": [
                 "DELETE"
             ],
             "type": "string"
         },
+        "AuthChallengeRequest": {
+            "documentation": "<p>A request made by Amazon Q Business to a third paty authentication server to authenticate a custom plugin user.</p>",
+            "members": {
+                "authorizationUrl": {
+                    "documentation": "<p>The URL sent by Amazon Q Business to the third party authentication server to authenticate a custom plugin user through an OAuth protocol.</p>",
+                    "shape": "Url"
+                }
+            },
+            "required": [
+                "authorizationUrl"
+            ],
+            "type": "structure"
+        },
+        "AuthChallengeRequestEvent": {
+            "documentation": "<p>An authentication verification event activated by an end user request to use a custom plugin.</p>",
+            "event": true,
+            "members": {
+                "authorizationUrl": {
+                    "documentation": "<p>The URL sent by Amazon Q Business to a third party authentication server in response to an authentication verification event activated by an end user request to use a custom plugin. </p>",
+                    "shape": "Url"
+                }
+            },
+            "required": [
+                "authorizationUrl"
+            ],
+            "type": "structure"
+        },
+        "AuthChallengeResponse": {
+            "documentation": "<p>Contains details of the authentication information received from a third party authentication server in response to an authentication challenge.</p>",
+            "members": {
+                "responseMap": {
+                    "documentation": "<p>The mapping of key-value pairs in an authentication challenge response.</p>",
+                    "shape": "AuthorizationResponseMap"
+                }
+            },
+            "required": [
+                "responseMap"
+            ],
+            "type": "structure"
+        },
+        "AuthChallengeResponseEvent": {
+            "documentation": "<p>An authentication verification event response by a third party authentication server to Amazon Q Business.</p>",
+            "event": true,
+            "members": {
+                "responseMap": {
+                    "documentation": "<p>The mapping of key-value pairs in an authentication challenge response.</p>",
+                    "shape": "AuthorizationResponseMap"
+                }
+            },
+            "required": [
+                "responseMap"
+            ],
+            "type": "structure"
+        },
+        "AuthResponseKey": {
+            "max": 100,
+            "min": 1,
+            "type": "string"
+        },
+        "AuthResponseValue": {
+            "max": 2048,
+            "min": 1,
+            "type": "string"
+        },
+        "AuthorizationResponseMap": {
+            "key": {
+                "shape": "AuthResponseKey"
+            },
+            "type": "map",
+            "value": {
+                "shape": "AuthResponseValue"
+            }
+        },
         "BasicAuthConfiguration": {
             "documentation": "<p>Information about the basic authentication credentials used to configure a plugin.</p>",
             "members": {
                 "roleArn": {
                     "documentation": "<p>The ARN of an IAM role used by Amazon Q Business to access the basic authentication credentials stored in a Secrets Manager secret.</p>",
                     "shape": "RoleArn"
                 },
                 "secretArn": {
                     "documentation": "<p>The ARN of the Secrets Manager secret that stores the basic authentication credentials used for plugin configuration..</p>",
                     "shape": "SecretArn"
                 }
             },
             "required": [
-                "roleArn",
-                "secretArn"
+                "secretArn",
+                "roleArn"
             ],
             "type": "structure"
         },
         "BatchDeleteDocumentRequest": {
             "members": {
                 "applicationId": {
                     "documentation": "<p>The identifier of the Amazon Q Business application.</p>",
@@ -2425,16 +2639,16 @@
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
                 "applicationId",
-                "documents",
-                "indexId"
+                "indexId",
+                "documents"
             ],
             "type": "structure"
         },
         "BatchDeleteDocumentResponse": {
             "members": {
                 "failedDocuments": {
                     "documentation": "<p>A list of documents that couldn't be removed from the Amazon Q Business index. Each entry contains an error message that indicates why the document couldn't be removed from the index. </p>",
@@ -2468,16 +2682,16 @@
                 "roleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an IAM role with permission to access your S3 bucket.</p>",
                     "shape": "RoleArn"
                 }
             },
             "required": [
                 "applicationId",
-                "documents",
-                "indexId"
+                "indexId",
+                "documents"
             ],
             "type": "structure"
         },
         "BatchPutDocumentResponse": {
             "members": {
                 "failedDocuments": {
                     "documentation": "<p> A list of documents that were not added to the Amazon Q Business index because the document failed a validation check. Each document contains an error message that indicates why the document couldn't be added to the index. </p>",
@@ -2488,15 +2702,15 @@
         },
         "Blob": {
             "type": "blob"
         },
         "BlockedPhrase": {
             "max": 36,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "BlockedPhrases": {
             "max": 5,
             "member": {
                 "shape": "BlockedPhrase"
             },
@@ -2541,14 +2755,95 @@
         },
         "BoostingDurationInSeconds": {
             "box": true,
             "max": 999999999,
             "min": 0,
             "type": "long"
         },
+        "ChatInput": {
+            "members": {
+                "applicationId": {
+                    "documentation": "<p>The identifier of the Amazon Q Business application linked to a streaming Amazon Q Business conversation.</p>",
+                    "location": "uri",
+                    "locationName": "applicationId",
+                    "shape": "ApplicationId"
+                },
+                "clientToken": {
+                    "documentation": "<p>A token that you provide to identify the chat input.</p>",
+                    "idempotencyToken": true,
+                    "location": "querystring",
+                    "locationName": "clientToken",
+                    "shape": "ClientToken"
+                },
+                "conversationId": {
+                    "documentation": "<p>The identifier of the Amazon Q Business conversation.</p>",
+                    "location": "querystring",
+                    "locationName": "conversationId",
+                    "shape": "ConversationId"
+                },
+                "inputStream": {
+                    "documentation": "<p>The streaming input for the <code>Chat</code> API.</p>",
+                    "shape": "ChatInputStream"
+                },
+                "parentMessageId": {
+                    "documentation": "<p>The identifier used to associate a user message with a AI generated response.</p>",
+                    "location": "querystring",
+                    "locationName": "parentMessageId",
+                    "shape": "MessageId"
+                },
+                "userGroups": {
+                    "documentation": "<p>The groups that a user associated with the chat input belongs to.</p>",
+                    "location": "querystring",
+                    "locationName": "userGroups",
+                    "shape": "UserGroups"
+                },
+                "userId": {
+                    "documentation": "<p>The identifier of the user attached to the chat input. </p>",
+                    "location": "querystring",
+                    "locationName": "userId",
+                    "shape": "UserId"
+                }
+            },
+            "payload": "inputStream",
+            "required": [
+                "applicationId"
+            ],
+            "type": "structure"
+        },
+        "ChatInputStream": {
+            "documentation": "<p>The streaming input for the <code>Chat</code> API.</p>",
+            "eventstream": true,
+            "members": {
+                "actionExecutionEvent": {
+                    "documentation": "<p>A request from an end user to perform an Amazon Q Business plugin action.</p>",
+                    "shape": "ActionExecutionEvent"
+                },
+                "attachmentEvent": {
+                    "documentation": "<p>A request by an end user to upload a file during chat.</p>",
+                    "shape": "AttachmentInputEvent"
+                },
+                "authChallengeResponseEvent": {
+                    "documentation": "<p>An authentication verification event response by a third party authentication server to Amazon Q Business.</p>",
+                    "shape": "AuthChallengeResponseEvent"
+                },
+                "configurationEvent": {
+                    "documentation": "<p>A configuration event activated by an end user request to select a specific chat mode.</p>",
+                    "shape": "ConfigurationEvent"
+                },
+                "endOfInputEvent": {
+                    "documentation": "<p>The end of the streaming input for the <code>Chat</code> API.</p>",
+                    "shape": "EndOfInputEvent"
+                },
+                "textEvent": {
+                    "documentation": "<p>Information about the payload of the <code>ChatInputStream</code> event containing the end user message input.</p>",
+                    "shape": "TextInputEvent"
+                }
+            },
+            "type": "structure"
+        },
         "ChatMode": {
             "enum": [
                 "RETRIEVAL_MODE",
                 "CREATOR_MODE",
                 "PLUGIN_MODE"
             ],
             "type": "string"
@@ -2560,14 +2855,51 @@
                     "documentation": "<p>Configuration information required to invoke chat in <code>PLUGIN_MODE</code>.</p>",
                     "shape": "PluginConfiguration"
                 }
             },
             "type": "structure",
             "union": true
         },
+        "ChatOutput": {
+            "members": {
+                "outputStream": {
+                    "documentation": "<p>The streaming output for the <code>Chat</code> API.</p>",
+                    "shape": "ChatOutputStream"
+                }
+            },
+            "payload": "outputStream",
+            "type": "structure"
+        },
+        "ChatOutputStream": {
+            "documentation": "<p>The streaming output for the <code>Chat</code> API.</p>",
+            "eventstream": true,
+            "members": {
+                "actionReviewEvent": {
+                    "documentation": "<p>A request from Amazon Q Business to the end user for information Amazon Q Business needs to successfully complete a requested plugin action.</p>",
+                    "shape": "ActionReviewEvent"
+                },
+                "authChallengeRequestEvent": {
+                    "documentation": "<p>An authentication verification event activated by an end user request to use a custom plugin.</p>",
+                    "shape": "AuthChallengeRequestEvent"
+                },
+                "failedAttachmentEvent": {
+                    "documentation": "<p>A failed file upload event during a web experience chat.</p>",
+                    "shape": "FailedAttachmentEvent"
+                },
+                "metadataEvent": {
+                    "documentation": "<p>A metadata event for a AI-generated text output message in a Amazon Q Business conversation. </p>",
+                    "shape": "MetadataEvent"
+                },
+                "textEvent": {
+                    "documentation": "<p>Information about the payload of the <code>ChatOutputStream</code> event containing the AI-generated message output.</p>",
+                    "shape": "TextOutputEvent"
+                }
+            },
+            "type": "structure"
+        },
         "ChatSyncInput": {
             "members": {
                 "actionExecution": {
                     "documentation": "<p>A request from an end user to perform an Amazon Q Business plugin action.</p>",
                     "shape": "ActionExecution"
                 },
                 "applicationId": {
@@ -2580,16 +2912,20 @@
                     "documentation": "<p>A list of files uploaded directly during chat. You can upload a maximum of 5 files of upto 10 MB each.</p>",
                     "shape": "AttachmentsInput"
                 },
                 "attributeFilter": {
                     "documentation": "<p>Enables filtering of Amazon Q Business web experience responses based on document attributes or metadata fields.</p>",
                     "shape": "AttributeFilter"
                 },
+                "authChallengeResponse": {
+                    "documentation": "<p>An authentication verification event response by a third party authentication server to Amazon Q Business.</p>",
+                    "shape": "AuthChallengeResponse"
+                },
                 "chatMode": {
-                    "documentation": "<p>The chat modes available in an Amazon Q Business web experience.</p> <ul> <li> <p> <code>RETRIEVAL_MODE</code> - The default chat mode for an Amazon Q Business application. When this mode is enabled, Amazon Q Business generates responses only from data sources connected to an Amazon Q Business application.</p> </li> <li> <p> <code>CREATOR_MODE</code> - By selecting this mode, users can choose to generate responses only from the LLM knowledge, without consulting connected data sources, for a chat request.</p> </li> <li> <p> <code>PLUGIN_MODE</code> - By selecting this mode, users can choose to use plugins in chat.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/guardrails.html\">Admin controls and guardrails</a>, <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/plugins.html\">Plugins</a>, and <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/using-web-experience.html#chat-source-scope\">Conversation settings</a>.</p>",
+                    "documentation": "<p>The chat modes available to an Amazon Q Business end user.</p> <ul> <li> <p> <code>RETRIEVAL_MODE</code> - The default chat mode for an Amazon Q Business application. When this mode is enabled, Amazon Q Business generates responses only from data sources connected to an Amazon Q Business application.</p> </li> <li> <p> <code>CREATOR_MODE</code> - By selecting this mode, users can choose to generate responses only from the LLM knowledge, without consulting connected data sources, for a chat request.</p> </li> <li> <p> <code>PLUGIN_MODE</code> - By selecting this mode, users can choose to use plugins in chat.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/guardrails.html\">Admin controls and guardrails</a>, <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/plugins.html\">Plugins</a>, and <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/using-web-experience.html#chat-source-scope\">Conversation settings</a>.</p>",
                     "shape": "ChatMode"
                 },
                 "chatModeConfiguration": {
                     "documentation": "<p>The chat mode configuration for an Amazon Q Business application.</p>",
                     "shape": "ChatModeConfiguration"
                 },
                 "clientToken": {
@@ -2629,14 +2965,18 @@
         },
         "ChatSyncOutput": {
             "members": {
                 "actionReview": {
                     "documentation": "<p>A request from Amazon Q Business to the end user for information Amazon Q Business needs to successfully complete a requested plugin action.</p>",
                     "shape": "ActionReview"
                 },
+                "authChallengeRequest": {
+                    "documentation": "<p>An authentication verification event activated by an end user request to use a custom plugin.</p>",
+                    "shape": "AuthChallengeRequest"
+                },
                 "conversationId": {
                     "documentation": "<p>The identifier of the Amazon Q Business conversation.</p>",
                     "shape": "ConversationId"
                 },
                 "failedAttachments": {
                     "documentation": "<p>A list of files which failed to upload during chat.</p>",
                     "shape": "AttachmentsOutput"
@@ -2661,14 +3001,31 @@
             "type": "structure"
         },
         "ClientToken": {
             "max": 100,
             "min": 1,
             "type": "string"
         },
+        "ConfigurationEvent": {
+            "documentation": "<p>A configuration event activated by an end user request to select a specific chat mode.</p>",
+            "event": true,
+            "members": {
+                "attributeFilter": {
+                    "shape": "AttributeFilter"
+                },
+                "chatMode": {
+                    "documentation": "<p>The chat modes available to an Amazon Q Business end user.</p> <ul> <li> <p> <code>RETRIEVAL_MODE</code> - The default chat mode for an Amazon Q Business application. When this mode is enabled, Amazon Q Business generates responses only from data sources connected to an Amazon Q Business application.</p> </li> <li> <p> <code>CREATOR_MODE</code> - By selecting this mode, users can choose to generate responses only from the LLM knowledge, without consulting connected data sources, for a chat request.</p> </li> <li> <p> <code>PLUGIN_MODE</code> - By selecting this mode, users can choose to use plugins in chat.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/guardrails.html\">Admin controls and guardrails</a>, <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/plugins.html\">Plugins</a>, and <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/using-web-experience.html#chat-source-scope\">Conversation settings</a>.</p>",
+                    "shape": "ChatMode"
+                },
+                "chatModeConfiguration": {
+                    "shape": "ChatModeConfiguration"
+                }
+            },
+            "type": "structure"
+        },
         "ConflictException": {
             "documentation": "<p>You are trying to perform an action that conflicts with the current status of your resource. Fix any inconsistences with your resources and try again.</p>",
             "error": {
                 "httpStatusCode": 409,
                 "senderFault": true
             },
             "exception": true,
@@ -2747,15 +3104,15 @@
                 }
             },
             "type": "structure"
         },
         "ConversationId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "ConversationTitle": {
             "type": "string"
         },
         "Conversations": {
             "member": {
@@ -2796,16 +3153,15 @@
                 },
                 "tags": {
                     "documentation": "<p>A list of key-value pairs that identify or categorize your Amazon Q Business application. You can also use tags to help control access to the application. Tag keys and values can consist of Unicode letters, digits, white space, and any of the following symbols: _ . : / = + - @.</p>",
                     "shape": "Tags"
                 }
             },
             "required": [
-                "displayName",
-                "roleArn"
+                "displayName"
             ],
             "type": "structure"
         },
         "CreateApplicationResponse": {
             "members": {
                 "applicationArn": {
                     "documentation": "<p> The Amazon Resource Name (ARN) of the Amazon Q Business application. </p>",
@@ -2867,17 +3223,17 @@
                 "vpcConfiguration": {
                     "documentation": "<p>Configuration information for an Amazon VPC (Virtual Private Cloud) to connect to your data source. For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/connector-vpc.html\">Using Amazon VPC with Amazon Q Business connectors</a>.</p>",
                     "shape": "DataSourceVpcConfiguration"
                 }
             },
             "required": [
                 "applicationId",
-                "configuration",
+                "indexId",
                 "displayName",
-                "indexId"
+                "configuration"
             ],
             "type": "structure"
         },
         "CreateDataSourceResponse": {
             "members": {
                 "dataSourceArn": {
                     "documentation": "<p> The Amazon Resource Name (ARN) of a data source in an Amazon Q Business application. </p>",
@@ -2914,14 +3270,18 @@
                 "displayName": {
                     "documentation": "<p>A name for the Amazon Q Business index.</p>",
                     "shape": "IndexName"
                 },
                 "tags": {
                     "documentation": "<p>A list of key-value pairs that identify or categorize the index. You can also use tags to help control access to the index. Tag keys and values can consist of Unicode letters, digits, white space, and any of the following symbols: _ . : / = + - @.</p>",
                     "shape": "Tags"
+                },
+                "type": {
+                    "documentation": "<p>The index type that's suitable for your needs. For more information on what's included in each type of index or index tier, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/what-is.html#tiers\">Amazon Q Business tiers</a>.</p>",
+                    "shape": "IndexType"
                 }
             },
             "required": [
                 "applicationId",
                 "displayName"
             ],
             "type": "structure"
@@ -2951,14 +3311,18 @@
                     "shape": "PluginAuthConfiguration"
                 },
                 "clientToken": {
                     "documentation": "<p>A token that you provide to identify the request to create your Amazon Q Business plugin.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
+                "customPluginConfiguration": {
+                    "documentation": "<p>Contains configuration for a custom plugin.</p>",
+                    "shape": "CustomPluginConfiguration"
+                },
                 "displayName": {
                     "documentation": "<p>A the name for your plugin.</p>",
                     "shape": "PluginName"
                 },
                 "serverUrl": {
                     "documentation": "<p>The source URL used for plugin configuration.</p>",
                     "shape": "Url"
@@ -2970,23 +3334,26 @@
                 "type": {
                     "documentation": "<p>The type of plugin you want to create.</p>",
                     "shape": "PluginType"
                 }
             },
             "required": [
                 "applicationId",
-                "authConfiguration",
                 "displayName",
-                "serverUrl",
-                "type"
+                "type",
+                "authConfiguration"
             ],
             "type": "structure"
         },
         "CreatePluginResponse": {
             "members": {
+                "buildStatus": {
+                    "documentation": "<p>The current status of a plugin. A plugin is modified asynchronously.</p>",
+                    "shape": "PluginBuildStatus"
+                },
                 "pluginArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of a plugin.</p>",
                     "shape": "PluginArn"
                 },
                 "pluginId": {
                     "documentation": "<p>The identifier of the plugin created.</p>",
                     "shape": "PluginId"
@@ -3025,17 +3392,17 @@
                 "type": {
                     "documentation": "<p>The type of retriever you are using.</p>",
                     "shape": "RetrieverType"
                 }
             },
             "required": [
                 "applicationId",
-                "configuration",
+                "type",
                 "displayName",
-                "type"
+                "configuration"
             ],
             "type": "structure"
         },
         "CreateRetrieverResponse": {
             "members": {
                 "retrieverArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an IAM role associated with a retriever.</p>",
@@ -3160,14 +3527,37 @@
         "CreatorModeControl": {
             "enum": [
                 "ENABLED",
                 "DISABLED"
             ],
             "type": "string"
         },
+        "CustomPluginConfiguration": {
+            "documentation": "<p> Configuration information required to create a custom plugin.</p>",
+            "members": {
+                "apiSchema": {
+                    "documentation": "<p>Contains either details about the S3 object containing the OpenAPI schema for the action group or the JSON or YAML-formatted payload defining the schema.</p>",
+                    "shape": "APISchema"
+                },
+                "apiSchemaType": {
+                    "documentation": "<p>The type of OpenAPI schema to use.</p>",
+                    "shape": "APISchemaType"
+                },
+                "description": {
+                    "documentation": "<p>A description for your custom plugin configuration.</p>",
+                    "shape": "PluginDescription"
+                }
+            },
+            "required": [
+                "description",
+                "apiSchemaType",
+                "apiSchema"
+            ],
+            "type": "structure"
+        },
         "DataSource": {
             "documentation": "<p>A data source in an Amazon Q Business application.</p>",
             "members": {
                 "createdAt": {
                     "documentation": "<p>The Unix timestamp when the Amazon Q Business data source was created.</p>",
                     "shape": "Timestamp"
                 },
@@ -3193,41 +3583,41 @@
                 }
             },
             "type": "structure"
         },
         "DataSourceArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "DataSourceConfiguration": {
             "document": true,
             "documentation": "<p>Provides the configuration information for an Amazon Q Business data source.</p>",
             "members": {},
             "type": "structure"
         },
         "DataSourceId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "DataSourceIds": {
             "max": 1,
             "member": {
                 "shape": "DataSourceId"
             },
             "min": 1,
             "type": "list"
         },
         "DataSourceName": {
             "max": 1000,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "DataSourceStatus": {
             "enum": [
                 "PENDING_CREATION",
                 "CREATING",
                 "ACTIVE",
@@ -3314,15 +3704,15 @@
                 "shape": "DataSourceSyncJob"
             },
             "type": "list"
         },
         "DataSourceUserId": {
             "max": 1024,
             "min": 1,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "DataSourceVpcConfiguration": {
             "documentation": "<p>Provides configuration information needed to connect to an Amazon VPC (Virtual Private Cloud).</p>",
             "members": {
                 "securityGroupIds": {
                     "documentation": "<p>A list of identifiers of security groups within your Amazon VPC. The security groups should enable Amazon Q Business to connect to the data source.</p>",
@@ -3330,16 +3720,16 @@
                 },
                 "subnetIds": {
                     "documentation": "<p>A list of identifiers for subnets within your Amazon VPC. The subnets should be able to connect to each other in the VPC, and they should have outgoing access to the Internet through a NAT device.</p>",
                     "shape": "SubnetIds"
                 }
             },
             "required": [
-                "securityGroupIds",
-                "subnetIds"
+                "subnetIds",
+                "securityGroupIds"
             ],
             "type": "structure"
         },
         "DataSources": {
             "member": {
                 "shape": "DataSource"
             },
@@ -3416,16 +3806,16 @@
                     "documentation": "<p>The identifier of the user who is deleting the conversation.</p>",
                     "location": "querystring",
                     "locationName": "userId",
                     "shape": "UserId"
                 }
             },
             "required": [
-                "applicationId",
-                "conversationId"
+                "conversationId",
+                "applicationId"
             ],
             "type": "structure"
         },
         "DeleteConversationResponse": {
             "members": {},
             "type": "structure"
         },
@@ -3448,16 +3838,16 @@
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
                 "applicationId",
-                "dataSourceId",
-                "indexId"
+                "indexId",
+                "dataSourceId"
             ],
             "type": "structure"
         },
         "DeleteDataSourceResponse": {
             "members": {},
             "type": "structure"
         },
@@ -3505,16 +3895,16 @@
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
                 "applicationId",
-                "groupName",
-                "indexId"
+                "indexId",
+                "groupName"
             ],
             "type": "structure"
         },
         "DeleteGroupResponse": {
             "members": {},
             "type": "structure"
         },
@@ -3642,15 +4032,15 @@
         "DeleteWebExperienceResponse": {
             "members": {},
             "type": "structure"
         },
         "Description": {
             "max": 1000,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "Document": {
             "documentation": "<p>A document in an Amazon Q Business application.</p>",
             "members": {
                 "accessConfiguration": {
                     "documentation": "<p>Configuration information for access permission to a document.</p>",
@@ -3751,15 +4141,15 @@
             "documentation": "<p>The condition used for the target document attribute or metadata field when ingesting documents into Amazon Q Business. You use this with <a href=\"https://docs.aws.amazon.com/amazonq/latest/api-reference/API_DocumentAttributeTarget.html\"> <code>DocumentAttributeTarget</code> </a> to apply the condition.</p> <p>For example, you can create the 'Department' target field and have it prefill department names associated with the documents based on information in the 'Source_URI' field. Set the condition that if the 'Source_URI' field contains 'financial' in its URI value, then prefill the target field 'Department' with the target value 'Finance' for the document.</p> <p>Amazon Q Business can't create a target field if it has not already been created as an index field. After you create your index field, you can create a document metadata field using <code>DocumentAttributeTarget</code>. Amazon Q Business then will map your newly created metadata field to your index field.</p>",
             "members": {
                 "key": {
                     "documentation": "<p>The identifier of the document attribute used for the condition.</p> <p>For example, 'Source_URI' could be an identifier for the attribute or metadata field that contains source URIs associated with the documents.</p> <p>Amazon Q Business currently doesn't support <code>_document_body</code> as an attribute key used for the condition.</p>",
                     "shape": "DocumentAttributeKey"
                 },
                 "operator": {
-                    "documentation": "<p>The identifier of the document attribute used for the condition.</p> <p>For example, 'Source_URI' could be an identifier for the attribute or metadata field that contains source URIs associated with the documents.</p> <p>Amazon Kendra currently does not support <code>_document_body</code> as an attribute key used for the condition.</p>",
+                    "documentation": "<p>The identifier of the document attribute used for the condition.</p> <p>For example, 'Source_URI' could be an identifier for the attribute or metadata field that contains source URIs associated with the documents.</p> <p>Amazon Q Business currently does not support <code>_document_body</code> as an attribute key used for the condition.</p>",
                     "shape": "DocumentEnrichmentConditionOperator"
                 },
                 "value": {
                     "shape": "DocumentAttributeValue"
                 }
             },
             "required": [
@@ -3769,15 +4159,15 @@
             "type": "structure"
         },
         "DocumentAttributeConfiguration": {
             "documentation": "<p>Configuration information for document attributes. Document attributes are metadata or fields associated with your documents. For example, the company department name associated with each document.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/doc-attributes.html\">Understanding document attributes</a>.</p>",
             "members": {
                 "name": {
                     "documentation": "<p>The name of the document attribute.</p>",
-                    "shape": "String"
+                    "shape": "DocumentMetadataConfigurationName"
                 },
                 "search": {
                     "documentation": "<p>Information about whether the document attribute can be used by an end user to search for information on their web experience.</p>",
                     "shape": "Status"
                 },
                 "type": {
                     "documentation": "<p>The type of document attribute.</p>",
@@ -3793,15 +4183,15 @@
             },
             "min": 1,
             "type": "list"
         },
         "DocumentAttributeKey": {
             "max": 200,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9_][a-zA-Z0-9_-]*$",
+            "pattern": "[a-zA-Z0-9_][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "DocumentAttributeStringListValue": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
@@ -3946,15 +4336,21 @@
                 }
             },
             "type": "structure"
         },
         "DocumentId": {
             "max": 1825,
             "min": 1,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
+            "type": "string"
+        },
+        "DocumentMetadataConfigurationName": {
+            "max": 30,
+            "min": 1,
+            "pattern": "[a-zA-Z0-9_][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "DocumentStatus": {
             "enum": [
                 "RECEIVED",
                 "PROCESSING",
                 "INDEXED",
@@ -4002,14 +4398,20 @@
                 "kmsKeyId": {
                     "documentation": "<p>The identifier of the KMS key. Amazon Q Business doesn't support asymmetric keys.</p>",
                     "shape": "KmsKeyId"
                 }
             },
             "type": "structure"
         },
+        "EndOfInputEvent": {
+            "documentation": "<p>The end of the streaming input for the <code>Chat</code> API.</p>",
+            "event": true,
+            "members": {},
+            "type": "structure"
+        },
         "ErrorCode": {
             "enum": [
                 "InternalError",
                 "InvalidRequest",
                 "ResourceInactive",
                 "ResourceNotFound"
             ],
@@ -4028,37 +4430,59 @@
                 }
             },
             "type": "structure"
         },
         "ErrorMessage": {
             "max": 2048,
             "min": 1,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "ExampleChatMessage": {
             "max": 350,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "ExampleChatMessages": {
             "max": 5,
             "member": {
                 "shape": "ExampleChatMessage"
             },
             "min": 0,
             "type": "list"
         },
         "ExecutionId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
+        "FailedAttachmentEvent": {
+            "documentation": "<p>A failed file upload during web experience chat.</p>",
+            "event": true,
+            "members": {
+                "attachment": {
+                    "shape": "AttachmentOutput"
+                },
+                "conversationId": {
+                    "documentation": "<p> The identifier of the conversation associated with the failed file upload.</p>",
+                    "shape": "ConversationId"
+                },
+                "systemMessageId": {
+                    "documentation": "<p>The identifier of the AI-generated message associated with the file upload.</p>",
+                    "shape": "MessageId"
+                },
+                "userMessageId": {
+                    "documentation": "<p>The identifier of the end user chat message associated with the file upload.</p>",
+                    "shape": "MessageId"
+                }
+            },
+            "type": "structure"
+        },
         "FailedDocument": {
             "documentation": "<p>A list of documents that could not be removed from an Amazon Q Business index. Each entry contains an error message that indicates why the document couldn't be removed from the index.</p>",
             "members": {
                 "dataSourceId": {
                     "documentation": "<p>The identifier of the Amazon Q Business data source connector that contains the failed document.</p>",
                     "shape": "DataSourceId"
                 },
@@ -4216,16 +4640,16 @@
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
                 "applicationId",
-                "dataSourceId",
-                "indexId"
+                "indexId",
+                "dataSourceId"
             ],
             "type": "structure"
         },
         "GetDataSourceResponse": {
             "members": {
                 "applicationId": {
                     "documentation": "<p>The identifier of the Amazon Q Business application.</p>",
@@ -4318,16 +4742,16 @@
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
                 "applicationId",
-                "groupName",
-                "indexId"
+                "indexId",
+                "groupName"
             ],
             "type": "structure"
         },
         "GetGroupResponse": {
             "members": {
                 "status": {
                     "documentation": "<p>The current status of the group.</p>",
@@ -4403,14 +4827,18 @@
                     "documentation": "<p>Provides information about the number of documents indexed.</p>",
                     "shape": "IndexStatistics"
                 },
                 "status": {
                     "documentation": "<p>The current status of the index. When the value is <code>ACTIVE</code>, the index is ready for use. If the <code>Status</code> field value is <code>FAILED</code>, the <code>ErrorMessage</code> field contains a message that explains why.</p>",
                     "shape": "IndexStatus"
                 },
+                "type": {
+                    "documentation": "<p>The type of index attached to your Amazon Q Business application.</p>",
+                    "shape": "IndexType"
+                },
                 "updatedAt": {
                     "documentation": "<p>The Unix timestamp when the Amazon Q Business index was last updated.</p>",
                     "shape": "Timestamp"
                 }
             },
             "type": "structure"
         },
@@ -4440,18 +4868,26 @@
                 "applicationId": {
                     "documentation": "<p>The identifier of the application which contains the plugin.</p>",
                     "shape": "ApplicationId"
                 },
                 "authConfiguration": {
                     "shape": "PluginAuthConfiguration"
                 },
+                "buildStatus": {
+                    "documentation": "<p>The current status of a plugin. A plugin is modified asynchronously.</p>",
+                    "shape": "PluginBuildStatus"
+                },
                 "createdAt": {
                     "documentation": "<p>The timestamp for when the plugin was created.</p>",
                     "shape": "Timestamp"
                 },
+                "customPluginConfiguration": {
+                    "documentation": "<p>Configuration information required to create a custom plugin.</p>",
+                    "shape": "CustomPluginConfiguration"
+                },
                 "displayName": {
                     "documentation": "<p>The name of the plugin.</p>",
                     "shape": "PluginName"
                 },
                 "pluginArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the role with permission to access resources needed to create the plugin.</p>",
                     "shape": "PluginArn"
@@ -4598,19 +5034,21 @@
         "GetWebExperienceResponse": {
             "members": {
                 "applicationId": {
                     "documentation": "<p>The identifier of the Amazon Q Business application linked to the web experience.</p>",
                     "shape": "ApplicationId"
                 },
                 "authenticationConfiguration": {
+                    "deprecated": true,
+                    "deprecatedMessage": "Property associated with legacy SAML IdP flow. Deprecated in favor of using AWS IAM Identity Center for user management.",
                     "documentation": "<p>The authentication configuration information for your Amazon Q Business web experience.</p>",
                     "shape": "WebExperienceAuthConfiguration"
                 },
                 "createdAt": {
-                    "documentation": "<p>The Unix timestamp when the retriever was created.</p>",
+                    "documentation": "<p>The Unix timestamp when the Amazon Q Business web experience was last created.</p>",
                     "shape": "Timestamp"
                 },
                 "defaultEndpoint": {
                     "documentation": "<p>The endpoint of your Amazon Q Business web experience.</p>",
                     "shape": "Url"
                 },
                 "error": {
@@ -4634,15 +5072,15 @@
                     "shape": "WebExperienceSubtitle"
                 },
                 "title": {
                     "documentation": "<p>The title for your Amazon Q Business web experience. </p>",
                     "shape": "WebExperienceTitle"
                 },
                 "updatedAt": {
-                    "documentation": "<p>The Unix timestamp when the data source connector was last updated.</p>",
+                    "documentation": "<p>The Unix timestamp when the Amazon Q Business web experience was last updated.</p>",
                     "shape": "Timestamp"
                 },
                 "webExperienceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the role with the permission to access the Amazon Q Business web experience and required resources.</p>",
                     "shape": "WebExperienceArn"
                 },
                 "webExperienceId": {
@@ -4669,15 +5107,15 @@
                 }
             },
             "type": "structure"
         },
         "GroupName": {
             "max": 1024,
             "min": 1,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "GroupStatus": {
             "enum": [
                 "FAILED",
                 "SUCCEEDED",
                 "PROCESSING",
@@ -4723,15 +5161,15 @@
         "GroupSummaryList": {
             "member": {
                 "shape": "GroupSummary"
             },
             "type": "list"
         },
         "HookConfiguration": {
-            "documentation": "<p>Provides the configuration information for invoking a Lambda function in Lambda to alter document metadata and content when ingesting documents into Amazon Q Business.</p> <p>You can configure your Lambda function using <a href=\"https://docs.aws.amazon.com/amazonq/latest/api-reference/API_DocumentEnrichmentConfiguration.html\">PreExtractionHookConfiguration</a> if you want to apply advanced alterations on the original or raw documents.</p> <p>If you want to apply advanced alterations on the Amazon Q Business structured documents, you must configure your Lambda function using <a href=\"https://docs.aws.amazon.com/amazonq/latest/api-reference/API_DocumentEnrichmentConfiguration.html\">PostExtractionHookConfiguration</a>.</p> <p>You can only invoke one Lambda function. However, this function can invoke other functions it requires.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/custom-document-enrichment.html\">Custom document enrichment</a>. </p>",
+            "documentation": "<p>Provides the configuration information for invoking a Lambda function in Lambda to alter document metadata and content when ingesting documents into Amazon Q Business.</p> <p>You can configure your Lambda function using the <code>PreExtractionHookConfiguration</code> parameter if you want to apply advanced alterations on the original or raw documents.</p> <p>If you want to apply advanced alterations on the Amazon Q Business structured documents, you must configure your Lambda function using <code>PostExtractionHookConfiguration</code>.</p> <p>You can only invoke one Lambda function. However, this function can invoke other functions it requires.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/custom-document-enrichment.html\">Custom document enrichment</a>. </p>",
             "members": {
                 "invocationCondition": {
                     "documentation": "<p>The condition used for when a Lambda function should be invoked.</p> <p>For example, you can specify a condition that if there are empty date-time values, then Amazon Q Business should invoke a function that inserts the current date-time.</p>",
                     "shape": "DocumentAttributeCondition"
                 },
                 "lambdaArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of a role with permission to run a Lambda function during ingestion. For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/iam-roles.html#cde-iam-role\">IAM roles for Custom Document Enrichment (CDE)</a>.</p>",
@@ -4747,15 +5185,15 @@
                 }
             },
             "type": "structure"
         },
         "IdcApplicationArn": {
             "max": 1224,
             "min": 10,
-            "pattern": "^arn:(aws|aws-us-gov|aws-cn|aws-iso|aws-iso-b):sso::\\d{12}:application/(sso)?ins-[a-zA-Z0-9-.]{16}/apl-[a-zA-Z0-9]{16}$",
+            "pattern": "arn:(aws|aws-us-gov|aws-cn|aws-iso|aws-iso-b):sso::\\d{12}:application/(sso)?ins-[a-zA-Z0-9-.]{16}/apl-[a-zA-Z0-9]{16}",
             "type": "string"
         },
         "Index": {
             "documentation": "<p>Summary information for your Amazon Q Business index.</p>",
             "members": {
                 "createdAt": {
                     "documentation": "<p>The Unix timestamp when the index was created.</p>",
@@ -4779,15 +5217,15 @@
                 }
             },
             "type": "structure"
         },
         "IndexArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "IndexCapacityConfiguration": {
             "documentation": "<p>Provides information about index capacity configuration.</p>",
             "members": {
                 "units": {
                     "documentation": "<p>The number of storage units configured for an Amazon Q Business index.</p>",
@@ -4800,21 +5238,21 @@
             "box": true,
             "min": 1,
             "type": "integer"
         },
         "IndexId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "IndexName": {
             "max": 1000,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "IndexStatistics": {
             "documentation": "<p>Provides information about the number of documents in an index.</p>",
             "members": {
                 "textDocumentStatistics": {
                     "documentation": "<p>The number of documents indexed.</p>",
@@ -4829,14 +5267,21 @@
                 "ACTIVE",
                 "DELETING",
                 "FAILED",
                 "UPDATING"
             ],
             "type": "string"
         },
+        "IndexType": {
+            "enum": [
+                "ENTERPRISE",
+                "STARTER"
+            ],
+            "type": "string"
+        },
         "IndexedTextBytes": {
             "box": true,
             "min": 0,
             "type": "long"
         },
         "IndexedTextDocument": {
             "box": true,
@@ -4872,15 +5317,15 @@
             },
             "min": 1,
             "type": "list"
         },
         "InstanceArn": {
             "max": 1224,
             "min": 10,
-            "pattern": "^arn:(aws|aws-us-gov|aws-cn|aws-iso|aws-iso-b):sso:::instance/(sso)?ins-[a-zA-Z0-9-.]{16}$",
+            "pattern": "arn:(aws|aws-us-gov|aws-cn|aws-iso|aws-iso-b):sso:::instance/(sso)?ins-[a-zA-Z0-9-.]{16}",
             "type": "string"
         },
         "Integer": {
             "box": true,
             "type": "integer"
         },
         "InternalServerException": {
@@ -4912,27 +5357,27 @@
                 "indexId"
             ],
             "type": "structure"
         },
         "KendraIndexId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "KmsKeyId": {
             "max": 2048,
             "min": 1,
             "sensitive": true,
             "type": "string"
         },
         "LambdaArn": {
             "max": 2048,
             "min": 1,
-            "pattern": "^arn:aws[a-zA-Z-]*:lambda:[a-z-]*-[0-9]:[0-9]{12}:function:[a-zA-Z0-9-_]+(/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12})?(:[a-zA-Z0-9-_]+)?$",
+            "pattern": "arn:aws[a-zA-Z-]*:lambda:[a-z-]*-[0-9]:[0-9]{12}:function:[a-zA-Z0-9-_]+(/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12})?(:[a-zA-Z0-9-_]+)?",
             "type": "string"
         },
         "LicenseNotFoundException": {
             "documentation": "<p>You don't have permissions to perform the action because your license is inactive. Ask your admin to activate your license and try again after your licence is active.</p>",
             "error": {
                 "httpStatusCode": 400,
                 "senderFault": true
@@ -5071,16 +5516,16 @@
                     "documentation": "<p>Only returns synchronization jobs with the <code>Status</code> field equal to the specified status.</p>",
                     "location": "querystring",
                     "locationName": "syncStatus",
                     "shape": "DataSourceSyncJobStatus"
                 }
             },
             "required": [
-                "applicationId",
                 "dataSourceId",
+                "applicationId",
                 "indexId"
             ],
             "type": "structure"
         },
         "ListDataSourceSyncJobsResponse": {
             "members": {
                 "history": {
@@ -5320,16 +5765,16 @@
                     "documentation": "<p>The identifier of the user involved in the Amazon Q Business web experience conversation.</p>",
                     "location": "querystring",
                     "locationName": "userId",
                     "shape": "UserId"
                 }
             },
             "required": [
-                "applicationId",
-                "conversationId"
+                "conversationId",
+                "applicationId"
             ],
             "type": "structure"
         },
         "ListMessagesResponse": {
             "members": {
                 "messages": {
                     "documentation": "<p>An array of information on one or more messages.</p>",
@@ -5657,21 +6102,21 @@
                 }
             },
             "type": "structure"
         },
         "MessageBody": {
             "max": 1000,
             "min": 0,
-            "pattern": "^\\P{C}*$}$",
+            "pattern": "\\P{C}*$}",
             "type": "string"
         },
         "MessageId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "MessageType": {
             "enum": [
                 "USER",
                 "SYSTEM"
             ],
@@ -5683,15 +6128,15 @@
                 "NOT_USEFUL"
             ],
             "type": "string"
         },
         "MessageUsefulnessComment": {
             "max": 1000,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "MessageUsefulnessFeedback": {
             "documentation": "<p>End user feedback on an AI-generated web experience chat message usefulness.</p>",
             "members": {
                 "comment": {
                     "documentation": "<p>A comment given by an end user on the usefulness of an AI-generated chat message.</p>",
@@ -5707,16 +6152,16 @@
                 },
                 "usefulness": {
                     "documentation": "<p>The usefulness value assigned by an end user to a message.</p>",
                     "shape": "MessageUsefulness"
                 }
             },
             "required": [
-                "submittedAt",
-                "usefulness"
+                "usefulness",
+                "submittedAt"
             ],
             "type": "structure"
         },
         "MessageUsefulnessReason": {
             "enum": [
                 "NOT_FACTUALLY_CORRECT",
                 "HARMFUL_OR_UNSAFE",
@@ -5735,16 +6180,43 @@
         },
         "Messages": {
             "member": {
                 "shape": "Message"
             },
             "type": "list"
         },
+        "MetadataEvent": {
+            "documentation": "<p>A metadata event for a AI-generated text output message in a Amazon Q Business conversation, containing associated metadata generated.</p>",
+            "event": true,
+            "members": {
+                "conversationId": {
+                    "documentation": "<p>The identifier of the conversation with which the generated metadata is associated.</p>",
+                    "shape": "ConversationId"
+                },
+                "finalTextMessage": {
+                    "documentation": "<p>The final text output message generated by the system.</p>",
+                    "shape": "String"
+                },
+                "sourceAttributions": {
+                    "documentation": "<p>The source documents used to generate the conversation response.</p>",
+                    "shape": "SourceAttributions"
+                },
+                "systemMessageId": {
+                    "documentation": "<p>The identifier of an Amazon Q Business AI generated message within the conversation.</p>",
+                    "shape": "MessageId"
+                },
+                "userMessageId": {
+                    "documentation": "<p>The identifier of an Amazon Q Business end user text input message within the conversation.</p>",
+                    "shape": "MessageId"
+                }
+            },
+            "type": "structure"
+        },
         "MetricValue": {
-            "pattern": "^(([1-9][0-9]*)|0)$",
+            "pattern": "(([1-9][0-9]*)|0)",
             "type": "string"
         },
         "NativeIndexConfiguration": {
             "documentation": "<p>Configuration information for an Amazon Q Business index.</p>",
             "members": {
                 "boostingOverride": {
                     "documentation": "<p>Overrides the default boosts applied by Amazon Q Business to supported document attribute data types.</p>",
@@ -5761,14 +6233,19 @@
             "type": "structure"
         },
         "NextToken": {
             "max": 800,
             "min": 1,
             "type": "string"
         },
+        "NoAuthConfiguration": {
+            "documentation": "<p>Information about invoking a custom plugin without any authentication or authorization requirement.</p>",
+            "members": {},
+            "type": "structure"
+        },
         "NumberAttributeBoostingConfiguration": {
             "documentation": "<p>Provides information on boosting <code>NUMBER</code> type document attributes.</p> <p>For more information on how boosting document attributes work in Amazon Q Business, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/metadata-boosting.html\">Boosting using document attributes</a>.</p>",
             "members": {
                 "boostingLevel": {
                     "documentation": "<p>Specifies the duration, in seconds, of a boost applies to a <code>NUMBER</code> type document attribute.</p>",
                     "shape": "DocumentAttributeBoostingLevel"
                 },
@@ -5798,22 +6275,30 @@
                 },
                 "secretArn": {
                     "documentation": "<p>The ARN of the Secrets Manager secret that stores the OAuth 2.0 credentials/token used for plugin configuration.</p>",
                     "shape": "SecretArn"
                 }
             },
             "required": [
-                "roleArn",
-                "secretArn"
+                "secretArn",
+                "roleArn"
             ],
             "type": "structure"
         },
+        "Payload": {
+            "sensitive": true,
+            "type": "string"
+        },
         "Plugin": {
             "documentation": "<p>Information about an Amazon Q Business plugin and its configuration.</p>",
             "members": {
+                "buildStatus": {
+                    "documentation": "<p>The status of the plugin.</p>",
+                    "shape": "PluginBuildStatus"
+                },
                 "createdAt": {
                     "documentation": "<p>The timestamp for when the plugin was created.</p>",
                     "shape": "Timestamp"
                 },
                 "displayName": {
                     "documentation": "<p>The name of the plugin.</p>",
                     "shape": "PluginName"
@@ -5840,70 +6325,92 @@
                 }
             },
             "type": "structure"
         },
         "PluginArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "PluginAuthConfiguration": {
             "documentation": "<p>Authentication configuration information for an Amazon Q Business plugin.</p>",
             "members": {
                 "basicAuthConfiguration": {
                     "documentation": "<p>Information about the basic authentication credentials used to configure a plugin.</p>",
                     "shape": "BasicAuthConfiguration"
                 },
+                "noAuthConfiguration": {
+                    "documentation": "<p>Information about invoking a custom plugin without any authentication.</p>",
+                    "shape": "NoAuthConfiguration"
+                },
                 "oAuth2ClientCredentialConfiguration": {
                     "documentation": "<p>Information about the OAuth 2.0 authentication credential/token used to configure a plugin.</p>",
                     "shape": "OAuth2ClientCredentialConfiguration"
                 }
             },
             "type": "structure",
             "union": true
         },
+        "PluginBuildStatus": {
+            "enum": [
+                "READY",
+                "CREATE_IN_PROGRESS",
+                "CREATE_FAILED",
+                "UPDATE_IN_PROGRESS",
+                "UPDATE_FAILED",
+                "DELETE_IN_PROGRESS",
+                "DELETE_FAILED"
+            ],
+            "type": "string"
+        },
         "PluginConfiguration": {
             "documentation": "<p>Configuration information required to invoke chat in <code>PLUGIN_MODE</code>.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/guardrails.html\">Admin controls and guardrails</a>, <a href=\"https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/plugins.html\">Plugins</a>, and <a href=\"https://docs.aws.amazon.com/amazonq/latest/business-use-dg/using-web-experience.html#chat-source-scope\">Conversation settings</a>.</p>",
             "members": {
                 "pluginId": {
                     "documentation": "<p> The identifier of the plugin you want to use.</p>",
                     "shape": "PluginId"
                 }
             },
             "required": [
                 "pluginId"
             ],
             "type": "structure"
         },
+        "PluginDescription": {
+            "max": 200,
+            "min": 1,
+            "type": "string"
+        },
         "PluginId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}$",
+            "pattern": "[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}",
             "type": "string"
         },
         "PluginName": {
             "max": 100,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "PluginState": {
             "enum": [
                 "ENABLED",
                 "DISABLED"
             ],
             "type": "string"
         },
         "PluginType": {
             "enum": [
                 "SERVICE_NOW",
                 "SALESFORCE",
                 "JIRA",
-                "ZENDESK"
+                "ZENDESK",
+                "CUSTOM"
             ],
             "type": "string"
         },
         "Plugins": {
             "member": {
                 "shape": "Plugin"
             },
@@ -6042,18 +6549,18 @@
                 "type": {
                     "documentation": "<p>The type of the group.</p>",
                     "shape": "MembershipType"
                 }
             },
             "required": [
                 "applicationId",
-                "groupMembers",
-                "groupName",
                 "indexId",
-                "type"
+                "groupName",
+                "type",
+                "groupMembers"
             ],
             "type": "structure"
         },
         "PutGroupResponse": {
             "members": {},
             "type": "structure"
         },
@@ -6124,15 +6631,15 @@
                 }
             },
             "type": "structure"
         },
         "RetrieverArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "RetrieverConfiguration": {
             "documentation": "<p>Provides information on how the retriever used for your Amazon Q Business application is configured.</p>",
             "members": {
                 "kendraIndexConfiguration": {
                     "documentation": "<p>Provides information on how the Amazon Kendra index used as a retriever for your Amazon Q Business application is configured.</p>",
@@ -6145,21 +6652,21 @@
             },
             "type": "structure",
             "union": true
         },
         "RetrieverId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "RetrieverName": {
             "max": 1000,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9_-]*$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_-]*",
             "type": "string"
         },
         "RetrieverStatus": {
             "enum": [
                 "CREATING",
                 "ACTIVE",
                 "FAILED"
@@ -6178,15 +6685,15 @@
                 "shape": "Retriever"
             },
             "type": "list"
         },
         "RoleArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "Rule": {
             "documentation": "<p>Guardrail rules for an Amazon Q Business application. Amazon Q Business supports only one rule at a time.</p>",
             "members": {
                 "excludedUsersAndGroups": {
                     "documentation": "<p>Users and groups to be excluded from a rule.</p>",
@@ -6256,15 +6763,15 @@
                 "key"
             ],
             "type": "structure"
         },
         "S3BucketName": {
             "max": 63,
             "min": 1,
-            "pattern": "^[a-z0-9][\\.\\-a-z0-9]{1,61}[a-z0-9]$",
+            "pattern": "[a-z0-9][\\.\\-a-z0-9]{1,61}[a-z0-9]",
             "type": "string"
         },
         "S3ObjectKey": {
             "max": 1024,
             "min": 1,
             "type": "string"
         },
@@ -6299,27 +6806,27 @@
                 "userIdAttribute"
             ],
             "type": "structure"
         },
         "SamlMetadataXML": {
             "max": 10000000,
             "min": 1000,
-            "pattern": "^.*$",
+            "pattern": ".*",
             "type": "string"
         },
         "SecretArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "SecurityGroupId": {
             "max": 200,
             "min": 1,
-            "pattern": "^[-0-9a-zA-Z]+$",
+            "pattern": "[-0-9a-zA-Z]+",
             "type": "string"
         },
         "SecurityGroupIds": {
             "max": 10,
             "member": {
                 "shape": "SecurityGroupId"
             },
@@ -6350,14 +6857,27 @@
             "required": [
                 "message",
                 "resourceId",
                 "resourceType"
             ],
             "type": "structure"
         },
+        "SnippetExcerpt": {
+            "documentation": "<p>Contains the relevant text excerpt from a source that was used to generate a citation text segment in an Amazon Q Business chat response.</p>",
+            "members": {
+                "text": {
+                    "documentation": "<p>The relevant text excerpt from a source that was used to generate a citation text segment in an Amazon Q chat response.</p>",
+                    "shape": "SnippetExcerptText"
+                }
+            },
+            "type": "structure"
+        },
+        "SnippetExcerptText": {
+            "type": "string"
+        },
         "SourceAttribution": {
             "documentation": "<p>The documents used to generate an Amazon Q Business web experience response.</p>",
             "members": {
                 "citationNumber": {
                     "documentation": "<p>The number attached to a citation in an Amazon Q Business generated response.</p>",
                     "shape": "Integer"
                 },
@@ -6408,16 +6928,16 @@
                     "documentation": "<p>The identifier of the index used with the data source connector.</p>",
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
-                "applicationId",
                 "dataSourceId",
+                "applicationId",
                 "indexId"
             ],
             "type": "structure"
         },
         "StartDataSourceSyncJobResponse": {
             "members": {
                 "executionId": {
@@ -6452,16 +6972,16 @@
                     "documentation": "<p>The identifier of the index used with the Amazon Q Business data source connector.</p>",
                     "location": "uri",
                     "locationName": "indexId",
                     "shape": "IndexId"
                 }
             },
             "required": [
-                "applicationId",
                 "dataSourceId",
+                "applicationId",
                 "indexId"
             ],
             "type": "structure"
         },
         "StopDataSourceSyncJobResponse": {
             "members": {},
             "type": "structure"
@@ -6520,39 +7040,39 @@
                 "boostingLevel"
             ],
             "type": "structure"
         },
         "SubnetId": {
             "max": 200,
             "min": 1,
-            "pattern": "^[-0-9a-zA-Z]+$",
+            "pattern": "[-0-9a-zA-Z]+",
             "type": "string"
         },
         "SubnetIds": {
             "member": {
                 "shape": "SubnetId"
             },
             "type": "list"
         },
         "SyncSchedule": {
             "max": 998,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "SystemMessageId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{35}",
             "type": "string"
         },
         "SystemMessageOverride": {
             "max": 350,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "Tag": {
             "documentation": "<p>A list of key/value pairs that identify an index, FAQ, or data source. Tag keys and values can consist of Unicode letters, digits, white space, and any of the following symbols: _ . : / = + - @.</p>",
             "members": {
                 "key": {
                     "documentation": "<p> The key for the tag. Keys are not case sensitive and must be unique for the Amazon Q Business application or data source.</p>",
@@ -6628,24 +7148,65 @@
                 "indexedTextDocumentCount": {
                     "documentation": "<p>The number of text documents indexed.</p>",
                     "shape": "IndexedTextDocument"
                 }
             },
             "type": "structure"
         },
+        "TextInputEvent": {
+            "documentation": "<p>An input event for a end user message in an Amazon Q Business web experience. </p>",
+            "event": true,
+            "members": {
+                "userMessage": {
+                    "documentation": "<p>A user message in a text message input event.</p>",
+                    "shape": "UserMessage"
+                }
+            },
+            "required": [
+                "userMessage"
+            ],
+            "type": "structure"
+        },
+        "TextOutputEvent": {
+            "documentation": "<p>An output event for an AI-generated response in an Amazon Q Business web experience.</p>",
+            "event": true,
+            "members": {
+                "conversationId": {
+                    "documentation": "<p>The identifier of the conversation with which the text output event is associated.</p>",
+                    "shape": "ConversationId"
+                },
+                "systemMessage": {
+                    "documentation": "<p>An AI-generated message in a <code>TextOutputEvent</code>.</p>",
+                    "shape": "String"
+                },
+                "systemMessageId": {
+                    "documentation": "<p>The identifier of an AI-generated message in a <code>TextOutputEvent</code>.</p>",
+                    "shape": "MessageId"
+                },
+                "userMessageId": {
+                    "documentation": "<p>The identifier of an end user message in a <code>TextOutputEvent</code>.</p>",
+                    "shape": "MessageId"
+                }
+            },
+            "type": "structure"
+        },
         "TextSegment": {
             "documentation": "<p>Provides information about a text extract in a chat response that can be attributed to a source document.</p>",
             "members": {
                 "beginOffset": {
                     "documentation": "<p>The zero-based location in the response string where the source attribution starts.</p>",
                     "shape": "Integer"
                 },
                 "endOffset": {
                     "documentation": "<p>The zero-based location in the response string where the source attribution ends.</p>",
                     "shape": "Integer"
+                },
+                "snippetExcerpt": {
+                    "documentation": "<p>The relevant text excerpt from a source that was used to generate a citation text segment in an Amazon Q Business chat response.</p>",
+                    "shape": "SnippetExcerpt"
                 }
             },
             "type": "structure"
         },
         "TextSegmentList": {
             "member": {
                 "shape": "TextSegment"
@@ -6702,29 +7263,29 @@
                 "rules"
             ],
             "type": "structure"
         },
         "TopicConfigurationName": {
             "max": 36,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]{0,35}$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]{0,35}",
             "type": "string"
         },
         "TopicConfigurations": {
             "max": 10,
             "member": {
                 "shape": "TopicConfiguration"
             },
             "min": 0,
             "type": "list"
         },
         "TopicDescription": {
             "max": 350,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "UntagResourceRequest": {
             "members": {
                 "resourceARN": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon Q Business application, or data source to remove the tag from.</p>",
                     "location": "uri",
@@ -6764,14 +7325,18 @@
                     "documentation": "<p>A description for the Amazon Q Business application.</p>",
                     "shape": "Description"
                 },
                 "displayName": {
                     "documentation": "<p>A name for the Amazon Q Business application.</p>",
                     "shape": "ApplicationName"
                 },
+                "identityCenterInstanceArn": {
+                    "documentation": "<p> The Amazon Resource Name (ARN) of the IAM Identity Center instance you are either creating for\u2014or connecting to\u2014your Amazon Q Business application.</p>",
+                    "shape": "InstanceArn"
+                },
                 "roleArn": {
                     "documentation": "<p>An Amazon Web Services Identity and Access Management (IAM) role that gives Amazon Q Business permission to access Amazon CloudWatch logs and metrics.</p>",
                     "shape": "RoleArn"
                 }
             },
             "required": [
                 "applicationId"
@@ -6869,16 +7434,16 @@
                 },
                 "vpcConfiguration": {
                     "shape": "DataSourceVpcConfiguration"
                 }
             },
             "required": [
                 "applicationId",
-                "dataSourceId",
-                "indexId"
+                "indexId",
+                "dataSourceId"
             ],
             "type": "structure"
         },
         "UpdateDataSourceResponse": {
             "members": {},
             "type": "structure"
         },
@@ -6931,14 +7496,18 @@
                     "locationName": "applicationId",
                     "shape": "ApplicationId"
                 },
                 "authConfiguration": {
                     "documentation": "<p>The authentication configuration the plugin is using.</p>",
                     "shape": "PluginAuthConfiguration"
                 },
+                "customPluginConfiguration": {
+                    "documentation": "<p>The configuration for a custom plugin.</p>",
+                    "shape": "CustomPluginConfiguration"
+                },
                 "displayName": {
                     "documentation": "<p>The name of the plugin.</p>",
                     "shape": "PluginName"
                 },
                 "pluginId": {
                     "documentation": "<p>The identifier of the plugin.</p>",
                     "location": "uri",
@@ -7051,17 +7620,23 @@
                 "applicationId": {
                     "documentation": "<p>The identifier of the Amazon Q Business application attached to the web experience.</p>",
                     "location": "uri",
                     "locationName": "applicationId",
                     "shape": "ApplicationId"
                 },
                 "authenticationConfiguration": {
+                    "deprecated": true,
+                    "deprecatedMessage": "Property associated with legacy SAML IdP flow. Deprecated in favor of using AWS IAM Identity Center for user management.",
                     "documentation": "<p>The authentication configuration of the Amazon Q Business web experience.</p>",
                     "shape": "WebExperienceAuthConfiguration"
                 },
+                "roleArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the role with permission to access the Amazon Q Business web experience and required resources.</p>",
+                    "shape": "RoleArn"
+                },
                 "samplePromptsControlMode": {
                     "documentation": "<p>Determines whether sample prompts are enabled in the web experience for an end user.</p>",
                     "shape": "WebExperienceSamplePromptsControlMode"
                 },
                 "subtitle": {
                     "documentation": "<p>The subtitle of the Amazon Q Business web experience.</p>",
                     "shape": "WebExperienceSubtitle"
@@ -7090,15 +7665,15 @@
         "UpdateWebExperienceResponse": {
             "members": {},
             "type": "structure"
         },
         "Url": {
             "max": 2048,
             "min": 1,
-            "pattern": "^(https?|ftp|file)://([^\\s]*)$",
+            "pattern": "(https?|ftp|file)://([^\\s]*)",
             "type": "string"
         },
         "UserAlias": {
             "documentation": "<p>Aliases attached to a user id within an Amazon Q Business application.</p>",
             "members": {
                 "dataSourceId": {
                     "documentation": "<p>The identifier of the data source that the user aliases are associated with.</p>",
@@ -7129,15 +7704,15 @@
                 "shape": "String"
             },
             "type": "list"
         },
         "UserId": {
             "max": 1024,
             "min": 1,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "UserIds": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
@@ -7197,16 +7772,16 @@
                 },
                 "name": {
                     "documentation": "<p>The field name where the invalid entry was detected.</p>",
                     "shape": "String"
                 }
             },
             "required": [
-                "message",
-                "name"
+                "name",
+                "message"
             ],
             "type": "structure"
         },
         "ValidationExceptionFields": {
             "member": {
                 "shape": "ValidationExceptionField"
             },
@@ -7245,15 +7820,15 @@
                 }
             },
             "type": "structure"
         },
         "WebExperienceArn": {
             "max": 1284,
             "min": 0,
-            "pattern": "^arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}$",
+            "pattern": "arn:[a-z0-9-\\.]{1,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[a-z0-9-\\.]{0,63}:[^/].{0,1023}",
             "type": "string"
         },
         "WebExperienceAuthConfiguration": {
             "documentation": "<p>Provides the authorization configuration information needed to deploy a Amazon Q Business web experience to end users.</p>",
             "members": {
                 "samlConfiguration": {
                     "shape": "SamlConfiguration"
@@ -7261,15 +7836,15 @@
             },
             "type": "structure",
             "union": true
         },
         "WebExperienceId": {
             "max": 36,
             "min": 36,
-            "pattern": "^[a-zA-Z0-9][a-zA-Z0-9-]*$",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9-]*",
             "type": "string"
         },
         "WebExperienceSamplePromptsControlMode": {
             "enum": [
                 "ENABLED",
                 "DISABLED"
             ],
@@ -7284,21 +7859,21 @@
                 "PENDING_AUTH_CONFIG"
             ],
             "type": "string"
         },
         "WebExperienceSubtitle": {
             "max": 500,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "WebExperienceTitle": {
             "max": 500,
             "min": 0,
-            "pattern": "^\\P{C}*$",
+            "pattern": "\\P{C}*",
             "type": "string"
         },
         "WebExperienceWelcomeMessage": {
             "max": 300,
             "min": 0,
             "type": "string"
         },
```

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/botocore_a_la_carte_qbusiness.egg-info/PKG-INFO` & `botocore-a-la-carte-qbusiness-1.34.95/botocore_a_la_carte_qbusiness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-qbusiness
-Version: 1.34.94
+Version: 1.34.95
 Summary: qbusiness data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-qbusiness-1.34.94/setup.py` & `botocore-a-la-carte-qbusiness-1.34.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-qbusiness',
-    version="1.34.94",
+    version="1.34.95",
     description='qbusiness data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/qbusiness/*/*.json'],
```

