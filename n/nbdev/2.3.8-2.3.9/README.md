# Comparing `tmp/nbdev-2.3.8.tar.gz` & `tmp/nbdev-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-2.3.8.tar", last modified: Wed Nov  2 02:07:57 2022, max compression
+gzip compressed data, was "nbdev-2.3.9.tar", last modified: Tue Nov  8 23:17:38 2022, max compression
```

## Comparing `nbdev-2.3.8.tar` & `nbdev-2.3.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-11-02 02:07:57.273327 nbdev-2.3.8/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2344 2022-07-24 22:10:56.000000 nbdev-2.3.8/CONTRIBUTING.md
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11357 2022-07-24 22:10:56.000000 nbdev-2.3.8/LICENSE
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      111 2022-07-24 22:10:56.000000 nbdev-2.3.8/MANIFEST.in
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    10288 2022-11-02 02:07:57.273327 nbdev-2.3.8/PKG-INFO
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9421 2022-10-17 01:10:27.000000 nbdev-2.3.8/README.md
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-11-02 02:07:57.269327 nbdev-2.3.8/nbdev/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       89 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    37630 2022-11-02 02:02:56.000000 nbdev-2.3.8/nbdev/_modidx.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9114 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/clean.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4080 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/cli.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11928 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/config.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9670 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/doclinks.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2472 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/export.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2208 2022-07-24 22:10:56.000000 nbdev-2.3.8/nbdev/extract_attachments.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2181 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/frontmatter.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       95 2022-07-24 22:10:56.000000 nbdev-2.3.8/nbdev/imports.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9601 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/maker.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4257 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/merge.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7271 2022-11-02 02:02:56.000000 nbdev-2.3.8/nbdev/migrate.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5692 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/process.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9977 2022-11-02 02:02:56.000000 nbdev-2.3.8/nbdev/processors.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2931 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/qmd.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9645 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/quarto.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    13354 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/release.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2834 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/serve.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      657 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/serve_drv.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9134 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/showdoc.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2866 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/sync.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4313 2022-10-17 01:10:27.000000 nbdev-2.3.8/nbdev/test.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-11-02 02:07:57.273327 nbdev-2.3.8/nbdev.egg-info/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    10288 2022-11-02 02:07:56.000000 nbdev-2.3.8/nbdev.egg-info/PKG-INFO
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      660 2022-11-02 02:07:57.000000 nbdev-2.3.8/nbdev.egg-info/SOURCES.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-11-02 02:07:56.000000 nbdev-2.3.8/nbdev.egg-info/dependency_links.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     1218 2022-11-02 02:07:57.000000 nbdev-2.3.8/nbdev.egg-info/entry_points.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-02-15 01:05:39.000000 nbdev-2.3.8/nbdev.egg-info/not-zip-safe
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      152 2022-11-02 02:07:57.000000 nbdev-2.3.8/nbdev.egg-info/requires.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        6 2022-11-02 02:07:57.000000 nbdev-2.3.8/nbdev.egg-info/top_level.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2203 2022-10-17 01:10:27.000000 nbdev-2.3.8/settings.ini
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       38 2022-11-02 02:07:57.273327 nbdev-2.3.8/setup.cfg
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2705 2022-10-17 01:10:27.000000 nbdev-2.3.8/setup.py
+drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-11-08 23:17:38.844982 nbdev-2.3.9/
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2344 2022-07-24 22:10:56.000000 nbdev-2.3.9/CONTRIBUTING.md
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11357 2022-07-24 22:10:56.000000 nbdev-2.3.9/LICENSE
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      111 2022-07-24 22:10:56.000000 nbdev-2.3.9/MANIFEST.in
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    10288 2022-11-08 23:17:38.844982 nbdev-2.3.9/PKG-INFO
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9421 2022-10-17 01:10:27.000000 nbdev-2.3.9/README.md
+drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-11-08 23:17:38.844982 nbdev-2.3.9/nbdev/
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       89 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/__init__.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    37759 2022-11-08 23:13:15.000000 nbdev-2.3.9/nbdev/_modidx.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9114 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/clean.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4080 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/cli.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11928 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/config.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9912 2022-11-08 23:13:15.000000 nbdev-2.3.9/nbdev/doclinks.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2505 2022-11-08 23:13:15.000000 nbdev-2.3.9/nbdev/export.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2208 2022-07-24 22:10:56.000000 nbdev-2.3.9/nbdev/extract_attachments.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2181 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/frontmatter.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       95 2022-07-24 22:10:56.000000 nbdev-2.3.9/nbdev/imports.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9601 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/maker.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4257 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/merge.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7271 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/migrate.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5692 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/process.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9985 2022-11-08 23:13:15.000000 nbdev-2.3.9/nbdev/processors.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2931 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/qmd.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9703 2022-11-08 23:13:15.000000 nbdev-2.3.9/nbdev/quarto.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    13831 2022-11-08 23:13:15.000000 nbdev-2.3.9/nbdev/release.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2834 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/serve.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      657 2022-10-17 01:10:27.000000 nbdev-2.3.9/nbdev/serve_drv.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9134 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/showdoc.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2866 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/sync.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4313 2022-11-02 02:57:43.000000 nbdev-2.3.9/nbdev/test.py
+drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-11-08 23:17:38.844982 nbdev-2.3.9/nbdev.egg-info/
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    10288 2022-11-08 23:17:38.000000 nbdev-2.3.9/nbdev.egg-info/PKG-INFO
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      660 2022-11-08 23:17:38.000000 nbdev-2.3.9/nbdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-11-08 23:17:38.000000 nbdev-2.3.9/nbdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     1218 2022-11-08 23:17:38.000000 nbdev-2.3.9/nbdev.egg-info/entry_points.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-02-15 01:05:39.000000 nbdev-2.3.9/nbdev.egg-info/not-zip-safe
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      152 2022-11-08 23:17:38.000000 nbdev-2.3.9/nbdev.egg-info/requires.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        6 2022-11-08 23:17:38.000000 nbdev-2.3.9/nbdev.egg-info/top_level.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2203 2022-11-02 02:57:43.000000 nbdev-2.3.9/settings.ini
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       38 2022-11-08 23:17:38.848982 nbdev-2.3.9/setup.cfg
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2705 2022-10-17 01:10:27.000000 nbdev-2.3.9/setup.py
```

### Comparing `nbdev-2.3.8/CONTRIBUTING.md` & `nbdev-2.3.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/LICENSE` & `nbdev-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/PKG-INFO` & `nbdev-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev
-Version: 2.3.8
+Version: 2.3.9
 Summary: Create delightful software with Jupyter Notebooks
 Home-page: https://github.com/fastai/nbdev
 Author: Jeremy Howard and Hamel Husain
 Author-email: j@fast.ai
 License: Apache Software License 2.0
 Project-URL: Documentation, https://nbdev.fast.ai/
 Keywords: nbdev fastai jupyter notebook export
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nbdev Version: 2.3.8 Summary: Create delightful
+Metadata-Version: 2.1 Name: nbdev Version: 2.3.9 Summary: Create delightful
 software with Jupyter Notebooks Home-page: https://github.com/fastai/nbdev
 Author: Jeremy Howard and Hamel Husain Author-email: j@fast.ai License: Apache
 Software License 2.0 Project-URL: Documentation, https://nbdev.fast.ai/
 Keywords: nbdev fastai jupyter notebook export Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `nbdev-2.3.8/README.md` & `nbdev-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/_modidx.py` & `nbdev-2.3.9/nbdev/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,16 @@
                                'nbdev.release.pypi_details': ('api/release.html#pypi_details', 'nbdev/release.py'),
                                'nbdev.release.pypi_json': ('api/release.html#pypi_json', 'nbdev/release.py'),
                                'nbdev.release.release_both': ('api/release.html#release_both', 'nbdev/release.py'),
                                'nbdev.release.release_conda': ('api/release.html#release_conda', 'nbdev/release.py'),
                                'nbdev.release.release_gh': ('api/release.html#release_gh', 'nbdev/release.py'),
                                'nbdev.release.release_git': ('api/release.html#release_git', 'nbdev/release.py'),
                                'nbdev.release.release_pypi': ('api/release.html#release_pypi', 'nbdev/release.py'),
-                               'nbdev.release.write_conda_meta': ('api/release.html#write_conda_meta', 'nbdev/release.py')},
+                               'nbdev.release.write_conda_meta': ('api/release.html#write_conda_meta', 'nbdev/release.py'),
+                               'nbdev.release.write_requirements': ('api/release.html#write_requirements', 'nbdev/release.py')},
             'nbdev.serve': { 'nbdev.serve._is_qpy': ('api/serve.html#_is_qpy', 'nbdev/serve.py'),
                              'nbdev.serve._proc_file': ('api/serve.html#_proc_file', 'nbdev/serve.py'),
                              'nbdev.serve.proc_nbs': ('api/serve.html#proc_nbs', 'nbdev/serve.py')},
             'nbdev.serve_drv': {},
             'nbdev.showdoc': { 'nbdev.showdoc.BasicHtmlRenderer': ('api/showdoc.html#basichtmlrenderer', 'nbdev/showdoc.py'),
                                'nbdev.showdoc.BasicHtmlRenderer._repr_html_': ( 'api/showdoc.html#basichtmlrenderer._repr_html_',
                                                                                 'nbdev/showdoc.py'),
@@ -327,8 +328,8 @@
                             'nbdev.sync._to_absolute': ('api/sync.html#_to_absolute', 'nbdev/sync.py'),
                             'nbdev.sync._update_mod': ('api/sync.html#_update_mod', 'nbdev/sync.py'),
                             'nbdev.sync._update_nb': ('api/sync.html#_update_nb', 'nbdev/sync.py'),
                             'nbdev.sync.absolute_import': ('api/sync.html#absolute_import', 'nbdev/sync.py'),
                             'nbdev.sync.nbdev_update': ('api/sync.html#nbdev_update', 'nbdev/sync.py')},
             'nbdev.test': { 'nbdev.test._keep_file': ('api/test.html#_keep_file', 'nbdev/test.py'),
                             'nbdev.test.nbdev_test': ('api/test.html#nbdev_test', 'nbdev/test.py'),
-                            'nbdev.test.test_nb': ('api/test.html#test_nb', 'nbdev/test.py')}}}
+                            'nbdev.test.test_nb': ('api/test.html#test_nb', 'nbdev/test.py')}}}
```

