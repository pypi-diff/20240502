# Comparing `tmp/dynamicroutingtask-0.1.98.tar.gz` & `tmp/dynamicroutingtask-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicroutingtask-0.1.98.tar", last modified: Mon Apr 22 20:22:31 2024, max compression
+gzip compressed data, was "dynamicroutingtask-0.1.99.tar", last modified: Sat Apr 27 00:29:26 2024, max compression
```

## Comparing `dynamicroutingtask-0.1.98.tar` & `dynamicroutingtask-0.1.99.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:31.457668 dynamicroutingtask-0.1.98/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:31.453668 dynamicroutingtask-0.1.98/Analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    34706 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/DynamicRoutingAnalysisUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    64785 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/RLmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/RLmodelHPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/RLmodelSlurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/RLmodel_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/behaviorClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/dr_analysis_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)   111619 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/dr_behav_figs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/dr_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/glm_hmm_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/ncb_meeting_01272023.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/npc_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/npc_analysis_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/presentation_June2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/regressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/sac_may2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/sessionSummaryFigs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/sound_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/sound_sync_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/Analysis/variableBlockDur.py
--rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/DynamicRouting1.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/DynamicRouting1_postSessionAnalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:31.457668 dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 20:22:31.000000 dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-22 20:22:31.000000 dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:22:31.000000 dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 20:22:31.000000 dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 20:22:31.000000 dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:31.453668 dynamicroutingtask-0.1.98/OptoGui/
--rw-r--r--   0 runner    (1001) docker     (127)    34134 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/OptoGui/OptoGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/OptoTagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 20:22:31.457668 dynamicroutingtask-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/RFMapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:31.453668 dynamicroutingtask-0.1.98/SamStimGui/
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/SamStimGui/SamStimGui.py
--rw-r--r--   0 runner    (1001) docker     (127)    62595 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/TaskControl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/TaskUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/camstimControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 20:22:28.000000 dynamicroutingtask-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/runTask.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 20:22:31.457668 dynamicroutingtask-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-22 20:22:02.000000 dynamicroutingtask-0.1.98/startTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:29:26.570706 dynamicroutingtask-0.1.99/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:29:26.566706 dynamicroutingtask-0.1.99/Analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    34726 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/DynamicRoutingAnalysisUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66366 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/RLmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/RLmodelHPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/RLmodelSlurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/RLmodel_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/behaviorClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/dr_analysis_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111912 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/dr_behav_figs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/dr_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/glm_hmm_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/ncb_meeting_01272023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/npc_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/npc_analysis_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/presentation_June2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/regressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/sac_may2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/sessionSummaryFigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/sound_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/sound_sync_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/Analysis/variableBlockDur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/DynamicRouting1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/DynamicRouting1_postSessionAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:29:26.570706 dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-27 00:29:26.000000 dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-27 00:29:26.000000 dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:29:26.000000 dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:29:26.000000 dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 00:29:26.000000 dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:29:26.566706 dynamicroutingtask-0.1.99/OptoGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    34134 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/OptoGui/OptoGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/OptoTagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-27 00:29:26.570706 dynamicroutingtask-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/RFMapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:29:26.570706 dynamicroutingtask-0.1.99/SamStimGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/SamStimGui/SamStimGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62590 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/TaskControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/TaskUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/camstimControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-27 00:29:23.000000 dynamicroutingtask-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/runTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:29:26.570706 dynamicroutingtask-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-27 00:28:55.000000 dynamicroutingtask-0.1.99/startTask.py
```

### Comparing `dynamicroutingtask-0.1.98/Analysis/DynamicRoutingAnalysisUtils.py` & `dynamicroutingtask-0.1.99/Analysis/DynamicRoutingAnalysisUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
                                 nextTask = 'stage 4 ori tone ori'
                             else:
                                 nextTask = 'stage 4 ori tone' if 'stage 4 tone' in task else 'stage 4 tone ori'
                         elif 'stage 5' in task:
                             if 'stage 5' in prevTask and np.all(np.sum((np.array(dprimeSame) >= dprimeThresh) & (np.array(dprimeOther) >= dprimeThresh),axis=1) > 3):
                                 passStage = 1
                                 handOff = True
