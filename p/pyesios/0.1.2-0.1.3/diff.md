# Comparing `tmp/pyesios-0.1.2.tar.gz` & `tmp/pyesios-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesios-0.1.2.tar", max compression
+gzip compressed data, was "pyesios-0.1.3.tar", max compression
```

## Comparing `pyesios-0.1.2.tar` & `pyesios-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35147 2023-10-24 13:24:31.573980 pyesios-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1503 2023-10-30 14:30:37.594367 pyesios-0.1.2/README.md
--rw-r--r--   0        0        0    15194 2023-10-30 14:29:22.857699 pyesios-0.1.2/pyesios/ESIOS.py
--rw-r--r--   0        0        0       53 2023-10-24 13:24:31.577313 pyesios-0.1.2/pyesios/__init__.py
--rw-r--r--   0        0        0       79 2023-10-24 13:24:31.577313 pyesios-0.1.2/pyesios/__version__.py
--rw-r--r--   0        0        0     1234 2023-10-24 17:07:10.857376 pyesios-0.1.2/pyesios/utils.py
--rw-r--r--   0        0        0     1304 2023-10-25 10:29:57.473302 pyesios-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 pyesios-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-10-24 13:24:31.573980 pyesios-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1503 2023-10-30 14:38:18.257702 pyesios-0.1.3/README.md
+-rw-r--r--   0        0        0    15543 2024-04-03 18:13:42.616485 pyesios-0.1.3/pyesios/ESIOS.py
+-rw-r--r--   0        0        0       53 2023-10-24 13:24:31.577313 pyesios-0.1.3/pyesios/__init__.py
+-rw-r--r--   0        0        0       79 2023-10-24 13:24:31.577313 pyesios-0.1.3/pyesios/__version__.py
+-rw-r--r--   0        0        0     1234 2023-10-30 14:38:18.257702 pyesios-0.1.3/pyesios/utils.py
+-rw-r--r--   0        0        0     1304 2024-04-03 18:15:20.806482 pyesios-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 pyesios-0.1.3/PKG-INFO
```

### Comparing `pyesios-0.1.2/LICENSE.txt` & `pyesios-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyesios-0.1.2/README.md` & `pyesios-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyesios-0.1.2/pyesios/ESIOS.py` & `pyesios-0.1.3/pyesios/ESIOS.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import datetime
 import json
 import pickle
 import urllib
+import urllib.error
+import urllib.parse
 import urllib.request
 import warnings
 
 import numpy as np
 import pandas as pd
 
 from pyesios.utils import time_diff_in_group
@@ -85,15 +87,15 @@
         Prepares the CURL headers
         :return: A dictionary with the headers.
         :rtype: dict
         """
         headers = {
             "Accept": "application/json; application/vnd.esios-api-v2+json",
             "Content-Type": "application/json",
-            "Host": "api.esios.ree.es",
+            # "Host": "api.esios.ree.es",
             "x-api-key": self.token,
             "Cookie": "",
         }
         return headers
 
     def __make_request__(self, url):
         """
@@ -101,20 +103,44 @@
         :param url: The URL to make the request to.
         :type url: str
         :return: The JSON response.
         :rtype: dict
         """
         headers = self.__get_headers__()
         req = urllib.request.Request(url, headers=headers)
-        with urllib.request.urlopen(req) as response:
-            try:
-                json_data = response.read().decode("utf-8")
-            except Exception as e:
-                warnings.warn(e)
-                json_data = response.readall().decode("utf-8")
+
+        # with urllib.request.urlopen(req) as response:
+        #     try:
+        #         json_data = response.read().decode("utf-8")
+        #     except Exception as e:
+        #         warnings.warn(e)
+        #         json_data = response.readall().decode("utf-8")
+
+        """
+        In order to handle redirections, follow:
+        https://stackoverflow.com/questions/62384020/python-3-7-urllib-request-doesnt-follow-redirect-url
+        """
+
+        try:
+            response = urllib.request.urlopen(req)
+        except urllib.error.HTTPError as e:
+            if e.status != 307:
+                raise  # not a status code that can be handled here
+            redirected_url = urllib.parse.urljoin(url, e.headers["Location"])
+            response = urllib.request.urlopen(redirected_url)
+            print(
+                "Redirected -> %s" % redirected_url
+            )  # the original redirected url
+
+        try:
+            json_data = response.read().decode("utf-8")
+        except Exception as e:
+            warnings.warn(e)
+            json_data = response.readall().decode("utf-8")
+
         return json.loads(json_data)
 
     def get_indicators(self):
         """
         Get the indicators and their name.
         The indicators are the indices assigned to the available data series
         :return:
@@ -242,14 +268,16 @@
             )
             warnings.warn(warn_msg)
             timegroup = "hour"
 
         # This is how the URL is built
 
         #  https://www.esios.ree.es/es/analisis/1293?vis=2&start_date=21-06-2016T00%3A00&end_date=21-06-2016T23%3A50&compare_start_date=20-06-2016T00%3A00&groupby=minutes10&compare_indicators=545,544#JSON
+        #  https://www.esios.ree.es/es/analisis/1293?vis=2&start_date=21-06-2022T00%3A00&end_date=21-06-2022T23%3A50&compare_start_date=20-06-2022T00%3A00&groupby=minutes10&compare_indicators=545,544#JSON
+
         url = (
             "https://api.esios.ree.es/indicators/"
             + indicator
             + "?start_date="
             + start_str
             + "&end_date="
             + end_str
@@ -279,15 +307,18 @@
             indicator, start, end, timegroup=timegroup, **options
         )
 
         # transform the data
         d = result["indicator"]["values"]  # dictionary of values
         if len(d) > 0:
             df = pd.DataFrame(d)
-
+            not_utc_index = df[df["datetime_utc"].str.len() > 21].index
+            df.loc[not_utc_index, "datetime_utc"] = pd.to_datetime(
+                df.loc[not_utc_index]["datetime_utc"]
+            ).dt.strftime("%Y-%m-%dT%H:%M:%SZ")
             df["datetime_utc"] = pd.to_datetime(
                 df["datetime_utc"]
             )  # convert to datetime
 
             df = df.set_index("datetime_utc")  # Set the index column
 
             # del df.index.name  # to avoid the index name bullshit
@@ -342,36 +373,17 @@
                 date_range.append(end)
             else:
                 date_range[-1] = end
 
             # Create a list to store the date pairs
             all_dfs = []
             # Loop over the date range
-            last = False
             for i in range(len(date_range) - 1):
-                if last:
-                    continue
                 # Add the date pair to the list
                 start_str = date_range[i].strftime(self.dateformat)
-                # The API is not workinf for 2022 on
-                # https://github.com/SanPen/ESIOS/issues/10
-                if date_range[i + 1].year > 2021:
-                    warnings.warn("API not working for anything after 2022")
-                    warnings.warn("Setting to last hour of 2021")
-                    date_range[i + 1] = date_range[i + 1].replace(year=2021)
-                    date_range[i + 1] = date_range[i + 1].replace(month=12)
-                    date_range[i + 1] = date_range[i + 1].replace(day=31)
-                    # Set the time to the last minute of the day
-                    date_range[i + 1] = date_range[i + 1].replace(
-                        hour=23, minute=59, second=59
-                    )
-                    # Convert the datetime object back to a string
-                    date_range[i + 1].strftime("%Y-%m-%dT%H:%M:%S")
-                    last = True
-
                 end_str = date_range[i + 1].strftime(self.dateformat)
                 all_dfs.append(
                     self._get_data(
                         indicator,
                         start_str,
                         end_str,
                         timegroup=timegroup,
```

### Comparing `pyesios-0.1.2/pyesios/utils.py` & `pyesios-0.1.3/pyesios/utils.py`

 * *Files identical despite different names*

### Comparing `pyesios-0.1.2/pyproject.toml` & `pyesios-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyesios"
-version = "0.1.2"
+version = "0.1.3"
 description = "Access to the ESIOS data, the Spanish electricity market entity."
 authors = ["Santiago Peñate Vera <santiago.penate.vera@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://github.com/SanPen/ESIOS"
 repository = "https://github.com/SanPen/ESIOS"
```

### Comparing `pyesios-0.1.2/PKG-INFO` & `pyesios-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesios
-Version: 0.1.2
+Version: 0.1.3
 Summary: Access to the ESIOS data, the Spanish electricity market entity.
 Home-page: https://github.com/SanPen/ESIOS
 License: LICENSE.txt
 Author: Santiago Peñate Vera
 Author-email: santiago.penate.vera@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