### Comparing `nbdev-2.3.8/nbdev/clean.py` & `nbdev-2.3.9/nbdev/clean.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/cli.py` & `nbdev-2.3.9/nbdev/cli.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/config.py` & `nbdev-2.3.9/nbdev/config.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/doclinks.py` & `nbdev-2.3.9/nbdev/doclinks.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,24 @@
 # %% ../nbs/api/doclinks.ipynb 9
 def _iter_py_cells(p):
     "Yield cells from an exported Python file."
     p = Path(p)
     cells = p.read_text().split("\n# %% ")
     for cell in cells[1:]:
         top,code = cell.split('\n', 1)
-        nb,idx = top.split()
+        try: nb,idx = top.split()
+        except ValueError:
+            raise NotImplementedError(f"Unexpected format in '{p}' at cell:\n```\n# %% {cell.strip()}.\n```\n"
+                                      "The expected format is: '# %% {nb_path} {cell_idx}'.")
         nb_path = None if nb=='auto' else (p.parent/nb).resolve()  # NB paths are stored relative to .py file
         if code.endswith('\n'): code=code[:-1]
         yield AttrDict(nb=nb, idx=int(idx), code=code, nb_path=nb_path, py_path=p.resolve())
 
 # %% ../nbs/api/doclinks.ipynb 11
