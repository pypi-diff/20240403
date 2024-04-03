# Comparing `tmp/sentralify-1.2.1.tar.gz` & `tmp/sentralify-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentralify-1.2.1.tar", last modified: Wed Mar 20 07:22:06 2024, max compression
+gzip compressed data, was "sentralify-1.2.2.tar", last modified: Wed Apr  3 00:07:20 2024, max compression
```

## Comparing `sentralify-1.2.1.tar` & `sentralify-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-03-20 07:22:06.887412 sentralify-1.2.1/
--rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.1/LICENSE
--rw-r--r--   0 James     (1000) James     (1000)    55549 2024-03-20 07:22:06.887412 sentralify-1.2.1/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)    14342 2024-03-20 07:22:05.000000 sentralify-1.2.1/README.md
--rw-r--r--   0 James     (1000) James     (1000)      884 2024-03-20 07:22:02.000000 sentralify-1.2.1/pyproject.toml
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-03-20 07:22:06.887412 sentralify-1.2.1/setup.cfg
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.1/setup.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-03-20 07:22:06.887412 sentralify-1.2.1/src/
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-03-20 07:22:06.887412 sentralify-1.2.1/src/sentralify/
--rw-rw-r--   0 James     (1000) James     (1000)     4049 2024-03-20 07:22:05.000000 sentralify-1.2.1/src/sentralify/__init__.py
--rw-r--r--   0 James     (1000) James     (1000)    15726 2024-03-20 07:22:05.000000 sentralify-1.2.1/src/sentralify/generators.py
--rw-r--r--   0 James     (1000) James     (1000)    12481 2024-03-20 07:22:05.000000 sentralify-1.2.1/src/sentralify/scrapers.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-03-20 07:22:06.887412 sentralify-1.2.1/src/sentralify.egg-info/
--rw-r--r--   0 James     (1000) James     (1000)    55549 2024-03-20 07:22:06.000000 sentralify-1.2.1/src/sentralify.egg-info/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)      313 2024-03-20 07:22:06.000000 sentralify-1.2.1/src/sentralify.egg-info/SOURCES.txt
--rw-r--r--   0 James     (1000) James     (1000)        1 2024-03-20 07:22:06.000000 sentralify-1.2.1/src/sentralify.egg-info/dependency_links.txt
--rw-r--r--   0 James     (1000) James     (1000)       97 2024-03-20 07:22:06.000000 sentralify-1.2.1/src/sentralify.egg-info/requires.txt
--rw-r--r--   0 James     (1000) James     (1000)       11 2024-03-20 07:22:06.000000 sentralify-1.2.1/src/sentralify.egg-info/top_level.txt
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 00:07:20.738993 sentralify-1.2.2/
+-rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.2/LICENSE
+-rw-r--r--   0 James     (1000) James     (1000)    55567 2024-04-03 00:07:20.738993 sentralify-1.2.2/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)    14360 2024-04-03 00:07:19.000000 sentralify-1.2.2/README.md
+-rw-r--r--   0 James     (1000) James     (1000)      884 2024-04-03 00:06:23.000000 sentralify-1.2.2/pyproject.toml
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-04-03 00:07:20.738993 sentralify-1.2.2/setup.cfg
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.2/setup.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 00:07:20.735659 sentralify-1.2.2/src/
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 00:07:20.738993 sentralify-1.2.2/src/sentralify/
+-rw-r--r--   0 James     (1000) James     (1000)     4032 2024-04-03 00:07:19.000000 sentralify-1.2.2/src/sentralify/__init__.py
+-rw-r--r--   0 James     (1000) James     (1000)    18560 2024-04-03 00:07:19.000000 sentralify-1.2.2/src/sentralify/generators.py
+-rw-r--r--   0 James     (1000) James     (1000)    12503 2024-04-03 00:07:19.000000 sentralify-1.2.2/src/sentralify/scrapers.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-03 00:07:20.738993 sentralify-1.2.2/src/sentralify.egg-info/
+-rw-r--r--   0 James     (1000) James     (1000)    55567 2024-04-03 00:07:20.000000 sentralify-1.2.2/src/sentralify.egg-info/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)      313 2024-04-03 00:07:20.000000 sentralify-1.2.2/src/sentralify.egg-info/SOURCES.txt
+-rw-r--r--   0 James     (1000) James     (1000)        1 2024-04-03 00:07:20.000000 sentralify-1.2.2/src/sentralify.egg-info/dependency_links.txt
+-rw-r--r--   0 James     (1000) James     (1000)       97 2024-04-03 00:07:20.000000 sentralify-1.2.2/src/sentralify.egg-info/requires.txt
+-rw-r--r--   0 James     (1000) James     (1000)       11 2024-04-03 00:07:20.000000 sentralify-1.2.2/src/sentralify.egg-info/top_level.txt
```

### Comparing `sentralify-1.2.1/LICENSE` & `sentralify-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.1/PKG-INFO` & `sentralify-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.1
+Version: 1.2.2
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -958,15 +958,15 @@
 }
 
 ```
 Yes I'm doing Bowling for sport, yes all my friends are doing it too, yes, I'm a coder, so no, I do not like doing proper sport.
 This is a lot of data, but having it nicely formatted and laid out here, should make it easier to understand. If I wanted to access the third class's teacher, then I would use ```sentralify(config)['student_details']['classes'][2]['teacher']```
 
 #### Attendance
-Okay, the attendance is really long, but I did it for you, you're welcome!
+Okay, the attendance (added in v1.2.0) is really long, but I did it for you, you're welcome!
 Below is a small snippet of one day of data
 ```
 [
     [
         [
             {
                 "date": "Mon Jan 29 00:00:00 2024",
```

### Comparing `sentralify-1.2.1/README.md` & `sentralify-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
 }
 
 ```
 Yes I'm doing Bowling for sport, yes all my friends are doing it too, yes, I'm a coder, so no, I do not like doing proper sport.
 This is a lot of data, but having it nicely formatted and laid out here, should make it easier to understand. If I wanted to access the third class's teacher, then I would use ```sentralify(config)['student_details']['classes'][2]['teacher']```
 
 #### Attendance
-Okay, the attendance is really long, but I did it for you, you're welcome!
+Okay, the attendance (added in v1.2.0) is really long, but I did it for you, you're welcome!
 Below is a small snippet of one day of data
 ```
 [
     [
         [
             {
                 "date": "Mon Jan 29 00:00:00 2024",
```

### Comparing `sentralify-1.2.1/pyproject.toml` & `sentralify-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentralify"
-version = "1.2.1"
+version = "1.2.2"
 description = "Scrape Sentral data and use it!"
 readme = "README.md"
 authors = [{ name = "mario872", email = "jamesaglynn10@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sentralify-1.2.1/src/sentralify/__init__.py` & `sentralify-1.2.2/src/sentralify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     data['student_details'] = Sentral.generate_student_details(student_details) # Save the formatted student details in the return data
         
     # A bunch of if blocks to determine whether or not to scrape parts of sentral
     if notices:
         notices = Sentral.generate_notices(scraper.save_notices(page))
         data['notices'] = notices
     if timetable:
-        timetable = Sentral.generate_timetable(scraper.save_timetable(page), daily_timetable)
+        timetable = Sentral.generate_timetable(scraper.save_timetable(page))
         data['timetable'] = timetable
     if calendar:
         calendar = Sentral.generate_calendar(scraper.save_calendar(page))
         data['calendar'] = calendar
         
     browser.close() # Close the browser, as  our work is done
     p.stop() # Stopping playwright instance
```

### Comparing `sentralify-1.2.1/src/sentralify/scrapers.py` & `sentralify-1.2.2/src/sentralify/scrapers.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         # I mean, changing the frontend so that most people agree that it's worse, probably just to break a python package that takes data
         # from Sentral made by a bunch of high schoolers (https://github.com/J-J-B-J/get-sentral [Great project, this was made because that got broken by the update]) is enough work anyway, right?
         
         # Oh man, that was a really long rant.
         # Anyway, this just scrapes the page for the json, and converts it to a dictionary that python can acess.
         # I found this url after watching some kids at my school go into the network tab in dev tools in Chrome, and look at what Sentral was accessing. Thank you!
         
-        page.goto(f"https://{self.config['base_url']}.sentral.com.au/s-Y7eXkn/portal2/timetable/getFullTimetable/{str(self.student_id)}")
+        page.goto(f"https://{self.config['base_url']}.sentral.com.au/s-Y7eXkn/portal2/timetable/getFullTimetableInDates/{str(self.student_id)}/undefined/true")
         return json.loads(BeautifulSoup(page.content(), "lxml").text)
 
     def save_notices(self, page):
         """
         Saves the notices page and returns the html
 
         Args:
```

### Comparing `sentralify-1.2.1/src/sentralify.egg-info/PKG-INFO` & `sentralify-1.2.2/src/sentralify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.1
+Version: 1.2.2
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -958,15 +958,15 @@
 }
 
 ```
 Yes I'm doing Bowling for sport, yes all my friends are doing it too, yes, I'm a coder, so no, I do not like doing proper sport.
 This is a lot of data, but having it nicely formatted and laid out here, should make it easier to understand. If I wanted to access the third class's teacher, then I would use ```sentralify(config)['student_details']['classes'][2]['teacher']```
 
 #### Attendance
-Okay, the attendance is really long, but I did it for you, you're welcome!
+Okay, the attendance (added in v1.2.0) is really long, but I did it for you, you're welcome!
 Below is a small snippet of one day of data
 ```
 [
     [
         [
             {
                 "date": "Mon Jan 29 00:00:00 2024",
```

