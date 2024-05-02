# Comparing `tmp/pylammpstrj-1.0.3rc0.tar.gz` & `tmp/pylammpstrj-1.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpstrj-1.0.3rc0.tar", last modified: Wed Jan 17 15:29:46 2024, max compression
+gzip compressed data, was "pylammpstrj-1.0.4a0.tar", last modified: Thu May  2 13:31:46 2024, max compression
```

## Comparing `pylammpstrj-1.0.3rc0.tar` & `pylammpstrj-1.0.4a0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxr-x   0 heiarii   (1000) heiarii   (1000)        0 2024-01-17 15:29:46.897281 pylammpstrj-1.0.3rc0/
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)    35149 2024-01-05 11:49:05.000000 pylammpstrj-1.0.3rc0/LICENSE
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)       90 2024-01-10 07:56:02.000000 pylammpstrj-1.0.3rc0/MANIFEST.in
--rw-r--r--   0 heiarii   (1000) heiarii   (1000)    42831 2024-01-17 15:29:46.897281 pylammpstrj-1.0.3rc0/PKG-INFO
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     1661 2024-01-05 11:49:05.000000 pylammpstrj-1.0.3rc0/README.md
-drwxrwxr-x   0 heiarii   (1000) heiarii   (1000)        0 2024-01-17 15:29:46.893281 pylammpstrj-1.0.3rc0/pylammpstrj/
-drwxrwxr-x   0 heiarii   (1000) heiarii   (1000)        0 2024-01-17 15:29:46.897281 pylammpstrj-1.0.3rc0/pylammpstrj/include/
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     2376 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/atom.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      717 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/box.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     1302 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/pyatom.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      682 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/pybox.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      296 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/pylammpstrjmodule.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     3848 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/pytrajectory.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      381 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/pyutils.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      890 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/read.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     3730 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/trajectory.h
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      561 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/include/utils.h
-drwxrwxr-x   0 heiarii   (1000) heiarii   (1000)        0 2024-01-17 15:29:46.897281 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)    11791 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/atom.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     8313 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/average.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      579 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/box.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)    18526 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/read.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)    11607 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/select.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     1941 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/skip.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     1497 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/trajectory.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     5425 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/trajectoryfile.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      250 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/utils.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     5074 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/pyatom.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     2003 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/pybox.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     4234 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/pylammpstrjmodule.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)    10481 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/pytrajectory.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     7436 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/pytrajectoryfile.c
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)     2143 2024-01-17 15:28:21.000000 pylammpstrj-1.0.3rc0/pylammpstrj/pyutils.c
-drwxrwxr-x   0 heiarii   (1000) heiarii   (1000)        0 2024-01-17 15:29:46.897281 pylammpstrj-1.0.3rc0/pylammpstrj.egg-info/
--rw-r--r--   0 heiarii   (1000) heiarii   (1000)    42831 2024-01-17 15:29:46.000000 pylammpstrj-1.0.3rc0/pylammpstrj.egg-info/PKG-INFO
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      931 2024-01-17 15:29:46.000000 pylammpstrj-1.0.3rc0/pylammpstrj.egg-info/SOURCES.txt
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)        1 2024-01-17 15:29:46.000000 pylammpstrj-1.0.3rc0/pylammpstrj.egg-info/dependency_links.txt
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)       12 2024-01-17 15:29:46.000000 pylammpstrj-1.0.3rc0/pylammpstrj.egg-info/top_level.txt
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      733 2024-01-17 15:29:35.000000 pylammpstrj-1.0.3rc0/pyproject.toml
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)       38 2024-01-17 15:29:46.897281 pylammpstrj-1.0.3rc0/setup.cfg
--rw-rw-r--   0 heiarii   (1000) heiarii   (1000)      972 2024-01-17 15:28:46.000000 pylammpstrj-1.0.3rc0/setup.py
+drwxrwxr-x   0 louchao   (1002) louchao   (1002)        0 2024-05-02 13:31:46.606336 pylammpstrj-1.0.4a0/
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)    35149 2024-01-05 13:30:57.000000 pylammpstrj-1.0.4a0/LICENSE
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)       36 2024-03-28 10:43:20.000000 pylammpstrj-1.0.4a0/MANIFEST.in
+-rw-r--r--   0 louchao   (1002) louchao   (1002)    42830 2024-05-02 13:31:46.606336 pylammpstrj-1.0.4a0/PKG-INFO
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     1661 2024-01-05 13:30:57.000000 pylammpstrj-1.0.4a0/README.md
+drwxrwxr-x   0 louchao   (1002) louchao   (1002)        0 2024-05-02 13:31:46.602336 pylammpstrj-1.0.4a0/include/
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     2651 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/atom.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     2475 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/bond.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      717 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/box.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     1302 2024-05-02 13:28:28.000000 pylammpstrj-1.0.4a0/include/pyatom.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      378 2024-05-02 13:28:28.000000 pylammpstrj-1.0.4a0/include/pybond.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      682 2024-05-02 13:28:28.000000 pylammpstrj-1.0.4a0/include/pybox.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      296 2024-05-02 13:28:28.000000 pylammpstrj-1.0.4a0/include/pylammpstrjmodule.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     3422 2024-05-02 13:28:28.000000 pylammpstrj-1.0.4a0/include/pytrajectory.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      459 2024-05-02 13:28:28.000000 pylammpstrj-1.0.4a0/include/pyutils.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      865 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/read.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      876 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/select.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     3772 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/trajectory.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     1491 2024-05-02 13:28:22.000000 pylammpstrj-1.0.4a0/include/utils.h
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      733 2024-05-02 13:31:35.000000 pylammpstrj-1.0.4a0/pyproject.toml
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)       38 2024-05-02 13:31:46.606336 pylammpstrj-1.0.4a0/setup.cfg
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      763 2024-05-02 13:14:29.000000 pylammpstrj-1.0.4a0/setup.py
+drwxrwxr-x   0 louchao   (1002) louchao   (1002)        0 2024-05-02 13:31:46.606336 pylammpstrj-1.0.4a0/src/
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)    12960 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/atom.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)    17241 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/bond.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      579 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/box.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     9772 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/property.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     5972 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pyatom.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     4422 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pybond.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     2249 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pybox.c
+drwxrwxr-x   0 louchao   (1002) louchao   (1002)        0 2024-05-02 13:31:46.606336 pylammpstrj-1.0.4a0/src/pylammpstrj.egg-info/
+-rw-r--r--   0 louchao   (1002) louchao   (1002)    42830 2024-05-02 13:31:46.000000 pylammpstrj-1.0.4a0/src/pylammpstrj.egg-info/PKG-INFO
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)      691 2024-05-02 13:31:46.000000 pylammpstrj-1.0.4a0/src/pylammpstrj.egg-info/SOURCES.txt
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)        1 2024-05-02 13:31:46.000000 pylammpstrj-1.0.4a0/src/pylammpstrj.egg-info/dependency_links.txt
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)       12 2024-05-02 13:31:46.000000 pylammpstrj-1.0.4a0/src/pylammpstrj.egg-info/top_level.txt
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     5450 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pylammpstrjmodule.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)    16440 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pytrajectory.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     7665 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pytrajectoryfile.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     4211 2024-05-02 13:28:01.000000 pylammpstrj-1.0.4a0/src/pyutils.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)    25459 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/read.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)    20270 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/select.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     1929 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/skip.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     2955 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/trajectory.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     5372 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/trajectoryfile.c
+-rw-rw-r--   0 louchao   (1002) louchao   (1002)     2052 2024-05-02 13:27:38.000000 pylammpstrj-1.0.4a0/src/utils.c
```

### Comparing `pylammpstrj-1.0.3rc0/LICENSE` & `pylammpstrj-1.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpstrj-1.0.3rc0/PKG-INFO` & `pylammpstrj-1.0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpstrj
-Version: 1.0.3rc0
+Version: 1.0.4a0
 Summary: Processing LAMMPS trajectory files.
 Author-email: Heiarii Lou Chao <heiariilouchao@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pylammpstrj-1.0.3rc0/README.md` & `pylammpstrj-1.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/include/atom.h` & `pylammpstrj-1.0.4a0/include/atom.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #ifndef _ATOM_H
 #define _ATOM_H
+#include "box.h"
 #include "utils.h"
 
-#include <stdlib.h>
 #include <stdio.h>
 
 /** The number of characters for additional fields of type str. */
 #define ATOM_FIELD_STR_LIMIT 10
