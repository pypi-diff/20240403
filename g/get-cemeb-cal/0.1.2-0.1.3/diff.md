# Comparing `tmp/get_cemeb_cal-0.1.2.tar.gz` & `tmp/get_cemeb_cal-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_cemeb_cal-0.1.2.tar", last modified: Wed Mar 27 16:10:34 2024, max compression
+gzip compressed data, was "get_cemeb_cal-0.1.3.tar", last modified: Fri Mar 29 10:45:21 2024, max compression
```

## Comparing `get_cemeb_cal-0.1.2.tar` & `get_cemeb_cal-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-27 16:10:34.078590 get_cemeb_cal-0.1.2/
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)    35149 2024-03-26 13:14:58.000000 get_cemeb_cal-0.1.2/COPYING
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)     2391 2024-03-27 16:10:34.078590 get_cemeb_cal-0.1.2/PKG-INFO
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)     1518 2024-03-27 12:43:33.000000 get_cemeb_cal-0.1.2/README.md
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)      988 2024-03-27 16:10:14.000000 get_cemeb_cal-0.1.2/pyproject.toml
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)       38 2024-03-27 16:10:34.078590 get_cemeb_cal-0.1.2/setup.cfg
-drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-27 16:10:34.075256 get_cemeb_cal-0.1.2/src/
-drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-27 16:10:34.075256 get_cemeb_cal-0.1.2/src/get_cemeb_cal/
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)      754 2024-03-27 09:50:48.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal/__init__.py
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)     9460 2024-03-27 16:06:28.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal/__main__.py
-drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-27 16:10:34.078590 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)     2391 2024-03-27 16:10:34.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/PKG-INFO
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)      340 2024-03-27 16:10:34.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/SOURCES.txt
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)        1 2024-03-27 16:10:34.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/dependency_links.txt
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)       62 2024-03-27 16:10:34.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/entry_points.txt
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)       59 2024-03-27 16:10:34.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/requires.txt
--rw-r--r--   0 rwolff    (1000) rwolff    (1001)       14 2024-03-27 16:10:34.000000 get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/top_level.txt
+drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-29 10:45:21.778768 get_cemeb_cal-0.1.3/
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)    35149 2024-03-26 13:14:58.000000 get_cemeb_cal-0.1.3/COPYING
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)     2391 2024-03-29 10:45:21.778768 get_cemeb_cal-0.1.3/PKG-INFO
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)     1518 2024-03-27 12:43:33.000000 get_cemeb_cal-0.1.3/README.md
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)      988 2024-03-29 10:44:54.000000 get_cemeb_cal-0.1.3/pyproject.toml
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)       38 2024-03-29 10:45:21.778768 get_cemeb_cal-0.1.3/setup.cfg
+drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-29 10:45:21.775435 get_cemeb_cal-0.1.3/src/
+drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-29 10:45:21.775435 get_cemeb_cal-0.1.3/src/get_cemeb_cal/
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)      754 2024-03-27 09:50:48.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal/__init__.py
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)    10367 2024-03-29 10:42:18.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal/__main__.py
+drwxr-xr-x   0 rwolff    (1000) rwolff    (1001)        0 2024-03-29 10:45:21.778768 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)     2391 2024-03-29 10:45:21.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/PKG-INFO
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)      340 2024-03-29 10:45:21.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/SOURCES.txt
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)        1 2024-03-29 10:45:21.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/dependency_links.txt
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)       62 2024-03-29 10:45:21.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/entry_points.txt
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)       59 2024-03-29 10:45:21.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/requires.txt
+-rw-r--r--   0 rwolff    (1000) rwolff    (1001)       14 2024-03-29 10:45:21.000000 get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/top_level.txt
```

### Comparing `get_cemeb_cal-0.1.2/COPYING` & `get_cemeb_cal-0.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `get_cemeb_cal-0.1.2/PKG-INFO` & `get_cemeb_cal-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_cemeb_cal
-Version: 0.1.2
+Version: 0.1.3
 Summary: Get calendar from CeMEB
 Author-email: Robert Wolff <mahlzahn@posteo.de>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Source, https://codeberg.org/mahlzahn/get_cemeb_cal
 Project-URL: Issues, https://codeberg.org/mahlzahn/get_cemeb_cal/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `get_cemeb_cal-0.1.2/README.md` & `get_cemeb_cal-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `get_cemeb_cal-0.1.2/pyproject.toml` & `get_cemeb_cal-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "get_cemeb_cal"
-version = "0.1.2"
+version = "0.1.3"
 description = "Get calendar from CeMEB"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "beautifulsoup4",
     "icalendar",
     "lxml",
```

### Comparing `get_cemeb_cal-0.1.2/src/get_cemeb_cal/__init__.py` & `get_cemeb_cal-0.1.3/src/get_cemeb_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `get_cemeb_cal-0.1.2/src/get_cemeb_cal/__main__.py` & `get_cemeb_cal-0.1.3/src/get_cemeb_cal/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,17 +45,16 @@
                         help='date to which search for in form of d/m/Y')
     parser.add_argument('-d', '--duration', default=90,
                         help='default event duration in minutes')
     parser.add_argument('-i', '--input', type=argparse.FileType('r'),
                         help='input icalendar file, if given only new events will be added')
     parser.add_argument('-o', '--output',
                         help='output icalendar file instead of stdout')
