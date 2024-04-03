# Comparing `tmp/amit_hvac_control-0.3.1.tar.gz` & `tmp/amit_hvac_control-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amit_hvac_control-0.3.1.tar", last modified: Sun Mar 31 07:16:41 2024, max compression
+gzip compressed data, was "amit_hvac_control-0.3.2.tar", last modified: Wed Apr  3 18:49:04 2024, max compression
```

## Comparing `amit_hvac_control-0.3.1.tar` & `amit_hvac_control-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-03-31 07:16:41.751442 amit_hvac_control-0.3.1/
--rw-r--r--   0 mitchdries   (501) staff       (20)     1068 2024-03-01 21:43:32.000000 amit_hvac_control-0.3.1/LICENSE
--rw-r--r--   0 mitchdries   (501) staff       (20)      923 2024-03-31 07:16:41.750717 amit_hvac_control-0.3.1/PKG-INFO
--rw-r--r--   0 mitchdries   (501) staff       (20)      610 2024-03-31 07:11:33.000000 amit_hvac_control-0.3.1/README.md
--rw-r--r--   0 mitchdries   (501) staff       (20)      391 2024-03-29 07:26:08.000000 amit_hvac_control-0.3.1/pyproject.toml
--rw-r--r--   0 mitchdries   (501) staff       (20)       38 2024-03-31 07:16:41.751619 amit_hvac_control-0.3.1/setup.cfg
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-03-31 07:16:41.737750 amit_hvac_control-0.3.1/src/
--rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-03-22 12:57:51.000000 amit_hvac_control-0.3.1/src/__init__.py
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-03-31 07:16:41.740582 amit_hvac_control-0.3.1/src/amit_hvac_control/
--rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-03-05 12:01:36.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/__init__.py
--rw-r--r--   0 mitchdries   (501) staff       (20)      909 2024-03-31 06:57:11.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/__main__.py
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-03-31 07:16:41.747050 amit_hvac_control-0.3.1/src/amit_hvac_control/api/
--rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-03-06 19:54:50.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/api/__init__.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     2298 2024-03-22 15:32:57.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/api/status.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     2806 2024-03-25 18:28:25.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/api/temperature.py
--rw-r--r--   0 mitchdries   (501) staff       (20)      377 2024-03-06 20:01:06.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/api/utils.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     5227 2024-03-29 07:25:54.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/api/ventilation.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     2121 2024-03-22 13:23:38.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/client.py
--rw-r--r--   0 mitchdries   (501) staff       (20)     1307 2024-03-05 11:41:14.000000 amit_hvac_control-0.3.1/src/amit_hvac_control/models.py
-drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-03-31 07:16:41.748818 amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/
--rw-r--r--   0 mitchdries   (501) staff       (20)      923 2024-03-31 07:16:41.000000 amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/PKG-INFO
--rw-r--r--   0 mitchdries   (501) staff       (20)      595 2024-03-31 07:16:41.000000 amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/SOURCES.txt
--rw-r--r--   0 mitchdries   (501) staff       (20)        1 2024-03-31 07:16:41.000000 amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/dependency_links.txt
--rw-r--r--   0 mitchdries   (501) staff       (20)       29 2024-03-31 07:16:41.000000 amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/requires.txt
--rw-r--r--   0 mitchdries   (501) staff       (20)       27 2024-03-31 07:16:41.000000 amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/top_level.txt
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.646937 amit_hvac_control-0.3.2/
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1068 2024-03-01 21:43:32.000000 amit_hvac_control-0.3.2/LICENSE
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1064 2024-04-03 18:49:04.646020 amit_hvac_control-0.3.2/PKG-INFO
+-rw-r--r--   0 mitchdries   (501) staff       (20)      610 2024-03-31 07:11:33.000000 amit_hvac_control-0.3.2/README.md
+-rw-r--r--   0 mitchdries   (501) staff       (20)      528 2024-04-03 18:41:33.000000 amit_hvac_control-0.3.2/pyproject.toml
+-rw-r--r--   0 mitchdries   (501) staff       (20)       38 2024-04-03 18:49:04.647515 amit_hvac_control-0.3.2/setup.cfg
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.635863 amit_hvac_control-0.3.2/src/
+-rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:01.000000 amit_hvac_control-0.3.2/src/__init__.py
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.637381 amit_hvac_control-0.3.2/src/amit_hvac_control/
+-rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/__init__.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)      909 2024-04-03 18:42:39.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/__main__.py
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.643958 amit_hvac_control-0.3.2/src/amit_hvac_control/api/
+-rw-r--r--   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:44:06.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/__init__.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     2610 2024-04-03 18:48:32.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/status.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     2806 2024-03-25 18:28:25.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/temperature.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)      377 2024-03-06 20:01:06.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/utils.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     5227 2024-03-29 07:25:54.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/api/ventilation.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     2121 2024-03-22 13:23:38.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/client.py
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1307 2024-03-05 11:41:14.000000 amit_hvac_control-0.3.2/src/amit_hvac_control/models.py
+drwxr-xr-x   0 mitchdries   (501) staff       (20)        0 2024-04-03 18:49:04.644953 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/
+-rw-r--r--   0 mitchdries   (501) staff       (20)     1064 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/PKG-INFO
+-rw-r--r--   0 mitchdries   (501) staff       (20)      595 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/SOURCES.txt
+-rw-r--r--   0 mitchdries   (501) staff       (20)        1 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/dependency_links.txt
+-rw-r--r--   0 mitchdries   (501) staff       (20)       29 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/requires.txt
+-rw-r--r--   0 mitchdries   (501) staff       (20)       27 2024-04-03 18:49:04.000000 amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/top_level.txt
```

### Comparing `amit_hvac_control-0.3.1/LICENSE` & `amit_hvac_control-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/PKG-INFO` & `amit_hvac_control-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: amit_hvac_control
-Version: 0.3.1
+Version: 0.3.2
 Summary: Amit HVAC control
 Author-email: Mitch Dries <mitch.dries@gmail.com>
