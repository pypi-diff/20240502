# Comparing `tmp/autocbei-1.7.tar.gz` & `tmp/autocbei-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocbei-1.7.tar", last modified: Fri Jan 28 23:27:16 2022, max compression
+gzip compressed data, was "autocbei-1.8.tar", last modified: Thu May  2 11:25:49 2024, max compression
```

## Comparing `autocbei-1.7.tar` & `autocbei-1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 atlas     (1000) atlas     (1000)        0 2022-01-28 23:27:16.545737 autocbei-1.7/
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)    11340 2021-12-14 00:14:11.000000 autocbei-1.7/LICENSE
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)      548 2022-01-28 23:27:16.542737 autocbei-1.7/PKG-INFO
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)    10082 2022-01-28 23:18:15.000000 autocbei-1.7/README.md
-drwxrwxrwx   0 atlas     (1000) atlas     (1000)        0 2022-01-28 23:27:16.344118 autocbei-1.7/autocbei/
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)   519648 2021-12-14 00:14:11.000000 autocbei-1.7/autocbei/Bacillus_subtilis.part500.cds.all.fa
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)      463 2021-12-14 00:14:11.000000 autocbei-1.7/autocbei/__init__.py
-drwxrwxrwx   0 atlas     (1000) atlas     (1000)        0 2022-01-28 23:27:16.526604 autocbei-1.7/autocbei/cbei/
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)        0 2021-12-14 00:14:11.000000 autocbei-1.7/autocbei/cbei/__init__.py
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)     4298 2022-01-28 23:08:30.000000 autocbei-1.7/autocbei/cbei/autoCBEI.py
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)     9471 2021-12-14 00:14:11.000000 autocbei-1.7/autocbei/cbei/cbei.py
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)     3422 2022-01-28 23:07:52.000000 autocbei-1.7/autocbei/cbei/judges.py
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)    11710 2021-12-14 00:14:11.000000 autocbei-1.7/autocbei/cbei/stat.py
-drwxrwxrwx   0 atlas     (1000) atlas     (1000)        0 2022-01-28 23:27:16.430446 autocbei-1.7/autocbei.egg-info/
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)      548 2022-01-28 23:27:16.000000 autocbei-1.7/autocbei.egg-info/PKG-INFO
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)      407 2022-01-28 23:27:16.000000 autocbei-1.7/autocbei.egg-info/SOURCES.txt
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)        1 2022-01-28 23:27:16.000000 autocbei-1.7/autocbei.egg-info/dependency_links.txt
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)       48 2022-01-28 23:27:16.000000 autocbei-1.7/autocbei.egg-info/entry_points.txt
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)       21 2022-01-28 23:27:16.000000 autocbei-1.7/autocbei.egg-info/requires.txt
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)        9 2022-01-28 23:27:16.000000 autocbei-1.7/autocbei.egg-info/top_level.txt
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)       38 2022-01-28 23:27:16.546737 autocbei-1.7/setup.cfg
--rwxrwxrwx   0 atlas     (1000) atlas     (1000)      939 2022-01-28 23:24:51.000000 autocbei-1.7/setup.py
+drwxr-xr-x   0 hyu      (14366) NR4\JIC_c1 (10917)        0 2024-05-02 11:25:49.863982 autocbei-1.8/
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)    11340 2024-05-02 10:20:38.000000 autocbei-1.8/LICENSE
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)      571 2024-05-02 11:25:49.863699 autocbei-1.8/PKG-INFO
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)    10082 2024-05-02 10:20:38.000000 autocbei-1.8/README.md
+drwxr-xr-x   0 hyu      (14366) NR4\JIC_c1 (10917)        0 2024-05-02 11:25:49.857613 autocbei-1.8/autocbei/
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)   519648 2024-05-02 10:20:38.000000 autocbei-1.8/autocbei/Bacillus_subtilis.part500.cds.all.fa
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)      464 2024-05-02 10:54:24.000000 autocbei-1.8/autocbei/__init__.py
+drwxr-xr-x   0 hyu      (14366) NR4\JIC_c1 (10917)        0 2024-05-02 11:25:49.862753 autocbei-1.8/autocbei/cbei/
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)        0 2024-05-02 10:20:38.000000 autocbei-1.8/autocbei/cbei/__init__.py
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)     4254 2024-05-02 11:08:47.000000 autocbei-1.8/autocbei/cbei/autoCBEI.py
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)     9427 2024-05-02 11:08:58.000000 autocbei-1.8/autocbei/cbei/cbei.py
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)     3350 2024-05-02 10:20:38.000000 autocbei-1.8/autocbei/cbei/judges.py
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)    11720 2024-05-02 11:10:46.000000 autocbei-1.8/autocbei/cbei/stat.py
+drwxr-xr-x   0 hyu      (14366) NR4\JIC_c1 (10917)        0 2024-05-02 11:25:49.863275 autocbei-1.8/autocbei.egg-info/
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)      571 2024-05-02 11:25:49.000000 autocbei-1.8/autocbei.egg-info/PKG-INFO
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)      407 2024-05-02 11:25:49.000000 autocbei-1.8/autocbei.egg-info/SOURCES.txt
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)        1 2024-05-02 11:25:49.000000 autocbei-1.8/autocbei.egg-info/dependency_links.txt
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)       47 2024-05-02 11:25:49.000000 autocbei-1.8/autocbei.egg-info/entry_points.txt
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)       21 2024-05-02 11:25:49.000000 autocbei-1.8/autocbei.egg-info/requires.txt
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)        9 2024-05-02 11:25:49.000000 autocbei-1.8/autocbei.egg-info/top_level.txt
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)       38 2024-05-02 11:25:49.864061 autocbei-1.8/setup.cfg
+-rw-r--r--   0 hyu      (14366) NR4\JIC_c1 (10917)      939 2024-05-02 11:20:28.000000 autocbei-1.8/setup.py
```

### Comparing `autocbei-1.7/LICENSE` & `autocbei-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autocbei-1.7/README.md` & `autocbei-1.8/README.md`

 * *Files identical despite different names*

### Comparing `autocbei-1.7/autocbei/Bacillus_subtilis.part500.cds.all.fa` & `autocbei-1.8/autocbei/Bacillus_subtilis.part500.cds.all.fa`

 * *Files identical despite different names*

### Comparing `autocbei-1.7/autocbei/cbei/autoCBEI.py` & `autocbei-1.8/autocbei/cbei/autoCBEI.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     print("-"*30)
     sys.exit()
 
 def mainAutoCBEI():
     #Set the Base editor parameter
     # [PAM, spacer length, edit beg, edit end, direction]
     # Direction refers to spacer at the 5' or 3' end of PAM sequence (5 or 3, respectively). 
