# Comparing `tmp/specifipy-0.2.1.tar.gz` & `tmp/specifipy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specifipy-0.2.1.tar", max compression
+gzip compressed data, was "specifipy-0.3.0.tar", max compression
```

## Comparing `specifipy-0.2.1.tar` & `specifipy-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      787 2024-04-28 19:56:32.102478 specifipy-0.2.1/LICENSE
--rw-r--r--   0        0        0      475 2024-04-29 14:28:56.073415 specifipy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-21 19:38:27.704635 specifipy-0.2.1/specifipy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 21:19:27.669788 specifipy-0.2.1/specifipy/diagram_engines/__init__.py
--rw-r--r--   0        0        0      440 2024-04-29 23:56:13.768169 specifipy-0.2.1/specifipy/diagram_engines/hashable_connection.py
--rw-r--r--   0        0        0        0 2022-11-23 00:36:11.690401 specifipy-0.2.1/specifipy/file_scanners/__init__.py
--rw-r--r--   0        0        0     4196 2024-04-29 23:23:55.544508 specifipy-0.2.1/specifipy/file_scanners/directory_scanner.py
--rw-r--r--   0        0        0        0 2022-11-13 01:23:17.772427 specifipy-0.2.1/specifipy/parsers/__init__.py
--rw-r--r--   0        0        0      159 2022-11-21 19:38:37.871943 specifipy-0.2.1/specifipy/parsers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3232 2024-04-29 23:50:20.980382 specifipy-0.2.1/specifipy/parsers/__pycache__/generic_parser.cpython-310.pyc
--rw-r--r--   0        0        0      656 2022-11-21 21:38:53.247387 specifipy-0.2.1/specifipy/parsers/__pycache__/results.cpython-310.pyc
--rw-r--r--   0        0        0     5253 2024-04-29 23:23:55.532508 specifipy-0.2.1/specifipy/parsers/diagram_generator_d2.py
--rw-r--r--   0        0        0     5572 2024-04-29 14:18:05.944043 specifipy-0.2.1/specifipy/parsers/generic_parser.py
--rw-r--r--   0        0        0      372 2022-11-21 21:26:32.295737 specifipy-0.2.1/specifipy/parsers/results.py
--rw-r--r--   0        0        0        0 2022-11-13 12:43:58.920266 specifipy-0.2.1/specifipy/parsers/structure/__init__.py
--rw-r--r--   0        0        0      169 2022-11-21 19:39:10.949975 specifipy-0.2.1/specifipy/parsers/structure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2751 2024-04-29 23:50:20.980382 specifipy-0.2.1/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc
--rw-r--r--   0        0        0     1946 2024-04-29 14:16:50.909123 specifipy-0.2.1/specifipy/parsers/structure/code_structure_definitions.py
--rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 specifipy-0.2.1/setup.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 specifipy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      787 2024-04-28 19:56:32.102478 specifipy-0.3.0/LICENSE
+-rw-r--r--   0        0        0      475 2024-05-02 16:48:14.108554 specifipy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-21 19:38:27.704635 specifipy-0.3.0/specifipy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:19:27.669788 specifipy-0.3.0/specifipy/diagram_engines/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-29 23:56:13.768169 specifipy-0.3.0/specifipy/diagram_engines/hashable_connection.py
+-rw-r--r--   0        0        0        0 2022-11-23 00:36:11.690401 specifipy-0.3.0/specifipy/file_scanners/__init__.py
+-rw-r--r--   0        0        0     4629 2024-05-02 16:47:34.220242 specifipy-0.3.0/specifipy/file_scanners/directory_scanner.py
+-rw-r--r--   0        0        0        0 2022-11-13 01:23:17.772427 specifipy-0.3.0/specifipy/parsers/__init__.py
+-rw-r--r--   0        0        0      159 2022-11-21 19:38:37.871943 specifipy-0.3.0/specifipy/parsers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6145 2024-05-02 16:48:31.092880 specifipy-0.3.0/specifipy/parsers/__pycache__/generic_parser.cpython-310.pyc
+-rw-r--r--   0        0        0      764 2024-05-02 16:48:31.092880 specifipy-0.3.0/specifipy/parsers/__pycache__/results.cpython-310.pyc
+-rw-r--r--   0        0        0     5865 2024-05-02 16:47:34.220242 specifipy-0.3.0/specifipy/parsers/diagram_generator_d2.py
+-rw-r--r--   0        0        0    10032 2024-05-02 16:47:34.220242 specifipy-0.3.0/specifipy/parsers/generic_parser.py
+-rw-r--r--   0        0        0      464 2024-05-02 16:47:34.220242 specifipy-0.3.0/specifipy/parsers/results.py
+-rw-r--r--   0        0        0        0 2022-11-13 12:43:58.920266 specifipy-0.3.0/specifipy/parsers/structure/__init__.py
+-rw-r--r--   0        0        0      169 2022-11-21 19:39:10.949975 specifipy-0.3.0/specifipy/parsers/structure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2874 2024-05-02 16:48:31.092880 specifipy-0.3.0/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc
+-rw-r--r--   0        0        0     2010 2024-05-02 16:47:34.220242 specifipy-0.3.0/specifipy/parsers/structure/code_structure_definitions.py
+-rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 specifipy-0.3.0/setup.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 specifipy-0.3.0/PKG-INFO
```

### Comparing `specifipy-0.2.1/LICENSE` & `specifipy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `specifipy-0.2.1/specifipy/file_scanners/directory_scanner.py` & `specifipy-0.3.0/specifipy/file_scanners/directory_scanner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import os
+from enum import Enum
 
 from py_d2 import D2Diagram
 
 from specifipy.diagram_engines.hashable_connection import D2HashableConnection
 from specifipy.parsers.diagram_generator_d2 import DiagramGenerator
+from specifipy.parsers.generic_parser import FileType
 
 
 class DirectoryScanner:
     scan_path: str = None
     full_dir_paths: list[str] = []
     full_file_paths: list[str] = []
+    file_type: FileType = FileType.PYTHON
+
+    file_extension_mapping: dict[str, str] = {"python": "py", "java": "java"}
 
     def __matches_file_classification(self, full_file_path) -> bool:
         file_name = full_file_path.split("/")[-1]
+        expected_file_type_expression_length = (
+            len(self.file_extension_mapping[self.file_type.value]) + 1
+        )
         return (
             os.path.isfile(full_file_path)
             and file_name[0] != "."
-            and file_name[-3:] == ".py"
+            and file_name[-expected_file_type_expression_length:]
+            == f".{self.file_extension_mapping[self.file_type.value]}"
         )
 
     def __matches_directory_classification(self, full_dir_path) -> bool:
         dir_name: str = full_dir_path.split("/")[-1]
         return (
             os.path.isdir(full_dir_path)
             and dir_name[0] != "."
             and not "venv" in dir_name
             and not "virtualenv" in dir_name
         )
 
-    def __init__(self, base_path: str):
+    def __init__(self, base_path: str, file_type: FileType = FileType.PYTHON):
+        self.file_type = file_type
         self.scan_path = os.path.abspath(base_path)
         for obj in os.listdir(self.scan_path):
             os.path.join(self.scan_path, obj)
         file_system_element: str
 
         # Perform initial directories scanning
         self.full_dir_paths = [
@@ -50,30 +60,27 @@
             if self.__matches_file_classification(
                 os.path.join(self.scan_path, file_system_element)
             )
         ]
 
         self.do_recursive_directory_scanning()
 
-    def show_vars(self):
-        print(self.full_dir_paths, self.full_file_paths)
-
     def make_diagrams(
         self,
         collect_files=True,
-        file_name_containers=False,
+        file_name_containers: bool = False,
         base_path: str | None = None,
     ):
-        diagram_generator = DiagramGenerator()
+        diagram_generator = DiagramGenerator(self.file_type)
         diagrams: list[D2Diagram] = []
         for f in self.full_file_paths:
             name = f.split("/")[-1]
-            with open(f) as python_file:
+            with open(f) as code_file:
                 diagram = diagram_generator.generate_diagram(
-                    python_file.read(),
+                    code_file.read(),
                     name,
                     base_path=base_path,
                     save_file=not collect_files,
                     file_name_container=file_name_containers,
                 )
                 if collect_files and diagram:
                     diagrams.append(diagram)
```

