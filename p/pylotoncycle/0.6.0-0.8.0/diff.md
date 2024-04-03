# Comparing `tmp/pylotoncycle-0.6.0.tar.gz` & `tmp/pylotoncycle-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylotoncycle-0.6.0.tar", last modified: Mon Jan  2 17:49:47 2023, max compression
+gzip compressed data, was "pylotoncycle-0.8.0.tar", last modified: Wed Apr  3 06:02:31 2024, max compression
```

## Comparing `pylotoncycle-0.6.0.tar` & `pylotoncycle-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 adukia    (1000) adukia    (1000)        0 2023-01-02 17:49:47.823014 pylotoncycle-0.6.0/
--rw-r--r--   0 adukia    (1000) adukia    (1000)     8608 2023-01-02 17:49:47.823014 pylotoncycle-0.6.0/PKG-INFO
--rw-r--r--   0 adukia    (1000) adukia    (1000)     6790 2023-01-02 17:20:47.000000 pylotoncycle-0.6.0/README.md
-drwxr-xr-x   0 adukia    (1000) adukia    (1000)        0 2023-01-02 17:49:47.823014 pylotoncycle-0.6.0/pylotoncycle/
--rw-r--r--   0 adukia    (1000) adukia    (1000)      139 2023-01-02 17:30:08.000000 pylotoncycle-0.6.0/pylotoncycle/__init__.py
--rw-r--r--   0 adukia    (1000) adukia    (1000)     2761 2023-01-02 17:29:35.000000 pylotoncycle-0.6.0/pylotoncycle/parser.py
--rwxr-xr-x   0 adukia    (1000) adukia    (1000)     5728 2023-01-02 17:29:51.000000 pylotoncycle-0.6.0/pylotoncycle/pylotoncycle.py
-drwxr-xr-x   0 adukia    (1000) adukia    (1000)        0 2023-01-02 17:49:47.823014 pylotoncycle-0.6.0/pylotoncycle.egg-info/
--rw-r--r--   0 adukia    (1000) adukia    (1000)     8608 2023-01-02 17:49:47.000000 pylotoncycle-0.6.0/pylotoncycle.egg-info/PKG-INFO
--rw-r--r--   0 adukia    (1000) adukia    (1000)      289 2023-01-02 17:49:47.000000 pylotoncycle-0.6.0/pylotoncycle.egg-info/SOURCES.txt
--rw-r--r--   0 adukia    (1000) adukia    (1000)        1 2023-01-02 17:49:47.000000 pylotoncycle-0.6.0/pylotoncycle.egg-info/dependency_links.txt
--rw-r--r--   0 adukia    (1000) adukia    (1000)        9 2023-01-02 17:49:47.000000 pylotoncycle-0.6.0/pylotoncycle.egg-info/requires.txt
--rw-r--r--   0 adukia    (1000) adukia    (1000)       13 2023-01-02 17:49:47.000000 pylotoncycle-0.6.0/pylotoncycle.egg-info/top_level.txt
--rw-r--r--   0 adukia    (1000) adukia    (1000)       30 2023-01-02 17:28:47.000000 pylotoncycle-0.6.0/pyproject.toml
--rw-r--r--   0 adukia    (1000) adukia    (1000)       38 2023-01-02 17:49:47.823014 pylotoncycle-0.6.0/setup.cfg
--rw-r--r--   0 adukia    (1000) adukia    (1000)      627 2023-01-02 17:49:08.000000 pylotoncycle-0.6.0/setup.py
+drwxr-xr-x   0 adukia    (1000) adukia    (1000)        0 2024-04-03 06:02:31.509538 pylotoncycle-0.8.0/
+-rw-r--r--   0 adukia    (1000) adukia    (1000)     1340 2024-04-03 05:59:31.000000 pylotoncycle-0.8.0/LICENSE
+-rw-r--r--   0 adukia    (1000) adukia    (1000)     7175 2024-04-03 06:02:31.509538 pylotoncycle-0.8.0/PKG-INFO
+-rw-r--r--   0 adukia    (1000) adukia    (1000)     6790 2024-04-03 05:59:31.000000 pylotoncycle-0.8.0/README.md
+drwxr-xr-x   0 adukia    (1000) adukia    (1000)        0 2024-04-03 06:02:31.509538 pylotoncycle-0.8.0/pylotoncycle/
+-rw-r--r--   0 adukia    (1000) adukia    (1000)      139 2024-04-03 05:59:31.000000 pylotoncycle-0.8.0/pylotoncycle/__init__.py
+-rw-r--r--   0 adukia    (1000) adukia    (1000)     2761 2024-04-03 05:59:31.000000 pylotoncycle-0.8.0/pylotoncycle/parser.py
+-rwxr-xr-x   0 adukia    (1000) adukia    (1000)     6021 2024-04-03 05:59:31.000000 pylotoncycle-0.8.0/pylotoncycle/pylotoncycle.py
+drwxr-xr-x   0 adukia    (1000) adukia    (1000)        0 2024-04-03 06:02:31.509538 pylotoncycle-0.8.0/pylotoncycle.egg-info/
+-rw-r--r--   0 adukia    (1000) adukia    (1000)     7175 2024-04-03 06:02:31.000000 pylotoncycle-0.8.0/pylotoncycle.egg-info/PKG-INFO
+-rw-r--r--   0 adukia    (1000) adukia    (1000)      297 2024-04-03 06:02:31.000000 pylotoncycle-0.8.0/pylotoncycle.egg-info/SOURCES.txt
+-rw-r--r--   0 adukia    (1000) adukia    (1000)        1 2024-04-03 06:02:31.000000 pylotoncycle-0.8.0/pylotoncycle.egg-info/dependency_links.txt
+-rw-r--r--   0 adukia    (1000) adukia    (1000)        9 2024-04-03 06:02:31.000000 pylotoncycle-0.8.0/pylotoncycle.egg-info/requires.txt
+-rw-r--r--   0 adukia    (1000) adukia    (1000)       13 2024-04-03 06:02:31.000000 pylotoncycle-0.8.0/pylotoncycle.egg-info/top_level.txt
+-rw-r--r--   0 adukia    (1000) adukia    (1000)       30 2024-04-03 05:59:31.000000 pylotoncycle-0.8.0/pyproject.toml
+-rw-r--r--   0 adukia    (1000) adukia    (1000)       38 2024-04-03 06:02:31.509538 pylotoncycle-0.8.0/setup.cfg
+-rw-r--r--   0 adukia    (1000) adukia    (1000)      627 2024-04-03 06:00:34.000000 pylotoncycle-0.8.0/setup.py
```

### Comparing `pylotoncycle-0.6.0/PKG-INFO` & `pylotoncycle-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,191 @@
 Metadata-Version: 2.1
 Name: pylotoncycle
