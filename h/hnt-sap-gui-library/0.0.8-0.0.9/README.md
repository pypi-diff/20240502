# Comparing `tmp/hnt_sap_gui_library-0.0.8.tar.gz` & `tmp/hnt_sap_gui_library-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_sap_gui_library-0.0.8.tar", last modified: Tue Mar 12 17:43:10 2024, max compression
+gzip compressed data, was "hnt_sap_gui_library-0.0.9.tar", last modified: Tue Mar 26 14:28:43 2024, max compression
```

## Comparing `hnt_sap_gui_library-0.0.8.tar` & `hnt_sap_gui_library-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 17:43:10.433439 hnt_sap_gui_library-0.0.8/
--rw-rw-rw-   0        0        0      252 2024-03-12 17:43:10.428674 hnt_sap_gui_library-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2024-03-12 13:53:27.000000 hnt_sap_gui_library-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 17:43:10.342159 hnt_sap_gui_library-0.0.8/hnt_sap_gui/
--rw-rw-rw-   0        0        0       22 2024-03-12 15:33:47.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:43:10.350735 hnt_sap_gui_library-0.0.8/hnt_sap_gui/common/
--rw-rw-rw-   0        0        0      322 2024-03-12 13:53:27.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui/common/sap_status_bar.py
--rw-rw-rw-   0        0        0     1932 2024-03-12 13:53:27.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui/common/session.py
--rw-rw-rw-   0        0        0      724 2024-03-12 15:42:19.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui/hnt_sap.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:43:10.358829 hnt_sap_gui_library-0.0.8/hnt_sap_gui/nota_fiscal/
--rw-rw-rw-   0        0        0      204 2024-03-12 13:53:27.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui/nota_fiscal/miro_transaction.py
--rw-rw-rw-   0        0        0     7216 2024-03-12 15:40:24.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:43:10.426674 hnt_sap_gui_library-0.0.8/hnt_sap_gui_library.egg-info/
--rw-rw-rw-   0        0        0      252 2024-03-12 17:43:10.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2024-03-12 17:43:10.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 17:43:10.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-03-12 17:43:10.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-12 17:43:10.000000 hnt_sap_gui_library-0.0.8/hnt_sap_gui_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-12 17:43:10.434204 hnt_sap_gui_library-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      430 2024-03-12 17:43:08.000000 hnt_sap_gui_library-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:43:10.420239 hnt_sap_gui_library-0.0.8/tests/
--rw-rw-rw-   0        0        0      504 2024-03-12 15:40:24.000000 hnt_sap_gui_library-0.0.8/tests/test_nota_pedido.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-03-26 14:28:43.450694 hnt_sap_gui_library-0.0.9/
+-rw-r--r--   0 ipepe      (501) staff       (20)      243 2024-03-26 14:28:43.449766 hnt_sap_gui_library-0.0.9/PKG-INFO
+-rw-r--r--   0 ipepe      (501) staff       (20)     1500 2024-03-26 14:25:55.000000 hnt_sap_gui_library-0.0.9/README.md
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-03-26 14:28:43.420996 hnt_sap_gui_library-0.0.9/hnt_sap_gui/
+-rw-r--r--   0 ipepe      (501) staff       (20)       22 2024-03-26 14:25:55.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/__init__.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-03-26 14:28:43.423084 hnt_sap_gui_library-0.0.9/hnt_sap_gui/common/
+-rw-r--r--   0 ipepe      (501) staff       (20)      311 2024-03-26 14:25:55.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/common/sap_status_bar.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     1886 2024-03-26 14:25:55.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/common/session.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      884 2024-03-26 14:26:04.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/hnt_sap.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-03-26 14:28:43.430689 hnt_sap_gui_library-0.0.9/hnt_sap_gui/nota_fiscal/
+-rw-r--r--   0 ipepe      (501) staff       (20)      870 2024-03-26 14:26:04.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      202 2024-03-26 14:25:55.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/nota_fiscal/miro_transaction.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     7127 2024-03-26 14:25:55.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-03-26 14:28:43.448950 hnt_sap_gui_library-0.0.9/hnt_sap_gui_library.egg-info/
+-rw-r--r--   0 ipepe      (501) staff       (20)      243 2024-03-26 14:28:42.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui_library.egg-info/PKG-INFO
+-rw-r--r--   0 ipepe      (501) staff       (20)      516 2024-03-26 14:28:43.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui_library.egg-info/SOURCES.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)        1 2024-03-26 14:28:42.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui_library.egg-info/dependency_links.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)       43 2024-03-26 14:28:42.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui_library.egg-info/requires.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)       12 2024-03-26 14:28:42.000000 hnt_sap_gui_library-0.0.9/hnt_sap_gui_library.egg-info/top_level.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)       38 2024-03-26 14:28:43.450850 hnt_sap_gui_library-0.0.9/setup.cfg
+-rw-r--r--   0 ipepe      (501) staff       (20)      417 2024-03-26 14:26:04.000000 hnt_sap_gui_library-0.0.9/setup.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-03-26 14:28:43.447990 hnt_sap_gui_library-0.0.9/tests/
+-rw-r--r--   0 ipepe      (501) staff       (20)      464 2024-03-26 14:26:04.000000 hnt_sap_gui_library-0.0.9/tests/test_nota_pedido.py
```

### Comparing `hnt_sap_gui_library-0.0.8/README.md` & `hnt_sap_gui_library-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hnt_sap_gui_library-0.0.8/hnt_sap_gui/common/session.py` & `hnt_sap_gui_library-0.0.9/hnt_sap_gui/common/session.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from functools import wraps
-import os
-import logging
-
-logger = logging.getLogger(__name__)
-
-def sessionable(original_function):
-    @wraps(original_function)
-    def wrapped(*args, **kwargs):
-        this = args[0]
-        try:
-            _open(this)
-            response = original_function(*args, **kwargs)
-            _close(this)
-            return response
-        except Exception as exception:
-            logger.error(msg=str(exception))
-            if exception.args[0].endswith("object has no attribute 'sapapp'"):
-                raise exception
-            _close(this)
-    return wrapped
-
-def _open(sap_gui):
-    logger.info("enter _open")
-    sap_gui.connect_to_session()
-    
-    sap_gui.open_connection(os.getenv("SAP_OPEN_CONNECTION"))
-
-    sap_gui.session.findById("wnd[0]/usr/txtRSYST-MANDT").text = os.getenv("SAP_MANDANTE")
-    sap_gui.session.findById("wnd[0]/usr/txtRSYST-BNAME").text = os.getenv("SAP_USERNAME")
-    sap_gui.session.findById("wnd[0]/usr/pwdRSYST-BCODE").text = os.getenv("SAP_PASSWORD")
-    sap_gui.session.findById("wnd[0]/usr/txtRSYST-LANGU").text = os.getenv("SAP_LANGUAGE")
-    sap_gui.send_vkey(0)
-    if sap_gui.session.findById("wnd[1]/usr/radMULTI_LOGON_OPT2", False) != None:
-        sap_gui.session.findById("wnd[1]/usr/radMULTI_LOGON_OPT2").select()
-        sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]").press()
-        if sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]", False) != None:
-            sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]").press()
-    elif sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]", False) != None:
-        sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]").press()
-    logger.info("leave _open")
-
-def _close(sap_gui):
-    logger.info("enter _close")
-    sap_gui.session.findById("wnd[0]").close()
-    sap_gui.session.findById("wnd[1]/usr/btnSPOP-OPTION1").press()
+from functools import wraps
+import os
+import logging
+
+logger = logging.getLogger(__name__)
+
+def sessionable(original_function):
+    @wraps(original_function)
+    def wrapped(*args, **kwargs):
+        this = args[0]
+        try:
+            _open(this)
+            response = original_function(*args, **kwargs)
+            _close(this)
+            return response
+        except Exception as exception:
+            logger.error(msg=str(exception))
+            if exception.args[0].endswith("object has no attribute 'sapapp'"):
+                raise exception
+            _close(this)
+    return wrapped
+
+def _open(sap_gui):
+    logger.info("enter _open")
+    sap_gui.connect_to_session()
+    
+    sap_gui.open_connection(os.getenv("SAP_OPEN_CONNECTION"))
+
+    sap_gui.session.findById("wnd[0]/usr/txtRSYST-MANDT").text = os.getenv("SAP_MANDANTE")
+    sap_gui.session.findById("wnd[0]/usr/txtRSYST-BNAME").text = os.getenv("SAP_USERNAME")
+    sap_gui.session.findById("wnd[0]/usr/pwdRSYST-BCODE").text = os.getenv("SAP_PASSWORD")
+    sap_gui.session.findById("wnd[0]/usr/txtRSYST-LANGU").text = os.getenv("SAP_LANGUAGE")
+    sap_gui.send_vkey(0)
+    if sap_gui.session.findById("wnd[1]/usr/radMULTI_LOGON_OPT2", False) != None:
+        sap_gui.session.findById("wnd[1]/usr/radMULTI_LOGON_OPT2").select()
+        sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]").press()
+        if sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]", False) != None:
+            sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]").press()
+    elif sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]", False) != None:
+        sap_gui.session.findById("wnd[1]/tbar[0]/btn[0]").press()
+    logger.info("leave _open")
+
+def _close(sap_gui):
+    logger.info("enter _close")
+    sap_gui.session.findById("wnd[0]").close()
+    sap_gui.session.findById("wnd[1]/usr/btnSPOP-OPTION1").press()
     logger.info("leave _close")
