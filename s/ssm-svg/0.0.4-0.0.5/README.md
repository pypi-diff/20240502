# Comparing `tmp/ssm_svg-0.0.4.tar.gz` & `tmp/ssm_svg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm_svg-0.0.4.tar", last modified: Thu May  2 19:00:12 2024, max compression
+gzip compressed data, was "ssm_svg-0.0.5.tar", last modified: Thu May  2 20:29:41 2024, max compression
```

## Comparing `ssm_svg-0.0.4.tar` & `ssm_svg-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:12.456330 ssm_svg-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-02 19:00:12.456330 ssm_svg-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:00:12.456330 ssm_svg-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:12.456330 ssm_svg-0.0.4/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/ssm/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:12.456330 ssm_svg-0.0.4/ssm_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-02 19:00:12.000000 ssm_svg-0.0.4/ssm_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 19:00:12.000000 ssm_svg-0.0.4/ssm_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:00:12.000000 ssm_svg-0.0.4/ssm_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 19:00:12.000000 ssm_svg-0.0.4/ssm_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 19:00:12.000000 ssm_svg-0.0.4/ssm_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 19:00:12.000000 ssm_svg-0.0.4/ssm_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:12.456330 ssm_svg-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-02 18:59:49.000000 ssm_svg-0.0.4/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/ssm_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 20:29:41.000000 ssm_svg-0.0.5/ssm_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:29:41.543870 ssm_svg-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-02 20:29:33.000000 ssm_svg-0.0.5/tests/test_ssm.py
```

### Comparing `ssm_svg-0.0.4/LICENSE` & `ssm_svg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm_svg-0.0.4/setup.py` & `ssm_svg-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="ssm-svg",
-    version="0.0.4",
+    version="0.0.5",
     description="SVG spritesheet maker",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/ssm",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

### Comparing `ssm_svg-0.0.4/ssm/ssm.py` & `ssm_svg-0.0.5/ssm/ssm.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pathlib import Path
 from lxml import etree
 import lxml.html
 from lxml.builder import E
 import sys
 import os
 from typing import List
