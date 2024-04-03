# Comparing `tmp/inpython_package-1.0.6-py3-none-any.whl.zip` & `tmp/inpython_package-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 4225 bytes, number of entries: 9
+Zip file size: 4782 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat       47 b- defN 23-Jul-14 10:00 inpython/__init__.py
 -rw-rw-rw-  2.0 fat       30 b- defN 23-Jul-14 10:01 inpython/__main__.py
--rw-rw-rw-  2.0 fat      162 b- defN 23-Jul-14 14:27 inpython/ingraph/__init__.py
--rw-rw-rw-  2.0 fat     2038 b- defN 23-Oct-04 09:27 inpython/ingraph/ingraph.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Oct-04 09:28 inpython_package-1.0.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1106 b- defN 23-Oct-04 09:28 inpython_package-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-04 09:28 inpython_package-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Oct-04 09:28 inpython_package-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      752 b- defN 23-Oct-04 09:28 inpython_package-1.0.6.dist-info/RECORD
-9 files, 5328 bytes uncompressed, 2913 bytes compressed:  45.3%
+-rw-rw-rw-  2.0 fat      160 b- defN 23-Oct-30 11:13 inpython/aotools/__init__.py
+-rw-rw-rw-  2.0 fat       33 b- defN 23-Oct-30 11:15 inpython/aotools/aogeo.py
+-rw-rw-rw-  2.0 fat      162 b- defN 24-Mar-20 08:28 inpython/ingraph/__init__.py
+-rw-rw-rw-  2.0 fat     2029 b- defN 24-Apr-03 10:08 inpython/ingraph/ingraph.py
+-rw-rw-rw-  2.0 fat     1092 b- defN 24-Apr-03 10:14 inpython_package-1.0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1277 b- defN 24-Apr-03 10:14 inpython_package-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 10:14 inpython_package-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-03 10:14 inpython_package-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      916 b- defN 24-Apr-03 10:14 inpython_package-1.0.7.dist-info/RECORD
+11 files, 5847 bytes uncompressed, 3212 bytes compressed:  45.1%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: inpython/__init__.py
 Comment: 
 
 Filename: inpython/__main__.py
 Comment: 
 
+Filename: inpython/aotools/__init__.py
+Comment: 
+
+Filename: inpython/aotools/aogeo.py
+Comment: 
+
 Filename: inpython/ingraph/__init__.py
 Comment: 
 
 Filename: inpython/ingraph/ingraph.py
 Comment: 
 
-Filename: inpython_package-1.0.6.dist-info/LICENSE.txt
+Filename: inpython_package-1.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: inpython_package-1.0.6.dist-info/METADATA
+Filename: inpython_package-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: inpython_package-1.0.6.dist-info/WHEEL
+Filename: inpython_package-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: inpython_package-1.0.6.dist-info/top_level.txt
+Filename: inpython_package-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: inpython_package-1.0.6.dist-info/RECORD
+Filename: inpython_package-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inpython/ingraph/ingraph.py

```diff
@@ -42,12 +42,12 @@
             authority=config["authority"],
             client_credential={"thumbprint": config["thumbprint"],
                                "private_key": privatekey},
             )
         # try to get a token
         result = msal_app.acquire_token_for_client(scopes=config["scope"])
         result = json.dumps(result)
+        return result
     except:
         # toute exception issue de la séquence try arrive ici et est remontée à l'appelant 'uvpython'  
         raise  # pour que l'appelant reçoive l'exception
-    finally:
-        return result
+
```

## Comparing `inpython_package-1.0.6.dist-info/LICENSE.txt` & `inpython_package-1.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `inpython_package-1.0.6.dist-info/METADATA` & `inpython_package-1.0.7.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: inpython-package
-Version: 1.0.6
+Version: 1.0.7
 Summary: # Infodata's IN-Tools U2Python Package
 Home-page: https://bitbucket.org/infodata-dev/inpython
 Author: infodata
 Author-email: efv@infodata.lu
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: msal >=1.22
 
 # README #
 