```

### Comparing `hnt_sap_gui_library-0.0.8/hnt_sap_gui/hnt_sap.py` & `hnt_sap_gui_library-0.0.9/hnt_sap_gui/hnt_sap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-import logging
-from SapGuiLibrary import SapGuiLibrary
-from dotenv import load_dotenv
-from .common.session import sessionable
-from .nota_fiscal.nota_pedido_transaction import NotaPedidoTransaction
-
-logger = logging.getLogger(__name__)
-
-class SapGui(SapGuiLibrary):
-    def __init__(self) -> None:
-        load_dotenv()
-        pass
-
-    @sessionable
-    def hnt_run_transaction(self, data):
-        logger.info(f"enter execute run_hnt_transactions data:{data}")
-        codigo = NotaPedidoTransaction().execute(self, nota_pedido=data)
-        result = {
-            "codigo": codigo
-        }
-        logger.info(f"leave execute run_hnt_transactions result{str(result)}")
-        return result
+import logging
+from SapGuiLibrary import SapGuiLibrary
+from dotenv import load_dotenv
+
+from .common.session import sessionable
+from .nota_fiscal.nota_pedido_transaction import NotaPedidoTransaction
+from .nota_fiscal.liberacao_transaction import LiberacaoTransaction
+
+logger = logging.getLogger(__name__)
+
+class SapGui(SapGuiLibrary):
+    def __init__(self) -> None:
+        load_dotenv()
+        pass
+
+    @sessionable
+    def hnt_run_transaction(self, data):
+        logger.info(f"enter execute run_hnt_transactions data:{data}")
+        codigo = NotaPedidoTransaction().execute(self, nota_pedido=data)
+        cod_liberacao = LiberacaoTransaction().execute(self, codigo)
+        result = {
+            "codigo": codigo,
+            "cod_liberacao": cod_liberacao
+        }
+        logger.info(f"leave execute run_hnt_transactions result{str(result)}")
+        return result
```

### Comparing `hnt_sap_gui_library-0.0.8/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py` & `hnt_sap_gui_library-0.0.9/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import logging
-import re
-
-from hnt_sap_gui.common.sap_status_bar import sbar_extracted_text
-
-
-logger = logging.getLogger(__name__)
-MSG_SAP_CODIGO_NOTA_PEDIDO = "^Ped.C.Custo\\/Ordem criado sob o nº ([0-9]{10,11})$"
-class NotaPedidoTransaction:
-    def __init__(self) -> None:
-        pass
-
-    def execute(self, sapGuiLib, nota_pedido):
-        logger.info(f"enter execute nota_pedido:{nota_pedido}")
-        sapGuiLib.run_transaction('/nme21n')
-
-        sapGuiLib.send_vkey(0)
-
-        # REORGANIZA ELEMENTOS PARA GARANTIR QUE CABEÇALHO ESTEJA ABERTO
-        sapGuiLib.send_vkey(29) # Fechar Cabeçalho
-        sapGuiLib.send_vkey(30) # Fechar Síntese de itens
-        sapGuiLib.send_vkey(31) # Fechar Detahe de item
-        sapGuiLib.send_vkey(26) # Abrir Cabeçalho
-
-        # PREENCHE DADOS INICIAIS (Antes do cabeçalho)
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/cmbMEPO_TOPLINE-BSART").Key = nota_pedido['tipo'] # Define o tipo de pedido como Ped.C.Custo/Ordem
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/ctxtMEPO_TOPLINE-SUPERFIELD").Text = nota_pedido['cod_fornecedor'] # Fornecedor
-
-        # CABEÇALHO | Aba Dados Organizacionais
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9").Select() #Seleciona a aba Dados organizacionais
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKORG").Text = nota_pedido['org_compras'] #orgCompras
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKGRP").Text = nota_pedido['grp_compradores'] #grpCompradores '(Constante: S01)
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-BUKRS").Text = nota_pedido['empresa'] #empresa '(Constante: HFNT)
-        # Application.Wait Now + #12:00:02 AM# '(Avaliar a necessidade de inserir espera)
-
-        # REORGANIZA ELEMENTOS PARA GARANTIR QUE SÍNTESE DE ITENS ESTEJA ABERTO
-        sapGuiLib.send_vkey(29) #Fechar cabeçalho
-        sapGuiLib.send_vkey(27) #Abrir Síntese de itens
-        sapGuiLib.send_vkey(31) #Fechar Detahe de item
-        sapGuiLib.send_vkey(26) #Abrir Cabeçalho
-        sapGuiLib.send_vkey(29) #Fechar cabeçalho
-
-
-        # SÍNTESE DE ITENS
-        for sintese_de_iten in nota_pedido['sintese_itens']: 
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-KNTTP[2,0]").Text = sintese_de_iten['categoria_cc'] #categoriaCC '(Constante: K)
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-EMATN[4,0]").Text = sintese_de_iten['cod_material']  # material
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/txtMEPO1211-MENGE[6,0]").Text = sintese_de_iten['quantidade'] #quantidade
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-NAME1[10,0]").Text = sintese_de_iten['item']['centro'] #centro 'Local de negócio
-            sapGuiLib.send_vkey(0)
-
-
-            # DETALHES DE ITEM | Aba C|C
-
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13").Select() #Seleciona a aba C|C
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13/ssubTABSTRIPCONTROL1SUB:SAPLMEVIEWS:1101/subSUB2:SAPLMEACCTVI:0100/subSUB1:SAPLMEACCTVI:1100/subKONTBLOCK:SAPLKACB:1101/ctxtCOBL-KOSTL").Text = sintese_de_iten['item']['centro_custo'] #centroCusto
-            sapGuiLib.send_vkey(0)
-            sapGuiLib.send_vkey(0)
-            sapGuiLib.send_vkey(0)
-
-
-            # DETALHES DE ITEM | Aba Fatura
-
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7").Select() #Seleciona a aba fatura
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0015/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1317/ctxtMEPO1317-MWSKZ").Text = sintese_de_iten['item']['cod_imposto'] #codigoImposto #Inclui o código do imposto
-            sapGuiLib.send_vkey(0 )
-
-
-            # DETALHES DE ITEM | Aba Condições
-
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0015/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8").Select() #Seleciona a aba Condições
-            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1333/ssubSUB0:SAPLV69A:6201/tblSAPLV69ATCTRL_KONDITIONEN/txtKOMV-KBETR[3,1]").Text = sintese_de_iten['item']['valor_bruto'] #valorItem 'Valor bruto
-            sapGuiLib.send_vkey(0 )
-
-        # PROCESSO PARA ANEXAR O DOCUMENTO NO PEDIDO
-        sapGuiLib.session.findById("wnd[0]/titl/shellcont/shell").pressButton("%GOS_TOOLBOX")
-        sapGuiLib.session.findById("wnd[0]/shellcont[1]/shell").pressContextButton("CREATE_ATTA")
-        sapGuiLib.session.findById("wnd[0]/shellcont[1]/shell").selectContextMenuItem("PCATTA_CREA")
-        sapGuiLib.session.findById("wnd[1]/usr/ctxtDY_PATH").Text = nota_pedido['anexo']['path'] #Diretório de NFs
-        sapGuiLib.session.findById("wnd[1]/usr/ctxtDY_FILENAME").Text = nota_pedido['anexo']['filename'] #PDF da DANFE
-        sapGuiLib.session.findById("wnd[1]/tbar[0]/btn[0]").press()
-
-        sapGuiLib.session.findById("wnd[0]/tbar[0]/btn[11]").press() #'Grava o lançamento
-
-        cod_nota_pedido = sbar_extracted_text(MSG_SAP_CODIGO_NOTA_PEDIDO,
-                                              sapGuiLib.session.findById("wnd[0]/sbar").Text)
-
-        logger.info(f"Leave execute código da nota_pedido:{cod_nota_pedido}")
-        return cod_nota_pedido
+import logging
+import re
+
+from hnt_sap_gui.common.sap_status_bar import sbar_extracted_text
+
+
+logger = logging.getLogger(__name__)
+MSG_SAP_CODIGO_NOTA_PEDIDO = "^Ped.C.Custo\\/Ordem criado sob o nº ([0-9]{10,11})$"
+class NotaPedidoTransaction:
+    def __init__(self) -> None:
+        pass
+
+    def execute(self, sapGuiLib, nota_pedido):
+        logger.info(f"enter execute nota_pedido:{nota_pedido}")
+        sapGuiLib.run_transaction('/nme21n')
+
+        sapGuiLib.send_vkey(0)
+
+        # REORGANIZA ELEMENTOS PARA GARANTIR QUE CABEÇALHO ESTEJA ABERTO
+        sapGuiLib.send_vkey(29) # Fechar Cabeçalho
+        sapGuiLib.send_vkey(30) # Fechar Síntese de itens
+        sapGuiLib.send_vkey(31) # Fechar Detahe de item
+        sapGuiLib.send_vkey(26) # Abrir Cabeçalho
+
+        # PREENCHE DADOS INICIAIS (Antes do cabeçalho)
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/cmbMEPO_TOPLINE-BSART").Key = nota_pedido['tipo'] # Define o tipo de pedido como Ped.C.Custo/Ordem
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/ctxtMEPO_TOPLINE-SUPERFIELD").Text = nota_pedido['cod_fornecedor'] # Fornecedor
+
+        # CABEÇALHO | Aba Dados Organizacionais
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9").Select() #Seleciona a aba Dados organizacionais
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKORG").Text = nota_pedido['org_compras'] #orgCompras
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKGRP").Text = nota_pedido['grp_compradores'] #grpCompradores '(Constante: S01)
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-BUKRS").Text = nota_pedido['empresa'] #empresa '(Constante: HFNT)
+        # Application.Wait Now + #12:00:02 AM# '(Avaliar a necessidade de inserir espera)
+
+        # REORGANIZA ELEMENTOS PARA GARANTIR QUE SÍNTESE DE ITENS ESTEJA ABERTO
+        sapGuiLib.send_vkey(29) #Fechar cabeçalho
+        sapGuiLib.send_vkey(27) #Abrir Síntese de itens
+        sapGuiLib.send_vkey(31) #Fechar Detahe de item
+        sapGuiLib.send_vkey(26) #Abrir Cabeçalho
+        sapGuiLib.send_vkey(29) #Fechar cabeçalho
+
+
+        # SÍNTESE DE ITENS
+        for sintese_de_iten in nota_pedido['sintese_itens']: 
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-KNTTP[2,0]").Text = sintese_de_iten['categoria_cc'] #categoriaCC '(Constante: K)
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-EMATN[4,0]").Text = sintese_de_iten['cod_material']  # material
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/txtMEPO1211-MENGE[6,0]").Text = sintese_de_iten['quantidade'] #quantidade
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0016/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-NAME1[10,0]").Text = sintese_de_iten['item']['centro'] #centro 'Local de negócio
+            sapGuiLib.send_vkey(0)
+
+
+            # DETALHES DE ITEM | Aba C|C
+
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13").Select() #Seleciona a aba C|C
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13/ssubTABSTRIPCONTROL1SUB:SAPLMEVIEWS:1101/subSUB2:SAPLMEACCTVI:0100/subSUB1:SAPLMEACCTVI:1100/subKONTBLOCK:SAPLKACB:1101/ctxtCOBL-KOSTL").Text = sintese_de_iten['item']['centro_custo'] #centroCusto
+            sapGuiLib.send_vkey(0)
+            sapGuiLib.send_vkey(0)
+            sapGuiLib.send_vkey(0)
+
+
+            # DETALHES DE ITEM | Aba Fatura
+
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7").Select() #Seleciona a aba fatura
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0015/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1317/ctxtMEPO1317-MWSKZ").Text = sintese_de_iten['item']['cod_imposto'] #codigoImposto #Inclui o código do imposto
+            sapGuiLib.send_vkey(0 )
+
+
+            # DETALHES DE ITEM | Aba Condições
+
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0015/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8").Select() #Seleciona a aba Condições
+            sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0019/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1333/ssubSUB0:SAPLV69A:6201/tblSAPLV69ATCTRL_KONDITIONEN/txtKOMV-KBETR[3,1]").Text = sintese_de_iten['item']['valor_bruto'] #valorItem 'Valor bruto
+            sapGuiLib.send_vkey(0 )
+
+        # PROCESSO PARA ANEXAR O DOCUMENTO NO PEDIDO
+        sapGuiLib.session.findById("wnd[0]/titl/shellcont/shell").pressButton("%GOS_TOOLBOX")
+        sapGuiLib.session.findById("wnd[0]/shellcont[1]/shell").pressContextButton("CREATE_ATTA")
+        sapGuiLib.session.findById("wnd[0]/shellcont[1]/shell").selectContextMenuItem("PCATTA_CREA")
+        sapGuiLib.session.findById("wnd[1]/usr/ctxtDY_PATH").Text = nota_pedido['anexo']['path'] #Diretório de NFs
+        sapGuiLib.session.findById("wnd[1]/usr/ctxtDY_FILENAME").Text = nota_pedido['anexo']['filename'] #PDF da DANFE
+        sapGuiLib.session.findById("wnd[1]/tbar[0]/btn[0]").press()
+
+        sapGuiLib.session.findById("wnd[0]/tbar[0]/btn[11]").press() #'Grava o lançamento
+
+        cod_nota_pedido = sbar_extracted_text(MSG_SAP_CODIGO_NOTA_PEDIDO,
+                                              sapGuiLib.session.findById("wnd[0]/sbar").Text)
+
+        logger.info(f"Leave execute código da nota_pedido:{cod_nota_pedido}")
+        return cod_nota_pedido
```