### Comparing `specifipy-0.2.1/specifipy/parsers/__pycache__/results.cpython-310.pyc` & `specifipy-0.3.0/specifipy/parsers/__pycache__/results.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Nov 21 21:26:32 2022 UTC, .py size: 372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,48 @@
-00000000: 6f0d 0d0a 0000 0000 08ed 7b63 7401 0000  o.........{ct...
+00000000: 6f0d 0d0a 0000 0000 eede 3266 d001 0000  o.........2f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
+00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 6d04 5a04 0100 6500 6a05 4700  m.Z.m.Z...e.j.G.
-00000050: 6403 6404 8400 6404 8302 8301 5a06 6401  d.d...d.....Z.d.
-00000060: 5300 2905 e900 0000 004e 2903 da18 436c  S.)......N)...Cl
-00000070: 6173 7353 7472 7563 7475 7265 4465 6669  assStructureDefi
-00000080: 6e69 7469 6f6e da18 4669 656c 6453 7472  nition..FieldStr
-00000090: 7563 7475 7265 4465 6669 6e69 7469 6f6e  uctureDefinition
-000000a0: da1b 4675 6e63 7469 6f6e 5374 7275 6374  ..FunctionStruct
-000000b0: 7572 6544 6566 696e 6974 696f 6e63 0000  ureDefinitionc..
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000000d0: 0000 4000 0000 7332 0000 0065 005a 0164  ..@...s2...e.Z.d
-000000e0: 005a 0255 0065 0365 0419 0065 0564 013c  .Z.U.e.e...e.d.<
-000000f0: 0065 0365 0619 0065 0564 023c 0065 0365  .e.e...e.d.<.e.e
-00000100: 0719 0065 0564 033c 0064 0453 0029 05da  ...e.d.<.d.S.)..
-00000110: 0d50 6172 7369 6e67 5265 7375 6c74 da07  .ParsingResult..
-00000120: 636c 6173 7365 73da 0966 756e 6374 696f  classes..functio
-00000130: 6e73 da0c 636c 6173 735f 6669 656c 6473  ns..class_fields
-00000140: 4e29 08da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000150: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000160: 6c6e 616d 655f 5fda 046c 6973 7472 0200  lname__..listr..
-00000170: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
-00000180: 735f 5f72 0400 0000 7203 0000 00a9 0072  s__r....r......r
-00000190: 0e00 0000 720e 0000 00fa 452f 686f 6d65  ....r.....E/home
-000001a0: 2f6e 6574 7361 7461 6e2f 5079 6368 6172  /netsatan/Pychar
-000001b0: 6d50 726f 6a65 6374 732f 7370 6563 6966  mProjects/specif
-000001c0: 6970 792f 7370 6563 6966 6970 792f 7061  ipy/specifipy/pa
-000001d0: 7273 6572 732f 7265 7375 6c74 732e 7079  rsers/results.py
-000001e0: 7205 0000 000a 0000 0073 0800 0000 0a00  r........s......
-000001f0: 0c02 0c01 1001 7205 0000 0029 07da 0b64  ......r....)...d
-00000200: 6174 6163 6c61 7373 6573 da36 7370 6563  ataclasses.6spec
-00000210: 6966 6970 792e 7061 7273 6572 732e 7374  ifipy.parsers.st
-00000220: 7275 6374 7572 652e 636f 6465 5f73 7472  ructure.code_str
-00000230: 7563 7475 7265 5f64 6566 696e 6974 696f  ucture_definitio
-00000240: 6e73 7202 0000 0072 0300 0000 7204 0000  nsr....r....r...
-00000250: 00da 0964 6174 6163 6c61 7373 7205 0000  ...dataclassr...
-00000260: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-00000270: 720f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000280: 0000 0073 0800 0000 0800 1402 0407 1401  ...s............
+00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
+00000050: 6d06 5a06 6d07 5a07 0100 6500 6a08 4700  m.Z.m.Z...e.j.G.
+00000060: 6404 6405 8400 6405 8302 8301 5a09 6401  d.d...d.....Z.d.
+00000070: 5300 2906 e900 0000 004e 2901 da08 4f70  S.)......N)...Op
+00000080: 7469 6f6e 616c 2904 da18 436c 6173 7353  tional)...ClassS
+00000090: 7472 7563 7475 7265 4465 6669 6e69 7469  tructureDefiniti
+000000a0: 6f6e da09 446f 6373 7472 696e 67da 1846  on..Docstring..F
+000000b0: 6965 6c64 5374 7275 6374 7572 6544 6566  ieldStructureDef
+000000c0: 696e 6974 696f 6eda 1b46 756e 6374 696f  inition..Functio
+000000d0: 6e53 7472 7563 7475 7265 4465 6669 6e69  nStructureDefini
+000000e0: 7469 6f6e 6300 0000 0000 0000 0000 0000  tionc...........
+000000f0: 0000 0000 0003 0000 0040 0000 0073 4600  .........@...sF.
+00000100: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000110: 1900 6505 6401 3c00 6503 6506 1900 6505  ..e.d.<.e.e...e.
+00000120: 6402 3c00 6503 6507 1900 6505 6403 3c00  d.<.e.e...e.d.<.
+00000130: 6404 5a08 6509 6503 650a 1900 1900 6505  d.Z.e.e.e.....e.
+00000140: 6405 3c00 6404 5300 2906 da0d 5061 7273  d.<.d.S.)...Pars
+00000150: 696e 6752 6573 756c 74da 0763 6c61 7373  ingResult..class
+00000160: 6573 da09 6675 6e63 7469 6f6e 73da 0c63  es..functions..c
+00000170: 6c61 7373 5f66 6965 6c64 734e da0a 646f  lass_fieldsN..do
+00000180: 6373 7472 696e 6773 290b da08 5f5f 6e61  cstrings)...__na
+00000190: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000001a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da04  ..__qualname__..
+000001b0: 6c69 7374 7203 0000 00da 0f5f 5f61 6e6e  listr......__ann
+000001c0: 6f74 6174 696f 6e73 5f5f 7206 0000 0072  otations__r....r
+000001d0: 0500 0000 720b 0000 0072 0200 0000 7204  ....r....r....r.
+000001e0: 0000 00a9 0072 1100 0000 7211 0000 00fa  .....r....r.....
+000001f0: 452f 686f 6d65 2f6e 6574 7361 7461 6e2f  E/home/netsatan/
+00000200: 5079 6368 6172 6d50 726f 6a65 6374 732f  PycharmProjects/
+00000210: 7370 6563 6966 6970 792f 7370 6563 6966  specifipy/specif
+00000220: 6970 792f 7061 7273 6572 732f 7265 7375  ipy/parsers/resu
+00000230: 6c74 732e 7079 7207 0000 000c 0000 0073  lts.pyr........s
+00000240: 0a00 0000 0a00 0c02 0c01 0c01 1801 7207  ..............r.
+00000250: 0000 0029 0ada 0b64 6174 6163 6c61 7373  ...)...dataclass
+00000260: 6573 da06 7479 7069 6e67 7202 0000 00da  es..typingr.....
+00000270: 3673 7065 6369 6669 7079 2e70 6172 7365  6specifipy.parse
+00000280: 7273 2e73 7472 7563 7475 7265 2e63 6f64  rs.structure.cod
+00000290: 655f 7374 7275 6374 7572 655f 6465 6669  e_structure_defi
+000002a0: 6e69 7469 6f6e 7372 0300 0000 7204 0000  nitionsr....r...
+000002b0: 0072 0500 0000 7206 0000 00da 0964 6174  .r....r......dat
+000002c0: 6163 6c61 7373 7207 0000 0072 1100 0000  aclassr....r....
+000002d0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+000002e0: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
+000002f0: 0000 0800 0c01 1802 0408 1401            ............
```

### Comparing `specifipy-0.2.1/specifipy/parsers/diagram_generator_d2.py` & `specifipy-0.3.0/specifipy/parsers/diagram_generator_d2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from py_d2 import D2Connection, D2Diagram, D2Shape
+from py_d2 import D2Connection, D2Diagram, D2Shape, Direction
 from py_d2.shape import Shape
 
