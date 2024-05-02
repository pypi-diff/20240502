# Comparing `tmp/openyieldtables-2.1.0.tar.gz` & `tmp/openyieldtables-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openyieldtables-2.1.0.tar", max compression
+gzip compressed data, was "openyieldtables-2.2.0.tar", max compression
```

## Comparing `openyieldtables-2.1.0.tar` & `openyieldtables-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1089 2024-04-24 07:46:27.741979 openyieldtables-2.1.0/LICENSE
--rw-r--r--   0        0        0     1509 2024-04-24 07:46:27.741979 openyieldtables-2.1.0/README.md
--rw-r--r--   0        0        0     1784 2024-04-24 07:46:28.653981 openyieldtables-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 07:46:27.745979 openyieldtables-2.1.0/src/openyieldtables/__init__.py
--rw-r--r--   0        0        0   462163 2024-04-24 07:46:27.745979 openyieldtables-2.1.0/src/openyieldtables/data/yield_tables.csv
--rw-r--r--   0        0        0     7351 2024-04-24 07:46:27.745979 openyieldtables-2.1.0/src/openyieldtables/data/yield_tables_meta.csv
--rw-r--r--   0        0        0      119 2024-04-24 07:46:27.749979 openyieldtables-2.1.0/src/openyieldtables/models/__init__.py
--rw-r--r--   0        0        0     1118 2024-04-24 07:46:27.749979 openyieldtables-2.1.0/src/openyieldtables/models/yieldtable.py
--rw-r--r--   0        0        0        0 2024-04-24 07:46:27.749979 openyieldtables-2.1.0/src/openyieldtables/py.typed
--rw-r--r--   0        0        0       55 2024-04-24 07:46:27.749979 openyieldtables-2.1.0/src/openyieldtables/utils/__init__.py
--rw-r--r--   0        0        0     1379 2024-04-24 07:46:27.749979 openyieldtables-2.1.0/src/openyieldtables/utils/utils.py
--rw-r--r--   0        0        0     6249 2024-04-24 07:46:27.749979 openyieldtables-2.1.0/src/openyieldtables/yieldtables.py
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 openyieldtables-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-02 13:29:40.293870 openyieldtables-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1509 2024-05-02 13:29:40.293870 openyieldtables-2.2.0/README.md
+-rw-r--r--   0        0        0     1784 2024-05-02 13:29:41.101869 openyieldtables-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 13:29:40.293870 openyieldtables-2.2.0/src/openyieldtables/__init__.py
+-rw-r--r--   0        0        0   462163 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/data/yield_tables.csv
+-rw-r--r--   0        0        0     9631 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/data/yield_tables_meta.csv
+-rw-r--r--   0        0        0      119 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/models/__init__.py
+-rw-r--r--   0        0        0     1118 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/models/yieldtable.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/py.typed
+-rw-r--r--   0        0        0       55 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/utils/__init__.py
+-rw-r--r--   0        0        0     1379 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/utils/utils.py
+-rw-r--r--   0        0        0     6249 2024-05-02 13:29:40.297870 openyieldtables-2.2.0/src/openyieldtables/yieldtables.py
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 openyieldtables-2.2.0/PKG-INFO
```

### Comparing `openyieldtables-2.1.0/LICENSE` & `openyieldtables-2.2.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 to Tree.ly FlexKapG and FMM GmbH
+Copyright (c) 2024 to Tree.ly GmbH and FMM GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `openyieldtables-2.1.0/README.md` & `openyieldtables-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.1.0/pyproject.toml` & `openyieldtables-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openyieldtables"
-version = "2.1.0"
+version = "2.2.0"
 description = ""
 authors = ["Tree.ly <hello@tree.ly>", "FMM <fmm@fmm.at>"]
 maintainers = ["FMM <fmm@fmm.at>", "Tree.ly <hello@tree.ly>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/treely/openyieldtables"
 documentation = "https://openyieldtables.readthedocs.io"
```

### Comparing `openyieldtables-2.1.0/src/openyieldtables/data/yield_tables.csv` & `openyieldtables-2.2.0/src/openyieldtables/data/yield_tables.csv`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.1.0/src/openyieldtables/data/yield_tables_meta.csv` & `openyieldtables-2.2.0/src/openyieldtables/data/yield_tables_meta.csv`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 id;title;country_codes;type;source;link;yield_class_step;age_step
-1;Fichte Hochgebirge;AT,DE;dgz_100;Marschall;;1;10
-2;Fichte Bayern;AT,DE;dgz_100;Marschall;;1;10
-3;Fichte Bruck;AT,DE;dgz_100;Marschall;;1;10
-4;Fichte Weitra;AT,DE;dgz_100;Marschall;;1;10
-5;Tanne NWD;AT,DE;dgz_100;Marschall;;1;10
-6;Tanne Württemberg;AT,DE;dgz_100;Marschall;;2;10
-7;Douglasie BW;AT,DE;dgz_75;Marschall;;1;5
-8;Laerche Schweiz;AT,DE;dgz_100;Marschall;;1;10
-9;Kiefer Litschau;AT,DE;dgz_100;Marschall;;1;10
-10;Buche Braunschweig;AT,DE;dgz_100;Marschall;;1;10
-11;Eiche Ungarn;AT,DE;dgz_100;Marschall;;1;10
+1;Fichte Hochgebirge;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+2;Fichte Bayern;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+3;Fichte Bruck;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+4;Fichte Weitra;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+5;Tanne NWD;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+6;Tanne Württemberg;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;2;10
+7;Douglasie BW;AT,DE;dgz_75;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;5
+8;Laerche Schweiz;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+9;Kiefer Litschau;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+10;Buche Braunschweig;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
+11;Eiche Ungarn;AT,DE;dgz_100;1975, Julius Marschall: Hilfstafeln für die Forsteinrichtung, Neunte Auflage, Österreichischer Agrarverlag;https://www.avbuch-shop.at/landwirtschaft/lehrbuecher/1347/hilfstafeln-fuer-die-forsteinrichtung;1;10
 12;Esche;AT,DE;dgz_100;TimberControl Database;;1;10
 13;Europaeische Pappel;AT,DE;dgz_50;TimberControl Database;;1;10
 14;Hybrid Pappel;AT,DE;dgz_50;TimberControl Database;;1;10
 15;Hainbuche;AT,DE;dgz_100;TimberControl Database;;1;10
 16;Robinie;AT,DE;dgz_50;TimberControl Database;;1;10
 17;Schwarzkiefer;AT,DE;dgz_100;TimberControl Database;;1;10
 18;Strobe H;AT,DE;dgz_80;TimberControl Database;;1;10
 19;Erle Schwappach;AT,DE;dgz_100;TimberControl Database;;1;10