-Version: 0.6.0
+Version: 0.8.0
 Summary: Module to access your Peloton workout data
 Home-page: https://github.com/justmedude/pylotoncycle
 Author: Vikram Adukia
 Author-email: github@fireitup.net
 License: BSD
-Description: # PylotonCycle
-        Python Library for getting your Peloton workout data.
-        
-        ## Table of contents
-        * [General info](#general-info)
-        * [Example Usage](#example-usage)
-        
-        ## General info
-        As someone who wants to see my progress over time, I've been wanting a way
-        to pull and play with my ride data. However, I'm also cautious about linking
-        myself to too many external parties. As I've been playing with other libraries
-        out there, I wanted something that was a bit more intuitive and would play
-        nicer with the rest of my python code. So, PylotonCycle is born.
-        
-        ## Example Usage
-        ```
-        import pylotoncycle
-        
-        username = 'your username or email address'
-        password = 'your password'
-        conn = pylotoncycle.PylotonCycle(username, password)
-        workouts = conn.GetRecentWorkouts(5)
-        ```
-        `workouts` is a list of workouts.
-        
-        An example of a list element
-        
-        ```
-        {'achievement_templates': [{'description': 'Awarded for working out with a '
-                                                   'friend.',
-                                    'id': '<some id hash>',
-                                    'image_url': 'https://s3.amazonaws.com/peloton-achievement-images-prod/702495cd985d4791bfd3d25f36e0df72',
-                                    'name': 'Dynamic Duo',
-                                    'slug': 'two_to_tango'},
-                                   {'description': 'Awarded for achieving Silver in '
-                                                   'the May Cycling Challenge.',
-                                    'id': '<some id hash>',
-                                    'image_url': 'https://s3.amazonaws.com/challenges-and-tiers-image-prod/6b772477ccd04f189fba16f2f877faad',
-                                    'name': 'May Cycling Challenge',
-                                    'slug': 'may_cycling_challenge_silver'}],
-         'created': 1589642476,
-         'created_at': 1589642476,
-         'device_time_created_at': 1589617276,
-         'device_type': 'home_bike_v1',
-         'device_type_display_name': 'Bike',
-         'end_time': 1589644336,
-         'fitbit_id': None,
-         'fitness_discipline': 'cycling',
-         'ftp_info': {'ftp': 111,
-                      'ftp_source': 'ftp_workout_source',
-                      'ftp_workout_id': '<some id hash>'},
-         'has_leaderboard_metrics': True,
-         'has_pedaling_metrics': True,
-         'id': '<some id hash>',
-         'instructor_name': 'Matt Wilpers',
-         'is_total_work_personal_record': False,
-         'leaderboard_rank': 5015,
-         'metrics_type': 'cycling',
-         'name': 'Cycling Workout',
-         'overall_summary': {'avg_cadence': 85.48,
-                             'avg_heart_rate': 0.0,
-                             'avg_power': 179.24,
-                             'avg_resistance': 47.61,
-                             'avg_speed': 20.39,
-                             'cadence': 0.0,
-                             'calories': 496.71,
-                             'distance': 10.19,
-                             'heart_rate': 0.0,
-                             'id': '<some id hash>',
-                             'instant': 1589644336,
-                             'max_cadence': 122.0,
-                             'max_heart_rate': 0.0,
-                             'max_power': 255.8,
-                             'max_resistance': 60.95,
-                             'max_speed': 23.48,
-                             'power': 0.0,
-                             'resistance': 0.0,
-                             'seconds_since_pedaling_start': 0,
-                             'speed': 0.0,
-                             'total_work': 322417.21,
-                             'workout_id': '<some id hash>'},
-         'peloton_id': '<some id hash>',
-         'platform': 'home_bike',
-         'ride': {'captions': ['en-US'],
-                  'class_type_ids': ['<some id hash>'],
-                  'content_format': 'video',
-                  'content_provider': 'peloton',
-                  'description': 'Max out the effectiveness of your training with this '
-                                 'ride. Instructors will expertly guide you through '
-                                 'specific output ranges 1 through 7 to help you build '
-                                 'endurance, strength and speed.',
-                  'difficulty_estimate': 6.3779,
-                  'difficulty_level': None,
-                  'difficulty_rating_avg': 6.3779,
-                  'difficulty_rating_count': 17157,
-                  'duration': 1800,
-                  'equipment_ids': [],
-                  'equipment_tags': [],
-                  'excluded_platforms': [],
-                  'extra_images': [],
-                  'fitness_discipline': 'cycling',
-                  'fitness_discipline_display_name': 'Cycling',
-                  'has_closed_captions': True,
-                  'has_free_mode': False,
-                  'has_pedaling_metrics': True,
-                  'home_peloton_id': '<some id hash>',
-                  'id': '<some id hash>',
-                  'image_url': 'https://s3.amazonaws.com/peloton-ride-images/58aa8ebc7d51d09d6513e1a2fab53c4c62c076c6/img_1580922399_a5f1fd0e3a2e48d38ecdd6a3d874820f.png',
-                  'instructor_id': '<some id hash>',
-                  'is_archived': True,
-                  'is_closed_caption_shown': True,
-                  'is_explicit': False,
-                  'is_live_in_studio_only': False,
-                  'language': 'english',
-                  'length': 1940,
-                  'live_stream_id': '<some id hash>-live',
-                  'live_stream_url': None,
-                  'location': 'nyc',
-                  'metrics': ['heart_rate', 'cadence', 'calories'],
-                  'origin_locale': 'en-US',
-                  'original_air_time': 1580919480,
-                  'overall_estimate': 0.9956,
-                  'overall_rating_avg': 0.9956,
-                  'overall_rating_count': 20737,
-                  'pedaling_duration': 1800,
-                  'pedaling_end_offset': 1860,
-                  'pedaling_start_offset': 60,
-                  'rating': 0,
-                  'ride_type_id': '<some id hash>',
-                  'ride_type_ids': ['<some id hash>'],
-                  'sample_vod_stream_url': None,
-                  'scheduled_start_time': 1580920200,
-                  'series_id': '<some id hash>',
-                  'sold_out': False,
-                  'studio_peloton_id': '<some id hash>',
-                  'title': '30 min Power Zone Endurance Ride',
-                  'total_in_progress_workouts': 0,
-                  'total_ratings': 0,
-                  'total_workouts': 32489,
-                  'vod_stream_id': '<some id hash>-vod',
-                  'vod_stream_url': None},
-         'start_time': 1589642537,
-         'status': 'COMPLETE',
-         'strava_id': None,
-         'timezone': 'America/Los_Angeles',
-         'title': None,
-         'total_leaderboard_users': 31240,
-         'total_work': 322417.21,
-         'user_id': '<some id hash>',
-         'workout_type': 'class'}
-        ```
-        
-        An example of how you may fetch performance data for a ride
-        ```
-        import pprint
-        
-        conn = pylotoncycle.PylotonCycle(username, password)
-        workouts = conn.GetRecentWorkouts(5)
-        for w in workouts:
-            workout_id = w['id']
-            resp = conn.GetWorkoutMetricsById(workout_id)
-            pprint.pprint(resp)
-        
-        ```
-        
-        ## Install
-        This package is available via pip install.
-        ```
-        pip install pylotoncycle
-        ```
-        
-        ## TODO
-        * Lots more to cover. I want to find the right format for pulling in the
-        ride performance data.
-        * Pull in GPS data for outdoor runs
-        
-        ## Note to folks who want to contribute
-        I'm very happy to take pull requests and fix bugs that come up. But, this is definitely a side project for me.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PylotonCycle
+Python Library for getting your Peloton workout data.
+
+## Table of contents
+* [General info](#general-info)
+* [Example Usage](#example-usage)
+
+## General info
+As someone who wants to see my progress over time, I've been wanting a way
+to pull and play with my ride data. However, I'm also cautious about linking
+myself to too many external parties. As I've been playing with other libraries
+out there, I wanted something that was a bit more intuitive and would play
+nicer with the rest of my python code. So, PylotonCycle is born.
+
+## Example Usage
+```
+import pylotoncycle
+
+username = 'your username or email address'
+password = 'your password'
+conn = pylotoncycle.PylotonCycle(username, password)
+workouts = conn.GetRecentWorkouts(5)
+```
+`workouts` is a list of workouts.
+
+An example of a list element
+
+```
+{'achievement_templates': [{'description': 'Awarded for working out with a '
+                                           'friend.',
+                            'id': '<some id hash>',
+                            'image_url': 'https://s3.amazonaws.com/peloton-achievement-images-prod/702495cd985d4791bfd3d25f36e0df72',
+                            'name': 'Dynamic Duo',
+                            'slug': 'two_to_tango'},
+                           {'description': 'Awarded for achieving Silver in '
+                                           'the May Cycling Challenge.',
+                            'id': '<some id hash>',
+                            'image_url': 'https://s3.amazonaws.com/challenges-and-tiers-image-prod/6b772477ccd04f189fba16f2f877faad',
+                            'name': 'May Cycling Challenge',
+                            'slug': 'may_cycling_challenge_silver'}],
+ 'created': 1589642476,
+ 'created_at': 1589642476,
+ 'device_time_created_at': 1589617276,
+ 'device_type': 'home_bike_v1',
+ 'device_type_display_name': 'Bike',
+ 'end_time': 1589644336,
+ 'fitbit_id': None,
+ 'fitness_discipline': 'cycling',
+ 'ftp_info': {'ftp': 111,
+              'ftp_source': 'ftp_workout_source',
+              'ftp_workout_id': '<some id hash>'},
+ 'has_leaderboard_metrics': True,
+ 'has_pedaling_metrics': True,
+ 'id': '<some id hash>',
+ 'instructor_name': 'Matt Wilpers',
+ 'is_total_work_personal_record': False,
+ 'leaderboard_rank': 5015,
+ 'metrics_type': 'cycling',
+ 'name': 'Cycling Workout',
+ 'overall_summary': {'avg_cadence': 85.48,
+                     'avg_heart_rate': 0.0,
+                     'avg_power': 179.24,
+                     'avg_resistance': 47.61,
+                     'avg_speed': 20.39,
+                     'cadence': 0.0,
+                     'calories': 496.71,
+                     'distance': 10.19,
+                     'heart_rate': 0.0,
+                     'id': '<some id hash>',
+                     'instant': 1589644336,
+                     'max_cadence': 122.0,
+                     'max_heart_rate': 0.0,
+                     'max_power': 255.8,
+                     'max_resistance': 60.95,
+                     'max_speed': 23.48,
+                     'power': 0.0,
+                     'resistance': 0.0,
+                     'seconds_since_pedaling_start': 0,
+                     'speed': 0.0,
+                     'total_work': 322417.21,
+                     'workout_id': '<some id hash>'},
+ 'peloton_id': '<some id hash>',
+ 'platform': 'home_bike',
+ 'ride': {'captions': ['en-US'],
+          'class_type_ids': ['<some id hash>'],
+          'content_format': 'video',
+          'content_provider': 'peloton',
+          'description': 'Max out the effectiveness of your training with this '
+                         'ride. Instructors will expertly guide you through '
+                         'specific output ranges 1 through 7 to help you build '
+                         'endurance, strength and speed.',
+          'difficulty_estimate': 6.3779,
+          'difficulty_level': None,
+          'difficulty_rating_avg': 6.3779,
+          'difficulty_rating_count': 17157,
+          'duration': 1800,
+          'equipment_ids': [],
+          'equipment_tags': [],
+          'excluded_platforms': [],
+          'extra_images': [],
+          'fitness_discipline': 'cycling',
+          'fitness_discipline_display_name': 'Cycling',
+          'has_closed_captions': True,
+          'has_free_mode': False,
+          'has_pedaling_metrics': True,
+          'home_peloton_id': '<some id hash>',
+          'id': '<some id hash>',
+          'image_url': 'https://s3.amazonaws.com/peloton-ride-images/58aa8ebc7d51d09d6513e1a2fab53c4c62c076c6/img_1580922399_a5f1fd0e3a2e48d38ecdd6a3d874820f.png',
+          'instructor_id': '<some id hash>',
+          'is_archived': True,
+          'is_closed_caption_shown': True,
+          'is_explicit': False,
+          'is_live_in_studio_only': False,
+          'language': 'english',
+          'length': 1940,
+          'live_stream_id': '<some id hash>-live',
+          'live_stream_url': None,
+          'location': 'nyc',
+          'metrics': ['heart_rate', 'cadence', 'calories'],
+          'origin_locale': 'en-US',
+          'original_air_time': 1580919480,
+          'overall_estimate': 0.9956,
+          'overall_rating_avg': 0.9956,
+          'overall_rating_count': 20737,
+          'pedaling_duration': 1800,
+          'pedaling_end_offset': 1860,
+          'pedaling_start_offset': 60,
+          'rating': 0,
+          'ride_type_id': '<some id hash>',
+          'ride_type_ids': ['<some id hash>'],
+          'sample_vod_stream_url': None,
+          'scheduled_start_time': 1580920200,
+          'series_id': '<some id hash>',
+          'sold_out': False,
+          'studio_peloton_id': '<some id hash>',
+          'title': '30 min Power Zone Endurance Ride',
+          'total_in_progress_workouts': 0,
+          'total_ratings': 0,
+          'total_workouts': 32489,
+          'vod_stream_id': '<some id hash>-vod',
+          'vod_stream_url': None},
+ 'start_time': 1589642537,
+ 'status': 'COMPLETE',
+ 'strava_id': None,
+ 'timezone': 'America/Los_Angeles',
+ 'title': None,
+ 'total_leaderboard_users': 31240,
+ 'total_work': 322417.21,
+ 'user_id': '<some id hash>',
+ 'workout_type': 'class'}
+```
+
+An example of how you may fetch performance data for a ride
+```
+import pprint
+
+conn = pylotoncycle.PylotonCycle(username, password)
+workouts = conn.GetRecentWorkouts(5)
+for w in workouts:
+    workout_id = w['id']
+    resp = conn.GetWorkoutMetricsById(workout_id)
+    pprint.pprint(resp)
+
+```
+
+## Install
+This package is available via pip install.
+```
+pip install pylotoncycle
+```
+
+## TODO
+* Lots more to cover. I want to find the right format for pulling in the
+ride performance data.
+* Pull in GPS data for outdoor runs
+
+## Note to folks who want to contribute
+I'm very happy to take pull requests and fix bugs that come up. But, this is definitely a side project for me.
```

### Comparing `pylotoncycle-0.6.0/README.md` & `pylotoncycle-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pylotoncycle-0.6.0/pylotoncycle/parser.py` & `pylotoncycle-0.8.0/pylotoncycle/parser.py`

 * *Files identical despite different names*

### Comparing `pylotoncycle-0.6.0/pylotoncycle/pylotoncycle.py` & `pylotoncycle-0.8.0/pylotoncycle/pylotoncycle.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,19 @@
         url = "%s/api/me" % self.base_url
         resp = self.s.get(url, timeout=10).json()
         self.username = resp["username"]
         self.userid = resp["id"]
         self.total_workouts = resp["total_workouts"]
         return resp
 
+    def GetSettings(self):
+        url = "%s/api/user/%s/settings" % (self.base_url, self.userid)
+        resp = self.s.get(url, timeout=10).json()
+        return resp
+
     def GetUrl(self, url):
         resp = self.s.get(url, timeout=10).json()
         return resp
 
     def GetWorkoutList(self, num_workouts=None):
         """
         Generally, not intended to call this directly, but
@@ -106,43 +111,46 @@
     def GetRecentWorkouts(self, num_workouts=None):
         workout_list = self.GetWorkoutList(num_workouts)
         workouts_info = []
 
         for i in workout_list:
             workout_id = i["id"]
 
-            resp_summary = self.GetWorkoutSummaryById(workout_id)
+            performance_graph = self.GetWorkoutMetricsById(workout_id)
             resp_workout = self.GetWorkoutById(workout_id)
 
             if "instructor_id" in resp_workout["ride"]:
                 instructor_id = resp_workout["ride"]["instructor_id"]
                 resp_instructor = self.GetInstructorById(instructor_id)
             elif "instructor" in resp_workout["ride"]:
                 resp_instructor = {
                     "name": resp_workout["ride"]["instructor"]["name"]
                 }
 
-            resp_workout["overall_summary"] = resp_summary
+            resp_workout["performance_graph"] = performance_graph
             try:
                 resp_workout["instructor_name"] = resp_instructor["name"]
             except KeyError:
                 resp_workout["instructor_name"] = None
             workouts_info.append(resp_workout)
         return workouts_info
 
     def GetWorkoutSummaryById(self, workout_id):
         url = "%s/api/workout/%s" % (self.base_url, workout_id)
         resp = self.GetUrl(url)
         return resp
 
     def GetWorkoutMetricsById(self, workout_id, frequency=50):
-        url = "%s/api/workout/%s/performance_graph?every_n=%s" % (
+        performance_frequency = (
+            "?every_n=%s" % (frequency) if frequency > 0 else ""
+        )
+        url = "%s/api/workout/%s/performance_graph%s" % (
             self.base_url,
             workout_id,
-            frequency,
+            performance_frequency,
         )
         resp = self.GetUrl(url)
         return resp
 
     def GetWorkoutById(self, workout_id):
         url = "%s/api/workout/%s" % (self.base_url, workout_id)
         resp = self.GetUrl(url)
```

### Comparing `pylotoncycle-0.6.0/pylotoncycle.egg-info/PKG-INFO` & `pylotoncycle-0.8.0/pylotoncycle.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,191 @@
 Metadata-Version: 2.1
 Name: pylotoncycle
-Version: 0.6.0
+Version: 0.8.0
 Summary: Module to access your Peloton workout data
 Home-page: https://github.com/justmedude/pylotoncycle
 Author: Vikram Adukia
 Author-email: github@fireitup.net
 License: BSD
-Description: # PylotonCycle
-        Python Library for getting your Peloton workout data.
-        
-        ## Table of contents
-        * [General info](#general-info)
-        * [Example Usage](#example-usage)
-        
-        ## General info
-        As someone who wants to see my progress over time, I've been wanting a way
-        to pull and play with my ride data. However, I'm also cautious about linking
-        myself to too many external parties. As I've been playing with other libraries
-        out there, I wanted something that was a bit more intuitive and would play
-        nicer with the rest of my python code. So, PylotonCycle is born.
-        
-        ## Example Usage
-        ```
-        import pylotoncycle
-        
-        username = 'your username or email address'
-        password = 'your password'
-        conn = pylotoncycle.PylotonCycle(username, password)
-        workouts = conn.GetRecentWorkouts(5)
-        ```
-        `workouts` is a list of workouts.
-        
-        An example of a list element
-        
-        ```
-        {'achievement_templates': [{'description': 'Awarded for working out with a '
-                                                   'friend.',
-                                    'id': '<some id hash>',
-                                    'image_url': 'https://s3.amazonaws.com/peloton-achievement-images-prod/702495cd985d4791bfd3d25f36e0df72',
-                                    'name': 'Dynamic Duo',
-                                    'slug': 'two_to_tango'},
-                                   {'description': 'Awarded for achieving Silver in '
-                                                   'the May Cycling Challenge.',
-                                    'id': '<some id hash>',
-                                    'image_url': 'https://s3.amazonaws.com/challenges-and-tiers-image-prod/6b772477ccd04f189fba16f2f877faad',
-                                    'name': 'May Cycling Challenge',
-                                    'slug': 'may_cycling_challenge_silver'}],
-         'created': 1589642476,
-         'created_at': 1589642476,
-         'device_time_created_at': 1589617276,
-         'device_type': 'home_bike_v1',
-         'device_type_display_name': 'Bike',
-         'end_time': 1589644336,
-         'fitbit_id': None,
-         'fitness_discipline': 'cycling',
-         'ftp_info': {'ftp': 111,
-                      'ftp_source': 'ftp_workout_source',
-                      'ftp_workout_id': '<some id hash>'},
-         'has_leaderboard_metrics': True,
-         'has_pedaling_metrics': True,
-         'id': '<some id hash>',
-         'instructor_name': 'Matt Wilpers',
-         'is_total_work_personal_record': False,
-         'leaderboard_rank': 5015,
-         'metrics_type': 'cycling',
-         'name': 'Cycling Workout',
-         'overall_summary': {'avg_cadence': 85.48,
-                             'avg_heart_rate': 0.0,
-                             'avg_power': 179.24,
-                             'avg_resistance': 47.61,
-                             'avg_speed': 20.39,
-                             'cadence': 0.0,
-                             'calories': 496.71,
-                             'distance': 10.19,
-                             'heart_rate': 0.0,
-                             'id': '<some id hash>',
-                             'instant': 1589644336,
-                             'max_cadence': 122.0,
-                             'max_heart_rate': 0.0,
-                             'max_power': 255.8,
-                             'max_resistance': 60.95,
-                             'max_speed': 23.48,
-                             'power': 0.0,
-                             'resistance': 0.0,
-                             'seconds_since_pedaling_start': 0,
-                             'speed': 0.0,
-                             'total_work': 322417.21,
-                             'workout_id': '<some id hash>'},
-         'peloton_id': '<some id hash>',
-         'platform': 'home_bike',
-         'ride': {'captions': ['en-US'],
-                  'class_type_ids': ['<some id hash>'],
-                  'content_format': 'video',
-                  'content_provider': 'peloton',
-                  'description': 'Max out the effectiveness of your training with this '
-                                 'ride. Instructors will expertly guide you through '
-                                 'specific output ranges 1 through 7 to help you build '
-                                 'endurance, strength and speed.',
-                  'difficulty_estimate': 6.3779,
-                  'difficulty_level': None,
-                  'difficulty_rating_avg': 6.3779,
-                  'difficulty_rating_count': 17157,
-                  'duration': 1800,
-                  'equipment_ids': [],
-                  'equipment_tags': [],
-                  'excluded_platforms': [],
-                  'extra_images': [],
-                  'fitness_discipline': 'cycling',
-                  'fitness_discipline_display_name': 'Cycling',
-                  'has_closed_captions': True,
-                  'has_free_mode': False,
-                  'has_pedaling_metrics': True,
-                  'home_peloton_id': '<some id hash>',
-                  'id': '<some id hash>',
-                  'image_url': 'https://s3.amazonaws.com/peloton-ride-images/58aa8ebc7d51d09d6513e1a2fab53c4c62c076c6/img_1580922399_a5f1fd0e3a2e48d38ecdd6a3d874820f.png',
-                  'instructor_id': '<some id hash>',
-                  'is_archived': True,
-                  'is_closed_caption_shown': True,
-                  'is_explicit': False,
-                  'is_live_in_studio_only': False,
-                  'language': 'english',
-                  'length': 1940,
-                  'live_stream_id': '<some id hash>-live',
-                  'live_stream_url': None,
-                  'location': 'nyc',
-                  'metrics': ['heart_rate', 'cadence', 'calories'],
-                  'origin_locale': 'en-US',
-                  'original_air_time': 1580919480,
-                  'overall_estimate': 0.9956,
-                  'overall_rating_avg': 0.9956,
-                  'overall_rating_count': 20737,
-                  'pedaling_duration': 1800,
-                  'pedaling_end_offset': 1860,
-                  'pedaling_start_offset': 60,
-                  'rating': 0,
-                  'ride_type_id': '<some id hash>',
-                  'ride_type_ids': ['<some id hash>'],
-                  'sample_vod_stream_url': None,
-                  'scheduled_start_time': 1580920200,
-                  'series_id': '<some id hash>',
-                  'sold_out': False,
-                  'studio_peloton_id': '<some id hash>',
-                  'title': '30 min Power Zone Endurance Ride',
-                  'total_in_progress_workouts': 0,
-                  'total_ratings': 0,
-                  'total_workouts': 32489,
-                  'vod_stream_id': '<some id hash>-vod',
-                  'vod_stream_url': None},
-         'start_time': 1589642537,
-         'status': 'COMPLETE',
-         'strava_id': None,
-         'timezone': 'America/Los_Angeles',
-         'title': None,
-         'total_leaderboard_users': 31240,
-         'total_work': 322417.21,
-         'user_id': '<some id hash>',
-         'workout_type': 'class'}
-        ```
-        
-        An example of how you may fetch performance data for a ride
-        ```
-        import pprint
-        
-        conn = pylotoncycle.PylotonCycle(username, password)
-        workouts = conn.GetRecentWorkouts(5)
-        for w in workouts:
-            workout_id = w['id']
-            resp = conn.GetWorkoutMetricsById(workout_id)
-            pprint.pprint(resp)
-        
-        ```
-        
-        ## Install
-        This package is available via pip install.
-        ```
-        pip install pylotoncycle
-        ```
-        
-        ## TODO
-        * Lots more to cover. I want to find the right format for pulling in the
-        ride performance data.
-        * Pull in GPS data for outdoor runs
-        
-        ## Note to folks who want to contribute
-        I'm very happy to take pull requests and fix bugs that come up. But, this is definitely a side project for me.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PylotonCycle
+Python Library for getting your Peloton workout data.
+
+## Table of contents
+* [General info](#general-info)
+* [Example Usage](#example-usage)
+
+## General info
+As someone who wants to see my progress over time, I've been wanting a way
+to pull and play with my ride data. However, I'm also cautious about linking
+myself to too many external parties. As I've been playing with other libraries
+out there, I wanted something that was a bit more intuitive and would play
+nicer with the rest of my python code. So, PylotonCycle is born.
+
+## Example Usage
+```
+import pylotoncycle
+
+username = 'your username or email address'
+password = 'your password'
+conn = pylotoncycle.PylotonCycle(username, password)
+workouts = conn.GetRecentWorkouts(5)
+```
+`workouts` is a list of workouts.
+
+An example of a list element
+
+```
+{'achievement_templates': [{'description': 'Awarded for working out with a '
+                                           'friend.',
+                            'id': '<some id hash>',
+                            'image_url': 'https://s3.amazonaws.com/peloton-achievement-images-prod/702495cd985d4791bfd3d25f36e0df72',
+                            'name': 'Dynamic Duo',
+                            'slug': 'two_to_tango'},
+                           {'description': 'Awarded for achieving Silver in '
+                                           'the May Cycling Challenge.',
+                            'id': '<some id hash>',
+                            'image_url': 'https://s3.amazonaws.com/challenges-and-tiers-image-prod/6b772477ccd04f189fba16f2f877faad',
+                            'name': 'May Cycling Challenge',
+                            'slug': 'may_cycling_challenge_silver'}],
+ 'created': 1589642476,
+ 'created_at': 1589642476,
+ 'device_time_created_at': 1589617276,
+ 'device_type': 'home_bike_v1',
+ 'device_type_display_name': 'Bike',
+ 'end_time': 1589644336,
+ 'fitbit_id': None,
+ 'fitness_discipline': 'cycling',
+ 'ftp_info': {'ftp': 111,
+              'ftp_source': 'ftp_workout_source',
+              'ftp_workout_id': '<some id hash>'},
+ 'has_leaderboard_metrics': True,
+ 'has_pedaling_metrics': True,
+ 'id': '<some id hash>',
+ 'instructor_name': 'Matt Wilpers',
+ 'is_total_work_personal_record': False,
+ 'leaderboard_rank': 5015,
+ 'metrics_type': 'cycling',
+ 'name': 'Cycling Workout',
+ 'overall_summary': {'avg_cadence': 85.48,
+                     'avg_heart_rate': 0.0,
+                     'avg_power': 179.24,
+                     'avg_resistance': 47.61,
+                     'avg_speed': 20.39,
+                     'cadence': 0.0,
+                     'calories': 496.71,
+                     'distance': 10.19,
+                     'heart_rate': 0.0,
+                     'id': '<some id hash>',
+                     'instant': 1589644336,
+                     'max_cadence': 122.0,
+                     'max_heart_rate': 0.0,
+                     'max_power': 255.8,
+                     'max_resistance': 60.95,
+                     'max_speed': 23.48,
+                     'power': 0.0,
+                     'resistance': 0.0,
+                     'seconds_since_pedaling_start': 0,
+                     'speed': 0.0,
+                     'total_work': 322417.21,
+                     'workout_id': '<some id hash>'},
+ 'peloton_id': '<some id hash>',
+ 'platform': 'home_bike',
+ 'ride': {'captions': ['en-US'],
+          'class_type_ids': ['<some id hash>'],
+          'content_format': 'video',
+          'content_provider': 'peloton',
+          'description': 'Max out the effectiveness of your training with this '
+                         'ride. Instructors will expertly guide you through '
+                         'specific output ranges 1 through 7 to help you build '
+                         'endurance, strength and speed.',
+          'difficulty_estimate': 6.3779,
+          'difficulty_level': None,
+          'difficulty_rating_avg': 6.3779,
+          'difficulty_rating_count': 17157,
+          'duration': 1800,
+          'equipment_ids': [],
+          'equipment_tags': [],
+          'excluded_platforms': [],
+          'extra_images': [],
+          'fitness_discipline': 'cycling',
+          'fitness_discipline_display_name': 'Cycling',
+          'has_closed_captions': True,
+          'has_free_mode': False,
+          'has_pedaling_metrics': True,
+          'home_peloton_id': '<some id hash>',
+          'id': '<some id hash>',
+          'image_url': 'https://s3.amazonaws.com/peloton-ride-images/58aa8ebc7d51d09d6513e1a2fab53c4c62c076c6/img_1580922399_a5f1fd0e3a2e48d38ecdd6a3d874820f.png',
+          'instructor_id': '<some id hash>',
+          'is_archived': True,
+          'is_closed_caption_shown': True,
+          'is_explicit': False,
+          'is_live_in_studio_only': False,
+          'language': 'english',
+          'length': 1940,
+          'live_stream_id': '<some id hash>-live',
+          'live_stream_url': None,
+          'location': 'nyc',
+          'metrics': ['heart_rate', 'cadence', 'calories'],
+          'origin_locale': 'en-US',
+          'original_air_time': 1580919480,
+          'overall_estimate': 0.9956,
+          'overall_rating_avg': 0.9956,
+          'overall_rating_count': 20737,
+          'pedaling_duration': 1800,
+          'pedaling_end_offset': 1860,
+          'pedaling_start_offset': 60,
+          'rating': 0,
+          'ride_type_id': '<some id hash>',
+          'ride_type_ids': ['<some id hash>'],
+          'sample_vod_stream_url': None,
+          'scheduled_start_time': 1580920200,
+          'series_id': '<some id hash>',
+          'sold_out': False,
+          'studio_peloton_id': '<some id hash>',
+          'title': '30 min Power Zone Endurance Ride',
+          'total_in_progress_workouts': 0,
+          'total_ratings': 0,
+          'total_workouts': 32489,
+          'vod_stream_id': '<some id hash>-vod',
+          'vod_stream_url': None},
+ 'start_time': 1589642537,
+ 'status': 'COMPLETE',
+ 'strava_id': None,
+ 'timezone': 'America/Los_Angeles',
+ 'title': None,
+ 'total_leaderboard_users': 31240,
+ 'total_work': 322417.21,
+ 'user_id': '<some id hash>',
+ 'workout_type': 'class'}
+```
+
+An example of how you may fetch performance data for a ride
+```
+import pprint
+
+conn = pylotoncycle.PylotonCycle(username, password)
+workouts = conn.GetRecentWorkouts(5)
+for w in workouts:
+    workout_id = w['id']
+    resp = conn.GetWorkoutMetricsById(workout_id)
+    pprint.pprint(resp)
+
+```
+
+## Install
+This package is available via pip install.
+```
+pip install pylotoncycle
+```
+
+## TODO
+* Lots more to cover. I want to find the right format for pulling in the
+ride performance data.
+* Pull in GPS data for outdoor runs
+
+## Note to folks who want to contribute
+I'm very happy to take pull requests and fix bugs that come up. But, this is definitely a side project for me.
```

### Comparing `pylotoncycle-0.6.0/setup.py` & `pylotoncycle-0.8.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pylotoncycle",
-    version="0.6.0",
+    version="0.8.0",
     description="Module to access your Peloton workout data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/justmedude/pylotoncycle",
     author="Vikram Adukia",
     author_email="github@fireitup.net",
     license="BSD",
```

