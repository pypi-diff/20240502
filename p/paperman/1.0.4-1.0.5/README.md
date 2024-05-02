# Comparing `tmp/paperman-1.0.4.tar.gz` & `tmp/paperman-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperman-1.0.4.tar", last modified: Tue Apr 30 05:53:26 2024, max compression
+gzip compressed data, was "paperman-1.0.5.tar", last modified: Thu May  2 06:10:21 2024, max compression
```

## Comparing `paperman-1.0.4.tar` & `paperman-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2024-02-15 07:11:38.000000 paperman-1.0.4/LICENSE.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11699 2024-04-30 05:53:26.545028 paperman-1.0.4/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11360 2024-02-15 07:32:45.000000 paperman-1.0.4/README.md
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman/
--rw-r--r--   0 bredol    (1000) bredol    (1000)      418 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/__init__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11362 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/__main__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     5072 2024-04-30 05:53:10.000000 paperman-1.0.4/paperman/cfg.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     6384 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/finder.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4656 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/io.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman/parser/
--rw-r--r--   0 bredol    (1000) bredol    (1000)       98 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/__init__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    15175 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/bib.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    16701 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/cite.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      609 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/common.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1232 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/img.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    57618 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/journal.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    13003 2024-04-30 05:53:10.000000 paperman-1.0.4/paperman/parser/tex.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     5040 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/project.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman/subcommands/
--rw-r--r--   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/__init__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4344 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/bib.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1610 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/clean.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     6012 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/collect.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1173 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/common.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      146 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/config.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     5682 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/diff.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     3221 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/img.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      871 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/inp.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      496 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/journal.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     7600 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/lib.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      298 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/lint.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1317 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/sort_authors.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4440 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/sync.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1482 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/utils.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman.egg-info/
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11699 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)      953 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/SOURCES.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/dependency_links.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       52 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/entry_points.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       49 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/requires.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        9 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/top_level.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2024-04-30 05:53:26.545028 paperman-1.0.4/setup.cfg
--rwxr-xr-x   0 bredol    (1000) bredol    (1000)     1545 2024-04-30 05:53:26.000000 paperman-1.0.4/setup.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-05-02 06:10:21.894408 paperman-1.0.5/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2024-02-15 07:11:38.000000 paperman-1.0.5/LICENSE.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11724 2024-05-02 06:10:21.894408 paperman-1.0.5/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11360 2024-02-15 07:32:45.000000 paperman-1.0.5/README.md
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-05-02 06:10:21.894408 paperman-1.0.5/paperman/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      418 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/__init__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11362 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/__main__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4935 2024-04-30 06:09:25.000000 paperman-1.0.5/paperman/cfg.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     6384 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/finder.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4656 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/io.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-05-02 06:10:21.894408 paperman-1.0.5/paperman/parser/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       98 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/parser/__init__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    16711 2024-05-02 06:08:58.000000 paperman-1.0.5/paperman/parser/bib.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    17654 2024-05-02 06:08:58.000000 paperman-1.0.5/paperman/parser/cite.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      609 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/parser/common.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1232 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/parser/img.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    57618 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/parser/journal.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    13233 2024-05-02 06:08:58.000000 paperman-1.0.5/paperman/parser/tex.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     5040 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/project.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-05-02 06:10:21.894408 paperman-1.0.5/paperman/subcommands/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/__init__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4344 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/bib.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1610 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/clean.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     5262 2024-05-02 06:08:58.000000 paperman-1.0.5/paperman/subcommands/collect.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1173 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/common.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      146 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/config.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     5682 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/diff.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     3221 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/img.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      871 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/inp.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      496 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/journal.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     7520 2024-05-02 05:59:08.000000 paperman-1.0.5/paperman/subcommands/lib.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      298 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/lint.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1317 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/sort_authors.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4440 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/subcommands/sync.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1482 2024-02-15 07:11:38.000000 paperman-1.0.5/paperman/utils.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-05-02 06:10:21.894408 paperman-1.0.5/paperman.egg-info/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11724 2024-05-02 06:10:21.000000 paperman-1.0.5/paperman.egg-info/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      953 2024-05-02 06:10:21.000000 paperman-1.0.5/paperman.egg-info/SOURCES.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2024-05-02 06:10:21.000000 paperman-1.0.5/paperman.egg-info/dependency_links.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       52 2024-05-02 06:10:21.000000 paperman-1.0.5/paperman.egg-info/entry_points.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       59 2024-05-02 06:10:21.000000 paperman-1.0.5/paperman.egg-info/requires.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        9 2024-05-02 06:10:21.000000 paperman-1.0.5/paperman.egg-info/top_level.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2024-05-02 06:10:21.894408 paperman-1.0.5/setup.cfg
+-rwxr-xr-x   0 bredol    (1000) bredol    (1000)     1558 2024-05-02 06:10:21.000000 paperman-1.0.5/setup.py
```

### Comparing `paperman-1.0.4/LICENSE.txt` & `paperman-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/PKG-INFO` & `paperman-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: paperman
-Version: 1.0.4
+Version: 1.0.5
 Summary: latex project and bibliography management utility
 Author: zaphB
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: appdirs
 Requires-Dist: argparse
 Requires-Dist: argcomplete
 Requires-Dist: pyyaml
 Requires-Dist: cloudscraper
