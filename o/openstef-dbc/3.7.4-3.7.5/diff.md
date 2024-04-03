# Comparing `tmp/openstef_dbc-3.7.4.tar.gz` & `tmp/openstef_dbc-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.7.4.tar", last modified: Wed Mar 13 13:38:06 2024, max compression
+gzip compressed data, was "openstef_dbc-3.7.5.tar", last modified: Wed Apr  3 14:15:51 2024, max compression
```

## Comparing `openstef_dbc-3.7.4.tar` & `openstef_dbc-3.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:38:06.944087 openstef_dbc-3.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-13 13:38:06.944087 openstef_dbc-3.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:38:06.940087 openstef_dbc-3.7.4/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:38:06.940087 openstef_dbc-3.7.4/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:38:06.940087 openstef_dbc-3.7.4/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:38:06.940087 openstef_dbc-3.7.4/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:38:06.940087 openstef_dbc-3.7.4/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-13 13:38:06.000000 openstef_dbc-3.7.4/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-13 13:38:06.000000 openstef_dbc-3.7.4/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:38:06.000000 openstef_dbc-3.7.4/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-13 13:38:06.000000 openstef_dbc-3.7.4/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 13:38:06.000000 openstef_dbc-3.7.4/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-13 13:38:06.944087 openstef_dbc-3.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-13 13:37:57.000000 openstef_dbc-3.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:15:51.293472 openstef_dbc-3.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-03 14:15:51.293472 openstef_dbc-3.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:15:51.289472 openstef_dbc-3.7.5/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:15:51.289472 openstef_dbc-3.7.5/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:15:51.289472 openstef_dbc-3.7.5/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:15:51.293472 openstef_dbc-3.7.5/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:15:51.293472 openstef_dbc-3.7.5/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-03 14:15:51.000000 openstef_dbc-3.7.5/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 14:15:51.000000 openstef_dbc-3.7.5/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:15:51.000000 openstef_dbc-3.7.5/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 14:15:51.000000 openstef_dbc-3.7.5/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:15:51.000000 openstef_dbc-3.7.5/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 14:15:51.293472 openstef_dbc-3.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-03 14:15:37.000000 openstef_dbc-3.7.5/setup.py
```

### Comparing `openstef_dbc-3.7.4/LICENSE` & `openstef_dbc-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/PKG-INFO` & `openstef_dbc-3.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.7.4
+Version: 3.7.5
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,20 +18,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ciso8601~=2.3.0
 Requires-Dist: geopy~=2.3.0
 Requires-Dist: openstef~=3.4.4
 Requires-Dist: pydantic-settings~=2.1.0
 Requires-Dist: influxdb-client~=1.36.1
-Requires-Dist: mysql-connector-python~=8.0.31
-Requires-Dist: pandas==2.1.3
+Requires-Dist: mysql-connector-python~=8.3.0
 Requires-Dist: PyMySQL~=1.0.2
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.28.1
-Requires-Dist: SQLAlchemy~=1.4.46
+Requires-Dist: SQLAlchemy~=2.0.21
 
 <!--
 SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com>
 
 SPDX-License-Identifier: MPL-2.0
 -->
 [![Python Build](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml/badge.svg?branch=master)](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml)