-                            if 'stage 5' in prevTask and 'repeats' not in prevTask:
+                            if regimen==8 and 'stage 5' in prevTask and 'repeats' not in prevTask:
                                 handOff = True
                             if 'AMN' in task:
                                 nextTask = 'stage 5 AMN ori' if 'stage 5 ori' in task else 'stage 5 ori AMN'
                             else:
                                 nextTask = 'stage 5 tone ori' if 'stage 5 ori' in task else 'stage 5 ori tone'
                         elif 'stage variable' in task:
                             if not np.any(np.isnan(obj.dprimeOtherModalGo)):
@@ -500,15 +500,15 @@
             continue
         mouseId = str(mouseId)
         mouseDir = allMiceDf.loc[mouseInd,'data path']
         behavFiles = glob.glob(os.path.join(mouseDir,'**','DynamicRouting*.hdf5'))
         behavFiles += glob.glob(os.path.join(baseDir,'Data',mouseId,'DynamicRouting*.hdf5'))
         df = sheets[mouseId] if mouseId in sheets else None
         exps = []
-        for f in behavFiles:
+        for f in set(behavFiles):
             startTime = re.search('.*_([0-9]{8}_[0-9]{6})',f).group(1)
             startTime = pd.to_datetime(startTime,format='%Y%m%d_%H%M%S')
             if df is None or np.sum(df['start time']==startTime) < 1:
                 try:
                     obj = DynRoutData()
                     obj.loadBehavData(f)
                     exps.append(obj)
