# Comparing `tmp/recurring_ical_events-2.2.0.tar.gz` & `tmp/recurring_ical_events-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurring_ical_events-2.2.0.tar", last modified: Sat Mar 30 16:55:33 2024, max compression
+gzip compressed data, was "recurring_ical_events-2.2.1.tar", last modified: Wed Apr  3 10:47:37 2024, max compression
```

## Comparing `recurring_ical_events-2.2.0.tar` & `recurring_ical_events-2.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:55:33.287437 recurring_ical_events-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-03-30 16:55:33.287437 recurring_ical_events-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:55:33.287437 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-03-30 16:55:33.000000 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-30 16:55:33.000000 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:55:33.000000 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-30 16:55:33.000000 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 16:55:33.000000 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:55:33.000000 recurring_ical_events-2.2.0/recurring_ical_events.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/recurring_ical_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 16:55:33.287437 recurring_ical_events-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-30 16:55:24.000000 recurring_ical_events-2.2.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:37.398185 recurring_ical_events-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19850 2024-04-03 10:47:37.398185 recurring_ical_events-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18734 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:37.398185 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19850 2024-04-03 10:47:37.000000 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 10:47:37.000000 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:47:37.000000 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 10:47:37.000000 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 10:47:37.000000 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:47:37.000000 recurring_ical_events-2.2.1/recurring_ical_events.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    28597 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/recurring_ical_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:47:37.398185 recurring_ical_events-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 10:47:28.000000 recurring_ical_events-2.2.1/test-requirements.txt
```

### Comparing `recurring_ical_events-2.2.0/LICENSE` & `recurring_ical_events-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recurring_ical_events-2.2.0/PKG-INFO` & `recurring_ical_events-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurring_ical_events
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python module which repeats ICalendar events by RRULE, RDATE and EXDATE.
 Home-page: https://github.com/niccokunzmann/python-recurring-ical-events
 Author: Nicco Kunzmann
 Author-email: niccokunzmann@rambler.ru
 License: LGPL-3.0-or-later
 Keywords: icalendar
 Platform: UNKNOWN
@@ -26,27 +26,23 @@
 
 Recurring ICal events for Python
 ================================
 
 .. image:: https://github.com/niccokunzmann/python-recurring-ical-events/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/niccokunzmann/python-recurring-ical-events/actions/workflows/tests.yml
    :alt: GitHub CI build and test status
-
 .. image:: https://badge.fury.io/py/recurring-ical-events.svg
    :target: https://pypi.python.org/pypi/recurring-ical-events
    :alt: Python Package Version on Pypi
-
 .. image:: https://img.shields.io/pypi/dm/recurring-ical-events.svg
    :target: https://pypi.org/project/recurring-ical-events/#files
    :alt: Downloads from Pypi
-
 .. image:: https://img.shields.io/opencollective/all/open-web-calendar?label=support%20on%20open%20collective
    :target: https://opencollective.com/open-web-calendar/
    :alt: Support on Open Collective
-
 .. image:: https://img.shields.io/github/issues/niccokunzmann/python-recurring-ical-events/polar?label=issues%20seek%20funding&color=%23374e96
    :target: https://polar.sh/niccokunzmann/python-recurring-ical-events
    :alt: issues seek funding
 
 
 
 ICal has some complexity to it:
@@ -63,14 +59,15 @@
 * normal events (DONE)
 * recurrence of dates but not hours, minutes, and smaller (DONE)
 * endless recurrence (DONE)
 * ending recurrence (DONE)
 * events with start date and no end date (DONE)
 * events with start as date and start as datetime (DONE)
 * `RRULE <https://www.kanzaki.com/docs/ical/rrule.html>`_ (DONE)
+* events with multiple RRULE (DONE)
 * `RDATE <https://www.kanzaki.com/docs/ical/rdate.html>`_ (DONE)
 * `DURATION <https://www.kanzaki.com/docs/ical/duration.html>`_ (DONE)
 * `EXDATE <https://www.kanzaki.com/docs/ical/exdate.html>`_ (DONE)
 * `X-WR-TIMEZONE` compatibilty (DONE)
 
 Not included:
 
@@ -313,14 +310,18 @@
        python3 setup.py tag_and_deploy
 
 6. notify the issues about their release
 
 Changelog
 ---------
 
+- v2.2.1
+
+  - Add support for multiple RRULE in events.
+
 - v2.2.0
 
   - Add ``after()`` method to iterate over upcoming events.
 
 - v2.1.3
 
   - Test and support Python 3.12.
