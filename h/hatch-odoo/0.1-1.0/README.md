# Comparing `tmp/hatch_odoo-0.1.tar.gz` & `tmp/hatch_odoo-1.0.tar.gz`

## Comparing `hatch_odoo-0.1.tar` & `hatch_odoo-1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hatch_odoo-0.1/.flake8
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hatch_odoo-0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-0.1/src/hatch_odoo/__init__.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 hatch_odoo-0.1/src/hatch_odoo/build_hook.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 hatch_odoo-0.1/src/hatch_odoo/config.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hatch_odoo-0.1/src/hatch_odoo/hooks.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 hatch_odoo-0.1/src/hatch_odoo/metadata_hook.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/conftest.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/test_build.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/test_editable.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/test_metadata.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/odoo/addons/addon_uninstallable/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/odoo/addons/addon_uninstallable/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/odoo/addons/addona/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/odoo/addons/addona/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/odoo/addons/addonb/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/odoo/addons/addonb/__manifest__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project1/src/project1/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/README.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/addon_uninstallable/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/addon_uninstallable/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/addona/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/addona/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/addonb/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/addonb/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project2/src/project2/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/odoo/addons/addon_uninstallable/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/odoo/addons/addon_uninstallable/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/odoo/addons/addona/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/odoo/addons/addona/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/odoo/addons/addonb/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/odoo/addons/addonb/__manifest__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project3/project3/__init__.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/README.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/addons_group1/odoo/addons/addon_uninstallable/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/addons_group1/odoo/addons/addon_uninstallable/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/addons_group1/odoo/addons/addona/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/addons_group1/odoo/addons/addona/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/addons_group2/odoo/addons/addonb/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/addons_group2/odoo/addons/addonb/__manifest__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project4/src/project4/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/README.md
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/addons_group1/addon_uninstallable/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/addons_group1/addon_uninstallable/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/addons_group1/addona/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/addons_group1/addona/__manifest__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/addons_group2/addonb/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/addons_group2/addonb/__manifest__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-0.1/tests/data/project5/project5/__init__.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 hatch_odoo-0.1/.gitignore
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 hatch_odoo-0.1/LICENSE.txt
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 hatch_odoo-0.1/README.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 hatch_odoo-0.1/pyproject.toml
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 hatch_odoo-0.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hatch_odoo-1.0/.flake8
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hatch_odoo-1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-1.0/src/hatch_odoo/__init__.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 hatch_odoo-1.0/src/hatch_odoo/build_hook.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 hatch_odoo-1.0/src/hatch_odoo/config.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hatch_odoo-1.0/src/hatch_odoo/hooks.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 hatch_odoo-1.0/src/hatch_odoo/metadata_hook.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/test_build.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/test_editable.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/README.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/odoo/addons/addon_uninstallable/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/odoo/addons/addon_uninstallable/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/odoo/addons/addona/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/odoo/addons/addona/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/odoo/addons/addonb/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/odoo/addons/addonb/__manifest__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project1/src/project1/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/README.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/addon_uninstallable/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/addon_uninstallable/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/addona/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/addona/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/addonb/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/addonb/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project2/src/project2/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/odoo/addons/addon_uninstallable/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/odoo/addons/addon_uninstallable/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/odoo/addons/addona/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/odoo/addons/addona/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/odoo/addons/addonb/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/odoo/addons/addonb/__manifest__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project3/project3/__init__.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/addons_group1/odoo/addons/addon_uninstallable/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/addons_group1/odoo/addons/addon_uninstallable/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/addons_group1/odoo/addons/addona/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/addons_group1/odoo/addons/addona/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/addons_group2/odoo/addons/addonb/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/addons_group2/odoo/addons/addonb/__manifest__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project4/src/project4/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/README.md
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/addons_group1/addon_uninstallable/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/addons_group1/addon_uninstallable/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/addons_group1/addona/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/addons_group1/addona/__manifest__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/addons_group2/addonb/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/addons_group2/addonb/__manifest__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_odoo-1.0/tests/data/project5/project5/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 hatch_odoo-1.0/.gitignore
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 hatch_odoo-1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 hatch_odoo-1.0/README.md
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 hatch_odoo-1.0/pyproject.toml
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 hatch_odoo-1.0/PKG-INFO
```

### Comparing `hatch_odoo-0.1/src/hatch_odoo/build_hook.py` & `hatch_odoo-1.0/src/hatch_odoo/build_hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,10 +57,10 @@
                 with tempfile.NamedTemporaryFile(
                     mode="w", encoding="utf-8", delete=False
                 ) as pth_file:
                     atexit.register(Path(pth_file.name).unlink)
                     pth_file.write(str(editable_path) + "\n")
                 project_name = get_project_name(self.root)
                 force_include_editable = build_data["force_include_editable"]