-ce projet 'inpython-package' rassemble tous les packages et modules python exploitÃ©s par Integrix .
+Ce projet **inpython-package** rassemble tous les packages et modules python exploitÃ©s par Integrix .
 
-# inpython.ingarph
-package pour la gestion avec MS-Graph.
+# sub-package **inpython.ingraph**
+package pour la gestion avec MS-Graph en exploitant le module 'msal' (Microsoft Authentication Library).
 
 ### How do I get set up? ###
 
-* les bases de u2Python c.f. [wiki sys/proc/install u2ptyhon](https://wiki.infodata.lu/sys/proc/install_u2python)
+* Les bases de u2Python c.f. [wiki sys/proc/install u2Python](https://wiki.infodata.lu/sys/proc/install_u2python)
 * [U2Python par RocketSoftware](https://docs.rocketsoftware.com/bundle/UniVerse_PythonUserGuide_V1134/resource/UniVerse_PythonUserGuide_V1134.pdf)
-* vÃ©rifier la version de u2Python, au TCL uv 
+* VÃ©rifier la version de u2Python, au TCL uv 
 ```python
 >python 
 import sys
-sys.version  # ->>  '3.4.1 (default, Feb 18 2015, 13:36:51) \n[GCC 4.4.7 20120313 (Red Hat 4.4.7-3)]'
+print(sys.version)
+print(sys.executable) # -> 'C:\\U2\\UV\\BIN\\uv.exe' uvbin !!
+print('\n'.join(sys.path)) # les path en cours
 exit()
 ```
 
 ### Install inPackages into U2python 
-`pip install inpython-package`
+- `pip3 install inpython-package`
 
+### Manage Package 
+- c.f. [devREADME](devREADME.md)
```

## Comparing `inpython_package-1.0.6.dist-info/RECORD` & `inpython_package-1.0.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 inpython/__init__.py,sha256=ZZMTm5QeMRlmewa5jmhBldUYnLX-ZbLxLut_PyXHFmw,47
 inpython/__main__.py,sha256=_WTI7FZVtIi59VDIyBe4IL0mii4TWinjfmPNxNc7Fy0,30
+inpython/aotools/__init__.py,sha256=394QRN-l_cGTB2KGZCGbid1Xpn5wZiNTNsacE7cuDus,160
+inpython/aotools/aogeo.py,sha256=ViZoeUgpNTeelAPzoLZRqGh9INoe5dOER4XWFpDds80,33
 inpython/ingraph/__init__.py,sha256=FMGklQI9h9OL3qvXadTPja-WUZkS5ugdzZCNQhtuKq0,162
-inpython/ingraph/ingraph.py,sha256=9FlgpeLvLw6LhJl9i_o1ymfMkSgqv3pn0WgvrANAfVQ,2038
-inpython_package-1.0.6.dist-info/LICENSE.txt,sha256=IirBHVsB--MNPRVyUzq8A99ot9-F-IiAW2t2auIxJDA,1092
-inpython_package-1.0.6.dist-info/METADATA,sha256=uJDk4asLE8I8CscQPfrO3yyBaJVP54ND9HT0YDYzitM,1106
-inpython_package-1.0.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-inpython_package-1.0.6.dist-info/top_level.txt,sha256=cY6uggTAnozInE_EbHweIn8VjImvJcHc1w9WK4kYmXI,9
-inpython_package-1.0.6.dist-info/RECORD,,
+inpython/ingraph/ingraph.py,sha256=uUomSwnLwJ18Altqxnbb--Zpvyspw20KGXSZVCovPMk,2029
+inpython_package-1.0.7.dist-info/LICENSE.txt,sha256=IirBHVsB--MNPRVyUzq8A99ot9-F-IiAW2t2auIxJDA,1092
+inpython_package-1.0.7.dist-info/METADATA,sha256=PiQFwMJkd7htM-MCce0pIXhM_806x56YhXVGhN2C7OE,1277
+inpython_package-1.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+inpython_package-1.0.7.dist-info/top_level.txt,sha256=cY6uggTAnozInE_EbHweIn8VjImvJcHc1w9WK4kYmXI,9
+inpython_package-1.0.7.dist-info/RECORD,,
```