```

### Comparing `recurring_ical_events-2.2.0/README.rst` & `recurring_ical_events-2.2.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Recurring ICal events for Python
 ================================
 
 .. image:: https://github.com/niccokunzmann/python-recurring-ical-events/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/niccokunzmann/python-recurring-ical-events/actions/workflows/tests.yml
    :alt: GitHub CI build and test status
-
 .. image:: https://badge.fury.io/py/recurring-ical-events.svg
    :target: https://pypi.python.org/pypi/recurring-ical-events
    :alt: Python Package Version on Pypi
-
 .. image:: https://img.shields.io/pypi/dm/recurring-ical-events.svg
    :target: https://pypi.org/project/recurring-ical-events/#files
    :alt: Downloads from Pypi
-
 .. image:: https://img.shields.io/opencollective/all/open-web-calendar?label=support%20on%20open%20collective
    :target: https://opencollective.com/open-web-calendar/
    :alt: Support on Open Collective
-
 .. image:: https://img.shields.io/github/issues/niccokunzmann/python-recurring-ical-events/polar?label=issues%20seek%20funding&color=%23374e96
    :target: https://polar.sh/niccokunzmann/python-recurring-ical-events
    :alt: issues seek funding
 
 
 
 ICal has some complexity to it:
@@ -37,14 +33,15 @@
 * normal events (DONE)
 * recurrence of dates but not hours, minutes, and smaller (DONE)
 * endless recurrence (DONE)
 * ending recurrence (DONE)
 * events with start date and no end date (DONE)
 * events with start as date and start as datetime (DONE)
 * `RRULE <https://www.kanzaki.com/docs/ical/rrule.html>`_ (DONE)
+* events with multiple RRULE (DONE)
 * `RDATE <https://www.kanzaki.com/docs/ical/rdate.html>`_ (DONE)
 * `DURATION <https://www.kanzaki.com/docs/ical/duration.html>`_ (DONE)
 * `EXDATE <https://www.kanzaki.com/docs/ical/exdate.html>`_ (DONE)
 * `X-WR-TIMEZONE` compatibilty (DONE)
 
 Not included:
 
@@ -287,14 +284,18 @@
        python3 setup.py tag_and_deploy
 
 6. notify the issues about their release
 
 Changelog
 ---------
 
+- v2.2.1
+
+  - Add support for multiple RRULE in events.
+
 - v2.2.0
 
   - Add ``after()`` method to iterate over upcoming events.
 
 - v2.1.3
 
   - Test and support Python 3.12.
```

### Comparing `recurring_ical_events-2.2.0/recurring_ical_events.egg-info/PKG-INFO` & `recurring_ical_events-2.2.1/recurring_ical_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurring-ical-events
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python module which repeats ICalendar events by RRULE, RDATE and EXDATE.
 Home-page: https://github.com/niccokunzmann/python-recurring-ical-events
 Author: Nicco Kunzmann
 Author-email: niccokunzmann@rambler.ru
 License: LGPL-3.0-or-later
 Keywords: icalendar
 Platform: UNKNOWN
@@ -26,27 +26,23 @@
 
 Recurring ICal events for Python
 ================================
 
 .. image:: https://github.com/niccokunzmann/python-recurring-ical-events/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/niccokunzmann/python-recurring-ical-events/actions/workflows/tests.yml
    :alt: GitHub CI build and test status
-
 .. image:: https://badge.fury.io/py/recurring-ical-events.svg
    :target: https://pypi.python.org/pypi/recurring-ical-events
    :alt: Python Package Version on Pypi
-
 .. image:: https://img.shields.io/pypi/dm/recurring-ical-events.svg
    :target: https://pypi.org/project/recurring-ical-events/#files
    :alt: Downloads from Pypi
-
 .. image:: https://img.shields.io/opencollective/all/open-web-calendar?label=support%20on%20open%20collective
    :target: https://opencollective.com/open-web-calendar/
    :alt: Support on Open Collective
-
 .. image:: https://img.shields.io/github/issues/niccokunzmann/python-recurring-ical-events/polar?label=issues%20seek%20funding&color=%23374e96
    :target: https://polar.sh/niccokunzmann/python-recurring-ical-events
    :alt: issues seek funding
 
 
 
 ICal has some complexity to it:
@@ -63,14 +59,15 @@
 * normal events (DONE)
 * recurrence of dates but not hours, minutes, and smaller (DONE)
 * endless recurrence (DONE)
 * ending recurrence (DONE)
 * events with start date and no end date (DONE)
 * events with start as date and start as datetime (DONE)
 * `RRULE <https://www.kanzaki.com/docs/ical/rrule.html>`_ (DONE)