+Requires-Dist: unidecode
 
 # Latex Project and Bibliography Management Utilities
 
 Paperman is a command line utility designed to accelerate your latex writing workflow by automating tasks as:
  * finding and copying frequently used images, bibtex entries and input tex-files from your other tex documents
  * identifying unused image files and bibtex entries in your latex project
  * maintaining consistent capitalization of titles in bibtex entries
```

### Comparing `paperman-1.0.4/README.md` & `paperman-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/__main__.py` & `paperman-1.0.5/paperman/__main__.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/cfg.py` & `paperman-1.0.5/paperman/cfg.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,18 +51,14 @@
     known_authors=[],
 #    check_spelling=[]
   ),
   library_path = '~/Documents/bibliography',
   library_sync_additional_paths = [],
   library_collect_paths = ['~/Desktop', '~/Downloads'],
   library_folder_pattern = '%Y-%m',
-  library_max_filename_len = 60,
-  library_max_filename_segment_len = 60,
-  library_max_key_len = 20,
-  library_max_key_segment_len = 5,
   library_sync_device = '',
   library_sync_max_age = 365*24*60*60,
   z_bib_words_protect_capitalization = [],
   z_bib_words_dont_protect_capitalization = [],
   z_bib_journals = {},
   z_verified_urls = [],
   z_verified_dois = []
```

### Comparing `paperman-1.0.4/paperman/finder.py` & `paperman-1.0.5/paperman/finder.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/io.py` & `paperman-1.0.5/paperman/io.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/parser/bib.py` & `paperman-1.0.5/paperman/parser/bib.py`

 * *Files 7% similar despite different names*

```diff
@@ -341,14 +341,38 @@
                 and state == 'comment',
             'citation section was started but never ended,\n'
             'probably due to unmatched curly braces')
 
     return res
 
 
+  def _duplicates(self):
+    byKey, byGeneratedKey, byCompareAuthorTitle = {}, {}, {}
+    for cite in self.cites():
+      for d, k in zip([byKey, byGeneratedKey, byCompareAuthorTitle],
+                      [cite.key, cite.makeKey(), cite.compareAuthorTitle()]):
+        if k not in d.keys():
+          d[k] = []
+        d[k].append(cite)
+    return [ [c for c in d.values() if len(c)>1]
+                    for d in (byKey, byGeneratedKey, byCompareAuthorTitle) ]
+
+  
+  def duplicatesKeys(self):
+    return self._duplicates()[0]
+
+
+  def duplicatesGeneratedKeys(self):
+    return self._duplicates()[1]
+
+
+  def duplicatesAuthorTitle(self):
+    return self._duplicates()[2]
+
+
   def addCites(self, cites):
     if cites:
       with open(self.path, 'a') as f:
         f.write('\n'+'\n\n'.join([c.pretty() for c in cites])+'\n')
       self._cites = None
       self.cites()
 
@@ -418,7 +442,30 @@
                           + "--" + entries.get('endpage', '') + '},\n')
                   + 'url={'+entries['url']+'},\n'
                   + '}\n')
     io.dbg('converted ris to bib: ', bibStr)
     res = BibFile('')
     res._content = bibStr
     return res