+#define ATOM_FIELD_STR_LIMIT_SCANF "9"
 
 /** An union to store additional `Atom` fields. */
 union AtomField
 {
     int i;
     double d;
     char s[ATOM_FIELD_STR_LIMIT];
@@ -25,14 +26,16 @@
 /**
  * The maximum number of characters to read for element strings.
  *
  * The null-terminator is excluded.
  */
 #define LABEL_SCANF_LIMIT "2"
 
+#define N_BONDS_LIMIT 8
+
 /**
  * The data structure used to represent atoms.
  *
  * The atoms are identified by their `id`.
  *
  * This data structure holds the informations about an atom's `label`,
  * `position`, and `charge`.
@@ -42,21 +45,26 @@
     unsigned int id;
     unsigned int type;
     char label[LABEL_LIMIT];
     double position[3];
     double charge;
 
     union AtomField *additionnal_fields;
+
+    // Non-essential attributes
+    unsigned int N_bonds;
+    unsigned int *ids;
+    double *bond_orders;  // Stores one more slot for the sum
+    double total_bo;
 };
 
 /** Deletes an atom. */
 void atom_delete(struct Atom *atom);
 
-typedef union AtomField (*AtomBuilderParsingFunction)(
-    const char[BUFFER_LIMIT]);
+typedef union AtomField (*AtomBuilderParsingFunction)(const char[BUFFER_LIMIT]);
 
 /** An enum to identify additional `Atom` fields types. */
 enum AtomFieldType
 {
     AFT_NULL,
     AFT_INT,
     AFT_DOUBLE,
@@ -73,28 +81,27 @@
 
     unsigned int N_fields;
     unsigned int N_additional;
     char (*field_names)[FIELD_NAME_LIMIT];  // A pointer to static arrays
     size_t *offsets;
     int *is_additional;
     enum AtomFieldType *fields_types;
-    AtomBuilderParsingFunction *parsing_functions;
 };
 
 /** Creates an `AtomBuilder`. */
 struct AtomBuilder atom_builder_new(const char *dump_format, FILE *input);
 
 /** Copies an `AtomBuilder` to another */
 void atom_builder_copy(struct AtomBuilder *, const struct AtomBuilder);
 
 /** Deletes an `AtomBuilder`. */
 void atom_builder_delete(struct AtomBuilder *ab);
 
 /** Copies an `Atom` to another. */
-void atom_copy(struct Atom *dest, const struct Atom src,
-               const struct AtomBuilder atom_builder);
+void atom_copy(struct Atom *dest, const struct Atom src, const struct AtomBuilder atom_builder);
 
 /** Creates an `Atom` from a line of a trajectory file. */
-struct Atom read_atom_entry(const struct AtomBuilder atom_builder,
-                            char line[BUFFER_LIMIT]);
+void atom_read_entry(struct Atom *atom, const struct AtomBuilder atom_builder, char line[BUFFER_LIMIT], union AtomField *additional_fields);
+
+double atom_compute_distance(const double lengths[3], const struct Atom a1, const struct Atom a2);
 
 #endif
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/include/box.h` & `pylammpstrj-1.0.4a0/include/box.h`

 * *Files identical despite different names*

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/include/pyatom.h` & `pylammpstrj-1.0.4a0/include/pyatom.h`

 * *Files identical despite different names*

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/include/pybox.h` & `pylammpstrj-1.0.4a0/include/pybox.h`

 * *Files identical despite different names*

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/include/pytrajectory.h` & `pylammpstrj-1.0.4a0/include/pytrajectory.h`

 * *Files 22% similar despite different names*

```diff
@@ -2,107 +2,96 @@
 #define _PYTRAJECTORY_H
 
 #include "trajectory.h"
 
 #include <Python.h>
 #include <stdbool.h>
 
+#include <descrobject.h>
+#include <methodobject.h>
+#include <object.h>
+#include <pymacro.h>
+
 typedef struct PyTrajectoryObject
 {
-    PyObject_HEAD
-    struct Trajectory trajectory;
+    PyObject_HEAD struct Trajectory trajectory;
 } PyTrajectoryObject;
 
 void PyTrajectory_dealloc(PyTrajectoryObject *self);
 
-PyObject *PyTrajectory_new(PyTypeObject *type, PyObject *Py_UNUSED(args),
-                           PyObject *Py_UNUSED(kwargs));
+PyObject *PyTrajectory_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwargs));
+
+PyObject *PyTrajectory_get_N_configurations(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_N_configurations(PyTrajectoryObject *self,
-                                            void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_steps(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_steps(PyTrajectoryObject *self,
-                                 void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_N_atoms(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_N_atoms(PyTrajectoryObject *self,
-                                   void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_dump_format(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_dump_format(PyTrajectoryObject *self,
-                                       void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_field_names(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_field_names(PyTrajectoryObject *self,
-                                       void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_additional_fields(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_additional_fields(PyTrajectoryObject *self,
-                                             void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_atoms(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_atoms(PyTrajectoryObject *self,
-                                 void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_boxes(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
-PyObject *PyTrajectory_get_boxes(PyTrajectoryObject *self,
-                                 void *Py_UNUSED(closure));
+PyObject *PyTrajectory_get_bond_mode(PyTrajectoryObject *self, void *Py_UNUSED(closure));
 
 extern PyGetSetDef PyTrajectory_getset[];
 
 PyObject *PyTrajectory_str(PyTrajectoryObject *self);
 
 PyObject *PyTrajectory_repr(PyTrajectoryObject *self);
 
-void PyTrajectory_initialize(PyTrajectoryObject *self,
-                             struct Trajectory trajectory);
+void PyTrajectory_initialize(PyTrajectoryObject *self, struct Trajectory trajectory);
+
+PyObject *PyTrajectory_select(PyTrajectoryObject *self, PyObject *args, PyObject *kwargs);
+
+PyObject *PyTrajectory_moving_select(PyTrajectoryObject *self, PyObject *args, PyObject *kwargs);
 
-PyObject *PyTrajectory_select_atoms(PyTrajectoryObject *self, PyObject *args,
-                                    PyObject *kwargs);
+PyObject *PyTrajectory_compute_bonds(PyTrajectoryObject *self, PyObject *args);
 
-PyObject *PyTrajectory_compute_average(PyTrajectoryObject *self,
-                                       PyObject *args);
+PyObject *PyTrajectory_compute_average(PyTrajectoryObject *self, PyObject *args);
 
 extern PyMethodDef PyTrajectory_methods[];
 
 extern PyTypeObject PyTrajectoryType;
 
 typedef struct PyTrajectoryFileObject
 {
     PyObject_HEAD struct TrajectoryFile trajectory_file;
 } PyTrajectoryFileObject;
 
-PyObject *PyTrajectoryFile_new(PyTypeObject *type, PyObject *Py_UNUSED(args),
-                               PyObject *Py_UNUSED(kwargs));
+PyObject *PyTrajectoryFile_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwargs));
 
-void PyTrajectoryFile_initialize(PyTrajectoryFileObject *self,
-                                 const struct TrajectoryFile trajectory_file);
+void PyTrajectoryFile_initialize(PyTrajectoryFileObject *self, const struct TrajectoryFile trajectory_file);
 
 void PyTrajectoryFile_dealloc(PyTrajectoryFileObject *self);
 
 PyObject *PyTrajectoryFile_str(PyTrajectoryFileObject *self);
 
 PyObject *PyTrajectoryFile_repr(PyTrajectoryFileObject *self);
 
-PyObject *PyTrajectoryFile_get_N_configurations(PyTrajectoryFileObject *self,
-                                                PyObject *Py_UNUSED(closure));
+PyObject *PyTrajectoryFile_get_N_configurations(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure));
 
-PyObject *PyTrajectoryFile_get_steps(PyTrajectoryFileObject *self,
-                                     PyObject *Py_UNUSED(closure));
+PyObject *PyTrajectoryFile_get_steps(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure));
 
-PyObject *PyTrajectoryFile_get_file_name(PyTrajectoryFileObject *self,
-                                         PyObject *Py_UNUSED(closure));
+PyObject *PyTrajectoryFile_get_file_name(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure));
 
-PyObject *PyTrajectoryFile_get_batch_size(PyTrajectoryFileObject *self,
-                                          PyObject *Py_UNUSED(closure));
+PyObject *PyTrajectoryFile_get_batch_size(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure));
 
-PyObject *PyTrajectoryFile_get_selections(PyTrajectoryFileObject *self,
-                                          PyObject *Py_UNUSED(closure));
+PyObject *PyTrajectoryFile_get_selections(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure));
 
 extern PyGetSetDef PyTrajectoryFile_getset[];
 
-PyObject *PyTrajectoryFile_select_atoms(PyTrajectoryFileObject *self,
-                                   PyObject *args);
+PyObject *PyTrajectory_select(PyTrajectoryObject *self, PyObject *args, PyObject *kwargs);
 
-PyObject *PyTrajectoryFile_compute_average(PyTrajectoryFileObject *self,
-                                           PyObject *args);
+PyObject *PyTrajectoryFile_compute_average(PyTrajectoryFileObject *self, PyObject *args);
 
 PyObject *PyTrajectoryFile_load(PyTrajectoryFileObject *self);
 
 extern PyMethodDef PyTrajectoryFile_methods[];
 
 extern PyTypeObject PyTrajectoryFileType;
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/include/read.h` & `pylammpstrj-1.0.4a0/include/read.h`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,19 @@
 
 /** The base number of configurations for memory allocation. */
 #define BASE_N_CONFIGURATIONS 100
 
 /** The number of configurations increment for memory allocation. */
 #define N_CONFIGURATIONS_INCR 100
 
-/** The number of characters to skip in the header line to obtain the dump
- * format. */
+/** The number of characters to skip in the header line to obtain the dump format. */
 #define DUMP_FORMAT_OFFSET 12
 
 void read_current_step(FILE *input, unsigned long *current_step);
 
 void read_dump_format(FILE *input, char dump_format[BUFFER_LIMIT]);
 
-void read_parameters(FILE **input, const char dump_format[BUFFER_LIMIT],
-                     unsigned int *timestep, unsigned int *N_atoms,
-                     struct Box *box);
+void read_parameters(FILE **input, const char dump_format[BUFFER_LIMIT], unsigned int *timestep, unsigned int *N_atoms, struct Box *box);
 
-void read_atoms(FILE **input, const struct AtomBuilder atom_builder,
-                const unsigned int N_atoms, struct Atom *atoms);
+void read_atoms(FILE **input, const struct AtomBuilder atom_builder, const unsigned int N_atoms, struct Atom *atoms, union AtomField *additional_fields);
 
 #endif
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/atom.c` & `pylammpstrj-1.0.4a0/src/atom.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,70 @@
-#include "utils.h"
 #include "atom.h"
+#include "utils.h"
 
 #include <ctype.h>
 #include <errno.h>
 #include <stddef.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <strings.h>
 
-void atom_delete(struct Atom *atom) { free(atom->additionnal_fields); }
+void atom_delete(struct Atom *atom)
+{
+    if (atom->additionnal_fields != NULL) atom->additionnal_fields = NULL;  // Only need to dereference
+    if (atom->N_bonds != 0)
+    {
+        free(atom->ids);
+        free(atom->bond_orders);
+    }
+}
 
-void atom_copy(struct Atom *dest, const struct Atom src,
-               const struct AtomBuilder atom_builder)
+void atom_copy(struct Atom *dest, const struct Atom src, const struct AtomBuilder atom_builder)
 {
     dest->id = src.id;
     dest->type = src.type;
     strncpy(dest->label, src.label, LABEL_LIMIT);
     memcpy(dest->position, src.position, 3 * sizeof(double));
     dest->charge = src.charge;
-    dest->additionnal_fields =
-        malloc(atom_builder.N_additional * sizeof(union AtomField));
-    if (dest->additionnal_fields == NULL)
+    if (atom_builder.N_additional != 0)
+        memcpy(dest->additionnal_fields, src.additionnal_fields, atom_builder.N_additional * sizeof(union AtomField));  // To check
+    dest->N_bonds = src.N_bonds;
+    if (src.N_bonds != 0)
     {
-        errno = ENOMEM;
-        perror(
-            "Error while allocating memory (atom_copy.dest.additional_fields)");
-        return;
+        dest->ids = calloc(src.N_bonds, sizeof(unsigned int));
+        if (dest->ids == NULL)
+        {
+            errno = ENOMEM;
+            perror("Error while allocating memory (atom_copy.dest.ids)");
+            return;
+        }
+        memcpy(dest->ids, src.ids, src.N_bonds * sizeof(unsigned int));
+        if (src.bond_orders != NULL)
+        {
+            dest->bond_orders = calloc(src.N_bonds, sizeof(double));
+            if (dest->bond_orders == NULL)
+            {
+                errno = ENOMEM;
+                perror("Error while allocating memory (atom_copy.dest.bond_orders)");
+                return;
+            }
+            memcpy(dest->bond_orders, src.bond_orders, src.N_bonds * sizeof(double));
+            dest->total_bo = src.total_bo;
+        }
     }
-    memcpy(dest->additionnal_fields, src.additionnal_fields,
-           atom_builder.N_additional * sizeof(union AtomField));
 }
 
 #define FIELDS_BASE_SIZE 10
 #define FIELDS_SIZE_INCR 10
 
 void get_field_names(struct AtomBuilder *ab)
 {
     char buffer[BUFFER_LIMIT], *ptr;
-    char(*names)[FIELD_NAME_LIMIT] =
-        calloc(FIELDS_BASE_SIZE, sizeof(char[FIELD_NAME_LIMIT]));
+    char(*names)[FIELD_NAME_LIMIT] = calloc(FIELDS_BASE_SIZE, sizeof(char[FIELD_NAME_LIMIT]));
 
     if (names == NULL)
     {
         errno = ENOMEM;
         perror("Error while allocating memory (AtomBuilder.names)");
         return;
     }
@@ -54,17 +75,15 @@
     strncpy(buffer, ab->dump_format, BUFFER_LIMIT);
     ptr = strtok(buffer, " ");
 
     while (ptr != NULL)
     {
         if (n >= names_size)
         {
-            char(*new_names)[FIELD_NAME_LIMIT] =
-                realloc(names, (names_size + FIELDS_SIZE_INCR) *
-                                   sizeof(char[FIELD_NAME_LIMIT]));
+            char(*new_names)[FIELD_NAME_LIMIT] = realloc(names, (names_size + FIELDS_SIZE_INCR) * sizeof(char[FIELD_NAME_LIMIT]));
 
             if (new_names == NULL)
             {
                 free(new_names);
                 errno = ENOMEM;
                 perror("Error while reallocating memory (AtomBuilder.names)");
                 return;
@@ -88,16 +107,15 @@
 
 void check_names(struct AtomBuilder *ab)
 {
     ab->offsets = calloc(ab->N_fields, sizeof(size_t));
     ab->is_additional = calloc(ab->N_fields, sizeof(int));
     ab->fields_types = malloc(ab->N_fields * sizeof(enum AtomFieldType));
 
-    if (ab->offsets == NULL || ab->is_additional == NULL ||
-        ab->fields_types == NULL)
+    if (ab->offsets == NULL || ab->is_additional == NULL || ab->fields_types == NULL)
     {
         errno = ENOMEM;
         perror("Error while allocating memory (AtomBuilder.check_names)");
         return;
     }
 
     unsigned int N_additional = 0;
@@ -110,18 +128,17 @@
             (ab->fields_types)[f] = AFT_INT;
         }
         else if (strcmp((ab->field_names)[f], "type") == 0)
         {
             (ab->offsets)[f] = offsetof(struct Atom, type);
             (ab->fields_types)[f] = AFT_INT;
         }
-        else if (strcmp((ab->field_names)[f], "element") == 0 ||
-                 strcmp((ab->field_names)[f], "label") == 0)
+        else if (strcmp((ab->field_names)[f], "element") == 0 || strcmp((ab->field_names)[f], "label") == 0)
         {
-            (ab->offsets)[f] = offsetof(struct Atom, id);
+            (ab->offsets)[f] = offsetof(struct Atom, label);
             (ab->fields_types)[f] = AFT_STRING;
         }
         else if (strlen((ab->field_names)[f]) == 1)
         {
             if ((ab->field_names)[f][0] == 'x')
                 (ab->offsets)[f] = offsetof(struct Atom, position[0]);
             else if ((ab->field_names)[f][0] == 'y')
@@ -131,194 +148,174 @@
             else if ((ab->field_names)[f][0] == 'q')
                 (ab->offsets)[f] = offsetof(struct Atom, charge);
 
             if ((ab->offsets)[f] != 0) (ab->fields_types)[f] = AFT_DOUBLE;
         }
         else
         {
-            (ab->offsets)[f] =
-                N_additional;  // the rank in the additional_fields array
+            (ab->offsets)[f] = N_additional;  // the rank in the additional_fields array
             (ab->is_additional)[f] = 1;
             N_additional++;
         }
     }
     ab->N_additional = N_additional;
 }
 
-void get_additional_types(const char line[BUFFER_LIMIT],
-                          struct AtomBuilder *ab)
+void get_additional_types(const char line[BUFFER_LIMIT], struct AtomBuilder *ab)
 {
     char buffer[BUFFER_LIMIT];
     strncpy(buffer, line, BUFFER_LIMIT);
+    buffer[BUFFER_LIMIT - 1] = '\0';
 
     char *ptr = strtok(buffer, " ");
 
     for (unsigned int f = 0; f < ab->N_fields; ptr = strtok(NULL, " "), f++)
     {
         if (!(ab->is_additional)[f]) continue;
 
         if (isalpha(ptr[0]))
             (ab->fields_types)[f] = AFT_STRING;
         else
             (ab->fields_types)[f] = AFT_DOUBLE;
     }
 }
 
-static union AtomField str_to_int(const char field[BUFFER_LIMIT])
-{
-    return (union AtomField){.i = atoi(field)};
-}
-
-static union AtomField str_to_double(const char field[BUFFER_LIMIT])
-{
-    return (union AtomField){.d = atof(field)};
-}
-
-static union AtomField str_to_str(const char field[BUFFER_LIMIT])
-{
-    union AtomField af;
-    strncpy(af.s, field, ATOM_FIELD_STR_LIMIT);
-    return af;
-}
-
-void initialize_functions(struct AtomBuilder *ab)
-{
-    union AtomField (**functions)(const char[BUFFER_LIMIT]) =
-        malloc(ab->N_fields *
-               sizeof(union AtomField(*)(const char[BUFFER_LIMIT])));
-
-    if (functions == NULL)
-    {
-        errno = ENOMEM;
-        perror("Error while allocating memory (AtomBuilder.parsing_functions)");
-        return;
-    }
-
-    for (unsigned int field = 0; field < ab->N_fields; field++)
-    {
-        switch (ab->fields_types[field])
-        {
-            case AFT_INT:
-                functions[field] = &str_to_int;
-                break;
-            case AFT_DOUBLE:
-                functions[field] = &str_to_double;
-                break;
-            case AFT_STRING:
-                functions[field] = &str_to_str;
-                break;
-            default:
-                errno = EINVAL;
-                perror("Error while scanning the types (AFT_NULL)");
-                ab->parsing_functions = functions;
-                return;
-        }
-    }
-    ab->parsing_functions = functions;
-}
-
 struct AtomBuilder atom_builder_new(const char *dump_format, FILE *input)
 {
-    struct AtomBuilder ab;
+    struct AtomBuilder ab = {0};
 
+    // Initialize the dump format
     strncpy(ab.dump_format, dump_format, BUFFER_LIMIT);
+    ab.dump_format[BUFFER_LIMIT - 1] = '\0';
 
+    // Initialize the field names
     get_field_names(&ab);
     if (errno != 0) return ab;
 
+    // Initialize offsets, is_additional, and fields_types
     check_names(&ab);
     if (errno != 0)
     {
         free(ab.field_names);
         return ab;
     }
 
+    // Skip to the atoms section header
     char line[BUFFER_LIMIT];
     long pos = ftell(input);
     do
         if (fgets(line, BUFFER_LIMIT, input) == NULL)
         {
             free(ab.fields_types);
             free(ab.is_additional);
             free(ab.offsets);
             free(ab.field_names);
             errno = EIO;
             perror("Error while reading a line (AtomBuilder.atom_builder_new)");
+            return ab;
         }
     while (strncmp(line, "ITEM: ATOMS", 11) != 0);
 
-    fgets(line, BUFFER_LIMIT, input);
-    get_additional_types(line, &ab);
-
-    initialize_functions(&ab);
-    if (errno != 0)
+    if (fgets(line, BUFFER_LIMIT, input) == NULL)
     {
-        free(ab.parsing_functions);
         free(ab.fields_types);
         free(ab.is_additional);
         free(ab.offsets);
         free(ab.field_names);
+        errno = EIO;
+        perror("Error while reading a line");
         return ab;
     }
+    get_additional_types(line, &ab);  // Parse the header
+    fseek(input, pos, SEEK_SET);      // Reset the file pointer position
 
-    fseek(input, pos, SEEK_SET);
     return ab;
 }
 
-struct Atom read_atom_entry(const struct AtomBuilder ab,
-                            char line[BUFFER_LIMIT])
+void atom_read_entry(struct Atom *atom, const struct AtomBuilder builder, char line[BUFFER_LIMIT], union AtomField *additional_fields)
 {
-    struct Atom atom;
-    atom.additionnal_fields = malloc(ab.N_additional * sizeof(union AtomField));
-    if (atom.additionnal_fields == NULL)
-    {
-        errno = ENOMEM;
-        perror("Error while allocating memory (Atom.additional_fields)");
-        return atom;
-    }
-
-    char *field = strtok(line, " ");
-
-    for (unsigned int f = 0; f < ab.N_fields; field = strtok(NULL, " "), f++)
-    {
-        union AtomField res = ab.parsing_functions[f](field);
-        size_t offset = ab.offsets[f];
-        if ((ab.is_additional)[f])
-            (atom.additionnal_fields)[offset] = res;
-        else
+    *atom = (struct Atom) {0};
+    char *start = line;
+    for (unsigned int f = 0; f < builder.N_fields; f++)
+    {
+        // Parse the current field
+        size_t offset = builder.offsets[f];
+        if ((builder.is_additional)[f])  // Fill additional fields
         {
-            switch (ab.fields_types[f])
+            union AtomField atom_field = {0};
+            switch (builder.fields_types[f])
             {
                 case AFT_INT:
+                    if (sscanf(start, " %d ", &atom_field.i) != 1)
                     {
-                        int *ptr = (int *) ((void *) &atom + offset);
-                        *ptr = res.i;
-                        break;
+                        errno = EIO;
+                        perror("Error while parsing an atom field (read_atom_entry.atom_field.i)");
+                        return;
                     }
+                    break;
                 case AFT_DOUBLE:
+                    if (sscanf(start, " %lf ", &atom_field.d) != 1)
                     {
-                        double *ptr = (double *) ((void *) &atom + offset);
-                        *ptr = res.d;
-                        break;
+                        errno = EIO;
+                        perror("Error while parsing an atom field (read_atom_entry.atom_field.d)");
+                        return;
                     }
+                    break;
                 case AFT_STRING:
-                    // Only if the field is `label`
-                    strncpy(atom.label, res.s, LABEL_LIMIT);
+                    if (sscanf(start, " %" ATOM_FIELD_STR_LIMIT_SCANF "s ", (char *) &atom_field.s) != 1)
+                    {
+                        errno = EIO;
+                        perror("Error while parsing an atom field (read_atom_entry.atom_field.s)");
+                        return;
+                    }
                     break;
                 default:
                     errno = EINVAL;
-                    perror(
-                        "Error while reading an entry "
-                        "(AtomBuilder.new_atom_entry)");
-                    return atom;
+                    perror("Error while parging an atom field (read_atom_entry.atom_field, AFT_NULL)");
+                    return;
             }
+            additional_fields[offset] = atom_field;
         }
-    }
+        else  // Fill base fields
+            switch (builder.fields_types[f])
+            {
+                case AFT_INT:
+                    if (sscanf(start, " %d ", (int *) ((void *) atom + offset)) != 1)
+                    {
+                        errno = EIO;
+                        perror("Error while parsing an atom field (read_atom_entry.atom, AFT_INT)");
+                        return;
+                    }
+                    break;
+                case AFT_DOUBLE:
+                    if (sscanf(start, " %lf ", (double *) ((void *) atom + offset)) != 1)
+                    {
+                        errno = EIO;
+                        perror("Error while parsing an atom field (read_atom_entry.atom, AFT_DOUBLE)");
+                        return;
+                    }
+                    break;
+                case AFT_STRING:
+                    // Only authorized str base field is the label
+                    if (sscanf(start, " %" LABEL_SCANF_LIMIT "s ", (char *) atom->label) != 1)
+                    {
+                        errno = EIO;
+                        perror("Error while parsing an atom field (read_atom_entry.atom, AFT_STRING)");
+                        return;
+                    }
+                    break;
+                default:
+                    errno = EINVAL;
+                    perror("Error while parging an atom field (read_atom_entry.atom, AFT_NULL)");
+                    return;
+            }
 
-    return atom;
+        // Go to next field
+        start = str_go_to_next(start, ' ');
+    }
 }
 
 void atom_builder_copy(struct AtomBuilder *dest, const struct AtomBuilder src)
 {
     strncpy(dest->dump_format, src.dump_format, BUFFER_LIMIT);
 
     dest->N_fields = src.N_fields;
@@ -329,24 +326,22 @@
     {
         errno = ENOMEM;
         perror(
             "Error while allocation memory "
             "(atom_builder_copy.dest.field_names)");
         return;
     }
-    memcpy(dest->field_names, src.field_names,
-           src.N_fields * sizeof(char[FIELD_NAME_LIMIT]));
+    memcpy(dest->field_names, src.field_names, src.N_fields * sizeof(char[FIELD_NAME_LIMIT]));
 
     dest->offsets = malloc(src.N_fields * sizeof(size_t));
     if (dest->offsets == NULL)
     {
         free(dest->field_names);
         errno = ENOMEM;
-        perror(
-            "Error while allocation memory (atom_builder_copy.dest.offsets)");
+        perror("Error while allocation memory (atom_builder_copy.dest.offsets)");
         return;
     }
     memcpy(dest->offsets, src.offsets, src.N_fields * sizeof(size_t));
 
     dest->is_additional = malloc(src.N_fields * sizeof(int));
     if (dest->is_additional == NULL)
     {
@@ -368,36 +363,36 @@
         free(dest->field_names);
         errno = ENOMEM;
         perror(
             "Error while allocation memory "
             "(atom_builder_copy.dest.fields_types)");
         return;
     }
-    memcpy(dest->fields_types, src.fields_types,
-           src.N_fields * sizeof(enum AtomFieldType));
-
-    dest->parsing_functions =
-        malloc(src.N_fields * sizeof(AtomBuilderParsingFunction));
-    if (dest->parsing_functions == NULL)
-    {
-        free(dest->fields_types);
-        free(dest->is_additional);
-        free(dest->offsets);
-        free(dest->field_names);
-        errno = ENOMEM;
-        perror(
-            "Error while allocation memory "
-            "(atom_builder_copy.dest.parsing_functions)");
-        return;
-    }
-    memcpy(dest->parsing_functions, src.parsing_functions,
-           src.N_fields * sizeof(AtomBuilderParsingFunction));
+    memcpy(dest->fields_types, src.fields_types, src.N_fields * sizeof(enum AtomFieldType));
 }
 
 void atom_builder_delete(struct AtomBuilder *ab)
 {
-    free(ab->parsing_functions);
     free(ab->field_names);
     free(ab->offsets);
     free(ab->is_additional);
     free(ab->fields_types);
 }
+
+double atom_compute_distance(const double lengths[3], const struct Atom a1, const struct Atom a2)
+{
+    double res = 0.;
+    for (unsigned int d = 0; d < 3; d++)
+    {
+        double pos1 = a1.position[d], pos2 = a2.position[d];
+        double img = pos2;  // the closest periodic image of a2 to a1 in the current direction
+
+        // Applying the PBCs
+        if (pos2 - pos1 < -lengths[d] / 2.)
+            img += lengths[d];
+        else if (pos2 - pos1 > lengths[d] / 2.)
+            img -= lengths[d];
+
+        res += (img - pos1) * (img - pos1);
+    }
+    return res;
+}
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/average.c` & `pylammpstrj-1.0.4a0/src/property.c`

 * *Files 19% similar despite different names*

```diff
@@ -1,247 +1,263 @@
+#include "atom.h"
 #include "trajectory.h"
 
 #include <errno.h>
 #include <math.h>
+#include <omp.h>
 #include <stdbool.h>
 #include <stddef.h>
+#include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
-static double *compute_average(const size_t offset,
-                               const enum AtomFieldType type,
-                               const struct Trajectory trajectory)
+union AtomField *trajectory_get_property(const struct Trajectory trajectory, const unsigned int field, unsigned long *size)
 {
-    double *averages = calloc(trajectory.N_configurations, sizeof(double));
-    if (averages == NULL)
+    // Preparing the array
+    union AtomField *property = calloc(trajectory._total_atoms, sizeof(union AtomField));
+    if (property == NULL)  // Could not allocate memory
     {
         errno = ENOMEM;
-        perror("Error while allocating memory (compute_average.averages)");
+        perror("Error while allocating memory (trajectory_get_property)");
         return NULL;
     }
 
-    for (unsigned int c = 0, i = 0; c < trajectory.N_configurations; c++)
+    size_t offset = trajectory.atom_builder.offsets[field];
+
+    // Transfering the data
+    if (trajectory.atom_builder.is_additional[field])
+        for (unsigned int a = 0; a < trajectory._total_atoms; a++) property[a] = trajectory._additional_fields[a * trajectory.atom_builder.N_additional + offset];
+    else
+        for (unsigned int a = 0; a < trajectory._total_atoms; a++)
+            property[a] = *(union AtomField *) ((void *) (trajectory.atoms + a) + offset);
+
+    *size = trajectory._total_atoms;
+    return property;
+}
+
+union AtomField *trajectoryfile_get_property(const struct TrajectoryFile trajectory_file, const unsigned int field, unsigned long *size)
+{
+    // Preparing the array
+    union AtomField *properties = NULL;
+    unsigned int properties_size = 0;
+
+    // Preparing to read
+    unsigned int N_batches = (unsigned int) floor((double) trajectory_file.N_configurations / trajectory_file.batch_size);
+    unsigned int remaining_conf = trajectory_file.N_configurations % trajectory_file.batch_size;
+
+    // Transfering the data
+    for (unsigned int batch = 0; batch < N_batches; batch++)
     {
-        for (unsigned int a = 0; a < trajectory.N_atoms[c]; a++, i++)
+        struct Trajectory trajectory;
+        trajectoryfile_read_slice(trajectory_file, trajectory_file.steps[batch * trajectory_file.batch_size], trajectory_file.batch_size,
+                                  &trajectory);
+        if (errno != 0)  // Could not read slice
+        {
+            if (properties != NULL) free(properties);
+            perror("Error while reading a slice (trajectoryfile_average_property.trajectory)");
+            return NULL;
+        }
+
+        // Sub-optimal
+        unsigned long n_atoms;
+        union AtomField *tmp = trajectory_get_property(trajectory, field, &n_atoms);
+        if (tmp == NULL)
         {
-            switch (type)
+            if (properties != NULL) free(properties);
+            trajectory_delete(&trajectory);
+            errno = ENOMEM;
+            perror("Error while reallocating memory (trajectoryfile_get_property)");
+            return NULL;
+        }
+
+        // (Re)Allocating memory
+        {
+            union AtomField *new_properties = realloc(properties, (properties_size + n_atoms) * sizeof(union AtomField));
+            if (new_properties == NULL)  // Could not reallocate memory
             {
-                case AFT_INT:
-                    averages[c] += (double) *(
-                        int *) ((void *) (trajectory.atoms + i) + offset);
-                    break;
-                case AFT_DOUBLE:
-                    averages[c] +=
-                        *(double *) ((void *) (trajectory.atoms + i) + offset);
-                    break;
-                default:
-                    free(averages);
-                    averages = NULL;
-                    errno = EINVAL;
-                    perror("Error while selecting type of value");
-                    return NULL;
+                if (properties != NULL) free(properties);
+                trajectory_delete(&trajectory);
+                errno = ENOMEM;
+                perror("Error while reallocating memory (trajectoryfile_get_property)");
+                return NULL;
             }
+            // properties_size += n_atoms;  // Not now otherwise we won't be able to add the new properties
+            properties = new_properties;
         }
-        averages[c] /= trajectory.N_atoms[c];
-    }
-
-    return averages;
-}
 
-static double *compute_average_additional(const size_t offset,
-                                       const enum AtomFieldType type,
-                                       const struct Trajectory trajectory)
-{
-    double *averages = calloc(trajectory.N_configurations, sizeof(double));
-    if (averages == NULL)
-    {
-        errno = ENOMEM;
-        perror("Error while allocating memory (compute_average.averages)");
-        return NULL;
+        memcpy(properties + properties_size, tmp, n_atoms * sizeof(union AtomField));
+        properties_size += n_atoms;
+        free(tmp);
+        trajectory_delete(&trajectory);
     }
 
-    for (unsigned int c = 0, i = 0; c < trajectory.N_configurations; c++)
+    if (remaining_conf != 0)
     {
-        for (unsigned int a = 0; a < trajectory.N_atoms[c]; a++, i++)
+        struct Trajectory trajectory;
+        trajectoryfile_read_slice(trajectory_file, trajectory_file.steps[N_batches * trajectory_file.batch_size], remaining_conf,
+                                  &trajectory);
+        if (errno != 0)  // Could not read slice
+        {
+            free(properties);
+            perror("Error while reading a slice (trajectoryfile_average_property.trajectory)");
+            return NULL;
+        }
+
+        unsigned long n_atoms;
+        union AtomField *tmp = trajectory_get_property(trajectory, field, &n_atoms);
+        if (tmp == NULL)
         {
-            switch (type)
+            free(properties);
+            trajectory_delete(&trajectory);
+            errno = ENOMEM;
+            perror("Error while reallocating memory (trajectoryfile_get_property)");
+            return NULL;
+        }
+
+        // (Re)Allocating memory
+        {
+            union AtomField *new_properties = realloc(properties, (properties_size + n_atoms) * sizeof(union AtomField));
+            if (new_properties == NULL)  // Could not reallocate memory
             {
-                case AFT_INT:
-                    averages[c] += (double) trajectory.atoms[i]
-                                          .additionnal_fields[offset]
-                                          .i;
-                    break;
-                case AFT_DOUBLE:
-                    averages[c] +=
-                        trajectory.atoms[i].additionnal_fields[offset].d;
-                    break;
-                default:
-                    free(averages);
-                    errno = EINVAL;
-                    perror("Error while selecting type of value");
-                    return NULL;
+                trajectory_delete(&trajectory);
+                free(properties);
+                errno = ENOMEM;
+                perror("Error while reallocating memory (trajectoryfile_get_property)");
+                return NULL;
             }
+            // properties_size += n_atoms;  // Not now otherwise we won't be able to add the new properties
+            properties = new_properties;
         }
-        averages[c] /= trajectory.N_atoms[c];
+
+        memcpy(properties + properties_size, tmp, n_atoms * sizeof(union AtomField));
+        properties_size += n_atoms;
+        free(tmp);
+        trajectory_delete(&trajectory);
     }
 
-    return averages;
+    *size = properties_size;
+    return properties;
 }
 
-double *trajectory_average_property(const struct Trajectory trajectory,
-                                    const unsigned int field)
+double *trajectory_average_property(const struct Trajectory trajectory, const unsigned int field)
 {
     // Preparing the array
-    double *averages;
-
-    // Transforming the field into an offset
-    size_t offset = trajectory.atom_builder.offsets[field];
+    double *averages = calloc(trajectory.N_configurations, sizeof(double));
+    if (averages == NULL)  // Could not allocate memory
+    {
+        errno = ENOMEM;
+        perror("Error while allocating memory (trajectory_average_property)");
+        return NULL;
+    }
 
-    // Getting the type of data
+    // Checking the type of data
     enum AtomFieldType type = trajectory.atom_builder.fields_types[field];
 
-    if (!trajectory.atom_builder.is_additional[field])
+    // Gathering the data
+    unsigned long size;
+    union AtomField *properties = trajectory_get_property(trajectory, field, &size);
+    if (properties == NULL)  // Something went wrong
     {
-        averages = compute_average(offset, type, trajectory);
-        if (errno != 0) return NULL;
+        free(averages);
+        perror("Error while getting the property (trajectory_average_property)");
+        return NULL;
     }
-    else
+
+    // Computing the averages
+    if (type == AFT_INT)
+        for (unsigned int c = 0, n_atoms = 0; c < trajectory.N_configurations; c++)
+        {
+            for (unsigned int a = 0; a < trajectory.N_atoms[c]; a++, n_atoms++) averages[c] += (double) properties[n_atoms].i;
+            averages[c] /= trajectory.N_atoms[c];
+        }
+    else if (type == AFT_DOUBLE)
+        for (unsigned int c = 0, n_atoms = 0; c < trajectory.N_configurations; c++)
+        {
+            for (unsigned int a = 0; a < trajectory.N_atoms[c]; a++, n_atoms++) averages[c] += properties[n_atoms].d;
+            averages[c] /= trajectory.N_atoms[c];
+        }
+    else  // Can not compute the average of string values
     {
-        averages = compute_average_additional(offset, type, trajectory);
-        if (errno != 0) return NULL;
+        free(properties);
+        free(averages);
+        errno = EINVAL;
+        perror("Can not compute the average of string values");
+        return NULL;
     }
 
+    free(properties);
+
     return averages;
 }
 
-double *trajectoryfile_average_property(
-    const struct TrajectoryFile trajectory_file, const unsigned int field)
+double *trajectoryfile_average_property(const struct TrajectoryFile trajectory_file, const unsigned int field)
 {
-    // Initializing
-    struct Trajectory tmp_trajectory;
-    trajectoryfile_read_slice(trajectory_file, 0, 1, &tmp_trajectory);
-    if (errno != 0)
-    {
-        perror(
-            "Error while initializing a trajectory "
-            "(trajectoryfile_average_property.tmp_trajectory)");
-        return NULL;
-    }
-
     // Preparing the array
     double *averages = calloc(trajectory_file.N_configurations, sizeof(double));
     if (averages == NULL)
     {
         errno = ENOMEM;
-        perror(
-            "Error while allocating memory "
-            "(compute_average_property.averages)");
+        perror("Error while allocating memory (trajectoryfile_average_property)");
         return NULL;
     }
 
-    // Transforming the field into an offset
-    size_t offset = tmp_trajectory.atom_builder.offsets[field];
-
-    // Getting the type of data
-    enum AtomFieldType type = tmp_trajectory.atom_builder.fields_types[field];
-
     // Preparing to read
-    unsigned int N_batches = (unsigned int) floor(
-        (double) trajectory_file.N_configurations / trajectory_file.batch_size);
+    unsigned int N_batches = (unsigned int) floor((double) trajectory_file.N_configurations / trajectory_file.batch_size);
     unsigned int remaining_conf = trajectory_file.N_configurations % trajectory_file.batch_size;
 
-    if (!tmp_trajectory.atom_builder.is_additional[field])
+    // Transfering the data
+    for (unsigned int batch = 0; batch < N_batches; batch++)
     {
-        for (unsigned int batch = 0; batch < N_batches; batch++)
+        struct Trajectory trajectory;
+        trajectoryfile_read_slice(trajectory_file, trajectory_file.steps[batch * trajectory_file.batch_size], trajectory_file.batch_size,
+                                  &trajectory);
+        if (errno != 0)  // Could not read slice
         {
-            struct Trajectory trajectory;
-            trajectoryfile_read_slice(
-                trajectory_file,
-                trajectory_file.steps[batch * trajectory_file.batch_size],
-                trajectory_file.batch_size, &trajectory);
-            if (errno != 0)  // Could not read slice
-            {
-                free(averages);
-                perror(
-                    "Error while reading a slice "
-                    "(trajectoryfile_average_property.trajectory)");
-                return NULL;
-            }
-
-            double *tmp = compute_average(offset, type, trajectory);
-            memcpy(averages + batch * trajectory_file.batch_size, tmp, trajectory_file.batch_size * sizeof(double));
-            free(tmp);
             trajectory_delete(&trajectory);
+            free(averages);
+            perror("Error while reading a slice (trajectoryfile_average_property.trajectory)");
+            return NULL;
         }
 
-        if (remaining_conf != 0)
+        double *tmp = trajectory_average_property(trajectory, field);
+        if (tmp == NULL)
         {
-            struct Trajectory trajectory;
-            trajectoryfile_read_slice(
-                trajectory_file,
-                trajectory_file.steps[N_batches * trajectory_file.batch_size],
-                remaining_conf, &trajectory);
-            if (errno != 0)  // Could not read slice
-            {
-                free(averages);
-                perror(
-                    "Error while reading a slice "
-                    "(trajectoryfile_average_property.trajectory)");
-                return NULL;
-            }
-
-            double *tmp = compute_average(offset, type, trajectory);
-            memcpy(averages + N_batches * trajectory_file.batch_size, tmp, remaining_conf * sizeof(double));
-            free(tmp);
             trajectory_delete(&trajectory);
+            free(averages);
+            errno = ENOMEM;
+            perror("Error while computing the average (trajectoryfile_average_property)");
+            return NULL;
         }
+        memcpy(averages + batch * trajectory_file.batch_size, tmp, trajectory_file.batch_size * sizeof(double));
+        free(tmp);
+        trajectory_delete(&trajectory);
     }
-    else
+
+    if (remaining_conf != 0)
     {
-        for (unsigned int batch = 0; batch < N_batches; batch++)
+        struct Trajectory trajectory;
+        trajectoryfile_read_slice(trajectory_file, trajectory_file.steps[N_batches * trajectory_file.batch_size], remaining_conf,
+                                  &trajectory);
+        if (errno != 0)  // Could not read slice
         {
-            struct Trajectory trajectory;
-            trajectoryfile_read_slice(
-                trajectory_file,
-                trajectory_file.steps[batch * trajectory_file.batch_size],
-                trajectory_file.batch_size, &trajectory);
-            if (errno != 0)  // Could not read slice
-            {
-                free(averages);
-                perror(
-                    "Error while reading a slice "
-                    "(trajectoryfile_average_property.trajectory)");
-                return NULL;
-            }
-
-            double *tmp = compute_average_additional(offset, type, trajectory);
-            memcpy(averages + batch * trajectory_file.batch_size, tmp, trajectory_file.batch_size * sizeof(double));
-            free(tmp);
             trajectory_delete(&trajectory);
+            free(averages);
+            perror("Error while reading a slice (trajectoryfile_average_property.trajectory)");
+            return NULL;
         }
 
-        if (remaining_conf != 0)
+        double *tmp = trajectory_average_property(trajectory, field);
+        if (tmp == NULL)
         {
-            struct Trajectory trajectory;
-            trajectoryfile_read_slice(
-                trajectory_file,
-                trajectory_file.steps[N_batches * trajectory_file.batch_size],
-                remaining_conf, &trajectory);
-            if (errno != 0)  // Could not read slice
-            {
-                free(averages);
-                perror(
-                    "Error while reading a slice "
-                    "(trajectoryfile_average_property.trajectory)");
-                return NULL;
-            }
-
-            double *tmp = compute_average_additional(offset, type, trajectory);
-            memcpy(averages + N_batches * trajectory_file.batch_size, tmp, remaining_conf * sizeof(double));
-            free(tmp);
             trajectory_delete(&trajectory);
+            free(averages);
+            errno = ENOMEM;
+            perror("Error while computing the average (trajectoryfile_average_property)");
+            return NULL;
         }
+        memcpy(averages + N_batches * trajectory_file.batch_size, tmp, remaining_conf * sizeof(double));
+        free(tmp);
+        trajectory_delete(&trajectory);
     }
 
-    trajectory_delete(&tmp_trajectory);
     return averages;
 }
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/box.c` & `pylammpstrj-1.0.4a0/src/box.c`

 * *Files identical despite different names*

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/read.c` & `pylammpstrj-1.0.4a0/src/bond.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,577 +1,487 @@
-/**
- * \file
- * Implementation of the reading functions.
- *
- * The API currently implements two versions of the reading function: a serial,
- * and a parallel one.
- */
-#include "read.h"
+#include "bond.h"
+#include "atom.h"
+#include "box.h"
 #include "trajectory.h"
 #include "utils.h"
 
 #include <errno.h>
+#include <stdarg.h>
 #include <stdbool.h>
+#include <stddef.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
-void read_current_step(FILE *input, unsigned long *current_step)
+struct BondTable bondtable_new(const unsigned int N_entries, ...)
 {
-    char dump[BUFFER_LIMIT];
-    long pos = ftell(input);
-    while (fscanf(input, "ITEM: TIMESTEP %lu", current_step) != 1)
-        if (fgets(dump, BUFFER_LIMIT, input) == NULL)
-        {
-            errno = EIO;
-            perror("Error while skipping a line (read_current_step)");
-            return;
-        }
-    fseek(input, pos, SEEK_SET);
+    // Initializing the bond table
+    struct BondTable table = {0};
+    struct BondTableEntry *entries = calloc(N_entries, sizeof(struct BondTableEntry));
+    if (entries == NULL)  // Could not allocate memory
+    {
+        errno = ENOMEM;
+        perror("Error while allocating memory (bondtable_new.entries)");
+        return table;
+    }
+
+    // Parsing the arguments
+    va_list args;
+    va_start(args, N_entries);
+    for (unsigned int e = 0; e < N_entries; e++) entries[e] = va_arg(args, struct BondTableEntry);
+    va_end(args);
+
+    // Transfering the data
+    table.N_entries = N_entries;
+    table.entries = entries;
+    return table;
 }
 
-void read_dump_format(FILE *input, char dump_format[BUFFER_LIMIT])
+double bondtable_get_length_from_types(const struct BondTable table, const void *t1, const void *t2)
 {
-    char line[BUFFER_LIMIT];
-
-    long pos = ftell(input);
-    do
-        if (fgets(line, BUFFER_LIMIT, input) == NULL)
-        {
-            errno = EIO;
-            perror("Error while skipping a line (read_dump_format)");
-            return;
-        }
-    while (strncmp(line, "ITEM: ATOMS", DUMP_FORMAT_OFFSET - 1) != 0);
-
-    strncpy(dump_format, line + DUMP_FORMAT_OFFSET, BUFFER_LIMIT);
-    string_remove_newlines(dump_format, '\0');
-    fseek(input, pos, SEEK_SET);
-}
-
-void read_parameters(FILE **input, const char dump_format[BUFFER_LIMIT],
-                     unsigned int *timestep, unsigned int *N_atoms,
-                     struct Box *box)
-{
-    char line[BUFFER_LIMIT];
-    // Reading the timestep, number of atoms and box flag
-    if (fscanf(*input,
-               "ITEM: TIMESTEP %u ITEM: NUMBER OF ATOMS %u ITEM: BOX BOUNDS "
-               "%" BOX_FLAG_SCANF_LIMIT "c",
-               timestep, N_atoms, box->flag) != 3)  // Something went wrong
+    const unsigned int type1 = *(unsigned int *) t1, type2 = *(unsigned int *) t2;
+    for (unsigned int e = 0; e < table.N_entries; e++)
     {
-        errno = EINVAL;
-        perror(
-            "Error while scanning a line "
-            "(read_parameters.timestep/n_atoms)");
-        return;
+        const struct BondTableEntry entry = table.entries[e];
+        if ((entry.atoms[0].type == type1 && entry.atoms[1].type == type2) ||
+            (entry.atoms[1].type == type1 && entry.atoms[0].type == type2))
+            return entry.length;
     }
 
-    // Reading the box bounds
-    for (unsigned int b = 0; b < BOX_BOUNDS_LIMIT; b++)
-        if (fscanf(*input, " %lf ", box->bounds + b) !=
-            1)  // Something went wrong
-        {
-            errno = EINVAL;
-            perror(
-                "Error while scanning a line "
-                "(read_parameters.box.bounds)");
-            return;
-        }
+    fprintf(stderr, "Warning: Type not found in table\n");
+    return 0.;
+}
 
-    // Checking the dump format
-    if (fgets(line, BUFFER_LIMIT, *input) == NULL)  // Could not read line
+double bondtable_get_length_from_elements(const struct BondTable table, const void *e1, const void *e2)
+{
+    const char *element1 = (char *) e1, *element2 = (char *) e2;
+    for (unsigned int e = 0; e < table.N_entries; e++)
     {
-        perror("Error while scanning a line (read_parameters.line)");
-        return;
+        const struct BondTableEntry entry = table.entries[e];
+        if ((strncmp(element1, entry.atoms[0].element, LABEL_LIMIT) == 0 && strncmp(element2, entry.atoms[1].element, LABEL_LIMIT) == 0) ||
+            (strncmp(element1, entry.atoms[1].element, LABEL_LIMIT) == 0 && strncmp(element2, entry.atoms[0].element, LABEL_LIMIT) == 0))
+            return entry.length;
     }
-    string_remove_newlines(line, '\0');
-    if (strncmp(line + DUMP_FORMAT_OFFSET, dump_format, BUFFER_LIMIT) !=
-        0)  // Dump formats don't match
+
+    // fprintf(stderr, "Warning: Type not found in table\n");
+    return 0.;
+}
+
+void bondtable_copy(const struct BondTable src, struct BondTable *dest)
+{
+    dest->N_entries = src.N_entries;
+    dest->entries = calloc(src.N_entries, sizeof(struct BondTableEntry));
+    if (dest->entries == NULL)  // Could not allocate memory
     {
-        errno = EINVAL;
-        perror("Error while scanning the dump format (read_parameters.line)");
+        errno = ENOMEM;
+        perror("Error while allocating memory (bondtable_copy)");
         return;
     }
+
+    memcpy(dest->entries, src.entries, src.N_entries * sizeof(struct BondTableEntry));
 }
 
-void read_atoms(FILE **input, const struct AtomBuilder atom_builder,
-                const unsigned int N_atoms, struct Atom *atoms)
+void bondtable_delete(struct BondTable *table)
 {
-    char line[BUFFER_LIMIT];
-
-    // Reading the atoms
-    for (unsigned int a = 0; a < N_atoms; a++)
-    {
-        if (fgets(line, BUFFER_LIMIT, *input) == NULL)  // Could not read line
-        {
-            for (unsigned int at = 0; at < a - 1; at++) atom_delete(atoms + at);
-            perror(
-                "Error while scanning an atom line"
-                "(read_atoms.line)");
-            errno = EINVAL;
-            return;
-        }
-
-        atoms[a] = read_atom_entry(atom_builder, line);
-        if (errno != 0)  // Something went wrong
-        {
-            for (unsigned int at = 0; at < a; at++) atom_delete(atoms + at);
-            perror(
-                "Error while reading an atom entry "
-                "(read_atoms.read_atom_entry)");
-            errno = EINVAL;
-            return;
-        }
-    }
+    if (table->entries != NULL) free(table->entries);
 }
 
-void trajectory_read(const char *file_name, const unsigned long start,
-                     const char *user_format, struct Trajectory *trajectory)
+struct BondMap bondmap_new(const struct BondTable table, const bool by_type)
 {
-    // To store the error value
-    int errsv;
+    struct BondMap map = {0};
+    map.seed = 31;
+    if (by_type)
+        for (unsigned int e = 0; e < table.N_entries; e++)
+            map.table[bondmap_hash_types(&(table.entries[e].atoms[0].type), &(table.entries[e].atoms[1].type))] = table.entries[e].length;
+    else
+        for (unsigned int e = 0; e < table.N_entries; e++)
+            map.table[bondmap_hash_elements(&(table.entries[e].atoms[0].element), &(table.entries[e].atoms[1].element))] =
+                table.entries[e].length;
+    return map;
+}
 
-    // Opening the file
-    FILE *input = fopen(file_name, "r");
-    if (input == NULL)  // File could not be open
-    {
-        errno = EIO;
-        perror("Error while opening the file (trajectory_read)");
-        return;
-    }
+unsigned int bondmap_hash_types(void *t1, void *t2) { return (*(unsigned int *) t1 * *(unsigned int *) t2) % BOND_MAP_SIZE; }
 
-    // Skipping the first configurations
-    trajectory_skip(&input, start);
-    if (errno != 0)  // Something went wrong
+unsigned int bondmap_hash_elements(void *e1, void *e2)
+{
+    unsigned int element1 = 0, element2 = 0;
+    for (unsigned int c = 0; c < LABEL_LIMIT; c++)
     {
-        perror("Error while skipping configurations (trajectory_read)");
-        fclose(input);
-        return;
+        element1 += (unsigned int) *(char *) (e1 + c);
+        element2 += (unsigned int) *(char *) (e2 + c);
     }
+    return (element1 * element2) % BOND_MAP_SIZE;
+}
 
-    // Getting the current step
-    unsigned long current_step;
-    read_current_step(input, &current_step);
-    if (errno != 0)  // Could not read the current timestep
-    {
-        errsv = errno;
-        fclose(input);
-        errno = errsv;
-        perror("Error while reading the current step (trajectory_read)");
-        return;
-    }
+struct BondBuilder bondbuilder_new(const char *file_name, const enum BondMode mode, const enum BondSource source,
+                                   const struct BondTable table)
+{
+    struct BondBuilder bond_builder = {0};
+    if (file_name != NULL) strncpy(bond_builder.file_name, file_name, BUFFER_LIMIT - 1);
+    bond_builder.mode = mode;
+    bond_builder.source = source;
+    bond_builder.table = table;
+    return bond_builder;
+}
 
-    // Getting the dump format
-    char dump_format[BUFFER_LIMIT];
-    if (user_format == NULL)
-    {
-        read_dump_format(input, dump_format);
-        if (errno != 0)  // Could not read the dump format
-        {
-            errsv = errno;
-            fclose(input);
-            errno = errsv;
-            perror("Error while reading the dump format (trajectory_read)");
-            return;
-        }
-    }
-    else
+void bondbuilder_init(struct BondBuilder *bond_builder, const char *file_name, const enum BondMode mode, const enum BondSource source,
+                      const struct BondTable table)
+{
+    if (file_name != NULL)
     {
-        strncpy(dump_format, user_format, BUFFER_LIMIT);
-        string_remove_newlines(dump_format, '\0');
+        strncpy(bond_builder->file_name, file_name, FILE_NAME_LIMIT - 1);
+        bond_builder->file_name[FILE_NAME_LIMIT - 1] = '\0';
     }
 
-    // Initializing the atom builder
-    struct AtomBuilder atom_builder = atom_builder_new(dump_format, input);
-    if (errno != 0)  // Something went wrong
-    {
-        perror("Error while creating the atom builder (trajectory_read)");
-        fclose(input);
-        return;
-    }
+    bond_builder->mode = mode;
+    bond_builder->source = source;
+    bondtable_copy(table, &(bond_builder->table));
+    if (errno != 0) perror("Error while copying the bond table (bondbuilder_init)");
+}
 
-    // Preparing the arrays
-    unsigned int *N_atoms =
-        malloc(BASE_N_CONFIGURATIONS * sizeof(unsigned int));
-    if (N_atoms == NULL)  // Allocation failed
-    {
-        atom_builder_delete(&atom_builder);
-        fclose(input);
-        errno = ENOMEM;
-        perror("Error while allocating memory (trajectory_read.N_atoms)");
-        return;
-    }
-    unsigned int *steps = malloc(BASE_N_CONFIGURATIONS * sizeof(unsigned int));
-    if (steps == NULL)
+void bondbuilder_copy(const struct BondBuilder src, struct BondBuilder *dest)
+{
+    bondbuilder_init(dest, src.file_name, src.mode, src.source, src.table);
+}
+
+void bondbuilder_read_bond_entry(const struct BondBuilder bond_builder, char line[BUFFER_LIMIT], struct Atom *atom)
+{
+    char *start = line;
+    unsigned int id = 0, type = 0, N_bonds = 0, *bonded_ids = NULL;
+    double *bonded_bos = NULL;
+    double total_bo = 0.;
+    if (sscanf(line, " %u %u %u ", &id, &type, &N_bonds) != 3)  // Could not read the fields
     {
-        free(N_atoms);
-        atom_builder_delete(&atom_builder);
-        fclose(input);
-        errno = ENOMEM;
-        perror("Error while allocating memory (trajectory_read.steps)");
+        errno = EIO;
+        perror("Error while scanning the first fields (bondbuilder_read_bond_entry)");
         return;
     }
-    struct Box *boxes = malloc(BASE_N_CONFIGURATIONS * sizeof(struct Box));
-    if (boxes == NULL)  // Allocation failed
+
+    if (id != atom->id)  // Lines don't match
     {
-        free(steps);
-        free(N_atoms);
-        atom_builder_delete(&atom_builder);
-        fclose(input);
-        errno = ENOMEM;
-        perror("Error while allocating memory (trajectory_read.boxes)");
+        errno = EINVAL;
+        perror("Error while checking the atom index (bondbuilder_read_bond_entry)");
         return;
     }
-    unsigned long boxes_size = BASE_N_CONFIGURATIONS;
-    struct Atom *atoms = NULL;
-    unsigned long atoms_size = 0;
-
-    // Preparing the variables
-    unsigned long N_configurations = 0;
-    unsigned long total_atoms = 0;  // To keep track of the number of atoms read
-
-    // Reading
-    int chr = fgetc(input);
-    while (chr != EOF)
-    {
-        ungetc(chr, input);
 
-        // Reallocating memory
-        if (N_configurations == boxes_size)
+    // Skipping the first 3 fields (the ones already read)
+    for (unsigned int f = 0; f < 3 + 1; f++)  // Need to add 1 bc of implementation of function
+        start = str_go_to_next(start, ' ');
+
+    if (N_bonds != 0)
+    {
+        // Reading the bonded IDs
+        if (bond_builder.mode == BM_ID || bond_builder.mode == BM_FULL)
         {
-            unsigned int *new_N_atoms =
-                realloc(N_atoms, (boxes_size + N_CONFIGURATIONS_INCR) *
-                                     sizeof(unsigned int));
-            if (new_N_atoms == NULL)  // Could not realloc memory
+            bonded_ids = calloc(N_bonds, sizeof(unsigned int));
+            if (bonded_ids == NULL)  // Could not allocate memory
             {
-                for (unsigned int a = 0; a < total_atoms; a++)
-                    atom_delete(atoms + a);
-                if (atoms != NULL) free(atoms);
-                free(boxes);
-                free(steps);
-                free(N_atoms);
-                atom_builder_delete(&atom_builder);
-                fclose(input);
                 errno = ENOMEM;
-                perror(
-                    "Error while reallocating memory "
-                    "(trajectory_read.N_atoms)");
+                perror("Error while allocating the bond array (bondbuilder_read_bond_entry)");
                 return;
             }
-            N_atoms = new_N_atoms;
 
-            unsigned int *new_steps =
-                realloc(steps, (boxes_size + N_CONFIGURATIONS_INCR) *
-                                   sizeof(unsigned int));
-            if (new_steps == NULL)  // Could not realloc memory
+            for (unsigned int b = 0; b < N_bonds; b++)
             {
-                for (unsigned int a = 0; a < total_atoms; a++)
-                    atom_delete(atoms + a);
-                if (atoms != NULL) free(atoms);
-                free(boxes);
-                free(steps);
-                free(N_atoms);
-                atom_builder_delete(&atom_builder);
-                fclose(input);
-                errno = ENOMEM;
-                perror(
-                    "Error while reallocating memory (trajectory_read.steps)");
-                return;
+                if (sscanf(start, " %u ", &(bonded_ids[b])) != 1)
+                {
+                    free(bonded_ids);
+                    errno = EIO;
+                    perror("Error while scanning a bonded id (bondbuilder_read_bond_entry)");
+                    return;
+                }
+                start = str_go_to_next(start, ' ');
             }
-            steps = new_steps;
+        }
 
-            struct Box *new_boxes =
-                realloc(boxes, (boxes_size + N_CONFIGURATIONS_INCR) *
-                                   sizeof(struct Box));
-            if (new_boxes == NULL)  // Could not realloc memory
+        // Reading the bond orders
+        if (bond_builder.mode == BM_BOND_ORDER || bond_builder.mode == BM_FULL)
+        {
+            // We allocate one more slot to also store the sum
+            bonded_bos = calloc(N_bonds, sizeof(double));
+            if (bonded_bos == NULL)
             {
-                for (unsigned int a = 0; a < total_atoms; a++)
-                    atom_delete(atoms + a);
-                if (atoms != NULL) free(atoms);
-                free(boxes);
-                free(steps);
-                free(N_atoms);
-                atom_builder_delete(&atom_builder);
-                fclose(input);
+                free(bonded_ids);
                 errno = ENOMEM;
-                perror(
-                    "Error while reallocating memory (trajectory_read.boxes)");
+                perror("Error while allocating the bond orders array (bondbuiler_read_bond_entry)");
                 return;
             }
-            boxes = new_boxes;
-
-            boxes_size += N_CONFIGURATIONS_INCR;
-        }
 
-        read_parameters(&input, dump_format, steps + N_configurations,
-                        N_atoms + N_configurations, boxes + N_configurations);
-        if (errno != 0)  // Could not read parameters
-        {
-            errsv = errno;
-            for (unsigned int a = 0; a < total_atoms; a++)
-                atom_delete(atoms + a);
-            if (atoms != NULL) free(atoms);
-            free(boxes);
-            free(steps);
-            free(N_atoms);
-            atom_builder_delete(&atom_builder);
-            fclose(input);
-            errno = errsv;
-            perror(
-                "Error while reading the configuration parameters "
-                "(trajectory_read)");
-            return;
-        }
+            start = str_go_to_next(start, ' ');  // Skip an unused field (mol id)
+            start = str_skip_spaces(start);
+            for (unsigned int b = 0; b < N_bonds; b++)
+            {
+                if (sscanf(start, " %lf ", &(bonded_bos[b])) != 1)
+                {
+                    free(bonded_ids);
+                    free(bonded_bos);
+                    errno = EIO;
+                    perror("Error while scanning a bond order (bondbuilder_read_bond_entry)");
+                    return;
+                }
+                start = str_go_to_next(start, ' ');
+                start = str_skip_spaces(start);
+            }
 
-        // Reallocating memory
-        {
-            struct Atom *new_atoms =
-                realloc(atoms, (atoms_size + N_atoms[N_configurations]) *
-                                   sizeof(struct Atom));
-            if (new_atoms == NULL)
+            if (sscanf(start, " %lf ", &total_bo) != 1)
             {
-                for (unsigned int a = 0; a < total_atoms; a++)
-                    atom_delete(atoms + a);
-                if (atoms != NULL) free(atoms);
-                free(N_atoms);
-                free(steps);
-                free(boxes);
-                atom_builder_delete(&atom_builder);
-                fclose(input);
-                errno = ENOMEM;
-                perror(
-                    "Error while reallocating memory (trajectory_read.atoms)");
+                free(bonded_ids);
+                free(bonded_bos);
+                errno = EIO;
+                perror("Error while scanning the total bond order (bondbuilder_read_bond_entry)");
                 return;
             }
-            atoms = new_atoms;
-            atoms_size += N_atoms[N_configurations];
         }
-
-        read_atoms(&input, atom_builder, N_atoms[N_configurations],
-                   atoms + total_atoms);
-        if (errno != 0)  // Could not read the atoms
-        {
-            errsv = errno;
-            for (unsigned int at = 0; at <= total_atoms; at++)
-                atom_delete(atoms + at);
-            if (atoms != NULL) free(atoms);
-            free(boxes);
-            free(steps);
-            free(N_atoms);
-            atom_builder_delete(&atom_builder);
-            fclose(input);
-            errno = errsv;
-            perror(
-                "Error while reading the atoms of the configuration "
-                "(trajectory_read)");
-            return;
-        }
-        total_atoms += N_atoms[N_configurations];
-
-        N_configurations++;
-        chr = fgetc(input);
     }
 
-    fclose(input);
-    trajectory_init(trajectory, atom_builder, N_configurations, steps, N_atoms,
-                    boxes, atoms);
+    // Transfering the data
+    atom->type = type;
+    atom->N_bonds = N_bonds;
+    atom->ids = bonded_ids;
+    atom->bond_orders = bonded_bos;
+    atom->total_bo = total_bo;
 }
 
-void trajectoryfile_read_slice(struct TrajectoryFile trajectory_file,
-                               unsigned long start,
-                               unsigned long N_configurations,
-                               struct Trajectory *trajectory)
+void bondbuilder_delete(struct BondBuilder *builder) { bondtable_delete(&(builder->table)); }
+
+void trajectory_compute_bonds(struct Trajectory *trajectory, const struct BondTable table)
 {
-    // To store an error value
-    int errsv;
+    // Getting the atoms types checking attribute (either type or label)
+    bool flag = (bool) trajectory->atoms[0].type;
 
-    // Opening the file
-    FILE *input = fopen(trajectory_file.file_name, "r");
-    if (input == NULL)
+    // Preparing to compute the optimizations
+    unsigned long *N_atoms_so_far = malloc(trajectory->N_configurations * sizeof(unsigned long));
+    if (N_atoms_so_far == NULL)  // Could not allocate memory
     {
-        errno = EIO;
-        perror("Error while opening the trajectory file (trajectoryfile_read)");
+        errno = ENOMEM;
+        perror("Error while allocating memory (trajectory_compute_bonds.N_atoms_so_far)");
         return;
     }
 
-    // Moving to the right configuration
-    long pos = 0;
-    for (unsigned int c = 0; c < trajectory_file.N_configurations; c++)
-        if (trajectory_file.steps[c] >= start)
+    unsigned int offset = 0;
+    unsigned int N_max_atoms = 0, N_traversed = 0;
+    for (unsigned int c = 0; c < trajectory->N_configurations; c++)
+    {
+        if (c == 0)
+            N_atoms_so_far[c] = 0;
+        else
+            N_atoms_so_far[c] = N_traversed;
+        if (N_max_atoms < trajectory->N_atoms[c])
         {
-            pos = trajectory_file.conf_pos[c];
-            break;
+            N_max_atoms = trajectory->N_atoms[c];
+            offset = N_traversed;
         }
-    fseek(input, pos, SEEK_SET);
+        N_traversed += trajectory->N_atoms[c];
+    }
 
-    // Getting the dump format
-    char dump_format[BUFFER_LIMIT];
-    if (trajectory_file.user_format[0] == '\0')
+    // Using a hash table to match types to bond lengths
+    struct BondMap map = bondmap_new(table, flag);
+    unsigned int (*hash)(void *a, void *b) = NULL;
+    size_t type_offset = 0;
+
+    if (flag)
     {
-        read_dump_format(input, dump_format);
-        if (errno != 0)
-        {
-            errsv = errno;
-            fclose(input);
-            errno = errsv;
-            perror("Error while reading the dump format");
-            return;
-        }
+        hash = &bondmap_hash_types;
+        type_offset = offsetof(struct Atom, type);
     }
     else
     {
-        strncpy(dump_format, trajectory_file.user_format, BUFFER_LIMIT);
-        string_remove_newlines(dump_format, '\0');
+        hash = &bondmap_hash_elements;
+        type_offset = offsetof(struct Atom, label);
     }
 
-    // Initializing the atom builder
-    struct AtomBuilder atom_builder = atom_builder_new(dump_format, input);
-    if (errno != 0)  // Something went wrong
+    // Using a mask to optimize the first atom loop
+    bool *mask = calloc(N_max_atoms, sizeof(bool));
+    if (mask == NULL)  // Could not allocate memory
     {
-        perror("Error while creating the atom builder (trajectoryfile_read)");
-        fclose(input);
+        errno = ENOMEM;
+        perror("Error while allocating memory (trajectory_compute_bonds.mask)");
         return;
     }
 
-    // Preparing the arrays
-    unsigned int *N_atoms = malloc(N_configurations * sizeof(unsigned int));
-    if (N_atoms == NULL)  // Allocation failed
+    int skip = 0;
+#pragma omp parallel for
+    for (unsigned int a = 0; a < N_max_atoms; a++)
     {
-        atom_builder_delete(&atom_builder);
-        fclose(input);
-        errno = ENOMEM;
-        perror("Error while allocating memory (trajectoryfile_read.N_atoms)");
-        return;
+        if (skip) continue;
+        const struct Atom atom = trajectory->atoms[offset + a];
+        for (unsigned int e = 0; e < table.N_entries; e++)
+        {
+            const struct BondTableEntry entry = table.entries[e];
+            if (atom.id - 1 >= N_max_atoms)
+            {
+                skip = EINVAL;
+                break;
+            }
+            // mask[atom.id - 1] = (atom.type == entry.atoms[0].type) || (atom.type == entry.atoms[1].type) ||
+            //                     (strncmp(atom.label, entry.atoms[0].element, LABEL_LIMIT) == 0) ||
+            //                     (strncmp(atom.label, entry.atoms[1].element, LABEL_LIMIT) == 0);
+            mask[atom.id - 1] = flag ? ((atom.type == entry.atoms[0].type) || (atom.type == entry.atoms[1].type))
+                                     : ((strncmp(atom.label, entry.atoms[0].element, LABEL_LIMIT) == 0) ||
+                                        (strncmp(atom.label, entry.atoms[1].element, LABEL_LIMIT) == 0));
+            if (mask[atom.id - 1]) break;
+        }
     }
-    unsigned int *steps = malloc(N_configurations * sizeof(unsigned int));
-    if (steps == NULL)
+
+    if (skip)
     {
-        free(N_atoms);
-        atom_builder_delete(&atom_builder);
-        fclose(input);
-        errno = ENOMEM;
-        perror("Error while allocating memory (trajectoryfile_read.steps)");
+        free(mask);
+        errno = skip;
+        perror("Error while computing the mask (trajectory_compute_bonds)");
         return;
     }
-    struct Box *boxes = malloc(N_configurations * sizeof(struct Box));
-    if (boxes == NULL)  // Allocation failed
+
+
+#pragma omp parallel for
+    for (unsigned int c = 0; c < trajectory->N_configurations; c++)
     {
-        free(steps);
-        free(N_atoms);
-        atom_builder_delete(&atom_builder);
-        fclose(input);
-        errno = ENOMEM;
-        perror("Error while allocating memory (trajectoryfile_read.boxes)");
-        return;
-    }
-    struct Atom *atoms = NULL;
-    unsigned long atoms_size = 0;
+        if (skip) continue;
+        // Trying to use the cache thangs, stack or sum like this...
+        struct Atom *atoms = trajectory->atoms + N_atoms_so_far[c];
+        unsigned int N_atoms = trajectory->N_atoms[c];
+        double box_lengths[3] = {0};
+        for (unsigned int d = 0; d < 3; d++) box_lengths[d] = trajectory->box[c].bounds[2 * d + 1] - trajectory->box[c].bounds[2 * d];
 
-    // Preparing the variables
-    unsigned long n_configurations = 0;
-    unsigned long total_atoms = 0;  // To keep track of the number of atoms read
-
-    // Reading
-    int chr = fgetc(input);
-    while (chr != EOF && n_configurations < N_configurations)
-    {
-        ungetc(chr, input);
-
-        // Reading the parameters: `N_atoms`, `box.flags`, `box.bounds`
-        read_parameters(&input, dump_format, steps + n_configurations,
-                        N_atoms + n_configurations, boxes + n_configurations);
-        if (errno != 0)  // Could not read parameters
+        for (unsigned int i = 0; i < N_atoms; i++)
         {
-            errsv = errno;
-            if (atoms != NULL)
+            struct Atom *a1 = atoms + i;
+            if (!mask[a1->id - 1] || skip) continue;
+            for (unsigned int j = i + 1; j < N_atoms; j++)
             {
-                for (unsigned int a = 0; a < total_atoms; a++)
-                    atom_delete(atoms + a);
-                free(atoms);
-            }
-            free(boxes);
-            free(steps);
-            free(N_atoms);
-            atom_builder_delete(&atom_builder);
-            fclose(input);
-            errno = errsv;
-            perror(
-                "Error while reading the configuration parameters "
-                "(trajectoryfile_read)");
-            return;
-        }
+                struct Atom *a2 = atoms + j;
 
-        // Reallocating memory for the atoms
-        {
-            // Allocating the new block of memory
-            struct Atom *new_atoms =
-                realloc(atoms, (atoms_size + N_atoms[n_configurations]) *
-                                   sizeof(struct Atom));
-            if (new_atoms == NULL)  // Reallocation failed
-            {
-                if (atoms != NULL)
+                // Gathering the bond length
+                double length = map.table[hash((void *) a1 + type_offset, (void *) a2 + type_offset)];
+
+                if (length != 0. && atom_compute_distance(box_lengths, *a1, *a2) <= length * length)
                 {
-                    for (unsigned int a = 0; a < total_atoms;
-                         a++)  // Freeing all the atoms read so far
-                        atom_delete(atoms + a);
-                    free(atoms);
+                    // Modifying the bonds lists
+                    if (a1->N_bonds == 0)
+                    {
+                        unsigned int *new_ids = realloc(a1->ids, N_BONDS_LIMIT * sizeof(unsigned int));
+                        if (new_ids == NULL)  // Could not reallocate memory
+                        {
+#pragma omp critical
+                            skip = ENOMEM;
+                            perror("Error while reallocating memory (trajectory_compute_bonds.new_ids)");
+                            break;
+                        }
+                        a1->ids = new_ids;
+                    }
+                    else if (a1->N_bonds % N_BONDS_LIMIT == N_BONDS_LIMIT - 1)
+                    {
+                        unsigned int *new_ids = realloc(a1->ids, (a1->N_bonds + 1 + N_BONDS_LIMIT) * sizeof(unsigned int));
+                        if (new_ids == NULL)  // Could not reallocate memory
+                        {
+#pragma omp critical
+                            skip = ENOMEM;
+                            perror("Error while reallocating memory (trajectory_compute_bonds.new_ids)");
+                            break;
+                        }
+                        a1->ids = new_ids;
+                    }
+                    a1->ids[a1->N_bonds] = a2->id;
+                    (a1->N_bonds)++;
+
+                    if (a2->N_bonds == 0)
+                    {
+                        unsigned int *new_ids = realloc(a2->ids, N_BONDS_LIMIT * sizeof(unsigned int));
+                        if (new_ids == NULL)  // Could not reallocate memory
+                        {
+#pragma omp critical
+                            skip = ENOMEM;
+                            perror("Error while reallocating memory (trajectory_compute_bonds.new_ids)");
+                            break;
+                        }
+                        a2->ids = new_ids;
+                    }
+                    else if (a2->N_bonds % N_BONDS_LIMIT == N_BONDS_LIMIT - 1)
+                    {
+                        unsigned int *new_ids = realloc(a2->ids, (a2->N_bonds + 1 + N_BONDS_LIMIT) * sizeof(unsigned int));
+                        if (new_ids == NULL)  // Could not reallocate memory
+                        {
+#pragma omp critical
+                            skip = ENOMEM;
+                            perror("Error while reallocating memory (trajectory_compute_bonds.new_ids)");
+                            break;
+                        }
+                        a2->ids = new_ids;
+                    }
+                    a2->ids[a2->N_bonds] = a1->id;
+                    (a2->N_bonds)++;
                 }
-                free(N_atoms);
-                free(steps);
-                free(boxes);
-                atom_builder_delete(&atom_builder);
-                fclose(input);
-                errno = ENOMEM;
-                perror(
-                    "Error while reallocating memory "
-                    "(trajectoryfile_read.atoms)");
-                return;
             }
-            atoms = new_atoms;
-            atoms_size += N_atoms[n_configurations];
         }
+    }
 
-        // Reading the atoms
-        read_atoms(&input, atom_builder, N_atoms[n_configurations],
-                   atoms + total_atoms);
-        if (errno != 0)  // Could not read the atoms
-        {
-            errsv = errno;
-            if (atoms != NULL)
-            {
-                for (unsigned int at = 0; at < total_atoms; at++)
-                    atom_delete(atoms + at);
-                free(atoms);
-            }
-            free(boxes);
-            free(steps);
-            free(N_atoms);
-            atom_builder_delete(&atom_builder);
-            fclose(input);
-            errno = errsv;
-            perror(
-                "Error while reading the atoms of the configuration "
-                "(trajectoryfile_read)");
-            return;
-        }
-        total_atoms += N_atoms[n_configurations];
+    free(mask);
+    free(N_atoms_so_far);
 
-        n_configurations++;
-        chr = fgetc(input);
+    if (skip)
+    {
+        errno = skip;
+        return;
     }
 
-    fclose(input);
-    trajectory_init(trajectory, atom_builder, N_configurations, steps, N_atoms,
-                    boxes, atoms);
-    for (unsigned int s = 0; s < trajectory_file.N_selections; s++)
+    // Initializing the bond builder
+    bondbuilder_init(&(trajectory->bond_builder), NULL, BM_ID, BS_COMPUTE, table);
+}
+
+void trajectory_write_bonds(const struct Trajectory trajectory, const char *file_name)
+{
+    // Opening the file
+    FILE *output = NULL;
+    if (file_name == NULL || strcmp(file_name, "stdout") == 0)  // Enable outputting to stdout
+        output = stdout;
+    else
+        output = fopen(file_name, "w");
+    if (output == NULL)
+    {
+        perror("Error while opening the file (trajectory_write_bonds)");
+        return;
+    }
+
+    // Preparing for writing
+    bool flag = (bool) trajectory.atoms[0].type;  // if 0 then flag is false
+
+    // Writing the bonds
+    fprintf(output, "# id");
+
+    if (flag)
+        fprintf(output, " type");
+    else
+        fprintf(output, " element");
+
+    fprintf(output, " N_bonds id_0...id_N\n");
+    unsigned long a = 0;
+    for (unsigned int c = 0; c < trajectory.N_configurations; c++)
     {
-        select_atoms(trajectory, trajectory_file.parameters[s].field, trajectory_file.parameters[s].op, trajectory_file.parameters[s].value, (bool) 1, NULL);
-        if (errno != 0)  // Could not select atoms
+        const struct Atom *atoms = trajectory.atoms + a;
+        const unsigned int N_atoms = trajectory.N_atoms[c];
+        fprintf(output, "# Timestep: %u\n# Number of atoms: %u\n", trajectory.steps[c], N_atoms);
+        for (unsigned int i = 0; i < N_atoms; i++)
         {
-            trajectory_delete(trajectory);
-            trajectoryfile_delete(&trajectory_file);
-            perror("Error while selecting atoms (trajectoryfile_read_slice)");
-            return;
+            const struct Atom atom = atoms[i];
+
+            // The id
+            fprintf(output, " %u", atom.id);
+
+            // The type or element
+            if (flag)
+                fprintf(output, " %u", atom.type);
+            else
+                fprintf(output, " %s", atom.label);
+
+            // The number of bonds
+            fprintf(output, " %u", atom.N_bonds);
+
+            // The bonded ids
+            for (unsigned int b = 0; b < atom.N_bonds; b++) fprintf(output, " %u", atom.ids[b]);
+
+            fprintf(output, "\n");
         }
+        a += N_atoms;
     }
+
+    // Closing the file
+    fclose(output);
 }
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/skip.c` & `pylammpstrj-1.0.4a0/src/skip.c`

 * *Files 4% similar despite different names*

```diff
@@ -17,38 +17,37 @@
     do
     {
         starting_pos = ftell(*input);
 
         // Reading the current timestep and number of atoms
         if (fscanf(*input,
                    "ITEM: TIMESTEP %lu ITEM: NUMBER OF ATOMS %u ITEM: BOX "
-                   "BOUNDS %*" BOX_FLAG_SCANF_LIMIT "c",
+                   "BOUNDS %*" BOX_FLAG_SCANF_LIMIT "c\n",
                    &current_step, &N_atoms) != 2)
         {
             errno = EINVAL;
             if (feof(*input))
                 perror("Error reached end of file (trajectory_skip)");
             else
                 perror("Error while scanning a line (trajectory_skip)");
             return;
         }
 
-        double bound;
-        for (unsigned int b = 0; b < BOX_BOUNDS_LIMIT; b++)
-            if (fscanf(*input, " %lf ", &bound) != 1)
+        for (unsigned int b = 0; b < BOX_BOUNDS_LIMIT / 2; b++)
+            if (fgets(dump, BUFFER_LIMIT, *input) == NULL)
             {
-                errno = EINVAL;
-                perror("Error while dumping the box bounds (trajectory_skip)");
+                errno = EIO;
+                perror("Error while skipping the box bounds (trajectory_skip)");
                 return;
             }
 
         if (fgets(dump, BUFFER_LIMIT, *input) == NULL)
         {
             errno = EIO;
-            perror("Error while dumping the dumping format (trajectory_skip)");
+            perror("Error while skipping the dumping format (trajectory_skip)");
             return;
         }
 
         if (current_step >= start)
         {
             // Returning to the start position
             fseek(*input, starting_pos, SEEK_SET);
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/lammpstrj/trajectoryfile.c` & `pylammpstrj-1.0.4a0/src/trajectoryfile.c`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 #include "utils.h"
 
 #include <errno.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
-struct TrajectoryFile trajectoryfile_new(const char *file_name,
-                                         const char *user_format,
-                                         const unsigned int batch_size)
+struct TrajectoryFile trajectoryfile_new(const char *file_name, const char *user_format, const unsigned int batch_size)
 {
-    struct TrajectoryFile trajectory_file = {
-        .file_name = {0}, .N_configurations = 0, .conf_pos = NULL};
+    struct TrajectoryFile trajectory_file = {.file_name = {0}, .N_configurations = 0, .conf_pos = NULL};
 
     // Reading the file
     FILE *input = fopen(file_name, "r");
     if (input == NULL)  // File could not be open
     {
         errno = EIO;
         perror("Error while opening the file (trajectoryfile_new)");
@@ -26,16 +23,15 @@
     // Preparing to read
     char dump[BUFFER_LIMIT] = {0};
     unsigned long N_configurations = 0;
     unsigned long step;
     long pos;
 
     // Allocating memory
-    unsigned long *steps =
-        malloc(BASE_N_CONFIGURATIONS * sizeof(unsigned long));
+    unsigned long *steps = malloc(BASE_N_CONFIGURATIONS * sizeof(unsigned long));
     if (steps == NULL)
     {
         fclose(input);
         errno = ENOMEM;
         perror("Error while allocating memory (trajectoryfile_new.steps)");
         return trajectory_file;
     }
@@ -54,32 +50,29 @@
     while (chr != EOF)
     {
         ungetc(chr, input);
 
         // Reallocating memory if necessary
         if (N_configurations >= steps_size)
         {
-            unsigned long *new_steps =
-                realloc(steps, (steps_size + N_CONFIGURATIONS_INCR) *
-                                   sizeof(unsigned long));
+            unsigned long *new_steps = realloc(steps, (steps_size + N_CONFIGURATIONS_INCR) * sizeof(unsigned long));
             if (new_steps == NULL)
             {
                 free(conf_pos);
                 free(steps);
                 fclose(input);
                 errno = ENOMEM;
                 perror(
                     "Error while reallocating memory "
                     "(trajectoryfile_new.new_steps)");
                 return trajectory_file;
             }
             steps = new_steps;
 
-            long *new_conf_pos = realloc(
-                conf_pos, (steps_size + N_CONFIGURATIONS_INCR) * sizeof(long));
+            long *new_conf_pos = realloc(conf_pos, (steps_size + N_CONFIGURATIONS_INCR) * sizeof(long));
             if (new_conf_pos == NULL)  // Could not reallocate memory
             {
                 free(conf_pos);
                 fclose(input);
                 errno = ENOMEM;
                 perror(
                     "Error while reallocating memory "
@@ -98,15 +91,17 @@
             {
                 free(conf_pos);
                 free(steps);
                 fclose(input);
                 perror("Error while reading a line (trajectoryfile_new.dump)");
                 return trajectory_file;
             }
-            fscanf(input, " %lu ", &step);  // res doesn't need to be checked
+            if (fscanf(input, " %lu ", &step) != 1)
+            {
+            }                                                             // res doesn't need to be checked
         } while (strcmp(dump, "ITEM: TIMESTEP\n") != 0 && !feof(input));  // it is checked here
 
         // Reached end of file
         if (feof(input)) break;
 
         // Saving the data
         steps[N_configurations] = step;
@@ -116,59 +111,56 @@
         chr = fgetc(input);
     }
     fclose(input);
 
     // Resizing the array
     if (steps_size != N_configurations)
     {
-        unsigned long *new_steps =
-            realloc(steps, (steps_size + N_CONFIGURATIONS_INCR) *
-                               sizeof(unsigned long));
+        unsigned long *new_steps = realloc(steps, (steps_size + N_CONFIGURATIONS_INCR) * sizeof(unsigned long));
         if (new_steps == NULL)
         {
             free(conf_pos);
             free(steps);
-            fclose(input);
             errno = ENOMEM;
-            perror(
-                "Error while reallocating memory "
-                "(trajectoryfile_new.new_steps)");
+            perror("Error while reallocating memory (trajectoryfile_new.new_steps)");
             return trajectory_file;
         }
         steps = new_steps;
 
         long *new_conf_pos = realloc(conf_pos, N_configurations * sizeof(long));
         if (new_conf_pos == NULL)  // Could not reallocate memory
         {
             free(conf_pos);
             free(steps);
-            fclose(input);
             errno = ENOMEM;
-            perror(
-                "Error while reallocating memory "
-                "(trajectoryfile_new.new_conf_pos)");
+            perror("Error while reallocating memory (trajectoryfile_new.new_conf_pos)");
             return trajectory_file;
         }
 
         steps_size = N_configurations;
         conf_pos = new_conf_pos;
     }
 
     // Copying the data
     strncpy(trajectory_file.file_name, file_name, FILE_NAME_LIMIT);
+    trajectory_file.file_name[FILE_NAME_LIMIT - 1] = '\0';
     if (user_format != NULL)  // if a user format is provided
+    {
         strncpy(trajectory_file.user_format, user_format, BUFFER_LIMIT);
+        trajectory_file.user_format[BUFFER_LIMIT - 1] = '\0';
+    }
     else
         trajectory_file.user_format[0] = '\0';  // Disables the user format
     trajectory_file.batch_size = batch_size;
     trajectory_file.N_configurations = N_configurations;
     trajectory_file.steps = steps;
     trajectory_file.conf_pos = conf_pos;
+    trajectory_file.selections = NULL;
     return trajectory_file;
 }
 
 void trajectoryfile_delete(struct TrajectoryFile *trajectory_file)
 {
-    free(trajectory_file->parameters);
+    trajectoryfile_clear_selections(trajectory_file);
     free(trajectory_file->steps);
     free(trajectory_file->conf_pos);
 }
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/pybox.c` & `pylammpstrj-1.0.4a0/src/pybox.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 #define PY_SSIZE_T_CLEAN
 
 #include "pybox.h"
+#include "box.h"
 
+#include <Python.h>
 #include <stdbool.h>
 #include <stddef.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
-void PyBox_dealloc(PyBoxObject *self)
-{
-    Py_TYPE(self)->tp_free((PyObject *) self);
-}
+#include <descrobject.h>
+#include <floatobject.h>
+#include <listobject.h>
+#include <object.h>
+#include <pymacro.h>
+#include <unicodeobject.h>
+
+void PyBox_dealloc(PyBoxObject *self) { Py_TYPE(self)->tp_free((PyObject *) self); }
 
-PyObject *PyBox_new(PyTypeObject *type, PyObject *Py_UNUSED(args),
-                    PyObject *Py_UNUSED(kwargs))
+PyObject *PyBox_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwargs))
 {
     PyBoxObject *self;
     self = (PyBoxObject *) type->tp_alloc(type, 0);
     return (PyObject *) self;
 }
 
 PyObject *PyBox_get_bounds(PyBoxObject *self, PyObject *Py_UNUSED(closure))
 {
     PyObject *list = PyList_New(6);
-    for (unsigned int b = 0; b < 6; b++)
-        PyList_SetItem(list, b, PyFloat_FromDouble(self->box.bounds[b]));
+    for (unsigned int b = 0; b < 6; b++) PyList_SetItem(list, b, PyFloat_FromDouble(self->box.bounds[b]));
     return list;
 }
 
-PyObject *PyBox_get_flag(PyBoxObject *self, PyObject *Py_UNUSED(closure))
-{
-    return PyUnicode_FromString(self->box.flag);
-}
+PyObject *PyBox_get_flag(PyBoxObject *self, PyObject *Py_UNUSED(closure)) { return PyUnicode_FromString(self->box.flag); }
 
-PyGetSetDef PyBox_getset[] = {
-    {.name = "bounds",
-     .get = (getter) PyBox_get_bounds,
-     .doc = "The box bounds."},
-    {.name = "flags", .get = (getter) PyBox_get_flag, .doc = "The box flag."},
-    {NULL, NULL, NULL, NULL, NULL}};
+PyGetSetDef PyBox_getset[] = {{.name = "bounds", .get = (getter) PyBox_get_bounds, .doc = "The box bounds."},
+                              {.name = "flags", .get = (getter) PyBox_get_flag, .doc = "The box flag."},
+                              {NULL, NULL, NULL, NULL, NULL}};
 
 PyObject *PyBox_str(PyBoxObject *self)
 {
-    return PyUnicode_FromFormat("[%S '%s']",
-                                PyObject_Str(PyBox_get_bounds(self, NULL)),
-                                self->box.flag);
+    return PyUnicode_FromFormat("[%S '%s']", PyObject_Str(PyBox_get_bounds(self, NULL)), self->box.flag);
 }
 
 PyObject *PyBox_repr(PyBoxObject *self)
 {
-    return PyUnicode_FromFormat("box(bounds=%S flag='%s')",
-                                PyObject_Str(PyBox_get_bounds(self, NULL)),
-                                self->box.flag);
+    return PyUnicode_FromFormat("box(bounds=%S flag='%s')", PyObject_Str(PyBox_get_bounds(self, NULL)), self->box.flag);
 }
 
 void PyBox_initialize(PyBoxObject *self, struct Box box) { self->box = box; }
 
-PyTypeObject PyBoxType = {
-    PyVarObject_HEAD_INIT(NULL, 0).tp_name = "pylammpstrj.PyBox",
-    .tp_doc = "Box objects",
-    .tp_basicsize = sizeof(PyBoxObject),
-    .tp_itemsize = 0,
-    .tp_flags = Py_TPFLAGS_DEFAULT,
-    .tp_dealloc = (destructor) PyBox_dealloc,
-    .tp_new = PyBox_new,
-    .tp_getset = PyBox_getset,
-    .tp_str = (reprfunc) PyBox_str,
-    .tp_repr = (reprfunc) PyBox_repr};
+PyTypeObject PyBoxType = {PyVarObject_HEAD_INIT(NULL, 0).tp_name = "pylammpstrj.PyBox",
+                          .tp_doc = "Box objects",
+                          .tp_basicsize = sizeof(PyBoxObject),
+                          .tp_itemsize = 0,
+                          .tp_flags = Py_TPFLAGS_DEFAULT,
+                          .tp_dealloc = (destructor) PyBox_dealloc,
+                          .tp_new = PyBox_new,
+                          .tp_getset = PyBox_getset,
+                          .tp_str = (reprfunc) PyBox_str,
+                          .tp_repr = (reprfunc) PyBox_repr};
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj/pytrajectoryfile.c` & `pylammpstrj-1.0.4a0/src/pytrajectoryfile.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,114 +1,103 @@
-#include "atom.h"
+#define PY_SSIZE_T_CLEAN
+
 #include "pytrajectory.h"
-#include "pyutils.h"
+#include "select.h"
 #include "trajectory.h"
 
 #include <errno.h>
+#include <Python.h>
+#include <stdio.h>
+#include <stdlib.h>
+
+#include <descrobject.h>
 #include <floatobject.h>
 #include <listobject.h>
 #include <longobject.h>
 #include <methodobject.h>
 #include <modsupport.h>
 #include <object.h>
 #include <pyerrors.h>
-#include <Python.h>
-#include <stdio.h>
+#include <pymacro.h>
+#include <pyutils.h>
 #include <unicodeobject.h>
 
-PyObject *PyTrajectoryFile_new(PyTypeObject *type, PyObject *Py_UNUSED(args),
-                               PyObject *Py_UNUSED(kwargs))
+PyObject *PyTrajectoryFile_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwargs))
 {
     PyTrajectoryFileObject *self;
     self = (PyTrajectoryFileObject *) type->tp_alloc(type, 0);
     return (PyObject *) self;
 }
 
-void PyTrajectoryFile_initialize(PyTrajectoryFileObject *self,
-                                 const struct TrajectoryFile trajectory_file)
+void PyTrajectoryFile_initialize(PyTrajectoryFileObject *self, const struct TrajectoryFile trajectory_file)
 {
     self->trajectory_file = trajectory_file;
 }
 
 void PyTrajectoryFile_dealloc(PyTrajectoryFileObject *self)
 {
     trajectoryfile_delete(&(self->trajectory_file));
     PyTrajectoryFileType.tp_free((PyObject *) self);
 }
 
 PyObject *PyTrajectoryFile_str(PyTrajectoryFileObject *self)
 {
-    return PyUnicode_FromFormat("%S %s %S",
-            PyObject_Str(PyTrajectoryFile_get_N_configurations(self, NULL)),
-            PyTrajectoryFile_get_file_name(self, NULL),
-            PyObject_Str(PyTrajectoryFile_get_batch_size(self, NULL)));
+    return PyUnicode_FromFormat("%S %s %S", PyObject_Str(PyTrajectoryFile_get_N_configurations(self, NULL)),
+                                PyTrajectoryFile_get_file_name(self, NULL), PyObject_Str(PyTrajectoryFile_get_batch_size(self, NULL)));
 }
 
 PyObject *PyTrajectoryFile_repr(PyTrajectoryFileObject *self)
 {
     return PyUnicode_FromFormat("trajectoryfile(N_configuration=%S file_name=%s batch_size=%S)",
-            PyObject_Str(PyTrajectoryFile_get_N_configurations(self, NULL)),
-            PyTrajectoryFile_get_file_name(self, NULL),
-            PyObject_Str(PyTrajectoryFile_get_batch_size(self, NULL)));
+                                PyObject_Str(PyTrajectoryFile_get_N_configurations(self, NULL)), PyTrajectoryFile_get_file_name(self, NULL),
+                                PyObject_Str(PyTrajectoryFile_get_batch_size(self, NULL)));
 }
 
-PyObject *PyTrajectoryFile_get_N_configurations(PyTrajectoryFileObject *self,
-                                                PyObject *Py_UNUSED(closure))
+PyObject *PyTrajectoryFile_get_N_configurations(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure))
 {
     return PyLong_FromLong(self->trajectory_file.N_configurations);
 }
 
