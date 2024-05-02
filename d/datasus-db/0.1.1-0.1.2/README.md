# Comparing `tmp/datasus_db-0.1.1.tar.gz` & `tmp/datasus_db-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasus_db-0.1.1.tar", max compression
+gzip compressed data, was "datasus_db-0.1.2.tar", max compression
```

## Comparing `datasus_db-0.1.1.tar` & `datasus_db-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1233 2023-12-07 20:14:19.985646 datasus_db-0.1.1/datasus_db/__init__.py
--rw-r--r--   0        0        0     1200 2023-12-07 20:14:19.985646 datasus_db-0.1.1/datasus_db/cnv.py
--rw-r--r--   0        0        0       70 2023-12-07 20:14:19.986658 datasus_db-0.1.1/datasus_db/datasources/__init__.py
--rw-r--r--   0        0        0     4333 2023-12-07 20:14:19.987656 datasus_db-0.1.1/datasus_db/datasources/auxiliar.py
--rw-r--r--   0        0        0     2820 2023-12-07 20:14:19.987656 datasus_db-0.1.1/datasus_db/datasources/ibge_pop.py
--rw-r--r--   0        0        0     1880 2023-12-07 20:14:19.989169 datasus_db-0.1.1/datasus_db/datasources/ibge_pop_tcu.py
--rw-r--r--   0        0        0     2568 2023-12-07 20:14:19.989169 datasus_db-0.1.1/datasus_db/datasources/po.py
--rw-r--r--   0        0        0     7220 2023-12-07 20:14:19.990610 datasus_db-0.1.1/datasus_db/datasources/sih_rd.py
--rw-r--r--   0        0        0     7730 2023-12-07 20:14:19.990610 datasus_db-0.1.1/datasus_db/datasources/sim_do.py
--rw-r--r--   0        0        0     5527 2023-12-07 20:14:19.991958 datasus_db-0.1.1/datasus_db/datasus.py
--rw-r--r--   0        0        0     2275 2023-12-07 20:14:19.993246 datasus_db-0.1.1/datasus_db/db.py
--rw-r--r--   0        0        0      576 2023-12-07 20:14:19.993246 datasus_db-0.1.1/datasus_db/dbf.py
--rw-r--r--   0        0        0     1674 2023-12-07 20:14:19.993246 datasus_db-0.1.1/datasus_db/ftp.py
--rw-r--r--   0        0        0     2080 2023-12-07 20:14:19.994758 datasus_db-0.1.1/datasus_db/pl_utils.py
--rw-r--r--   0        0        0      567 2023-12-07 20:14:19.995783 datasus_db-0.1.1/datasus_db/utils.py
--rw-r--r--   0        0        0       46 2023-12-07 20:14:19.995783 datasus_db-0.1.1/datasus_db/views/__init__.py
--rw-r--r--   0        0        0      747 2023-12-07 17:22:06.691412 datasus_db-0.1.1/datasus_db/views/ibge_piramide_etaria.py
--rw-r--r--   0        0        0     1092 2023-12-07 17:22:06.679832 datasus_db-0.1.1/LICENSE
--rw-r--r--   0        0        0      816 2023-12-07 20:45:27.870426 datasus_db-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2357 2023-12-07 20:44:50.952173 datasus_db-0.1.1/README.md
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 datasus_db-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-30 20:36:47.905655 datasus_db-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2515 2024-05-02 18:46:15.708163 datasus_db-0.1.2/README.md
+-rw-r--r--   0        0        0     1393 2024-05-02 18:55:10.466363 datasus_db-0.1.2/datasus_db/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/cnv.py
+-rw-r--r--   0        0        0       67 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasources/__init__.py
+-rw-r--r--   0        0        0     4198 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasources/auxiliar.py
+-rw-r--r--   0        0        0     2726 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasources/ibge_pop.py
+-rw-r--r--   0        0        0     1819 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasources/ibge_pop_tcu.py
+-rw-r--r--   0        0        0     2490 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasources/po.py
+-rw-r--r--   0        0        0     4470 2024-05-02 18:47:05.209067 datasus_db-0.1.2/datasus_db/datasources/sia_pa.py
+-rw-r--r--   0        0        0     6958 2024-05-02 18:46:15.708163 datasus_db-0.1.2/datasus_db/datasources/sih_rd.py
+-rw-r--r--   0        0        0     3495 2024-05-02 18:46:15.708163 datasus_db-0.1.2/datasus_db/datasources/sih_sp.py
+-rw-r--r--   0        0        0     7529 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasources/sim_do.py
+-rw-r--r--   0        0        0     5374 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/datasus.py
+-rw-r--r--   0        0        0     2197 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/db.py
+-rw-r--r--   0        0        0      553 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/dbf.py
+-rw-r--r--   0        0        0     1607 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/ftp.py
+-rw-r--r--   0        0        0     2007 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/pl_utils.py
+-rw-r--r--   0        0        0      538 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/utils.py
+-rw-r--r--   0        0        0       43 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/views/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-30 20:36:47.905655 datasus_db-0.1.2/datasus_db/views/ibge_piramide_etaria.py
+-rw-r--r--   0        0        0      859 2024-05-02 18:56:53.876412 datasus_db-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3499 1970-01-01 00:00:00.000000 datasus_db-0.1.2/PKG-INFO
```

### Comparing `datasus_db-0.1.1/datasus_db/datasources/ibge_pop.py` & `datasus_db-0.1.2/datasus_db/datasources/ibge_pop.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import polars as pl
-import os.path as path
-import logging
-from ..pl_utils import to_schema, Column
-from ..views.ibge_piramide_etaria import create_piramide_etaria_view
-from ..datasus import import_from_ftp
-from ..utils import format_year
-from ..ftp import fetch_from_zip
-
-MAIN_TABLE = "IBGE_POP"
-
-
-def import_ibge_pop(db_file="datasus.db", years=["*"]):
-    """Import IBGE population by age and sex per city.
-    https://google.com
-
-    Args:
-        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
-        years (list, optional): list of years for which data will be imported (if available). Eg: `[2012, 2000, 2010]. Defaults to ["*"].
-
-    ---
-
-    Extra:
-    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/ibge_pop.pdf
-    - **ftp path**: ftp.datasus.gov.br/dissemin/publicos/IBGE/POP/POPBR*.zip
-    """
-    logging.info(f"⏳ [{MAIN_TABLE}] Starting import...")
-
-    import_from_ftp(
-        [MAIN_TABLE],
-        [
-            f"/dissemin/publicos/IBGE/POP/POPBR{format_year(year)}.zip*"
-            for year in years
-        ],
-        fetch_ibge_pop,
-        db_file=db_file,
-    )
-
-    create_piramide_etaria_view()
-
-
-def fetch_ibge_pop(ftp_path: str):
-    csv_file = path.basename(ftp_path).split(".")[0] + ".csv"
-    files = fetch_from_zip(ftp_path, [csv_file])
-    df = pl.read_csv(
-        files[csv_file],
-        schema={
-            "MUNIC_RES": pl.UInt32,
-            "ANO": pl.UInt32,
-            "SEXO": pl.UInt32,
-            "SITUACAO": pl.UInt32,
-            "FXETARIA": pl.Utf8,
-            "POPULACAO": pl.UInt32,
-        },
-    )
-
-    return {MAIN_TABLE: map_ibge_pop(df)}
-
-
-def map_ibge_pop(df: pl.DataFrame):
-    df = (
-        df.with_columns(
-            pl.when(pl.col("FXETARIA").is_in(["I000", "R000"]))
-            .then("-100")
-            .otherwise(pl.col("FXETARIA"))
-            .name.keep(),
-        )
-        .with_columns(
-            pl.col("FXETARIA").cast(pl.Int64),
-        )
-        .with_columns(
-            pl.when(pl.col("FXETARIA") == 0)
-            .then(0)
-            .otherwise(pl.col("FXETARIA") // 100)
-            .alias("INICIO_FXETARIA"),
-            pl.when(pl.col("FXETARIA") == 0)
-            .then(0)
-            .otherwise(pl.col("FXETARIA") % 100)
-            .alias("FIM_FXETARIA"),
-        )
-    )
-
-    return to_schema(
-        df,
-        [
-            Column("MUNIC_RES", pl.UInt32),
-            Column("ANO", pl.UInt16),
-            Column("SEXO", pl.UInt8),
-            Column("SITUACAO", pl.UInt8),
-            Column("INICIO_FXETARIA", pl.Int8),
-            Column("FIM_FXETARIA", pl.Int8),
-            Column("POPULACAO", pl.UInt32),
-        ],
-    )
+import polars as pl
+import os.path as path
+import logging
+from ..pl_utils import to_schema, Column
+from ..views.ibge_piramide_etaria import create_piramide_etaria_view
+from ..datasus import import_from_ftp
+from ..utils import format_year
+from ..ftp import fetch_from_zip
+
+MAIN_TABLE = "IBGE_POP"
+
+
+def import_ibge_pop(db_file="datasus.db", years=["*"]):
+    """Import IBGE population by age and sex per city.
+    https://google.com
+
+    Args:
+        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
+        years (list, optional): list of years for which data will be imported (if available). Eg: `[2012, 2000, 2010]. Defaults to ["*"].
+
+    ---
+
+    Extra:
+    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/ibge_pop.pdf
+    - **ftp path**: ftp.datasus.gov.br/dissemin/publicos/IBGE/POP/POPBR*.zip
+    """
+    logging.info(f"⏳ [{MAIN_TABLE}] Starting import...")
+
+    import_from_ftp(
+        [MAIN_TABLE],
+        [
+            f"/dissemin/publicos/IBGE/POP/POPBR{format_year(year)}.zip*"
+            for year in years
+        ],
+        fetch_ibge_pop,
+        db_file=db_file,
+    )
+
+    create_piramide_etaria_view()
+
+
+def fetch_ibge_pop(ftp_path: str):
+    csv_file = path.basename(ftp_path).split(".")[0] + ".csv"
+    files = fetch_from_zip(ftp_path, [csv_file])
+    df = pl.read_csv(
+        files[csv_file],
+        schema={
+            "MUNIC_RES": pl.UInt32,
+            "ANO": pl.UInt32,
+            "SEXO": pl.UInt32,
+            "SITUACAO": pl.UInt32,
+            "FXETARIA": pl.Utf8,
+            "POPULACAO": pl.UInt32,
+        },
+    )
+
+    return {MAIN_TABLE: map_ibge_pop(df)}
+
+
+def map_ibge_pop(df: pl.DataFrame):
+    df = (
+        df.with_columns(
+            pl.when(pl.col("FXETARIA").is_in(["I000", "R000"]))
+            .then("-100")
+            .otherwise(pl.col("FXETARIA"))
+            .name.keep(),
+        )
+        .with_columns(
+            pl.col("FXETARIA").cast(pl.Int64),
+        )
+        .with_columns(
+            pl.when(pl.col("FXETARIA") == 0)
+            .then(0)
+            .otherwise(pl.col("FXETARIA") // 100)
+            .alias("INICIO_FXETARIA"),
+            pl.when(pl.col("FXETARIA") == 0)
+            .then(0)
+            .otherwise(pl.col("FXETARIA") % 100)
+            .alias("FIM_FXETARIA"),
+        )
+    )
+
+    return to_schema(
+        df,
+        [
+            Column("MUNIC_RES", pl.UInt32),
+            Column("ANO", pl.UInt16),
+            Column("SEXO", pl.UInt8),
+            Column("SITUACAO", pl.UInt8),
+            Column("INICIO_FXETARIA", pl.Int8),
+            Column("FIM_FXETARIA", pl.Int8),
+            Column("POPULACAO", pl.UInt32),
+        ],
+    )
```

### Comparing `datasus_db-0.1.1/datasus_db/datasources/po.py` & `datasus_db-0.1.2/datasus_db/datasources/po.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import polars as pl
-import logging
-from ..pl_utils import to_schema, Column, DateColumn
-from ..datasus import import_from_ftp
-from ..utils import format_year
-from ..ftp import fetch_dbc_as_df
-
-MAIN_TABLE = "PO"
-
-
-def import_po(db_file="datasus.db", years=["*"]):
-    """Import PO (Painel de Oncologia) data (since 2013).
-
-    Args:
-        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
-        years (list, optional): list of years for which data will be imported (if available). Eg: `[2013, 2020]` Defaults to ["*"].
-
-    ---
-
-    Extra:
-    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/po.pdf
-    - **ftp path**: ftp.datasus.gov.br/dissemin/publicos/IBGE/POP/POPBR*.zip
-    """
-    logging.info(f"⏳ [{MAIN_TABLE}] Starting import...")
-
-    import_from_ftp(
-        [MAIN_TABLE],
-        [
-            f"/dissemin/publicos/PAINEL_ONCOLOGIA/DADOS/POBR{format_year(year, digits=4)}.dbc*"
-            for year in years
-        ],
-        fetch_po,
-        db_file=db_file,
-    )
-
-
-def fetch_po(ftp_path: str):
-    df = fetch_dbc_as_df(ftp_path)
-    return {MAIN_TABLE: map_po(df)}
-
-
-def map_po(df: pl.DataFrame):
-    df = df.with_columns(
-        [
-            pl.when(pl.col(pl.Utf8).str.len_chars() == 0)
-            .then(None)
-            .otherwise(pl.col(pl.Utf8))
-            .name.keep(),
-        ]
-    )
-    return to_schema(
-        df,
-        [
-            Column("ANO_DIAGN", pl.UInt16),
-            Column("ANOMES_DIA", pl.UInt32),
-            Column("ANO_TRATAM", pl.UInt16),
-            Column("ANOMES_TRA", pl.UInt32),
-            Column("UF_RESID", pl.UInt8),
-            Column("MUN_RESID", pl.UInt32),
-            Column("UF_TRATAM", pl.UInt8),
-            Column("MUN_TRATAM", pl.UInt32),
-            Column("UF_DIAGN", pl.UInt8),
-            Column("MUN_DIAG", pl.UInt32),
-            Column("TRATAMENTO", pl.UInt8),
-            Column("DIAGNOSTIC", pl.UInt8),
-            Column("IDADE", pl.UInt8, strict=False),
-            Column("SEXO", pl.Utf8),
-            Column("ESTADIAM", pl.UInt8),
-            Column("CNES_DIAG", pl.UInt32),
-            Column("CNES_TRAT", pl.UInt32),
-            Column("TEMPO_TRAT", pl.Utf8),
-            Column("CNS_PAC", pl.Utf8),
-            Column("DIAG_DETH", pl.Utf8),
-            DateColumn("DT_DIAG", "%d/%m/%Y"),
-            DateColumn("DT_TRAT", "%d/%m/%Y"),
-            DateColumn("DT_NASC", "%d/%m/%Y"),
-        ],
-    )
+import polars as pl
+import logging
+from ..pl_utils import to_schema, Column, DateColumn
+from ..datasus import import_from_ftp
+from ..utils import format_year
+from ..ftp import fetch_dbc_as_df
+
+MAIN_TABLE = "PO"
+
+
+def import_po(db_file="datasus.db", years=["*"]):
+    """Import PO (Painel de Oncologia) data (since 2013).
+
+    Args:
+        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
+        years (list, optional): list of years for which data will be imported (if available). Eg: `[2013, 2020]` Defaults to ["*"].
+
+    ---
+
+    Extra:
+    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/po.pdf
+    - **ftp path**: ftp.datasus.gov.br/dissemin/publicos/IBGE/POP/POPBR*.zip
+    """
+    logging.info(f"⏳ [{MAIN_TABLE}] Starting import...")
+
+    import_from_ftp(
+        [MAIN_TABLE],
+        [
+            f"/dissemin/publicos/PAINEL_ONCOLOGIA/DADOS/POBR{format_year(year, digits=4)}.dbc*"
+            for year in years
+        ],
+        fetch_po,
+        db_file=db_file,
+    )
+
+
+def fetch_po(ftp_path: str):
+    df = fetch_dbc_as_df(ftp_path)
+    return {MAIN_TABLE: map_po(df)}
+
+
+def map_po(df: pl.DataFrame):
+    df = df.with_columns(
+        [
+            pl.when(pl.col(pl.Utf8).str.len_chars() == 0)
+            .then(None)
+            .otherwise(pl.col(pl.Utf8))
+            .name.keep(),
+        ]
+    )
+    return to_schema(
+        df,
+        [
+            Column("ANO_DIAGN", pl.UInt16),
+            Column("ANOMES_DIA", pl.UInt32),
+            Column("ANO_TRATAM", pl.UInt16),
+            Column("ANOMES_TRA", pl.UInt32),
+            Column("UF_RESID", pl.UInt8),
+            Column("MUN_RESID", pl.UInt32),
+            Column("UF_TRATAM", pl.UInt8),
+            Column("MUN_TRATAM", pl.UInt32),
+            Column("UF_DIAGN", pl.UInt8),
+            Column("MUN_DIAG", pl.UInt32),
+            Column("TRATAMENTO", pl.UInt8),
+            Column("DIAGNOSTIC", pl.UInt8),
+            Column("IDADE", pl.UInt8, strict=False),
+            Column("SEXO", pl.Utf8),
+            Column("ESTADIAM", pl.UInt8),
+            Column("CNES_DIAG", pl.UInt32),
+            Column("CNES_TRAT", pl.UInt32),
+            Column("TEMPO_TRAT", pl.Utf8),
+            Column("CNS_PAC", pl.Utf8),
+            Column("DIAG_DETH", pl.Utf8),
+            DateColumn("DT_DIAG", "%d/%m/%Y"),
+            DateColumn("DT_TRAT", "%d/%m/%Y"),
+            DateColumn("DT_NASC", "%d/%m/%Y"),
+        ],
+    )
```

### Comparing `datasus_db-0.1.1/datasus_db/datasources/sih_rd.py` & `datasus_db-0.1.2/datasus_db/datasources/sih_rd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-import polars as pl
-import logging
-from ..pl_utils import to_schema, Column, DateColumn
-from ..datasus import import_from_ftp
-from ..utils import format_year, format_month
-from ..ftp import fetch_dbc_as_df
-
-MAIN_TABLE = "SIH_RD"
-
-
-def import_sih_rd(db_file="datasus.db", years=["*"], states=["*"], months=["*"]):
-    """Import RD (Autorização de Internação Hospitalar Reduzida) from SIMSUS (Sistema de Informações Hospitalares do SUS).
-
-    Args:
-        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
-        years (list, optional): list of years for which data will be imported (if available). Eg: `[2012, 2000, 2010]`. Defaults to ["*"].
-        states (list, optional): list of brazilian 2 letters state for which data will be imported (if available). Eg: `["SP", "RJ"]`. Defaults to ["*"].
-        months (list, optional): list of months numbers (1-12) for which data will be imported (if available). Eg: `[1, 12, 6]`. Defaults to ["*"].
-
-    ---
-
-    Extra:
-    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/sih_rd.pdf
-    - **ftp path**: ftp.datasus.gov.br/dissemin/publicos/SIHSUS/200801_/Dados/RD*.dbc
-    """
-    logging.info(f"⏳ [{MAIN_TABLE}] Starting import...")
-
-    import_from_ftp(
-        [MAIN_TABLE],
-        [
-            f"/dissemin/publicos/SIHSUS/200801_/Dados/RD{state.upper()}{format_year(year)}{format_month(month)}.dbc*"
-            for year in years
-            for state in states
-            for month in months
-        ],
-        fetch_sih_rh,
-        db_file=db_file,
-    )
-
-
-def fetch_sih_rh(ftp_path: str):
-    df = fetch_dbc_as_df(ftp_path)
-    return {MAIN_TABLE: map_sih_rd(df)}
-
-
-def map_sih_rd(df: pl.DataFrame):
-    df = df.with_columns(
-        pl.when(pl.col(pl.Utf8).str.len_chars() == 0)
-        .then(None)
-        .otherwise(pl.col(pl.Utf8))
-        .name.keep(),
-    ).with_columns(
-        pl.when(pl.col("GESTOR_CPF").str.contains("[1-9]"))
-        .then(pl.col("GESTOR_CPF"))
-        .otherwise(None)
-        .name.keep(),
-        pl.when(pl.col("INSC_PN").str.contains("[1-9]"))
-        .then(pl.col("INSC_PN"))
-        .otherwise(None)
-        .name.keep(),
-    )
-
-    return to_schema(
-        df,
-        [
-            Column("UF_ZI", pl.UInt32),
-            Column("ANO_CMPT", pl.UInt16),
-            Column("MES_CMPT", pl.UInt8),
-            Column("ESPEC", pl.UInt8),
-            Column("CGC_HOSP", pl.Utf8),
-            Column("N_AIH", pl.Utf8),
-            Column("IDENT", pl.UInt8),
-            Column("CEP", pl.Utf8),
-            Column("MUNIC_RES", pl.UInt32),
-            DateColumn("NASC", "%Y%m%d"),
-            Column("SEXO", pl.UInt8),
-            Column("UTI_MES_IN", pl.UInt8),
-            Column("UTI_MES_AN", pl.UInt8),
-            Column("UTI_MES_AL", pl.UInt8),
-            Column("UTI_MES_TO", pl.UInt16),
-            Column("UTI_INT_IN", pl.UInt8),
-            Column("UTI_INT_AN", pl.UInt8),
-            Column("UTI_INT_AL", pl.UInt8),
-            Column("UTI_INT_TO", pl.UInt8),
-            Column("DIAR_ACOM", pl.UInt16),
-            Column("QT_DIARIAS", pl.UInt32),
-            Column("PROC_SOLIC", pl.Utf8),
-            Column("PROC_REA", pl.Utf8),
-            Column("VAL_SH", pl.Float64),
-            Column("VAL_SP", pl.Float64),
-            Column("VAL_SADT", pl.Float64),
-            Column("VAL_RN", pl.Float64),
-            Column("VAL_ACOMP", pl.Float64),
-            Column("VAL_ORTP", pl.Float64),
-            Column("VAL_SANGUE", pl.Float64),
-            Column("VAL_SADTSR", pl.Float64),
-            Column("VAL_TRANSP", pl.Float64),
-            Column("VAL_OBSANG", pl.Float64),
-            Column("VAL_PED1AC", pl.Float64),
-            Column("VAL_TOT", pl.Float64),
-            Column("VAL_UTI", pl.Float64),
-            Column("US_TOT", pl.Float64),
-            DateColumn("DT_INTER", "%Y%m%d"),
-            DateColumn("DT_SAIDA", "%Y%m%d"),
-            Column("DIAG_PRINC", pl.Utf8),
-            Column("DIAG_SECUN", pl.Utf8),
-            Column("COBRANCA", pl.UInt8),
-            Column("NATUREZA", pl.UInt8),
-            Column("NAT_JUR", pl.UInt16),
-            Column("GESTAO", pl.UInt8),
-            Column("RUBRICA", pl.UInt8),
-            Column("IND_VDRL", pl.UInt8),
-            Column("MUNIC_MOV", pl.UInt32),
-            Column("COD_IDADE", pl.UInt8),
-            Column("IDADE", pl.UInt8, strict=False),
-            Column("DIAS_PERM", pl.UInt16),
-            Column("MORTE", pl.UInt8),
-            Column("NACIONAL", pl.UInt16),
-            Column("NUM_PROC", pl.Utf8),
-            Column("CAR_INT", pl.UInt8),
-            Column("TOT_PT_SP", pl.UInt32),
-            Column("CPF_AUT", pl.Utf8),
-            Column("HOMONIMO", pl.UInt8),
-            Column("NUM_FILHOS", pl.UInt8),
-            Column("INSTRU", pl.UInt8),
-            Column("CID_NOTIF", pl.Utf8),
-            Column("CONTRACEP1", pl.UInt8),
-            Column("CONTRACEP2", pl.UInt8),
-            Column("GESTRISCO", pl.UInt8),
-            Column("INSC_PN", pl.Utf8),
-            Column("SEQ_AIH5", pl.Utf8),
-            Column("CBOR", pl.Utf8),
-            Column("CNAER", pl.UInt16),
-            Column("VINCPREV", pl.UInt8),
-            Column("GESTOR_COD", pl.UInt16),
-            Column("GESTOR_TP", pl.UInt8),
-            Column("GESTOR_CPF", pl.Utf8),
-            DateColumn("GESTOR_DT", "%Y%m%d"),
-            Column("CNES", pl.Utf8),
-            Column("CNPJ_MANT", pl.Utf8),
-            Column("INFEHOSP", pl.UInt8),
-            Column("CID_ASSO", pl.Utf8),
-            Column("CID_MORTE", pl.Utf8),
-            Column("COMPLEX", pl.UInt8),
-            Column("FINANC", pl.UInt8),
-            Column("FAEC_TP", pl.UInt32),
-            Column("REGCT", pl.UInt16),
-            Column("RACA_COR", pl.UInt8),
-            Column("ETNIA", pl.UInt16),
-            Column("SEQUENCIA", pl.UInt32),
-            Column("REMESSA", pl.Utf8),
-            Column("AUD_JUST", pl.Utf8),
-            Column("SIS_JUST", pl.Utf8),
-            Column("VAL_SH_FED", pl.Float64),
-            Column("VAL_SP_FED", pl.Float64),
-            Column("VAL_SH_GES", pl.Float64),
-            Column("VAL_SP_GES", pl.Float64),
-            Column("VAL_UCI", pl.Float64),
-            Column("MARCA_UCI", pl.UInt8),
-            Column("DIAGSEC1", pl.Utf8),
-            Column("DIAGSEC2", pl.Utf8),
-            Column("DIAGSEC3", pl.Utf8),
-            Column("DIAGSEC4", pl.Utf8),
-            Column("DIAGSEC5", pl.Utf8),
-            Column("DIAGSEC6", pl.Utf8),
-            Column("DIAGSEC7", pl.Utf8),
-            Column("DIAGSEC8", pl.Utf8),
-            Column("DIAGSEC9", pl.Utf8),
-            Column("TPDISEC1", pl.UInt8),
-            Column("TPDISEC2", pl.UInt8),
-            Column("TPDISEC3", pl.UInt8),
-            Column("TPDISEC4", pl.UInt8),
-            Column("TPDISEC5", pl.UInt8),
-            Column("TPDISEC6", pl.UInt8),
-            Column("TPDISEC7", pl.UInt8),
-            Column("TPDISEC8", pl.UInt8),
-            Column("TPDISEC9", pl.UInt8),
-        ],
-    )
+import polars as pl
+import logging
+from ..pl_utils import to_schema, Column, DateColumn
+from ..datasus import import_from_ftp
+from ..utils import format_year, format_month
+from ..ftp import fetch_dbc_as_df
+
+MAIN_TABLE = "SIH_RD"
+
+
+def import_sih_rd(db_file="datasus.db", years=["*"], states=["*"], months=["*"]):
+    """Import RD (Autorização de Internação Hospitalar Reduzida) from SIMSUS (Sistema de Informações Hospitalares do SUS).
+
+    Args:
+        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
+        years (list, optional): list of years for which data will be imported (if available). Eg: `[2012, 2000, 2010]`. Defaults to ["*"].
+        states (list, optional): list of brazilian 2 letters state for which data will be imported (if available). Eg: `["SP", "RJ"]`. Defaults to ["*"].
+        months (list, optional): list of months numbers (1-12) for which data will be imported (if available). Eg: `[1, 12, 6]`. Defaults to ["*"].
+
+    ---
+
+    Extra:
+    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/sih_rd.pdf
+    - **ftp path**: ftp.datasus.gov.br/dissemin/publicos/SIHSUS/200801_/Dados/RD*.dbc
+    """
+    logging.info(f"⏳ [{MAIN_TABLE}] Starting import...")
+
+    import_from_ftp(
+        [MAIN_TABLE],
+        [
+            f"/dissemin/publicos/SIHSUS/200801_/Dados/RD{state.upper()}{format_year(year)}{format_month(month)}.dbc*"
+            for year in years
+            for state in states
+            for month in months
+        ],
+        fetch_sih_rh,
+        db_file=db_file,
+    )
+
+
+def fetch_sih_rh(ftp_path: str):
+    df = fetch_dbc_as_df(ftp_path)
+    return {MAIN_TABLE: map_sih_rd(df)}
+
+
+def map_sih_rd(df: pl.DataFrame):
+    df = df.with_columns(
+        pl.when(pl.col(pl.Utf8).str.len_chars() == 0)
+        .then(None)
+        .otherwise(pl.col(pl.Utf8))
+        .name.keep(),
+    ).with_columns(
+        pl.when(pl.col("GESTOR_CPF").str.contains("[1-9]"))
+        .then(pl.col("GESTOR_CPF"))
+        .otherwise(None)
+        .name.keep(),
+        pl.when(pl.col("INSC_PN").str.contains("[1-9]"))
+        .then(pl.col("INSC_PN"))
+        .otherwise(None)
+        .name.keep(),
+    )
+
+    return to_schema(
+        df,
+        [
+            Column("UF_ZI", pl.Utf8),
+            Column("ANO_CMPT", pl.Utf8),
+            Column("MES_CMPT", pl.Utf8),
+            Column("ESPEC", pl.Utf8),
+            Column("CGC_HOSP", pl.Utf8),
+            Column("N_AIH", pl.Utf8),
+            Column("IDENT", pl.Utf8),
+            Column("CEP", pl.Utf8),
+            Column("MUNIC_RES", pl.Utf8),
+            Column("NASC", pl.Utf8),
+            Column("SEXO", pl.Utf8),
+            Column("UTI_MES_IN", pl.Utf8),
+            Column("UTI_MES_AN", pl.Utf8),
+            Column("UTI_MES_AL", pl.Utf8),
+            Column("UTI_MES_TO", pl.Utf8),
+            Column("UTI_INT_IN", pl.Utf8),
+            Column("UTI_INT_AN", pl.Utf8),
+            Column("UTI_INT_AL", pl.Utf8),
+            Column("UTI_INT_TO", pl.Utf8),
+            Column("DIAR_ACOM", pl.Utf8),
+            Column("QT_DIARIAS", pl.Utf8),
+            Column("PROC_SOLIC", pl.Utf8),
+            Column("PROC_REA", pl.Utf8),
+            Column("VAL_SH", pl.Float64),
+            Column("VAL_SP", pl.Float64),
+            Column("VAL_SADT", pl.Float64),
+            Column("VAL_RN", pl.Float64),
+            Column("VAL_ACOMP", pl.Float64),
+            Column("VAL_ORTP", pl.Float64),
+            Column("VAL_SANGUE", pl.Float64),
+            Column("VAL_SADTSR", pl.Float64),
+            Column("VAL_TRANSP", pl.Float64),
+            Column("VAL_OBSANG", pl.Float64),
+            Column("VAL_PED1AC", pl.Float64),
+            Column("VAL_TOT", pl.Float64),
+            Column("VAL_UTI", pl.Float64),
+            Column("US_TOT", pl.Float64),
+            Column("DT_INTER", pl.Utf8),
+            Column("DT_SAIDA", pl.Utf8),
+            Column("DIAG_PRINC", pl.Utf8),
+            Column("DIAG_SECUN", pl.Utf8),
+            Column("COBRANCA", pl.Utf8),
+            Column("NATUREZA", pl.Utf8),
+            Column("NAT_JUR", pl.Utf8),
+            Column("GESTAO", pl.Utf8),
+            Column("RUBRICA", pl.Utf8),
+            Column("IND_VDRL", pl.Utf8),
+            Column("MUNIC_MOV", pl.Utf8),
+            Column("COD_IDADE", pl.Utf8),
+            Column("IDADE", pl.Utf8, strict=False),
+            Column("DIAS_PERM", pl.Utf8),
+            Column("MORTE", pl.Utf8),
+            Column("NACIONAL", pl.Utf8),
+            Column("NUM_PROC", pl.Utf8),
+            Column("CAR_INT", pl.Utf8),
+            Column("TOT_PT_SP", pl.Utf8),
+            Column("CPF_AUT", pl.Utf8),
+            Column("HOMONIMO", pl.Utf8),
+            Column("NUM_FILHOS", pl.Utf8),
+            Column("INSTRU", pl.Utf8),
+            Column("CID_NOTIF", pl.Utf8),
+            Column("CONTRACEP1", pl.Utf8),
+            Column("CONTRACEP2", pl.Utf8),
+            Column("GESTRISCO", pl.Utf8),
+            Column("INSC_PN", pl.Utf8),
+            Column("SEQ_AIH5", pl.Utf8),
+            Column("CBOR", pl.Utf8),
+            Column("CNAER", pl.Utf8),
+            Column("VINCPREV", pl.Utf8),
+            Column("GESTOR_COD", pl.Utf8),
+            Column("GESTOR_TP", pl.Utf8),
+            Column("GESTOR_CPF", pl.Utf8),
+            Column("GESTOR_DT", pl.Utf8),
+            Column("CNES", pl.Utf8),
+            Column("CNPJ_MANT", pl.Utf8),
+            Column("INFEHOSP", pl.Utf8),
+            Column("CID_ASSO", pl.Utf8),
+            Column("CID_MORTE", pl.Utf8),
+            Column("COMPLEX", pl.UInt8),
+            Column("FINANC", pl.UInt8),
+            Column("FAEC_TP", pl.Utf8),
+            Column("REGCT", pl.Utf8),
+            Column("RACA_COR", pl.UInt8),
+            Column("ETNIA", pl.Utf8),
+            Column("SEQUENCIA", pl.Utf8),
+            Column("REMESSA", pl.Utf8),
+            Column("AUD_JUST", pl.Utf8),
+            Column("SIS_JUST", pl.Utf8),
+            Column("VAL_SH_FED", pl.Float64),
+            Column("VAL_SP_FED", pl.Float64),
+            Column("VAL_SH_GES", pl.Float64),
+            Column("VAL_SP_GES", pl.Float64),
+            Column("VAL_UCI", pl.Float64),
+            Column("MARCA_UCI", pl.UInt8),
+            Column("DIAGSEC1", pl.Utf8),
+            Column("DIAGSEC2", pl.Utf8),
+            Column("DIAGSEC3", pl.Utf8),
+            Column("DIAGSEC4", pl.Utf8),
+            Column("DIAGSEC5", pl.Utf8),
+            Column("DIAGSEC6", pl.Utf8),
+            Column("DIAGSEC7", pl.Utf8),
+            Column("DIAGSEC8", pl.Utf8),
+            Column("DIAGSEC9", pl.Utf8),
+            Column("TPDISEC1", pl.UInt8),
+            Column("TPDISEC2", pl.UInt8),
+            Column("TPDISEC3", pl.UInt8),
+            Column("TPDISEC4", pl.UInt8),
+            Column("TPDISEC5", pl.UInt8),
+            Column("TPDISEC6", pl.UInt8),
+            Column("TPDISEC7", pl.UInt8),
+            Column("TPDISEC8", pl.UInt8),
+            Column("TPDISEC9", pl.UInt8),
+        ],
+    )
```

### Comparing `datasus_db-0.1.1/datasus_db/datasources/sim_do.py` & `datasus_db-0.1.2/datasus_db/datasources/sim_do.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-import polars as pl
-import logging
-from ..pl_utils import (
-    upsert_column,
-    to_schema,
-    Column,
-    DateColumn,
-    rename_columns,
-    fill_empty,
-    fill_text,
-    fill_non_numeric,
-)
-from ..datasus import import_from_ftp
-from ..utils import format_year
-from ..ftp import fetch_dbc_as_df
-
-MAIN_TABLE = "SIM_DO"
-
-
-def import_sim_do(db_file="datasus.db", years=["*"], states=["*"]):
-    """Import DO (Declaração de Óbito) from SIM (Sistema de informações de Mortalidade).
-
-    Args:
-        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
-        years (list, optional): list of years for which data will be imported (if available). Eg: `[2012, 2000, 2010]`. Defaults to ["*"].
-        states (list, optional): list of brazilian 2 letters state for which data will be imported (if available). Eg: `["SP", "RJ"]`. Defaults to ["*"].
-
-    ---
-
-    Extra:
-    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/sim_do.pdf
-    - **ftp path non preliminary data**: ftp.datasus.gov.br/dissemin/publicos/SIM/CID10/DORES/DO*.dbc
-    - **ftp path preliminary data**: ftp.datasus.gov.br/dissemin/publicos/SIM/PRELIM/DORES/DO*.dbc
-    """
-    logging.info(f"⏳ [{MAIN_TABLE}] Starting import for non preliminary data...")
-    import_from_ftp(
-        [MAIN_TABLE],
-        [
-            f"/dissemin/publicos/SIM/CID10/DORES/DO{state.upper()}{format_year(year, digits=4)}.dbc*"
-            for year in years
-            for state in states
-        ],
-        fetch_sim_do,
-        ftp_exclude_regex=r".*/DOBR.*\.dbc",
-        db_file=db_file,
-    )
-
-    logging.info(f"⏳ [{MAIN_TABLE}] Starting import for preliminary data...")
-    import_from_ftp(
-        [MAIN_TABLE],
-        [
-            f"/dissemin/publicos/SIM/PRELIM/DORES/DO{state.upper()}{format_year(year, digits=4)}.dbc*"
-            for year in years
-            for state in states
-        ],
-        fetch_sim_do,
-        ftp_exclude_regex=r".*/DOBR.*\.dbc",
-        db_file=db_file,
-    )
-
-
-def fetch_sim_do(ftp_path: str):
-    df = fetch_dbc_as_df(ftp_path)
-    return {MAIN_TABLE: map_sim_do(df)}
-
-
-def map_sim_do(df: pl.DataFrame):
-    df = (
-        df.with_columns(fill_empty(None))
-        .with_columns(
-            fill_text("NULL", None),
-        )
-        .with_columns(
-            fill_text("00000000", None),
-        )
-        .with_columns(
-            fill_non_numeric(None, pl.col(["PESO", "NATURAL"])),
-        )
-    )
-    df = rename_columns(df, {"contador": "CONTADOR"})
-
-    df = (
-        df.with_columns(upsert_column(df, "DTCADASTRO", pl.Utf8))
-        .with_columns(
-            pl.when(pl.col("DTOBITO").str.len_chars() == 4)
-            .then("0101" + pl.col("DTOBITO"))
-            .otherwise(pl.col("DTOBITO"))
-            .name.keep(),
-            pl.when(pl.col("DTNASC").str.len_chars() == 4)
-            .then("0101" + pl.col("DTNASC"))
-            .otherwise(pl.col("DTNASC"))
-            .name.keep(),
-            pl.when(pl.col("DTCADASTRO").str.len_chars() == 7)
-            .then("0" + pl.col("DTCADASTRO"))
-            .otherwise(pl.col("DTCADASTRO"))
-            .name.keep(),
-        )
-        .with_columns(
-            pl.when(pl.col("DTOBITO").str.len_chars() == 6)
-            .then("01" + pl.col("DTOBITO"))
-            .otherwise(pl.col("DTOBITO"))
-            .name.keep(),
-            pl.when(pl.col("DTNASC").str.len_chars() == 6)
-            .then("01" + pl.col("DTNASC"))
-            .otherwise(pl.col("DTNASC"))
-            .name.keep(),
-        )
-    )
-
-    return to_schema(
-        df,
-        [
-            Column("ORIGEM", pl.UInt8),
-            Column("TIPOBITO", pl.UInt8),
-            DateColumn("DTOBITO", "%d%m%Y", strict=False),
-            Column("HORAOBITO", pl.Utf8),
-            Column("NATURAL", pl.UInt32),
-            Column("CODMUNNATU", pl.UInt32),
-            DateColumn("DTNASC", "%d%m%Y", strict=False),
-            Column("IDADE", pl.UInt16),
-            Column("SEXO", pl.UInt8),
-            Column("RACACOR", pl.UInt8),
-            Column("ESTCIV", pl.UInt8, strict=False),
-            Column("ESC", pl.UInt8, strict=False),
-            Column("ESC2010", pl.UInt8, strict=False),
-            Column("SERIESCFAL", pl.UInt8),
-            Column("OCUP", pl.Utf8),
-            Column("CODMUNRES", pl.UInt32),
-            Column("LOCOCOR", pl.UInt8),
-            Column("CODESTAB", pl.UInt32, strict=False),
-            Column("ESTABDESCR", pl.Utf8),
-            Column("CODMUNOCOR", pl.UInt32),
-            Column("IDADEMAE", pl.UInt16, strict=False),
-            Column("ESCMAE", pl.Int8, strict=False),
-            Column("ESCMAE2010", pl.Int8, strict=False),
-            Column("SERIESCMAE", pl.Int8),
-            Column("OCUPMAE", pl.Utf8),
-            Column("QTDFILVIVO", pl.UInt8, strict=False),
-            Column("QTDFILMORT", pl.UInt8, strict=False),
-            Column("GRAVIDEZ", pl.UInt8),
-            Column("SEMAGESTAC", pl.UInt8),
-            Column("GESTACAO", pl.UInt8, strict=False),
-            Column("PARTO", pl.UInt8),
-            Column("OBITOPARTO", pl.UInt8),
-            Column("PESO", pl.UInt32),
-            Column("TPMORTEOCO", pl.UInt8),
-            Column("OBITOGRAV", pl.UInt8),
-            Column("OBITOPUERP", pl.UInt8),
-            Column("ASSISTMED", pl.UInt8),
-            Column("EXAME", pl.UInt8),
-            Column("CIRURGIA", pl.UInt8),
-            Column("NECROPSIA", pl.UInt8),
-            Column("LINHAA", pl.Utf8),
-            Column("LINHAB", pl.Utf8),
-            Column("LINHAC", pl.Utf8),
-            Column("LINHAD", pl.Utf8),
-            Column("LINHAII", pl.Utf8),
-            Column("CAUSABAS", pl.Utf8),
-            Column("CB_PRE", pl.Utf8),
-            Column("COMUNSVOIM", pl.Utf8),
-            DateColumn("DTATESTADO", "%d%m%Y", strict=False),
-            Column("CIRCOBITO", pl.UInt8, strict=False),
-            Column("ACIDTRAB", pl.UInt8),
-            Column("FONTE", pl.Utf8),
-            Column("NUMEROLOTE", pl.Utf8),
-            Column("TPPOS", pl.Utf8),
-            DateColumn("DTINVESTIG", "%d%m%Y"),
-            Column("CAUSABAS_O", pl.Utf8),
-            DateColumn("DTCADASTRO", "%d%m%Y"),
-            Column("ATESTANTE", pl.UInt8),
-            Column("STCODIFICA", pl.Utf8),
-            Column("CODIFICADO", pl.Utf8),
-            Column("VERSAOSIST", pl.Utf8),
-            Column("VERSAOSCB", pl.Utf8),
-            Column("FONTEINV", pl.Utf8),
-            DateColumn("DTRECEBIM", "%d%m%Y"),
-            Column("ATESTADO", pl.Utf8),
-            DateColumn("DTRECORIGA", "%d%m%Y"),
-            Column("CAUSAMAT", pl.Utf8),
-            Column("ESCMAEAGR1", pl.UInt8),
-            Column("ESCFALAGR1", pl.UInt8),
-            Column("STDOEPIDEM", pl.UInt8),
-            Column("STDONOVA", pl.UInt8),
-            Column("DIFDATA", pl.UInt16),
-            Column("NUDIASOBCO", pl.UInt16),
-            Column("NUDIASOBIN", pl.UInt16),
-            DateColumn("DTCADINV", "%d%m%Y"),
-            Column("TPOBITOCOR", pl.UInt8),
-            DateColumn("DTCONINV", "%d%m%Y"),
-            Column("FONTES", pl.Utf8),
-            Column("TPRESGINFO", pl.UInt8),
-            Column("TPNIVELINV", pl.Utf8),
-            Column("NUDIASINF", pl.UInt16),
-            DateColumn("DTCADINF", "%d%m%Y"),
-            Column("MORTEPARTO", pl.UInt8),
-            DateColumn("DTCONCASO", "%d%m%Y"),
-            Column("FONTESINF", pl.Utf8),
-            Column("ALTCAUSA", pl.UInt8),
-            Column("CONTADOR", pl.UInt32),
-        ],
-    )
+import polars as pl
+import logging
+from ..pl_utils import (
+    upsert_column,
+    to_schema,
+    Column,
+    DateColumn,
+    rename_columns,
+    fill_empty,
+    fill_text,
+    fill_non_numeric,
+)
+from ..datasus import import_from_ftp
+from ..utils import format_year
+from ..ftp import fetch_dbc_as_df
+
+MAIN_TABLE = "SIM_DO"
+
+
+def import_sim_do(db_file="datasus.db", years=["*"], states=["*"]):
+    """Import DO (Declaração de Óbito) from SIM (Sistema de informações de Mortalidade).
+
+    Args:
+        db_file (str, optional): path to the duckdb file in which the data will be imported to. Defaults to "datasus.db".
+        years (list, optional): list of years for which data will be imported (if available). Eg: `[2012, 2000, 2010]`. Defaults to ["*"].
+        states (list, optional): list of brazilian 2 letters state for which data will be imported (if available). Eg: `["SP", "RJ"]`. Defaults to ["*"].
+
+    ---
+
+    Extra:
+    - **Data description**: https://github.com/mymatsubara/datasus-db/blob/main/docs/sim_do.pdf
+    - **ftp path non preliminary data**: ftp.datasus.gov.br/dissemin/publicos/SIM/CID10/DORES/DO*.dbc
+    - **ftp path preliminary data**: ftp.datasus.gov.br/dissemin/publicos/SIM/PRELIM/DORES/DO*.dbc
+    """
+    logging.info(f"⏳ [{MAIN_TABLE}] Starting import for non preliminary data...")
+    import_from_ftp(
+        [MAIN_TABLE],
+        [
+            f"/dissemin/publicos/SIM/CID10/DORES/DO{state.upper()}{format_year(year, digits=4)}.dbc*"
+            for year in years
+            for state in states
+        ],
+        fetch_sim_do,
+        ftp_exclude_regex=r".*/DOBR.*\.dbc",
+        db_file=db_file,
+    )
+
+    logging.info(f"⏳ [{MAIN_TABLE}] Starting import for preliminary data...")
+    import_from_ftp(
+        [MAIN_TABLE],
+        [
+            f"/dissemin/publicos/SIM/PRELIM/DORES/DO{state.upper()}{format_year(year, digits=4)}.dbc*"
+            for year in years
+            for state in states
+        ],
+        fetch_sim_do,
+        ftp_exclude_regex=r".*/DOBR.*\.dbc",
+        db_file=db_file,
+    )
+
+
+def fetch_sim_do(ftp_path: str):
+    df = fetch_dbc_as_df(ftp_path)
+    return {MAIN_TABLE: map_sim_do(df)}
+
+
+def map_sim_do(df: pl.DataFrame):
+    df = (
+        df.with_columns(fill_empty(None))
+        .with_columns(
+            fill_text("NULL", None),
+        )
+        .with_columns(
+            fill_text("00000000", None),
+        )
+        .with_columns(
+            fill_non_numeric(None, pl.col(["PESO", "NATURAL"])),
+        )
+    )
+    df = rename_columns(df, {"contador": "CONTADOR"})
+
+    df = (
+        df.with_columns(upsert_column(df, "DTCADASTRO", pl.Utf8))
+        .with_columns(
+            pl.when(pl.col("DTOBITO").str.len_chars() == 4)
+            .then("0101" + pl.col("DTOBITO"))
+            .otherwise(pl.col("DTOBITO"))
+            .name.keep(),
+            pl.when(pl.col("DTNASC").str.len_chars() == 4)
+            .then("0101" + pl.col("DTNASC"))
+            .otherwise(pl.col("DTNASC"))
+            .name.keep(),
+            pl.when(pl.col("DTCADASTRO").str.len_chars() == 7)
+            .then("0" + pl.col("DTCADASTRO"))
+            .otherwise(pl.col("DTCADASTRO"))
+            .name.keep(),
+        )
+        .with_columns(
+            pl.when(pl.col("DTOBITO").str.len_chars() == 6)
+            .then("01" + pl.col("DTOBITO"))
+            .otherwise(pl.col("DTOBITO"))
+            .name.keep(),
+            pl.when(pl.col("DTNASC").str.len_chars() == 6)
+            .then("01" + pl.col("DTNASC"))
+            .otherwise(pl.col("DTNASC"))
+            .name.keep(),
+        )
+    )
+
+    return to_schema(
+        df,
+        [
+            Column("ORIGEM", pl.UInt8),
+            Column("TIPOBITO", pl.UInt8),
+            DateColumn("DTOBITO", "%d%m%Y", strict=False),
+            Column("HORAOBITO", pl.Utf8),
+            Column("NATURAL", pl.UInt32),
+            Column("CODMUNNATU", pl.UInt32),
+            DateColumn("DTNASC", "%d%m%Y", strict=False),
+            Column("IDADE", pl.UInt16),
+            Column("SEXO", pl.UInt8),
+            Column("RACACOR", pl.UInt8),
+            Column("ESTCIV", pl.UInt8, strict=False),
+            Column("ESC", pl.UInt8, strict=False),
+            Column("ESC2010", pl.UInt8, strict=False),
+            Column("SERIESCFAL", pl.UInt8),
+            Column("OCUP", pl.Utf8),
+            Column("CODMUNRES", pl.UInt32),
+            Column("LOCOCOR", pl.UInt8),
+            Column("CODESTAB", pl.UInt32, strict=False),
+            Column("ESTABDESCR", pl.Utf8),
+            Column("CODMUNOCOR", pl.UInt32),
+            Column("IDADEMAE", pl.UInt16, strict=False),
+            Column("ESCMAE", pl.Int8, strict=False),
+            Column("ESCMAE2010", pl.Int8, strict=False),
+            Column("SERIESCMAE", pl.Int8),
+            Column("OCUPMAE", pl.Utf8),
+            Column("QTDFILVIVO", pl.UInt8, strict=False),
+            Column("QTDFILMORT", pl.UInt8, strict=False),
+            Column("GRAVIDEZ", pl.UInt8),
+            Column("SEMAGESTAC", pl.UInt8),
+            Column("GESTACAO", pl.UInt8, strict=False),
+            Column("PARTO", pl.UInt8),
+            Column("OBITOPARTO", pl.UInt8),
+            Column("PESO", pl.UInt32),
+            Column("TPMORTEOCO", pl.UInt8),
+            Column("OBITOGRAV", pl.UInt8),
+            Column("OBITOPUERP", pl.UInt8),
+            Column("ASSISTMED", pl.UInt8),
+            Column("EXAME", pl.UInt8),
+            Column("CIRURGIA", pl.UInt8),
+            Column("NECROPSIA", pl.UInt8),
+            Column("LINHAA", pl.Utf8),
+            Column("LINHAB", pl.Utf8),
+            Column("LINHAC", pl.Utf8),
+            Column("LINHAD", pl.Utf8),
+            Column("LINHAII", pl.Utf8),
+            Column("CAUSABAS", pl.Utf8),
+            Column("CB_PRE", pl.Utf8),
+            Column("COMUNSVOIM", pl.Utf8),
+            DateColumn("DTATESTADO", "%d%m%Y", strict=False),
+            Column("CIRCOBITO", pl.UInt8, strict=False),
+            Column("ACIDTRAB", pl.UInt8),
+            Column("FONTE", pl.Utf8),
+            Column("NUMEROLOTE", pl.Utf8),
+            Column("TPPOS", pl.Utf8),
+            DateColumn("DTINVESTIG", "%d%m%Y"),
+            Column("CAUSABAS_O", pl.Utf8),
+            DateColumn("DTCADASTRO", "%d%m%Y"),
+            Column("ATESTANTE", pl.UInt8),
+            Column("STCODIFICA", pl.Utf8),
+            Column("CODIFICADO", pl.Utf8),
+            Column("VERSAOSIST", pl.Utf8),
+            Column("VERSAOSCB", pl.Utf8),
+            Column("FONTEINV", pl.Utf8),
+            DateColumn("DTRECEBIM", "%d%m%Y"),
+            Column("ATESTADO", pl.Utf8),
+            DateColumn("DTRECORIGA", "%d%m%Y"),
+            Column("CAUSAMAT", pl.Utf8),
+            Column("ESCMAEAGR1", pl.UInt8),
+            Column("ESCFALAGR1", pl.UInt8),
+            Column("STDOEPIDEM", pl.UInt8),
+            Column("STDONOVA", pl.UInt8),
+            Column("DIFDATA", pl.UInt16),
+            Column("NUDIASOBCO", pl.UInt16),
+            Column("NUDIASOBIN", pl.UInt16),
+            DateColumn("DTCADINV", "%d%m%Y"),
+            Column("TPOBITOCOR", pl.UInt8),
+            DateColumn("DTCONINV", "%d%m%Y"),
+            Column("FONTES", pl.Utf8),
+            Column("TPRESGINFO", pl.UInt8),
+            Column("TPNIVELINV", pl.Utf8),
+            Column("NUDIASINF", pl.UInt16),
+            DateColumn("DTCADINF", "%d%m%Y"),
+            Column("MORTEPARTO", pl.UInt8),
+            DateColumn("DTCONCASO", "%d%m%Y"),
+            Column("FONTESINF", pl.Utf8),
+            Column("ALTCAUSA", pl.UInt8),
+            Column("CONTADOR", pl.UInt32),
+        ],
+    )
```

### Comparing `datasus_db-0.1.1/datasus_db/db.py` & `datasus_db-0.1.2/datasus_db/db.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""
-Module with common functions used to interact with DuckDB
-"""
-
-import duckdb
-import os.path as path
-import polars as pl
-
-IMPORT_TABLE = "__import"
-
-
-def create_import_table(db_con: duckdb.DuckDBPyConnection):
-    db_con.sql(
-        f"""
-CREATE TABLE IF NOT EXISTS {IMPORT_TABLE} (
-    file VARCHAR(255),
-    table_name VARCHAR(255),
-    created_at TIMESTAMP DEFAULT current_timestamp,
-    PRIMARY KEY (file, table_name)
-)"""
-    )
-
-
-def check_new_files(
-    files: list[str], target_tables: list[str], db_con: duckdb.DuckDBPyConnection
-):
-    tables = ",".join((f"'{table}'" for table in target_tables))
-
-    imported_files = db_con.query(
-        f"""
-SELECT file, count(*) as count 
-FROM {IMPORT_TABLE}  
-WHERE table_name IN ({tables})
-GROUP BY file
-HAVING count = {len(target_tables)}"""
-    ).pl()["file"]
-    imported_files = set(imported_files)
-
-    return [file for file in files if not path.basename(file) in imported_files]
-
-
-def is_file_imported(
-    file: str, target_table: str, db_con: duckdb.DuckDBPyConnection
-) -> bool:
-    return (
-        db_con.execute(
-            f"SELECT COUNT(*) as count FROM {IMPORT_TABLE} WHERE table_name = ? AND file = ?",
-            [target_table, path.basename(file)],
-        ).pl()["count"][0]
-        == 1
-    )
-
-
-def import_dataframe(
-    table_name: str, df: pl.DataFrame, db_con: duckdb.DuckDBPyConnection
-):
-    # Since this is function is running on a controlled environment we don't sanitize the table name
-    if has_table(table_name, db_con):
-        cols = ",".join((f'"{col}"' for col in df.columns))
-        db_con.sql(f"INSERT INTO {table_name} ({cols}) SELECT * FROM df")
-    else:
-        db_con.sql(f"CREATE TABLE {table_name} AS SELECT * FROM df")
-
-
-def mark_file_as_imported(
-    file: str, table_name: str, db_con: duckdb.DuckDBPyConnection
-):
-    db_con.execute(
-        f"INSERT INTO {IMPORT_TABLE} (file, table_name) VALUES (?, ?)",
-        [path.basename(file), table_name],
-    )
-
-
-def has_table(table_name: str, db_con: duckdb.DuckDBPyConnection) -> bool:
-    return db_con.execute(
-        "SELECT count(*) == 1 as has_table FROM duckdb_tables where table_name = ?",
-        [table_name],
-    ).pl()["has_table"][0]
+"""
+Module with common functions used to interact with DuckDB
+"""
+
+import duckdb
+import os.path as path
+import polars as pl
+
+IMPORT_TABLE = "__import"
+
+
+def create_import_table(db_con: duckdb.DuckDBPyConnection):
+    db_con.sql(
+        f"""
+CREATE TABLE IF NOT EXISTS {IMPORT_TABLE} (
+    file VARCHAR(255),
+    table_name VARCHAR(255),
+    created_at TIMESTAMP DEFAULT current_timestamp,
+    PRIMARY KEY (file, table_name)
+)"""
+    )
+
+
+def check_new_files(
+    files: list[str], target_tables: list[str], db_con: duckdb.DuckDBPyConnection
+):
+    tables = ",".join((f"'{table}'" for table in target_tables))
+
+    imported_files = db_con.query(
+        f"""
+SELECT file, count(*) as count 
+FROM {IMPORT_TABLE}  
+WHERE table_name IN ({tables})
+GROUP BY file
+HAVING count = {len(target_tables)}"""
+    ).pl()["file"]
+    imported_files = set(imported_files)
+
+    return [file for file in files if not path.basename(file) in imported_files]
+
+
+def is_file_imported(
+    file: str, target_table: str, db_con: duckdb.DuckDBPyConnection
+) -> bool:
+    return (
+        db_con.execute(
+            f"SELECT COUNT(*) as count FROM {IMPORT_TABLE} WHERE table_name = ? AND file = ?",
+            [target_table, path.basename(file)],
+        ).pl()["count"][0]
+        == 1
+    )
+
+
+def import_dataframe(
+    table_name: str, df: pl.DataFrame, db_con: duckdb.DuckDBPyConnection
+):
+    # Since this is function is running on a controlled environment we don't sanitize the table name
+    if has_table(table_name, db_con):
+        cols = ",".join((f'"{col}"' for col in df.columns))
+        db_con.sql(f"INSERT INTO {table_name} ({cols}) SELECT * FROM df")
+    else:
+        db_con.sql(f"CREATE TABLE {table_name} AS SELECT * FROM df")
+
+
+def mark_file_as_imported(
+    file: str, table_name: str, db_con: duckdb.DuckDBPyConnection
+):
+    db_con.execute(
+        f"INSERT INTO {IMPORT_TABLE} (file, table_name) VALUES (?, ?)",
+        [path.basename(file), table_name],
+    )
+
+
+def has_table(table_name: str, db_con: duckdb.DuckDBPyConnection) -> bool:
+    return db_con.execute(
+        "SELECT count(*) == 1 as has_table FROM duckdb_tables where table_name = ?",
+        [table_name],
+    ).pl()["has_table"][0]
```

### Comparing `datasus_db-0.1.1/datasus_db/dbf.py` & `datasus_db-0.1.2/datasus_db/dbf.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""
-Module with helper functions to handler with *.dbf files
-"""
-import os.path as path
-import polars as pl
-from dbfread import DBF
-from .utils import rm
-
-
-def read_as_df(filename: str, bytes: bytes, encoding: str = None):
-    tmp_file = path.join(".tmp", path.basename(filename).split(".")[0] + ".dbf")
-
-    with open(tmp_file, "wb") as f:
-        f.write(bytes)
-
-    try:
-        dbf = DBF(tmp_file, encoding=encoding)
-        df = pl.DataFrame(iter(dbf))
-        return df
-    except Exception as e:
-        raise e
-    finally:
-        rm(tmp_file)
+"""
+Module with helper functions to handler with *.dbf files
+"""
+import os.path as path
+import polars as pl
+from dbfread import DBF
+from .utils import rm
+
+
+def read_as_df(filename: str, bytes: bytes, encoding: str = None):
+    tmp_file = path.join(".tmp", path.basename(filename).split(".")[0] + ".dbf")
+
+    with open(tmp_file, "wb") as f:
+        f.write(bytes)
+
+    try:
+        dbf = DBF(tmp_file, encoding=encoding)
+        df = pl.DataFrame(iter(dbf))
+        return df
+    except Exception as e:
+        raise e
+    finally:
+        rm(tmp_file)
```

### Comparing `datasus_db-0.1.1/datasus_db/ftp.py` & `datasus_db-0.1.2/datasus_db/ftp.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""
-Module with helper functions to interact with DATASUS ftp server
-"""
-
-import urllib.request as request
-import ftplib
-import logging
-import io
-from typing import Iterable
-import os.path as path
-import os
-from zipfile import ZipFile
-from dbfread import DBF
-import polars as pl
-import datasus_dbc
-from .utils import rm, flatten
-
-
-def fetch_dbc_as_df(ftp_path: str) -> pl.DataFrame:
-    response = request.urlopen(ftp_path)
-    dbc_raw = response.read()
-
-    filename = path.basename(ftp_path).split(".")[0]
-    dbc_file = f".tmp/{filename}.dbc"
-    dbf_file = f".tmp/{filename}.dbf"
-
-    os.makedirs(path.dirname(dbc_file), exist_ok=True)
-    with open(
-        dbc_file,
-        "wb",
-    ) as f:
-        f.write(dbc_raw)
-
-    datasus_dbc.decompress(dbc_file, dbf_file)
-
-    df = pl.DataFrame(iter(DBF(dbf_file, encoding="iso-8859-1")))
-
-    rm(dbc_file)
-    rm(dbf_file)
-
-    return df
-
-
-def get_matching_files(host: str, patterns: Iterable[str]):
-    ftp = ftplib.FTP(host)
-    ftp.login()
-
-    return set(flatten((try_nlst(pattern, ftp) for pattern in patterns)))
-
-
-def try_nlst(pattern: str, ftp: ftplib.FTP):
-    files = ftp.nlst(pattern)
-    if len(files) == 0:
-        logging.warn(f"⚠️  Could not found file matching: {pattern}")
-
-    return files
-
-
-def fetch_from_zip(ftp_path: str, files: list[str]):
-    response = request.urlopen(ftp_path)
-    zip_file = ZipFile(io.BytesIO(response.read()))
-
-    lowercase_filenames = {
-        file.filename.lower(): file.filename for file in zip_file.filelist
-    }
-
-    return {file: zip_file.read(lowercase_filenames[file.lower()]) for file in files}
+"""
+Module with helper functions to interact with DATASUS ftp server
+"""
+
+import urllib.request as request
+import ftplib
+import logging
+import io
+from typing import Iterable
+import os.path as path
+import os
+from zipfile import ZipFile
+from dbfread import DBF
+import polars as pl
+import datasus_dbc
+from .utils import rm, flatten
+
+
+def fetch_dbc_as_df(ftp_path: str) -> pl.DataFrame:
+    response = request.urlopen(ftp_path)
+    dbc_raw = response.read()
+
+    filename = path.basename(ftp_path).split(".")[0]
+    dbc_file = f".tmp/{filename}.dbc"
+    dbf_file = f".tmp/{filename}.dbf"
+
+    os.makedirs(path.dirname(dbc_file), exist_ok=True)
+    with open(
+        dbc_file,
+        "wb",
+    ) as f:
+        f.write(dbc_raw)
+
+    datasus_dbc.decompress(dbc_file, dbf_file)
+
+    df = pl.DataFrame(iter(DBF(dbf_file, encoding="iso-8859-1")))
+
+    rm(dbc_file)
+    rm(dbf_file)
+
+    return df
+
+
+def get_matching_files(host: str, patterns: Iterable[str]):
+    ftp = ftplib.FTP(host)
+    ftp.login()
+
+    return set(flatten((try_nlst(pattern, ftp) for pattern in patterns)))
+
+
+def try_nlst(pattern: str, ftp: ftplib.FTP):
+    files = ftp.nlst(pattern)
+    if len(files) == 0:
+        logging.warn(f"⚠️  Could not found file matching: {pattern}")
+
+    return files
+
+
+def fetch_from_zip(ftp_path: str, files: list[str]):
+    response = request.urlopen(ftp_path)
+    zip_file = ZipFile(io.BytesIO(response.read()))
+
+    lowercase_filenames = {
+        file.filename.lower(): file.filename for file in zip_file.filelist
+    }
+
+    return {file: zip_file.read(lowercase_filenames[file.lower()]) for file in files}
```

### Comparing `datasus_db-0.1.1/datasus_db/pl_utils.py` & `datasus_db-0.1.2/datasus_db/pl_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""
-Module with helper functions to work with polars dataframes.
-"""
-
-import polars as pl
-from dataclasses import dataclass
-
-
-@dataclass
-class Column:
-    name: str
-    dtype: pl.PolarsDataType
-    strict: bool = True
-
-    def upsert(self, df: pl.DataFrame):
-        return upsert_column(df, self.name, self.dtype, strict=self.strict)
-
-
-@dataclass
-class DateColumn:
-    name: str
-    format: str
-    strict: bool = True
-
-    def upsert(self, df: pl.DataFrame):
-        return upsert_date_column(df, self.name, self.format, strict=self.strict)
-
-
-def upsert_column(df: pl.DataFrame, name: str, dtype: pl.PolarsDataType, strict=True):
-    if name in df.columns:
-        return pl.col(name).cast(dtype, strict=strict)
-    else:
-        return pl.lit(None, dtype).alias(name)
-
-
-def upsert_date_column(df: pl.DataFrame, name: str, format: str, strict=True):
-    dtype = pl.Date
-    if name in df.columns:
-        return pl.col(name).str.to_date(format, strict=strict)
-    else:
-        return pl.lit(None, dtype).alias(name)
-
-
-def to_schema(df: pl.DataFrame, schema: list[Column]):
-    schema_cols = {col.name for col in schema}
-    cols_to_remove = [col for col in df.columns if not col in schema_cols]
-    df = df.drop(cols_to_remove)
-
-    return df.with_columns([col.upsert(df) for col in schema])
-
-
-def rename_columns(df: pl.DataFrame, mapping: dict[str, str]):
-    cur_cols = set(df.columns)
-    mapping_possible = {
-        col: mapping[col] for (col) in mapping.keys() if col in cur_cols
-    }
-
-    if len(mapping_possible) == 0:
-        return df
-    else:
-        return df.rename(mapping_possible)
-
-
-def fill_empty(fill: object, col=pl.col(pl.Utf8)):
-    return pl.when(col.str.len_chars() == 0).then(fill).otherwise(col).name.keep()
-
-
-def fill_text(match: str, fill: object, col=pl.col(pl.Utf8)):
-    return pl.when(col == match).then(fill).otherwise(col).name.keep()
-
-
-def fill_non_numeric(fill: object, col: pl.Expr):
-    return pl.when(col.str.contains(r"\D")).then(fill).otherwise(col).name.keep()
+"""
+Module with helper functions to work with polars dataframes.
+"""
+
+import polars as pl
+from dataclasses import dataclass
+
+
+@dataclass
+class Column:
+    name: str
+    dtype: pl.PolarsDataType
+    strict: bool = True
+
+    def upsert(self, df: pl.DataFrame):
+        return upsert_column(df, self.name, self.dtype, strict=self.strict)
+
+
+@dataclass
+class DateColumn:
+    name: str
+    format: str
+    strict: bool = True
+
+    def upsert(self, df: pl.DataFrame):
+        return upsert_date_column(df, self.name, self.format, strict=self.strict)
+
+
+def upsert_column(df: pl.DataFrame, name: str, dtype: pl.PolarsDataType, strict=True):
+    if name in df.columns:
+        return pl.col(name).cast(dtype, strict=strict)
+    else:
+        return pl.lit(None, dtype).alias(name)
+
+
+def upsert_date_column(df: pl.DataFrame, name: str, format: str, strict=True):
+    dtype = pl.Date
+    if name in df.columns:
+        return pl.col(name).str.to_date(format, strict=strict)
+    else:
+        return pl.lit(None, dtype).alias(name)
+
+
+def to_schema(df: pl.DataFrame, schema: list[Column]):
+    schema_cols = {col.name for col in schema}
+    cols_to_remove = [col for col in df.columns if not col in schema_cols]
+    df = df.drop(cols_to_remove)
+
+    return df.with_columns([col.upsert(df) for col in schema])
+
+
+def rename_columns(df: pl.DataFrame, mapping: dict[str, str]):
+    cur_cols = set(df.columns)
+    mapping_possible = {
+        col: mapping[col] for (col) in mapping.keys() if col in cur_cols
+    }
+
+    if len(mapping_possible) == 0:
+        return df
+    else:
+        return df.rename(mapping_possible)
+
+
+def fill_empty(fill: object, col=pl.col(pl.Utf8)):
+    return pl.when(col.str.len_chars() == 0).then(fill).otherwise(col).name.keep()
+
+
+def fill_text(match: str, fill: object, col=pl.col(pl.Utf8)):
+    return pl.when(col == match).then(fill).otherwise(col).name.keep()
+
+
+def fill_non_numeric(fill: object, col: pl.Expr):
+    return pl.when(col.str.contains(r"\D")).then(fill).otherwise(col).name.keep()
```

### Comparing `datasus_db-0.1.1/pyproject.toml` & `datasus_db-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-[tool.poetry]
-name = "datasus-db"
-version = "0.1.1"
-description = "Download and import DATASUS's public data to a DuckDB database"
-authors = ["Murilo Matsubara <murilo.matsubara@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-keywords = ["datasus", "duckdb", "data science", "database"]
-packages = [
-    { include = "datasus_db" }
-]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-repository = "https://github.com/mymatsubara/datasus-db"
-
-[tool.poetry.dependencies]
-python = "^3.11"
-dbfread = "^2.0.7"
-duckdb = "^0.9.2"
-polars = "^0.19.19"
-pyarrow = "^14.0.1"
-datasus-dbc = "^0.1.1"
-
-
-[tool.poetry.group.dev.dependencies]
-pdoc = "^14.1.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "datasus-db"
+version = "0.1.2"
+description = "Download and import DATASUS's public data to a DuckDB database"
+authors = ["Murilo Matsubara <murilo.matsubara@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+keywords = ["datasus", "duckdb", "data science", "database"]
+packages = [
+    { include = "datasus_db" }
+]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+repository = "https://github.com/mymatsubara/datasus-db"
+documentation = "https://mymatsubara.github.io/datasus-db/datasus_db.html"
+
+[tool.poetry.dependencies]
+python = "^3.11"
+dbfread = "^2.0.7"
+duckdb = "^0.9.2"
+polars = "^0.19.19"
+pyarrow = "^14.0.1"
+datasus-dbc = "^0.1.1"
+
+
+[tool.poetry.group.dev.dependencies]
+pdoc = "^14.1.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `datasus_db-0.1.1/README.md` & `datasus_db-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,66 @@
-# datasus-db
-
-[![PyPI version](https://badge.fury.io/py/datasus-db.svg)](https://pypi.org/project/datasus-db/ "Go to project PyPi page")
-[![Documentation](https://img.shields.io/badge/Documentation-3fba11)](https://mymatsubara.github.io/datasus-db/datasus_db.html "Go to project documentation")
-
-A python package to **download and import** public available data from **DATASUS's** ftp servers into a [DuckDB](https://duckdb.org/) database.
-
-## Why DuckDB?
-[DuckDB](https://duckdb.org/) is a local database similar to [sqlite](https://www.sqlite.org/index.html), but it is tailor made with analytical processing in mind, which makes it a great tool for analysing DATASUS's data. To see all the features DuckDB provides, check out their [documentation](https://www.sqlite.org/index.html).
-
-
-## Installation
-```
-pip install datasus-db
-```
-
-## Usage
-
-```python
-import datasus_db
-import logging
-
-
-def main():
-    # If you want to enable logging
-    logging.getLogger().setLevel(logging.INFO)
-
-    # Import SIM DO (Sistema de Informações de Mortalidade - Declarações de Óbito) data
-    # By default the data is imported to the file `datasus.db`
-    datasus_db.import_sim_do()
-
-    # Import SIH RD (Sistema de Informações Hospitalares do SUS - AIH Reduzida) data
-    # If you want, you can import to another duckdb file changing the `db_file` argument
-    datasus_db.import_sih_rd(db_file="other-name.db")
-
-    # Import PO (Painel de Oncologia) data
-    datasus_db.import_po()
-
-    # Import IBGE POP (População IBGE - Agregada por município, sexo e faixa etaria) data
-    datasus_db.import_ibge_pop()
-
-    # Import IBGE POP TCU (População IBGE - Tribunal de Contas da União) data
-    datasus_db.import_ibge_pop_tcu()
-
-    # Import auxiliar tables (Municipios, UFs e doenças)
-    datasus_db.import_auxiliar_tables()
-
-
-if __name__ == "__main__":
-    main()
-```
-
-## Documentation
-Check out the project's documentation:
-
-[![View documentation](https://img.shields.io/badge/VIEW-DOCUMENTATION-3fba11?style=for-the-badge)](https://mymatsubara.github.io/datasus-db/datasus_db.html "Go to project documentation")
-
-## Found a bug or want a new feature?
-Feel free to create an [issue](https://github.com/mymatsubara/datasus-dbc-py/issues/new) here if you found a bug or if you want a new feature!
-
-
+# datasus-db
+
+[![PyPI version](https://badge.fury.io/py/datasus-db.svg)](https://pypi.org/project/datasus-db/ "Go to project PyPi page")
+[![Documentation](https://img.shields.io/badge/Documentation-3fba11)](https://mymatsubara.github.io/datasus-db/datasus_db.html "Go to project documentation")
+
+A python package to **download and import** public available data from **DATASUS's** ftp servers into a [DuckDB](https://duckdb.org/) database.
+
+## Why DuckDB?
+[DuckDB](https://duckdb.org/) is a local database similar to [sqlite](https://www.sqlite.org/index.html), but it is tailor made with analytical processing in mind, which makes it a great tool for analysing DATASUS's data. To see all the features DuckDB provides, check out their [documentation](https://www.sqlite.org/index.html).
+
+
+## Installation
+```
+pip install datasus-db
+```
+
+## Usage
+
+```python
+import datasus_db
+import logging
+
+
+def main():
+    # If you want to enable logging
+    logging.getLogger().setLevel(logging.INFO)
+
+    # Import SIM DO (Sistema de Informações de Mortalidade - Declarações de Óbito) data
+    # By default the data is imported to the file `datasus.db`
+    datasus_db.import_sim_do()
+
+    # Import PO (Painel de Oncologia) data
+    datasus_db.import_po(db_file="other-name.db")
+
+    # Import SIH RD (Sistema de Informações Hospitalares do SUS - AIH Reduzida) data
+    datasus_db.import_sih_rd()
+
+    # Import SP (Autorização de Internação Hospitalar Saúde do Profissional) from SIHSUS (Sistema de Informações Hospitalares do SUS).
+    datasus_db.import_sih_sp()
+
+    # Import PA (Produção Ambulatorial) from SIASUS (Sistema de Informações Ambulatorial do SUS).
+    datasus_db.import_sia_pa()
+
+    # Import IBGE POP (População IBGE - Agregada por município, sexo e faixa etaria) data
+    datasus_db.import_ibge_pop()
+
+    # Import IBGE POP TCU (População IBGE - Tribunal de Contas da União) data
+    datasus_db.import_ibge_pop_tcu()
+
+    # Import auxiliar tables (Municipios, UFs e doenças)
+    datasus_db.import_auxiliar_tables()
+
+
+if __name__ == "__main__":
+    main()
+```
+
+## Documentation
+Check out the project's documentation:
+
+[![View documentation](https://img.shields.io/badge/VIEW-DOCUMENTATION-3fba11?style=for-the-badge)](https://mymatsubara.github.io/datasus-db/datasus_db.html "Go to project documentation")
+
+## Found a bug or want a new feature?
+Feel free to create an [issue](https://github.com/mymatsubara/datasus-dbc-py/issues/new) here if you found a bug or if you want a new feature!
+
+
```

### Comparing `datasus_db-0.1.1/PKG-INFO` & `datasus_db-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasus-db
-Version: 0.1.1
+Version: 0.1.2
 Summary: Download and import DATASUS's public data to a DuckDB database
 Home-page: https://github.com/mymatsubara/datasus-db
 License: MIT
 Keywords: datasus,duckdb,data science,database
 Author: Murilo Matsubara
 Author-email: murilo.matsubara@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasus-dbc (>=0.1.1,<0.2.0)
 Requires-Dist: dbfread (>=2.0.7,<3.0.0)
 Requires-Dist: duckdb (>=0.9.2,<0.10.0)
 Requires-Dist: polars (>=0.19.19,<0.20.0)
 Requires-Dist: pyarrow (>=14.0.1,<15.0.0)
+Project-URL: Documentation, https://mymatsubara.github.io/datasus-db/datasus_db.html
 Project-URL: Repository, https://github.com/mymatsubara/datasus-db
 Description-Content-Type: text/markdown
 
 # datasus-db
 
 [![PyPI version](https://badge.fury.io/py/datasus-db.svg)](https://pypi.org/project/datasus-db/ "Go to project PyPi page")
 [![Documentation](https://img.shields.io/badge/Documentation-3fba11)](https://mymatsubara.github.io/datasus-db/datasus_db.html "Go to project documentation")
@@ -48,20 +49,25 @@
     # If you want to enable logging
     logging.getLogger().setLevel(logging.INFO)
 
     # Import SIM DO (Sistema de Informações de Mortalidade - Declarações de Óbito) data
     # By default the data is imported to the file `datasus.db`
     datasus_db.import_sim_do()
 
+    # Import PO (Painel de Oncologia) data
+    datasus_db.import_po(db_file="other-name.db")
+
     # Import SIH RD (Sistema de Informações Hospitalares do SUS - AIH Reduzida) data
-    # If you want, you can import to another duckdb file changing the `db_file` argument
-    datasus_db.import_sih_rd(db_file="other-name.db")
+    datasus_db.import_sih_rd()
 
-    # Import PO (Painel de Oncologia) data
-    datasus_db.import_po()
+    # Import SP (Autorização de Internação Hospitalar Saúde do Profissional) from SIHSUS (Sistema de Informações Hospitalares do SUS).
+    datasus_db.import_sih_sp()
+
+    # Import PA (Produção Ambulatorial) from SIASUS (Sistema de Informações Ambulatorial do SUS).
+    datasus_db.import_sia_pa()
 
     # Import IBGE POP (População IBGE - Agregada por município, sexo e faixa etaria) data
     datasus_db.import_ibge_pop()
 
     # Import IBGE POP TCU (População IBGE - Tribunal de Contas da União) data
     datasus_db.import_ibge_pop_tcu()
```