-def _nbpath2html(p): return p.with_name(re.sub(r'\d+[a-zA-Z0-9]*_', '', p.name.lower())).with_suffix('.html')
+def _nbpath2html(p): return p.with_name(re.sub(r'\d+[a-zA-Z0-9]+_', '', p.name.lower())).with_suffix('.html')
 
 # %% ../nbs/api/doclinks.ipynb 13
 def _get_modidx(py_path, code_root, nbs_path):
     "Get module symbol index for a Python source file"
     cfg = get_config()
     rel_name = py_path.resolve().relative_to(code_root).as_posix()
     mod_name = '.'.join(rel_name.rpartition('.')[0].split('/'))  # module name created by py_path
@@ -92,15 +95,15 @@
     if idxfile.exists(): res = exec_local(idxfile.read_text(), 'd')
     else: res = dict(syms={}, settings={}) 
     res['settings'] = {k:v for k,v in get_config().d.items()
                        if k in ('doc_host','doc_baseurl','lib_path','git_url','branch')}
     code_root = dest.parent.resolve()
     for file in globtastic(dest, file_glob="*.py", skip_file_re='^_', skip_folder_re="\.ipynb_checkpoints"):
         res['syms'].update(_get_modidx((dest.parent/file).resolve(), code_root, nbs_path=nbs_path))