```

### Comparing `dynamicroutingtask-0.1.98/Analysis/RLmodel.py` & `dynamicroutingtask-0.1.99/Analysis/RLmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @author: samgale
 """
 
 import copy
 import glob
 import os
 import numpy as np
+import scipy.stats
 import matplotlib
 import matplotlib.pyplot as plt
 matplotlib.rcParams['pdf.fonttype'] = 42
 import sklearn.metrics
 from DynamicRoutingAnalysisUtils import getSessionData, calcDprime
 from RLmodelHPC import calcLogisticProb, runModel
 
@@ -236,32 +237,76 @@
                     s['qStim'] = []
                     s['wHabit'] = []
                     s['wReward'] = []
                     s['expectedValue'] = []
                     s['qTotal'] = []
                     s['prediction'] = []
                     s['logLossTest'] = []
-                    s['simulation'] = []
-                    s['logLossSimulation'] = []
                     for i,params in enumerate(s['params']):
                         pContext,qContext,qStim,wHabit,wReward,expectedValue,qTotal,pAction,action = [val[0] for val in runModel(obj,*params,**modelTypeParams[modelType])]
                         s['pContext'].append(pContext)
                         s['qContext'].append(qContext)
                         s['qStim'].append(qStim)
                         s['wHabit'].append(wHabit)
                         s['wReward'].append(wReward)
                         s['expectedValue'].append(expectedValue)
                         s['qTotal'].append(qTotal)
                         s['prediction'].append(pAction)
                         s['logLossTest'].append(sklearn.metrics.log_loss(obj.trialResponse,pAction))
-                        pSimulate = np.mean(runModel(obj,*params,useHistory=True,nReps=100,**modelTypeParams[modelType])[-2],axis=0)
-                        s['simulation'].append(pSimulate)
-                        s['logLossSimulation'].append(sklearn.metrics.log_loss(obj.trialResponse,pSimulate))
-
                         
+
+# model simulation
+for trainingPhase in trainingPhases:
+    print(trainingPhase)
+    d = modelData[trainingPhase]
+    for mouse in d:
+        for session in d[mouse]:
+            obj = sessionData[trainingPhase][mouse][session]
+            for modelType in modelTypes:
+                s = d[mouse][session][modelType]
+                params = s['params'][0]
+                pSimulate = np.mean(runModel(obj,*params,useHistory=False,nReps=100,**modelTypeParams[modelType])[-2],axis=0)
+                s['simulation'] = pSimulate
+                s['logLossSimulation'] = sklearn.metrics.log_loss(obj.trialResponse,pSimulate)
+             
+for trainingPhase in trainingPhases:
+    d = modelData[trainingPhase]
+    for modelType in modelTypes:
+        fig = plt.figure()
+        ax = fig.add_subplot(1,1,1)
+        pred = []
+        sim = []
+        for mouse in d:
+            for session in d[mouse]: 
+                s = d[mouse][session][modelType]
+                pred.append(s['logLossTest'][0])
+                sim.append(s['logLossSimulation'])
+        ax.plot(pred,sim,'o',mec='k',mfc=None,alpha=0.25)
+        ax.set_xlim([0,1.5])
+        ax.set_ylim([0,1.5])
+        ax.set_aspect('equal')
+        ax.set_xlabel('log loss of model prediction')
+        ax.set_ylabel('log loss of model simulation')
+        slope,yint,rval,pval,stderr = scipy.stats.linregress(pred,sim)
+        ax.set_title(trainingPhase+', '+modelType+'\nr = '+str(round(rval,2)))
+ 
+for trainingPhase in trainingPhases:
+    d = modelData[trainingPhase]
+    for modelType in modelTypes:
+        r = []  
+        for mouse in d:
+            for session in d[mouse]: 
+                s = d[mouse][session][modelType]
+                pred = s['prediction'][0]
+                sim = s['simulation']
+                slope,yint,rval,pval,stderr = scipy.stats.linregress(pred,sim)
+                r.append(rval**2)
+        print(trainingPhase,modelType,round(np.median(r),2))
+        
+
 # get performance data
 performanceData = {trainingPhase: {modelType: {} for modelType in modelTypes} for trainingPhase in trainingPhases}
 for trainingPhase in trainingPhases:
     for modelType in modelTypes:
         for fixedParam in ('mice',) + fixedParamNames[modelType]:
             performanceData[trainingPhase][modelType][fixedParam] = {'respFirst': [],'respLast': [],'dprime': []}
             if fixedParam == 'mice':
```

### Comparing `dynamicroutingtask-0.1.98/Analysis/RLmodelHPC.py` & `dynamicroutingtask-0.1.99/Analysis/RLmodelHPC.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/RLmodelSlurm.py` & `dynamicroutingtask-0.1.99/Analysis/RLmodelSlurm.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/RLmodel_old.py` & `dynamicroutingtask-0.1.99/Analysis/RLmodel_old.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/behaviorClustering.py` & `dynamicroutingtask-0.1.99/Analysis/behaviorClustering.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/dr_analysis_sam.py` & `dynamicroutingtask-0.1.99/Analysis/dr_analysis_sam.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/dr_behav_figs.py` & `dynamicroutingtask-0.1.99/Analysis/dr_behav_figs.py`

 * *Files 1% similar despite different names*

```diff
@@ -884,22 +884,22 @@
             ax.legend(bbox_to_anchor=(1,1),loc='upper left',fontsize=12)
             ax.set_title('previous trial '+prevTrialType+'\n'+blockLabel)
         plt.tight_layout()
 
 
 # time dependence of effect of prior reward or response
 stimType = ('rewarded target','non-rewarded target','non-target (rewarded modality)','non-target (unrewarded modality)')
-prevTrialTypes = ('response to rewarded target','response to non-rewarded target','response to either target','response to either non-target')
+prevTrialTypes = ('response','response to rewarded target','response to non-rewarded target','response to either target')
 resp = {s: [] for s in stimType}
 trialsSince = {prevTrial: {s: [] for s in stimType} for prevTrial in prevTrialTypes}
 timeSince = copy.deepcopy(trialsSince)
 for obj in [obj for exps,s in zip(sessionData,sessionsToPass) for obj in exps[s:]]:
     for blockInd,rewStim in enumerate(obj.blockStimRewarded):
-        # if obj.hitRate[blockInd] < 0.9:
-        #     continue
+        if obj.hitRate[blockInd] < 0.85:
+            continue
         otherModalTarget = np.setdiff1d(obj.blockStimRewarded,rewStim)[0]
         blockTrials = (obj.trialBlock==blockInd+1) & ~obj.catchTrials
         rewTrials = np.where(blockTrials & obj.trialRewarded)[0]
         nonRewTargetTrials = np.where(blockTrials & obj.trialResponse & ~obj.trialRewarded & (obj.trialStim==otherModalTarget))[0]
         targetRespTrials = np.where(blockTrials & obj.trialResponse & np.in1d(obj.trialStim,(rewStim,otherModalTarget)))[0]
         respTrials = np.where(blockTrials & obj.trialResponse)[0]
         for s in stimType:
@@ -908,120 +908,129 @@
             elif s=='non-rewarded target':
                 stim = otherModalTarget
             elif s=='non-target (rewarded modality)':
                 stim = rewStim[:-1]+'2'
             else:
                 stim = otherModalTarget[:-1]+'2'
             stimTrials = np.where(blockTrials & (obj.trialStim==stim))[0]
-            for prevTrialType,trials in zip(prevTrialTypes,(rewTrials,nonRewTargetTrials,targetRespTrials,respTrials)):
+            for prevTrialType,trials in zip(prevTrialTypes,(respTrials,rewTrials,nonRewTargetTrials,targetRespTrials)):
                 if len(trials) > 0:
                     prevTrial = trials[np.searchsorted(trials,stimTrials) - 1]
-                    trialsSince[prevTrialType][s].extend(stimTrials - prevTrial)
-                    timeSince[prevTrialType][s].extend(obj.stimStartTimes[stimTrials] - obj.stimStartTimes[prevTrial])
+                    notValid = stimTrials <= trials[0]
+                    tr = stimTrials - prevTrial
+                    tr[notValid] = -1
+                    tm = obj.stimStartTimes[stimTrials] - obj.stimStartTimes[prevTrial]
+                    tm[notValid] = np.nan
+                    trialsSince[prevTrialType][s].extend(tr)
+                    timeSince[prevTrialType][s].extend(tm)
                 else:
                     trialsSince[prevTrialType][s].extend(np.full(len(stimTrials),np.nan))
                     timeSince[prevTrialType][s].extend(np.full(len(stimTrials),np.nan))
             resp[s].extend(obj.trialResponse[stimTrials])
 
 for i,prevTrialType in enumerate(prevTrialTypes):
     for s in stimType:
         trialsSince[prevTrialType][s] = np.array(trialsSince[prevTrialType][s])
         timeSince[prevTrialType][s] = np.array(timeSince[prevTrialType][s])
         if i==0:
             resp[s] = np.array(resp[s])
 
-x = np.arange(20)
+correctRespRate = False
+r = {}
+trialBins = np.arange(20)
 for prevTrialType in prevTrialTypes:
     fig = plt.figure(figsize=(8,4.5))
     ax = fig.add_subplot(1,1,1)
     for s,clr,ls in zip(stimType,'gmgm',('-','-','--','--')):
-        n = np.zeros(x.size)
-        p = np.zeros(x.size)
-        ci = np.zeros((x.size,2))
-        for i in x:
+        n = np.zeros(trialBins.size)
+        p = np.zeros(trialBins.size)
+        for i in trialBins:
             if i>0:
                 j = trialsSince[prevTrialType][s]==i
                 n[i] += j.sum()
                 p[i] += resp[s][j].sum()
         p /= n
-        ci = np.array([[b/n[i] for b in scipy.stats.binom.interval(0.95,n[i],p[i])] for i in x])
-        ax.plot(x,p,color=clr,ls=ls,label=s)
-        ax.fill_between(x,ci[:,0],ci[:,1],color=clr,alpha=0.25)
+        if correctRespRate:
+            if prevTrialType == 'response':
+                r[s] = p
+            else:
+                p -= r[s]
+        ci = np.array([[b/n[i] for b in scipy.stats.binom.interval(0.95,n[i],p[i])] for i in trialBins])
+        ax.plot(trialBins,p,color=clr,ls=ls,label=s)
+        ax.fill_between(trialBins,ci[:,0],ci[:,1],color=clr,alpha=0.25)
     for side in ('right','top'):
         ax.spines[side].set_visible(False)
     ax.tick_params(direction='out',top=False,right=False)
     ax.set_xlim([0,12])
-    ax.set_ylim([0,1.01])
+    # ax.set_ylim([0,1.01])
     ax.set_xlabel('Trials since last '+prevTrialType)
     ax.set_ylabel('Response rate')
     ax.legend(bbox_to_anchor=(1,1),loc='upper left')
     plt.tight_layout()
 
 y = {prevTrial: {} for prevTrial in prevTrialTypes}
 binWidth = 5
-x = np.arange(0,120,binWidth)
+timeBins = np.arange(0,120,binWidth)
 for prevTrialType in prevTrialTypes:    
     fig = plt.figure(figsize=(8,4.5))
     ax = fig.add_subplot(1,1,1)
     for s,clr,ls in zip(stimType,'gmgm',('-','-','--','--')):
-        n = np.zeros(x.size)
-        p = np.zeros(x.size)
-        ci = np.zeros((x.size,2))
-        for i,t in enumerate(x):
+        n = np.zeros(timeBins.size)
+        p = np.zeros(timeBins.size)
+        for i,t in enumerate(timeBins):
             j = (timeSince[prevTrialType][s] > t) & (timeSince[prevTrialType][s] < t+5)
             n[i] += j.sum()
             p[i] += resp[s][j].sum()
         p /= n
-        ci = np.array([[b/n[i] for b in scipy.stats.binom.interval(0.95,n[i],p[i])] for i in range(x.size)])
-        ax.plot(x+binWidth/2,p,color=clr,ls=ls,label=s)
-        ax.fill_between(x+binWidth/2,ci[:,0],ci[:,1],color=clr,alpha=0.25)
+        if correctRespRate:
+            if prevTrialType == 'response':
+                r[s] = p
+            else:
+                p -= r[s]
+        ci = np.array([[b/n[i] for b in scipy.stats.binom.interval(0.95,n[i],p[i])] for i in range(timeBins.size)])
+        ax.plot(timeBins+binWidth/2,p,color=clr,ls=ls,label=s)
+        ax.fill_between(timeBins+binWidth/2,ci[:,0],ci[:,1],color=clr,alpha=0.25)
         y[prevTrialType][s] = p
     for side in ('right','top'):
         ax.spines[side].set_visible(False)
     ax.tick_params(direction='out',top=False,right=False)
-    ax.set_xlim([0,92.5])
-    ax.set_ylim([0,1.01])
+    # ax.set_xlim([0,87.5])
+    # ax.set_ylim([0,1.01])
     ax.set_xlabel('Time since last '+prevTrialType+' (s)')
     ax.set_ylabel('Response rate')
     ax.legend(bbox_to_anchor=(1,1),loc='upper left')
     plt.tight_layout()
     
 fig = plt.figure()
 ax = fig.add_subplot(1,1,1)
-t = x+binWidth/2
-tend = np.where(t==92.5)[0][0] + 1
-func = lambda t,tau,a,b: 1 - a * -np.exp(t/tau) + b
+t = timeBins + binWidth/2
+func = lambda t,tau,a,b: 1 - a * np.exp(-t/tau) + b
 p = y['response to rewarded target']['non-rewarded target']
-tau,a,b = scipy.optimize.curve_fit(func,t[2:tend],p[2:tend],p0=(t[tend],p[2],p[-1]-p[2]))[0]
+tau,a,b = scipy.optimize.curve_fit(func,t[2:],p[2:],p0=(t[-1],p[-1]-p[2],p[2]))[0]
 ax.plot(t,p,'m',lw=2,label='non-rewarded target')
-ax.plot(t[2:tend],func(t[2:tend],tau,a,b),'k--',label='expontential fit (tau = '+str(np.round(tau,1))+' s)')
+ax.plot(t[2:],func(t[2:],tau,a,b),'k--',label='expontential fit (tau = '+str(np.round(tau,1))+' s)')
 for side in ('right','top'):
     ax.spines[side].set_visible(False)
 ax.tick_params(direction='out',top=False,right=False)
-ax.set_xlim([0,92.5])
-ax.set_ylim([0.35,0.6])
+# ax.set_xlim([0,92.5])
+# ax.set_ylim([0.35,0.6])
 ax.set_xlabel('Time since last response to rewarded target (s)')
 ax.set_ylabel('Response rate')
 ax.legend(loc='upper left')
 plt.tight_layout()
 
-tSort = np.sort(np.concatenate([timeSince['response to rewarded target'][s] for s in stimType]))
-cumProb = [np.sum(tSort<=i)/tSort.size for i in tSort]
-
-fig = plt.figure()
-ax = fig.add_subplot(1,1,1)
-ax.plot(tSort,cumProb,'k')
-for side in ('right','top'):
-    ax.spines[side].set_visible(False)
-ax.tick_params(direction='out',top=False,right=False)
-ax.set_xlim([0,92.5])
-ax.set_ylim([0,1.01])
-ax.set_xlabel('Time since last response to rewarded target (s)')
-ax.set_ylabel('Cumulative probability')
-plt.tight_layout()
+for s in stimType:
+    fig = plt.figure()
+    ax = fig.add_subplot(1,1,1)
+    ax.hist(timeSince['response to rewarded target'][s],bins=timeBins)
+    ax.set_yscale('log')
+    for side in ('right','top'):
+        ax.spines[side].set_visible(False)
+    ax.tick_params(direction='out',top=False,right=False)
+    plt.tight_layout()
 
 
 # performance by block number
 fig = plt.figure()
 ax = fig.add_subplot(1,1,1)
 x = np.arange(6)+1
 for rewardStim,clr,blockLbl in zip(('vis1','sound1'),'gm',('visual rewarded','auditory rewarded')):
```

### Comparing `dynamicroutingtask-0.1.98/Analysis/dr_ephys_analysis.py` & `dynamicroutingtask-0.1.99/Analysis/dr_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/glm_hmm_sam.py` & `dynamicroutingtask-0.1.99/Analysis/glm_hmm_sam.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/ncb_meeting_01272023.py` & `dynamicroutingtask-0.1.99/Analysis/ncb_meeting_01272023.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/npc_analysis.py` & `dynamicroutingtask-0.1.99/Analysis/npc_analysis.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/npc_analysis_2.py` & `dynamicroutingtask-0.1.99/Analysis/npc_analysis_2.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/presentation_June2023.py` & `dynamicroutingtask-0.1.99/Analysis/presentation_June2023.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/regressionModel.py` & `dynamicroutingtask-0.1.99/Analysis/regressionModel.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/sac_may2023.py` & `dynamicroutingtask-0.1.99/Analysis/sac_may2023.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/sessionSummaryFigs.py` & `dynamicroutingtask-0.1.99/Analysis/sessionSummaryFigs.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/sound_ephys_analysis.py` & `dynamicroutingtask-0.1.99/Analysis/sound_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/sound_sync_test.py` & `dynamicroutingtask-0.1.99/Analysis/sound_sync_test.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/Analysis/variableBlockDur.py` & `dynamicroutingtask-0.1.99/Analysis/variableBlockDur.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/DynamicRouting1.py` & `dynamicroutingtask-0.1.99/DynamicRouting1.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/DynamicRouting1_postSessionAnalysis.py` & `dynamicroutingtask-0.1.99/DynamicRouting1_postSessionAnalysis.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/DynamicRoutingTask.egg-info/SOURCES.txt` & `dynamicroutingtask-0.1.99/DynamicRoutingTask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/OptoGui/OptoGui.py` & `dynamicroutingtask-0.1.99/OptoGui/OptoGui.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/OptoTagging.py` & `dynamicroutingtask-0.1.99/OptoTagging.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/RFMapping.py` & `dynamicroutingtask-0.1.99/RFMapping.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/SamStimGui/SamStimGui.py` & `dynamicroutingtask-0.1.99/SamStimGui/SamStimGui.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/TaskControl.py` & `dynamicroutingtask-0.1.99/TaskControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,16 @@
                         self.solenoidOpenTime = 0.03
                         self.networkNidaqDevices = ['zcDAQ9185-213AB43']
                         self.soundMode = 'daq'
                         self.soundNidaqDevice = 'zcDAQ1Mod1'
                         self.soundChannel = (0,1)
                         self.soundCalibrationFit = (26.532002859656085,-2.820908344083334,52.33566140075705)
                         self.optoNidaqDevice = 'zcDAQ9185-213AB43Mod4'
-                        self.galvoChannels = (0,1,np.nan)
-                        self.optoChannels = {'laser_488': (2,3), 'laser_633': (4,5)}
+                        self.galvoChannels = (0,1,2)
+                        self.optoChannels = {'laser_488': (3,4), 'laser_633': (5,6)}
                 elif self.rigName in ('B1','B2','B3','B4','B5','B6'):
                     self.behavNidaqDevice = 'Dev1'
                     self.rewardLine = (0,7)
                     self.rewardSoundLine = None
                     self.lickLine = (0,0)
                     if self.rigName == 'B1':
                         self.rotaryEncoderSerialPort = 'COM3'
```

### Comparing `dynamicroutingtask-0.1.98/TaskUtils.py` & `dynamicroutingtask-0.1.99/TaskUtils.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/camstimControl.py` & `dynamicroutingtask-0.1.99/camstimControl.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/pyproject.toml` & `dynamicroutingtask-0.1.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DynamicRoutingTask"
-version = "0.1.98"
+version = "0.1.99"
 dependencies = [
     "h5py",
     "numpy",
     "pandas",
     "scipy",
     "matplotlib",
 ]
```

### Comparing `dynamicroutingtask-0.1.98/runTask.py` & `dynamicroutingtask-0.1.99/runTask.py`

 * *Files identical despite different names*

### Comparing `dynamicroutingtask-0.1.98/startTask.py` & `dynamicroutingtask-0.1.99/startTask.py`

 * *Files identical despite different names*