-PyObject *PyTrajectoryFile_get_steps(PyTrajectoryFileObject *self,
-                                     PyObject *Py_UNUSED(closure))
+PyObject *PyTrajectoryFile_get_steps(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure))
 {
     PyObject *list = PyList_New(self->trajectory_file.N_configurations);
     if (list == NULL) return NULL;
 
     for (unsigned int c = 0; c < self->trajectory_file.N_configurations; c++)
-        PyList_SetItem(list, c,
-                       PyLong_FromLong(self->trajectory_file.steps[c]));
+        PyList_SetItem(list, c, PyLong_FromLong(self->trajectory_file.steps[c]));
 
     return list;
 }
 
-PyObject *PyTrajectoryFile_get_file_name(PyTrajectoryFileObject *self,
-                                         PyObject *Py_UNUSED(closure))
+PyObject *PyTrajectoryFile_get_file_name(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure))
 {
     return PyUnicode_FromString(self->trajectory_file.file_name);
 }
 
-PyObject *PyTrajectoryFile_get_batch_size(PyTrajectoryFileObject *self,
-                                          PyObject *Py_UNUSED(closure))
+PyObject *PyTrajectoryFile_get_batch_size(PyTrajectoryFileObject *self, PyObject *Py_UNUSED(closure))
 {
     return PyLong_FromLong(self->trajectory_file.batch_size);
 }
 
 PyGetSetDef PyTrajectoryFile_getset[] = {
-    {.name = "N_configurations",
-     .get = (getter) PyTrajectoryFile_get_N_configurations,
-     .doc = "The number of configurations."},
-    {.name = "steps",
-     .get = (getter) PyTrajectoryFile_get_steps,
-     .doc = "The timesteps."},
-    {.name = "file_name",
-     .get = (getter) PyTrajectoryFile_get_file_name,
-     .doc = "The name of the trajectory file."},
-    {.name = "batch_size",
-     .get = (getter) PyTrajectoryFile_get_batch_size,
-     .doc = "The size of the batches."},
+    {.name = "N_configurations", .get = (getter) PyTrajectoryFile_get_N_configurations, .doc = "The number of configurations."},
+    {.name = "steps", .get = (getter) PyTrajectoryFile_get_steps, .doc = "The timesteps."},
+    {.name = "file_name", .get = (getter) PyTrajectoryFile_get_file_name, .doc = "The name of the trajectory file."},
+    {.name = "batch_size", .get = (getter) PyTrajectoryFile_get_batch_size, .doc = "The size of the batches."},
     {0}};
 