-    idxfile.write_text("# Autogenerated by nbdev\n\nd = "+pformat(res, width=140, indent=2, compact=True))
+    idxfile.write_text("# Autogenerated by nbdev\n\nd = "+pformat(res, width=140, indent=2, compact=True)+'\n')
 
 # %% ../nbs/api/doclinks.ipynb 20
 @delegates(globtastic)
 def nbglob(path=None, skip_folder_re = '^[_.]', file_glob='*.ipynb', skip_file_re='^[_.]', key='nbs_path', as_path=False, **kwargs):
     "Find all files in a directory matching an extension given a config key."
     path = Path(path or get_config()[key])
     recursive=get_config().recursive
```

### Comparing `nbdev-2.3.8/nbdev/export.py` & `nbdev-2.3.9/nbdev/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     except: raise ImportError("You must install black: `pip install black` if you wish to use black formatting with nbdev")
     else:
         _format_str = partial(black.format_str, mode = black.Mode())
         try: cell.source = _format_str(cell.source).strip()
         except: pass
 
 # %% ../nbs/api/export.ipynb 9
-def nb_export(nbname, lib_path=None, procs=black_format, debug=False, mod_maker=ModuleMaker):
+def nb_export(nbname, lib_path=None, procs=black_format, debug=False, mod_maker=ModuleMaker, name=None):
     "Create module(s) from notebook"
     if lib_path is None: lib_path = get_config().lib_path
     exp = ExportModuleProc()
     nb = NBProcessor(nbname, [exp]+L(procs), debug=debug)
     nb.process()
     for mod,cells in exp.modules.items():
         all_cells = exp.in_all[mod]
-        name = getattr(exp, 'default_exp', None) if mod=='#' else mod
-        if not name:
+        nm = ifnone(name, getattr(exp, 'default_exp', None) if mod=='#' else mod)
+        if not nm:
             warn(f"Notebook '{nbname}' uses `#|export` without `#|default_exp` cell.\n"
                  "Note nbdev2 no longer supports nbdev1 syntax. Run `nbdev_migrate` to upgrade.\n"
                  "See https://nbdev.fast.ai/getting_started.html for more information.")
             return
-        mm = mod_maker(dest=lib_path, name=name, nb_path=nbname, is_new=mod=='#')
+        mm = mod_maker(dest=lib_path, name=nm, nb_path=nbname, is_new=bool(name) or mod=='#')
         mm.make(cells, all_cells, lib_path=lib_path)
```

### Comparing `nbdev-2.3.8/nbdev/extract_attachments.py` & `nbdev-2.3.9/nbdev/extract_attachments.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/frontmatter.py` & `nbdev-2.3.9/nbdev/frontmatter.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/maker.py` & `nbdev-2.3.9/nbdev/maker.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/merge.py` & `nbdev-2.3.9/nbdev/merge.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/migrate.py` & `nbdev-2.3.9/nbdev/migrate.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/process.py` & `nbdev-2.3.9/nbdev/process.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/processors.py` & `nbdev-2.3.9/nbdev/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     def end(self):
         try: from ipywidgets import Widget
         except ImportError: pass
         else:
             mimetype = 'application/vnd.jupyter.widget-state+json'
             old = nested_idx(self.nb.metadata, 'widgets', mimetype) or {'state': {}}
             new = Widget.get_manager_state(drop_defaults=True)