+
+
+  def lint(self, visited=[]):
+    reported = []
+
+    # report duplicates
+    for duplicates in self.duplicatesKeys():
+      if duplicates not in reported:
+        reported.append(duplicates)
+        yield (self.path, '?', f'found bib entries with duplicate '
+                  f'key {duplicates[0].key}')
+
+    for duplicates in self.duplicatesGeneratedKeys():
+      if duplicates not in reported:
+        reported.append(duplicates)
+        yield (self.path, '?', f'found bib entries with conflicting generated '
+                  f'keys:\n{", ".join([d.key for d in duplicates])}')
+
+    for duplicates in self.duplicatesAuthorTitle():
+      if duplicates not in reported:
+        reported.append(duplicates)
+        yield (self.path, '?', f'found bib entries with identical authors and title:\n'
+                  f'{", ".join([d.key for d in duplicates])}')
```

### Comparing `paperman-1.0.4/paperman/parser/cite.py` & `paperman-1.0.5/paperman/parser/cite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import requests
 import cloudscraper
 import time
+import unidecode
 
 from .. import io
 from .. import cfg
 from .. import utils
 
 FORBIDDEN_KEY_CHARS = r'''#'",=(){}%~\ '''
 
@@ -238,17 +239,21 @@
     if item.lower() not in lkeys:
       return None, None
 
     k = keys[lkeys.index(item.lower())]
 
     # if limited by { and } or ", strip those
     f = self.fields[k]
-    p = self.fieldsParseInfo.get(k, {})
-    if p and p['opens'] and p['closes']:
-      return k, f[p['opens'][0]+1:p['closes'][-1]]
+    while (( f.strip().startswith('{') 
+              and f.strip().endswith('}') )
+        or ( f.strip().startswith('"') 
+              and f.strip().endswith('"') ) ):
+      f = f.strip()[1:-1]
+
+    # return key and result
     return k, f
 
 
   def insertNonexistingItems(self, cite):
     lkeys = [k.lower() for k in self.fields.keys()]
     for k, v in cite.fields.items():
       if k not in lkeys:
@@ -288,14 +293,41 @@
       fieldsStr += f'  {k} = {v},\n'
     # strip trailing comma+newline and wrap properly
     if fieldsStr:
       fieldsStr = f',\n{fieldsStr[:-2]}\n'
     return f'@{self.section}{{{self.key}'+fieldsStr+'}'
 
 
+  def makeKey(self):
+    res = []
+    author, title, year = [self.get(k, '') for k in 'author title year'.split()]
+
+    # add first author's lastname
+    author = re.sub(r'[^a-z0-9,\s]+', '', unidecode.unidecode(author).lower())
+    if author:
+      firstAuthor = author.split('and')[0]
+      lastName = firstAuthor.split(',')[0].split()[-1]
+      res.append(lastName.lower())
+
+    # add title
+    title = re.sub(r'[^a-z0-9\s]+', '', unidecode.unidecode(title).lower())
+    if title:
+      segments = [s.strip() for s in title.split() 
+                    if s.strip() and s not in (
+                        'in', 'of', 'for', 'by', 'the', 'and', 'a', 'on')]
+      res.extend(segments[:2])
+
+    # add year
+    year = re.sub(r'[^a-z0-9\s]+', '', unidecode.unidecode(year).lower())
+    if year:
+      res.append(year)
+
+    return '_'.join(res)
+
+
   def pretty(self):
     fieldsStr = ''
     if self.fields is not None:
       # strip http etc. from doi field if existing
       doi = self['doi']
       if (cfg.get('bib_repair', 'repair_doi')
           and doi is not None):
@@ -321,28 +353,26 @@
         if err:
           if 'cloudflare' in err.lower():
             _printCloudflareWarning()
             io.dbg(f'citation {self.key} has {err}')
           else:
             io.warn(f'citation {self.key} has {err}')
 