+    
     beinfos = {
         "BE":["NGG",20,4,8,5],
         "YE1-BE3":["NGG",20,5,7,5],
         "EE-BE3":["NGG",20,5,6,5],
         "YEE-BE3":["NGG",20,6,6,5],
         "VQR-BE3":["NGAN",20,4,11,5],
         "VRER-BE3":["NGCG",20,3,10,5],
@@ -90,19 +91,18 @@
     for key in beinfos.keys():
         print("\t"+key,end="\t")
         for t in beinfos[key]:
             print(t,end="\t")
         print()
 
     seqDict = SeqIO.index(args.cds, "fasta")
-    tName=os.path.basename(args.cds).split(".")
-    fileName=tName[0]
+    fileName=pre
     for key in beinfos:
         print("Start calculating: "+key)
-        cbei.runBatch(key, beinfos[key], seqDict,rawPath)
+        cbei.runBatch(key, beinfos[key], seqDict,rawPath,pre)
     print("Calculate complete!")
 
     if (not args.nostat):
         print("Begin statistics...")
         print("The statistics directory: "+resPath)
         print("The plot directory: "+plotPath)
```

### Comparing `autocbei-1.7/autocbei/cbei/cbei.py` & `autocbei-1.8/autocbei/cbei/cbei.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys,re,json,os,shutil
 from Bio import SeqIO
-from Bio.SeqUtils import GC
 
 baseT = {
     "A": "T",
     "T": "A",
     "C": "G",
     "G": "C",
     "U": "A",
@@ -244,18 +243,18 @@
 
         pamInfo['editpos'] = editPos
         pamInfo['location'] = location
         pamInfo['editpatten'] = editPatten
         preStop.append(pamInfo)
     return preStop
 
-def runBatch(bename, beinfo, seqDict,rawPath):
+def runBatch(bename, beinfo, seqDict,rawPath,prefix):
     if ( not os.path.exists(rawPath)):
         os.mkdir(rawPath)
-    outFileName=bename+"_"+os.path.basename(sys.argv[1])+".cbei";
+    outFileName=bename+"_"+prefix+".cbei";
     endReg = re.compile(r'cag|caa|cga', re.I)
     endRegM = re.compile(r'cca', re.I)
     pamReg = getPAMReg(beinfo[0])
     out=open(os.path.join(rawPath,outFileName),"w");
     for key in seqDict.keys():
         seq = str(seqDict[key].seq)
         seqr = tranStrand(seq)
```

### Comparing `autocbei-1.7/autocbei/cbei/stat.py` & `autocbei-1.8/autocbei/cbei/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os,re,random
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FuncFormatter
 import numpy as np
-from Bio.SeqUtils import GC
-from cycler import cycler
+from Bio.SeqUtils import gc_fraction
 
 def statCBEI(seqDict,cbeiPath,plotPath,statPath,fileName):
     transNum=len(seqDict)
     if (not os.path.exists(plotPath)):
         os.mkdir(plotPath)
 
     if (not os.path.exists(statPath)):
         os.mkdir(statPath)
 
-    files=os.listdir(cbeiPath)
+    # files=os.listdir(cbeiPath)
     allRaio={}
-    for cfile in files:
-        if(re.match(r'.*'+fileName+'.*\.cbei$',cfile,re.I)):
-            tmp=cfile.split(".")
-            be=tmp[0].split("_")[0]
-            filePath=os.path.join(cbeiPath,cfile)
-            cbeiInfo=getInfo(be,fileName,filePath,statPath)
-            allRaio[be]=[len(cbeiInfo["t25"])/transNum,len(cbeiInfo["t5"])/transNum,len(cbeiInfo["t75"])/transNum,]        
-            editablePie(cfile,transNum,cbeiInfo["t25"],cbeiInfo["t5"],cbeiInfo["t75"],plotPath)
+    for cfile in os.listdir(cbeiPath):
+        if (not cfile.endswith(".cbei")):
+            continue
+        # if(re.match(r'.*'+fileName+'.*\.cbei$',cfile,re.I)):
+        tmp=cfile.split(".")
+        be=tmp[0].split("_")[0]
+        filePath=os.path.join(cbeiPath,cfile)
+        cbeiInfo=getInfo(be,fileName,filePath,statPath)
+        allRaio[be]=[len(cbeiInfo["t25"])/transNum,len(cbeiInfo["t5"])/transNum,len(cbeiInfo["t75"])/transNum,]        
+        editablePie(cfile,transNum,cbeiInfo["t25"],cbeiInfo["t5"],cbeiInfo["t75"],plotPath)
     print("#"*20)
     print("Pie charts for different BEs have been generated. \nPath:")
     print("\t"+os.path.join(plotPath,"[BE names]_"+fileName+".statPie.png"))
     
     transGCStat(fileName,seqDict,plotPath)
     print("Transcript statistics and mapping completed.\nPath:\n\t"+os.path.join(plotPath,fileName+"_CDSlength.png"))
     print("\t"+os.path.join(plotPath,fileName+"_GCstats.png"))
@@ -37,17 +38,16 @@
     print("The comparison of CBEI ratio of different BE has been completed.\nPath:")
     print("\t"+os.path.join(plotPath,fileName+".statBar.png"))
     begROC(transNum, cbeiPath, plotPath,fileName)
     print("\t"+os.path.join(plotPath,fileName+".statROC.png"))
     
 def begROC(transNum, cbeiPath, plotPath,fileName):
     beName={}
-    files=os.listdir(cbeiPath)
-    for file in files:
-        if not (re.match(r".*"+fileName+".*\.cbei$",file,re.I)):
+    for file in os.listdir(cbeiPath):
+        if (not file.endswith(".cbei")):
             continue
         title=file.strip().split(".")
         beName[title[0]]=[0 for k in range(0,100)]
         with open(os.path.join(cbeiPath,file)) as f:
             tgene={}
             for line in f:
                 if (re.match(r'^#.*$',line,re.I)):
@@ -197,15 +197,15 @@
             continue
         for i in range(0, len(seq), 3):
             codon = seq[i : i + 3]
             if (codon in Codons):
                 Codons[codon]+=1
                 cCount+=1
         seqlength.append(len(seq))
-        gc_values.append(GC(seq))
+        gc_values.append(gc_fraction(seq))
     gc_values=sorted(gc_values)
     plt.subplots(figsize=(6, 6))
     plt.plot(gc_values)
     plt.title("GC%% of %i CDSs \n from %.2f%% to %.2f%%" % (len(seqDict),min(gc_values),max(gc_values)))
     plt.ylabel("GC content (%)")
     plt.xlabel("CDSs")
     plt.savefig(os.path.join(plotPath,fileName+"_GCstats.png"),dpi=300)
```

### Comparing `autocbei-1.7/setup.py` & `autocbei-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="autocbei",
-    version="1.7",
+    version="1.8",
     packages=find_packages(exclude=["cbeiUnitTests"]),
     description = '"autoCBEI.py" can calculate the potential CBEI loci of the target CDSs and perform statistics and plots.',
     author = "Haopeng Yu",
     author_email = "atlasbioin4@gmail.com",
     url = "https://github.com/atlasbioinfo/CRISPR-CBEI/tree/master/autoCBEI",
-    python_requires='>=3.6.0',
+    python_requires='>=3.7.0',
     license='Apache-2.0',
     entry_points = {
         'console_scripts' : [
             'autocbei = autocbei:mainCBEI'
         ]
     },
     classifiers=[
```

