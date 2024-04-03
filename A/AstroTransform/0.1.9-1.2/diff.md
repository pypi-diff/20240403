# Comparing `tmp/AstroTransform-0.1.9.tar.gz` & `tmp/AstroTransform-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroTransform-0.1.9.tar", last modified: Mon Sep 25 12:58:49 2023, max compression
+gzip compressed data, was "AstroTransform-1.2.tar", last modified: Wed Apr  3 10:12:40 2024, max compression
```

## Comparing `AstroTransform-0.1.9.tar` & `AstroTransform-1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.942524 AstroTransform-0.1.9/
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.389997 AstroTransform-0.1.9/AstroTransform/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)       22 2023-09-11 13:42:03.000000 AstroTransform-0.1.9/AstroTransform/__init__.py
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.589357 AstroTransform-0.1.9/AstroTransform/coords/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     2251 2023-09-25 12:57:32.000000 AstroTransform-0.1.9/AstroTransform/coords/AltAz.py
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/coords/__init__.py
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1561 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/coords/hour_angle.py
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.651768 AstroTransform-0.1.9/AstroTransform/parse/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1322 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/parse/LatLon.py
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/parse/__init__.py
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.756579 AstroTransform-0.1.9/AstroTransform/time/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     3080 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/time/JD.py
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/time/__init__.py
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     2664 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/AstroTransform/time/lst.py
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.492941 AstroTransform-0.1.9/AstroTransform.egg-info/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)      204 2023-09-25 12:58:48.000000 AstroTransform-0.1.9/AstroTransform.egg-info/PKG-INFO
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)      680 2023-09-25 12:58:49.000000 AstroTransform-0.1.9/AstroTransform.egg-info/SOURCES.txt
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)        1 2023-09-25 12:58:48.000000 AstroTransform-0.1.9/AstroTransform.egg-info/dependency_links.txt
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)       21 2023-09-25 12:58:48.000000 AstroTransform-0.1.9/AstroTransform.egg-info/top_level.txt
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1087 2023-09-06 10:13:17.000000 AstroTransform-0.1.9/LICENSE
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)      204 2023-09-25 12:58:49.938467 AstroTransform-0.1.9/PKG-INFO
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)       67 2023-09-06 10:13:17.000000 AstroTransform-0.1.9/README.md
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)       38 2023-09-25 12:58:49.944537 AstroTransform-0.1.9/setup.cfg
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)      302 2023-09-25 12:57:42.000000 AstroTransform-0.1.9/setup.py
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.848400 AstroTransform-0.1.9/tests/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/tests/__init__.py
-drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-25 12:58:49.910982 AstroTransform-0.1.9/tests/test_time/
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/tests/test_time/__init__.py
--rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1905 2023-09-06 10:14:47.000000 AstroTransform-0.1.9/tests/test_time/test_JD.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.997564 AstroTransform-1.2/
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.531394 AstroTransform-1.2/AstroTransform/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)       20 2024-04-03 10:11:15.000000 AstroTransform-1.2/AstroTransform/__init__.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.707012 AstroTransform-1.2/AstroTransform/coords/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     3634 2023-12-04 13:49:01.000000 AstroTransform-1.2/AstroTransform/coords/AltAz.py
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-1.2/AstroTransform/coords/__init__.py
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1561 2023-09-06 10:14:47.000000 AstroTransform-1.2/AstroTransform/coords/hour_angle.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.764529 AstroTransform-1.2/AstroTransform/parse/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1322 2023-09-06 10:14:47.000000 AstroTransform-1.2/AstroTransform/parse/LatLon.py
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-1.2/AstroTransform/parse/__init__.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.837045 AstroTransform-1.2/AstroTransform/time/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     3080 2023-09-06 10:14:47.000000 AstroTransform-1.2/AstroTransform/time/JD.py
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-1.2/AstroTransform/time/__init__.py
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     2696 2023-10-12 12:13:11.000000 AstroTransform-1.2/AstroTransform/time/lst.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.612909 AstroTransform-1.2/AstroTransform.egg-info/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)      202 2024-04-03 10:12:39.000000 AstroTransform-1.2/AstroTransform.egg-info/PKG-INFO
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)      680 2024-04-03 10:12:39.000000 AstroTransform-1.2/AstroTransform.egg-info/SOURCES.txt
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)        1 2024-04-03 10:12:39.000000 AstroTransform-1.2/AstroTransform.egg-info/dependency_links.txt
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)       21 2024-04-03 10:12:39.000000 AstroTransform-1.2/AstroTransform.egg-info/top_level.txt
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1087 2023-09-06 10:13:17.000000 AstroTransform-1.2/LICENSE
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)      202 2024-04-03 10:12:39.993566 AstroTransform-1.2/PKG-INFO
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)       67 2023-09-06 10:13:17.000000 AstroTransform-1.2/README.md
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)       38 2024-04-03 10:12:39.998567 AstroTransform-1.2/setup.cfg
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)      300 2024-04-03 10:11:36.000000 AstroTransform-1.2/setup.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.906049 AstroTransform-1.2/tests/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-1.2/tests/__init__.py
+drwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2024-04-03 10:12:39.964568 AstroTransform-1.2/tests/test_time/
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)        0 2023-09-06 10:14:47.000000 AstroTransform-1.2/tests/test_time/__init__.py
+-rwxrwxrwx   0 physical256  (1000) physical256  (1000)     1905 2023-09-06 10:14:47.000000 AstroTransform-1.2/tests/test_time/test_JD.py
```

### Comparing `AstroTransform-0.1.9/AstroTransform/coords/AltAz.py` & `AstroTransform-1.2/AstroTransform/coords/AltAz.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 from datetime import datetime, timedelta
 from AstroTransform.time import JD, lst
 from AstroTransform.coords import hour_angle
 from astropy.time import Time
 