-20;Zirbe;AT,DE;dgz_200;ET-digital.xls;;1;10
+20;Tirol Zirbe Murau;AT,DE;dgz_200;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 21;Birke;AT,DE;dgz_100;TimberControl Database;;1;10
 87;Fichte Oststeiermark Eckmüllner;AT,DE;dgz_100;TimberControl Database;;1;10
 88;Tirol Fichte Kalk Ertragsniveau nieder;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 89;Tirol Fichte Kalk Ertragsniveau mittel;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 90;Tirol Fichte Silikat Ertragsniveau mittel;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 91;Tirol Fichte Silikat Ertragsniveau hoch;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 92;Tirol Laerche Suedtirol;AT,DE;dgz_150;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 93;Tirol Kiefer Suedtirol;AT,DE;dgz_150;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 94;Tirol Buche;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 99;Tirol Kiefer Suedtirol;AT,DE,IT;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 100;Tirol Laerche Suedtirol;AT,DE,IT;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
 101;Tirol Tanne;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;1;10
-102;Tirol Zirbe;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;;10
+102;Tirol Zirbe Murau;AT,DE;dgz_100;Ertragstafeln für Tirol, Amt der Tiroler Landesregierung;https://www.tirol.gv.at/umwelt/wald/waldwirtschaft/ertragstafeln-in-tirol/;;10
 103;Cerny Buche;CZ;dgz_100;1996, Martin Černý, Jan Pařez: Růstové a taxační tabulky hlavních dřevin České republiky: (smrk, borovice, buk, dub). Jílové u Prahy: IFER.;https://katalog.mendelu.cz/records/5b86d7f6-2962-425e-b679-474a975de497;2;10
 104;Cerny Eiche;CZ;dgz_100;1996, Martin Černý, Jan Pařez: Růstové a taxační tabulky hlavních dřevin České republiky: (smrk, borovice, buk, dub). Jílové u Prahy: IFER.;https://katalog.mendelu.cz/records/5b86d7f6-2962-425e-b679-474a975de497;2;10
 105;Cerny Fichte;CZ;dgz_100;1996, Martin Černý, Jan Pařez: Růstové a taxační tabulky hlavních dřevin České republiky: (smrk, borovice, buk, dub). Jílové u Prahy: IFER.;https://katalog.mendelu.cz/records/5b86d7f6-2962-425e-b679-474a975de497;2;10
 106;Cerny Kiefer;CZ;dgz_100;1996, Martin Černý, Jan Pařez: Růstové a taxační tabulky hlavních dřevin České republiky: (smrk, borovice, buk, dub). Jílové u Prahy: IFER.;https://katalog.mendelu.cz/records/5b86d7f6-2962-425e-b679-474a975de497;2;10
 120;Lockow Birke Nordostdeutschland;DE;dgz_100;Forstliche Forschungsanstalt Eberswalde, Fachgebiet Waldwachstum Eberswalde 1996;https://plan-birke.de/app/uploads/2019/01/Sandbirke_1996_Lockow.pdf;1;10
 133;Wiedemann Birke Baden-Wuerttemberg;DE;dgz_80;Schober, R. (Hg.): Ertragstafeln wichtiger Baumarten bei verschiedener Durchforstung. 4. Aufl., Frankfurt am Main: J. D. Sauerländer`s Verlag, 1995.;https://www.eurobuch.com/buch/isbn/3793907309.html;1;10
 134;Wiedemann Buche Baden-Wuerttemberg;DE;dgz_100;Schober, R. (Hg.): Ertragstafeln wichtiger Baumarten bei verschiedener Durchforstung. 4. Aufl., Frankfurt am Main: J. D. Sauerländer`s Verlag, 1995.;https://www.eurobuch.com/buch/isbn/3793907309.html;1;10
```

### Comparing `openyieldtables-2.1.0/src/openyieldtables/models/yieldtable.py` & `openyieldtables-2.2.0/src/openyieldtables/models/yieldtable.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.1.0/src/openyieldtables/utils/utils.py` & `openyieldtables-2.2.0/src/openyieldtables/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.1.0/src/openyieldtables/yieldtables.py` & `openyieldtables-2.2.0/src/openyieldtables/yieldtables.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.1.0/PKG-INFO` & `openyieldtables-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openyieldtables
-Version: 2.1.0
+Version: 2.2.0
 Summary: 
 Home-page: https://github.com/treely/openyieldtables
 License: MIT
 Author: Tree.ly
 Author-email: hello@tree.ly
 Maintainer: FMM
 Maintainer-email: fmm@fmm.at
```

