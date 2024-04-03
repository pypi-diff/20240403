# Comparing `tmp/cfdiclient-1.5.6.tar.gz` & `tmp/cfdiclient-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdiclient-1.5.6.tar", last modified: Thu Mar 31 06:44:33 2022, max compression
+gzip compressed data, was "cfdiclient-1.5.9.tar", last modified: Wed Apr  3 05:12:28 2024, max compression
```

## Comparing `cfdiclient-1.5.6.tar` & `cfdiclient-1.5.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 06:44:33.655667 cfdiclient-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-03-31 06:44:33.655667 cfdiclient-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 06:44:33.655667 cfdiclient-1.5.6/cfdiclient/
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/autenticacion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/autenticacion.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/descargamasiva.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/descargamasiva.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/fiel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/signer.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/signer.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/solicitadescarga.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/solicitadescarga.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/validacioncfdi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/verificasolicituddescarga.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/verificasolicituddescarga.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/cfdiclient/webservicerequest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 06:44:33.655667 cfdiclient-1.5.6/cfdiclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-03-31 06:44:33.000000 cfdiclient-1.5.6/cfdiclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-03-31 06:44:33.000000 cfdiclient-1.5.6/cfdiclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 06:44:33.000000 cfdiclient-1.5.6/cfdiclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-31 06:44:33.000000 cfdiclient-1.5.6/cfdiclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-03-31 06:44:33.000000 cfdiclient-1.5.6/cfdiclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-03-31 06:44:33.659667 cfdiclient-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 06:44:33.655667 cfdiclient-1.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-03-31 06:43:34.000000 cfdiclient-1.5.6/tests/test_cfdiclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:28.769386 cfdiclient-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-03 05:12:28.769386 cfdiclient-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:28.765386 cfdiclient-1.5.9/cfdiclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/autenticacion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/autenticacion.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/descargamasiva.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/descargamasiva.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/fiel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/signer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/solicitadescarga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/solicitadescarga.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/validacioncfdi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/verificasolicituddescarga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/verificasolicituddescarga.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/cfdiclient/webservicerequest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:28.769386 cfdiclient-1.5.9/cfdiclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-03 05:12:28.000000 cfdiclient-1.5.9/cfdiclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-03 05:12:28.000000 cfdiclient-1.5.9/cfdiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:12:28.000000 cfdiclient-1.5.9/cfdiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 05:12:28.000000 cfdiclient-1.5.9/cfdiclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 05:12:28.000000 cfdiclient-1.5.9/cfdiclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 05:12:28.769386 cfdiclient-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:28.769386 cfdiclient-1.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 05:12:04.000000 cfdiclient-1.5.9/tests/test_cfdiclient.py
```

### Comparing `cfdiclient-1.5.6/LICENSE` & `cfdiclient-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/PKG-INFO` & `cfdiclient-1.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: cfdiclient
-Version: 1.5.6
+Version: 1.5.9
 Summary: Cliente Python Web Service del SAT para la descarga masiva de CFDIs
 Home-page: https://github.com/luisiturrios1/python-cfdiclient
 Author: Luis Iturrios
 Author-email: luisiturrios1@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml>=4.2.5
+Requires-Dist: requests>=2.21.0
+Requires-Dist: pycryptodome>=3.7.2
+Requires-Dist: pyOpenSSL>=18.0.0
 
 # python-cfdiclient
 
 Cliente Python Web Service del SAT para la descarga masiva de xml
 
 ## Consulta y recuperación de comprobantes (Nuevo)
 
@@ -246,9 +248,7 @@
 uuid = '0XXX0X00-000-0XX0-XX0X-000X0X0XXX00'
 
 estado = validacion.obtener_estado(rfc_emisor, rfc_receptor, total, uuid)
 
 print(estado)
 # {'codigo_estatus': 'S - Comprobante obtenido satisfactoriamente.', 'es_cancelable': 'Cancelable con aceptación', 'estado': 'Vigente'}
 ```
-
-
```

