# Comparing `tmp/weather_wise-0.1.4.tar.gz` & `tmp/weather_wise-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_wise-0.1.4.tar", max compression
+gzip compressed data, was "weather_wise-0.1.5.tar", max compression
```

## Comparing `weather_wise-0.1.4.tar` & `weather_wise-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1800 2024-03-11 17:53:36.931164 weather_wise-0.1.4/README.md
--rw-r--r--   0        0        0      656 2024-03-12 13:34:19.876871 weather_wise-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       46 2024-02-29 00:15:12.026008 weather_wise-0.1.4/weather_wise/__init__.py
--rw-r--r--   0        0        0  2972714 2024-02-16 23:05:32.457530 weather_wise-0.1.4/weather_wise/data/2022_gazetteer_zcta_national.json
--rw-r--r--   0        0        0  6792182 2024-02-16 23:52:47.920693 weather_wise-0.1.4/weather_wise/data/2022_gazetteer_zcta_national.txt
--rw-r--r--   0        0        0     5573 2024-03-12 13:31:23.936928 weather_wise-0.1.4/weather_wise/weather_wise.py
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 weather_wise-0.1.4/setup.py
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 weather_wise-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1867 2024-04-03 02:16:57.192605 weather_wise-0.1.5/README.md
+-rw-r--r--   0        0        0      656 2024-04-03 02:17:42.312600 weather_wise-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       46 2024-02-29 00:15:12.026008 weather_wise-0.1.5/weather_wise/__init__.py
+-rw-r--r--   0        0        0  2972714 2024-04-02 23:51:27.653440 weather_wise-0.1.5/weather_wise/data/2022_gazetteer_zcta_national.json
+-rw-r--r--   0        0        0  6792182 2024-04-02 23:51:27.673440 weather_wise-0.1.5/weather_wise/data/2022_gazetteer_zcta_national.txt
+-rw-r--r--   0        0        0     6049 2024-04-02 23:52:31.123455 weather_wise-0.1.5/weather_wise/weather_wise.py
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 weather_wise-0.1.5/setup.py
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 weather_wise-0.1.5/PKG-INFO
```

### Comparing `weather_wise-0.1.4/README.md` & `weather_wise-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,30 +18,34 @@
 print(weather._get_weather_forecast_url())
 print(json.dumps(weather._get_weather_data(), indent=2))
 
 # Get the short forecast.
 short_forecast = weather.get_short_forecast()
 print(short_forecast)
 
-# Get the detailed forecast.
-detailed_forecast = weather.get_detailed_forecast()
-print(detailed_forecast)
-
 # Get the temperature in fahrenheit.
 temperature_in_fahrenheit = weather.get_temperature_in_fahrenheit(temperature_unit=True)
 print(temperature_in_fahrenheit)
 
 # Get the temperature in celsius.
 temperature_in_celsius = weather.get_temperature_in_celsius()
 print(temperature_in_celsius)
 
 # Get the chance of rain.
 chance_of_rain = weather.get_probability_of_precipitation()
 print(chance_of_rain)
 
+# Get the wind speed.
+wind_speed = weather.get_wind_speed()
+print(wind_speed)
+
+# Get the wind direction.
+wind_direction = weather.get_wind_direction()
+print(wind_direction)
+
 # Get the wind.
 wind = weather.get_wind()
 print(wind)
 ```
 
 ## References
```

### Comparing `weather_wise-0.1.4/pyproject.toml` & `weather_wise-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather-wise"
-version = "0.1.4"
+version = "0.1.5"
 description = "Obtain local weather information based on zipcode."
 authors = ["Aaron Britton <brittonleeaaron@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "weather_wise"},
 ]