-            widgets = {**old, **new, 'state': {**old['state'], **new['state']}}
+            widgets = {**old, **new, 'state': {**old.get('state', {}), **new['state']}}
             self.nb.metadata['widgets'] = {mimetype: widgets}
 
 # %% ../nbs/api/processors.ipynb 42
 def _import_obj(s):
     mod_nm, obj_nm = s.split(':')
     mod = importlib.import_module(mod_nm)
     return getattr(mod, obj_nm)
```

### Comparing `nbdev-2.3.8/nbdev/qmd.py` & `nbdev-2.3.9/nbdev/qmd.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/quarto.py` & `nbdev-2.3.9/nbdev/quarto.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     except subprocess.CalledProcessError as cpe: sys.exit(cpe.returncode)
 
 # %% ../nbs/api/quarto.ipynb 6
 BASE_QUARTO_URL='https://www.quarto.org/download/latest/'
 
 def _install_linux():
     system(f'curl -LO {BASE_QUARTO_URL}quarto-linux-amd64.deb')
-    system('sudo dpkg -i *64.deb && rm *64.deb')
+    system('sudo dpkg -i quarto-linux-amd64.deb && rm quarto-linux-amd64.deb')
     
 def _install_mac():
     system(f'curl -LO {BASE_QUARTO_URL}quarto-macos.pkg')
-    system('sudo installer -pkg quarto-macos.pkg -target /')
+    system('sudo installer -pkg quarto-macos.pkg -target / && rm quarto-macos.pkg')
 
 @call_parse
 def install_quarto():
     "Install latest Quarto on macOS or Linux, prints instructions for Windows"
     if sys.platform not in ('darwin','linux'):
         return print('Please visit https://quarto.org/docs/get-started/ to install quarto')
     print("Installing or upgrading quarto -- this requires root access.")
@@ -100,15 +100,15 @@
             res.append(_pre(d.parent) + f'section: {title}')
             res.append(_pre(d.parent, False) + 'contents:')
             lastd = d
         res.append(f'{_pre(d)}{d.joinpath(name)}')
 
     yml_path = path/'sidebar.yml'
     yml = "website:\n  sidebar:\n    contents:\n"
-    yml += '\n'.join(f'      {o}' for o in res)
+    yml += '\n'.join(f'      {o}' for o in res)+'\n'
     if printit: return print(yml)
     yml_path.write_text(yml)
 
 # %% ../nbs/api/quarto.ipynb 13
 _quarto_yml="""project:
   type: website
```

### Comparing `nbdev-2.3.8/nbdev/release.py` & `nbdev-2.3.9/nbdev/release.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/release.ipynb.
 
 # %% auto 0
 __all__ = ['GH_HOST', 'Release', 'changelog', 'release_git', 'release_gh', 'pypi_json', 'latest_pypi', 'pypi_details',
-           'conda_output_path', 'write_conda_meta', 'anaconda_upload', 'release_conda', 'chk_conda_rel', 'release_pypi',
-           'release_both', 'bump_version', 'nbdev_bump_version']
+           'conda_output_path', 'write_conda_meta', 'write_requirements', 'anaconda_upload', 'release_conda',
+           'chk_conda_rel', 'release_pypi', 'release_both', 'bump_version', 'nbdev_bump_version']
 
 # %% ../nbs/api/release.ipynb 14
 from fastcore.all import *
 from ghapi.core import *
 
 from datetime import datetime
 import shutil,subprocess
@@ -174,17 +174,17 @@
             print(line, end='')
             res += line
 
     if p.returncode != 0: raise CalledProcessError(p.returncode, p.args)
     return res
 
 # %% ../nbs/api/release.ipynb 38
-def conda_output_path(name):
+def conda_output_path(name, build='build'):
     "Output path for conda build"
-    return run(f'conda build --output {name}').strip().replace('\\', '/')
+    return run(f'conda {build} --output {name}').strip().replace('\\', '/')
 
 # %% ../nbs/api/release.ipynb 39
 def _write_yaml(path, name, d1, d2):
     path = Path(path)
     p = path/name
     p.mkdir(exist_ok=True, parents=True)
     yaml.SafeDumper.ignore_aliases = lambda *args : True
@@ -232,76 +232,87 @@
 
 # %% ../nbs/api/release.ipynb 41
 def write_conda_meta(path='conda'):
     "Writes a `meta.yaml` file to the `conda` directory of the current directory"
     _write_yaml(path, *_get_conda_meta())
 
 # %% ../nbs/api/release.ipynb 43
+# This function is used as a utility for creating HF spaces.
+def write_requirements(directory=None):
+    "Writes a `requirements.txt` file to `directory` based on settings.ini."
+    cfg = get_config()
+    d = Path(directory) if directory else cfg.config_path
+    req = '\n'.join([cfg.get(k, '').replace(' ', '\n') for k in ['requirements', 'pip_requirements']])
+    (d/'requirements.txt').mk_write(req)
+
+# %% ../nbs/api/release.ipynb 45
 def anaconda_upload(name, loc=None, user=None, token=None, env_token=None):
     "Upload `name` to anaconda"
     user = f'-u {user} ' if user else ''
     if env_token: token = os.getenv(env_token)
     token = f'-t {token} ' if token else ''
     if not loc: loc = conda_output_path(name)
     if not loc: raise Exception("Failed to find output")
     return _run(f'anaconda {token} upload {user} {loc} --skip-existing')
 
-# %% ../nbs/api/release.ipynb 44
+# %% ../nbs/api/release.ipynb 47
 @call_parse
 def release_conda(
     path:str='conda', # Path where package will be created
     do_build:bool_arg=True,  # Run `conda build` step
     build_args:str='',  # Additional args (as str) to send to `conda build`
     skip_upload:store_true=False,  # Skip `anaconda upload` step
     mambabuild:store_true=False,  # Use `mambabuild` (requires `boa`)
     upload_user:str=None  # Optional user to upload package to
 ):
     "Create a `meta.yaml` file ready to be built into a package, and optionally build and upload it"
     name = get_config().lib_name
     write_conda_meta(path)
     out = f"Done. Next steps:\n```\ncd {path}\n"""
     os.chdir(path)