```

### Comparing `openstef_dbc-3.7.4/README.md` & `openstef_dbc-3.7.5/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/__init__.py` & `openstef_dbc-3.7.5/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/data_interface.py` & `openstef_dbc-3.7.5/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/database.py` & `openstef_dbc-3.7.5/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/ktp_api.py` & `openstef_dbc-3.7.5/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/log/logging.py` & `openstef_dbc-3.7.5/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/log/processors.py` & `openstef_dbc-3.7.5/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/models/measurement.py` & `openstef_dbc-3.7.5/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/ems.py` & `openstef_dbc-3.7.5/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/model_input.py` & `openstef_dbc-3.7.5/openstef_dbc/services/model_input.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,27 +21,29 @@
     def __init__(self) -> None:
         self.logger = structlog.get_logger(self.__class__.__name__)
 
     def get_model_input(
         self,
         pid: int = 295,
         location: Union[Tuple[int, int], str] = "Arnhem",
+        country: str = "NL",
         datetime_start: str = None,
         datetime_end: str = None,
         forecast_resolution: str = "15min",
     ) -> pd.DataFrame:
         """Get model input.
 
         Get load and predictors for given pid and datetime range. If the forecast_resolution
         is lower than the data resolution, the price data is filled, while the weather
         and load data is interpolated.
 
         Args:
             pid (int, optional): Prediction job id. Defaults to 295.
             location (str, optional): Location name or tuple with lat, lon. Defaults to "Arnhem".
+            country (str, optional): Country of were the location is located. Defaults to "NL", The Netherlands.
             datetime_start (datetime, optional): Start datetime. Defaults to None.
             datetime_end (datetime, optional): End datetime. Defaults to None.
             forecast_resolution (str, optional): Time resolution of model input
                 (see pandas Date Offset frequency strings). Defaults to "15min".
 
         Returns:
             pd.DataFrame: Model input.
@@ -100,27 +102,29 @@
         location: Union[Tuple[float, float], str],
         forecast_horizon: int,
         forecast_resolution: int,
         radius: float = 0.0,
         history: int = 14,
         datetime_start: datetime = None,
         sid: str = None,
+        country: str = "NL",
     ) -> pd.DataFrame:
         """This function retrieves the radiation and cloud forecast for the nearest weather location
         and the relevant pvdata from a specific system or region.
         It interpolates these values according to the forecast resolution.
         Parameters:
             - engine: database connection
             - location: lat/lon values [float] or input city [str] of turbine location
             - radius: 'None' when using a specific system, range in kms when using a region
             - history: days of historic weather and pvdata used, default 14
             - forecastHorizon: length of forecast in minutes [int]
             - forecastResolution: time resolution of forecast in minutes [int]
             - datetime_start: datetime of forecast
             - source: preferred weather source as a string, default for wind is DSN
+            - country (str, optional): Country of were the location is located. Defaults to "NL", The Netherlands.
         """
         if datetime_start is None:
             datetime_start = datetime.utcnow()
 
         systems_service = Systems()
 
         # sid selection for pvdata
@@ -141,15 +145,21 @@
 
         # Get weather data
         weather_params = ["radiation", "clouds"]
         start = datetime_start + timedelta(days=-history)  # '2017-10-10'
         end = datetime_start + timedelta(minutes=forecast_horizon)
 
         weather_data = Weather().get_weather_data(
-            location, weather_params, start, end, source="optimum"
+            location,
+            weather_params,
+            start,
+            end,
+            source="optimum",
+            resolution="15min",
+            country=country,
         )
 
         # Interpolate weather data to 15 minute values
         weather_data = weather_data.resample(str(forecast_resolution) + "T").asfreq()
         for col in weather_params:
             if col in weather_data:
                 weather_data.loc[:, col] = weather_data.loc[:, col].interpolate(
@@ -189,37 +199,41 @@
         self,
         location: Union[Tuple[float, float], str],
         hub_height: int,
         forecast_horizon: int,
         forecast_resolution: int,
         datetime_start: datetime = None,
         source: str = "optimum",
+        country: str = "NL",
     ) -> pd.DataFrame:
         """This function retrieves the wind speed forecast for the nearest weather location
         and calculates the wind speed based on the turbine's hub height.
         It interpolates these values according to the forecast resolution.
 
         Args:
             location: lat/lon values [int] or input city [str] of turbine location
             forecast_horizon: length of forecast in minutes [int]
             forecast_resolution: time resolution of forecast in minutes [int]
             datetime_start: datetime of forecast
             source: preferred weather source as a string, default for wind is DSN
+            country (str, optional): Country of were the location is located. Defaults to "NL", The Netherlands.
         """
 
         if datetime_start is None:
             datetime_start = datetime.utcnow()
         datetime_end = datetime_start + timedelta(minutes=forecast_horizon)
 
         windspeed = Weather().get_weather_data(
             location=location,
             weatherparams="windspeed_100m",
             datetime_start=datetime_start,
             datetime_end=datetime_end,
             source=source,
+            resolution="15min",
+            country=country,
         )
 
         # interpolate results to 15 minute values
         windspeed = windspeed.resample(str(forecast_resolution) + "T").asfreq()
         windspeed = windspeed.interpolate("cubic")
 
         return pd.DataFrame(windspeed.windspeed_100m)
```

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.7.5/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/predictions.py` & `openstef_dbc-3.7.5/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/predictor.py` & `openstef_dbc-3.7.5/openstef_dbc/services/predictor.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,28 @@
     def get_predictors(
         self,
         datetime_start: datetime.datetime,
         datetime_end: datetime.datetime,
         forecast_resolution: Optional[str] = None,
         location: Union[str, Tuple[float, float]] = None,
         predictor_groups: Union[List[PredictorGroups], List[str], None] = None,
+        country: str = "NL",
     ) -> pd.DataFrame:
         """Get predictors.
 
         Get predictors for a given datetime range. Optionally predictor groups can be
         selected. If the WEATHER_DATA group is included a location is required.
 
         Args:
             datetime_start (datetime): Date time end.
             datetime_end (datetime): Date time start.
             location (Union[str, Tuple[float, float]], optional): Location (for weather data).
                 Defaults to None.
