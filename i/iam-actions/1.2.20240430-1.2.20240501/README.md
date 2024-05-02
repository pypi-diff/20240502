# Comparing `tmp/iam_actions-1.2.20240430.tar.gz` & `tmp/iam_actions-1.2.20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240430.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240501.tar", max compression
```

## Comparing `iam_actions-1.2.20240430.tar` & `iam_actions-1.2.20240501.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/README.md
--rw-r--r--   0        0        0      228 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/__init__.py
--rw-r--r--   0        0        0  4816205 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/services.py
--rw-r--r--   0        0        0   626252 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/policies.json
--rw-r--r--   0        0        0   209050 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   607639 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-30 02:19:12.009023 iam_actions-1.2.20240430/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240430/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240430/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/README.md
+-rw-r--r--   0        0        0      228 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4821473 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   627134 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/policies.json
+-rw-r--r--   0        0        0   209154 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   608541 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-01 02:24:41.391637 iam_actions-1.2.20240501/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240501/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240501/PKG-INFO
```

### Comparing `iam_actions-1.2.20240430/LICENSE` & `iam_actions-1.2.20240501/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/README.md` & `iam_actions-1.2.20240501/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/actions.json` & `iam_actions-1.2.20240501/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973692378153256%*

 * *Differences: {"'qapps'": "OrderedDict([('UpdateLibraryItem', OrderedDict([('access_level', 'Undocumented'), "*

 * *            "('action', 'UpdateLibraryItem'), ('condition_keys', []), ('description', 'Not "*

 * *            "Documented by AWS'), ('orphan', False), ('resources', [])])), "*

 * *            "('CreateSubscriptionToken', OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *            "'CreateSubscriptionToken'), ('condition_keys', []), ('description', 'Not Documented "*

 * *            "by AWS'), ('orphan', False), ('r […]*

```diff
@@ -123392,14 +123392,184 @@
             "action": "UpdateTroubleshootingCommandResult",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
+    "qapps": {
+        "AssociateQAppWithUser": {
+            "access_level": "Undocumented",
+            "action": "AssociateQAppWithUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CopyQApp": {
+            "access_level": "Undocumented",
+            "action": "CopyQApp",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateLibraryItem": {
+            "access_level": "Undocumented",
+            "action": "CreateLibraryItem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateLibraryItemReview": {
+            "access_level": "Undocumented",
+            "action": "CreateLibraryItemReview",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateQApp": {
+            "access_level": "Undocumented",
+            "action": "CreateQApp",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateSubscriptionToken": {
+            "access_level": "Undocumented",
+            "action": "CreateSubscriptionToken",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteLibraryItem": {
+            "access_level": "Undocumented",
+            "action": "DeleteLibraryItem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteQApp": {
+            "access_level": "Undocumented",
+            "action": "DeleteQApp",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateQAppFromUser": {
+            "access_level": "Undocumented",
+            "action": "DisassociateQAppFromUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetLibraryItem": {
+            "access_level": "Undocumented",
+            "action": "GetLibraryItem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetQApp": {
+            "access_level": "Undocumented",
+            "action": "GetQApp",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ImportDocumentToQApp": {
+            "access_level": "Undocumented",
+            "action": "ImportDocumentToQApp",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ImportDocumentToQAppSession": {
+            "access_level": "Undocumented",
+            "action": "ImportDocumentToQAppSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListLibraryItems": {
+            "access_level": "Undocumented",
+            "action": "ListLibraryItems",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListQApps": {
+            "access_level": "Undocumented",
+            "action": "ListQApps",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PredictProblemStatementFromConversation": {
+            "access_level": "Undocumented",
+            "action": "PredictProblemStatementFromConversation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PredictQAppFromProblemStatement": {
+            "access_level": "Undocumented",
+            "action": "PredictQAppFromProblemStatement",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartQAppSession": {
+            "access_level": "Undocumented",
+            "action": "StartQAppSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopQAppSession": {
+            "access_level": "Undocumented",
+            "action": "StopQAppSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateLibraryItem": {
+            "access_level": "Undocumented",
+            "action": "UpdateLibraryItem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateQApp": {
+            "access_level": "Undocumented",
+            "action": "UpdateQApp",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "qbusiness": {
         "AddUserLicenses": {
             "access_level": "Undocumented",
             "action": "AddUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
@@ -123417,14 +123587,22 @@
             "access_level": "Undocumented",
             "action": "BatchPutDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "CancelSubscription": {
+            "access_level": "Undocumented",
+            "action": "CancelSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Chat": {
             "access_level": "Undocumented",
             "action": "Chat",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -123481,14 +123659,22 @@
             "access_level": "Undocumented",
             "action": "CreateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "CreateSubscription": {
+            "access_level": "Undocumented",
+            "action": "CreateSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateUser": {
             "access_level": "Undocumented",
             "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -123737,14 +123923,22 @@
             "access_level": "Undocumented",
             "action": "ListRetrievers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListSubscriptions": {
+            "access_level": "Undocumented",
+            "action": "ListSubscriptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -123865,14 +124059,22 @@
             "access_level": "Undocumented",
             "action": "UpdateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "UpdateSubscription": {
+            "access_level": "Undocumented",
+            "action": "UpdateSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateUser": {
             "access_level": "Undocumented",
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -159889,15 +160091,16 @@
             "condition_keys": [
                 "sts:RequestContext/${ContextKey}",
                 "sts:RequestContextProviders"
             ],
             "description": "Grants permission to set context keys on a STS session",
             "orphan": false,
             "resources": [
-                "role"
+                "role",
+                "self-session"
             ]
         },
         "SetSourceIdentity": {
             "access_level": "Write",
             "action": "SetSourceIdentity",
             "condition_keys": [
                 "sts:SourceIdentity"
@@ -161726,18 +161929,18 @@
             "description": "Grants permission to delete a table in your account",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
         "DescribeAccountSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAccountSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe your account settings",
             "orphan": false,
             "resources": []
         },
         "DescribeBatchLoadTask": {
             "access_level": "Read",
             "action": "DescribeBatchLoadTask",
             "condition_keys": [],
@@ -161957,18 +162160,18 @@
             "resources": [
                 "database",
                 "scheduled-query",
                 "table"
             ]
         },
         "UpdateAccountSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateAccountSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update your account settings",
             "orphan": false,
             "resources": []
         },
         "UpdateDatabase": {
             "access_level": "Write",
             "action": "UpdateDatabase",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20240430/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240501/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240501/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/generate/generate.py` & `iam_actions-1.2.20240501/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240501/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240501/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/generate/services.py` & `iam_actions-1.2.20240501/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240430/iam_actions/policies.json` & `iam_actions-1.2.20240501/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997560671283299%*

 * *Differences: {"'serviceMap'": "{'Amazon Q Business': {'Actions': {insert: [(3, 'CancelSubscription'), (12, "*

 * *                 "'CreateSubscription'), (45, 'ListSubscriptions'), (62, 'UpdateSubscription')]}}, "*

 * *                 "'Amazon Q Business Q Apps': OrderedDict([('StringPrefix', 'qapps'), ('Actions', "*

 * *                 "['AssociateQAppWithUser', 'CopyQApp', 'CreateLibraryItem', "*

 * *                 "'CreateLibraryItemReview', 'CreateQApp', 'CreateSubscriptionToken', "*

 * *                 "'DeleteLibraryItem', 'DeleteQA […]*

```diff
@@ -18840,22 +18840,24 @@
         "Amazon Q Business": {
             "ARNFormat": "arn:aws:qbusiness:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:qbusiness:.+:.+:.+",
             "Actions": [
                 "AddUserLicenses",
                 "BatchDeleteDocument",
                 "BatchPutDocument",
+                "CancelSubscription",
                 "Chat",
                 "ChatSync",
                 "CreateApplication",
                 "CreateDataSource",
                 "CreateIndex",
                 "CreateLicense",
                 "CreatePlugin",
                 "CreateRetriever",
+                "CreateSubscription",
                 "CreateUser",
                 "CreateWebExperience",
                 "DeleteApplication",
                 "DeleteChatControlsConfiguration",
                 "DeleteConversation",
                 "DeleteDataSource",
                 "DeleteGroup",
@@ -18880,14 +18882,15 @@
                 "ListDataSources",
                 "ListDocuments",
                 "ListGroups",
                 "ListIndices",
                 "ListMessages",
                 "ListPlugins",
                 "ListRetrievers",
+                "ListSubscriptions",
                 "ListTagsForResource",
                 "ListUserLicenses",
                 "ListWebExperiences",
                 "PutFeedback",
                 "PutGroup",
                 "RemoveUserLicenses",
                 "StartDataSourceSyncJob",
@@ -18896,25 +18899,55 @@
                 "UntagResource",
                 "UpdateApplication",
                 "UpdateChatControlsConfiguration",
                 "UpdateDataSource",
                 "UpdateIndex",
                 "UpdatePlugin",
                 "UpdateRetriever",
+                "UpdateSubscription",
                 "UpdateUser",
                 "UpdateWebExperience"
             ],
             "HasResource": true,
             "StringPrefix": "qbusiness",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "Amazon Q Business Q Apps": {
+            "ARNFormat": "arn:aws:qapps:${Region}:${Account}:${ResourceType}:${ResourcePath}",
+            "ARNRegex": "^arn:aws:qapps:.+:.+:.+",
+            "Actions": [
+                "AssociateQAppWithUser",
+                "CopyQApp",
+                "CreateLibraryItem",
+                "CreateLibraryItemReview",
+                "CreateQApp",
+                "CreateSubscriptionToken",
+                "DeleteLibraryItem",
+                "DeleteQApp",
+                "DisassociateQAppFromUser",
+                "GetLibraryItem",
+                "GetQApp",
+                "ImportDocumentToQApp",
+                "ImportDocumentToQAppSession",
+                "ListLibraryItems",
+                "ListQApps",
+                "PredictProblemStatementFromConversation",
+                "PredictQAppFromProblemStatement",
+                "StartQAppSession",
+                "StopQAppSession",
+                "UpdateLibraryItem",
+                "UpdateQApp"
+            ],
+            "HasResource": true,
+            "StringPrefix": "qapps"
+        },
         "Amazon Q in Connect": {
             "ARNFormat": "arn:aws:wisdom:${Region}:${Account}:${Resource}/${ResourceId}",
             "ARNRegex": "^arn:aws:wisdom:.+:.+:.+",
             "Actions": [
                 "CreateAssistant",
                 "CreateAssistantAssociation",
                 "CreateContent",
```

### Comparing `iam_actions-1.2.20240430/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240501/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970313825275657%*

 * *Differences: {"'qapps'": 'OrderedDict()',*

 * * "'sts'": "{'self-session': OrderedDict([('arn_pattern', 'arn:*:sts::*:self'), ('condition_keys', "*

 * *          'None)])}'}*

```diff
@@ -5133,14 +5133,15 @@
     "purchase-orders": {
         "purchase-order": {
             "arn_pattern": "arn:*:purchase-orders::*:purchase-order/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "q": {},
+    "qapps": {},
     "qbusiness": {},
     "qldb": {
         "catalog": {
             "arn_pattern": "arn:*:qldb:*:*:ledger/*/information_schema/user_tables",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "ledger": {
@@ -6559,14 +6560,18 @@
         }
     },
     "sts": {
         "role": {
             "arn_pattern": "arn:*:iam::*:role/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "self-session": {
+            "arn_pattern": "arn:*:sts::*:self",
+            "condition_keys": null
+        },
         "user": {
             "arn_pattern": "arn:*:iam::*:user/*",
             "condition_keys": null
         }
     },
     "support": {},
     "supportapp": {},
```

### Comparing `iam_actions-1.2.20240430/iam_actions/services.json` & `iam_actions-1.2.20240501/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974489463039081%*

 * *Differences: {"'qapps'": "OrderedDict([('Actions', ['AssociateQAppWithUser', 'CopyQApp', 'CreateLibraryItem', "*

 * *            "'CreateLibraryItemReview', 'CreateQApp', 'CreateSubscriptionToken', "*

 * *            "'DeleteLibraryItem', 'DeleteQApp', 'DisassociateQAppFromUser', 'GetLibraryItem', "*

 * *            "'GetQApp', 'ImportDocumentToQApp', 'ImportDocumentToQAppSession', 'ListLibraryItems', "*

 * *            "'ListQApps', 'PredictProblemStatementFromConversation', "*

 * *            "'PredictQAppFromProblemStatement', 'StartQAppSess […]*

```diff
@@ -17362,33 +17362,71 @@
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "Amazon Q"
         ]
     },
+    "qapps": {
+        "ARNFormats": [
+            "arn:aws:qapps:${Region}:${Account}:${ResourceType}:${ResourcePath}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:qapps:.+:.+:.+"
+        ],
+        "Actions": [
+            "AssociateQAppWithUser",
+            "CopyQApp",
+            "CreateLibraryItem",
+            "CreateLibraryItemReview",
+            "CreateQApp",
+            "CreateSubscriptionToken",
+            "DeleteLibraryItem",
+            "DeleteQApp",
+            "DisassociateQAppFromUser",
+            "GetLibraryItem",
+            "GetQApp",
+            "ImportDocumentToQApp",
+            "ImportDocumentToQAppSession",
+            "ListLibraryItems",
+            "ListQApps",
+            "PredictProblemStatementFromConversation",
+            "PredictQAppFromProblemStatement",
+            "StartQAppSession",
+            "StopQAppSession",
+            "UpdateLibraryItem",
+            "UpdateQApp"
+        ],
+        "ConditionKeys": [],
+        "HasResource": true,
+        "ServiceNames": [
+            "Amazon Q Business Q Apps"
+        ]
+    },
     "qbusiness": {
         "ARNFormats": [
             "arn:aws:qbusiness:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:qbusiness:.+:.+:.+"
         ],
         "Actions": [
             "AddUserLicenses",
             "BatchDeleteDocument",
             "BatchPutDocument",
+            "CancelSubscription",
             "Chat",
             "ChatSync",
             "CreateApplication",
             "CreateDataSource",
             "CreateIndex",
             "CreateLicense",
             "CreatePlugin",
             "CreateRetriever",
+            "CreateSubscription",
             "CreateUser",
             "CreateWebExperience",
             "DeleteApplication",
             "DeleteChatControlsConfiguration",
             "DeleteConversation",
             "DeleteDataSource",
             "DeleteGroup",
@@ -17413,14 +17451,15 @@
             "ListDataSources",
             "ListDocuments",
             "ListGroups",
             "ListIndices",
             "ListMessages",
             "ListPlugins",
             "ListRetrievers",
+            "ListSubscriptions",
             "ListTagsForResource",
             "ListUserLicenses",
             "ListWebExperiences",
             "PutFeedback",
             "PutGroup",
             "RemoveUserLicenses",
             "StartDataSourceSyncJob",
@@ -17429,14 +17468,15 @@
             "UntagResource",
             "UpdateApplication",
             "UpdateChatControlsConfiguration",
             "UpdateDataSource",
             "UpdateIndex",
             "UpdatePlugin",
             "UpdateRetriever",
+            "UpdateSubscription",
             "UpdateUser",
             "UpdateWebExperience"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20240430/pyproject.toml` & `iam_actions-1.2.20240501/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240430"
+version = "1.2.20240501"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240430/setup.py` & `iam_actions-1.2.20240501/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240430',
+    'version': '1.2.20240501',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240430/PKG-INFO` & `iam_actions-1.2.20240501/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240430
+Version: 1.2.20240501
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

