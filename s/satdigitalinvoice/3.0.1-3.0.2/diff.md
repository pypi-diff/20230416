# Comparing `tmp/satdigitalinvoice-3.0.1.tar.gz` & `tmp/satdigitalinvoice-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-3.0.1.tar", last modified: Sat Apr 15 21:41:52 2023, max compression
+gzip compressed data, was "satdigitalinvoice-3.0.2.tar", last modified: Sun Apr 16 00:16:02 2023, max compression
```

## Comparing `satdigitalinvoice-3.0.1.tar` & `satdigitalinvoice-3.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    37039 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37228 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_main.py
```

### Comparing `satdigitalinvoice-3.0.1/PKG-INFO` & `satdigitalinvoice-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.1
+Version: 3.0.2
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/__init__.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,18 @@
     fh.setLevel(logging.ERROR)
     formatter = logging.Formatter('%(asctime)s - %(message)s')
     fh.setFormatter(formatter)
     logging.root.addHandler(fh)
 
 
 class FacturacionLauncher:
-
-    def __init__(self, cwd=None, debug=False):
+    def __init__(self, cwd=None):
         app_dir = os.getcwd()
-
         if cwd:
             os.chdir(cwd)
-
-        # set up logging
-        if debug:
-            logging.basicConfig(
-                level=logging.DEBUG,
-                stream=sys.stderr,
-            )
         add_file_handler()
 
         # loading the sample.zip
         try:
             with ZipFile(os.path.join(app_dir, 'sample.zip'), 'r') as zf:
                 for member in zf.infolist():
                     if not os.path.exists(member.filename):
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/__version__.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/client_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,51 +17,51 @@
 def validar_client(client):
     rfc = client['Rfc']
     try:
         rfc = RFC(rfc)
         if not rfc.is_valid():
             raise ValueError("RFC Not Valid Regex")
     except ValueError as ex:
-        logger.info(f"{rfc}: {ex}")
+        print(f"{rfc}: {ex}")
         return
 
     for email in client["Email"]:
         match = re.fullmatch(EMAIL_REGEX, email)
         if not match:
-            logger.info(f"{rfc}: Correo '{email}' is invalid")
+            print(f"{rfc}: Correo '{email}' is invalid")
 
     if id_cif := client["IdCIF"]:
         try:
             res = csf.retrieve(rfc, id_cif=id_cif)
         except ValueError as ex:
-            logger.info(f"{rfc}: idCIF '{id_cif}' is invalid")
+            print(f"{rfc}: idCIF '{id_cif}' is invalid")
             return
 
         if rfc.type == RFCType.MORAL:
             if client['RazonSocial'] != res['Denominación o Razón Social']:
-                logger.info(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Denominación o Razón Social']}'")
+                print(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Denominación o Razón Social']}'")
         elif rfc.type == RFCType.FISICA:
             if client['RazonSocial'] != f"{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}":
-                logger.info(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}'")
+                print(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}'")
 
         if client['CodigoPostal'] != res['CP']:
-            logger.info(f"{rfc}: CodigoPostal '{client['CodigoPostal']}' is invalid, expected '{res['CP']}'")
+            print(f"{rfc}: CodigoPostal '{client['CodigoPostal']}' is invalid, expected '{res['CP']}'")
 
         if client['RegimenFiscal'] not in (r['RegimenFiscal'] for r in res['Regimenes']):
-            logger.info(
+            print(
                 f"{rfc}: RegimenFiscal '{client['RegimenFiscal']}' is invalid, "
                 f"expected '{(r['RegimenFiscal'].code for r in res['Regimenes'])}'"
             )
 
         if res['Situación del contribuyente'] not in ['ACTIVO', 'REACTIVADO']:
-            logger.info(f"{rfc}: Is not ACTIVO '{res['Situación del contribuyente']}'")
+            print(f"{rfc}: Is not ACTIVO '{res['Situación del contribuyente']}'")
 
         taxpayer_status = sat_service.list_69b(rfc)
         if taxpayer_status:
-            logger.info(f"{rfc}: has status '{taxpayer_status}'")
+            print(f"{rfc}: has status '{taxpayer_status}'")
 
 
 def clientes_generar_txt(clients):
     with open("clientes.txt", 'w') as f:
         for i, (cliente_rfc, cliente_data) in enumerate(clients.items(), start=1):
             f.write(f"{i}|{cliente_rfc}|{cliente_data['RazonSocial']}|{cliente_data['CodigoPostal']}")
             f.write("\n")
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/environments.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/facturacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         self.window['facturas_table'].bind('<Double-Button-1>', '_double_click')
         self.window['clientes_table'].bind('<Double-Button-1>', '_double_click')
         self.window['emitidas_table'].bind('<Double-Button-1>', '_double_click')
         self.window['ajustes_table'].bind('<Double-Button-1>', '_double_click')
 
         # Add logging to the window
         h = logging.StreamHandler(self.window['console'])
-        h.setLevel(logging.INFO)
+        h.setLevel(logging.ERROR)
         logging.root.addHandler(h)
 
         self.main_loop()
         self.window.close()
 
     def initial_screen(self, emisor_cif):
         self.header("ACERCA DE")
@@ -562,29 +562,32 @@
                                     receptor = clients[rfc]  # type: dict
                                     valor_unitario_raw = concepto["ValorUnitario"]
 
                                     if isinstance(valor_unitario_raw, dict):
                                         vud, vu = find_best_match(valor_unitario_raw, dp)
                                         vund, vun = find_best_match(valor_unitario_raw, dp_effective)
                                         meses = months_between(vund, vud)
-                                        ajuste_porcentaje = (vun / vu - 1)
+                                        if vun and vu:
+                                            ajuste_porcentaje = (vun / vu - 1)
+                                        else:
+                                            ajuste_porcentaje = None
                                     else:
                                         vu = valor_unitario_raw
                                         vun = None
                                         meses = None
                                         ajuste_porcentaje = None
 
                                     concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
                                     file_name = os.path.join(ajustes_dir, f'AjusteRenta_{rfc}_{i}.pdf')
 
                                     data = {
                                         "receptor": receptor,
                                         "emisor": clients[emisor_rfc],
                                         "concepto": concepto,
-                                        "valor_unitario": pesos(vu),
+                                        "valor_unitario": pesos(vu) if vu else "",
                                         "valor_unitario_nuevo": pesos(vun) if vun else "",
                                         "ajuste_porcentaje": porcentaje(ajuste_porcentaje, 2) if ajuste_porcentaje is not None else "",
                                         "ajuste_periodo": f"{meses} MESES",
                                         "efectivo_periodo_desc": periodicidad_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),
                                         "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
                                         "fecha_hoy": fecha(date.today()),
                                         'file_name': file_name
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/gui_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         conceptos=factura_details["Conceptos"]
     )
     invoice = invoice.process()
 
     expected_total = factura_details.get('Total')
     if expected_total is not None:
         if expected_total != invoice['Total']:
-            logger.info(f"{factura_details['Receptor']}: Total '{expected_total}' is invalid, expected '{invoice['Total']}'")
+            print(f"{factura_details['Receptor']}: Total '{expected_total}' is invalid, expected '{invoice['Total']}'")
             return None
 
     return invoice
 
 
 def parse_periodo_mes_ajuste(periodo_mes_ajuste: str):
     parts = periodo_mes_ajuste.split(".")
@@ -101,27 +101,27 @@
 
 
 def validad_facturas(clients, facturas):
     is_valid = True
     for factura_details in facturas:
         cliente = clients.get(factura_details['Receptor'])
         if not cliente:
-            logger.info(f"{factura_details['Receptor']}: client not found")
+            print(f"{factura_details['Receptor']}: client not found")
             is_valid = False
 
         for c in factura_details["Conceptos"]:
             periodo_mes_ajuste = c.get("_periodo_mes_ajuste", "")
             try:
                 parse_periodo_mes_ajuste(periodo_mes_ajuste)
             except ValueError:
-                logger.info(f"{factura_details['Receptor']}: _periodo_mes_ajuste '{periodo_mes_ajuste}' is invalid")
+                print(f"{factura_details['Receptor']}: _periodo_mes_ajuste '{periodo_mes_ajuste}' is invalid")
                 is_valid = False
 
         if factura_details["MetodoPago"] == "PPD" and factura_details["FormaPago"] != "99":
-            logger.info(f"{factura_details['Receptor']}: FormaPago '{factura_details['FormaPago']}' is invalid, expected '99' for PPD")
+            print(f"{factura_details['Receptor']}: FormaPago '{factura_details['FormaPago']}' is invalid, expected '99' for PPD")
             is_valid = False
 
     return is_valid
 
 
 def period_desc(dp: DatePeriod):
     return format_date(date(year=dp.year, month=dp.month, day=1), locale='es_MX', format="'Mes de' MMMM 'del' y").upper()
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-3.0.2/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/layout.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/localdb.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-3.0.2/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice/utils.py` & `satdigitalinvoice-3.0.2/satdigitalinvoice/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             # "emailAddress": signer.certificate.get_subject().emailAddress,
             #
             "Expira": convert_ans1_date(signer.certificate.get_notAfter()),
             "Creado": convert_ans1_date(signer.certificate.get_notBefore()),
         }
 
 
-def find_best_match(cases, dp: DatePeriod):
+def find_best_match(cases, dp: DatePeriod) -> (datetime, object):
     fk, fv = (None, None)
     for k, v in cases.items():
         k = datetime.strptime(k, '%Y-%m')
         if k <= dp:
             if fk is None or k > fk:
                 fk, fv = k, v
     return fk, fv
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.1
+Version: 3.0.2
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/setup.py` & `satdigitalinvoice-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/tests/test_crear_facturas.py` & `satdigitalinvoice-3.0.2/tests/test_crear_facturas.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 ym_date = DatePeriod(year=2023, month=4)
 clients = ClientsManager()
 module = __package__
 
 
 def test_generar_ingresos(caplog):
     caplog.set_level(logging.INFO)
-    config = ConfigManager()
     facturas = FacturasManager(ym_date)["Facturas"]
 
     with mock.patch(f'satcfdi.create.cfd.cfdi40.datetime') as m:
         m.now = mock.Mock(return_value=datetime(2022, 1, 1))
 
         facturas = generate_ingresos(
             clients=clients,
@@ -43,47 +42,47 @@
         verify = verify_result(data=pp.pformat(facturas), filename=f"facturas.pretty.py")
         assert verify
 
     # assert facturas[0]["Total"] == Decimal('18065.66')
     # assert facturas[0]["Conceptos"][0]["Descripcion"] == 1000
 
 
-def test_generar_ingresos_error(caplog):
+def test_generar_ingresos_error(caplog, capsys):
     caplog.set_level(logging.INFO)
-    config = ConfigManager()
     facturas = FacturasManager(ym_date)["FacturasIncorrectas"]
     print(len(facturas))
 
     ingresos = generate_ingresos(
         clients=clients,
         facturas=facturas,
         dp=date(year=2023, month=4, day=1),
         emisor_rfc=csd_signer.rfc
     )
 
-    assert len(caplog.records) == 1
-    assert caplog.records[0].message == "ABMG891115PD7: Total '41000.16' is invalid, expected '37019.16'"
+    captured = capsys.readouterr()
+    assert captured.out == "1\nABMG891115PD7: Total '41000.16' is invalid, expected '37019.16'\n"
+    assert captured.err == ""
     assert ingresos is None
 
 
-def test_generar_ingresos_error2(caplog):
+def test_generar_ingresos_error2(caplog, capsys):
     caplog.set_level(logging.INFO)
-    config = ConfigManager()
     facturas = FacturasManager(ym_date)["FacturasIncorrectas2"]
     print(len(facturas))
 
     ingresos = generate_ingresos(
         clients=ClientsManager(),
         facturas=facturas,
         dp=date(year=2023, month=4, day=1),
         emisor_rfc=csd_signer.rfc
     )
 
-    assert len(caplog.records) == 1
-    assert caplog.records[0].message == "XXXNOEXISTO: client not found"
+    captured = capsys.readouterr()
+    assert captured.out == "1\nXXXNOEXISTO: client not found\n"
+    assert captured.err == ""
     assert ingresos is None
 
 
 def test_periodo_desc():
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=0) == 'MES DE ENERO DEL 2021'
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=0) is None
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=0) is None
```

### Comparing `satdigitalinvoice-3.0.1/tests/test_localdb.py` & `satdigitalinvoice-3.0.2/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.1/tests/test_main.py` & `satdigitalinvoice-3.0.2/tests/test_main.py`

 * *Files identical despite different names*

