# Comparing `tmp/cdk-sops-secrets-1.7.1.tar.gz` & `tmp/cdk-sops-secrets-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.7.1.tar", last modified: Tue Apr 30 10:09:00 2024, max compression
+gzip compressed data, was "cdk-sops-secrets-1.7.2.tar", last modified: Thu May  2 15:07:52 2024, max compression
```

## Comparing `cdk-sops-secrets-1.7.1.tar` & `cdk-sops-secrets-1.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:00.381618 cdk-sops-secrets-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-30 10:09:00.381618 cdk-sops-secrets-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:09:00.381618 cdk-sops-secrets-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:00.365618 cdk-sops-secrets-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:00.369618 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    76606 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:00.369618 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  8963928 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.7.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:08:50.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:00.369618 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-30 10:09:00.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 10:09:00.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:09:00.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 10:09:00.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 10:09:00.000000 cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:52.641734 cdk-sops-secrets-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-02 15:07:52.641734 cdk-sops-secrets-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:07:52.641734 cdk-sops-secrets-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:52.629734 cdk-sops-secrets-1.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:52.629734 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76606 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:52.633734 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8963934 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.7.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:07:38.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:52.633734 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-02 15:07:52.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 15:07:52.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:07:52.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 15:07:52.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 15:07:52.000000 cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.7.1/LICENSE` & `cdk-sops-secrets-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.7.1/PKG-INFO` & `cdk-sops-secrets-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.7.1
+Version: 1.7.2
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-sops-secrets-1.7.1/README.md` & `cdk-sops-secrets-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.7.1/setup.py` & `cdk-sops-secrets-1.7.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.7.1",
+    "version": "1.7.2",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<markus.siebert@deutschebahn.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.7.1.jsii.tgz"
+            "cdk-sops-secrets@1.7.2.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.7.1/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.7.1.jsii.tgz` & `cdk-sops-secrets-1.7.2/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.7.2.jsii.tgz`

 * *Files 26% similar despite different names*

#### Comparing `cdk-sops-secrets@1.7.1.jsii.tgz-content` & `cdk-sops-secrets@1.7.2.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'fingerprint'": "'XETUa75BenKjnP9fumgYqzSvCGuPI5I4eeAv0Jwlhl8='",*

 * * "'jsiiVersion'": "'1.98.0 (build 00b106d)'",*

 * * "'version'": "'1.7.2'"}*