-def to_alt_az(RA, DEC, Lat, Lon, obs_time):
+def to_alt_az(RA, DEC, Lat, Lon, obs_time, time_zone=0):
     """
     Convert a target's RA and DEC to Altitude and Azimuth.
     
     Parameters
     ----------
     RA : float
         The right ascension of the target in hours.
@@ -41,37 +41,81 @@
         raise TypeError("Expected a float or int for 'DEC'.")
     if not isinstance(Lat, (int, float)):
         raise TypeError("Expected a float or int for 'Lat'.")
     if not isinstance(Lon, (int, float)):
         raise TypeError("Expected a float or int for 'Lon'.")
     if not isinstance(obs_time, datetime):
         raise TypeError("Expected a datetime.datetime object for 'obs_time'.")
-    
+
     #convert to radians
     RA_rad = np.deg2rad(RA * 15.0)
     DEC_rad = np.deg2rad(DEC)
     Lat_rad = np.deg2rad(Lat)
     Lon_rad = np.deg2rad(Lon)
 
     #calculate LST
-    LST = lst.lst(obs_time, Lon)
+    LST = lst.lst(obs_time, Lon, time_zone)
     
     #calculate hour angle
     HA = hour_angle.hourangle(LST, RA)
     HA_rad = np.deg2rad(HA*15.0)
     LSTrad = np.deg2rad(LST*15.0)
-
-    #calculate altitude
+    # calculate altitude
     sin_alt = np.sin(DEC_rad)*np.sin(Lat_rad) + np.cos(DEC_rad)*np.cos(Lat_rad)*np.cos(HA_rad)
     alt = np.arcsin(sin_alt)
-
-    #calculate azimuth
-    sin_az = -np.sin(HA_rad)*np.cos(DEC_rad)/np.cos(alt)
-    az = np.arcsin(sin_az)
-    
+    #calculate azimuth #
+    tolerance = 1e-6
+    cos_az = (np.sin(DEC_rad) - np.sin(alt)*np.sin(Lat_rad))/(np.cos(alt)*np.cos(Lat_rad))
+    if not -1 - tolerance <= cos_az <= 1 + tolerance:
+        # Log a warning or raise an error
+        print(f"Warning: cos_az value {cos_az} is significantly out of range.")
+    cos_az = np.clip(cos_az, -1.0, 1.0)
+    az = np.arccos(cos_az)
+
+    if np.sin(HA_rad) > 0:
+        az = 2*np.pi - az
+    else:
+        az = az
     #convert to degrees
     alt = np.rad2deg(alt)
     az = np.rad2deg(az)
 
-    
+
     return alt, az
 
+def max_alt(DEC, Lat):
+    """
+    Calculate the maximum altitude of a target.
+    
+    Parameters
+    ----------
+    DEC : float
+        The declination of the target in degrees.
+    Lat : float
+        The latitude of the observer in degrees.    
+    Returns
+    -------
+    float
+        The maximum altitude of the target in degrees.
+        
+    """
+    if not isinstance(DEC, (int, float)):
+        raise TypeError("Expected a float or int for 'DEC'.")
+    if not isinstance(Lat, (int, float)):
+        raise TypeError("Expected a float or int for 'Lat'.")
+    #convert to radians
+
+    DEC_rad = np.deg2rad(DEC)
+    Lat_rad = np.deg2rad(Lat)
+
+    
+    #calculate hour angle
+    HA = 0 # hour angle 0 when target transits
+    HA_rad = np.deg2rad(HA*15.0)
+
+    # calculate altitude
+    sin_alt = np.sin(DEC_rad)*np.sin(Lat_rad) + np.cos(DEC_rad)*np.cos(Lat_rad)*np.cos(HA_rad)
+    alt = np.arcsin(sin_alt)
+    #convert to degrees
+    alt = np.rad2deg(alt)
+    return alt
+
```

### Comparing `AstroTransform-0.1.9/AstroTransform/coords/hour_angle.py` & `AstroTransform-1.2/AstroTransform/coords/hour_angle.py`

 * *Files identical despite different names*

### Comparing `AstroTransform-0.1.9/AstroTransform/parse/LatLon.py` & `AstroTransform-1.2/AstroTransform/parse/LatLon.py`

 * *Files identical despite different names*

### Comparing `AstroTransform-0.1.9/AstroTransform/time/JD.py` & `AstroTransform-1.2/AstroTransform/time/JD.py`

 * *Files identical despite different names*

### Comparing `AstroTransform-0.1.9/AstroTransform/time/lst.py` & `AstroTransform-1.2/AstroTransform/time/lst.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Package for calculating Local Sidereal Time.
 """
 
 import numpy as np
 from datetime import datetime, timedelta
 from AstroTransform.time import JD
 