-from specifipy.parsers.generic_parser import GenericParser
+from specifipy.diagram_engines.hashable_connection import D2HashableConnection
+from specifipy.parsers.generic_parser import FileType, ParserFactory, PythonParser
 from specifipy.parsers.results import ParsingResult
 from specifipy.parsers.structure.code_structure_definitions import (
     ClassStructureDefinition,
     FieldStructureDefinition,
     FunctionStructureDefinition,
     StructureEnum,
     TypeAnnotatedFieldStructureDefinition,
 )
 
 
-class DiagramGenerator(GenericParser):
+class DiagramGenerator:
+    def __init__(self, file_type: FileType = FileType.PYTHON):
+        self.parser = ParserFactory.get_parser(file_type)
+
     def __generate_class_definition_d2(
         self,
         class_element: ClassStructureDefinition,
         fields: list[D2Shape] = None,
         methods: list[D2Shape] = None,
     ) -> D2Shape:
         fields = [] if fields is None else fields
@@ -61,24 +65,25 @@
         self,
         source_file_content: str,
         source_file_name: str,
         base_path: str = None,
         save_file: bool = True,
         file_name_container=False,
     ) -> D2Diagram | None:
-        parsing_result: ParsingResult = self.parse(source_file_content)
+        parsing_result: ParsingResult = self.parser.parse(source_file_content)
         elements_to_generate: list[D2Shape] = []
         link_to_generate: list[D2Connection] = []
 
         class_element: ClassStructureDefinition