-    loc = conda_output_path(name)
-    out_upl = f"anaconda upload {loc}"
     build = 'mambabuild' if mambabuild else 'build'
-    if not do_build: return print(f"{out}conda {build} .\n{out_upl}\n```")
+    if not do_build: return print(f"{out}conda {build} {name}")
 
-    print(f"conda {build} --no-anaconda-upload {build_args} {name}")
-    res = _run(f"conda {build} --no-anaconda-upload {build_args} {name}")
-    if skip_upload: return
+    cmd = f"conda {build} --output-folder out --no-anaconda-upload {build_args} {name}"
+    print(cmd)
+    res = _run(cmd)
+    outs = globtastic('out', file_glob='*.tar.bz2')
+    assert len(outs)==1
+    loc = outs[0]
+    if skip_upload: return print(loc)
     if not upload_user: upload_user = get_config().conda_user
     if not upload_user: return print("`conda_user` not in settings.ini and no `upload_user` passed. Cannot upload")
     if 'anaconda upload' not in res: return print(f"{res}\n\Failed. Check auto-upload not set in .condarc. Try `--do_build False`.")
     return anaconda_upload(name, loc)
 
-# %% ../nbs/api/release.ipynb 45
+# %% ../nbs/api/release.ipynb 48
 def chk_conda_rel(
     nm:str,  # Package name on pypi
     apkg:str=None,  # Anaconda Package (defaults to {nm})
     channel:str='fastai',  # Anaconda Channel
     force:store_true=False  # Always return github tag
 ):
     "Prints GitHub tag only if a newer release exists on Pypi compared to an Anaconda Repo."
     if not apkg: apkg=nm
     condavs = L(loads(run(f'mamba repoquery search {apkg} -c {channel} --json'))['result']['pkgs'])
     condatag = condavs.attrgot('version').map(parse)
     pypitag = latest_pypi(nm)
     if force or not condatag or pypitag > max(condatag): return f'{pypitag}'
 
-# %% ../nbs/api/release.ipynb 47
+# %% ../nbs/api/release.ipynb 50
 @call_parse
 def release_pypi(
     repository:str="pypi" # Respository to upload to (defined in ~/.pypirc)
 ):
     "Create and upload Python package to PyPI"
     _dir = get_config().lib_path.parent
     system(f'cd {_dir}  && rm -rf dist && python setup.py sdist bdist_wheel')
     system(f'twine upload --repository {repository} {_dir}/dist/*')
 