-
       # check if doi is valid if connected to the internet and doi present
       doi = self['doi']
       if (cfg.get('bib_repair', 'verify_doi_exists')
           and doi is not None):
         err = isDoiValid(doi)
         if err:
           if 'cloudflare' in err.lower():
             _printCloudflareWarning()
             io.dbg(f'citation {self.key} has {err}')
           else:
             io.warn(f'citation {self.key} has {err}')
 
-
       # reformat pages field if exists
       pages = self['pages']
       if (cfg.get('bib_repair', 'keep_only_startpage_in_pages')
                 and pages is not None):
         m = re.match(r'^(\d+)', pages)
         if m:
           self['pages'] = m.groups()[0]
```

### Comparing `paperman-1.0.4/paperman/parser/common.py` & `paperman-1.0.5/paperman/parser/common.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/parser/img.py` & `paperman-1.0.5/paperman/parser/img.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/parser/journal.py` & `paperman-1.0.5/paperman/parser/journal.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/parser/tex.py` & `paperman-1.0.5/paperman/parser/tex.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,20 +258,29 @@
   @utils.cacheReturnValue
   def missingCites(self):
     return [c for c in self.cites() if c.isHealthy() and not c.exists()]
 
 
   @utils.cacheReturnValue
   def lint(self, visited=[]):
+
+    # lint included files
     for i in self.includes():
       if i not in visited:
         for l in i.lint(visited=visited):
           yield l
         visited.append(i)
 
+    # lint included bib files
+    for b in self.bibs():
+      if b not in visited:
+        for l in b.lint(visited=visited):
+          yield l
+        visited.append(b)
+
     # detect author entries and check whether they exist in whitelist
     authorPattern = r'([^\n]*)\\author\{([^}]*)\}([^\n]*)'
     knownAuthors = list(cfg.get('lint', 'known_authors'))
 
     for pre, authorName, post in re.findall(authorPattern, self.content(), re.M):
       # skip lines marked as ok:
       textAround = pre + ' ' + post
@@ -282,15 +291,15 @@
       authorName = authorName.strip()
       if authorName not in knownAuthors:
         if io.conf(f'found author {authorName} which is not in known_authors list, ',
                    f'add to list?', default=False):
           knownAuthors = knownAuthors+[authorName]
           cfg.set('lint', 'known_authors', knownAuthors)
         else:
-          yield (self.path, nan,
+          yield (self.path, '?',
                  f'author name {authorName} is not in known_authors list')
 
 
     for ln, l in self.enumContent():
       # skip lines marked as ok:
       if 'nolint' in l.split() or '%nolint' in l.split():
         continue
@@ -350,15 +359,15 @@
         if re.search(r'\b'+word.lower()+r'\b', l.lower()):
           yield (self.path, ln,
                  f'found word {word}, which is on avoid-list')
 
       # find double words
       _l = re.sub(r'\s+', ' ', l.replace(',', '').replace('.', ''))
       for w1, w2 in zip(_l.split()[:-1], _l.split()[1:]):
-        if w1 == w2:
+        if w1 == w2 and re.match(r'[a-zA-Z0-9]', w1):
           yield (self.path, ln,
                  f'found duplicate word "{w1}"')
 
       # detect commas before that and because
       for word in ('because', 'that'):
         if re.search(r',\s*'+word, l.lower()):
           yield (self.path, ln,
```

### Comparing `paperman-1.0.4/paperman/project.py` & `paperman-1.0.5/paperman/project.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/bib.py` & `paperman-1.0.5/paperman/subcommands/bib.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/clean.py` & `paperman-1.0.5/paperman/subcommands/clean.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/collect.py` & `paperman-1.0.5/paperman/subcommands/collect.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,14 @@
 import time
 import shutil
 
 from .. import parser
 from . common import *
 
 
-def makeKey(string, maxTotLen, maxSegLen):
-  res = ""
-  for s in re.sub("[^a-z0-9 ]+", "", string.lower()).split():
-    s = s.lower().strip()
-    if len(res)+len(s[:maxSegLen])+1 > maxTotLen:
-      break
-    elif res == "":
-      res += s[:maxSegLen]
-    else:
-      res += "-"+s[:maxSegLen]
-  return res
-
-
 def main(args):
   # check of library path is set
   libraryPath = os.path.expanduser(cfg.get('library_path'))
   if not libraryPath:
     io.err('library_path is not set in config file')
     return
 
@@ -72,72 +59,63 @@
 
         if len(pdfs) == 1 and len(bibs) == 1:
           pdfPath = pdfs[0]
           bibPath = bibs[0]
 
           # load and parse bib file (retry five times in case bib file was not
           # completely written when it was initially discovered)
+          cites = []
           for _ in range(5):
             try:
               if bibPath.lower().endswith('.ris'):
                 r = parser.BibFile.fromRis('key', bibPath)
                 io.dbg(r)
                 cites = r.cites()
               else:
                 cites = parser.BibFile(bibPath).cites()
               if len(cites) != 1:
                 raise ValueError('invalid number of citations in bib file')
               break
-            except KeyboardInterrupt:
-              raise
-            except:
+            except Exception:
               time.sleep(.1)
 
           io.dbg('cites:', cites)
           if len(cites) == 1:
             cite = cites[0]
 
-            fullTitle = cite['title']
-            if fullTitle:
+            # run pretty method to clean up fields and trigger potential reformatting questions
+            cite.pretty()
 
-              # generate key and filename from paper title
-              libraryName = makeKey(fullTitle,
-                                    cfg.get('library_max_filename_len'),
-                                    cfg.get('library_max_filename_segment_len'))
-              cite.key = makeKey(fullTitle,
-                                 cfg.get('library_max_key_len'),
-                                 cfg.get('library_max_key_segment_len'))
-              libraryDir = os.path.join(libraryPath,
-                                        time.strftime(cfg.get('library_folder_pattern')))
-              target = os.path.join(libraryDir, libraryName)
-              os.makedirs(os.path.dirname(target), exist_ok=True)
-              if not any([f.startswith(target)
-                              for f in os.listdir(os.path.dirname(target))]):
-                targetName = target+'.'+cfg.get('bibtex_extensions')[0]
-                try:
-                  with open(targetName, 'w') as f:
-                    f.write(cite.pretty()+'\n')
-                except:
-                  if os.path.exists(targetName):
-                    os.remove(targetName)
-                  raise
-                os.remove(bibPath)
-                #io.info(f'moved "{bibPath}" -> "{target}.{cfg.get("bibtex_extensions")[0]}"')
-                shutil.move(pdfPath, target+'.pdf')
-                #io.info(f'moved "{pdfPath}" -> "{target}.pdf"')
-                io.info(f'imported "{cite.key}"')
-
-                # reset lastErr memory
-                lastErrStr = ''
-              else:
-                onError(pdfPath, 'failed to move files to library, target',
-                        '"'+target+'"', 'already exists')
+            # generate key and filename from paper title
+            cite.key = cite.makeKey()
+            libraryDir = os.path.join(libraryPath,
+                                      time.strftime(cfg.get('library_folder_pattern')))
+            target = os.path.join(libraryDir, cite.key)
+            os.makedirs(os.path.dirname(target), exist_ok=True)
+            if not any([f.startswith(target)
+                            for f in os.listdir(os.path.dirname(target))]):
+              targetName = target+'.'+cfg.get('bibtex_extensions')[0]
+              try:
+                with open(targetName, 'w') as f:
+                  f.write(cite.pretty()+'\n')
+              except Exception:
+                if os.path.exists(targetName):
+                  os.remove(targetName)
+                raise
+              os.remove(bibPath)
+              #io.info(f'moved "{bibPath}" -> "{target}.{cfg.get("bibtex_extensions")[0]}"')
+              shutil.move(pdfPath, target+'.pdf')
+              #io.info(f'moved "{pdfPath}" -> "{target}.pdf"')
+              io.info(f'imported "{cite.key}"')
 
+              # reset lastErr memory
+              lastErrStr = ''
             else:
-              onError(pdfPath, 'failed to find title in bib file')
+              onError(pdfPath, 'failed to move files to library, target',
+                      '"'+target+'"', 'already exists')
 
           else:
             onError(pdfPath, f'found unexpected citation count ({len(cites)}) in bib file')
 
         # situation that naturally occurs, do not print error
         elif (len(pdfs)==1 and len(bibs)==0) or (len(pdfs)==0 and len(bibs)==1):
           pass
```

### Comparing `paperman-1.0.4/paperman/subcommands/common.py` & `paperman-1.0.5/paperman/subcommands/common.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/diff.py` & `paperman-1.0.5/paperman/subcommands/diff.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/img.py` & `paperman-1.0.5/paperman/subcommands/img.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/inp.py` & `paperman-1.0.5/paperman/subcommands/inp.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/lib.py` & `paperman-1.0.5/paperman/subcommands/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,31 +63,27 @@
     for f in files:
       path = os.path.join(root, f)
       if any([f.lower().endswith('.'+e) for e in cfg.get('bibtex_extensions')]):
         # if bibfile and search is enabled, check of matching
         if search:
           try:
             c = parser.BibFile(path).cites()[0]
-          except KeyboardInterrupt:
-            raise
-          except:
+          except Exception:
             io.verb(f'skipping invalid library entry {path}')
           else:
             if all([any([s.lower() in v.lower()
                                   for v in c.fields.values()])
                                       for s in search]):
               matches.append(path)
 
         # if scan is enabled, check if file is successfully parsed
         if scan:
           try:
             c = parser.BibFile(path).cites()[0]
-          except KeyboardInterrupt:
-            raise
-          except:
+          except Exception:
             invalidBibFiles.append(path)
           else:
             # add to duplicate keys dict
             if c.key not in foundDuplicates:
               foundDuplicates[c.key] = []
             foundDuplicates[c.key].append(path)
 
@@ -140,15 +136,15 @@
               healthyCount += 0.5
             else:
               unpairedFiles.append(path)
 
   if search or fulltextSearch:
     if not matches:
       io.info('no matches')
-    for m in matches:
+    for m in sorted(matches):
       bibPath = None
       for ext in cfg.get('bibtex_extensions'):
         _bibPath = utils.replaceSuffix(m, ext)
         if os.path.exists(_bibPath):
           bibPath = _bibPath
           break
       if args.long:
```

### Comparing `paperman-1.0.4/paperman/subcommands/sort_authors.py` & `paperman-1.0.5/paperman/subcommands/sort_authors.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/subcommands/sync.py` & `paperman-1.0.5/paperman/subcommands/sync.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman/utils.py` & `paperman-1.0.5/paperman/utils.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/paperman.egg-info/PKG-INFO` & `paperman-1.0.5/paperman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: paperman
-Version: 1.0.4
+Version: 1.0.5
 Summary: latex project and bibliography management utility
 Author: zaphB
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: appdirs
 Requires-Dist: argparse
 Requires-Dist: argcomplete
 Requires-Dist: pyyaml
 Requires-Dist: cloudscraper
+Requires-Dist: unidecode
 
 # Latex Project and Bibliography Management Utilities
 
 Paperman is a command line utility designed to accelerate your latex writing workflow by automating tasks as:
  * finding and copying frequently used images, bibtex entries and input tex-files from your other tex documents
  * identifying unused image files and bibtex entries in your latex project
  * maintaining consistent capitalization of titles in bibtex entries
```

### Comparing `paperman-1.0.4/paperman.egg-info/SOURCES.txt` & `paperman-1.0.5/paperman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperman-1.0.4/setup.py` & `paperman-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3
 
 from setuptools import setup
 from setuptools.command.install import install
 
 # DO NOT CHANGE: this line will be replaced by ./dev/update-setup.py
-version = '1.0.4'
+version = '1.0.5'
 
 # if setup is run in project dir, update version number
 try:
   import os
   import subprocess
   p = os.path.join(os.path.dirname(__file__), 'dev/update-setup.sh')
   if (os.path.isfile(p) and os.access(p, os.X_OK)):
@@ -42,12 +42,12 @@
       packages=['paperman', 'paperman.subcommands', 'paperman.parser'],
       entry_points={
         'console_scripts': [
           'paperman = paperman.__main__:main'
         ],
         'gui_scripts': []
       },
-      install_requires=['appdirs', 'argparse', 'argcomplete', 'pyyaml', 'cloudscraper'],
+      install_requires=['appdirs', 'argparse', 'argcomplete', 'pyyaml', 'cloudscraper', 'unidecode'],
       cmdclass={
         'install': PostInstall
       }
 )
```