### Comparing `cfdiclient-1.5.6/README.md` & `cfdiclient-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/autenticacion.py` & `cfdiclient-1.5.9/cfdiclient/autenticacion.py`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/autenticacion.xml` & `cfdiclient-1.5.9/cfdiclient/autenticacion.xml`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/descargamasiva.py` & `cfdiclient-1.5.9/cfdiclient/descargamasiva.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     soap_action = 'http://DescargaMasivaTerceros.sat.gob.mx/IDescargaMasivaTercerosService/Descargar'
     solicitud_xpath = 's:Body/des:PeticionDescargaMasivaTercerosEntrada/des:peticionDescarga'
     result_xpath = 's:Body/RespuestaDescargaMasivaTercerosSalida/Paquete'
 
     def descargar_paquete(self, token, rfc_solicitante, id_paquete):
 
         arguments = {
-            'RfcSolicitante': rfc_solicitante,
+            'RfcSolicitante': rfc_solicitante.upper(),
             'IdPaquete': id_paquete,
         }
 
         element_response = self.request(token, arguments)
 
         respuesta = element_response.getparent().getparent().getparent().find(
             's:Header/h:respuesta', namespaces=self.external_nsmap
```

### Comparing `cfdiclient-1.5.6/cfdiclient/fiel.py` & `cfdiclient-1.5.9/cfdiclient/fiel.py`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/signer.py` & `cfdiclient-1.5.9/cfdiclient/signer.py`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/signer.xml` & `cfdiclient-1.5.9/cfdiclient/signer.xml`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/solicitadescarga.py` & `cfdiclient-1.5.9/cfdiclient/solicitadescarga.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,35 @@
     soap_action = 'http://DescargaMasivaTerceros.sat.gob.mx/ISolicitaDescargaService/SolicitaDescarga'
     solicitud_xpath = 's:Body/des:SolicitaDescarga/des:solicitud'
     result_xpath = 's:Body/SolicitaDescargaResponse/SolicitaDescargaResult'
 
     def solicitar_descarga(
         self, token, rfc_solicitante, fecha_inicial, fecha_final,
         rfc_emisor=None, rfc_receptor=None, tipo_solicitud='CFDI',
-        tipo_comprobante=None, estado_comprobante=None, 
+        tipo_comprobante=None, estado_comprobante=None,
         rfc_a_cuenta_terceros=None, complemento=None, uuid=None
     ):
 
         arguments = {
-            'RfcSolicitante': rfc_solicitante,
+            'RfcSolicitante': rfc_solicitante.upper(),
             'FechaFinal': fecha_final.strftime(self.DATE_TIME_FORMAT),
             'FechaInicial': fecha_inicial.strftime(self.DATE_TIME_FORMAT),
             'TipoSolicitud': tipo_solicitud,
             'TipoComprobante': tipo_comprobante,
             'EstadoComprobante': estado_comprobante,
             'RfcACuentaTerceros': rfc_a_cuenta_terceros,
             'Complemento': complemento,
             'UUID': uuid,
         }
 
         if rfc_emisor:
-            arguments['RfcEmisor'] = rfc_emisor
+            arguments['RfcEmisor'] = rfc_emisor.upper()
 
         if rfc_receptor:
-            arguments['RfcReceptores'] = [rfc_receptor]
+            arguments['RfcReceptores'] = [rfc_receptor.upper()]
 
         element_response = self.request(token, arguments)
 
         ret_val = {
             'id_solicitud': element_response.get('IdSolicitud'),
             'cod_estatus': element_response.get('CodEstatus'),
             'mensaje': element_response.get('Mensaje')
```

### Comparing `cfdiclient-1.5.6/cfdiclient/utils.py` & `cfdiclient-1.5.9/cfdiclient/utils.py`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/validacioncfdi.py` & `cfdiclient-1.5.9/cfdiclient/validacioncfdi.py`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient/verificasolicituddescarga.py` & `cfdiclient-1.5.9/cfdiclient/verificasolicituddescarga.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     soap_action = 'http://DescargaMasivaTerceros.sat.gob.mx/IVerificaSolicitudDescargaService/VerificaSolicitudDescarga'
     solicitud_xpath = 's:Body/des:VerificaSolicitudDescarga/des:solicitud'
     result_xpath = 's:Body/VerificaSolicitudDescargaResponse/VerificaSolicitudDescargaResult'
 
     def verificar_descarga(self, token, rfc_solicitante, id_solicitud):
 
         arguments = {
-            'RfcSolicitante': rfc_solicitante,
+            'RfcSolicitante': rfc_solicitante.upper(),
             'IdSolicitud': id_solicitud,
         }
 
         element_response = self.request(token, arguments)
 
         ret_val = {
             'cod_estatus': element_response.get('CodEstatus'),
```

### Comparing `cfdiclient-1.5.6/cfdiclient/webservicerequest.py` & `cfdiclient-1.5.9/cfdiclient/webservicerequest.py`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/cfdiclient.egg-info/PKG-INFO` & `cfdiclient-1.5.9/cfdiclient.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: cfdiclient
-Version: 1.5.6
+Version: 1.5.9
 Summary: Cliente Python Web Service del SAT para la descarga masiva de CFDIs
 Home-page: https://github.com/luisiturrios1/python-cfdiclient
 Author: Luis Iturrios
 Author-email: luisiturrios1@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml>=4.2.5
+Requires-Dist: requests>=2.21.0
+Requires-Dist: pycryptodome>=3.7.2
+Requires-Dist: pyOpenSSL>=18.0.0
 
 # python-cfdiclient
 
 Cliente Python Web Service del SAT para la descarga masiva de xml
 
 ## Consulta y recuperación de comprobantes (Nuevo)
 
@@ -246,9 +248,7 @@
 uuid = '0XXX0X00-000-0XX0-XX0X-000X0X0XXX00'
 
 estado = validacion.obtener_estado(rfc_emisor, rfc_receptor, total, uuid)
 
 print(estado)
 # {'codigo_estatus': 'S - Comprobante obtenido satisfactoriamente.', 'es_cancelable': 'Cancelable con aceptación', 'estado': 'Vigente'}
 ```
-
-
```

### Comparing `cfdiclient-1.5.6/cfdiclient.egg-info/SOURCES.txt` & `cfdiclient-1.5.9/cfdiclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfdiclient-1.5.6/setup.py` & `cfdiclient-1.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cfdiclient',
-    version='1.5.6',
+    version='1.5.9',
     author='Luis Iturrios',
     author_email='luisiturrios1@gmail.com',
     description='Cliente Python Web Service del SAT para la descarga masiva de CFDIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/luisiturrios1/python-cfdiclient',
     packages=setuptools.find_packages(),
```

