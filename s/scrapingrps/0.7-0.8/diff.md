# Comparing `tmp/scrapingrps-0.7.tar.gz` & `tmp/scrapingrps-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapingrps-0.7.tar", last modified: Tue Mar  5 16:32:55 2024, max compression
+gzip compressed data, was "scrapingrps-0.8.tar", last modified: Wed Apr  3 12:32:07 2024, max compression
```

## Comparing `scrapingrps-0.7.tar` & `scrapingrps-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 16:32:55.231959 scrapingrps-0.7/
--rw-rw-rw-   0        0        0      577 2024-03-05 16:32:55.226022 scrapingrps-0.7/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-01-04 13:05:23.000000 scrapingrps-0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-05 16:32:55.175168 scrapingrps-0.7/scrapingrps/
--rw-rw-rw-   0        0        0      308 2024-01-10 13:11:52.000000 scrapingrps-0.7/scrapingrps/__init__.py
--rw-rw-rw-   0        0        0    25640 2024-03-05 16:24:16.000000 scrapingrps-0.7/scrapingrps/scrapingrps.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:32:55.220962 scrapingrps-0.7/scrapingrps.egg-info/
--rw-rw-rw-   0        0        0      577 2024-03-05 16:32:54.000000 scrapingrps-0.7/scrapingrps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-03-05 16:32:54.000000 scrapingrps-0.7/scrapingrps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 16:32:54.000000 scrapingrps-0.7/scrapingrps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-05 16:32:54.000000 scrapingrps-0.7/scrapingrps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-05 16:32:54.000000 scrapingrps-0.7/scrapingrps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-05 16:32:55.232959 scrapingrps-0.7/setup.cfg
--rw-rw-rw-   0        0        0      738 2024-03-05 16:31:00.000000 scrapingrps-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:32:07.538418 scrapingrps-0.8/
+-rw-rw-rw-   0        0        0      577 2024-04-03 12:32:07.532062 scrapingrps-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-01-04 13:05:23.000000 scrapingrps-0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 12:32:07.460845 scrapingrps-0.8/scrapingrps/
+-rw-rw-rw-   0        0        0      308 2024-01-10 13:11:52.000000 scrapingrps-0.8/scrapingrps/__init__.py
+-rw-rw-rw-   0        0        0    25653 2024-04-03 12:28:54.000000 scrapingrps-0.8/scrapingrps/scrapingrps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:32:07.521151 scrapingrps-0.8/scrapingrps.egg-info/
+-rw-rw-rw-   0        0        0      577 2024-04-03 12:32:06.000000 scrapingrps-0.8/scrapingrps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-03 12:32:06.000000 scrapingrps-0.8/scrapingrps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:32:06.000000 scrapingrps-0.8/scrapingrps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-03 12:32:06.000000 scrapingrps-0.8/scrapingrps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 12:32:06.000000 scrapingrps-0.8/scrapingrps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:32:07.539422 scrapingrps-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      738 2024-04-03 12:28:54.000000 scrapingrps-0.8/setup.py
```

### Comparing `scrapingrps-0.7/PKG-INFO` & `scrapingrps-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapingrps
-Version: 0.7
+Version: 0.8
 Summary: Scraping interno
 Home-page: https://github.com/rafaelpsampaio/scrapingrps
 Author: Rafael Perroud Sampaio
 Author-email: rafapsampaio@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrapingrps-0.7/scrapingrps/scrapingrps.py` & `scrapingrps-0.8/scrapingrps/scrapingrps.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
                 if codigo_int != str(codigo):
                     print('Esquisito')
                     print(codigo)
                     print(codigo_int)
                     travou = 1
                 else:
                     try:
-                        botaojs(aba,"#root > arsenal-loader > div > div > div.sc-heIBml.dECqlF > soma-grid > soma-grid-row:nth-child(5) > soma-grid-col > soma-coachmark > soma-coachmark-highlight > soma-card > div.sc-lnPyaJ.dwtKZE > div.sc-kqGoIF.dgPowr > soma-button.sc-eBHhsj.boPyWa.soma-button.primary.sm.hydrated').shadowRoot.querySelector('button')")
-                        botaojs(aba,"#root > arsenal-loader > div > div > div.sc-heIBml.dECqlF > soma-grid > soma-grid-row:nth-child(5) > soma-grid-col > soma-coachmark > soma-coachmark-highlight > soma-card > div.sc-lnPyaJ.dwtKZE > div.sc-kqGoIF.dgPowr > div.sc-eyvILC.SVORC > soma-modal > div > div.sc-kWtpeL.lcfPlf > div > soma-button').shadowRoot.querySelector('button')")
+                        botaojs(aba,"#root > arsenal-loader > div > div > div.sc-ghzrUh.crcVtA > soma-grid > soma-grid-row:nth-child(5) > soma-grid-col > soma-coachmark > soma-coachmark-highlight > soma-card > div.sc-kqGoIF.cbzSzt > div.sc-knuQbY.ebfBRI > soma-button.sc-dExYaf.jacaKP.soma-button.primary.sm.hydrated').shadowRoot.querySelector('button')")
+                        botaojs(aba,"#root > arsenal-loader > div > div > div.sc-ghzrUh.crcVtA > soma-grid > soma-grid-row:nth-child(5) > soma-grid-col > soma-coachmark > soma-coachmark-highlight > soma-card > div.sc-kqGoIF.cbzSzt > div.sc-knuQbY.ebfBRI > div.sc-dBmzty.bBplVm > soma-modal > div > div.sc-bDpDS.goxwLD > div > soma-button:nth-child(2)').shadowRoot.querySelector('button')")
                     except:
                         print('Erro botões')
                         travou = 1
             if travou == 0:
                 travou = 1
                 filename_loc = f"XPerformance - {codigo_int}"
                 for t in range(0,tempowait_download):
```

### Comparing `scrapingrps-0.7/scrapingrps.egg-info/PKG-INFO` & `scrapingrps-0.8/scrapingrps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapingrps
-Version: 0.7
+Version: 0.8
 Summary: Scraping interno
 Home-page: https://github.com/rafaelpsampaio/scrapingrps
 Author: Rafael Perroud Sampaio
 Author-email: rafapsampaio@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrapingrps-0.7/setup.py` & `scrapingrps-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scrapingrps',
-    version='0.7',
+    version='0.8',
     author='Rafael Perroud Sampaio',
     author_email='rafapsampaio@gmail.com',
     description='Scraping interno',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rafaelpsampaio/scrapingrps',
     packages=find_packages(),
```