+* events with multiple RRULE (DONE)
 * `RDATE <https://www.kanzaki.com/docs/ical/rdate.html>`_ (DONE)
 * `DURATION <https://www.kanzaki.com/docs/ical/duration.html>`_ (DONE)
 * `EXDATE <https://www.kanzaki.com/docs/ical/exdate.html>`_ (DONE)
 * `X-WR-TIMEZONE` compatibilty (DONE)
 
 Not included:
 
@@ -313,14 +310,18 @@
        python3 setup.py tag_and_deploy
 
 6. notify the issues about their release
 
 Changelog
 ---------
 
+- v2.2.1
+
+  - Add support for multiple RRULE in events.
+
 - v2.2.0
 
   - Add ``after()`` method to iterate over upcoming events.
 
 - v2.1.3
 
   - Test and support Python 3.12.
```

### Comparing `recurring_ical_events-2.2.0/recurring_ical_events.py` & `recurring_ical_events-2.2.1/recurring_ical_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -209,35 +209,40 @@
                 else:
                     # we have a date/datetime
                     self.rdates.append(rdate.dt)
 
         self.make_all_dates_comparable()
 
         self.duration = self.end - self.start
-        self.rule = rule = rruleset(cache=True)
-        _rule = component.get("RRULE", None)
-        if _rule:
-            # We don't support multiple RRULE yet, but we can support cases
-            # where the same RRULE is erroneously repeated
-            if isinstance(_rule, list):
-                if len(_rule) > 0 and all(part == _rule[0] for part in _rule):
-                    _rule = _rule[0]
-                else:
-                    raise ValueError("Don't yet support multiple distinct RRULE properties")
-            self.rrule = self.create_rule_with_start(_rule.to_ical().decode())
-            rule.rrule(self.rrule)
-        else:
-            self.rrule = None
+        self.rule = rruleset(cache=True)
+        _component_rules = component.get("RRULE", None)
+        self.until = None
+        if _component_rules:
+            if not isinstance(_component_rules, list):
+                _component_rules = [_component_rules]
+            else:
+                _dedup_rules=[]
+                for _rule in _component_rules:
+                    if _rule not in _dedup_rules:
+                        _dedup_rules.append(_rule)
+                _component_rules = _dedup_rules
+    
+            for _rule in _component_rules:
+                rrule = self.create_rule_with_start(_rule.to_ical().decode())
+                self.rule.rrule(rrule)
+                if rrule.until and (not self.until or compare_greater(rrule.until, self.until)):
+                    self.until = rrule.until
 
         for exdate in self.exdates:
-            rule.exdate(exdate)
+            self.rule.exdate(exdate)
         for rdate in self.rdates:
-            rule.rdate(rdate)
-        if not self.rrule or not self.rrule.until or not compare_greater(self.start, self.rrule.until):
-            rule.rdate(self.start)
+            self.rule.rdate(rdate)
+        
+        if not self.until or not compare_greater(self.start, self.until):
+            self.rule.rdate(self.start)
 
     def create_rule_with_start(self, rule_string):
         """Helper to create an rrule from a rule_string starting at the start of the component.
 
         Since the creation is a bit more complex, this function handles special cases.
         """
         try:
@@ -335,15 +340,15 @@
         # may still be mixed because RDATE, EXDATE, start and rule.
         for start in self.rule.between(span_start, span_stop, inc=True):
             if isinstance(start, datetime.datetime) and is_pytz(start.tzinfo):
                 # update the time zone in case of summer/winter time change
                 start = start.tzinfo.localize(start.replace(tzinfo=None))
                 # We could now well be out of bounce of the end of the UNTIL
                 # value. This is tested by test/test_issue_20_exdate_ignored.py.
-                if self.rrule is not None and self.rrule.until is not None and start > self.rrule.until and start not in self.rdates:
+                if self.until is not None and start > self.until and start not in self.rdates:
                     continue
             if self._unify_exdate(start) in self.exdates_utc or start.date() in self.exdates_utc:
                 continue
             stop = self.replace_ends.get(timestamp(start), start + self.duration)
             yield Repetition(
                 self.component,
                 self.convert_to_original_type(start),
```

### Comparing `recurring_ical_events-2.2.0/setup.py` & `recurring_ical_events-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 
 PACKAGE_NAME = "recurring_ical_events"
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 sys.path.insert(0, HERE)  # for package import
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 __author__ = 'Nicco Kunzmann'
 
 
 def read_file_named(file_name):
     file_path = os.path.join(HERE, file_name)
     with open(file_path) as file:
         return file.read()
```