+            country (str, optional): Country code (for weather data).
+                Defaults to "NL".
             predictor_groups (Optional[List[str]], optional): The groups of predictors
                 to include (see the PredictorGroups enum for allowed values). When set to
                 None or not given all predictor groups will be returned. Defaults to None.
 
         Returns:
             pd.DataFrame: Requested predictors with timezone aware datetime index.
         """
@@ -67,14 +70,15 @@
         predictors = []
 
         if PredictorGroups.WEATHER_DATA in predictor_groups:
             weather_data_predictors = self.get_weather_data(
                 datetime_start,
                 datetime_end,
                 location=location,
+                country=country,
                 forecast_resolution=forecast_resolution,
             )
             predictors.append(weather_data_predictors)
 
         if PredictorGroups.MARKET_DATA in predictor_groups:
             market_data_predictors = self.get_market_data(
                 datetime_start, datetime_end, forecast_resolution=forecast_resolution
@@ -234,14 +238,15 @@
 
     def get_weather_data(
         self,
         datetime_start: datetime.datetime,
         datetime_end: datetime.datetime,
         location: Union[Tuple[float, float], str],
         forecast_resolution: str = None,
+        country: str = "NL",
     ) -> pd.DataFrame:
         # Get weather data
         weather_params = [
             "clouds",
             "radiation",
             "temp",
             "winddeg",
@@ -258,14 +263,15 @@
         ]
         weather_data = Weather().get_weather_data(
             location,
             weather_params,
             datetime_start,
             datetime_end,
             source="optimum",
+            country=country,
         )
 
         # Post process weather data
         # This might not be required anymore?
         if "source_1" in list(weather_data):
             weather_data["source"] = weather_data.source_1
             weather_data = weather_data.drop("source_1", axis=1)
```

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/splitting.py` & `openstef_dbc-3.7.5/openstef_dbc/services/splitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,31 +62,34 @@
         return result
 
     def get_wind_ref(
         self,
         location: Union[Tuple[float, float], str],
         datetime_start: datetime,
         datetime_end: datetime,
+        country: str = "NL",
     ) -> pd.DataFrame:
         """Function that gets windspeed data from the influx database and converts it to windref data suitable
         for splitting energy.
         Parameters:
             location: str, country or location
             datetime_start: datetime, start time of required windref
             datetime_end: datetime, end time of required windref
+            country: str, default is "NL"
         Output:
             windref: pandas dataframe containing the windref data"""
 
         # Get weather information from the influx database
         wind_speed = Weather().get_weather_data(
             location,
             ["windspeed_100m"],
             datetime_start=datetime_start,
             datetime_end=datetime_end,
             source="optimum",
+            country=country,
         )
 
         wind_ref = self._calculate_windspeed_at_hubheight(
             self, windspeed=wind_speed["windspeed_100m"], fromheight=100, hub_height=100
         )
         wind_ref = wind_ref / np.abs(np.amax(wind_ref))
```

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/systems.py` & `openstef_dbc-3.7.5/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/weather.py` & `openstef_dbc-3.7.5/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/services/write.py` & `openstef_dbc-3.7.5/openstef_dbc/services/write.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc/utils.py` & `openstef_dbc-3.7.5/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.7.5/openstef_dbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.7.4
+Version: 3.7.5
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,20 +18,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ciso8601~=2.3.0
 Requires-Dist: geopy~=2.3.0
 Requires-Dist: openstef~=3.4.4
 Requires-Dist: pydantic-settings~=2.1.0
 Requires-Dist: influxdb-client~=1.36.1
-Requires-Dist: mysql-connector-python~=8.0.31
-Requires-Dist: pandas==2.1.3
+Requires-Dist: mysql-connector-python~=8.3.0
 Requires-Dist: PyMySQL~=1.0.2
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.28.1
-Requires-Dist: SQLAlchemy~=1.4.46
+Requires-Dist: SQLAlchemy~=2.0.21
 
 <!--
 SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com>
 
 SPDX-License-Identifier: MPL-2.0
 -->
 [![Python Build](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml/badge.svg?branch=master)](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml)
```

### Comparing `openstef_dbc-3.7.4/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.7.5/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.4/setup.py` & `openstef_dbc-3.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.7.4",
+    version="3.7.5",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