-    #TODO parse content of pages from event URL
-    #parser.add_argument('-f', '--full',
-    #                    help='obtain full event description (leads to one request per event!)')
+    parser.add_argument('-F', '--full', action='store_true',
+                        help='obtain full event description (leads to one request per event!)')
     group = parser.add_mutually_exclusive_group()
     group.add_argument('--only-SEEM', action='store_true',
                        help='search only SEEM events')
     group.add_argument('--only-regional', action='store_true',
                        help='search only regional events')
     group.add_argument('--only-national-international', action='store_true',
                        help='search only national and international events')
@@ -107,29 +106,37 @@
             for page in range(1, int(m.groups()[0]) + 1):
                 params['page'] = page
                 r = s.get(url, params=params)
                 if r.ok:
                     pages.append(r.text)
                 else:
                     raise RuntimeError('Request was not successful')
-    events = []
-    for page in pages:
-        events += get_events(page, base_url=base_url)
+        events = []
+        for page in pages:
+            events_page = get_events(page, base_url=base_url)
+            if args.full:
+                for event in events_page:
+                    r = s.get(event.url)
+                    if r.ok:
+                        event.description = get_event_description(r.text)
+            events += events_page
     vevents = get_vevents(events, base_url=base_url, default_duration=args.duration)
     for vevent in vevents:
         cal.add_component(vevent)
     if args.output:
         with open(args.output, 'wb') as f:
             f.write(cal.to_ical())
     else:
         print(cal.to_ical().decode())
 
+
 class Event(argparse.Namespace):
     ...
 
+
 def get_events(page, base_url):
     body = bs4.BeautifulSoup(page, features='lxml').body
     agenda = body.find_all(
             lambda tag: 
             tag.name == 'div'
             and tag.has_attr('class')
             and 'view-agenda' in tag['class'])[-1]
@@ -175,20 +182,21 @@
             hour, minute = m.groups()
             hour = int(hour)
             minute = int(minute)
             location = location[m.end():]
         else:
             hour = None
             minute = None
-        abstract = event_raw.find(
+        description = event_raw.find(
                 lambda tag:
                 tag.name == 'span'
                 and tag.has_attr('class')
-                and 'resume' in tag['class']).contents
-        abstract = ''.join(str(a) for a in abstract)
+                and 'resume' in tag['class'])
+        if description:
+            description = description.get_text().strip()
         try:
             image = event_raw.find(
                     lambda tag:
                     tag.name == 'div'
                     and tag.has_attr('class')
                     and 'visuel' in tag['class']).find('img')['src']
         except:
@@ -198,20 +206,40 @@
                 url=url,
                 year=year,
                 day=day,
                 month=month,
                 hour=hour,
                 minute=minute,
                 location=location,
-                abstract=abstract,
+                description=description,
                 image=image,
                 )
         events.append(event)
     return events
 
+
+def get_event_description(page):
+    body = bs4.BeautifulSoup(page, features='lxml').body
+    content = body.find(
+            lambda tag:
+            tag.name == 'div'
+            and tag.has_attr('class')
+            and 'agenda_content' in tag['class'])
+    description = content.get_text().strip()
+    contact = body.find(
+            lambda tag:
+            tag.name == 'div'
+            and tag.has_attr('class')
+            and 'field-name-field-agenda-contact' in tag['class'])
+    if contact:
+        description += '\n' + contact.get_text().strip()
+    description = re.sub('\s*(\s)', '\\1', description)
+    return description
+
+
 def get_vevents(events, base_url, default_duration=90):
     dtstamp = datetime.datetime.utcnow().replace(microsecond=0)
     tzinfo = zoneinfo.ZoneInfo('Europe/Paris')
     vevents = []
     for i, event in enumerate(events):
         vevent = icalendar.Event()
         vevent.add('dtstamp', dtstamp)
@@ -230,15 +258,15 @@
                                                     event.hour,
                                                     event.minute,
                                                     tzinfo=tzinfo))
             vevent.add('duration', datetime.timedelta(minutes=default_duration))
         if event.image:
             vevent.add('attach', event.image, {'value': 'URI'})
         vevent.add('source', base_url, {'value': 'URI'})
-        vevent.add('description', event.abstract)
+        vevent.add('description', event.description)
         vevent.add('location', event.location)
         vevent.add('summary', event.title)
         vevent.add('url', event.url, {'value': 'URI'})
         vevents.append(vevent)
     return vevents
 
 if __name__ == "__main__":
```

### Comparing `get_cemeb_cal-0.1.2/src/get_cemeb_cal.egg-info/PKG-INFO` & `get_cemeb_cal-0.1.3/src/get_cemeb_cal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_cemeb_cal
-Version: 0.1.2
+Version: 0.1.3
 Summary: Get calendar from CeMEB
 Author-email: Robert Wolff <mahlzahn@posteo.de>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Source, https://codeberg.org/mahlzahn/get_cemeb_cal
 Project-URL: Issues, https://codeberg.org/mahlzahn/get_cemeb_cal/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