```

### Comparing `weather_wise-0.1.4/weather_wise/data/2022_gazetteer_zcta_national.json` & `weather_wise-0.1.5/weather_wise/data/2022_gazetteer_zcta_national.json`

 * *Files identical despite different names*

### Comparing `weather_wise-0.1.4/weather_wise/data/2022_gazetteer_zcta_national.txt` & `weather_wise-0.1.5/weather_wise/data/2022_gazetteer_zcta_national.txt`

 * *Files identical despite different names*

### Comparing `weather_wise-0.1.4/weather_wise/weather_wise.py` & `weather_wise-0.1.5/weather_wise/weather_wise.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         weather_data = weather_data_response.json()
         current_weather = weather_data["properties"]["periods"][0]
 
         weather_information = {
             "short_forecast": current_weather["shortForecast"],
             "detailed_forecast": current_weather["detailedForecast"],
             "temperature": current_weather["temperature"],
-            "probability_of_precipitation": current_weather["probabilityOfPrecipitation"]["value"],
             "temperature_unit": current_weather["temperatureUnit"],
+            "probability_of_precipitation": current_weather["probabilityOfPrecipitation"]["value"],
             "wind_speed": current_weather["windSpeed"],
             "wind_direction": current_weather["windDirection"],
         }
 
         return weather_information
 
     def get_short_forecast(self) -> str:
@@ -139,17 +139,37 @@
 
         Returns:
             str: Current probability of precipitation.
         """
         probability_of_precipitation = self.weather_details["probability_of_precipitation"]
 
         if probability_of_precipitation is None:
-            return "0%"
+            return "0"
+
+        return f"{probability_of_precipitation}"
+
+    def get_wind_speed(self) -> str:
+        """Get the current wind speed.
+
+        Returns:
+            str: Current wind speed.
+        """
+        wind_speed = self.weather_details["wind_speed"]
+
+        return wind_speed
+
+    def get_wind_direction(self) -> str:
+        """Get the current wind direction.
+
+        Returns:
+            str: Current wind direction.
+        """
+        wind_direction = self.weather_details["wind_direction"]
 
-        return f"{probability_of_precipitation}%"
+        return wind_direction
 
     def get_wind(self) -> str:
         """Get the current wind speed and wind direction.
 
         Returns:
             str: Current wind speed and wind direction.
         """
```

### Comparing `weather_wise-0.1.4/setup.py` & `weather_wise-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'weather_wise': ['data/*']}
 
 install_requires = \
 ['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'weather-wise',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Obtain local weather information based on zipcode.',
-    'long_description': '# Weather Wise\n\n## Overview\n\nGet the current weather forecast and other weather related information from a zipcode.  This module uses the U.S. Census 2022 Gazetteer (Zip Code Tabulation Areas).  The original file has been modified to JSON.\n\n## Usage\n\n```python\nimport json\nfrom weather_wise.weather_wise import WeatherWise\n\nweather = WeatherWise("32904")\n\n# Internal weather methods.\nprint(weather._load_json_data())\nprint(weather._get_latitude_longitude())\nprint(weather._get_weather_forecast_url())\nprint(json.dumps(weather._get_weather_data(), indent=2))\n\n# Get the short forecast.\nshort_forecast = weather.get_short_forecast()\nprint(short_forecast)\n\n# Get the detailed forecast.\ndetailed_forecast = weather.get_detailed_forecast()\nprint(detailed_forecast)\n\n# Get the temperature in fahrenheit.\ntemperature_in_fahrenheit = weather.get_temperature_in_fahrenheit(temperature_unit=True)\nprint(temperature_in_fahrenheit)\n\n# Get the temperature in celsius.\ntemperature_in_celsius = weather.get_temperature_in_celsius()\nprint(temperature_in_celsius)\n\n# Get the chance of rain.\nchance_of_rain = weather.get_probability_of_precipitation()\nprint(chance_of_rain)\n\n# Get the wind.\nwind = weather.get_wind()\nprint(wind)\n```\n\n## References\n\n- ### Gazetteer Files\n\n  - <https://www.census.gov/geographies/reference-files/time-series/geo/gazetteer-files.html>\n\n- ### API Documentation\n\n  - <https://www.weather.gov/documentation/services-web-api>\n\n- ### API Discussion\n\n  - <https://github.com/weather-gov/api/discussions>\n\n- ### Outage & Status Messages\n\n  - <https://www.nco.ncep.noaa.gov/status/messages/>\n\n## TODO\n\n- Get severe weather alerts.\n  - Active Alerts\n    - <https://api.weather.gov/alerts/active?point=38.9807,-76.9373>\n  - All Alerts\n    - <https://api.weather.gov/alerts?point=38.9807,-76.9373>\n',
+    'long_description': '# Weather Wise\n\n## Overview\n\nGet the current weather forecast and other weather related information from a zipcode.  This module uses the U.S. Census 2022 Gazetteer (Zip Code Tabulation Areas).  The original file has been modified to JSON.\n\n## Usage\n\n```python\nimport json\nfrom weather_wise.weather_wise import WeatherWise\n\nweather = WeatherWise("32904")\n\n# Internal weather methods.\nprint(weather._load_json_data())\nprint(weather._get_latitude_longitude())\nprint(weather._get_weather_forecast_url())\nprint(json.dumps(weather._get_weather_data(), indent=2))\n\n# Get the short forecast.\nshort_forecast = weather.get_short_forecast()\nprint(short_forecast)\n\n# Get the temperature in fahrenheit.\ntemperature_in_fahrenheit = weather.get_temperature_in_fahrenheit(temperature_unit=True)\nprint(temperature_in_fahrenheit)\n\n# Get the temperature in celsius.\ntemperature_in_celsius = weather.get_temperature_in_celsius()\nprint(temperature_in_celsius)\n\n# Get the chance of rain.\nchance_of_rain = weather.get_probability_of_precipitation()\nprint(chance_of_rain)\n\n# Get the wind speed.\nwind_speed = weather.get_wind_speed()\nprint(wind_speed)\n\n# Get the wind direction.\nwind_direction = weather.get_wind_direction()\nprint(wind_direction)\n\n# Get the wind.\nwind = weather.get_wind()\nprint(wind)\n```\n\n## References\n\n- ### Gazetteer Files\n\n  - <https://www.census.gov/geographies/reference-files/time-series/geo/gazetteer-files.html>\n\n- ### API Documentation\n\n  - <https://www.weather.gov/documentation/services-web-api>\n\n- ### API Discussion\n\n  - <https://github.com/weather-gov/api/discussions>\n\n- ### Outage & Status Messages\n\n  - <https://www.nco.ncep.noaa.gov/status/messages/>\n\n## TODO\n\n- Get severe weather alerts.\n  - Active Alerts\n    - <https://api.weather.gov/alerts/active?point=38.9807,-76.9373>\n  - All Alerts\n    - <https://api.weather.gov/alerts?point=38.9807,-76.9373>\n',
     'author': 'Aaron Britton',
     'author_email': 'brittonleeaaron@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `weather_wise-0.1.4/PKG-INFO` & `weather_wise-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-wise
-Version: 0.1.4
+Version: 0.1.5
 Summary: Obtain local weather information based on zipcode.
 Author: Aaron Britton
 Author-email: brittonleeaaron@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -31,30 +31,34 @@
 print(weather._get_weather_forecast_url())
 print(json.dumps(weather._get_weather_data(), indent=2))
 
 # Get the short forecast.
 short_forecast = weather.get_short_forecast()
 print(short_forecast)
 
-# Get the detailed forecast.
-detailed_forecast = weather.get_detailed_forecast()
-print(detailed_forecast)
-
 # Get the temperature in fahrenheit.
 temperature_in_fahrenheit = weather.get_temperature_in_fahrenheit(temperature_unit=True)
 print(temperature_in_fahrenheit)
 
 # Get the temperature in celsius.
 temperature_in_celsius = weather.get_temperature_in_celsius()
 print(temperature_in_celsius)
 
 # Get the chance of rain.
 chance_of_rain = weather.get_probability_of_precipitation()
 print(chance_of_rain)
 
+# Get the wind speed.
+wind_speed = weather.get_wind_speed()
+print(wind_speed)
+
+# Get the wind direction.
+wind_direction = weather.get_wind_direction()
+print(wind_direction)
+
 # Get the wind.
 wind = weather.get_wind()
 print(wind)
 ```
 
 ## References
```

