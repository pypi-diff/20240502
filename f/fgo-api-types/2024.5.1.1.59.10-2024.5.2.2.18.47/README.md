# Comparing `tmp/fgo_api_types-2024.5.1.1.59.10.tar.gz` & `tmp/fgo_api_types-2024.5.2.2.18.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2024.5.1.1.59.10.tar", max compression
+gzip compressed data, was "fgo_api_types-2024.5.2.2.18.47.tar", max compression
```

## Comparing `fgo_api_types-2024.5.1.1.59.10.tar` & `fgo_api_types-2024.5.2.2.18.47.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-05-01 01:58:54.818128 fgo_api_types-2024.5.1.1.59.10/LICENSE
--rw-r--r--   0        0        0      449 2024-05-01 01:58:54.818128 fgo_api_types-2024.5.1.1.59.10/README.md
--rw-r--r--   0        0        0        0 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/base.py
--rw-r--r--   0        0        0     4511 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3843 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/common.py
--rw-r--r--   0        0        0    41932 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/enums.py
--rw-r--r--   0        0        0   183237 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    86719 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/nice.py
--rw-r--r--   0        0        0    59461 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4518 2024-05-01 01:59:10.454170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19445 2024-05-01 01:59:10.458170 fgo_api_types-2024.5.1.1.59.10/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2024-05-01 01:59:10.774171 fgo_api_types-2024.5.1.1.59.10/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fgo_api_types-2024.5.1.1.59.10/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-02 02:18:30.563126 fgo_api_types-2024.5.2.2.18.47/LICENSE
+-rw-r--r--   0        0        0      449 2024-05-02 02:18:30.563126 fgo_api_types-2024.5.2.2.18.47/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4511 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3843 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/common.py
+-rw-r--r--   0        0        0    41947 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   183237 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    86981 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    59573 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4518 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19445 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2024-05-02 02:18:47.667302 fgo_api_types-2024.5.2.2.18.47/pyproject.toml
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fgo_api_types-2024.5.2.2.18.47/PKG-INFO
```

### Comparing `fgo_api_types-2024.5.1.1.59.10/LICENSE` & `fgo_api_types-2024.5.2.2.18.47/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/basic.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/common.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/enums.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1012,16 +1012,16 @@
     magicBullet = "magicBullet"
     protagonistCorrection = "protagonistCorrection"
     normalAokoBuff = "normalAokoBuff"
     magicBulletAtkBuff = "magicBulletAtkBuff"
     demeritFunction = "demeritFunction"
     extraBuff = "extraBuff"
     robinCounter = "robinCounter"
-    kuonjiAliceFormA = "kuonjiAliceFormA"
-    kuonjiAliceFormB = "kuonjiAliceFormB"
+    kuonjiAliceHasSkill3 = "kuonjiAliceHasSkill3"
+    kuonjiAliceStage3 = "kuonjiAliceStage3"
     instantDeathFunction = "instantDeathFunction"
     forceInstantDeathFunction = "forceInstantDeathFunction"
     buffGutsOnInstantDeath = "buffGutsOnInstantDeath"
     robinAllGone = "robinAllGone"
 
 
 TRAIT_NAME: dict[int, Trait] = {
@@ -1216,18 +1216,18 @@
     2881: Trait.groupServant,
     2883: Trait.FSNServant,
     2884: Trait.fieldDarkness,
     2885: Trait.magicBullet,
     2886: Trait.robinCounter,
     2887: Trait.robinAllGone,
     2888: Trait.protagonistCorrection,
-    2903: Trait.kuonjiAliceFormB,
+    2903: Trait.kuonjiAliceStage3,
     2911: Trait.normalAokoBuff,
     2912: Trait.magicBulletAtkBuff,
-    2913: Trait.kuonjiAliceFormA,
+    2913: Trait.kuonjiAliceHasSkill3,
     2914: Trait.buffGutsOnInstantDeath,
     # 2xxx: CQ or Story quests buff
     3000: Trait.attackPhysical,  # Normal attack, including NP
     3001: Trait.attackProjectile,
     3002: Trait.attackMagical,
     3004: Trait.buffPositiveEffect,
     3005: Trait.buffNegativeEffect,  # mutually exclusive with 3004
```

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/gameenums.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/nice.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2228,14 +2228,24 @@
 
 
 class NiceQuestPhaseScript(BaseModelORJson):
     phase: int
     scripts: list[ScriptLink]
 
 
+class NiceQuestPhasePresent(BaseModelORJson):
+    phase: int
+    gifts: list[NiceGift]
+    giftIcon: HttpUrl | None = None
+    condType: NiceCondType
+    condId: int
+    condNum: int
+    originalScript: dict[str, Any]
+
+
 class NiceQuest(BaseModelORJson):
     id: int
     name: str
     originalName: str
     type: NiceQuestType
     flags: list[NiceQuestFlag]
     consumeType: NiceConsumeType
@@ -2250,14 +2260,15 @@
     chapterId: int
     chapterSubId: int
     chapterSubStr: str
     giftIcon: HttpUrl | None = None
     gifts: list[NiceGift]
     releaseConditions: list[NiceQuestRelease]
     releaseOverwrites: list[NiceQuestReleaseOverwrite]
+    presents: list[NiceQuestPhasePresent]
     phases: list[int]
     phasesWithEnemies: list[int] = Field(
         [],
         title="List of phases with enemies data from Rayshift",
         description="List of phases with enemies data from Rayshift.",
     )
     phasesNoBattle: list[int] = Field(
```

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/raw.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1164,14 +1164,15 @@
     rewardType: int
     giftId: int
     bannerGroup: int
     priority: int
     rewardRarity: int
     notfyPriority: int
     presentMessageId: int
+    giftIconId: int | None = None
 
 
 class MstEventMissionCondition(BaseModelORJson):
     missionId: int
     missionProgressType: int
     priority: int
     id: int
@@ -1941,14 +1942,15 @@
     flag: int
 
 
 class MstQuestPhasePresent(BaseModelORJson):
     questId: int
     phase: int
     giftId: int
+    giftIconId: int
     presentMessageId: int
     condType: int
     condId: int
     condNum: int
     script: dict[str, Any]
 
 
@@ -2209,14 +2211,15 @@
     mstQuest: MstQuest
     mstQuestConsumeItem: list[MstQuestConsumeItem]
     mstQuestRelease: list[MstQuestRelease]
     mstQuestReleaseOverwrite: list[MstQuestReleaseOverwrite]
     mstClosedMessage: list[MstClosedMessage]
     mstGift: list[MstGift]
     mstGiftAdd: list[MstGiftAdd]
+    mstQuestPhasePresent: list[MstQuestPhasePresent] = []
     mstItem: list[MstItem] = []
     phases: list[int]
     phasesWithEnemies: list[int] = []
     phasesNoBattle: list[int] = []
     allScripts: list[ScriptFile]
```

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/rayshift.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.1.1.59.10/fgo_api_types/search.py` & `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.1.1.59.10/pyproject.toml` & `fgo_api_types-2024.5.2.2.18.47/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2024.05.01.01.59.10"
+version = "2024.05.02.02.18.47"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2024.5.1.1.59.10/PKG-INFO` & `fgo_api_types-2024.5.2.2.18.47/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2024.5.1.1.59.10
+Version: 2024.5.2.2.18.47
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