-def local_to_ut(local_time, longitude):
+def local_to_ut(local_time, longitude, time_zone):
     """
     Convert a local time to a Universal Time.
 
     Parameters
     ----------
     local_time : datetime.datetime
         The local time to convert to Universal Time.
@@ -24,22 +24,22 @@
     """
     if not isinstance(local_time, datetime):
         raise TypeError("Expected a datetime.datetime object for 'local_time'.")
     if not isinstance(longitude, (int, float)):
         raise TypeError("Expected a float or int for 'longitude'.")
 
     # Calculate the offset in hours
-    offset = longitude / 15.0
+    offset = time_zone
 
     # Convert to UT
     ut = local_time - timedelta(hours=offset)
 
     return ut
 
-def ut_to_local(ut, longitude):
+def ut_to_local(ut, longitude, time_zone):
     """
     Convert a Universal Time to a local time.
 
     Parameters
     ----------
     ut : datetime.datetime
         The Universal Time to convert to local time.  
@@ -54,22 +54,22 @@
 
     if not isinstance(ut, datetime):
         raise TypeError("Expected a datetime.datetime object for 'ut'.")
     if not isinstance(longitude, (int, float)):
         raise TypeError("Expected a float or int for 'longitude'.")
 
     # Calculate the offset in hours
-    offset = longitude / 15.0
+    offset = time_zone
 
     # Convert to local time
     local_time = ut + timedelta(hours=offset)
 
     return local_time
 
-def lst(date_time, longitude):
+def lst(date_time, longitude, time_zone=0):
     """
     Calculate the Local Sidereal Time.
 
     Parameters
     ----------
     date_time : datetime.datetime
         The datetime object to calculate the LST for.
@@ -79,15 +79,15 @@
     Returns
     -------
     float
         The Local Sidereal Time in hours.
     """
 
     #convert to UT
-    ut = local_to_ut(date_time, longitude)
+    ut = local_to_ut(date_time, longitude, time_zone)
 
     # Calculate the Julian Date
     jd = JD.to_jd(ut)
 
     # calculate the number of days since 1st january 2000 at 12:00 UT
     D = (jd - 2451545.0)
```

### Comparing `AstroTransform-0.1.9/AstroTransform.egg-info/SOURCES.txt` & `AstroTransform-1.2/AstroTransform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AstroTransform-0.1.9/LICENSE` & `AstroTransform-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AstroTransform-0.1.9/tests/test_time/test_JD.py` & `AstroTransform-1.2/tests/test_time/test_JD.py`

 * *Files identical despite different names*