+Project-URL: Homepage, https://github.com/mitch3s/amit-hvac-control
+Project-URL: Issues, https://github.com/mitch3s/amit-hvac-control/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: asyncio
 Requires-Dist: aiohttp
```

### Comparing `amit_hvac_control-0.3.1/README.md` & `amit_hvac_control-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control/__main__.py` & `amit_hvac_control-0.3.2/src/amit_hvac_control/__main__.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control/api/status.py` & `amit_hvac_control-0.3.2/src/amit_hvac_control/api/status.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 MAIN_URL = "/pages/index.hta"
 
 
 class DataResult:
     def __init__(
         self,
         temperature: float,
+        air_temperature: float,
         co_2: int,
         ventilation_mode: VentilationMode,
         season: Season,
         heating_mode: HeatingMode,
     ):
         self.temperature = temperature
+        self.air_temperature = air_temperature
         self.co_2 = co_2
         self.ventilation_mode = ventilation_mode
         self.season = season
         self.heating_mode = heating_mode
 
     def __str__(self):
         return f"""
-Temp:   {self.temperature}
-CO2:    {self.co_2}
+Air temperature:    {self.temperature}
+Room temperature:   {self.air_temperature}
+CO2:                {self.co_2}
 Ventilation:    {self.ventilation_mode.name}
 Comfort mode:   {self.heating_mode.name}
 Season:         {self.season.name}
 """
 
 
 class StatusApi:
@@ -43,24 +46,27 @@
         async with self.session.get(MAIN_URL) as response:
             text = await response.text()
             return self._extract_overview_details(text)
 
     def _extract_overview_details(self, content: str):
         soup = BeautifulSoup(content, "html.parser")
 
-        temp_el = soup.find(class_="AWNumericView1")
+        room_temp_el = soup.find(class_="AWNumericView1")
+        air_room_temp_el = soup.find(class_="AWNumericView3")
         [co2_el] = soup.select(".AWNumericView2,.AWNumericView2-alert-max")
 
         labels = self._get_aws_case_labels(content)
 
-        temp_val = float(temp_el.text)
+        temp_val = float(room_temp_el.text)
+        air_temp_val = float(air_room_temp_el.text)
         co2_val = int(co2_el.text)
 
         return DataResult(
             temperature=temp_val,
+            air_temperature=air_temp_val,
             co_2=co2_val,
             ventilation_mode=labels["ventilation"],
             season=labels["season"],
             heating_mode=labels["heating"],
         )
 
     def _get_aws_case_labels(self, contents: str):
```

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control/api/temperature.py` & `amit_hvac_control-0.3.2/src/amit_hvac_control/api/temperature.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control/api/ventilation.py` & `amit_hvac_control-0.3.2/src/amit_hvac_control/api/ventilation.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control/client.py` & `amit_hvac_control-0.3.2/src/amit_hvac_control/client.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control/models.py` & `amit_hvac_control-0.3.2/src/amit_hvac_control/models.py`

 * *Files identical despite different names*

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/PKG-INFO` & `amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: amit_hvac_control
-Version: 0.3.1
+Version: 0.3.2
 Summary: Amit HVAC control
 Author-email: Mitch Dries <mitch.dries@gmail.com>
+Project-URL: Homepage, https://github.com/mitch3s/amit-hvac-control
+Project-URL: Issues, https://github.com/mitch3s/amit-hvac-control/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: asyncio
 Requires-Dist: aiohttp
```

### Comparing `amit_hvac_control-0.3.1/src/amit_hvac_control.egg-info/SOURCES.txt` & `amit_hvac_control-0.3.2/src/amit_hvac_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

