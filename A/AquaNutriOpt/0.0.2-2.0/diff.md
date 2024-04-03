# Comparing `tmp/AquaNutriOpt-0.0.2.tar.gz` & `tmp/AquaNutriOpt-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AquaNutriOpt-0.0.2.tar", last modified: Thu Jul 20 23:52:20 2023, max compression
+gzip compressed data, was "AquaNutriOpt-2.0.tar", last modified: Wed Apr  3 12:41:15 2024, max compression
```

## Comparing `AquaNutriOpt-0.0.2.tar` & `AquaNutriOpt-2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 23:52:20.469187 AquaNutriOpt-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-20 23:52:20.431782 AquaNutriOpt-0.0.2/AquaNutriOpt/
--rw-rw-rw-   0        0        0    14547 2022-09-13 04:13:53.000000 AquaNutriOpt-0.0.2/AquaNutriOpt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 23:52:20.466188 AquaNutriOpt-0.0.2/AquaNutriOpt.egg-info/
--rw-rw-rw-   0        0        0      776 2023-07-20 23:52:19.000000 AquaNutriOpt-0.0.2/AquaNutriOpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-20 23:52:20.000000 AquaNutriOpt-0.0.2/AquaNutriOpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 23:52:19.000000 AquaNutriOpt-0.0.2/AquaNutriOpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 23:52:19.000000 AquaNutriOpt-0.0.2/AquaNutriOpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      155 2023-07-20 22:54:56.000000 AquaNutriOpt-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1068 2023-07-20 23:05:27.000000 AquaNutriOpt-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-07-20 22:56:54.000000 AquaNutriOpt-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      776 2023-07-20 23:52:20.468187 AquaNutriOpt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      660 2023-07-20 22:51:03.000000 AquaNutriOpt-0.0.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 23:52:20.470185 AquaNutriOpt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-07-20 23:40:00.000000 AquaNutriOpt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:41:15.954898 AquaNutriOpt-2.0/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:41:15.921728 AquaNutriOpt-2.0/AquaNutriOpt/
+-rw-rw-rw-   0        0        0    40057 2024-04-02 18:17:21.000000 AquaNutriOpt-2.0/AquaNutriOpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:41:15.950897 AquaNutriOpt-2.0/AquaNutriOpt.egg-info/
+-rw-rw-rw-   0        0        0      882 2024-04-03 12:41:15.000000 AquaNutriOpt-2.0/AquaNutriOpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-03 12:41:15.000000 AquaNutriOpt-2.0/AquaNutriOpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:41:15.000000 AquaNutriOpt-2.0/AquaNutriOpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 12:41:15.000000 AquaNutriOpt-2.0/AquaNutriOpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      299 2024-04-02 23:43:24.000000 AquaNutriOpt-2.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1068 2024-04-02 23:41:23.000000 AquaNutriOpt-2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-20 22:56:54.000000 AquaNutriOpt-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      882 2024-04-03 12:41:15.953899 AquaNutriOpt-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2024-04-02 23:40:24.000000 AquaNutriOpt-2.0/README.txt
+-rw-rw-rw-   0        0        0      989 2024-04-02 23:51:29.000000 AquaNutriOpt-2.0/runAquaNutriOpt.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:41:15.954898 AquaNutriOpt-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-02 23:55:40.000000 AquaNutriOpt-2.0/setup.py
```

### Comparing `AquaNutriOpt-0.0.2/LICENSE.txt` & `AquaNutriOpt-2.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2023 Ashim Khanal
+Copyright © 2024 Ashim Khanal
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `AquaNutriOpt-0.0.2/README.txt` & `AquaNutriOpt-2.0/README.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,3 +1,8 @@
 This is a python package that find the optimal location(here in terms of Nodes/Reaches) for the placement of Best Management Practices and/or Technologies to reduce Nutrient loading in the Lake Okeechobee.
 It takes two Files as input BMP_Tech.csv and Net_Data.csv. The specific format must be followed for this file which is explained in the Readme file of the foloowing github repository, https://github.com/Ashim-Khanal/AquaNutriOpt
 It returns the total loading of the nutrients(Phosphorous, Nitrogens) at the end of the network (here the lake) and also provides the placement of possible BMPs or technologies at that reach within the given total budget.
+
+AquNutriOpt v2.0 incorporates:
+a. Time Indexed Model which considers multiple timeperiods nutrient loadings and transport to provide better and robust BMPs prescription.
+b. Multi Objective Time Indexed Model where two measures Phosphorous and Nitrogen are to be minimized within provided budgets.
+
```

### Comparing `AquaNutriOpt-0.0.2/setup.py` & `AquaNutriOpt-2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name = 'AquaNutriOpt',
-    version='0.0.2',
-    description='Finds the optimal placement of BMPs and Technologies in a network in order to reduce the nutrient loadings at the lake',
+    version='2.0',
+    description='Finds the optimal placement of BMPs and Technologies in a network in order to reduce the nutrient loadings at the lake with multiple objectives taking different year nutrient loadings in consideration',
     Long_description = open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/Ashim-Khanal/AquaNutriOpt',
     author='Ashim Khanal',
     author_email = 'ashimkhanal18@gmail.com',
     license = 'MIT',
     classifiers=classifiers,
-    keywords='Optimization, Environment, Best Management Practices,Aqua, Technologies, Nutrient Load Reduction, environemnt protection',
+    keywords='Optimization, Environment, Best Management Practices, Aqua, Technologies, Nutrient Load Reduction, environemnt protection, Engineering, Environmental Modeling, Environmental Software',
     packages=find_packages(),
     install_requires=['']
 )
```