+
         for class_element in parsing_result.classes:
             class_functions = [
                 self.__generate_class_function_definition_d2(x)
                 for x in parsing_result.functions
-                if x.parent_class == class_element.name
+                if x.parent_class == class_element
             ]
             class_fields = [
                 self.__generate_field_definition_d2(x)
                 for x in parsing_result.class_fields
                 if x.parent_class == class_element
             ]
             if file_name_container:
@@ -94,14 +99,23 @@
                 if file_name_container:
                     class_element.inherits_from = f'{source_file_name.replace(".", "-")}.{class_element.inherits_from}'
                 link_to_generate.append(
                     D2Connection(
                         shape_1=class_element.name, shape_2=class_element.inherits_from
                     )
                 )
+            if class_element.implements:
+                for interface in class_element.implements:
+                    link_to_generate.append(
+                        D2HashableConnection(
+                            class_element.name,
+                            interface,
+                            "{ style: { stroke-dash: 3 } } ",
+                        )
+                    )
         self.add_missing_elements_from_links_as_classes(
             elements_to_generate, link_to_generate
         )
         diagram = D2Diagram(shapes=elements_to_generate, connections=link_to_generate)
         if str(diagram) is not None and str(diagram) != "":
             if save_file:
                 self.save_diagram_to_file(base_path, diagram, source_file_name)
```

### Comparing `specifipy-0.2.1/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc` & `specifipy-0.3.0/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 29 14:16:50 2024 UTC, .py size: 1946 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d2ab 2f66 9a07 0000  o........./f....
+00000000: 6f0d 0d0a 0000 0000 82bf 3366 da07 0000  o.........3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 4700 6405 6406 8400 6406 8302 5a04  Z.G.d.d...d...Z.
 00000060: 6500 6a05 4700 6407 6408 8400 6408 8302  e.j.G.d.d...d...
 00000070: 8301 5a06 6500 6a05 4700 6409 640a 8400  ..Z.e.j.G.d.d...
@@ -45,128 +45,136 @@
 000002c0: 6174 696f 6e73 5f5f 720f 0000 0072 0f00  ations__r....r..
 000002d0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
 000002e0: 000c 0000 0073 0600 0000 0a00 0801 0c01  .....s..........
 000002f0: 7211 0000 0063 0000 0000 0000 0000 0000  r....c..........
 00000300: 0000 0000 0000 0300 0000 4000 0000 f316  ..........@.....
 00000310: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
 00000320: 0464 013c 0064 0253 0029 03da 0944 6f63  .d.<.d.S.)...Doc