+from .__version__ import __version__
 
 
 SVG_XMLNS = {"xmlns": "http://www.w3.org/2000/svg"}
 
 
 class Sprite:
     """SVG sprite.
@@ -290,35 +291,47 @@
 
     for sprite in spritesheet.sprites:
         print(sprite.id)
 
 
 def _export_sprites(*sprites,
                     show_use: bool,
+                    export_dir: str = "",
                     spritesheet_filename: str) -> None:
     if not os.path.exists(spritesheet_filename):
         raise RuntimeError(f"Spritesheet '{spritesheet_filename}' "
                            "does not exist.")
+    if export_dir != "" and not os.path.isdir(export_dir):
+        raise RuntimeError("The directory specified does not exist.")
 
     sprites = list(sprites)
     spritesheet = Spritesheet(spritesheet_filename)
 
     for sprite in spritesheet.sprites:
-        if sprite.id in sprites:
-            print(sprite.export(show_use=show_use,
-                                spritesheet_filename=spritesheet_filename),
-                  end="")
+        if sprite.id not in sprites:
+            continue
+
+        sprite_data = sprite.export(show_use=show_use,
+                                    spritesheet_filename=spritesheet_filename)
+        if export_dir != "":
+            with open(f"{export_dir}/{sprite.id}.svg", "w") as f:
+                f.write(sprite_data)
+        else:
+            print(sprite_data, end="")
 
 
 def main() -> None:
     """Runs script.
     """
-    parser = ArgumentParser(prog="ssm.py",
+    parser = ArgumentParser(prog="ssm",
                             description=__doc__,
                             formatter_class=RawDescriptionHelpFormatter)
+    parser.add_argument("--version",
+                        action="version",
+                        version=f"%(prog)s {__version__}")
     subparsers = parser.add_subparsers()
 
     parser_create = subparsers.add_parser("create",
                                           description="Create SVG spritesheet",
                                           help="Create SVG spritesheet")
     parser_create.set_defaults(_parser="create")
     parser_create.add_argument("-f",
@@ -384,14 +397,19 @@
                                type=FileType(encoding="UTF-8"),
                                metavar="SPRITESHEET_FILE",
                                help="SVG spritesheet file")
     parser_export.add_argument("--use",
                                "-u",
                                action="store_true",
                                help="Print <use> for HTML")
+    parser_export.add_argument("--dir",
+                               type=str,
+                               metavar="EXPORT_DIR",
+                               default="",
+                               help="Write sprites to directory")
     parser_export.add_argument("sprites",
                                type=str,
                                metavar="SVG_SPRITES",
                                nargs="+",
                                help="SVG sprites")
 
     try:
@@ -416,14 +434,15 @@
             elif args._parser == "list":
                 _list_sprites(spritesheet_filename=(args.f.name
                                                     if args.f is not None
                                                     else ""))
             elif args._parser == "export":
                 _export_sprites(*args.sprites,
                                 show_use=args.use,
+                                export_dir=args.dir,
                                 spritesheet_filename=(args.f.name
                                                       if args.f is not None
                                                       else ""))
         else:
             parser.print_help()
     except RuntimeError as e:
         print(f"ERROR: {e}", file=sys.stderr)
```

### Comparing `ssm_svg-0.0.4/tests/test_ssm.py` & `ssm_svg-0.0.5/tests/test_ssm.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 SPRITESHEET_VOID = f"{ARTIFACT_DIR}/spritesheet_void.svg"
 SPRITESHEET_ONE_SPRITE = f"{ARTIFACT_DIR}/spritesheet_one_sprite.svg"
 SPRITESHEET_TWO_SPRITES = f"{ARTIFACT_DIR}/spritesheet_two_sprites.svg"
 SEARCH_SPRITE = f"{TEST_DIR}/search.svg"
 MENU_SPRITE = f"{TEST_DIR}/menu.svg"
 SEARCH_ID = "search"
 MENU_ID = "menu"
+EXPORTED_SVG = f"{ARTIFACT_DIR}/{SEARCH_ID}.svg"
 
 
 class TestSsm(unittest.TestCase):
     def setUp(self):
         if not os.path.exists(ARTIFACT_DIR):
             os.makedirs(ARTIFACT_DIR)
         shutil.copy(f"{TEST_DIR}/spritesheet_void.svg",
@@ -131,10 +132,29 @@
                                            capture_output=True)
         self.assertTrue(completed_process.returncode == 0,
                         "Failed to export sprite from spritesheet.")
         tree = etree.fromstring(completed_process.stdout)
         self.assertEqual(len(tree.xpath(f"/svg/use[@href='{Path(SPRITESHEET_TWO_SPRITES).name}#{SEARCH_ID}']")), 1,  # noqa
                          "Malformed spritesheet.")
 
+    def test_export_to_file(self):
+        completed_process = subprocess.run(["python",
+                                            "-m",
+                                            "ssm",
+                                            "export",
+                                            "-f",
+                                            f"{SPRITESHEET_TWO_SPRITES}",
+                                            "--dir",
+                                            f"{ARTIFACT_DIR}",
+                                            f"{SEARCH_ID}"])
+        self.assertTrue(completed_process.returncode == 0,
+                        "Failed to export sprite from spritesheet.")
+        self.assertTrue(os.path.isfile(f"{EXPORTED_SVG}"),
+                        "Failed to export sprite as file.")
+        tree = etree.parse(f"{EXPORTED_SVG}")
+        self.assertEqual(len(tree.xpath("/xmlns:svg/xmlns:path",
+                                        namespaces=SVG_XMLNS)), 1,
+                         "Malformed spritesheet.")
+
 
 if __name__ == '__main__':
     unittest.main()
```