```diff
@@ -2771,17 +2771,17 @@
             }
         }
     },
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "docs": {
         "stability": "experimental"
     },
-    "fingerprint": "gdYpPs8C3lERRywaaH5WkyirE+G5C7co0wjlH1GcbvQ=",
+    "fingerprint": "XETUa75BenKjnP9fumgYqzSvCGuPI5I4eeAv0Jwlhl8=",
     "homepage": "https://constructs.dev/packages/cdk-sops-secrets",
-    "jsiiVersion": "1.97.0 (build 729de35)",
+    "jsiiVersion": "1.98.0 (build 00b106d)",
     "keywords": [
         "cdk",
         "gitops",
         "kms",
         "mozilla/sops",
         "secrets",
         "secrets management",
@@ -3672,9 +3672,9 @@
                     "name": "ASSET"
                 }
             ],
             "name": "UploadType",
             "symbolId": "src/index:UploadType"
         }
     },
-    "version": "1.7.1"
+    "version": "1.7.2"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -142,15 +142,15 @@
         this.versionId = cr.getAttString('VersionId');
     }
 }
 exports.SopsSync = SopsSync;
 _a = JSII_RTTI_SYMBOL_1;
 SopsSync[_a] = {
     fqn: "cdk-sops-secrets.SopsSync",
-    version: "1.7.1"
+    version: "1.7.2"
 };
 class SopsSyncProvider extends aws_lambda_1.SingletonFunction {
     constructor(scope, id) {
         super(scope, id ?? 'SopsSyncProvider', {
             code: aws_lambda_1.Code.fromAsset(scope.node.tryGetContext('sops_sync_provider_asset_path') ||
                 path.join(__dirname, '../assets/cdk-sops-lambda.zip')),
             runtime: aws_lambda_1.Runtime.PROVIDED_AL2,
@@ -169,15 +169,15 @@
         this.sopsAgeKeys.push(key);
     }
 }
 exports.SopsSyncProvider = SopsSyncProvider;
 _b = JSII_RTTI_SYMBOL_1;
 SopsSyncProvider[_b] = {
     fqn: "cdk-sops-secrets.SopsSyncProvider",
-    version: "1.7.1"
+    version: "1.7.2"
 };
 /**
  * A drop in replacement for the normal Secret, that is populated with the encrypted
  * content of the given sops file.
  */
 class SopsSecret extends constructs_1.Construct {
     constructor(scope, id, props) {
@@ -234,10 +234,10 @@
         return this.secretValueFromJson('');
     }
 }
 exports.SopsSecret = SopsSecret;
 _c = JSII_RTTI_SYMBOL_1;
 SopsSecret[_c] = {
     fqn: "cdk-sops-secrets.SopsSecret",
-    version: "1.7.1"
+    version: "1.7.2"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSx5QkFBeUI7QUFDekIsNkJBQTZCO0FBQzdCLG1DQUFtQztBQUNuQyw2Q0FVcUI7QUFPckIsaURBQWdEO0FBQ2hELHVEQUEwRTtBQUMxRSw2REFBa0Q7QUFDbEQsdUVBT3dDO0FBQ3hDLDJDQUF1QztBQUV2QyxJQUFZLFVBU1g7QUFURCxXQUFZLFVBQVU7SUFDcEI7O09BRUc7SUFDSCwrQkFBaUIsQ0FBQTtJQUNqQjs7T0FFRztJQUNILDZCQUFlLENBQUE7QUFDakIsQ0FBQyxFQVRXLFVBQVUsR0FBVixrQkFBVSxLQUFWLGtCQUFVLFFBU3JCO0FBK0VEOztHQUVHO0FBQ0gsTUFBYSxRQUFTLFNBQVEsc0JBQVM7SUEwQnJDLFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBb0I7UUFDNUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLENBQUMsQ0FBQztRQUVqQixJQUFJLENBQUMsWUFBWSxHQUFHLEtBQUssQ0FBQyxhQUFhLElBQUksSUFBSSxDQUFDO1FBQ2hELElBQUksQ0FBQyxPQUFPLEdBQUcsS0FBSyxDQUFDLE9BQU8sSUFBSSxJQUFJLENBQUM7UUFDckMsSUFBSSxDQUFDLGlCQUFpQixHQUFHLEtBQUssQ0FBQyxlQUFlLElBQUksSUFBSSxDQUFDO1FBRXZELE1BQU0sY0FBYyxHQUNsQixLQUFLLENBQUMsY0FBYyxJQUFJLEtBQUssQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUFDLEdBQUcsQ0FBQyxDQUFDLEdBQUcsRUFBRSxDQUFDO1FBQzlELFFBQVEsY0FBYyxFQUFFO1lBQ3RCLEtBQUssTUFBTSxDQUFDLENBQUM7Z0JBQ1gsSUFBSSxDQUFDLGNBQWMsR0FBRyxNQUFNLENBQUM7Z0JBQzdCLE1BQU07YUFDUDtZQUNELEtBQUssTUFBTSxDQUFDLENBQUM7Z0JBQ1gsSUFBSSxDQUFDLGNBQWMsR0FBRyxN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QVcsQ0FBQyxjQUFjLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRTtZQUNoRCxTQUFTO1lBQ1QsU0FBUyxFQUFFLElBQUksQ0FBQyxJQUFJLENBQUMsU0FBUztTQUMvQixDQUFDLENBQUM7SUFDTCxDQUFDO0lBRUQsSUFBVyxXQUFXO1FBQ3BCLE9BQU8sSUFBSSxDQUFDLG1CQUFtQixDQUFDLEVBQUUsQ0FBQyxDQUFDO0lBQ3RDLENBQUM7O0FBL0VILGdDQWdGQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCAqIGFzIGZzIGZyb20gJ2ZzJztcbmltcG9ydCAqIGFzIHBhdGggZnJvbSAncGF0aCc7XG4vL2ltcG9ydCAqIGFzIGNyeXB0byBmcm9tICdjcnlwdG8nO1xuaW1wb3J0IHtcbiAgQW5ub3RhdGlvbnMsXG4gIEN1c3RvbVJlc291cmNlLFxuICBEdXJhdGlvbixcbiAgRmlsZVN5c3RlbSxcbiAgTGF6eSxcbiAgUmVtb3ZhbFBvbGljeSxcbiAgUmVzb3VyY2VFbnZpcm9ubWVudCxcbiAgU2VjcmV0VmFsdWUsXG4gIFN0YWNrLFxufSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQge1xuICBJR3JhbnRhYmxlLFxuICBHcmFudCxcbiAgUG9saWN5U3RhdGVtZW50LFxuICBBZGRUb1Jlc291cmNlUG9saWN5UmVzdWx0LFxufSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtaWFtJztcbmltcG9ydCB7IElLZXksIEtleSB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1rbXMnO1xuaW1wb3J0IHsgQ29kZSwgUnVudGltZSwgU2luZ2xldG9uRnVuY3Rpb24gfSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtbGFtYmRhJztcbmltcG9ydCB7IEFzc2V0IH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLXMzLWFzc2V0cyc7XG5pbXBvcnQge1xuICBJU2VjcmV0LFxuICBJU2VjcmV0QXR0YWNobWVudFRhcmdldCxcbiAgUm90YXRpb25TY2hlZHVsZSxcbiAgUm90YXRpb25TY2hlZHVsZU9wdGlvbnMsXG4gIFNlY3JldCxcbiAgU2VjcmV0UHJvcHMsXG59IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zZWNyZXRzbWFuYWdlcic7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuZXhwb3J0IGVudW0gVXBsb2FkVHlwZSB7XG4gIC8qKlxuICAgKiBQYXNzIHRoZSBzZWNyZXQgZGF0YSBpbmxpbmUgKGJhc2U2NCBlbmNvZGVkIGFuZCBjb21wcmVzc2VkKVxuICAgKi9cbiAgSU5MSU5FID0gJ0lOTElORScsXG4gIC8qKlxuICAgKiBVcGxhb2QgdGhlIHNlY2VydCBkYXRhIGFzIGFzc2V0XG4gICAqL1xuICBBU1NFVCA9ICdBU1NFVCcsXG59XG5cbi8qKlxuICogQ29uZmlndXJhdGlvbiBvcHRpb25zIGZvciB0aGUgU29wc1N5bmNcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBTb3BzU3luY09wdGlvbnMge1xuICAvKipcbiAgICogVGhlIGN1c3RvbSByZXNvdXJjZSBwcm92aWRlciB0byB1c2UuIElmIHlvdSBkb24ndCBzcGVjaWZ5IGFueSwgYSBuZXdcbiAgICogcHJvdmlkZXIgd2lsbCBiZSBjcmVhdGVkIC0gb3IgaWYgYWxyZWFkeSBleGlzdHMgd2l0aGluIHRoaXMgc3RhY2sgLSByZXVzZWQuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gQSBuZXcgc2luZ2xldG9uIHByb3ZpZGVyIHdpbGwgYmUgY3JlYXRlZFxuICAgKi9cbiAgcmVhZG9ubHkgc29wc1Byb3ZpZGVyPzogU29wc1N5bmNQcm92aWRlcjtcblxuICAvKipcbiAgICogVGhlIGZpbGVwYXRoIHRvIHRoZSBzb3BzIGZpbGVcbiAgICovXG4gIHJlYWRvbmx5IHNvcHNGaWxlUGF0aDogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBIb3cgc2hvdWxkIHRoZSBzZWNyZXQgYmUgcGFzc2VkIHRvIHRoZSBDdXN0b21SZXNvdXJjZT9cbiAgICogQGRlZmF1bHQgSU5MSU5FXG4gICAqL1xuICByZWFkb25seSB1cGxvYWRUeXBlPzogVXBsb2FkVHlwZTtcblxuICAvKipcbiAgICogVGhlIGZvcm1hdCBvZiB0aGUgc29wcyBmaWxlLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIFRoZSBmaWxlZm9ybWF0IHdpbGwgYmUgZGVyaXZlZCBmcm9tIHRoZSBmaWxlIGVuZGluZ1xuICAgKi9cbiAgcmVhZG9ubHkgc29wc0ZpbGVGb3JtYXQ/OiB1bmRlZmluZWQgfCAnanNvbicgfCAneWFtbCcgfCAnZG90ZW52JztcblxuICAvKipcbiAgICogVGhlIGttc0tleSB1c2VkIHRvIGVuY3J5cHQgdGhlIHNvcHMgZmlsZS4gRW5jcnlwdCBwZXJtaXNzaW9uc1xuICAgKiB3aWxsIGJlIGdyYW50ZWQgdG8gdGhlIGN1c3RvbSByZXNvdXJjZSBwcm92aWRlci5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBUaGUga2V5IHdpbGwgYmUgZGVyaXZlZCBmcm9tIHRoZSBzb3BzIGZpbGVcbiAgICovXG4gIHJlYWRvbmx5IHNvcHNLbXNLZXk/OiBJS2V5W107XG5cbiAgLyoqXG4gICAqIFRoZSBhZ2Uga2V5IHRoYXQgc2hvdWxkIGJlIHVzZWQgZm9yIGVuY3J5cHRpb24uXG4gICAqL1xuICByZWFkb25seSBzb3BzQWdlS2V5PzogU2VjcmV0VmFsdWU7XG5cbiAgLyoqXG4gICAqIFNob3VsZCB0aGUgZW5jcnlwdGVkIHNvcHMgdmFsdWUgc2hvdWxkIGJlIGNvbnZlcnRlZCB0byBKU09OP1xuICAgKiBPbmx5IEpTT04gY2FuIGJlIGhhbmRsZWQgYnkgY2xvdWQgZm9ybWF0aW9ucyBkeW5hbWljIHJlZmVyZW5jZXMuXG4gICAqXG4gICAqIEBkZWZhdWx0IHRydWVcbiAgICovXG4gIHJlYWRvbmx5IGNvbnZlcnRUb0pTT04/OiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBTaG91bGQgdGhlIHN0cnVjdHVyZSBiZSBmbGF0dGVuZWQ/IFRoZSByZXN1bHQgd2lsbCBiZSBhIGZsYXQgc3RydWN0dXJlIGFuZCBhbGxcbiAgICogb2JqZWN0IGtleXMgd2lsbCBiZSByZXBsYWNlZCB3aXRoIHRoZSBmdWxsIGpzb25wYXRoIGFzIGtleS5cbiAgICogVGhpcyBpcyB1c2VmdWxsIGZvciBkeW5hbWljIHJlZmVyZW5jZXMsIGFzIHRob3NlIGRvbid0IHN1cHBvcnQgbmVzdGVkIG9iamVjdHMuXG4gICAqXG4gICAqIEBkZWZhdWx0IHRydWVcbiAgICovXG4gIHJlYWRvbmx5IGZsYXR0ZW4/OiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBTaGFsbCBhbGwgdmFsdWVzIGJlIGZsYXR0ZW5lZD8gVGhpcyBpcyB1c2VmdWxsIGZvciBkeW5hbWljIHJlZmVyZW5jZXMsIGFzIHRoZXJlXG4gICAqIGFyZSBsb29rdXAgZXJyb3JzIGZvciBjZXJ0YWluIGZsb2F0IHR5cGVzXG4gICAqL1xuICByZWFkb25seSBzdHJpbmdpZnlWYWx1ZXM/OiBib29sZWFuO1xufVxuXG4vKipcbiAqIFRoZSBjb25maWd1cmF0aW9uIG9wdGlvbnMgZXh0ZW5kZWQgYnkgdGhlIHRhcmdldCBTZWNyZXRcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBTb3BzU3luY1Byb3BzIGV4dGVuZHMgU29wc1N5bmNPcHRpb25zIHtcbiAgLyoqXG4gICAqIFRoZSBzZWNyZXQgdGhhdCB3aWxsIGJlIHBvcHVsYXRlZCB3aXRoIHRoZSBlbmNyeXB0ZWQgc29wcyBmaWxlIGNvbnRlbnQuXG4gICAqL1xuICByZWFkb25seSBzZWNyZXQ6IElTZWNyZXQ7XG59XG5cbi8qKlxuICogVGhlIGN1c3RvbSByZXNvdXJjZSwgdGhhdCBpcyBzeW5jaW5nIHRoZSBjb250ZW50IGZyb20gYSBzb3BzIGZpbGUgdG8gYSBzZWNyZXQuXG4gKi9cbmV4cG9ydCBjbGFzcyBTb3BzU3luYyBleHRlbmRzIENvbnN0cnVjdCB7XG4gIC8qKlxuICAgKiBUaGUgY3VycmVudCB2ZXJzaW9uSWQgb2YgdGhlIHNlY3JldCBwb3B1bGF0ZWQgdmlhIHRoaXMgcmVzb3VyY2VcbiAgICovXG4gIHJlYWRvbmx5IHZlcnNpb25JZDogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBUaGUgZm9ybWF0IG9mIHRoZSBpbnB1dCBmaWxlXG4gICAqL1xuICByZWFkb25seSBzb3BzRmlsZUZvcm1hdDogJ2pzb24nIHwgJ3lhbWwnIHwgJ2RvdGVudic7XG5cbiAgLyoqXG4gICAqIFdhcyB0aGUgZm9ybWF0IGNvbnZlcnRlZCB0byBqc29uP1xuICAgKi9cbiAgcmVhZG9ubHkgY29udmVyVG9KU09OOiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBXYXMgdGhlIHN0cnVjdHVyZSBmbGF0dGVuZWQ/XG4gICAqL1xuICByZWFkb25seSBmbGF0dGVuOiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBXZXJlIHRoZSB2YWx1ZXMgc3RyaW5naWZpZWQ/XG4gICAqL1xuICByZWFkb25seSBzdHJpbmdpZmllZFZhbHVlczogYm9vbGVhbjtcblxuICBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogU29wc1N5bmNQcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG5cbiAgICB0aGlzLmNvbnZlclRvSlNPTiA9IHByb3BzLmNvbnZlcnRUb0pTT04gPz8gdHJ1ZTtcbiAgICB0aGlzLmZsYXR0ZW4gPSBwcm9wcy5mbGF0dGVuID8/IHRydWU7XG4gICAgdGhpcy5zdHJpbmdpZmllZFZhbHVlcyA9IHByb3BzLnN0cmluZ2lmeVZhbHVlcyA/PyB0cnVlO1xuXG4gICAgY29uc3Qgc29wc0ZpbGVGb3JtYXQgPVxuICAgICAgcHJvcHMuc29wc0ZpbGVGb3JtYXQgPz8gcHJvcHMuc29wc0ZpbGVQYXRoLnNwbGl0KCcuJykucG9wKCk7XG4gICAgc3dpdGNoIChzb3BzRmlsZUZvcm1hdCkge1xuICAgICAgY2FzZSAnanNvbic6IHtcbiAgICAgICAgdGhpcy5zb3BzRmlsZUZvcm1hdCA9ICdqc29uJztcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBjYXNlICd5YW1sJzoge1xuICAgICAgICB0aGlzLnNvcHNGaWxlRm9ybWF0ID0gJ3lhbWwnO1xuICAgICAgICBicmVhaztcbiAgICAgIH1cbiAgICAgIGNhc2UgJ3ltbCc6IHtcbiAgICAgICAgdGhpcy5zb3BzRmlsZUZvcm1hdCA9ICd5YW1sJztcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBjYXNlICdlbnYnOiB7XG4gICAgICAgIHRoaXMuc29wc0ZpbGVGb3JtYXQgPSAnZG90ZW52JztcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBkZWZhdWx0OiB7XG4gICAgICAgIHRocm93IG5ldyBFcnJvcihgVW5zdXBwb3J0ZWQgc29wc0ZpbGVGb3JtYXQgJHtzb3BzRmlsZUZvcm1hdH1gKTtcbiAgICAgIH1cbiAgICB9XG5cbiAgICBjb25zdCBwcm92aWRlciA9IHByb3BzLnNvcHNQcm92aWRlciA/PyBuZXcgU29wc1N5bmNQcm92aWRlcihzY29wZSk7XG5cbiAgICBpZiAoIWZzLmV4aXN0c1N5bmMocHJvcHMuc29wc0ZpbGVQYXRoKSkge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKGBGaWxlICR7cHJvcHMuc29wc0ZpbGVQYXRofSBkb2VzIG5vdCBleGlzdCFgKTtcbiAgICB9XG5cbiAgICAvKipcbiAgICAgKiBIYW5kbGUgdXBsb2FkVHlwZSBJTkxJTkUgb3IgQVNTRVRcbiAgICAgKi9cbiAgICBjb25zdCB1cGxvYWRUeXBlID0gcHJvcHMudXBsb2FkVHlwZSA/PyBVcGxvYWRUeXBlLklOTElORTtcbiAgICBsZXQgc29wc0Fzc2V0OiBBc3NldCB8IHVuZGVmaW5lZCA9IHVuZGVmaW5lZDtcbiAgICBsZXQgc29wc0lubGluZTogeyBDb250ZW50OiBzdHJpbmc7IEhhc2g6IHN0cmluZyB9IHwgdW5kZWZpbmVkID0gdW5kZWZpbmVkO1xuICAgIGxldCBzb3BzUzNGaWxlOiB7IEJ1Y2tldDogc3RyaW5nOyBLZXk6IHN0cmluZyB9IHwgdW5kZWZpbmVkID0gdW5kZWZpbmVkO1xuXG4gICAgc3dpdGNoICh1cGxvYWRUeXBlKSB7XG4gICAgICBjYXNlIFVwbG9hZFR5cGUuSU5MSU5FOiB7XG4gICAgICAgIHNvcHNJbmxpbmUgPSB7XG4gICAgICAgICAgQ29udGVudDogZnMucmVhZEZpbGVTeW5jKHByb3BzLnNvcHNGaWxlUGF0aCkudG9TdHJpbmcoJ2Jhc2U2NCcpLFxuICAgICAgICAgIC8vIFdlIGNhbGN1bGF0ZSB0aGUgaGFzaCB0aGUgc2FtZSB3YXkgYXMgaXQgd291bGQgYmUgZG9uZSBieSBuZXcgQXNzZXQoLi4pIC0gc28gd2UgY2FuIGVuc3VyZSBzdGFibGUgdmVyc2lvbiBuYW1lcyBldmVuIGlmIHN3aXRjaGluZyBmcm9tIElOTElORSB0byBBU1NFVCBhbmQgdmljZXZlcnNhLlxuICAgICAgICAgIEhhc2g6IEZpbGVTeXN0ZW0uZmluZ2VycHJpbnQocHJvcHMuc29wc0ZpbGVQYXRoKSxcbiAgICAgICAgfTtcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBjYXNlIFVwbG9hZFR5cGUuQVNTRVQ6IHtcbiAgICAgICAgc29wc0Fzc2V0ID0gbmV3IEFzc2V0KHRoaXMsICdBc3NldCcsIHtcbiAgICAgICAgICBwYXRoOiBwcm9wcy5zb3BzRmlsZVBhdGgsXG4gICAgICAgIH0pO1xuICAgICAgICBzb3BzUzNGaWxlID0ge1xuICAgICAgICAgIEJ1Y2tldDogc29wc0Fzc2V0LmJ1Y2tldC5idWNrZXROYW1lLFxuICAgICAgICAgIEtleTogc29wc0Fzc2V0LnMzT2JqZWN0S2V5LFxuICAgICAgICB9O1xuICAgICAgICBicmVhaztcbiAgICAgIH1cbiAgICB9XG5cbiAgICBpZiAocHJvdmlkZXIucm9sZSAhPT0gdW5kZWZpbmVkKSB7XG4gICAgICBpZiAocHJvcHMuc29wc0ttc0tleSAhPT0gdW5kZWZpbmVkKSB7XG4gICAgICAgIHByb3BzLnNvcHNLbXNLZXkuZm9yRWFjaCgoa2V5KSA9PiBrZXkuZ3JhbnREZWNyeXB0KHByb3ZpZGVyLnJvbGUhKSk7XG4gICAgICB9XG4gICAgICBjb25zdCBmaWxlQ29udGVudCA9IGZzLnJlYWRGaWxlU3luYyhwcm9wcy5zb3BzRmlsZVBhdGgpO1xuICAgICAgLy8gSGFuZGxlIGtleXNcbiAgICAgIGNvbnN0IHJlZ2V4S2V5ID0gL2Fybjphd3M6a21zOlthLXowLTktXSs6W1xcZF0rOmtleVxcL1thLXowLTktXSsvZztcbiAgICAgIGNvbnN0IHJlc3VsdHNLZXkgPSBmaWxlQ29udGVudC50b1N0cmluZygpLm1hdGNoKHJlZ2V4S2V5KTtcbiAgICAgIGlmIChyZXN1bHRzS2V5ICE9PSB1bmRlZmluZWQpIHtcbiAgICAgICAgcmVzdWx0c0tleT8uZm9yRWFjaCgocmVzdWx0LCBpbmRleCkgPT5cbiAgICAgICAgICBLZXkuZnJvbUtleUFybih0aGlzLCBgU29wc0tleSR7aW5kZXh9YCwgcmVzdWx0KS5ncmFudERlY3J5cHQoXG4gICAgICAgICAgICBwcm92aWRlci5yb2xlISxcbiAgICAgICAgICApLFxuICAgICAgICApO1xuICAgICAgfVxuICAgICAgY29uc3QgcmVnZXhBbGlhcyA9IC9hcm46YXdzOmttczpbYS16MC05LV0rOltcXGRdKzphbGlhc1xcL1thLXowLTktXSsvZztcbiAgICAgIGNvbnN0IHJlc3VsdHNBbGlhcyA9IGZpbGVDb250ZW50LnRvU3RyaW5nKCkubWF0Y2gocmVnZXhBbGlhcyk7XG4gICAgICBpZiAocmVzdWx0c0FsaWFzICE9PSB1bmRlZmluZWQpIHtcbiAgICAgICAgcmVzdWx0c0FsaWFzPy5mb3JFYWNoKChyZXN1bHQsIGluZGV4KSA9PlxuICAgICAgICAgIEtleS5mcm9tTG9va3VwKHRoaXMsIGBTb3BzQWxpYXMke2luZGV4fWAsIHtcbiAgICAgICAgICAgIGFsaWFzTmFtZTogYGFsaWFzLyR7cmVzdWx0LnNwbGl0KCcvJykuc2xpY2UoMSkuam9pbignLycpfWAsXG4gICAgICAgICAgfSkuZ3JhbnREZWNyeXB0KHByb3ZpZGVyLnJvbGUhKSxcbiAgICAgICAgKTtcbiAgICAgIH1cbiAgICAgIHByb3BzLnNlY3JldC5ncmFudFdyaXRlKHByb3ZpZGVyKTtcbiAgICAgIGlmIChzb3BzQXNzZXQgIT09IHVuZGVmaW5lZCkge1xuICAgICAgICBzb3BzQXNzZXQuYnVja2V0LmdyYW50UmVhZChwcm92aWRlcik7XG4gICAgICB9XG4gICAgICAvKipcbiAgICAgICAqIGZpeGVzICMyMzRcbiAgICAgICAqIElmIHRoZSBrbXMga2V5IGZvciBzZWNyZXRzIGVuY3J5cHRpb24gaXMgYW4gSUtleVxuICAgICAgICogdGhlcmUgd2lsbCBiZSBubyBwZXJtaXNzaW9ucyBvdGhlcndpc2VcbiAgICAgICAqL1xuICAgICAgaWYgKFxuICAgICAgICBwcm9wcy5zZWNyZXQuZW5jcnlwdGlvbktleSAhPT0gdW5kZWZpbmVkICYmXG4gICAgICAgICEocHJvcHMuc2VjcmV0LmVuY3J5cHRpb25LZXkgaW5zdGFuY2VvZiBLZXkpXG4gICAgICApIHtcbiAgICAgICAgcHJvcHMuc2VjcmV0LmVuY3J5cHRpb25LZXkuZ3JhbnRFbmNyeXB0RGVjcnlwdChwcm92aWRlcik7XG4gICAgICB9XG4gICAgfSBlbHNlIHtcbiAgICAgIEFubm90YXRpb25zLm9mKHRoaXMpLmFkZFdhcm5pbmcoXG4gICAgICAgIGBQbGVhc2UgZW5zdXJlIHByb3BwZXIgcGVybWlzc2lvbnMgZm9yIHRoZSBwYXNzZWQgbGFtYmRhIGZ1bmN0aW9uOlxcbiAgLSB3cml0ZSBBY2Nlc3MgdG8gdGhlIHNlY3JldFxcbiAgLSBlbmNyeXB0IHdpdGggdGhlIHNvcHNLbXNLZXkke1xuICAgICAgICAgIHVwbG9hZFR5cGUgPT09IFVwbG9hZFR5cGUuQVNTRVRcbiAgICAgICAgICAgID8gJ1xcbiAgLSBkb3dubG9hZCBmcm9tIGFzc2V0IGJ1Y2tldCdcbiAgICAgICAgICAgIDogJydcbiAgICAgICAgfWAsXG4gICAgICApO1xuICAgIH1cbiAgICBpZiAocHJvcHMuc29wc0FnZUtleSAhPT0gdW5kZWZpbmVkKSB7XG4gICAgICBwcm92aWRlci5hZGRBZ2VLZXkocHJvcHMuc29wc0FnZUtleSk7XG4gICAgfVxuXG4gICAgY29uc3QgY3IgPSBuZXcgQ3VzdG9tUmVzb3VyY2UodGhpcywgJ1Jlc291cmNlJywge1xuICAgICAgc2VydmljZVRva2VuOiBwcm92aWRlci5mdW5jdGlvbkFybixcbiAgICAgIHJlc291cmNlVHlwZTogJ0N1c3RvbTo6U29wc1N5bmMnLFxuICAgICAgcHJvcGVydGllczoge1xuICAgICAgICBTZWNyZXRBUk46IHByb3BzLnNlY3JldC5zZWNyZXRBcm4sXG4gICAgICAgIFNvcHNTM0ZpbGU6IHNvcHNTM0ZpbGUsXG4gICAgICAgIFNvcHNJbmxpbmU6IHNvcHNJbmxpbmUsXG4gICAgICAgIENvbnZlcnRUb0pTT046IHRoaXMuY29udmVyVG9KU09OLFxuICAgICAgICBGbGF0dGVuOiB0aGlzLmZsYXR0ZW4sXG4gICAgICAgIEZvcm1hdDogdGhpcy5zb3BzRmlsZUZvcm1hdCxcbiAgICAgICAgU3RyaW5naWZpZWRWYWx1ZXM6IHRoaXMuc3RyaW5naWZpZWRWYWx1ZXMsXG4gICAgICB9LFxuICAgIH0pO1xuICAgIHRoaXMudmVyc2lvbklkID0gY3IuZ2V0QXR0U3RyaW5nKCdWZXJzaW9uSWQnKTtcbiAgfVxufVxuXG5leHBvcnQgY2xhc3MgU29wc1N5bmNQcm92aWRlciBleHRlbmRzIFNpbmdsZXRvbkZ1bmN0aW9uIGltcGxlbWVudHMgSUdyYW50YWJsZSB7XG4gIHByaXZhdGUgc29wc0FnZUtleXM6IFNlY3JldFZhbHVlW107XG5cbiAgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ/OiBzdHJpbmcpIHtcbiAgICBzdXBlcihzY29wZSwgaWQgPz8gJ1NvcHNTeW5jUHJvdmlkZXInLCB7XG4gICAgICBjb2RlOiBDb2RlLmZyb21Bc3NldChcbiAgICAgICAgc2NvcGUubm9kZS50cnlHZXRDb250ZXh0KCdzb3BzX3N5bmNfcHJvdmlkZXJfYXNzZXRfcGF0aCcpIHx8XG4gICAgICAgICAgcGF0aC5qb2luKF9fZGlybmFtZSwgJy4uL2Fzc2V0cy9jZGstc29wcy1sYW1iZGEuemlwJyksXG4gICAgICApLFxuICAgICAgcnVudGltZTogUnVudGltZS5QUk9WSURFRF9BTDIsXG4gICAgICBoYW5kbGVyOiAnYm9vdHN0cmFwJyxcbiAgICAgIHV1aWQ6ICdTb3BzU3luY1Byb3ZpZGVyJyxcbiAgICAgIHRpbWVvdXQ6IER1cmF0aW9uLnNlY29uZHMoNjApLFxuICAgICAgZW52aXJvbm1lbnQ6IHtcbiAgICAgICAgU09QU19BR0VfS0VZOiBMYXp5LnN0cmluZyh7XG4gICAgICAgICAgcHJvZHVjZTogKCkgPT5cbiAgICAgICAgICAgICh0aGlzLnNvcHNBZ2VLZXlzLm1hcCgoc2VjcmV0KSA9PiBzZWNyZXQudG9TdHJpbmcoKSkgPz8gW10pLmpvaW4oXG4gICAgICAgICAgICAgICdcXG4nLFxuICAgICAgICAgICAgKSxcbiAgICAgICAgfSksXG4gICAgICB9LFxuICAgIH0pO1xuICAgIHRoaXMuc29wc0FnZUtleXMgPSBbXTtcbiAgfVxuXG4gIHB1YmxpYyBhZGRBZ2VLZXkoa2V5OiBTZWNyZXRWYWx1ZSkge1xuICAgIHRoaXMuc29wc0FnZUtleXMucHVzaChrZXkpO1xuICB9XG59XG5cbi8qKlxuICogVGhlIGNvbmZpZ3VyYXRpb24gb3B0aW9ucyBvZiB0aGUgU29wc1NlY3JldFxuICovXG5leHBvcnQgaW50ZXJmYWNlIFNvcHNTZWNyZXRQcm9wcyBleHRlbmRzIFNlY3JldFByb3BzLCBTb3BzU3luY09wdGlvbnMge31cblxuLyoqXG4gKiBBIGRyb3AgaW4gcmVwbGFjZW1lbnQgZm9yIHRoZSBub3JtYWwgU2VjcmV0LCB0aGF0IGlzIHBvcHVsYXRlZCB3aXRoIHRoZSBlbmNyeXB0ZWRcbiAqIGNvbnRlbnQgb2YgdGhlIGdpdmVuIHNvcHMgZmlsZS5cbiAqL1xuZXhwb3J0IGNsYXNzIFNvcHNTZWNyZXQgZXh0ZW5kcyBDb25zdHJ1Y3QgaW1wbGVtZW50cyBJU2VjcmV0IHtcbiAgcHJpdmF0ZSByZWFkb25seSBzZWNyZXQ6IFNlY3JldDtcbiAgcmVhZG9ubHkgZW5jcnlwdGlvbktleT86IElLZXkgfCB1bmRlZmluZWQ7XG4gIHJlYWRvbmx5IHNlY3JldEFybjogc3RyaW5nO1xuICByZWFkb25seSBzZWNyZXRGdWxsQXJuPzogc3RyaW5nIHwgdW5kZWZpbmVkO1xuICByZWFkb25seSBzZWNyZXROYW1lOiBzdHJpbmc7XG4gIHJlYWRvbmx5IHN0YWNrOiBTdGFjaztcbiAgcmVhZG9ubHkgZW52OiBSZXNvdXJjZUVudmlyb25tZW50O1xuXG4gIHJlYWRvbmx5IHN5bmM6IFNvcHNTeW5jO1xuICBwdWJsaWMgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM6IFNvcHNTZWNyZXRQcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG4gICAgdGhpcy5zZWNyZXQgPSBuZXcgU2VjcmV0KHRoaXMsICdSZXNvdXJjZScsIHByb3BzIGFzIFNlY3JldFByb3BzKTtcblxuICAgIC8vIEZ1bGxmaWxsIHNlY3JldCBJbnRlcmZhY2VcbiAgICB0aGlzLmVuY3J5cHRpb25LZXkgPSB0aGlzLnNlY3JldC5lbmNyeXB0aW9uS2V5O1xuICAgIHRoaXMuc2VjcmV0QXJuID0gdGhpcy5zZWNyZXQuc2VjcmV0QXJuO1xuICAgIHRoaXMuc2VjcmV0TmFtZSA9IHRoaXMuc2VjcmV0LnNlY3JldE5hbWU7XG4gICAgdGhpcy5zdGFjayA9IFN0YWNrLm9mKHNjb3BlKTtcbiAgICB0aGlzLmVudiA9IHtcbiAgICAgIGFjY291bnQ6IHRoaXMuc3RhY2suYWNjb3VudCxcbiAgICAgIHJlZ2lvbjogdGhpcy5zdGFjay5yZWdpb24sXG4gICAgfTtcblxuICAgIHRoaXMuc3luYyA9IG5ldyBTb3BzU3luYyh0aGlzLCAnU29wc1N5bmMnLCB7XG4gICAgICBzZWNyZXQ6IHRoaXMuc2VjcmV0LFxuICAgICAgLi4uKHByb3BzIGFzIFNvcHNTeW5jT3B0aW9ucyksXG4gICAgfSk7XG4gIH1cblxuICAvKipcbiAgICogUmV0dXJucyB0aGUgY3VycmVudCB2ZXJzaW9uSWQgdGhhdCB3YXMgY3JlYXRlZCB2aWEgdGhlIFNvcHNTeW5jXG4gICAqL1xuICBwdWJsaWMgY3VycmVudFZlcnNpb25JZCgpOiBzdHJpbmcge1xuICAgIHJldHVybiB0aGlzLnN5bmMudmVyc2lvbklkO1xuICB9XG5cbiAgcHVibGljIGdyYW50UmVhZChncmFudGVlOiBJR3JhbnRhYmxlLCB2ZXJzaW9uU3RhZ2VzPzogc3RyaW5nW10pOiBHcmFudCB7XG4gICAgcmV0dXJuIHRoaXMuc2VjcmV0LmdyYW50UmVhZChncmFudGVlLCB2ZXJzaW9uU3RhZ2VzKTtcbiAgfVxuICBwdWJsaWMgZ3JhbnRXcml0ZShfZ3JhbnRlZTogSUdyYW50YWJsZSk6IEdyYW50IHtcbiAgICB0aHJvdyBuZXcgRXJyb3IoXG4gICAgICBgTWV0aG9kIGdyYW50V3JpdGUoLi4uKSBub3QgYWxsb3dlZCBhcyB0aGlzIHNlY3JldCBpcyBtYW5hZ2VkIGJ5IFNvcHNTeW5jYCxcbiAgICApO1xuICB9XG4gIHB1YmxpYyBhZGRSb3RhdGlvblNjaGVkdWxlKFxuICAgIGlkOiBzdHJpbmcsXG4gICAgb3B0aW9uczogUm90YXRpb25TY2hlZHVsZU9wdGlvbnMsXG4gICk6IFJvdGF0aW9uU2NoZWR1bGUge1xuICAgIHRocm93IG5ldyBFcnJvcihcbiAgICAgIGBNZXRob2QgYWRkVG90YXRpb25TY2hlZHVsZSgnJHtpZH0nLCAke0pTT04uc3RyaW5naWZ5KFxuICAgICAgICBvcHRpb25zLFxuICAgICAgKX0pIG5vdCBhbGxvd2VkIGFzIHRoaXMgc2VjcmV0IGlzIG1hbmFnZWQgYnkgU29wc1N5bmNgLFxuICAgICk7XG4gIH1cbiAgcHVibGljIGFkZFRvUmVzb3VyY2VQb2xpY3koXG4gICAgc3RhdGVtZW50OiBQb2xpY3lTdGF0ZW1lbnQsXG4gICk6IEFkZFRvUmVzb3VyY2VQb2xpY3lSZXN1bHQge1xuICAgIHJldHVybiB0aGlzLnNlY3JldC5hZGRUb1Jlc291cmNlUG9saWN5KHN0YXRlbWVudCk7XG4gIH1cbiAgcHVibGljIGRlbnlBY2NvdW50Um9vdERlbGV0ZSgpOiB2b2lkIHtcbiAgICByZXR1cm4gdGhpcy5zZWNyZXQuZGVueUFjY291bnRSb290RGVsZXRlKCk7XG4gIH1cbiAgcHVibGljIGF0dGFjaCh0YXJnZXQ6IElTZWNyZXRBdHRhY2htZW50VGFyZ2V0KTogSVNlY3JldCB7XG4gICAgcmV0dXJuIHRoaXMuc2VjcmV0LmF0dGFjaCh0YXJnZXQpO1xuICB9XG4gIHB1YmxpYyBhcHBseVJlbW92YWxQb2xpY3kocG9saWN5OiBSZW1vdmFsUG9saWN5KTogdm9pZCB7XG4gICAgcmV0dXJuIHRoaXMuc2VjcmV0LmFwcGx5UmVtb3ZhbFBvbGljeShwb2xpY3kpO1xuICB9XG5cbiAgcHVibGljIHNlY3JldFZhbHVlRnJvbUpzb24oanNvbkZpZWxkOiBzdHJpbmcpIHtcbiAgICByZXR1cm4gU2VjcmV0VmFsdWUuc2VjcmV0c01hbmFnZXIodGhpcy5zZWNyZXRBcm4sIHtcbiAgICAgIGpzb25GaWVsZCxcbiAgICAgIHZlcnNpb25JZDogdGhpcy5zeW5jLnZlcnNpb25JZCxcbiAgICB9KTtcbiAgfVxuXG4gIHB1YmxpYyBnZXQgc2VjcmV0VmFsdWUoKTogU2VjcmV0VmFsdWUge1xuICAgIHJldHVybiB0aGlzLnNlY3JldFZhbHVlRnJvbUpzb24oJycpO1xuICB9XG59XG4iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9711111111111111%*

 * *Differences: {"'devDependencies'": "{'jsii-diff': '^1.98.0', 'jsii-pacmak': '^1.98.0'}", "'version'": "'1.7.2'"}*

```diff
@@ -18,17 +18,17 @@
         "eslint-config-prettier": "^8.10.0",
         "eslint-import-resolver-typescript": "^2.7.1",
         "eslint-plugin-import": "^2.29.1",
         "eslint-plugin-prettier": "^4.2.1",
         "jest": "^27",
         "jest-junit": "^15",
         "jsii": "1.x",
-        "jsii-diff": "^1.97.0",
+        "jsii-diff": "^1.98.0",
         "jsii-docgen": "^6.3.27",
-        "jsii-pacmak": "^1.97.0",
+        "jsii-pacmak": "^1.98.0",
         "jsii-rosetta": "1.x",
         "prettier": "^2.8.8",
         "projen": "^0.81.5",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.2",
         "typescript": "^4.9.5"
@@ -152,9 +152,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "1.7.1"
+    "version": "1.7.2"
 }
```

### Comparing `cdk-sops-secrets-1.7.1/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.7.2/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.7.1
+Version: 1.7.2
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