-                force_include_editable[
-                    pth_file.name
-                ] = f"{project_name}_editable_odoo_addons.pth"
+                force_include_editable[pth_file.name] = (
+                    f"{project_name}_editable_odoo_addons.pth"
+                )
```

### Comparing `hatch_odoo-0.1/src/hatch_odoo/config.py` & `hatch_odoo-1.0/src/hatch_odoo/config.py`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/src/hatch_odoo/hooks.py` & `hatch_odoo-1.0/src/hatch_odoo/hooks.py`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/src/hatch_odoo/metadata_hook.py` & `hatch_odoo-1.0/src/hatch_odoo/metadata_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/tests/test_build.py` & `hatch_odoo-1.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/tests/test_editable.py` & `hatch_odoo-1.0/tests/test_editable.py`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/tests/test_metadata.py` & `hatch_odoo-1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/tests/data/project1/pyproject.toml` & `hatch_odoo-1.0/tests/data/project1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/tests/data/project3/pyproject.toml` & `hatch_odoo-1.0/tests/data/project3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/tests/data/project4/pyproject.toml` & `hatch_odoo-1.0/tests/data/project4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/.gitignore` & `hatch_odoo-1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/LICENSE.txt` & `hatch_odoo-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_odoo-0.1/README.md` & `hatch_odoo-1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 be installed with pip:
 
 - automatically generates dependencies based on Odoo addons manifests,
 - package addons into the odoo/addons namespace independently of the source project
   layout,
 - install the addons in editable mode without fiddling with `--addons-path`,
 
+> 💡 This project is best used when working with end-customer projects. To package
+> individual reusable addons, consider the [whool](https://pypi.org/project/whool)
+> project.
+
 **Table of Contents**
 
 - [hatch-odoo](#hatch-odoo)
   - [Quick start](#quick-start)
   - [Alternative project layouts](#alternative-project-layouts)
   - [License](#license)
 
@@ -32,14 +36,15 @@
 requires = ["hatchling", "hatch-odoo"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MyAwesomeProject"
 version = "1.0"
 readme = "README.md"
+requires-python = ">=3.8"
 # Dependencies are dynamic because they will be generated from Odoo addons manifests.
 dynamic = ["dependencies"]
 
 # Enable the hatch-odoo metadata hook to generate dependencies from addons manifests.
 [tool.hatch.metadata.hooks.odoo-addons-dependencies]
 # Enable the hatch-odoo build hook to package the Odoo addons into odoo/addons.
 [tool.hatch.build.hooks.odoo-addons-dirs]
@@ -49,40 +54,40 @@
 odoo_version_override = "15.0"
 # Let's add additional dependencies that are not declared in addons manifests.
 dependencies = ["click-odoo-contrib"]
 # Our addons are in the project root directory.
 addons_dirs = ["."]
 ```
 
-You can then install it together with its dependencies in a virtual environment with a
-procedure like this:
+You can then install it in editable mode, together with its dependencies in a virtual
+environment with a procedure like this:
 
 ```console
 # python3 -m venv .venv
-# .venv/bin/activate
+# source .venv/bin/activate
 # pip install --upgrade pip setuptools wheel
 # pip install -r https://raw.githubusercontent.com/odoo/odoo/15.0/requirements.txt
 # pip install -e git+https://github.com/odoo/odoo@15.0
 # pip install -e .
 # odoo
 ```
 
 All dependencies (such as OCA addons and external dependencies) declared in your project
 addons manifests will be downloaded and installed from PyPI automatically.
 