-PyObject *PyTrajectoryFile_select_atoms(PyTrajectoryFileObject *self, PyObject *args)
+PyObject *PyTrajectoryFile_select(PyTrajectoryFileObject *self, PyObject *args)
 {
-    unsigned int field;
-    enum Operator op;
-    union AtomField value;
-    char *field_name;
-    long input_op;
-    PyObject *input_value;
+    unsigned int field = 0;
+    enum Operator op = 0;
+    union SelectionValue value = {0};
+    char *field_name = NULL;
+    long input_op = 0;
+    PyObject *input_value = NULL;
+    enum SelectionType type = 0;
 
     if (!PyArg_ParseTuple(args, "siO", &field_name, &input_op, &input_value))  // Could not parse the arguments
     {
         PyErr_SetString(PyExc_RuntimeError, "Could not parse the arguments");
         return NULL;
     }
 
@@ -117,109 +106,99 @@
     if (errno != 0)  // Could not read trajectory file
     {
         perror("Error while reading the trajectory file");
         PyErr_SetFromErrno(PyExc_RuntimeError);
         return NULL;
     }
 
-    field = parse_field_name(tmp.atom_builder, field_name);
+    field = parse_field_name(tmp.atom_builder, field_name, &type);
     if (PyErr_Occurred()) return NULL;
 
     op = parse_operator(input_op);
     if (PyErr_Occurred()) return NULL;
 
-    value = parse_value(tmp.atom_builder, field, input_value);
+    value = parse_selection_value(type, tmp.atom_builder, field, input_value);
     if (PyErr_Occurred()) return NULL;
 
     trajectory_delete(&tmp);
 
-    trajectoryfile_select_atoms(&(self->trajectory_file), field, op, value);
+    trajectoryfile_select_atoms(&(self->trajectory_file), (struct Selection){.type = type, .field = field, .op = op, .value = value});
     if (errno != 0)  // Could not select atoms
     {
         perror("Error while selecting the atoms");
         PyErr_SetFromErrno(PyExc_RuntimeError);
         return NULL;
     }
 
-    return Py_None;
+    Py_RETURN_NONE;
 }
 