-00000330: 7374 7269 6e67 da0b 6465 7363 7269 7074  string..descript
-00000340: 696f 6e4e 7214 0000 0072 0f00 0000 720f  ionNr....r....r.
-00000350: 0000 0072 0f00 0000 7210 0000 0072 1800  ...r....r....r..
-00000360: 0000 1100 0000 f304 0000 000a 000c 0272  ...............r
-00000370: 1800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000380: 0000 0000 0003 0000 0040 0000 0073 4600  .........@...sF.
-00000390: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-000003a0: 6401 3c00 6505 6504 6402 3c00 6506 6504  d.<.e.e.d.<.e.e.
-000003b0: 6403 3c00 6506 6504 6404 3c00 6700 6405  d.<.e.e.d.<.g.d.
-000003c0: a201 5a07 6406 6407 8400 5a08 6408 6409  ..Z.d.d...Z.d.d.
-000003d0: 8400 5a09 640a 5300 290b da13 5374 7275  ..Z.d.S.)...Stru
-000003e0: 6374 7572 6544 6566 696e 6974 696f 6eda  ctureDefinition.
-000003f0: 0e73 7472 7563 7475 7265 5f74 7970 6572  .structure_typer
-00000400: 1200 0000 da0a 7374 6172 745f 6c69 6e65  ......start_line
-00000410: da08 656e 645f 6c69 6e65 2909 da05 6c61  ..end_line)...la
-00000420: 6265 6cda 0563 6c61 7373 da07 636c 6173  bel..class..clas
-00000430: 7365 73da 0573 7479 6c65 da05 7368 6170  ses..style..shap
-00000440: 65da 0964 6972 6563 7469 6f6e da05 7769  e..direction..wi
-00000450: 6474 68da 0668 6569 6768 74da 046c 696e  dth..height..lin
-00000460: 6b63 0100 0000 0000 0000 0000 0000 0200  kc..............
-00000470: 0000 0200 0000 4300 0000 7328 0000 0064  ......C...s(...d
-00000480: 017d 017c 006a 00a0 01a1 007c 006a 0276  .}.|.j.....|.j.v
-00000490: 0072 127c 006a 007c 0117 007c 005f 0064  .r.|.j.|...|._.d
-000004a0: 0053 0064 0053 0029 024e 7503 0000 00e2  .S.d.S.).Nu.....
-000004b0: a080 2903 7212 0000 00da 056c 6f77 6572  ..).r......lower
-000004c0: da14 6432 5f72 6573 6572 7665 645f 6b65  ..d2_reserved_ke
-000004d0: 7977 6f72 6473 2902 da04 7365 6c66 da13  ywords)...self..
-000004e0: 6b65 7977 6f72 645f 6573 6361 7065 5f63  keyword_escape_c
-000004f0: 6861 7272 0f00 0000 720f 0000 0072 1000  harr....r....r..
-00000500: 0000 da11 7361 6e69 7469 7a65 5f64 325f  ....sanitize_d2_
-00000510: 6e61 6d65 732b 0000 0073 0800 0000 0401  names+...s......
-00000520: 1001 1001 04ff 7a25 5374 7275 6374 7572  ......z%Structur
-00000530: 6544 6566 696e 6974 696f 6e2e 7361 6e69  eDefinition.sani
-00000540: 7469 7a65 5f64 325f 6e61 6d65 7363 0100  tize_d2_namesc..
-00000550: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000560: 0000 4300 0000 730c 0000 007c 00a0 00a1  ..C...s....|....
-00000570: 0001 0064 0053 00a9 014e 2901 722c 0000  ...d.S...N).r,..
-00000580: 0029 0172 2a00 0000 720f 0000 0072 0f00  .).r*...r....r..
-00000590: 0000 7210 0000 00da 0d5f 5f70 6f73 745f  ..r......__post_
-000005a0: 696e 6974 5f5f 3000 0000 7302 0000 000c  init__0...s.....
-000005b0: 017a 2153 7472 7563 7475 7265 4465 6669  .z!StructureDefi
-000005c0: 6e69 7469 6f6e 2e5f 5f70 6f73 745f 696e  nition.__post_in
-000005d0: 6974 5f5f 4e29 0a72 0800 0000 7209 0000  it__N).r....r...
-000005e0: 0072 0a00 0000 7203 0000 0072 1600 0000  .r....r....r....
-000005f0: 7215 0000 00da 0369 6e74 7229 0000 0072  r......intr)...r
-00000600: 2c00 0000 722e 0000 0072 0f00 0000 720f  ,...r....r....r.
-00000610: 0000 0072 0f00 0000 7210 0000 0072 1b00  ...r....r....r..
-00000620: 0000 1600 0000 7310 0000 000a 0008 0208  ......s.........
-00000630: 0108 0108 0108 0308 0d0c 0572 1b00 0000  ...........r....
-00000640: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000650: 0003 0000 0040 0000 0072 1700 0000 2903  .....@...r....).
-00000660: da18 436c 6173 7353 7472 7563 7475 7265  ..ClassStructure
-00000670: 4465 6669 6e69 7469 6f6e da0d 696e 6865  Definition..inhe
-00000680: 7269 7473 5f66 726f 6d4e 7214 0000 0072  rits_fromNr....r
-00000690: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-000006a0: 0000 0072 3000 0000 3400 0000 721a 0000  ...r0...4...r...
-000006b0: 0072 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
-000006c0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000006d0: 3600 0000 6500 5a01 6400 5a02 5500 6503  6...e.Z.d.Z.U.e.
-000006e0: 6504 1900 6505 6401 3c00 6506 6505 6402  e...e.d.<.e.e.d.
-000006f0: 3c00 6403 5a07 6504 6505 6404 3c00 6405  <.d.Z.e.e.d.<.d.
-00000700: 6406 8400 5a08 6403 5300 2907 da1b 4675  d...Z.d.S.)...Fu
-00000710: 6e63 7469 6f6e 5374 7275 6374 7572 6544  nctionStructureD
-00000720: 6566 696e 6974 696f 6eda 0670 6172 616d  efinition..param
-00000730: 73da 0c70 6172 656e 745f 636c 6173 734e  s..parent_classN
-00000740: da0b 7265 7475 726e 5f74 7970 6563 0200  ..return_typec..
-00000750: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00000760: 0000 4300 0000 7330 0000 007c 006a 007c  ..C...s0...|.j.|
-00000770: 006a 017c 006a 027c 006a 037c 006a 0466  .j.|.j.|.j.|.j.f
-00000780: 057c 016a 007c 016a 017c 016a 027c 016a  .|.j.|.j.|.j.|.j
-00000790: 037c 016a 0466 056b 0253 0072 2d00 0000  .|.j.f.k.S.r-...
-000007a0: 2905 7212 0000 0072 3300 0000 721d 0000  ).r....r3...r...
-000007b0: 0072 1e00 0000 721c 0000 0029 0272 2a00  .r....r....).r*.
-000007c0: 0000 da05 6f74 6865 7272 0f00 0000 720f  ....otherr....r.
-000007d0: 0000 0072 1000 0000 da06 5f5f 6571 5f5f  ...r......__eq__
-000007e0: 3f00 0000 731a 0000 0004 0204 0104 0104  ?...s...........
-000007f0: 0104 0102 fb04 0704 0104 0104 0104 0102  ................
-00000800: fb04 fa7a 2246 756e 6374 696f 6e53 7472  ...z"FunctionStr
-00000810: 7563 7475 7265 4465 6669 6e69 7469 6f6e  uctureDefinition
-00000820: 2e5f 5f65 715f 5f29 0972 0800 0000 7209  .__eq__).r....r.
-00000830: 0000 0072 0a00 0000 da04 6c69 7374 7215  ...r......listr.
-00000840: 0000 0072 1600 0000 7230 0000 0072 3500  ...r....r0...r5.
-00000850: 0000 7237 0000 0072 0f00 0000 720f 0000  ..r7...r....r...
-00000860: 0072 0f00 0000 7210 0000 0072 3200 0000  .r....r....r2...
-00000870: 3900 0000 730a 0000 000a 000c 0208 010c  9...s...........
-00000880: 010c 0272 3200 0000 6300 0000 0000 0000  ...r2...c.......
-00000890: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000008a0: 0072 1700 0000 2903 da18 4669 656c 6453  .r....)...FieldS
-000008b0: 7472 7563 7475 7265 4465 6669 6e69 7469  tructureDefiniti
-000008c0: 6f6e 7234 0000 004e 2905 7208 0000 0072  onr4...N).r....r
-000008d0: 0900 0000 720a 0000 0072 3000 0000 7216  ....r....r0...r.
-000008e0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-000008f0: 0000 7210 0000 0072 3900 0000 4f00 0000  ..r....r9...O...
-00000900: 721a 0000 0072 3900 0000 6300 0000 0000  r....r9...c.....
-00000910: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000920: 0000 0072 1700 0000 2903 da25 5479 7065  ...r....)..%Type
-00000930: 416e 6e6f 7461 7465 6446 6965 6c64 5374  AnnotatedFieldSt
-00000940: 7275 6374 7572 6544 6566 696e 6974 696f  ructureDefinitio
-00000950: 6eda 0f74 7970 655f 616e 6e6f 7461 7469  n..type_annotati
-00000960: 6f6e 4e72 1400 0000 720f 0000 0072 0f00  onNr....r....r..
-00000970: 0000 720f 0000 0072 1000 0000 723a 0000  ..r....r....r:..
-00000980: 0054 0000 0072 1a00 0000 723a 0000 0063  .T...r....r:...c
-00000990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009a0: 0100 0000 4000 0000 730c 0000 0065 005a  ....@...s....e.Z
-000009b0: 0164 005a 0264 0153 0029 02da 284e 6f74  .d.Z.d.S.)..(Not
-000009c0: 5479 7065 416e 6e6f 7461 7465 6446 6965  TypeAnnotatedFie
-000009d0: 6c64 5374 7275 6374 7572 6544 6566 696e  ldStructureDefin
-000009e0: 6974 696f 6e4e 2903 7208 0000 0072 0900  itionN).r....r..
-000009f0: 0000 720a 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000a00: 0072 0f00 0000 7210 0000 0072 3c00 0000  .r....r....r<...
-00000a10: 5900 0000 7304 0000 0008 0004 0272 3c00  Y...s........r<.
-00000a20: 0000 290d da0b 6461 7461 636c 6173 7365  ..)...dataclasse
-00000a30: 73da 0465 6e75 6d72 0200 0000 7203 0000  s..enumr....r...
-00000a40: 0072 1100 0000 da09 6461 7461 636c 6173  .r......dataclas
-00000a50: 7372 1800 0000 721b 0000 0072 3000 0000  sr....r....r0...
-00000a60: 7232 0000 0072 3900 0000 723a 0000 0072  r2...r9...r:...r
-00000a70: 3c00 0000 720f 0000 0072 0f00 0000 720f  <...r....r....r.
-00000a80: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000a90: 653e 0100 0000 7324 0000 0008 000c 0110  e>....s$........
-00000aa0: 030e 0704 0510 0104 0410 0104 1d12 0104  ................
-00000ab0: 0412 0104 1512 0104 0412 0104 0416 01    ...............
+00000330: 7374 7269 6e67 da07 636f 6e74 656e 744e  string..contentN
+00000340: 7214 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000350: 0f00 0000 7210 0000 0072 1800 0000 1100  ....r....r......
+00000360: 0000 f304 0000 000a 000c 0272 1800 0000  ...........r....
+00000370: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000380: 0003 0000 0040 0000 0073 4600 0000 6500  .....@...sF...e.
+00000390: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+000003a0: 6505 6504 6402 3c00 6506 6504 6403 3c00  e.e.d.<.e.e.d.<.
+000003b0: 6506 6504 6404 3c00 6700 6405 a201 5a07  e.e.d.<.g.d...Z.
+000003c0: 6406 6407 8400 5a08 6408 6409 8400 5a09  d.d...Z.d.d...Z.
+000003d0: 640a 5300 290b da13 5374 7275 6374 7572  d.S.)...Structur
+000003e0: 6544 6566 696e 6974 696f 6eda 0e73 7472  eDefinition..str
+000003f0: 7563 7475 7265 5f74 7970 6572 1200 0000  ucture_typer....
+00000400: da0a 7374 6172 745f 6c69 6e65 da08 656e  ..start_line..en
+00000410: 645f 6c69 6e65 2909 da05 6c61 6265 6cda  d_line)...label.
+00000420: 0563 6c61 7373 da07 636c 6173 7365 73da  .class..classes.
+00000430: 0573 7479 6c65 da05 7368 6170 65da 0964  .style..shape..d
+00000440: 6972 6563 7469 6f6e da05 7769 6474 68da  irection..width.
+00000450: 0668 6569 6768 74da 046c 696e 6b63 0100  .height..linkc..
+00000460: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000470: 0000 4300 0000 7328 0000 0064 017d 017c  ..C...s(...d.}.|
+00000480: 006a 00a0 01a1 007c 006a 0276 0072 127c  .j.....|.j.v.r.|
+00000490: 006a 007c 0117 007c 005f 0064 0053 0064  .j.|...|._.d.S.d
+000004a0: 0053 0029 024e 7503 0000 00e2 a080 2903  .S.).Nu.......).
+000004b0: 7212 0000 00da 056c 6f77 6572 da14 6432  r......lower..d2
+000004c0: 5f72 6573 6572 7665 645f 6b65 7977 6f72  _reserved_keywor
+000004d0: 6473 2902 da04 7365 6c66 da13 6b65 7977  ds)...self..keyw
+000004e0: 6f72 645f 6573 6361 7065 5f63 6861 7272  ord_escape_charr
+000004f0: 0f00 0000 720f 0000 0072 1000 0000 da11  ....r....r......
+00000500: 7361 6e69 7469 7a65 5f64 325f 6e61 6d65  sanitize_d2_name
+00000510: 732b 0000 0073 0800 0000 0401 1001 1001  s+...s..........
+00000520: 04ff 7a25 5374 7275 6374 7572 6544 6566  ..z%StructureDef
+00000530: 696e 6974 696f 6e2e 7361 6e69 7469 7a65  inition.sanitize
+00000540: 5f64 325f 6e61 6d65 7363 0100 0000 0000  _d2_namesc......
+00000550: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000560: 0000 730c 0000 007c 00a0 00a1 0001 0064  ..s....|.......d
+00000570: 0053 00a9 014e 2901 722c 0000 0029 0172  .S...N).r,...).r
+00000580: 2a00 0000 720f 0000 0072 0f00 0000 7210  *...r....r....r.
+00000590: 0000 00da 0d5f 5f70 6f73 745f 696e 6974  .....__post_init
+000005a0: 5f5f 3000 0000 7302 0000 000c 017a 2153  __0...s......z!S
+000005b0: 7472 7563 7475 7265 4465 6669 6e69 7469  tructureDefiniti
+000005c0: 6f6e 2e5f 5f70 6f73 745f 696e 6974 5f5f  on.__post_init__
+000005d0: 4e29 0a72 0800 0000 7209 0000 0072 0a00  N).r....r....r..
+000005e0: 0000 7203 0000 0072 1600 0000 7215 0000  ..r....r....r...
+000005f0: 00da 0369 6e74 7229 0000 0072 2c00 0000  ...intr)...r,...
+00000600: 722e 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000610: 0f00 0000 7210 0000 0072 1b00 0000 1600  ....r....r......
+00000620: 0000 7310 0000 000a 0008 0208 0108 0108  ..s.............
+00000630: 0108 0308 0d0c 0572 1b00 0000 6300 0000  .......r....c...
+00000640: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000650: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000660: 5a02 5500 6503 6504 6401 3c00 6505 6a06  Z.U.e.e.d.<.e.j.
+00000670: 6507 6402 8d01 5a08 6507 6503 1900 6504  e.d...Z.e.e...e.
+00000680: 6403 3c00 6404 5300 2905 da18 436c 6173  d.<.d.S.)...Clas
+00000690: 7353 7472 7563 7475 7265 4465 6669 6e69  sStructureDefini
+000006a0: 7469 6f6e da0d 696e 6865 7269 7473 5f66  tion..inherits_f
+000006b0: 726f 6d29 01da 0f64 6566 6175 6c74 5f66  rom)...default_f
+000006c0: 6163 746f 7279 da0a 696d 706c 656d 656e  actory..implemen
+000006d0: 7473 4e29 0972 0800 0000 7209 0000 0072  tsN).r....r....r
+000006e0: 0a00 0000 7215 0000 0072 1600 0000 da0b  ....r....r......
+000006f0: 6461 7461 636c 6173 7365 73da 0566 6965  dataclasses..fie
+00000700: 6c64 da04 6c69 7374 7233 0000 0072 0f00  ld..listr3...r..
+00000710: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000720: 0072 3000 0000 3400 0000 7306 0000 000a  .r0...4...s.....
+00000730: 0008 021c 0172 3000 0000 6300 0000 0000  .....r0...c.....
+00000740: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000750: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
+00000760: 5500 6503 6504 1900 6505 6401 3c00 6506  U.e.e...e.d.<.e.
+00000770: 6505 6402 3c00 6403 5a07 6504 6505 6404  e.d.<.d.Z.e.e.d.
+00000780: 3c00 6405 6406 8400 5a08 6403 5300 2907  <.d.d...Z.d.S.).
+00000790: da1b 4675 6e63 7469 6f6e 5374 7275 6374  ..FunctionStruct
+000007a0: 7572 6544 6566 696e 6974 696f 6eda 0670  ureDefinition..p
+000007b0: 6172 616d 73da 0c70 6172 656e 745f 636c  arams..parent_cl
+000007c0: 6173 734e da0b 7265 7475 726e 5f74 7970  assN..return_typ
+000007d0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+000007e0: 0000 0600 0000 4300 0000 7330 0000 007c  ......C...s0...|
+000007f0: 006a 007c 006a 017c 006a 027c 006a 037c  .j.|.j.|.j.|.j.|
+00000800: 006a 0466 057c 016a 007c 016a 017c 016a  .j.f.|.j.|.j.|.j
+00000810: 027c 016a 037c 016a 0466 056b 0253 0072  .|.j.|.j.f.k.S.r
+00000820: 2d00 0000 2905 7212 0000 0072 3800 0000  -...).r....r8...
+00000830: 721d 0000 0072 1e00 0000 721c 0000 0029  r....r....r....)
+00000840: 0272 2a00 0000 da05 6f74 6865 7272 0f00  .r*.....otherr..
+00000850: 0000 720f 0000 0072 1000 0000 da06 5f5f  ..r....r......__
+00000860: 6571 5f5f 4000 0000 731a 0000 0004 0204  eq__@...s.......
+00000870: 0104 0104 0104 0102 fb04 0704 0104 0104  ................
+00000880: 0104 0102 fb04 fa7a 2246 756e 6374 696f  .......z"Functio
+00000890: 6e53 7472 7563 7475 7265 4465 6669 6e69  nStructureDefini
+000008a0: 7469 6f6e 2e5f 5f65 715f 5f29 0972 0800  tion.__eq__).r..
+000008b0: 0000 7209 0000 0072 0a00 0000 7236 0000  ..r....r....r6..
+000008c0: 0072 1500 0000 7216 0000 0072 3000 0000  .r....r....r0...
+000008d0: 723a 0000 0072 3c00 0000 720f 0000 0072  r:...r<...r....r
+000008e0: 0f00 0000 720f 0000 0072 1000 0000 7237  ....r....r....r7
+000008f0: 0000 003a 0000 0073 0a00 0000 0a00 0c02  ...:...s........
+00000900: 0801 0c01 0c02 7237 0000 0063 0000 0000  ......r7...c....
+00000910: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000920: 4000 0000 7217 0000 0029 03da 1846 6965  @...r....)...Fie
+00000930: 6c64 5374 7275 6374 7572 6544 6566 696e  ldStructureDefin
+00000940: 6974 696f 6e72 3900 0000 4e29 0572 0800  itionr9...N).r..
+00000950: 0000 7209 0000 0072 0a00 0000 7230 0000  ..r....r....r0..
+00000960: 0072 1600 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00000970: 720f 0000 0072 1000 0000 723d 0000 0050  r....r....r=...P
+00000980: 0000 0072 1a00 0000 723d 0000 0063 0000  ...r....r=...c..
+00000990: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000009a0: 0000 4000 0000 7217 0000 0029 03da 2554  ..@...r....)..%T
+000009b0: 7970 6541 6e6e 6f74 6174 6564 4669 656c  ypeAnnotatedFiel
+000009c0: 6453 7472 7563 7475 7265 4465 6669 6e69  dStructureDefini
+000009d0: 7469 6f6e da0f 7479 7065 5f61 6e6e 6f74  tion..type_annot
+000009e0: 6174 696f 6e4e 7214 0000 0072 0f00 0000  ationNr....r....
+000009f0: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000a00: 3e00 0000 5500 0000 721a 0000 0072 3e00  >...U...r....r>.
+00000a10: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000a20: 0000 0001 0000 0040 0000 0073 0c00 0000  .......@...s....
+00000a30: 6500 5a01 6400 5a02 6401 5300 2902 da28  e.Z.d.Z.d.S.)..(
+00000a40: 4e6f 7454 7970 6541 6e6e 6f74 6174 6564  NotTypeAnnotated
+00000a50: 4669 656c 6453 7472 7563 7475 7265 4465  FieldStructureDe
+00000a60: 6669 6e69 7469 6f6e 4e29 0372 0800 0000  finitionN).r....
+00000a70: 7209 0000 0072 0a00 0000 720f 0000 0072  r....r....r....r
+00000a80: 0f00 0000 720f 0000 0072 1000 0000 7240  ....r....r....r@
+00000a90: 0000 005a 0000 0073 0400 0000 0800 0402  ...Z...s........
+00000aa0: 7240 0000 0029 0d72 3400 0000 da04 656e  r@...).r4.....en
+00000ab0: 756d 7202 0000 0072 0300 0000 7211 0000  umr....r....r...
+00000ac0: 00da 0964 6174 6163 6c61 7373 7218 0000  ...dataclassr...
+00000ad0: 0072 1b00 0000 7230 0000 0072 3700 0000  .r....r0...r7...
+00000ae0: 723d 0000 0072 3e00 0000 7240 0000 0072  r=...r>...r@...r
+00000af0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00000b00: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000b10: 0073 2400 0000 0800 0c01 1003 0e07 0405  .s$.............
+00000b20: 1001 0404 1001 041d 1201 0405 1201 0415  ................
+00000b30: 1201 0404 1201 0404 1601                 ..........
```

### Comparing `specifipy-0.2.1/specifipy/parsers/structure/code_structure_definitions.py` & `specifipy-0.3.0/specifipy/parsers/structure/code_structure_definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class ParamDefinition:
     name: str
     type: str
 
 
 @dataclasses.dataclass
 class Docstring:
-    description: str
+    content: str
 
 
 @dataclasses.dataclass
 class StructureDefinition:
     structure_type: StructureEnum
     name: str
     start_line: int
@@ -48,14 +48,15 @@
     def __post_init__(self):
         self.sanitize_d2_names()
 
 
 @dataclasses.dataclass
 class ClassStructureDefinition(StructureDefinition):
     inherits_from: str
+    implements: list[str] = dataclasses.field(default_factory=list)
 
 
 @dataclasses.dataclass
 class FunctionStructureDefinition(StructureDefinition):
     params: list[str]
     parent_class: ClassStructureDefinition
     return_type: str = None
```

### Comparing `specifipy-0.2.1/setup.py` & `specifipy-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {'': ['*']}
 
 install_requires = \
 ['docstring-parser>=0.15,<0.16', 'py-d2==1.0.0', 'snakemd>=0.11.0,<0.12.0']
 
 setup_kwargs = {
     'name': 'specifipy',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Python package for auto-generating code diagrams',
     'long_description': 'None',
     'author': 'Bartosz Budzyński',
     'author_email': 'hi@bartosz.blog',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `specifipy-0.2.1/PKG-INFO` & `specifipy-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specifipy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python package for auto-generating code diagrams
 Author: Bartosz Budzyński
 Author-email: hi@bartosz.blog
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