-# %% ../nbs/api/release.ipynb 48
+# %% ../nbs/api/release.ipynb 51
 @call_parse
 def release_both(
     path:str='conda', # Path where package will be created
     do_build:bool_arg=True,  # Run `conda build` step
     build_args:str='',  # Additional args (as str) to send to `conda build`
     skip_upload:store_true=False,  # Skip `anaconda upload` step
     mambabuild:store_true=False,  # Use `mambabuild` (requires `boa`)
@@ -309,23 +320,23 @@
     repository:str="pypi" # Pypi respository to upload to (defined in ~/.pypirc)
 ):
     "Release both conda and PyPI packages"
     release_pypi.__wrapped__(repository)
     release_conda.__wrapped__(path, do_build=do_build, build_args=build_args, skip_upload=skip_upload, mambabuild=mambabuild, upload_user=upload_user)
     nbdev_bump_version.__wrapped__()
 
-# %% ../nbs/api/release.ipynb 50
+# %% ../nbs/api/release.ipynb 53
 def bump_version(version, part=2, unbump=False):
     version = version.split('.')
     incr = -1 if unbump else 1
     version[part] = str(int(version[part]) + incr)
     for i in range(part+1, 3): version[i] = '0'
     return '.'.join(version)
 
-# %% ../nbs/api/release.ipynb 51
+# %% ../nbs/api/release.ipynb 54
 @call_parse
 def nbdev_bump_version(
     part:int=2,  # Part of version to bump
     unbump:bool=False):  # Reduce version instead of increasing it
     "Increment version in settings.ini by one"
     cfg = get_config()
     print(f'Old version: {cfg.version}')
```

### Comparing `nbdev-2.3.8/nbdev/serve.py` & `nbdev-2.3.9/nbdev/serve.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/serve_drv.py` & `nbdev-2.3.9/nbdev/serve_drv.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/showdoc.py` & `nbdev-2.3.9/nbdev/showdoc.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/sync.py` & `nbdev-2.3.9/nbdev/sync.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev/test.py` & `nbdev-2.3.9/nbdev/test.py`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev.egg-info/PKG-INFO` & `nbdev-2.3.9/nbdev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev
-Version: 2.3.8
+Version: 2.3.9
 Summary: Create delightful software with Jupyter Notebooks
 Home-page: https://github.com/fastai/nbdev
 Author: Jeremy Howard and Hamel Husain
 Author-email: j@fast.ai
 License: Apache Software License 2.0
 Project-URL: Documentation, https://nbdev.fast.ai/
 Keywords: nbdev fastai jupyter notebook export
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nbdev Version: 2.3.8 Summary: Create delightful
+Metadata-Version: 2.1 Name: nbdev Version: 2.3.9 Summary: Create delightful
 software with Jupyter Notebooks Home-page: https://github.com/fastai/nbdev
 Author: Jeremy Howard and Hamel Husain Author-email: j@fast.ai License: Apache
 Software License 2.0 Project-URL: Documentation, https://nbdev.fast.ai/
 Keywords: nbdev fastai jupyter notebook export Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `nbdev-2.3.8/nbdev.egg-info/SOURCES.txt` & `nbdev-2.3.9/nbdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/nbdev.egg-info/entry_points.txt` & `nbdev-2.3.9/nbdev.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nbdev-2.3.8/settings.ini` & `nbdev-2.3.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 copyright = 2020 onwards, Jeremy Howard
 keywords = nbdev fastai jupyter notebook export
 user = fastai
 author = Jeremy Howard and Hamel Husain
 author_email = j@fast.ai
 branch = master
 min_python = 3.7
-version = 2.3.8
+version = 2.3.9
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
 requirements = fastcore>=1.5.27 execnb>=0.1.4 astunparse ghapi>=1.0.3 watchdog asttokens
 pip_requirements = PyYAML
```

### Comparing `nbdev-2.3.8/setup.py` & `nbdev-2.3.9/setup.py`

 * *Files identical despite different names*