-PyObject *PyTrajectoryFile_compute_average(PyTrajectoryFileObject *self,
-                                           PyObject *args)
+PyObject *PyTrajectoryFile_compute_average(PyTrajectoryFileObject *self, PyObject *args)
 {
     char *field_name;
     if (!PyArg_ParseTuple(args, "s", &field_name)) return NULL;
 
     struct Trajectory tmp;
     trajectoryfile_read_slice(self->trajectory_file, 0, 1, &tmp);
     if (errno != 0)  // Could not read the trajectory file
     {
         perror("Error while reading the trajectory file");
         PyErr_SetFromErrno(PyExc_RuntimeError);
         return NULL;
     }
 
     // Converting the field name
-    unsigned int field = parse_field_name(tmp.atom_builder, field_name);
+    enum SelectionType type = 0;
+    unsigned int field = parse_field_name(tmp.atom_builder, field_name, &type);
     trajectory_delete(&tmp);
 
     if (PyErr_Occurred()) return NULL;
 
-    double *averages =
-        trajectoryfile_average_property(self->trajectory_file, field);
+    double *averages = trajectoryfile_average_property(self->trajectory_file, field);
     PyObject *list = PyList_New(self->trajectory_file.N_configurations);
     if (list == NULL)
     {
         free(averages);
         return NULL;
     }
 
-    for (unsigned int c = 0; c < self->trajectory_file.N_configurations; c++)
-        PyList_SetItem(list, c, PyFloat_FromDouble(averages[c]));
+    for (unsigned int c = 0; c < self->trajectory_file.N_configurations; c++) PyList_SetItem(list, c, PyFloat_FromDouble(averages[c]));
 
     free(averages);
     return list;
 }
 
 PyObject *PyTrajectoryFile_load(PyTrajectoryFileObject *self)
 {
-    PyTrajectoryObject *pytrajectory =
-        (PyTrajectoryObject *) PyTrajectory_new(&PyTrajectoryType, NULL, NULL);
+    PyTrajectoryObject *pytrajectory = (PyTrajectoryObject *) PyTrajectory_new(&PyTrajectoryType, NULL, NULL);
 
     struct Trajectory trajectory;
-    trajectoryfile_read_slice(self->trajectory_file, 0,
-                              self->trajectory_file.N_configurations,
-                              &trajectory);
+    trajectoryfile_read_slice(self->trajectory_file, 0, self->trajectory_file.N_configurations, &trajectory);
     if (errno != 0)  // Could not read trajectory file
     {
         perror("Error while reading the trajectory file");
         PyErr_SetFromErrno(PyExc_RuntimeError);
         return NULL;
     }
 
     PyTrajectory_initialize(pytrajectory, trajectory);
     return (PyObject *) pytrajectory;
 }
 
 PyMethodDef PyTrajectoryFile_methods[] = {
-    {"select_atoms", (PyCFunction) PyTrajectoryFile_select_atoms, METH_VARARGS,
-     "Store selection parameters."},
-    {"compute_average", (PyCFunction) PyTrajectoryFile_compute_average,
-     METH_VARARGS, "Computes average of property over the atoms."},
-    {"load", (PyCFunction) PyTrajectoryFile_load, METH_NOARGS,
+    {"select", (PyCFunction) (void (*)(void)) PyTrajectoryFile_select, METH_VARARGS | METH_KEYWORDS, "Store selection parameters."},
+    {"compute_average", (PyCFunction) PyTrajectoryFile_compute_average, METH_VARARGS, "Computes average of property over the atoms."},
+    {"load", (PyCFunction) (void (*)(void)) PyTrajectoryFile_load, METH_NOARGS,
      "Loads a pylammpstrj.PyTrajectory from a pylammpstrj.PyTrajectoryFile."},
     {0}};
 
-PyTypeObject PyTrajectoryFileType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name = "pylammpstrj.PyTrajectoryFile",
-    .tp_doc = "Trajectory file object",
-    .tp_basicsize = sizeof(PyTrajectoryFileObject),
-    .tp_itemsize = 0,
-    .tp_flags = Py_TPFLAGS_DEFAULT,
-    .tp_dealloc = (destructor) PyTrajectoryFile_dealloc,
-    .tp_new = PyTrajectoryFile_new,
-    .tp_getset = PyTrajectoryFile_getset,
-    .tp_methods = PyTrajectoryFile_methods,
-    .tp_str = (reprfunc) PyTrajectoryFile_str,
-    .tp_repr = (reprfunc) PyTrajectoryFile_repr
-};
+PyTypeObject PyTrajectoryFileType = {PyVarObject_HEAD_INIT(NULL, 0).tp_name = "pylammpstrj.PyTrajectoryFile",
+                                     .tp_doc = "Trajectory file object",
+                                     .tp_basicsize = sizeof(PyTrajectoryFileObject),
+                                     .tp_itemsize = 0,
+                                     .tp_flags = Py_TPFLAGS_DEFAULT,
+                                     .tp_dealloc = (destructor) PyTrajectoryFile_dealloc,
+                                     .tp_new = PyTrajectoryFile_new,
+                                     .tp_getset = PyTrajectoryFile_getset,
+                                     .tp_methods = PyTrajectoryFile_methods,
+                                     .tp_str = (reprfunc) PyTrajectoryFile_str,
+                                     .tp_repr = (reprfunc) PyTrajectoryFile_repr};
```

### Comparing `pylammpstrj-1.0.3rc0/pylammpstrj.egg-info/PKG-INFO` & `pylammpstrj-1.0.4a0/src/pylammpstrj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpstrj
-Version: 1.0.3rc0
+Version: 1.0.4a0
 Summary: Processing LAMMPS trajectory files.
 Author-email: Heiarii Lou Chao <heiariilouchao@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pylammpstrj-1.0.3rc0/pyproject.toml` & `pylammpstrj-1.0.4a0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: C",
     "Programming Language :: Python :: 3.8",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Utilities"
 ]
-version = "1.0.3c"
+version = "1.0.4a"
 
 [project.urls]
 Repository = "https://github.com/heiariilouchao/thesis"
```