-There is no need to configure addons path, since the addons are installed in
+There is no need to configure the Odoo addons path: since addons are installed in
 `odoo/addons`, the regular Python import machinery works out of the box
 
 You can then pin dependencies for reproducibility with `pip freeze` or other tools.
 [pip-deepfreeze](https://pypi.org/project/pip-deepfreeze/) is known to work well with
 git URLs, but other tools such as `pip-tools`, may work as well.
 
 ## Alternative project layouts
 
-Depending on your tastes and requirements, there are several alternative ways to
+Depending on your taste and requirements, there are several alternative ways to
 organize your source code. The test projects in
 [tests/data](https://github.com/acsone/hatch-odoo/tree/main/tests/data) each have a
 README that describe the layout and corresponding tradeoffs, with the corresponding
 `pyproject.toml`.
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hatch_odoo-0.1/PKG-INFO` & `hatch_odoo-1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hatch-odoo
-Version: 0.1
+Version: 1.0
 Summary: A Hatch plugin for Odoo projects.
 Project-URL: Documentation, https://github.com/acsone/hatch-odoo#readme
 Project-URL: Issues, https://github.com/acsone/hatch-odoo/issues
 Project-URL: Source, https://github.com/acsone/hatch-odoo
 Author-email: Stéphane Bidoul <stephane.bidoul@acsone.eu>
-Classifier: Development Status :: 4 - Beta
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Hatch
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Requires-Dist: hatchling>=1.4.1
+Requires-Dist: hatchling!=1.19.0,>=1.4.1
 Requires-Dist: manifestoo-core[metadata]>0.8
 Requires-Dist: tomli; python_version < '3.11'
 Provides-Extra: test
 Requires-Dist: build; extra == 'test'
+Requires-Dist: editables; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # hatch-odoo
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hatch-odoo.svg)](https://pypi.org/project/hatch-odoo)
@@ -36,14 +41,18 @@
 be installed with pip:
 
 - automatically generates dependencies based on Odoo addons manifests,
 - package addons into the odoo/addons namespace independently of the source project
   layout,
 - install the addons in editable mode without fiddling with `--addons-path`,
 
+> 💡 This project is best used when working with end-customer projects. To package
+> individual reusable addons, consider the [whool](https://pypi.org/project/whool)
+> project.
+
 **Table of Contents**
 
 - [hatch-odoo](#hatch-odoo)
   - [Quick start](#quick-start)
   - [Alternative project layouts](#alternative-project-layouts)
   - [License](#license)
 
@@ -58,14 +67,15 @@
 requires = ["hatchling", "hatch-odoo"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MyAwesomeProject"
 version = "1.0"
 readme = "README.md"
+requires-python = ">=3.8"
 # Dependencies are dynamic because they will be generated from Odoo addons manifests.
 dynamic = ["dependencies"]
 
 # Enable the hatch-odoo metadata hook to generate dependencies from addons manifests.
 [tool.hatch.metadata.hooks.odoo-addons-dependencies]
 # Enable the hatch-odoo build hook to package the Odoo addons into odoo/addons.
 [tool.hatch.build.hooks.odoo-addons-dirs]
@@ -75,40 +85,40 @@
 odoo_version_override = "15.0"
 # Let's add additional dependencies that are not declared in addons manifests.
 dependencies = ["click-odoo-contrib"]
 # Our addons are in the project root directory.
 addons_dirs = ["."]
 ```
 
-You can then install it together with its dependencies in a virtual environment with a
-procedure like this:
+You can then install it in editable mode, together with its dependencies in a virtual
+environment with a procedure like this:
 
 ```console
 # python3 -m venv .venv
-# .venv/bin/activate
+# source .venv/bin/activate
 # pip install --upgrade pip setuptools wheel
 # pip install -r https://raw.githubusercontent.com/odoo/odoo/15.0/requirements.txt
 # pip install -e git+https://github.com/odoo/odoo@15.0
 # pip install -e .
 # odoo
 ```
 
 All dependencies (such as OCA addons and external dependencies) declared in your project
 addons manifests will be downloaded and installed from PyPI automatically.
 
-There is no need to configure addons path, since the addons are installed in
+There is no need to configure the Odoo addons path: since addons are installed in
 `odoo/addons`, the regular Python import machinery works out of the box
 
 You can then pin dependencies for reproducibility with `pip freeze` or other tools.
 [pip-deepfreeze](https://pypi.org/project/pip-deepfreeze/) is known to work well with
 git URLs, but other tools such as `pip-tools`, may work as well.
 
 ## Alternative project layouts
 
-Depending on your tastes and requirements, there are several alternative ways to
+Depending on your taste and requirements, there are several alternative ways to
 organize your source code. The test projects in
 [tests/data](https://github.com/acsone/hatch-odoo/tree/main/tests/data) each have a
 README that describe the layout and corresponding tradeoffs, with the corresponding
 `pyproject.toml`.
 
 ## License
```

