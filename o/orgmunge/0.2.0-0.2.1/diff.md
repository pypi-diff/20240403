# Comparing `tmp/orgmunge-0.2.0.tar.gz` & `tmp/orgmunge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orgmunge-0.2.0.tar", max compression
+gzip compressed data, was "orgmunge-0.2.1.tar", max compression
```

## Comparing `orgmunge-0.2.0.tar` & `orgmunge-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-11-01 11:42:01.928949 orgmunge-0.2.0/LICENSE
--rw-r--r--   0        0        0    15396 2023-11-13 03:20:46.479605 orgmunge-0.2.0/README.org
--rw-r--r--   0        0        0      489 2023-11-13 03:14:05.460992 orgmunge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-01 11:42:01.928949 orgmunge-0.2.0/src/orgmunge/Untitled Document
--rw-r--r--   0        0        0     8167 2023-11-13 03:14:51.270832 orgmunge-0.2.0/src/orgmunge/__init__.py
--rw-r--r--   0        0        0    29652 2023-11-13 03:04:18.463085 orgmunge-0.2.0/src/orgmunge/classes.py
--rw-r--r--   0        0        0     2781 2023-11-13 03:04:18.463085 orgmunge-0.2.0/src/orgmunge/lexer.py
--rw-r--r--   0        0        0    83137 2023-11-01 11:42:01.928949 orgmunge-0.2.0/src/orgmunge/parser.out
--rw-r--r--   0        0        0     6384 2023-11-13 03:04:18.463085 orgmunge-0.2.0/src/orgmunge/parser.py
--rw-r--r--   0        0        0    22422 2023-11-13 03:15:21.084062 orgmunge-0.2.0/src/orgmunge/parsetab.py
--rw-r--r--   0        0        0      180 2023-11-01 11:42:01.928949 orgmunge-0.2.0/src/orgmunge/todos.json
--rw-r--r--   0        0        0    15867 1970-01-01 00:00:00.000000 orgmunge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-11-27 03:09:11.255033 orgmunge-0.2.1/LICENSE
+-rw-r--r--   0        0        0    15857 2023-12-06 15:23:58.116040 orgmunge-0.2.1/README.org
+-rw-r--r--   0        0        0      489 2024-04-03 02:30:19.002869 orgmunge-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-27 03:09:14.538358 orgmunge-0.2.1/src/orgmunge/Untitled Document
+-rw-r--r--   0        0        0     9200 2024-03-24 20:22:14.487212 orgmunge-0.2.1/src/orgmunge/__init__.py
+-rw-r--r--   0        0        0    29904 2023-12-06 15:23:58.116040 orgmunge-0.2.1/src/orgmunge/classes.py
+-rw-r--r--   0        0        0     2802 2023-11-27 03:09:14.731691 orgmunge-0.2.1/src/orgmunge/lexer.py
+-rw-r--r--   0        0        0    88741 2024-03-24 20:17:20.317781 orgmunge-0.2.1/src/orgmunge/parser.out
+-rw-r--r--   0        0        0     6785 2024-03-24 20:21:57.743911 orgmunge-0.2.1/src/orgmunge/parser.py
+-rw-r--r--   0        0        0    17283 2024-03-24 20:17:20.314448 orgmunge-0.2.1/src/orgmunge/parsetab.py
+-rw-r--r--   0        0        0      180 2023-11-27 03:09:14.741690 orgmunge-0.2.1/src/orgmunge/todos.json
+-rw-r--r--   0        0        0    16379 1970-01-01 00:00:00.000000 orgmunge-0.2.1/PKG-INFO
```

### Comparing `orgmunge-0.2.0/LICENSE` & `orgmunge-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.0/README.org` & `orgmunge-0.2.1/README.org`

 * *Files 3% similar despite different names*

```diff
@@ -291,14 +291,24 @@
 regex unless =exact= is set to =True=, in which case, the function will
 return headings whose title matches the search string
 exactly. =re_flags= are flags passed to =re.search=. This argument is
 ignored if =exact= is =True=.
 Uses =filter_headings= under the hood so will return a generator of
 matching headings.
 
+*** Search for Headings by Path
+Use =Org.get_heading_by_path= to search for a heading with the given path:
+#+begin_src python
+  Org.get_heading_by_path(path, exact=False, re_flags=0)
+#+end_src
+=path= is a list of heading titles. Each member is interpreted the same
+way the =search_string= argument of =get_headings_by_title= is
+interpreted. This function returns the first heading of the tree that
+matches the given path or =None= if no such heading is found.
+
 * License
 #+INCLUDE: ./LICENSE
 
 
 
 * Contributors
 :PROPERTIES:
```

### Comparing `orgmunge-0.2.0/src/orgmunge/__init__.py` & `orgmunge-0.2.1/src/orgmunge/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import json
 import os
 import platform
 from .parser import Parser
 from .lexer import Lexer
 from .classes import *
-from typing import List, Dict, Optional, Generator, Callable
+from typing import List, Dict, Optional, Generator, Callable, Iterable
 
 class Org:
     def _parse_todos(self, inp: str) -> Optional[Dict[str, Dict[str, str]]]:
         payload = [l.strip() for l in inp.split('\n')
                    if l.startswith('#+TODO:') \
                    or l.startswith('#+SEQ_TODO:')\
                    or l.startswith('#+TYP_TODO:')]
@@ -160,14 +160,33 @@
         todo keywords or tags are considered."""
         if exact:
             condition = lambda h: h.title == search_string
         else:
             condition = lambda h: bool(re.search(fr'{search_string}', h.title, flags=re_flags))
         return self.filter_headings(condition)
 
+    def get_heading_by_path(self, path: List[str], exact: bool = False, re_flags: int = 0) -> Optional[Heading]:
+        """Return a heading by its given path. If exact is True, interpret the given path
+        as strings to match node titles exactly; otherwise, interpret them as regexes. If
+        no heading matches the given path, return None"""
+        if exact:
+            condition = lambda heading: heading.title == path[-1]
+        else:
+            condition = lambda heading: bool(re.search(fr'{path[-1]}', heading.title, flags=re_flags))
+        if not path:
+            return self.root
+        else:
+            headings_at_this_level = self.filter_headings(lambda h: h.level == len(path) and condition(h))  
+            candidates = (h for h in headings_at_this_level
+                          if h.parent is self.get_heading_by_path(path[:-1], exact=exact, re_flags=re_flags))
+            try:
+                return next(candidates)
+            except StopIteration:
+                return None
+        
     def __repr__(self):
         result = ''
         for keyword in self.metadata:
             result += self._metadata_values_to_string(keyword)
         if self.metadata:
             result += '\n'
         if self.initial_body:
```

### Comparing `orgmunge-0.2.0/src/orgmunge/classes.py` & `orgmunge-0.2.1/src/orgmunge/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,17 +563,17 @@
         else:
             raise ValueError(f"Unable to parse {line} as clocking information")
         return Clocking(start_time, end_time)
 
     def _get_clocking_info(self) -> List[Clocking]:
         if not self.drawers:
             return []
-        logbook = [d for d in self.drawers if d.name == 'LOGBOOK']
+        logbook = self.get_drawer_by_name('LOGBOOK')
         if logbook:
-            return [self._parse_clock_line(l) for l in logbook[0].contents if re.search(r'^\s*CLOCK:', l)]
+            return [self._parse_clock_line(l) for l in logbook.contents if re.search(r'^\s*CLOCK:', l)]
         else:
             return []
 
     def _get_properties_dict(self, contents: List[str]) -> Dict[str, str]:
         return {k: v for (k, v) in [re.search(r':([^:]+):\s+(.*)', line).groups()
                                     for line in contents]} 
 
@@ -589,23 +589,29 @@
         if type(val) is not dict:
             raise TypeError("Heading properties must be given in the form of a dict")
         else:
             self._properties = dict()
             for key in val:
                 self._properties[key] = val[key]
 
-
     def clocking(self, include_children: bool = False) -> List[Clocking]:
         "Return the clocking information of the given headline and possibly its children."
         own_clocking = self._get_clocking_info()
         if include_children and self.children != []:
             return own_clocking + reduce(add, [c.clocking(include_children=True) for c in self.children])
         else:
             return own_clocking
 
+    def get_drawer_by_name(self, name: str) -> Optional[Drawer]:
+        "Return the named drawer if it exists, or None if it doesn't"
+        try:
+            return next(d for d in self.drawers if d.name == name)
+        except StopIteration:
+            return None
+
     @property
     def headline(self):
         return self._headline
 
     @headline.setter
     def headline(self, value: Headline):
         if not isinstance(value, Headline):
```

### Comparing `orgmunge-0.2.0/src/orgmunge/lexer.py` & `orgmunge-0.2.1/src/orgmunge/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ATIMESTAMP = fr'<{TIMESTAMP}>'
     ITIMESTAMP = fr'\[{TIMESTAMP}\]'
 
     def __init__(self, todos):
 
         def t_error(t):
             print(f"Illegal character encountered: {t.value[0]}")
-            t.lexer.skip(1)
+            raise ValueError("Lexer error!")
 
         self.todos = todos
         all_todo_keywords = {**todos['todo_states'], **todos['done_states']}
         TODO = fr'(?:{"|".join(list(all_todo_keywords.values()))})'
 
         def t_METADATA(t):
             r'(?:^\#\+[^:\n]+:[^\n]*\n)*^\#\+[^:\n]+:[^\n]*'
@@ -90,15 +90,15 @@
             return t
 
         def t_TAGS(t):
             r'(?::\S+)+:'
             return t
 
         def t_SPACE(t):
-            r'[ \t]+'
+            r'[^\S\r\n]+'
             return t
 
         def t_TEXT(t):
             r'\S+'
             return t
 
         token_funcs = [func for func in locals() if func.startswith('t_')]
```

### Comparing `orgmunge-0.2.0/src/orgmunge/parser.out` & `orgmunge-0.2.1/src/orgmunge/parser.out`

 * *Files 2% similar despite different names*

```diff
@@ -1,1793 +1,1912 @@
 Created by PLY version 3.11 (http://www.dabeaz.com/ply)
 
 Grammar
 
 Rule 0     S' -> org_file
 Rule 1     org_file -> metadata org_tree
 Rule 2     org_file -> non_metadata_body_text SEPARATOR org_tree
-Rule 3     org_file -> metadata non_metadata_body_text SEPARATOR org_tree
-Rule 4     org_file -> metadata non_metadata_body_text SEPARATOR
-Rule 5     org_file -> metadata
-Rule 6     org_file -> org_tree
-Rule 7     org_file -> empty
-Rule 8     metadata -> METADATA SEPARATOR
-Rule 9     metadata -> METADATA NEWLINE
-Rule 10    org_tree -> heading
-Rule 11    org_tree -> heading SEPARATOR
-Rule 12    org_tree -> org_tree heading SEPARATOR
-Rule 13    org_tree -> org_tree heading
-Rule 14    heading -> headline NEWLINE contents
-Rule 15    heading -> headline SEPARATOR
-Rule 16    headline -> STARS SPACE comment todo priority title cookie tags
-Rule 17    comment -> COMMENT SPACE
-Rule 18    comment -> empty
-Rule 19    todo -> TODO SPACE
-Rule 20    todo -> empty
-Rule 21    priority -> PRIORITY SPACE
-Rule 22    priority -> empty
-Rule 23    title -> TEXT
-Rule 24    title -> title SPACE TEXT
-Rule 25    title -> title SPACE
-Rule 26    cookie -> COOKIE SPACE
-Rule 27    cookie -> COOKIE
-Rule 28    cookie -> empty
-Rule 29    tags -> TAGS
-Rule 30    tags -> empty
-Rule 31    contents -> scheduling drawers body
-Rule 32    scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE
-Rule 33    scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR
-Rule 34    scheduling_data -> SCHEDULING SPACE any_timestamp SPACE
-Rule 35    scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE
-Rule 36    scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR
-Rule 37    scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE
-Rule 38    scheduling -> scheduling_data
-Rule 39    scheduling -> empty
-Rule 40    any_timestamp -> ATIMESTAMP
-Rule 41    any_timestamp -> ITIMESTAMP
-Rule 42    drawer_data -> DRAWER NEWLINE
-Rule 43    drawer_data -> DRAWER SEPARATOR
-Rule 44    drawer_data -> drawer_data DRAWER NEWLINE
-Rule 45    drawer_data -> drawer_data DRAWER SEPARATOR
-Rule 46    drawers -> drawer_data
-Rule 47    drawers -> empty
-Rule 48    body -> body_text
-Rule 49    body -> empty
-Rule 50    non_metadata_body_text -> TEXT
-Rule 51    non_metadata_body_text -> SPACE
-Rule 52    non_metadata_body_text -> any_timestamp
-Rule 53    non_metadata_body_text -> non_metadata_body_text TEXT
-Rule 54    non_metadata_body_text -> non_metadata_body_text SPACE
-Rule 55    non_metadata_body_text -> non_metadata_body_text special_token
-Rule 56    non_metadata_body_text -> non_metadata_body_text NEWLINE
-Rule 57    special_token -> SCHEDULING
-Rule 58    special_token -> COOKIE
-Rule 59    special_token -> PRIORITY
-Rule 60    special_token -> TODO
-Rule 61    special_token -> any_timestamp
-Rule 62    special_token -> COMMENT
-Rule 63    special_token -> TAGS
-Rule 64    body_text -> TEXT
-Rule 65    body_text -> SPACE
-Rule 66    body_text -> METADATA
-Rule 67    body_text -> special_token
-Rule 68    body_text -> body_text TEXT
-Rule 69    body_text -> body_text SPACE
-Rule 70    body_text -> body_text special_token
-Rule 71    body_text -> body_text METADATA
-Rule 72    body_text -> body_text NEWLINE
-Rule 73    empty -> <empty>
+Rule 3     org_file -> non_metadata_body_text SEPARATOR
+Rule 4     org_file -> metadata non_metadata_body_text SEPARATOR org_tree
+Rule 5     org_file -> metadata non_metadata_body_text SEPARATOR
+Rule 6     org_file -> metadata
+Rule 7     org_file -> org_tree
+Rule 8     org_file -> SEPARATOR
+Rule 9     org_file -> empty
+Rule 10    metadata -> METADATA SEPARATOR
+Rule 11    metadata -> METADATA NEWLINE
+Rule 12    org_tree -> heading
+Rule 13    org_tree -> heading SEPARATOR
+Rule 14    org_tree -> org_tree heading SEPARATOR
+Rule 15    org_tree -> org_tree heading
+Rule 16    heading -> headline NEWLINE contents
+Rule 17    heading -> headline SEPARATOR
+Rule 18    headline -> STARS SPACE comment todo priority title cookie tags
+Rule 19    comment -> COMMENT SPACE
+Rule 20    comment -> empty
+Rule 21    todo -> TODO SPACE
+Rule 22    todo -> empty
+Rule 23    priority -> PRIORITY SPACE
+Rule 24    priority -> empty
+Rule 25    title -> TEXT
+Rule 26    title -> TODO
+Rule 27    title -> title SPACE TEXT
+Rule 28    title -> title SPACE TODO
+Rule 29    title -> title SPACE
+Rule 30    title -> empty
+Rule 31    cookie -> COOKIE SPACE
+Rule 32    cookie -> COOKIE
+Rule 33    cookie -> empty
+Rule 34    tags -> TAGS
+Rule 35    tags -> empty
+Rule 36    contents -> scheduling drawers body
+Rule 37    scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE
+Rule 38    scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR
+Rule 39    scheduling_data -> SCHEDULING SPACE any_timestamp SPACE
+Rule 40    scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE
+Rule 41    scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR
+Rule 42    scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE
+Rule 43    scheduling -> scheduling_data
+Rule 44    scheduling -> empty
+Rule 45    any_timestamp -> ATIMESTAMP
+Rule 46    any_timestamp -> ITIMESTAMP
+Rule 47    drawer_data -> DRAWER NEWLINE
+Rule 48    drawer_data -> DRAWER SEPARATOR
+Rule 49    drawer_data -> drawer_data DRAWER NEWLINE
+Rule 50    drawer_data -> drawer_data DRAWER SEPARATOR
+Rule 51    drawers -> drawer_data
+Rule 52    drawers -> empty
+Rule 53    body -> body_text
+Rule 54    body -> empty
+Rule 55    non_metadata_body_text -> TEXT
+Rule 56    non_metadata_body_text -> SPACE
+Rule 57    non_metadata_body_text -> any_timestamp
+Rule 58    non_metadata_body_text -> non_metadata_body_text TEXT
+Rule 59    non_metadata_body_text -> non_metadata_body_text SPACE
+Rule 60    non_metadata_body_text -> non_metadata_body_text special_token
+Rule 61    non_metadata_body_text -> non_metadata_body_text NEWLINE
+Rule 62    special_token -> SCHEDULING
+Rule 63    special_token -> COOKIE
+Rule 64    special_token -> PRIORITY
+Rule 65    special_token -> TODO
+Rule 66    special_token -> any_timestamp
+Rule 67    special_token -> COMMENT
+Rule 68    special_token -> TAGS
+Rule 69    body_text -> TEXT
+Rule 70    body_text -> SPACE
+Rule 71    body_text -> METADATA
+Rule 72    body_text -> special_token
+Rule 73    body_text -> body_text TEXT
+Rule 74    body_text -> body_text SPACE
+Rule 75    body_text -> body_text special_token
+Rule 76    body_text -> body_text METADATA
+Rule 77    body_text -> body_text NEWLINE
+Rule 78    empty -> <empty>
 
 Terminals, with rules where they appear
 
-ATIMESTAMP           : 40
-COMMENT              : 17 62
-COOKIE               : 26 27 58
-DRAWER               : 42 43 44 45
-ITIMESTAMP           : 41
-METADATA             : 8 9 66 71
-NEWLINE              : 9 14 32 35 42 44 56 72
-PRIORITY             : 21 59
-SCHEDULING           : 32 33 34 35 36 37 57
-SEPARATOR            : 2 3 4 8 11 12 15 33 36 43 45
-SPACE                : 16 17 19 21 24 25 26 32 33 34 34 35 36 37 37 51 54 65 69
-STARS                : 16
-TAGS                 : 29 63
-TEXT                 : 23 24 50 53 64 68
-TODO                 : 19 60
+ATIMESTAMP           : 45
+COMMENT              : 19 67
+COOKIE               : 31 32 63
+DRAWER               : 47 48 49 50
+ITIMESTAMP           : 46
+METADATA             : 10 11 71 76
+NEWLINE              : 11 16 37 40 47 49 61 77
+PRIORITY             : 23 64
+SCHEDULING           : 37 38 39 40 41 42 62
+SEPARATOR            : 2 3 4 5 8 10 13 14 17 38 41 48 50
+SPACE                : 18 19 21 23 27 28 29 31 37 38 39 39 40 41 42 42 56 59 70 74
+STARS                : 18
+TAGS                 : 34 68
+TEXT                 : 25 27 55 58 69 73
+TODO                 : 21 26 28 65
 error                : 
 
 Nonterminals, with rules where they appear
 
-any_timestamp        : 32 33 34 35 36 37 52 61
-body                 : 31
-body_text            : 48 68 69 70 71 72
-comment              : 16
-contents             : 14
-cookie               : 16
-drawer_data          : 44 45 46
-drawers              : 31
-empty                : 7 18 20 22 28 30 39 47 49
-heading              : 10 11 12 13
-headline             : 14 15
-metadata             : 1 3 4 5
-non_metadata_body_text : 2 3 4 53 54 55 56
+any_timestamp        : 37 38 39 40 41 42 57 66
+body                 : 36
+body_text            : 53 73 74 75 76 77
+comment              : 18
+contents             : 16
+cookie               : 18
+drawer_data          : 49 50 51
+drawers              : 36
+empty                : 9 20 22 24 30 33 35 44 52 54
+heading              : 12 13 14 15
+headline             : 16 17
+metadata             : 1 4 5 6
+non_metadata_body_text : 2 3 4 5 58 59 60 61
 org_file             : 0
-org_tree             : 1 2 3 6 12 13
-priority             : 16
-scheduling           : 31
-scheduling_data      : 35 36 37 38
-special_token        : 55 67 70
-tags                 : 16
-title                : 16 24 25
-todo                 : 16
+org_tree             : 1 2 4 7 14 15
+priority             : 18
+scheduling           : 36
+scheduling_data      : 40 41 42 43
+special_token        : 60 72 75
+tags                 : 18
+title                : 18 27 28 29
+todo                 : 18
 
 Parsing method: LALR
 
 state 0
 
     (0) S' -> . org_file
     (1) org_file -> . metadata org_tree
     (2) org_file -> . non_metadata_body_text SEPARATOR org_tree
-    (3) org_file -> . metadata non_metadata_body_text SEPARATOR org_tree
-    (4) org_file -> . metadata non_metadata_body_text SEPARATOR
-    (5) org_file -> . metadata
-    (6) org_file -> . org_tree
-    (7) org_file -> . empty
-    (8) metadata -> . METADATA SEPARATOR
-    (9) metadata -> . METADATA NEWLINE
-    (50) non_metadata_body_text -> . TEXT
-    (51) non_metadata_body_text -> . SPACE
-    (52) non_metadata_body_text -> . any_timestamp
-    (53) non_metadata_body_text -> . non_metadata_body_text TEXT
-    (54) non_metadata_body_text -> . non_metadata_body_text SPACE
-    (55) non_metadata_body_text -> . non_metadata_body_text special_token
-    (56) non_metadata_body_text -> . non_metadata_body_text NEWLINE
-    (10) org_tree -> . heading
-    (11) org_tree -> . heading SEPARATOR
-    (12) org_tree -> . org_tree heading SEPARATOR
-    (13) org_tree -> . org_tree heading
-    (73) empty -> .
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
-
-    METADATA        shift and go to state 6
-    TEXT            shift and go to state 7
-    SPACE           shift and go to state 8
-    $end            reduce using rule 73 (empty -> .)
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
-    STARS           shift and go to state 14
+    (3) org_file -> . non_metadata_body_text SEPARATOR
+    (4) org_file -> . metadata non_metadata_body_text SEPARATOR org_tree
+    (5) org_file -> . metadata non_metadata_body_text SEPARATOR
+    (6) org_file -> . metadata
+    (7) org_file -> . org_tree
+    (8) org_file -> . SEPARATOR
+    (9) org_file -> . empty
+    (10) metadata -> . METADATA SEPARATOR
+    (11) metadata -> . METADATA NEWLINE
+    (55) non_metadata_body_text -> . TEXT
+    (56) non_metadata_body_text -> . SPACE
+    (57) non_metadata_body_text -> . any_timestamp
+    (58) non_metadata_body_text -> . non_metadata_body_text TEXT
+    (59) non_metadata_body_text -> . non_metadata_body_text SPACE
+    (60) non_metadata_body_text -> . non_metadata_body_text special_token
+    (61) non_metadata_body_text -> . non_metadata_body_text NEWLINE
+    (12) org_tree -> . heading
+    (13) org_tree -> . heading SEPARATOR
+    (14) org_tree -> . org_tree heading SEPARATOR
+    (15) org_tree -> . org_tree heading
+    (78) empty -> .
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
+
+    SEPARATOR       shift and go to state 5
+    METADATA        shift and go to state 7
+    TEXT            shift and go to state 8
+    SPACE           shift and go to state 9
+    $end            reduce using rule 78 (empty -> .)
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
+    STARS           shift and go to state 15
 
     org_file                       shift and go to state 1
     metadata                       shift and go to state 2
     org_tree                       shift and go to state 3
     non_metadata_body_text         shift and go to state 4
-    empty                          shift and go to state 5
-    any_timestamp                  shift and go to state 9
-    heading                        shift and go to state 10
-    headline                       shift and go to state 13
+    empty                          shift and go to state 6
+    any_timestamp                  shift and go to state 10
+    heading                        shift and go to state 11
+    headline                       shift and go to state 14
 
 state 1
 
     (0) S' -> org_file .
 
 
 
 state 2
 
     (1) org_file -> metadata . org_tree
-    (3) org_file -> metadata . non_metadata_body_text SEPARATOR org_tree
-    (4) org_file -> metadata . non_metadata_body_text SEPARATOR
-    (5) org_file -> metadata .
-    (10) org_tree -> . heading
-    (11) org_tree -> . heading SEPARATOR
-    (12) org_tree -> . org_tree heading SEPARATOR
-    (13) org_tree -> . org_tree heading
-    (50) non_metadata_body_text -> . TEXT
-    (51) non_metadata_body_text -> . SPACE
-    (52) non_metadata_body_text -> . any_timestamp
-    (53) non_metadata_body_text -> . non_metadata_body_text TEXT
-    (54) non_metadata_body_text -> . non_metadata_body_text SPACE
-    (55) non_metadata_body_text -> . non_metadata_body_text special_token
-    (56) non_metadata_body_text -> . non_metadata_body_text NEWLINE
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
-
-    $end            reduce using rule 5 (org_file -> metadata .)
-    TEXT            shift and go to state 7
-    SPACE           shift and go to state 8
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
-    STARS           shift and go to state 14
-
-    org_tree                       shift and go to state 15
-    non_metadata_body_text         shift and go to state 16
-    heading                        shift and go to state 10
-    any_timestamp                  shift and go to state 9
-    headline                       shift and go to state 13
+    (4) org_file -> metadata . non_metadata_body_text SEPARATOR org_tree
+    (5) org_file -> metadata . non_metadata_body_text SEPARATOR
+    (6) org_file -> metadata .
+    (12) org_tree -> . heading
+    (13) org_tree -> . heading SEPARATOR
+    (14) org_tree -> . org_tree heading SEPARATOR
+    (15) org_tree -> . org_tree heading
+    (55) non_metadata_body_text -> . TEXT
+    (56) non_metadata_body_text -> . SPACE
+    (57) non_metadata_body_text -> . any_timestamp
+    (58) non_metadata_body_text -> . non_metadata_body_text TEXT
+    (59) non_metadata_body_text -> . non_metadata_body_text SPACE
+    (60) non_metadata_body_text -> . non_metadata_body_text special_token
+    (61) non_metadata_body_text -> . non_metadata_body_text NEWLINE
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
+
+    $end            reduce using rule 6 (org_file -> metadata .)
+    TEXT            shift and go to state 8
+    SPACE           shift and go to state 9
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
+    STARS           shift and go to state 15
+
+    org_tree                       shift and go to state 16
+    non_metadata_body_text         shift and go to state 17
+    heading                        shift and go to state 11
+    any_timestamp                  shift and go to state 10
+    headline                       shift and go to state 14
 
 state 3
 
-    (6) org_file -> org_tree .
-    (12) org_tree -> org_tree . heading SEPARATOR
-    (13) org_tree -> org_tree . heading
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
+    (7) org_file -> org_tree .
+    (14) org_tree -> org_tree . heading SEPARATOR
+    (15) org_tree -> org_tree . heading
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
 
-    $end            reduce using rule 6 (org_file -> org_tree .)
-    STARS           shift and go to state 14
+    $end            reduce using rule 7 (org_file -> org_tree .)
+    STARS           shift and go to state 15
 
-    heading                        shift and go to state 17
-    headline                       shift and go to state 13
+    heading                        shift and go to state 18
+    headline                       shift and go to state 14
 
 state 4
 
     (2) org_file -> non_metadata_body_text . SEPARATOR org_tree
-    (53) non_metadata_body_text -> non_metadata_body_text . TEXT
-    (54) non_metadata_body_text -> non_metadata_body_text . SPACE
-    (55) non_metadata_body_text -> non_metadata_body_text . special_token
-    (56) non_metadata_body_text -> non_metadata_body_text . NEWLINE
-    (57) special_token -> . SCHEDULING
-    (58) special_token -> . COOKIE
-    (59) special_token -> . PRIORITY
-    (60) special_token -> . TODO
-    (61) special_token -> . any_timestamp
-    (62) special_token -> . COMMENT
-    (63) special_token -> . TAGS
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
-
-    SEPARATOR       shift and go to state 18
-    TEXT            shift and go to state 19
-    SPACE           shift and go to state 20
-    NEWLINE         shift and go to state 22
-    SCHEDULING      shift and go to state 23
-    COOKIE          shift and go to state 24
-    PRIORITY        shift and go to state 25
-    TODO            shift and go to state 26
-    COMMENT         shift and go to state 28
-    TAGS            shift and go to state 29
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
+    (3) org_file -> non_metadata_body_text . SEPARATOR
+    (58) non_metadata_body_text -> non_metadata_body_text . TEXT
+    (59) non_metadata_body_text -> non_metadata_body_text . SPACE
+    (60) non_metadata_body_text -> non_metadata_body_text . special_token
+    (61) non_metadata_body_text -> non_metadata_body_text . NEWLINE
+    (62) special_token -> . SCHEDULING
+    (63) special_token -> . COOKIE
+    (64) special_token -> . PRIORITY
+    (65) special_token -> . TODO
+    (66) special_token -> . any_timestamp
+    (67) special_token -> . COMMENT
+    (68) special_token -> . TAGS
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
+
+    SEPARATOR       shift and go to state 19
+    TEXT            shift and go to state 20
+    SPACE           shift and go to state 21
+    NEWLINE         shift and go to state 23
+    SCHEDULING      shift and go to state 24
+    COOKIE          shift and go to state 25
+    PRIORITY        shift and go to state 26
+    TODO            shift and go to state 27
+    COMMENT         shift and go to state 29
+    TAGS            shift and go to state 30
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
 
-    special_token                  shift and go to state 21
-    any_timestamp                  shift and go to state 27
+    special_token                  shift and go to state 22
+    any_timestamp                  shift and go to state 28
 
 state 5
 
-    (7) org_file -> empty .
+    (8) org_file -> SEPARATOR .
 
-    $end            reduce using rule 7 (org_file -> empty .)
+    $end            reduce using rule 8 (org_file -> SEPARATOR .)
 
 
 state 6
 
-    (8) metadata -> METADATA . SEPARATOR
-    (9) metadata -> METADATA . NEWLINE
+    (9) org_file -> empty .
 
-    SEPARATOR       shift and go to state 30
-    NEWLINE         shift and go to state 31
+    $end            reduce using rule 9 (org_file -> empty .)
 
 
 state 7
 
-    (50) non_metadata_body_text -> TEXT .
+    (10) metadata -> METADATA . SEPARATOR
+    (11) metadata -> METADATA . NEWLINE
 
-    SEPARATOR       reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    TEXT            reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    SPACE           reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    NEWLINE         reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    SCHEDULING      reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    COOKIE          reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    PRIORITY        reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    TODO            reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    COMMENT         reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    TAGS            reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    ATIMESTAMP      reduce using rule 50 (non_metadata_body_text -> TEXT .)
-    ITIMESTAMP      reduce using rule 50 (non_metadata_body_text -> TEXT .)
+    SEPARATOR       shift and go to state 31
+    NEWLINE         shift and go to state 32
 
 
 state 8
 
-    (51) non_metadata_body_text -> SPACE .
+    (55) non_metadata_body_text -> TEXT .
 
-    SEPARATOR       reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    TEXT            reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    SPACE           reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    NEWLINE         reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    SCHEDULING      reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    COOKIE          reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    PRIORITY        reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    TODO            reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    COMMENT         reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    TAGS            reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    ATIMESTAMP      reduce using rule 51 (non_metadata_body_text -> SPACE .)
-    ITIMESTAMP      reduce using rule 51 (non_metadata_body_text -> SPACE .)
+    SEPARATOR       reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    TEXT            reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    SPACE           reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    NEWLINE         reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    SCHEDULING      reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    COOKIE          reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    PRIORITY        reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    TODO            reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    COMMENT         reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    TAGS            reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    ATIMESTAMP      reduce using rule 55 (non_metadata_body_text -> TEXT .)
+    ITIMESTAMP      reduce using rule 55 (non_metadata_body_text -> TEXT .)
 
 
 state 9
 
-    (52) non_metadata_body_text -> any_timestamp .
+    (56) non_metadata_body_text -> SPACE .
 
-    SEPARATOR       reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    TEXT            reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    SPACE           reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    NEWLINE         reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    SCHEDULING      reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    COOKIE          reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    PRIORITY        reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    TODO            reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    COMMENT         reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    TAGS            reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    ATIMESTAMP      reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
-    ITIMESTAMP      reduce using rule 52 (non_metadata_body_text -> any_timestamp .)
+    SEPARATOR       reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    TEXT            reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    SPACE           reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    NEWLINE         reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    SCHEDULING      reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    COOKIE          reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    PRIORITY        reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    TODO            reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    COMMENT         reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    TAGS            reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    ATIMESTAMP      reduce using rule 56 (non_metadata_body_text -> SPACE .)
+    ITIMESTAMP      reduce using rule 56 (non_metadata_body_text -> SPACE .)
 
 
 state 10
 
-    (10) org_tree -> heading .
-    (11) org_tree -> heading . SEPARATOR
+    (57) non_metadata_body_text -> any_timestamp .
 
-    STARS           reduce using rule 10 (org_tree -> heading .)
-    $end            reduce using rule 10 (org_tree -> heading .)
-    SEPARATOR       shift and go to state 32
+    SEPARATOR       reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    TEXT            reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    SPACE           reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    NEWLINE         reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    SCHEDULING      reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    COOKIE          reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    PRIORITY        reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    TODO            reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    COMMENT         reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    TAGS            reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    ATIMESTAMP      reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
+    ITIMESTAMP      reduce using rule 57 (non_metadata_body_text -> any_timestamp .)
 
 
 state 11
 
-    (40) any_timestamp -> ATIMESTAMP .
+    (12) org_tree -> heading .
+    (13) org_tree -> heading . SEPARATOR
 
-    SEPARATOR       reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    TEXT            reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    SPACE           reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    NEWLINE         reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    SCHEDULING      reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    COOKIE          reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    PRIORITY        reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    TODO            reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    COMMENT         reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    TAGS            reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    ATIMESTAMP      reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    ITIMESTAMP      reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    METADATA        reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    STARS           reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
-    $end            reduce using rule 40 (any_timestamp -> ATIMESTAMP .)
+    STARS           reduce using rule 12 (org_tree -> heading .)
+    $end            reduce using rule 12 (org_tree -> heading .)
+    SEPARATOR       shift and go to state 33
 
 
 state 12
 
-    (41) any_timestamp -> ITIMESTAMP .
+    (45) any_timestamp -> ATIMESTAMP .
 
-    SEPARATOR       reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    TEXT            reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    SPACE           reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    NEWLINE         reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    SCHEDULING      reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    COOKIE          reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    PRIORITY        reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    TODO            reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    COMMENT         reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    TAGS            reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    ATIMESTAMP      reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    ITIMESTAMP      reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    METADATA        reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    STARS           reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
-    $end            reduce using rule 41 (any_timestamp -> ITIMESTAMP .)
+    SEPARATOR       reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    TEXT            reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    SPACE           reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    NEWLINE         reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    SCHEDULING      reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    COOKIE          reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    PRIORITY        reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    TODO            reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    COMMENT         reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    TAGS            reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    ATIMESTAMP      reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    ITIMESTAMP      reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    METADATA        reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    STARS           reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
+    $end            reduce using rule 45 (any_timestamp -> ATIMESTAMP .)
 
 
 state 13
 
-    (14) heading -> headline . NEWLINE contents
-    (15) heading -> headline . SEPARATOR
+    (46) any_timestamp -> ITIMESTAMP .
 
-    NEWLINE         shift and go to state 33
-    SEPARATOR       shift and go to state 34
+    SEPARATOR       reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    TEXT            reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    SPACE           reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    NEWLINE         reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    SCHEDULING      reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    COOKIE          reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    PRIORITY        reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    TODO            reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    COMMENT         reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    TAGS            reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    ATIMESTAMP      reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    ITIMESTAMP      reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    METADATA        reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    STARS           reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
+    $end            reduce using rule 46 (any_timestamp -> ITIMESTAMP .)
 
 
 state 14
 
-    (16) headline -> STARS . SPACE comment todo priority title cookie tags
+    (16) heading -> headline . NEWLINE contents
+    (17) heading -> headline . SEPARATOR
 
-    SPACE           shift and go to state 35
+    NEWLINE         shift and go to state 34
+    SEPARATOR       shift and go to state 35
 
 
 state 15
 
-    (1) org_file -> metadata org_tree .
-    (12) org_tree -> org_tree . heading SEPARATOR
-    (13) org_tree -> org_tree . heading
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
+    (18) headline -> STARS . SPACE comment todo priority title cookie tags
 
-    $end            reduce using rule 1 (org_file -> metadata org_tree .)
-    STARS           shift and go to state 14
+    SPACE           shift and go to state 36
 
-    heading                        shift and go to state 17
-    headline                       shift and go to state 13
 
 state 16
 
-    (3) org_file -> metadata non_metadata_body_text . SEPARATOR org_tree
-    (4) org_file -> metadata non_metadata_body_text . SEPARATOR
-    (53) non_metadata_body_text -> non_metadata_body_text . TEXT
-    (54) non_metadata_body_text -> non_metadata_body_text . SPACE
-    (55) non_metadata_body_text -> non_metadata_body_text . special_token
-    (56) non_metadata_body_text -> non_metadata_body_text . NEWLINE
-    (57) special_token -> . SCHEDULING
-    (58) special_token -> . COOKIE
-    (59) special_token -> . PRIORITY
-    (60) special_token -> . TODO
-    (61) special_token -> . any_timestamp
-    (62) special_token -> . COMMENT
-    (63) special_token -> . TAGS
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
-
-    SEPARATOR       shift and go to state 36
-    TEXT            shift and go to state 19
-    SPACE           shift and go to state 20
-    NEWLINE         shift and go to state 22
-    SCHEDULING      shift and go to state 23
-    COOKIE          shift and go to state 24
-    PRIORITY        shift and go to state 25
-    TODO            shift and go to state 26
-    COMMENT         shift and go to state 28
-    TAGS            shift and go to state 29
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
+    (1) org_file -> metadata org_tree .
+    (14) org_tree -> org_tree . heading SEPARATOR
+    (15) org_tree -> org_tree . heading
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
+
+    $end            reduce using rule 1 (org_file -> metadata org_tree .)
+    STARS           shift and go to state 15
 
-    special_token                  shift and go to state 21
-    any_timestamp                  shift and go to state 27
+    heading                        shift and go to state 18
+    headline                       shift and go to state 14
 
 state 17
 
-    (12) org_tree -> org_tree heading . SEPARATOR
-    (13) org_tree -> org_tree heading .
+    (4) org_file -> metadata non_metadata_body_text . SEPARATOR org_tree
+    (5) org_file -> metadata non_metadata_body_text . SEPARATOR
+    (58) non_metadata_body_text -> non_metadata_body_text . TEXT
+    (59) non_metadata_body_text -> non_metadata_body_text . SPACE
+    (60) non_metadata_body_text -> non_metadata_body_text . special_token
+    (61) non_metadata_body_text -> non_metadata_body_text . NEWLINE
+    (62) special_token -> . SCHEDULING
+    (63) special_token -> . COOKIE
+    (64) special_token -> . PRIORITY
+    (65) special_token -> . TODO
+    (66) special_token -> . any_timestamp
+    (67) special_token -> . COMMENT
+    (68) special_token -> . TAGS
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
 
     SEPARATOR       shift and go to state 37
-    STARS           reduce using rule 13 (org_tree -> org_tree heading .)
-    $end            reduce using rule 13 (org_tree -> org_tree heading .)
+    TEXT            shift and go to state 20
+    SPACE           shift and go to state 21
+    NEWLINE         shift and go to state 23
+    SCHEDULING      shift and go to state 24
+    COOKIE          shift and go to state 25
+    PRIORITY        shift and go to state 26
+    TODO            shift and go to state 27
+    COMMENT         shift and go to state 29
+    TAGS            shift and go to state 30
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
 
+    special_token                  shift and go to state 22
+    any_timestamp                  shift and go to state 28
 
 state 18
 
-    (2) org_file -> non_metadata_body_text SEPARATOR . org_tree
-    (10) org_tree -> . heading
-    (11) org_tree -> . heading SEPARATOR
-    (12) org_tree -> . org_tree heading SEPARATOR
-    (13) org_tree -> . org_tree heading
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
-
-    STARS           shift and go to state 14
-
-    org_tree                       shift and go to state 38
-    heading                        shift and go to state 10
-    headline                       shift and go to state 13
+    (14) org_tree -> org_tree heading . SEPARATOR
+    (15) org_tree -> org_tree heading .
 
-state 19
+    SEPARATOR       shift and go to state 38
+    STARS           reduce using rule 15 (org_tree -> org_tree heading .)
+    $end            reduce using rule 15 (org_tree -> org_tree heading .)
 
-    (53) non_metadata_body_text -> non_metadata_body_text TEXT .
 
-    SEPARATOR       reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    TEXT            reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    SPACE           reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    NEWLINE         reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    SCHEDULING      reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    COOKIE          reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    PRIORITY        reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    TODO            reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    COMMENT         reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    TAGS            reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    ATIMESTAMP      reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
-    ITIMESTAMP      reduce using rule 53 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+state 19
 
+    (2) org_file -> non_metadata_body_text SEPARATOR . org_tree
+    (3) org_file -> non_metadata_body_text SEPARATOR .
+    (12) org_tree -> . heading
+    (13) org_tree -> . heading SEPARATOR
+    (14) org_tree -> . org_tree heading SEPARATOR
+    (15) org_tree -> . org_tree heading
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
+
+    $end            reduce using rule 3 (org_file -> non_metadata_body_text SEPARATOR .)
+    STARS           shift and go to state 15
+
+    org_tree                       shift and go to state 39
+    heading                        shift and go to state 11
+    headline                       shift and go to state 14
 
 state 20
 
-    (54) non_metadata_body_text -> non_metadata_body_text SPACE .
+    (58) non_metadata_body_text -> non_metadata_body_text TEXT .
 
-    SEPARATOR       reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    TEXT            reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    SPACE           reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    NEWLINE         reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    SCHEDULING      reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    COOKIE          reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    PRIORITY        reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    TODO            reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    COMMENT         reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    TAGS            reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    ATIMESTAMP      reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
-    ITIMESTAMP      reduce using rule 54 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    SEPARATOR       reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    TEXT            reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    SPACE           reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    NEWLINE         reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    SCHEDULING      reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    COOKIE          reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    PRIORITY        reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    TODO            reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    COMMENT         reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    TAGS            reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    ATIMESTAMP      reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
+    ITIMESTAMP      reduce using rule 58 (non_metadata_body_text -> non_metadata_body_text TEXT .)
 
 
 state 21
 
-    (55) non_metadata_body_text -> non_metadata_body_text special_token .
+    (59) non_metadata_body_text -> non_metadata_body_text SPACE .
 
-    SEPARATOR       reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    TEXT            reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    SPACE           reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    NEWLINE         reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    SCHEDULING      reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    COOKIE          reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    PRIORITY        reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    TODO            reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    COMMENT         reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    TAGS            reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    ATIMESTAMP      reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
-    ITIMESTAMP      reduce using rule 55 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    SEPARATOR       reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    TEXT            reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    SPACE           reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    NEWLINE         reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    SCHEDULING      reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    COOKIE          reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    PRIORITY        reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    TODO            reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    COMMENT         reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    TAGS            reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    ATIMESTAMP      reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
+    ITIMESTAMP      reduce using rule 59 (non_metadata_body_text -> non_metadata_body_text SPACE .)
 
 
 state 22
 
-    (56) non_metadata_body_text -> non_metadata_body_text NEWLINE .
+    (60) non_metadata_body_text -> non_metadata_body_text special_token .
 
-    SEPARATOR       reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    TEXT            reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    SPACE           reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    NEWLINE         reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    SCHEDULING      reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    COOKIE          reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    PRIORITY        reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    TODO            reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    COMMENT         reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    TAGS            reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    ATIMESTAMP      reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
-    ITIMESTAMP      reduce using rule 56 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    SEPARATOR       reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    TEXT            reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    SPACE           reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    NEWLINE         reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    SCHEDULING      reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    COOKIE          reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    PRIORITY        reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    TODO            reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    COMMENT         reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    TAGS            reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    ATIMESTAMP      reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
+    ITIMESTAMP      reduce using rule 60 (non_metadata_body_text -> non_metadata_body_text special_token .)
 
 
 state 23
 
-    (57) special_token -> SCHEDULING .
+    (61) non_metadata_body_text -> non_metadata_body_text NEWLINE .
 
-    SEPARATOR       reduce using rule 57 (special_token -> SCHEDULING .)
-    TEXT            reduce using rule 57 (special_token -> SCHEDULING .)
-    SPACE           reduce using rule 57 (special_token -> SCHEDULING .)
-    NEWLINE         reduce using rule 57 (special_token -> SCHEDULING .)
-    SCHEDULING      reduce using rule 57 (special_token -> SCHEDULING .)
-    COOKIE          reduce using rule 57 (special_token -> SCHEDULING .)
-    PRIORITY        reduce using rule 57 (special_token -> SCHEDULING .)
-    TODO            reduce using rule 57 (special_token -> SCHEDULING .)
-    COMMENT         reduce using rule 57 (special_token -> SCHEDULING .)
-    TAGS            reduce using rule 57 (special_token -> SCHEDULING .)
-    ATIMESTAMP      reduce using rule 57 (special_token -> SCHEDULING .)
-    ITIMESTAMP      reduce using rule 57 (special_token -> SCHEDULING .)
-    METADATA        reduce using rule 57 (special_token -> SCHEDULING .)
-    STARS           reduce using rule 57 (special_token -> SCHEDULING .)
-    $end            reduce using rule 57 (special_token -> SCHEDULING .)
+    SEPARATOR       reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    TEXT            reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    SPACE           reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    NEWLINE         reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    SCHEDULING      reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    COOKIE          reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    PRIORITY        reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    TODO            reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    COMMENT         reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    TAGS            reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    ATIMESTAMP      reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
+    ITIMESTAMP      reduce using rule 61 (non_metadata_body_text -> non_metadata_body_text NEWLINE .)
 
 
 state 24
 
-    (58) special_token -> COOKIE .
+    (62) special_token -> SCHEDULING .
 
-    SEPARATOR       reduce using rule 58 (special_token -> COOKIE .)
-    TEXT            reduce using rule 58 (special_token -> COOKIE .)
-    SPACE           reduce using rule 58 (special_token -> COOKIE .)
-    NEWLINE         reduce using rule 58 (special_token -> COOKIE .)
-    SCHEDULING      reduce using rule 58 (special_token -> COOKIE .)
-    COOKIE          reduce using rule 58 (special_token -> COOKIE .)
-    PRIORITY        reduce using rule 58 (special_token -> COOKIE .)
-    TODO            reduce using rule 58 (special_token -> COOKIE .)
-    COMMENT         reduce using rule 58 (special_token -> COOKIE .)
-    TAGS            reduce using rule 58 (special_token -> COOKIE .)
-    ATIMESTAMP      reduce using rule 58 (special_token -> COOKIE .)
-    ITIMESTAMP      reduce using rule 58 (special_token -> COOKIE .)
-    METADATA        reduce using rule 58 (special_token -> COOKIE .)
-    STARS           reduce using rule 58 (special_token -> COOKIE .)
-    $end            reduce using rule 58 (special_token -> COOKIE .)
+    SEPARATOR       reduce using rule 62 (special_token -> SCHEDULING .)
+    TEXT            reduce using rule 62 (special_token -> SCHEDULING .)
+    SPACE           reduce using rule 62 (special_token -> SCHEDULING .)
+    NEWLINE         reduce using rule 62 (special_token -> SCHEDULING .)
+    SCHEDULING      reduce using rule 62 (special_token -> SCHEDULING .)
+    COOKIE          reduce using rule 62 (special_token -> SCHEDULING .)
+    PRIORITY        reduce using rule 62 (special_token -> SCHEDULING .)
+    TODO            reduce using rule 62 (special_token -> SCHEDULING .)
+    COMMENT         reduce using rule 62 (special_token -> SCHEDULING .)
+    TAGS            reduce using rule 62 (special_token -> SCHEDULING .)
+    ATIMESTAMP      reduce using rule 62 (special_token -> SCHEDULING .)
+    ITIMESTAMP      reduce using rule 62 (special_token -> SCHEDULING .)
+    METADATA        reduce using rule 62 (special_token -> SCHEDULING .)
+    STARS           reduce using rule 62 (special_token -> SCHEDULING .)
+    $end            reduce using rule 62 (special_token -> SCHEDULING .)
 
 
 state 25
 
-    (59) special_token -> PRIORITY .
+    (63) special_token -> COOKIE .
 
-    SEPARATOR       reduce using rule 59 (special_token -> PRIORITY .)
-    TEXT            reduce using rule 59 (special_token -> PRIORITY .)
-    SPACE           reduce using rule 59 (special_token -> PRIORITY .)
-    NEWLINE         reduce using rule 59 (special_token -> PRIORITY .)
-    SCHEDULING      reduce using rule 59 (special_token -> PRIORITY .)
-    COOKIE          reduce using rule 59 (special_token -> PRIORITY .)
-    PRIORITY        reduce using rule 59 (special_token -> PRIORITY .)
-    TODO            reduce using rule 59 (special_token -> PRIORITY .)
-    COMMENT         reduce using rule 59 (special_token -> PRIORITY .)
-    TAGS            reduce using rule 59 (special_token -> PRIORITY .)
-    ATIMESTAMP      reduce using rule 59 (special_token -> PRIORITY .)
-    ITIMESTAMP      reduce using rule 59 (special_token -> PRIORITY .)
-    METADATA        reduce using rule 59 (special_token -> PRIORITY .)
-    STARS           reduce using rule 59 (special_token -> PRIORITY .)
-    $end            reduce using rule 59 (special_token -> PRIORITY .)
+    SEPARATOR       reduce using rule 63 (special_token -> COOKIE .)
+    TEXT            reduce using rule 63 (special_token -> COOKIE .)
+    SPACE           reduce using rule 63 (special_token -> COOKIE .)
+    NEWLINE         reduce using rule 63 (special_token -> COOKIE .)
+    SCHEDULING      reduce using rule 63 (special_token -> COOKIE .)
+    COOKIE          reduce using rule 63 (special_token -> COOKIE .)
+    PRIORITY        reduce using rule 63 (special_token -> COOKIE .)
+    TODO            reduce using rule 63 (special_token -> COOKIE .)
+    COMMENT         reduce using rule 63 (special_token -> COOKIE .)
+    TAGS            reduce using rule 63 (special_token -> COOKIE .)
+    ATIMESTAMP      reduce using rule 63 (special_token -> COOKIE .)
+    ITIMESTAMP      reduce using rule 63 (special_token -> COOKIE .)
+    METADATA        reduce using rule 63 (special_token -> COOKIE .)
+    STARS           reduce using rule 63 (special_token -> COOKIE .)
+    $end            reduce using rule 63 (special_token -> COOKIE .)
 
 
 state 26
 
-    (60) special_token -> TODO .
+    (64) special_token -> PRIORITY .
 
-    SEPARATOR       reduce using rule 60 (special_token -> TODO .)
-    TEXT            reduce using rule 60 (special_token -> TODO .)
-    SPACE           reduce using rule 60 (special_token -> TODO .)
-    NEWLINE         reduce using rule 60 (special_token -> TODO .)
-    SCHEDULING      reduce using rule 60 (special_token -> TODO .)
-    COOKIE          reduce using rule 60 (special_token -> TODO .)
-    PRIORITY        reduce using rule 60 (special_token -> TODO .)
-    TODO            reduce using rule 60 (special_token -> TODO .)
-    COMMENT         reduce using rule 60 (special_token -> TODO .)
-    TAGS            reduce using rule 60 (special_token -> TODO .)
-    ATIMESTAMP      reduce using rule 60 (special_token -> TODO .)
-    ITIMESTAMP      reduce using rule 60 (special_token -> TODO .)
-    METADATA        reduce using rule 60 (special_token -> TODO .)
-    STARS           reduce using rule 60 (special_token -> TODO .)
-    $end            reduce using rule 60 (special_token -> TODO .)
+    SEPARATOR       reduce using rule 64 (special_token -> PRIORITY .)
+    TEXT            reduce using rule 64 (special_token -> PRIORITY .)
+    SPACE           reduce using rule 64 (special_token -> PRIORITY .)
+    NEWLINE         reduce using rule 64 (special_token -> PRIORITY .)
+    SCHEDULING      reduce using rule 64 (special_token -> PRIORITY .)
+    COOKIE          reduce using rule 64 (special_token -> PRIORITY .)
+    PRIORITY        reduce using rule 64 (special_token -> PRIORITY .)
+    TODO            reduce using rule 64 (special_token -> PRIORITY .)
+    COMMENT         reduce using rule 64 (special_token -> PRIORITY .)
+    TAGS            reduce using rule 64 (special_token -> PRIORITY .)
+    ATIMESTAMP      reduce using rule 64 (special_token -> PRIORITY .)
+    ITIMESTAMP      reduce using rule 64 (special_token -> PRIORITY .)
+    METADATA        reduce using rule 64 (special_token -> PRIORITY .)
+    STARS           reduce using rule 64 (special_token -> PRIORITY .)
+    $end            reduce using rule 64 (special_token -> PRIORITY .)
 
 
 state 27
 
-    (61) special_token -> any_timestamp .
+    (65) special_token -> TODO .
 
-    SEPARATOR       reduce using rule 61 (special_token -> any_timestamp .)
-    TEXT            reduce using rule 61 (special_token -> any_timestamp .)
-    SPACE           reduce using rule 61 (special_token -> any_timestamp .)
-    NEWLINE         reduce using rule 61 (special_token -> any_timestamp .)
-    SCHEDULING      reduce using rule 61 (special_token -> any_timestamp .)
-    COOKIE          reduce using rule 61 (special_token -> any_timestamp .)
-    PRIORITY        reduce using rule 61 (special_token -> any_timestamp .)
-    TODO            reduce using rule 61 (special_token -> any_timestamp .)
-    COMMENT         reduce using rule 61 (special_token -> any_timestamp .)
-    TAGS            reduce using rule 61 (special_token -> any_timestamp .)
-    ATIMESTAMP      reduce using rule 61 (special_token -> any_timestamp .)
-    ITIMESTAMP      reduce using rule 61 (special_token -> any_timestamp .)
-    METADATA        reduce using rule 61 (special_token -> any_timestamp .)
-    STARS           reduce using rule 61 (special_token -> any_timestamp .)
-    $end            reduce using rule 61 (special_token -> any_timestamp .)
+    SEPARATOR       reduce using rule 65 (special_token -> TODO .)
+    TEXT            reduce using rule 65 (special_token -> TODO .)
+    SPACE           reduce using rule 65 (special_token -> TODO .)
+    NEWLINE         reduce using rule 65 (special_token -> TODO .)
+    SCHEDULING      reduce using rule 65 (special_token -> TODO .)
+    COOKIE          reduce using rule 65 (special_token -> TODO .)
+    PRIORITY        reduce using rule 65 (special_token -> TODO .)
+    TODO            reduce using rule 65 (special_token -> TODO .)
+    COMMENT         reduce using rule 65 (special_token -> TODO .)
+    TAGS            reduce using rule 65 (special_token -> TODO .)
+    ATIMESTAMP      reduce using rule 65 (special_token -> TODO .)
+    ITIMESTAMP      reduce using rule 65 (special_token -> TODO .)
+    METADATA        reduce using rule 65 (special_token -> TODO .)
+    STARS           reduce using rule 65 (special_token -> TODO .)
+    $end            reduce using rule 65 (special_token -> TODO .)
 
 
 state 28
 
-    (62) special_token -> COMMENT .
+    (66) special_token -> any_timestamp .
 
-    SEPARATOR       reduce using rule 62 (special_token -> COMMENT .)
-    TEXT            reduce using rule 62 (special_token -> COMMENT .)
-    SPACE           reduce using rule 62 (special_token -> COMMENT .)
-    NEWLINE         reduce using rule 62 (special_token -> COMMENT .)
-    SCHEDULING      reduce using rule 62 (special_token -> COMMENT .)
-    COOKIE          reduce using rule 62 (special_token -> COMMENT .)
-    PRIORITY        reduce using rule 62 (special_token -> COMMENT .)
-    TODO            reduce using rule 62 (special_token -> COMMENT .)
-    COMMENT         reduce using rule 62 (special_token -> COMMENT .)
-    TAGS            reduce using rule 62 (special_token -> COMMENT .)
-    ATIMESTAMP      reduce using rule 62 (special_token -> COMMENT .)
-    ITIMESTAMP      reduce using rule 62 (special_token -> COMMENT .)
-    METADATA        reduce using rule 62 (special_token -> COMMENT .)
-    STARS           reduce using rule 62 (special_token -> COMMENT .)
-    $end            reduce using rule 62 (special_token -> COMMENT .)
+    SEPARATOR       reduce using rule 66 (special_token -> any_timestamp .)
+    TEXT            reduce using rule 66 (special_token -> any_timestamp .)
+    SPACE           reduce using rule 66 (special_token -> any_timestamp .)
+    NEWLINE         reduce using rule 66 (special_token -> any_timestamp .)
+    SCHEDULING      reduce using rule 66 (special_token -> any_timestamp .)
+    COOKIE          reduce using rule 66 (special_token -> any_timestamp .)
+    PRIORITY        reduce using rule 66 (special_token -> any_timestamp .)
+    TODO            reduce using rule 66 (special_token -> any_timestamp .)
+    COMMENT         reduce using rule 66 (special_token -> any_timestamp .)
+    TAGS            reduce using rule 66 (special_token -> any_timestamp .)
+    ATIMESTAMP      reduce using rule 66 (special_token -> any_timestamp .)
+    ITIMESTAMP      reduce using rule 66 (special_token -> any_timestamp .)
+    METADATA        reduce using rule 66 (special_token -> any_timestamp .)
+    STARS           reduce using rule 66 (special_token -> any_timestamp .)
+    $end            reduce using rule 66 (special_token -> any_timestamp .)
 
 
 state 29
 
-    (63) special_token -> TAGS .
+    (67) special_token -> COMMENT .
 
-    SEPARATOR       reduce using rule 63 (special_token -> TAGS .)
-    TEXT            reduce using rule 63 (special_token -> TAGS .)
-    SPACE           reduce using rule 63 (special_token -> TAGS .)
-    NEWLINE         reduce using rule 63 (special_token -> TAGS .)
-    SCHEDULING      reduce using rule 63 (special_token -> TAGS .)
-    COOKIE          reduce using rule 63 (special_token -> TAGS .)
-    PRIORITY        reduce using rule 63 (special_token -> TAGS .)
-    TODO            reduce using rule 63 (special_token -> TAGS .)
-    COMMENT         reduce using rule 63 (special_token -> TAGS .)
-    TAGS            reduce using rule 63 (special_token -> TAGS .)
-    ATIMESTAMP      reduce using rule 63 (special_token -> TAGS .)
-    ITIMESTAMP      reduce using rule 63 (special_token -> TAGS .)
-    METADATA        reduce using rule 63 (special_token -> TAGS .)
-    STARS           reduce using rule 63 (special_token -> TAGS .)
-    $end            reduce using rule 63 (special_token -> TAGS .)
+    SEPARATOR       reduce using rule 67 (special_token -> COMMENT .)
+    TEXT            reduce using rule 67 (special_token -> COMMENT .)
+    SPACE           reduce using rule 67 (special_token -> COMMENT .)
+    NEWLINE         reduce using rule 67 (special_token -> COMMENT .)
+    SCHEDULING      reduce using rule 67 (special_token -> COMMENT .)
+    COOKIE          reduce using rule 67 (special_token -> COMMENT .)
+    PRIORITY        reduce using rule 67 (special_token -> COMMENT .)
+    TODO            reduce using rule 67 (special_token -> COMMENT .)
+    COMMENT         reduce using rule 67 (special_token -> COMMENT .)
+    TAGS            reduce using rule 67 (special_token -> COMMENT .)
+    ATIMESTAMP      reduce using rule 67 (special_token -> COMMENT .)
+    ITIMESTAMP      reduce using rule 67 (special_token -> COMMENT .)
+    METADATA        reduce using rule 67 (special_token -> COMMENT .)
+    STARS           reduce using rule 67 (special_token -> COMMENT .)
+    $end            reduce using rule 67 (special_token -> COMMENT .)
 
 
 state 30
 
-    (8) metadata -> METADATA SEPARATOR .
+    (68) special_token -> TAGS .
 
-    TEXT            reduce using rule 8 (metadata -> METADATA SEPARATOR .)
-    SPACE           reduce using rule 8 (metadata -> METADATA SEPARATOR .)
-    ATIMESTAMP      reduce using rule 8 (metadata -> METADATA SEPARATOR .)
-    ITIMESTAMP      reduce using rule 8 (metadata -> METADATA SEPARATOR .)
-    STARS           reduce using rule 8 (metadata -> METADATA SEPARATOR .)
-    $end            reduce using rule 8 (metadata -> METADATA SEPARATOR .)
+    SEPARATOR       reduce using rule 68 (special_token -> TAGS .)
+    TEXT            reduce using rule 68 (special_token -> TAGS .)
+    SPACE           reduce using rule 68 (special_token -> TAGS .)
+    NEWLINE         reduce using rule 68 (special_token -> TAGS .)
+    SCHEDULING      reduce using rule 68 (special_token -> TAGS .)
+    COOKIE          reduce using rule 68 (special_token -> TAGS .)
+    PRIORITY        reduce using rule 68 (special_token -> TAGS .)
+    TODO            reduce using rule 68 (special_token -> TAGS .)
+    COMMENT         reduce using rule 68 (special_token -> TAGS .)
+    TAGS            reduce using rule 68 (special_token -> TAGS .)
+    ATIMESTAMP      reduce using rule 68 (special_token -> TAGS .)
+    ITIMESTAMP      reduce using rule 68 (special_token -> TAGS .)
+    METADATA        reduce using rule 68 (special_token -> TAGS .)
+    STARS           reduce using rule 68 (special_token -> TAGS .)
+    $end            reduce using rule 68 (special_token -> TAGS .)
 
 
 state 31
 
-    (9) metadata -> METADATA NEWLINE .
+    (10) metadata -> METADATA SEPARATOR .
 
-    TEXT            reduce using rule 9 (metadata -> METADATA NEWLINE .)
-    SPACE           reduce using rule 9 (metadata -> METADATA NEWLINE .)
-    ATIMESTAMP      reduce using rule 9 (metadata -> METADATA NEWLINE .)
-    ITIMESTAMP      reduce using rule 9 (metadata -> METADATA NEWLINE .)
-    STARS           reduce using rule 9 (metadata -> METADATA NEWLINE .)
-    $end            reduce using rule 9 (metadata -> METADATA NEWLINE .)
+    TEXT            reduce using rule 10 (metadata -> METADATA SEPARATOR .)
+    SPACE           reduce using rule 10 (metadata -> METADATA SEPARATOR .)
+    ATIMESTAMP      reduce using rule 10 (metadata -> METADATA SEPARATOR .)
+    ITIMESTAMP      reduce using rule 10 (metadata -> METADATA SEPARATOR .)
+    STARS           reduce using rule 10 (metadata -> METADATA SEPARATOR .)
+    $end            reduce using rule 10 (metadata -> METADATA SEPARATOR .)
 
 
 state 32
 
-    (11) org_tree -> heading SEPARATOR .
+    (11) metadata -> METADATA NEWLINE .
 
-    STARS           reduce using rule 11 (org_tree -> heading SEPARATOR .)
-    $end            reduce using rule 11 (org_tree -> heading SEPARATOR .)
+    TEXT            reduce using rule 11 (metadata -> METADATA NEWLINE .)
+    SPACE           reduce using rule 11 (metadata -> METADATA NEWLINE .)
+    ATIMESTAMP      reduce using rule 11 (metadata -> METADATA NEWLINE .)
+    ITIMESTAMP      reduce using rule 11 (metadata -> METADATA NEWLINE .)
+    STARS           reduce using rule 11 (metadata -> METADATA NEWLINE .)
+    $end            reduce using rule 11 (metadata -> METADATA NEWLINE .)
 
 
 state 33
 
-    (14) heading -> headline NEWLINE . contents
-    (31) contents -> . scheduling drawers body
-    (38) scheduling -> . scheduling_data
-    (39) scheduling -> . empty
-    (32) scheduling_data -> . SCHEDULING SPACE any_timestamp NEWLINE
-    (33) scheduling_data -> . SCHEDULING SPACE any_timestamp SEPARATOR
-    (34) scheduling_data -> . SCHEDULING SPACE any_timestamp SPACE
-    (35) scheduling_data -> . scheduling_data SCHEDULING SPACE any_timestamp NEWLINE
-    (36) scheduling_data -> . scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR
-    (37) scheduling_data -> . scheduling_data SCHEDULING SPACE any_timestamp SPACE
-    (73) empty -> .
+    (13) org_tree -> heading SEPARATOR .
 
-  ! shift/reduce conflict for SCHEDULING resolved as shift
-    SCHEDULING      shift and go to state 43
-    DRAWER          reduce using rule 73 (empty -> .)
-    TEXT            reduce using rule 73 (empty -> .)
-    SPACE           reduce using rule 73 (empty -> .)
-    METADATA        reduce using rule 73 (empty -> .)
-    COOKIE          reduce using rule 73 (empty -> .)
-    PRIORITY        reduce using rule 73 (empty -> .)
-    TODO            reduce using rule 73 (empty -> .)
-    COMMENT         reduce using rule 73 (empty -> .)
-    TAGS            reduce using rule 73 (empty -> .)
-    ATIMESTAMP      reduce using rule 73 (empty -> .)
-    ITIMESTAMP      reduce using rule 73 (empty -> .)
-    SEPARATOR       reduce using rule 73 (empty -> .)
-    STARS           reduce using rule 73 (empty -> .)
-    $end            reduce using rule 73 (empty -> .)
-
-  ! SCHEDULING      [ reduce using rule 73 (empty -> .) ]
-
-    contents                       shift and go to state 39
-    scheduling                     shift and go to state 40
-    scheduling_data                shift and go to state 41
-    empty                          shift and go to state 42
+    STARS           reduce using rule 13 (org_tree -> heading SEPARATOR .)
+    $end            reduce using rule 13 (org_tree -> heading SEPARATOR .)
 
-state 34
 
-    (15) heading -> headline SEPARATOR .
+state 34
 
-    SEPARATOR       reduce using rule 15 (heading -> headline SEPARATOR .)
-    STARS           reduce using rule 15 (heading -> headline SEPARATOR .)
-    $end            reduce using rule 15 (heading -> headline SEPARATOR .)
+    (16) heading -> headline NEWLINE . contents
+    (36) contents -> . scheduling drawers body
+    (43) scheduling -> . scheduling_data
+    (44) scheduling -> . empty
+    (37) scheduling_data -> . SCHEDULING SPACE any_timestamp NEWLINE
+    (38) scheduling_data -> . SCHEDULING SPACE any_timestamp SEPARATOR
+    (39) scheduling_data -> . SCHEDULING SPACE any_timestamp SPACE
+    (40) scheduling_data -> . scheduling_data SCHEDULING SPACE any_timestamp NEWLINE
+    (41) scheduling_data -> . scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR
+    (42) scheduling_data -> . scheduling_data SCHEDULING SPACE any_timestamp SPACE
+    (78) empty -> .
 
+  ! shift/reduce conflict for SCHEDULING resolved as shift
+    SCHEDULING      shift and go to state 44
+    DRAWER          reduce using rule 78 (empty -> .)
+    TEXT            reduce using rule 78 (empty -> .)
+    SPACE           reduce using rule 78 (empty -> .)
+    METADATA        reduce using rule 78 (empty -> .)
+    COOKIE          reduce using rule 78 (empty -> .)
+    PRIORITY        reduce using rule 78 (empty -> .)
+    TODO            reduce using rule 78 (empty -> .)
+    COMMENT         reduce using rule 78 (empty -> .)
+    TAGS            reduce using rule 78 (empty -> .)
+    ATIMESTAMP      reduce using rule 78 (empty -> .)
+    ITIMESTAMP      reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
+    STARS           reduce using rule 78 (empty -> .)
+    $end            reduce using rule 78 (empty -> .)
+
+  ! SCHEDULING      [ reduce using rule 78 (empty -> .) ]
+
+    contents                       shift and go to state 40
+    scheduling                     shift and go to state 41
+    scheduling_data                shift and go to state 42
+    empty                          shift and go to state 43
 
 state 35
 
-    (16) headline -> STARS SPACE . comment todo priority title cookie tags
-    (17) comment -> . COMMENT SPACE
-    (18) comment -> . empty
-    (73) empty -> .
-
-    COMMENT         shift and go to state 45
-    TODO            reduce using rule 73 (empty -> .)
-    PRIORITY        reduce using rule 73 (empty -> .)
-    TEXT            reduce using rule 73 (empty -> .)
+    (17) heading -> headline SEPARATOR .
 
-    comment                        shift and go to state 44
-    empty                          shift and go to state 46
+    SEPARATOR       reduce using rule 17 (heading -> headline SEPARATOR .)
+    STARS           reduce using rule 17 (heading -> headline SEPARATOR .)
+    $end            reduce using rule 17 (heading -> headline SEPARATOR .)
 
-state 36
 
-    (3) org_file -> metadata non_metadata_body_text SEPARATOR . org_tree
-    (4) org_file -> metadata non_metadata_body_text SEPARATOR .
-    (10) org_tree -> . heading
-    (11) org_tree -> . heading SEPARATOR
-    (12) org_tree -> . org_tree heading SEPARATOR
-    (13) org_tree -> . org_tree heading
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
-
-    $end            reduce using rule 4 (org_file -> metadata non_metadata_body_text SEPARATOR .)
-    STARS           shift and go to state 14
-
-    org_tree                       shift and go to state 47
-    heading                        shift and go to state 10
-    headline                       shift and go to state 13
+state 36
 
-state 37
+    (18) headline -> STARS SPACE . comment todo priority title cookie tags
+    (19) comment -> . COMMENT SPACE
+    (20) comment -> . empty
+    (78) empty -> .
+
+    COMMENT         shift and go to state 46
+    TODO            reduce using rule 78 (empty -> .)
+    PRIORITY        reduce using rule 78 (empty -> .)
+    TEXT            reduce using rule 78 (empty -> .)
+    SPACE           reduce using rule 78 (empty -> .)
+    COOKIE          reduce using rule 78 (empty -> .)
+    TAGS            reduce using rule 78 (empty -> .)
+    NEWLINE         reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
 
-    (12) org_tree -> org_tree heading SEPARATOR .
+    comment                        shift and go to state 45
+    empty                          shift and go to state 47
 
-    STARS           reduce using rule 12 (org_tree -> org_tree heading SEPARATOR .)
-    $end            reduce using rule 12 (org_tree -> org_tree heading SEPARATOR .)
+state 37
 
+    (4) org_file -> metadata non_metadata_body_text SEPARATOR . org_tree
+    (5) org_file -> metadata non_metadata_body_text SEPARATOR .
+    (12) org_tree -> . heading
+    (13) org_tree -> . heading SEPARATOR
+    (14) org_tree -> . org_tree heading SEPARATOR
+    (15) org_tree -> . org_tree heading
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
+
+    $end            reduce using rule 5 (org_file -> metadata non_metadata_body_text SEPARATOR .)
+    STARS           shift and go to state 15
+
+    org_tree                       shift and go to state 48
+    heading                        shift and go to state 11
+    headline                       shift and go to state 14
 
 state 38
 
-    (2) org_file -> non_metadata_body_text SEPARATOR org_tree .
-    (12) org_tree -> org_tree . heading SEPARATOR
-    (13) org_tree -> org_tree . heading
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
+    (14) org_tree -> org_tree heading SEPARATOR .
 
-    $end            reduce using rule 2 (org_file -> non_metadata_body_text SEPARATOR org_tree .)
-    STARS           shift and go to state 14
+    STARS           reduce using rule 14 (org_tree -> org_tree heading SEPARATOR .)
+    $end            reduce using rule 14 (org_tree -> org_tree heading SEPARATOR .)
 
-    heading                        shift and go to state 17
-    headline                       shift and go to state 13
 
 state 39
 
-    (14) heading -> headline NEWLINE contents .
+    (2) org_file -> non_metadata_body_text SEPARATOR org_tree .
+    (14) org_tree -> org_tree . heading SEPARATOR
+    (15) org_tree -> org_tree . heading
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
 
-    SEPARATOR       reduce using rule 14 (heading -> headline NEWLINE contents .)
-    STARS           reduce using rule 14 (heading -> headline NEWLINE contents .)
-    $end            reduce using rule 14 (heading -> headline NEWLINE contents .)
+    $end            reduce using rule 2 (org_file -> non_metadata_body_text SEPARATOR org_tree .)
+    STARS           shift and go to state 15
 
+    heading                        shift and go to state 18
+    headline                       shift and go to state 14
 
 state 40
 
-    (31) contents -> scheduling . drawers body
-    (46) drawers -> . drawer_data
-    (47) drawers -> . empty
-    (42) drawer_data -> . DRAWER NEWLINE
-    (43) drawer_data -> . DRAWER SEPARATOR
-    (44) drawer_data -> . drawer_data DRAWER NEWLINE
-    (45) drawer_data -> . drawer_data DRAWER SEPARATOR
-    (73) empty -> .
-
-    DRAWER          shift and go to state 51
-    TEXT            reduce using rule 73 (empty -> .)
-    SPACE           reduce using rule 73 (empty -> .)
-    METADATA        reduce using rule 73 (empty -> .)
-    SCHEDULING      reduce using rule 73 (empty -> .)
-    COOKIE          reduce using rule 73 (empty -> .)
-    PRIORITY        reduce using rule 73 (empty -> .)
-    TODO            reduce using rule 73 (empty -> .)
-    COMMENT         reduce using rule 73 (empty -> .)
-    TAGS            reduce using rule 73 (empty -> .)
-    ATIMESTAMP      reduce using rule 73 (empty -> .)
-    ITIMESTAMP      reduce using rule 73 (empty -> .)
-    SEPARATOR       reduce using rule 73 (empty -> .)
-    STARS           reduce using rule 73 (empty -> .)
-    $end            reduce using rule 73 (empty -> .)
-
-    drawers                        shift and go to state 48
-    drawer_data                    shift and go to state 49
-    empty                          shift and go to state 50
-
-state 41
+    (16) heading -> headline NEWLINE contents .
 
-    (38) scheduling -> scheduling_data .
-    (35) scheduling_data -> scheduling_data . SCHEDULING SPACE any_timestamp NEWLINE
-    (36) scheduling_data -> scheduling_data . SCHEDULING SPACE any_timestamp SEPARATOR
-    (37) scheduling_data -> scheduling_data . SCHEDULING SPACE any_timestamp SPACE
+    SEPARATOR       reduce using rule 16 (heading -> headline NEWLINE contents .)
+    STARS           reduce using rule 16 (heading -> headline NEWLINE contents .)
+    $end            reduce using rule 16 (heading -> headline NEWLINE contents .)
 
-  ! shift/reduce conflict for SCHEDULING resolved as shift
-    DRAWER          reduce using rule 38 (scheduling -> scheduling_data .)
-    TEXT            reduce using rule 38 (scheduling -> scheduling_data .)
-    SPACE           reduce using rule 38 (scheduling -> scheduling_data .)
-    METADATA        reduce using rule 38 (scheduling -> scheduling_data .)
-    COOKIE          reduce using rule 38 (scheduling -> scheduling_data .)
-    PRIORITY        reduce using rule 38 (scheduling -> scheduling_data .)
-    TODO            reduce using rule 38 (scheduling -> scheduling_data .)
-    COMMENT         reduce using rule 38 (scheduling -> scheduling_data .)
-    TAGS            reduce using rule 38 (scheduling -> scheduling_data .)
-    ATIMESTAMP      reduce using rule 38 (scheduling -> scheduling_data .)
-    ITIMESTAMP      reduce using rule 38 (scheduling -> scheduling_data .)
-    SEPARATOR       reduce using rule 38 (scheduling -> scheduling_data .)
-    STARS           reduce using rule 38 (scheduling -> scheduling_data .)
-    $end            reduce using rule 38 (scheduling -> scheduling_data .)
-    SCHEDULING      shift and go to state 52
 
-  ! SCHEDULING      [ reduce using rule 38 (scheduling -> scheduling_data .) ]
+state 41
 
+    (36) contents -> scheduling . drawers body
+    (51) drawers -> . drawer_data
+    (52) drawers -> . empty
+    (47) drawer_data -> . DRAWER NEWLINE
+    (48) drawer_data -> . DRAWER SEPARATOR
+    (49) drawer_data -> . drawer_data DRAWER NEWLINE
+    (50) drawer_data -> . drawer_data DRAWER SEPARATOR
+    (78) empty -> .
+
+    DRAWER          shift and go to state 52
+    TEXT            reduce using rule 78 (empty -> .)
+    SPACE           reduce using rule 78 (empty -> .)
+    METADATA        reduce using rule 78 (empty -> .)
+    SCHEDULING      reduce using rule 78 (empty -> .)
+    COOKIE          reduce using rule 78 (empty -> .)
+    PRIORITY        reduce using rule 78 (empty -> .)
+    TODO            reduce using rule 78 (empty -> .)
+    COMMENT         reduce using rule 78 (empty -> .)
+    TAGS            reduce using rule 78 (empty -> .)
+    ATIMESTAMP      reduce using rule 78 (empty -> .)
+    ITIMESTAMP      reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
+    STARS           reduce using rule 78 (empty -> .)
+    $end            reduce using rule 78 (empty -> .)
+
+    drawers                        shift and go to state 49
+    drawer_data                    shift and go to state 50
+    empty                          shift and go to state 51
 
 state 42
 
-    (39) scheduling -> empty .
+    (43) scheduling -> scheduling_data .
+    (40) scheduling_data -> scheduling_data . SCHEDULING SPACE any_timestamp NEWLINE
+    (41) scheduling_data -> scheduling_data . SCHEDULING SPACE any_timestamp SEPARATOR
+    (42) scheduling_data -> scheduling_data . SCHEDULING SPACE any_timestamp SPACE
+
+  ! shift/reduce conflict for SCHEDULING resolved as shift
+    DRAWER          reduce using rule 43 (scheduling -> scheduling_data .)
+    TEXT            reduce using rule 43 (scheduling -> scheduling_data .)
+    SPACE           reduce using rule 43 (scheduling -> scheduling_data .)
+    METADATA        reduce using rule 43 (scheduling -> scheduling_data .)
+    COOKIE          reduce using rule 43 (scheduling -> scheduling_data .)
+    PRIORITY        reduce using rule 43 (scheduling -> scheduling_data .)
+    TODO            reduce using rule 43 (scheduling -> scheduling_data .)
+    COMMENT         reduce using rule 43 (scheduling -> scheduling_data .)
+    TAGS            reduce using rule 43 (scheduling -> scheduling_data .)
+    ATIMESTAMP      reduce using rule 43 (scheduling -> scheduling_data .)
+    ITIMESTAMP      reduce using rule 43 (scheduling -> scheduling_data .)
+    SEPARATOR       reduce using rule 43 (scheduling -> scheduling_data .)
+    STARS           reduce using rule 43 (scheduling -> scheduling_data .)
+    $end            reduce using rule 43 (scheduling -> scheduling_data .)
+    SCHEDULING      shift and go to state 53
 
-    DRAWER          reduce using rule 39 (scheduling -> empty .)
-    TEXT            reduce using rule 39 (scheduling -> empty .)
-    SPACE           reduce using rule 39 (scheduling -> empty .)
-    METADATA        reduce using rule 39 (scheduling -> empty .)
-    SCHEDULING      reduce using rule 39 (scheduling -> empty .)
-    COOKIE          reduce using rule 39 (scheduling -> empty .)
-    PRIORITY        reduce using rule 39 (scheduling -> empty .)
-    TODO            reduce using rule 39 (scheduling -> empty .)
-    COMMENT         reduce using rule 39 (scheduling -> empty .)
-    TAGS            reduce using rule 39 (scheduling -> empty .)
-    ATIMESTAMP      reduce using rule 39 (scheduling -> empty .)
-    ITIMESTAMP      reduce using rule 39 (scheduling -> empty .)
-    SEPARATOR       reduce using rule 39 (scheduling -> empty .)
-    STARS           reduce using rule 39 (scheduling -> empty .)
-    $end            reduce using rule 39 (scheduling -> empty .)
+  ! SCHEDULING      [ reduce using rule 43 (scheduling -> scheduling_data .) ]
 
 
 state 43
 
-    (32) scheduling_data -> SCHEDULING . SPACE any_timestamp NEWLINE
-    (33) scheduling_data -> SCHEDULING . SPACE any_timestamp SEPARATOR
-    (34) scheduling_data -> SCHEDULING . SPACE any_timestamp SPACE
+    (44) scheduling -> empty .
 
-    SPACE           shift and go to state 53
+    DRAWER          reduce using rule 44 (scheduling -> empty .)
+    TEXT            reduce using rule 44 (scheduling -> empty .)
+    SPACE           reduce using rule 44 (scheduling -> empty .)
+    METADATA        reduce using rule 44 (scheduling -> empty .)
+    SCHEDULING      reduce using rule 44 (scheduling -> empty .)
+    COOKIE          reduce using rule 44 (scheduling -> empty .)
+    PRIORITY        reduce using rule 44 (scheduling -> empty .)
+    TODO            reduce using rule 44 (scheduling -> empty .)
+    COMMENT         reduce using rule 44 (scheduling -> empty .)
+    TAGS            reduce using rule 44 (scheduling -> empty .)
+    ATIMESTAMP      reduce using rule 44 (scheduling -> empty .)
+    ITIMESTAMP      reduce using rule 44 (scheduling -> empty .)
+    SEPARATOR       reduce using rule 44 (scheduling -> empty .)
+    STARS           reduce using rule 44 (scheduling -> empty .)
+    $end            reduce using rule 44 (scheduling -> empty .)
 
 
 state 44
 
-    (16) headline -> STARS SPACE comment . todo priority title cookie tags
-    (19) todo -> . TODO SPACE
-    (20) todo -> . empty
-    (73) empty -> .
-
-    TODO            shift and go to state 55
-    PRIORITY        reduce using rule 73 (empty -> .)
-    TEXT            reduce using rule 73 (empty -> .)
+    (37) scheduling_data -> SCHEDULING . SPACE any_timestamp NEWLINE
+    (38) scheduling_data -> SCHEDULING . SPACE any_timestamp SEPARATOR
+    (39) scheduling_data -> SCHEDULING . SPACE any_timestamp SPACE
+
+    SPACE           shift and go to state 54
 
-    todo                           shift and go to state 54
-    empty                          shift and go to state 56
 
 state 45
 
-    (17) comment -> COMMENT . SPACE
+    (18) headline -> STARS SPACE comment . todo priority title cookie tags
+    (21) todo -> . TODO SPACE
+    (22) todo -> . empty
+    (78) empty -> .
+
+  ! shift/reduce conflict for TODO resolved as shift
+    TODO            shift and go to state 56
+    PRIORITY        reduce using rule 78 (empty -> .)
+    TEXT            reduce using rule 78 (empty -> .)
+    SPACE           reduce using rule 78 (empty -> .)
+    COOKIE          reduce using rule 78 (empty -> .)
+    TAGS            reduce using rule 78 (empty -> .)
+    NEWLINE         reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
 
-    SPACE           shift and go to state 57
+  ! TODO            [ reduce using rule 78 (empty -> .) ]
 
+    todo                           shift and go to state 55
+    empty                          shift and go to state 57
 
 state 46
 
-    (18) comment -> empty .
+    (19) comment -> COMMENT . SPACE
 
-    TODO            reduce using rule 18 (comment -> empty .)
-    PRIORITY        reduce using rule 18 (comment -> empty .)
-    TEXT            reduce using rule 18 (comment -> empty .)
+    SPACE           shift and go to state 58
 
 
 state 47
 
-    (3) org_file -> metadata non_metadata_body_text SEPARATOR org_tree .
-    (12) org_tree -> org_tree . heading SEPARATOR
-    (13) org_tree -> org_tree . heading
-    (14) heading -> . headline NEWLINE contents
-    (15) heading -> . headline SEPARATOR
-    (16) headline -> . STARS SPACE comment todo priority title cookie tags
+    (20) comment -> empty .
 
-    $end            reduce using rule 3 (org_file -> metadata non_metadata_body_text SEPARATOR org_tree .)
-    STARS           shift and go to state 14
+    TODO            reduce using rule 20 (comment -> empty .)
+    PRIORITY        reduce using rule 20 (comment -> empty .)
+    TEXT            reduce using rule 20 (comment -> empty .)
+    SPACE           reduce using rule 20 (comment -> empty .)
+    COOKIE          reduce using rule 20 (comment -> empty .)
+    TAGS            reduce using rule 20 (comment -> empty .)
+    NEWLINE         reduce using rule 20 (comment -> empty .)
+    SEPARATOR       reduce using rule 20 (comment -> empty .)
 
-    heading                        shift and go to state 17
-    headline                       shift and go to state 13
 
 state 48
 
-    (31) contents -> scheduling drawers . body
-    (48) body -> . body_text
-    (49) body -> . empty
-    (64) body_text -> . TEXT
-    (65) body_text -> . SPACE
-    (66) body_text -> . METADATA
-    (67) body_text -> . special_token
-    (68) body_text -> . body_text TEXT
-    (69) body_text -> . body_text SPACE
-    (70) body_text -> . body_text special_token
-    (71) body_text -> . body_text METADATA
-    (72) body_text -> . body_text NEWLINE
-    (73) empty -> .
-    (57) special_token -> . SCHEDULING
-    (58) special_token -> . COOKIE
-    (59) special_token -> . PRIORITY
-    (60) special_token -> . TODO
-    (61) special_token -> . any_timestamp
-    (62) special_token -> . COMMENT
-    (63) special_token -> . TAGS
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
-
-    TEXT            shift and go to state 61
-    SPACE           shift and go to state 62
-    METADATA        shift and go to state 63
-    SEPARATOR       reduce using rule 73 (empty -> .)
-    STARS           reduce using rule 73 (empty -> .)
-    $end            reduce using rule 73 (empty -> .)
-    SCHEDULING      shift and go to state 23
-    COOKIE          shift and go to state 24
-    PRIORITY        shift and go to state 25
-    TODO            shift and go to state 26
-    COMMENT         shift and go to state 28
-    TAGS            shift and go to state 29
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
-
-    body                           shift and go to state 58
-    body_text                      shift and go to state 59
-    empty                          shift and go to state 60
-    special_token                  shift and go to state 64
-    any_timestamp                  shift and go to state 27
+    (4) org_file -> metadata non_metadata_body_text SEPARATOR org_tree .
+    (14) org_tree -> org_tree . heading SEPARATOR
+    (15) org_tree -> org_tree . heading
+    (16) heading -> . headline NEWLINE contents
+    (17) heading -> . headline SEPARATOR
+    (18) headline -> . STARS SPACE comment todo priority title cookie tags
 
-state 49
+    $end            reduce using rule 4 (org_file -> metadata non_metadata_body_text SEPARATOR org_tree .)
+    STARS           shift and go to state 15
+
+    heading                        shift and go to state 18
+    headline                       shift and go to state 14
 
-    (46) drawers -> drawer_data .
-    (44) drawer_data -> drawer_data . DRAWER NEWLINE
-    (45) drawer_data -> drawer_data . DRAWER SEPARATOR
-
-    TEXT            reduce using rule 46 (drawers -> drawer_data .)
-    SPACE           reduce using rule 46 (drawers -> drawer_data .)
-    METADATA        reduce using rule 46 (drawers -> drawer_data .)
-    SCHEDULING      reduce using rule 46 (drawers -> drawer_data .)
-    COOKIE          reduce using rule 46 (drawers -> drawer_data .)
-    PRIORITY        reduce using rule 46 (drawers -> drawer_data .)
-    TODO            reduce using rule 46 (drawers -> drawer_data .)
-    COMMENT         reduce using rule 46 (drawers -> drawer_data .)
-    TAGS            reduce using rule 46 (drawers -> drawer_data .)
-    ATIMESTAMP      reduce using rule 46 (drawers -> drawer_data .)
-    ITIMESTAMP      reduce using rule 46 (drawers -> drawer_data .)
-    SEPARATOR       reduce using rule 46 (drawers -> drawer_data .)
-    STARS           reduce using rule 46 (drawers -> drawer_data .)
-    $end            reduce using rule 46 (drawers -> drawer_data .)
-    DRAWER          shift and go to state 65
+state 49
 
+    (36) contents -> scheduling drawers . body
+    (53) body -> . body_text
+    (54) body -> . empty
+    (69) body_text -> . TEXT
+    (70) body_text -> . SPACE
+    (71) body_text -> . METADATA
+    (72) body_text -> . special_token
+    (73) body_text -> . body_text TEXT
+    (74) body_text -> . body_text SPACE
+    (75) body_text -> . body_text special_token
+    (76) body_text -> . body_text METADATA
+    (77) body_text -> . body_text NEWLINE
+    (78) empty -> .
+    (62) special_token -> . SCHEDULING
+    (63) special_token -> . COOKIE
+    (64) special_token -> . PRIORITY
+    (65) special_token -> . TODO
+    (66) special_token -> . any_timestamp
+    (67) special_token -> . COMMENT
+    (68) special_token -> . TAGS
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
+
+    TEXT            shift and go to state 62
+    SPACE           shift and go to state 63
+    METADATA        shift and go to state 64
+    SEPARATOR       reduce using rule 78 (empty -> .)
+    STARS           reduce using rule 78 (empty -> .)
+    $end            reduce using rule 78 (empty -> .)
+    SCHEDULING      shift and go to state 24
+    COOKIE          shift and go to state 25
+    PRIORITY        shift and go to state 26
+    TODO            shift and go to state 27
+    COMMENT         shift and go to state 29
+    TAGS            shift and go to state 30
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
+
+    body                           shift and go to state 59
+    body_text                      shift and go to state 60
+    empty                          shift and go to state 61
+    special_token                  shift and go to state 65
+    any_timestamp                  shift and go to state 28
 
 state 50
 
-    (47) drawers -> empty .
-
-    TEXT            reduce using rule 47 (drawers -> empty .)
-    SPACE           reduce using rule 47 (drawers -> empty .)
-    METADATA        reduce using rule 47 (drawers -> empty .)
-    SCHEDULING      reduce using rule 47 (drawers -> empty .)
-    COOKIE          reduce using rule 47 (drawers -> empty .)
-    PRIORITY        reduce using rule 47 (drawers -> empty .)
-    TODO            reduce using rule 47 (drawers -> empty .)
-    COMMENT         reduce using rule 47 (drawers -> empty .)
-    TAGS            reduce using rule 47 (drawers -> empty .)
-    ATIMESTAMP      reduce using rule 47 (drawers -> empty .)
-    ITIMESTAMP      reduce using rule 47 (drawers -> empty .)
-    SEPARATOR       reduce using rule 47 (drawers -> empty .)
-    STARS           reduce using rule 47 (drawers -> empty .)
-    $end            reduce using rule 47 (drawers -> empty .)
+    (51) drawers -> drawer_data .
+    (49) drawer_data -> drawer_data . DRAWER NEWLINE
+    (50) drawer_data -> drawer_data . DRAWER SEPARATOR
+
+    TEXT            reduce using rule 51 (drawers -> drawer_data .)
+    SPACE           reduce using rule 51 (drawers -> drawer_data .)
+    METADATA        reduce using rule 51 (drawers -> drawer_data .)
+    SCHEDULING      reduce using rule 51 (drawers -> drawer_data .)
+    COOKIE          reduce using rule 51 (drawers -> drawer_data .)
+    PRIORITY        reduce using rule 51 (drawers -> drawer_data .)
+    TODO            reduce using rule 51 (drawers -> drawer_data .)
+    COMMENT         reduce using rule 51 (drawers -> drawer_data .)
+    TAGS            reduce using rule 51 (drawers -> drawer_data .)
+    ATIMESTAMP      reduce using rule 51 (drawers -> drawer_data .)
+    ITIMESTAMP      reduce using rule 51 (drawers -> drawer_data .)
+    SEPARATOR       reduce using rule 51 (drawers -> drawer_data .)
+    STARS           reduce using rule 51 (drawers -> drawer_data .)
+    $end            reduce using rule 51 (drawers -> drawer_data .)
+    DRAWER          shift and go to state 66
 
 
 state 51
 
-    (42) drawer_data -> DRAWER . NEWLINE
-    (43) drawer_data -> DRAWER . SEPARATOR
+    (52) drawers -> empty .
 
-    NEWLINE         shift and go to state 66
-    SEPARATOR       shift and go to state 67
+    TEXT            reduce using rule 52 (drawers -> empty .)
+    SPACE           reduce using rule 52 (drawers -> empty .)
+    METADATA        reduce using rule 52 (drawers -> empty .)
+    SCHEDULING      reduce using rule 52 (drawers -> empty .)
+    COOKIE          reduce using rule 52 (drawers -> empty .)
+    PRIORITY        reduce using rule 52 (drawers -> empty .)
+    TODO            reduce using rule 52 (drawers -> empty .)
+    COMMENT         reduce using rule 52 (drawers -> empty .)
+    TAGS            reduce using rule 52 (drawers -> empty .)
+    ATIMESTAMP      reduce using rule 52 (drawers -> empty .)
+    ITIMESTAMP      reduce using rule 52 (drawers -> empty .)
+    SEPARATOR       reduce using rule 52 (drawers -> empty .)
+    STARS           reduce using rule 52 (drawers -> empty .)
+    $end            reduce using rule 52 (drawers -> empty .)
 
 
 state 52
 
-    (35) scheduling_data -> scheduling_data SCHEDULING . SPACE any_timestamp NEWLINE
-    (36) scheduling_data -> scheduling_data SCHEDULING . SPACE any_timestamp SEPARATOR
-    (37) scheduling_data -> scheduling_data SCHEDULING . SPACE any_timestamp SPACE
+    (47) drawer_data -> DRAWER . NEWLINE
+    (48) drawer_data -> DRAWER . SEPARATOR
 
-    SPACE           shift and go to state 68
+    NEWLINE         shift and go to state 67
+    SEPARATOR       shift and go to state 68
 
 
 state 53
 
-    (32) scheduling_data -> SCHEDULING SPACE . any_timestamp NEWLINE
-    (33) scheduling_data -> SCHEDULING SPACE . any_timestamp SEPARATOR
-    (34) scheduling_data -> SCHEDULING SPACE . any_timestamp SPACE
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
+    (40) scheduling_data -> scheduling_data SCHEDULING . SPACE any_timestamp NEWLINE
+    (41) scheduling_data -> scheduling_data SCHEDULING . SPACE any_timestamp SEPARATOR
+    (42) scheduling_data -> scheduling_data SCHEDULING . SPACE any_timestamp SPACE
 
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
+    SPACE           shift and go to state 69
 
-    any_timestamp                  shift and go to state 69
 
 state 54
 
-    (16) headline -> STARS SPACE comment todo . priority title cookie tags
-    (21) priority -> . PRIORITY SPACE
-    (22) priority -> . empty
-    (73) empty -> .
+    (37) scheduling_data -> SCHEDULING SPACE . any_timestamp NEWLINE
+    (38) scheduling_data -> SCHEDULING SPACE . any_timestamp SEPARATOR
+    (39) scheduling_data -> SCHEDULING SPACE . any_timestamp SPACE
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
 
-    PRIORITY        shift and go to state 71
-    TEXT            reduce using rule 73 (empty -> .)
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
 
-    priority                       shift and go to state 70
-    empty                          shift and go to state 72
+    any_timestamp                  shift and go to state 70
 
 state 55
 
-    (19) todo -> TODO . SPACE
-
-    SPACE           shift and go to state 73
+    (18) headline -> STARS SPACE comment todo . priority title cookie tags
+    (23) priority -> . PRIORITY SPACE
+    (24) priority -> . empty
+    (78) empty -> .
+
+    PRIORITY        shift and go to state 72
+    TEXT            reduce using rule 78 (empty -> .)
+    TODO            reduce using rule 78 (empty -> .)
+    SPACE           reduce using rule 78 (empty -> .)
+    COOKIE          reduce using rule 78 (empty -> .)
+    TAGS            reduce using rule 78 (empty -> .)
+    NEWLINE         reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
 
+    priority                       shift and go to state 71
+    empty                          shift and go to state 73
 
 state 56
 
-    (20) todo -> empty .
+    (21) todo -> TODO . SPACE
 
-    PRIORITY        reduce using rule 20 (todo -> empty .)
-    TEXT            reduce using rule 20 (todo -> empty .)
+    SPACE           shift and go to state 74
 
 
 state 57
 
-    (17) comment -> COMMENT SPACE .
+    (22) todo -> empty .
 
-    TODO            reduce using rule 17 (comment -> COMMENT SPACE .)
-    PRIORITY        reduce using rule 17 (comment -> COMMENT SPACE .)
-    TEXT            reduce using rule 17 (comment -> COMMENT SPACE .)
+    PRIORITY        reduce using rule 22 (todo -> empty .)
+    TEXT            reduce using rule 22 (todo -> empty .)
+    TODO            reduce using rule 22 (todo -> empty .)
+    SPACE           reduce using rule 22 (todo -> empty .)
+    COOKIE          reduce using rule 22 (todo -> empty .)
+    TAGS            reduce using rule 22 (todo -> empty .)
+    NEWLINE         reduce using rule 22 (todo -> empty .)
+    SEPARATOR       reduce using rule 22 (todo -> empty .)
 
 
 state 58
 
-    (31) contents -> scheduling drawers body .
+    (19) comment -> COMMENT SPACE .
 
-    SEPARATOR       reduce using rule 31 (contents -> scheduling drawers body .)
-    STARS           reduce using rule 31 (contents -> scheduling drawers body .)
-    $end            reduce using rule 31 (contents -> scheduling drawers body .)
+    TODO            reduce using rule 19 (comment -> COMMENT SPACE .)
+    PRIORITY        reduce using rule 19 (comment -> COMMENT SPACE .)
+    TEXT            reduce using rule 19 (comment -> COMMENT SPACE .)
+    SPACE           reduce using rule 19 (comment -> COMMENT SPACE .)
+    COOKIE          reduce using rule 19 (comment -> COMMENT SPACE .)
+    TAGS            reduce using rule 19 (comment -> COMMENT SPACE .)
+    NEWLINE         reduce using rule 19 (comment -> COMMENT SPACE .)
+    SEPARATOR       reduce using rule 19 (comment -> COMMENT SPACE .)
 
 
 state 59
 
-    (48) body -> body_text .
-    (68) body_text -> body_text . TEXT
-    (69) body_text -> body_text . SPACE
-    (70) body_text -> body_text . special_token
-    (71) body_text -> body_text . METADATA
-    (72) body_text -> body_text . NEWLINE
-    (57) special_token -> . SCHEDULING
-    (58) special_token -> . COOKIE
-    (59) special_token -> . PRIORITY
-    (60) special_token -> . TODO
-    (61) special_token -> . any_timestamp
-    (62) special_token -> . COMMENT
-    (63) special_token -> . TAGS
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
-
-    SEPARATOR       reduce using rule 48 (body -> body_text .)
-    STARS           reduce using rule 48 (body -> body_text .)
-    $end            reduce using rule 48 (body -> body_text .)
-    TEXT            shift and go to state 74
-    SPACE           shift and go to state 75
-    METADATA        shift and go to state 77
-    NEWLINE         shift and go to state 78
-    SCHEDULING      shift and go to state 23
-    COOKIE          shift and go to state 24
-    PRIORITY        shift and go to state 25
-    TODO            shift and go to state 26
-    COMMENT         shift and go to state 28
-    TAGS            shift and go to state 29
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
+    (36) contents -> scheduling drawers body .
 
-    special_token                  shift and go to state 76
-    any_timestamp                  shift and go to state 27
+    SEPARATOR       reduce using rule 36 (contents -> scheduling drawers body .)
+    STARS           reduce using rule 36 (contents -> scheduling drawers body .)
+    $end            reduce using rule 36 (contents -> scheduling drawers body .)
 
-state 60
 
-    (49) body -> empty .
+state 60
 
-    SEPARATOR       reduce using rule 49 (body -> empty .)
-    STARS           reduce using rule 49 (body -> empty .)
-    $end            reduce using rule 49 (body -> empty .)
+    (53) body -> body_text .
+    (73) body_text -> body_text . TEXT
+    (74) body_text -> body_text . SPACE
+    (75) body_text -> body_text . special_token
+    (76) body_text -> body_text . METADATA
+    (77) body_text -> body_text . NEWLINE
+    (62) special_token -> . SCHEDULING
+    (63) special_token -> . COOKIE
+    (64) special_token -> . PRIORITY
+    (65) special_token -> . TODO
+    (66) special_token -> . any_timestamp
+    (67) special_token -> . COMMENT
+    (68) special_token -> . TAGS
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
+
+    SEPARATOR       reduce using rule 53 (body -> body_text .)
+    STARS           reduce using rule 53 (body -> body_text .)
+    $end            reduce using rule 53 (body -> body_text .)
+    TEXT            shift and go to state 75
+    SPACE           shift and go to state 76
+    METADATA        shift and go to state 78
+    NEWLINE         shift and go to state 79
+    SCHEDULING      shift and go to state 24
+    COOKIE          shift and go to state 25
+    PRIORITY        shift and go to state 26
+    TODO            shift and go to state 27
+    COMMENT         shift and go to state 29
+    TAGS            shift and go to state 30
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
 
+    special_token                  shift and go to state 77
+    any_timestamp                  shift and go to state 28
 
 state 61
 
-    (64) body_text -> TEXT .
+    (54) body -> empty .
 
-    TEXT            reduce using rule 64 (body_text -> TEXT .)
-    SPACE           reduce using rule 64 (body_text -> TEXT .)
-    METADATA        reduce using rule 64 (body_text -> TEXT .)
-    NEWLINE         reduce using rule 64 (body_text -> TEXT .)
-    SCHEDULING      reduce using rule 64 (body_text -> TEXT .)
-    COOKIE          reduce using rule 64 (body_text -> TEXT .)
-    PRIORITY        reduce using rule 64 (body_text -> TEXT .)
-    TODO            reduce using rule 64 (body_text -> TEXT .)
-    COMMENT         reduce using rule 64 (body_text -> TEXT .)
-    TAGS            reduce using rule 64 (body_text -> TEXT .)
-    ATIMESTAMP      reduce using rule 64 (body_text -> TEXT .)
-    ITIMESTAMP      reduce using rule 64 (body_text -> TEXT .)
-    SEPARATOR       reduce using rule 64 (body_text -> TEXT .)
-    STARS           reduce using rule 64 (body_text -> TEXT .)
-    $end            reduce using rule 64 (body_text -> TEXT .)
+    SEPARATOR       reduce using rule 54 (body -> empty .)
+    STARS           reduce using rule 54 (body -> empty .)
+    $end            reduce using rule 54 (body -> empty .)
 
 
 state 62
 
-    (65) body_text -> SPACE .
+    (69) body_text -> TEXT .
 
-    TEXT            reduce using rule 65 (body_text -> SPACE .)
-    SPACE           reduce using rule 65 (body_text -> SPACE .)
-    METADATA        reduce using rule 65 (body_text -> SPACE .)
-    NEWLINE         reduce using rule 65 (body_text -> SPACE .)
-    SCHEDULING      reduce using rule 65 (body_text -> SPACE .)
-    COOKIE          reduce using rule 65 (body_text -> SPACE .)
-    PRIORITY        reduce using rule 65 (body_text -> SPACE .)
-    TODO            reduce using rule 65 (body_text -> SPACE .)
-    COMMENT         reduce using rule 65 (body_text -> SPACE .)
-    TAGS            reduce using rule 65 (body_text -> SPACE .)
-    ATIMESTAMP      reduce using rule 65 (body_text -> SPACE .)
-    ITIMESTAMP      reduce using rule 65 (body_text -> SPACE .)
-    SEPARATOR       reduce using rule 65 (body_text -> SPACE .)
-    STARS           reduce using rule 65 (body_text -> SPACE .)
-    $end            reduce using rule 65 (body_text -> SPACE .)
+    TEXT            reduce using rule 69 (body_text -> TEXT .)
+    SPACE           reduce using rule 69 (body_text -> TEXT .)
+    METADATA        reduce using rule 69 (body_text -> TEXT .)
+    NEWLINE         reduce using rule 69 (body_text -> TEXT .)
+    SCHEDULING      reduce using rule 69 (body_text -> TEXT .)
+    COOKIE          reduce using rule 69 (body_text -> TEXT .)
+    PRIORITY        reduce using rule 69 (body_text -> TEXT .)
+    TODO            reduce using rule 69 (body_text -> TEXT .)
+    COMMENT         reduce using rule 69 (body_text -> TEXT .)
+    TAGS            reduce using rule 69 (body_text -> TEXT .)
+    ATIMESTAMP      reduce using rule 69 (body_text -> TEXT .)
+    ITIMESTAMP      reduce using rule 69 (body_text -> TEXT .)
+    SEPARATOR       reduce using rule 69 (body_text -> TEXT .)
+    STARS           reduce using rule 69 (body_text -> TEXT .)
+    $end            reduce using rule 69 (body_text -> TEXT .)
 
 
 state 63
 
-    (66) body_text -> METADATA .
+    (70) body_text -> SPACE .
 
-    TEXT            reduce using rule 66 (body_text -> METADATA .)
-    SPACE           reduce using rule 66 (body_text -> METADATA .)
-    METADATA        reduce using rule 66 (body_text -> METADATA .)
-    NEWLINE         reduce using rule 66 (body_text -> METADATA .)
-    SCHEDULING      reduce using rule 66 (body_text -> METADATA .)
-    COOKIE          reduce using rule 66 (body_text -> METADATA .)
-    PRIORITY        reduce using rule 66 (body_text -> METADATA .)
-    TODO            reduce using rule 66 (body_text -> METADATA .)
-    COMMENT         reduce using rule 66 (body_text -> METADATA .)
-    TAGS            reduce using rule 66 (body_text -> METADATA .)
-    ATIMESTAMP      reduce using rule 66 (body_text -> METADATA .)
-    ITIMESTAMP      reduce using rule 66 (body_text -> METADATA .)
-    SEPARATOR       reduce using rule 66 (body_text -> METADATA .)
-    STARS           reduce using rule 66 (body_text -> METADATA .)
-    $end            reduce using rule 66 (body_text -> METADATA .)
+    TEXT            reduce using rule 70 (body_text -> SPACE .)
+    SPACE           reduce using rule 70 (body_text -> SPACE .)
+    METADATA        reduce using rule 70 (body_text -> SPACE .)
+    NEWLINE         reduce using rule 70 (body_text -> SPACE .)
+    SCHEDULING      reduce using rule 70 (body_text -> SPACE .)
+    COOKIE          reduce using rule 70 (body_text -> SPACE .)
+    PRIORITY        reduce using rule 70 (body_text -> SPACE .)
+    TODO            reduce using rule 70 (body_text -> SPACE .)
+    COMMENT         reduce using rule 70 (body_text -> SPACE .)
+    TAGS            reduce using rule 70 (body_text -> SPACE .)
+    ATIMESTAMP      reduce using rule 70 (body_text -> SPACE .)
+    ITIMESTAMP      reduce using rule 70 (body_text -> SPACE .)
+    SEPARATOR       reduce using rule 70 (body_text -> SPACE .)
+    STARS           reduce using rule 70 (body_text -> SPACE .)
+    $end            reduce using rule 70 (body_text -> SPACE .)
 
 
 state 64
 
-    (67) body_text -> special_token .
+    (71) body_text -> METADATA .
 
-    TEXT            reduce using rule 67 (body_text -> special_token .)
-    SPACE           reduce using rule 67 (body_text -> special_token .)
-    METADATA        reduce using rule 67 (body_text -> special_token .)
-    NEWLINE         reduce using rule 67 (body_text -> special_token .)
-    SCHEDULING      reduce using rule 67 (body_text -> special_token .)
-    COOKIE          reduce using rule 67 (body_text -> special_token .)
-    PRIORITY        reduce using rule 67 (body_text -> special_token .)
-    TODO            reduce using rule 67 (body_text -> special_token .)
-    COMMENT         reduce using rule 67 (body_text -> special_token .)
-    TAGS            reduce using rule 67 (body_text -> special_token .)
-    ATIMESTAMP      reduce using rule 67 (body_text -> special_token .)
-    ITIMESTAMP      reduce using rule 67 (body_text -> special_token .)
-    SEPARATOR       reduce using rule 67 (body_text -> special_token .)
-    STARS           reduce using rule 67 (body_text -> special_token .)
-    $end            reduce using rule 67 (body_text -> special_token .)
+    TEXT            reduce using rule 71 (body_text -> METADATA .)
+    SPACE           reduce using rule 71 (body_text -> METADATA .)
+    METADATA        reduce using rule 71 (body_text -> METADATA .)
+    NEWLINE         reduce using rule 71 (body_text -> METADATA .)
+    SCHEDULING      reduce using rule 71 (body_text -> METADATA .)
+    COOKIE          reduce using rule 71 (body_text -> METADATA .)
+    PRIORITY        reduce using rule 71 (body_text -> METADATA .)
+    TODO            reduce using rule 71 (body_text -> METADATA .)
+    COMMENT         reduce using rule 71 (body_text -> METADATA .)
+    TAGS            reduce using rule 71 (body_text -> METADATA .)
+    ATIMESTAMP      reduce using rule 71 (body_text -> METADATA .)
+    ITIMESTAMP      reduce using rule 71 (body_text -> METADATA .)
+    SEPARATOR       reduce using rule 71 (body_text -> METADATA .)
+    STARS           reduce using rule 71 (body_text -> METADATA .)
+    $end            reduce using rule 71 (body_text -> METADATA .)
 
 
 state 65
 
-    (44) drawer_data -> drawer_data DRAWER . NEWLINE
-    (45) drawer_data -> drawer_data DRAWER . SEPARATOR
+    (72) body_text -> special_token .
 
-    NEWLINE         shift and go to state 79
-    SEPARATOR       shift and go to state 80
+    TEXT            reduce using rule 72 (body_text -> special_token .)
+    SPACE           reduce using rule 72 (body_text -> special_token .)
+    METADATA        reduce using rule 72 (body_text -> special_token .)
+    NEWLINE         reduce using rule 72 (body_text -> special_token .)
+    SCHEDULING      reduce using rule 72 (body_text -> special_token .)
+    COOKIE          reduce using rule 72 (body_text -> special_token .)
+    PRIORITY        reduce using rule 72 (body_text -> special_token .)
+    TODO            reduce using rule 72 (body_text -> special_token .)
+    COMMENT         reduce using rule 72 (body_text -> special_token .)
+    TAGS            reduce using rule 72 (body_text -> special_token .)
+    ATIMESTAMP      reduce using rule 72 (body_text -> special_token .)
+    ITIMESTAMP      reduce using rule 72 (body_text -> special_token .)
+    SEPARATOR       reduce using rule 72 (body_text -> special_token .)
+    STARS           reduce using rule 72 (body_text -> special_token .)
+    $end            reduce using rule 72 (body_text -> special_token .)
 
 
 state 66
 
-    (42) drawer_data -> DRAWER NEWLINE .
+    (49) drawer_data -> drawer_data DRAWER . NEWLINE
+    (50) drawer_data -> drawer_data DRAWER . SEPARATOR
 
-    DRAWER          reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    TEXT            reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    SPACE           reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    METADATA        reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    SCHEDULING      reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    COOKIE          reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    PRIORITY        reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    TODO            reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    COMMENT         reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    TAGS            reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    ATIMESTAMP      reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    ITIMESTAMP      reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    SEPARATOR       reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    STARS           reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
-    $end            reduce using rule 42 (drawer_data -> DRAWER NEWLINE .)
+    NEWLINE         shift and go to state 80
+    SEPARATOR       shift and go to state 81
 
 
 state 67
 
-    (43) drawer_data -> DRAWER SEPARATOR .
+    (47) drawer_data -> DRAWER NEWLINE .
 
-    DRAWER          reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    TEXT            reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    SPACE           reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    METADATA        reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    SCHEDULING      reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    COOKIE          reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    PRIORITY        reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    TODO            reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    COMMENT         reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    TAGS            reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    ATIMESTAMP      reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    ITIMESTAMP      reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    SEPARATOR       reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    STARS           reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
-    $end            reduce using rule 43 (drawer_data -> DRAWER SEPARATOR .)
+    DRAWER          reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    TEXT            reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    SPACE           reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    METADATA        reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    SCHEDULING      reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    COOKIE          reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    PRIORITY        reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    TODO            reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    COMMENT         reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    TAGS            reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    ATIMESTAMP      reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    ITIMESTAMP      reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    SEPARATOR       reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    STARS           reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
+    $end            reduce using rule 47 (drawer_data -> DRAWER NEWLINE .)
 
 
 state 68
 
-    (35) scheduling_data -> scheduling_data SCHEDULING SPACE . any_timestamp NEWLINE
-    (36) scheduling_data -> scheduling_data SCHEDULING SPACE . any_timestamp SEPARATOR
-    (37) scheduling_data -> scheduling_data SCHEDULING SPACE . any_timestamp SPACE
-    (40) any_timestamp -> . ATIMESTAMP
-    (41) any_timestamp -> . ITIMESTAMP
+    (48) drawer_data -> DRAWER SEPARATOR .
 
-    ATIMESTAMP      shift and go to state 11
-    ITIMESTAMP      shift and go to state 12
+    DRAWER          reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    TEXT            reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    SPACE           reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    METADATA        reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    SCHEDULING      reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    COOKIE          reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    PRIORITY        reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    TODO            reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    COMMENT         reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    TAGS            reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    ATIMESTAMP      reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    ITIMESTAMP      reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    SEPARATOR       reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    STARS           reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
+    $end            reduce using rule 48 (drawer_data -> DRAWER SEPARATOR .)
 
-    any_timestamp                  shift and go to state 81
 
 state 69
 
-    (32) scheduling_data -> SCHEDULING SPACE any_timestamp . NEWLINE
-    (33) scheduling_data -> SCHEDULING SPACE any_timestamp . SEPARATOR
-    (34) scheduling_data -> SCHEDULING SPACE any_timestamp . SPACE
-
-    NEWLINE         shift and go to state 83
-    SEPARATOR       shift and go to state 84
-    SPACE           shift and go to state 82
+    (40) scheduling_data -> scheduling_data SCHEDULING SPACE . any_timestamp NEWLINE
+    (41) scheduling_data -> scheduling_data SCHEDULING SPACE . any_timestamp SEPARATOR
+    (42) scheduling_data -> scheduling_data SCHEDULING SPACE . any_timestamp SPACE
+    (45) any_timestamp -> . ATIMESTAMP
+    (46) any_timestamp -> . ITIMESTAMP
 
+    ATIMESTAMP      shift and go to state 12
+    ITIMESTAMP      shift and go to state 13
 
-state 70
+    any_timestamp                  shift and go to state 82
 
-    (16) headline -> STARS SPACE comment todo priority . title cookie tags
-    (23) title -> . TEXT
-    (24) title -> . title SPACE TEXT
-    (25) title -> . title SPACE
+state 70
 
-    TEXT            shift and go to state 86
+    (37) scheduling_data -> SCHEDULING SPACE any_timestamp . NEWLINE
+    (38) scheduling_data -> SCHEDULING SPACE any_timestamp . SEPARATOR
+    (39) scheduling_data -> SCHEDULING SPACE any_timestamp . SPACE
+
+    NEWLINE         shift and go to state 84
+    SEPARATOR       shift and go to state 85
+    SPACE           shift and go to state 83
 
-    title                          shift and go to state 85
 
 state 71
 
-    (21) priority -> PRIORITY . SPACE
-
-    SPACE           shift and go to state 87
+    (18) headline -> STARS SPACE comment todo priority . title cookie tags
+    (25) title -> . TEXT
+    (26) title -> . TODO
+    (27) title -> . title SPACE TEXT
+    (28) title -> . title SPACE TODO
+    (29) title -> . title SPACE
+    (30) title -> . empty
+    (78) empty -> .
+
+    TEXT            shift and go to state 87
+    TODO            shift and go to state 88
+    SPACE           reduce using rule 78 (empty -> .)
+    COOKIE          reduce using rule 78 (empty -> .)
+    TAGS            reduce using rule 78 (empty -> .)
+    NEWLINE         reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
 
+    title                          shift and go to state 86
+    empty                          shift and go to state 89
 
 state 72
 
-    (22) priority -> empty .
+    (23) priority -> PRIORITY . SPACE
 
-    TEXT            reduce using rule 22 (priority -> empty .)
+    SPACE           shift and go to state 90
 
 
 state 73
 
-    (19) todo -> TODO SPACE .
+    (24) priority -> empty .
 
-    PRIORITY        reduce using rule 19 (todo -> TODO SPACE .)
-    TEXT            reduce using rule 19 (todo -> TODO SPACE .)
+    TEXT            reduce using rule 24 (priority -> empty .)
+    TODO            reduce using rule 24 (priority -> empty .)
+    SPACE           reduce using rule 24 (priority -> empty .)
+    COOKIE          reduce using rule 24 (priority -> empty .)
+    TAGS            reduce using rule 24 (priority -> empty .)
+    NEWLINE         reduce using rule 24 (priority -> empty .)
+    SEPARATOR       reduce using rule 24 (priority -> empty .)
 
 
 state 74
 
-    (68) body_text -> body_text TEXT .
+    (21) todo -> TODO SPACE .
 
-    TEXT            reduce using rule 68 (body_text -> body_text TEXT .)
-    SPACE           reduce using rule 68 (body_text -> body_text TEXT .)
-    METADATA        reduce using rule 68 (body_text -> body_text TEXT .)
-    NEWLINE         reduce using rule 68 (body_text -> body_text TEXT .)
-    SCHEDULING      reduce using rule 68 (body_text -> body_text TEXT .)
-    COOKIE          reduce using rule 68 (body_text -> body_text TEXT .)
-    PRIORITY        reduce using rule 68 (body_text -> body_text TEXT .)
-    TODO            reduce using rule 68 (body_text -> body_text TEXT .)
-    COMMENT         reduce using rule 68 (body_text -> body_text TEXT .)
-    TAGS            reduce using rule 68 (body_text -> body_text TEXT .)
-    ATIMESTAMP      reduce using rule 68 (body_text -> body_text TEXT .)
-    ITIMESTAMP      reduce using rule 68 (body_text -> body_text TEXT .)
-    SEPARATOR       reduce using rule 68 (body_text -> body_text TEXT .)
-    STARS           reduce using rule 68 (body_text -> body_text TEXT .)
-    $end            reduce using rule 68 (body_text -> body_text TEXT .)
+    PRIORITY        reduce using rule 21 (todo -> TODO SPACE .)
+    TEXT            reduce using rule 21 (todo -> TODO SPACE .)
+    TODO            reduce using rule 21 (todo -> TODO SPACE .)
+    SPACE           reduce using rule 21 (todo -> TODO SPACE .)
+    COOKIE          reduce using rule 21 (todo -> TODO SPACE .)
+    TAGS            reduce using rule 21 (todo -> TODO SPACE .)
+    NEWLINE         reduce using rule 21 (todo -> TODO SPACE .)
+    SEPARATOR       reduce using rule 21 (todo -> TODO SPACE .)
 
 
 state 75
 
-    (69) body_text -> body_text SPACE .
+    (73) body_text -> body_text TEXT .
 
-    TEXT            reduce using rule 69 (body_text -> body_text SPACE .)
-    SPACE           reduce using rule 69 (body_text -> body_text SPACE .)
-    METADATA        reduce using rule 69 (body_text -> body_text SPACE .)
-    NEWLINE         reduce using rule 69 (body_text -> body_text SPACE .)
-    SCHEDULING      reduce using rule 69 (body_text -> body_text SPACE .)
-    COOKIE          reduce using rule 69 (body_text -> body_text SPACE .)
-    PRIORITY        reduce using rule 69 (body_text -> body_text SPACE .)
-    TODO            reduce using rule 69 (body_text -> body_text SPACE .)
-    COMMENT         reduce using rule 69 (body_text -> body_text SPACE .)
-    TAGS            reduce using rule 69 (body_text -> body_text SPACE .)
-    ATIMESTAMP      reduce using rule 69 (body_text -> body_text SPACE .)
-    ITIMESTAMP      reduce using rule 69 (body_text -> body_text SPACE .)
-    SEPARATOR       reduce using rule 69 (body_text -> body_text SPACE .)
-    STARS           reduce using rule 69 (body_text -> body_text SPACE .)
-    $end            reduce using rule 69 (body_text -> body_text SPACE .)
+    TEXT            reduce using rule 73 (body_text -> body_text TEXT .)
+    SPACE           reduce using rule 73 (body_text -> body_text TEXT .)
+    METADATA        reduce using rule 73 (body_text -> body_text TEXT .)
+    NEWLINE         reduce using rule 73 (body_text -> body_text TEXT .)
+    SCHEDULING      reduce using rule 73 (body_text -> body_text TEXT .)
+    COOKIE          reduce using rule 73 (body_text -> body_text TEXT .)
+    PRIORITY        reduce using rule 73 (body_text -> body_text TEXT .)
+    TODO            reduce using rule 73 (body_text -> body_text TEXT .)
+    COMMENT         reduce using rule 73 (body_text -> body_text TEXT .)
+    TAGS            reduce using rule 73 (body_text -> body_text TEXT .)
+    ATIMESTAMP      reduce using rule 73 (body_text -> body_text TEXT .)
+    ITIMESTAMP      reduce using rule 73 (body_text -> body_text TEXT .)
+    SEPARATOR       reduce using rule 73 (body_text -> body_text TEXT .)
+    STARS           reduce using rule 73 (body_text -> body_text TEXT .)
+    $end            reduce using rule 73 (body_text -> body_text TEXT .)
 
 
 state 76
 
-    (70) body_text -> body_text special_token .
+    (74) body_text -> body_text SPACE .
 
-    TEXT            reduce using rule 70 (body_text -> body_text special_token .)
-    SPACE           reduce using rule 70 (body_text -> body_text special_token .)
-    METADATA        reduce using rule 70 (body_text -> body_text special_token .)
-    NEWLINE         reduce using rule 70 (body_text -> body_text special_token .)
-    SCHEDULING      reduce using rule 70 (body_text -> body_text special_token .)
-    COOKIE          reduce using rule 70 (body_text -> body_text special_token .)
-    PRIORITY        reduce using rule 70 (body_text -> body_text special_token .)
-    TODO            reduce using rule 70 (body_text -> body_text special_token .)
-    COMMENT         reduce using rule 70 (body_text -> body_text special_token .)
-    TAGS            reduce using rule 70 (body_text -> body_text special_token .)
-    ATIMESTAMP      reduce using rule 70 (body_text -> body_text special_token .)
-    ITIMESTAMP      reduce using rule 70 (body_text -> body_text special_token .)
-    SEPARATOR       reduce using rule 70 (body_text -> body_text special_token .)
-    STARS           reduce using rule 70 (body_text -> body_text special_token .)
-    $end            reduce using rule 70 (body_text -> body_text special_token .)
+    TEXT            reduce using rule 74 (body_text -> body_text SPACE .)
+    SPACE           reduce using rule 74 (body_text -> body_text SPACE .)
+    METADATA        reduce using rule 74 (body_text -> body_text SPACE .)
+    NEWLINE         reduce using rule 74 (body_text -> body_text SPACE .)
+    SCHEDULING      reduce using rule 74 (body_text -> body_text SPACE .)
+    COOKIE          reduce using rule 74 (body_text -> body_text SPACE .)
+    PRIORITY        reduce using rule 74 (body_text -> body_text SPACE .)
+    TODO            reduce using rule 74 (body_text -> body_text SPACE .)
+    COMMENT         reduce using rule 74 (body_text -> body_text SPACE .)
+    TAGS            reduce using rule 74 (body_text -> body_text SPACE .)
+    ATIMESTAMP      reduce using rule 74 (body_text -> body_text SPACE .)
+    ITIMESTAMP      reduce using rule 74 (body_text -> body_text SPACE .)
+    SEPARATOR       reduce using rule 74 (body_text -> body_text SPACE .)
+    STARS           reduce using rule 74 (body_text -> body_text SPACE .)
+    $end            reduce using rule 74 (body_text -> body_text SPACE .)
 
 
 state 77
 
-    (71) body_text -> body_text METADATA .
+    (75) body_text -> body_text special_token .
 
-    TEXT            reduce using rule 71 (body_text -> body_text METADATA .)
-    SPACE           reduce using rule 71 (body_text -> body_text METADATA .)
-    METADATA        reduce using rule 71 (body_text -> body_text METADATA .)
-    NEWLINE         reduce using rule 71 (body_text -> body_text METADATA .)
-    SCHEDULING      reduce using rule 71 (body_text -> body_text METADATA .)
-    COOKIE          reduce using rule 71 (body_text -> body_text METADATA .)
-    PRIORITY        reduce using rule 71 (body_text -> body_text METADATA .)
-    TODO            reduce using rule 71 (body_text -> body_text METADATA .)
-    COMMENT         reduce using rule 71 (body_text -> body_text METADATA .)
-    TAGS            reduce using rule 71 (body_text -> body_text METADATA .)
-    ATIMESTAMP      reduce using rule 71 (body_text -> body_text METADATA .)
-    ITIMESTAMP      reduce using rule 71 (body_text -> body_text METADATA .)
-    SEPARATOR       reduce using rule 71 (body_text -> body_text METADATA .)
-    STARS           reduce using rule 71 (body_text -> body_text METADATA .)
-    $end            reduce using rule 71 (body_text -> body_text METADATA .)
+    TEXT            reduce using rule 75 (body_text -> body_text special_token .)
+    SPACE           reduce using rule 75 (body_text -> body_text special_token .)
+    METADATA        reduce using rule 75 (body_text -> body_text special_token .)
+    NEWLINE         reduce using rule 75 (body_text -> body_text special_token .)
+    SCHEDULING      reduce using rule 75 (body_text -> body_text special_token .)
+    COOKIE          reduce using rule 75 (body_text -> body_text special_token .)
+    PRIORITY        reduce using rule 75 (body_text -> body_text special_token .)
+    TODO            reduce using rule 75 (body_text -> body_text special_token .)
+    COMMENT         reduce using rule 75 (body_text -> body_text special_token .)
+    TAGS            reduce using rule 75 (body_text -> body_text special_token .)
+    ATIMESTAMP      reduce using rule 75 (body_text -> body_text special_token .)
+    ITIMESTAMP      reduce using rule 75 (body_text -> body_text special_token .)
+    SEPARATOR       reduce using rule 75 (body_text -> body_text special_token .)
+    STARS           reduce using rule 75 (body_text -> body_text special_token .)
+    $end            reduce using rule 75 (body_text -> body_text special_token .)
 
 
 state 78
 
-    (72) body_text -> body_text NEWLINE .
+    (76) body_text -> body_text METADATA .
 
-    TEXT            reduce using rule 72 (body_text -> body_text NEWLINE .)
-    SPACE           reduce using rule 72 (body_text -> body_text NEWLINE .)
-    METADATA        reduce using rule 72 (body_text -> body_text NEWLINE .)
-    NEWLINE         reduce using rule 72 (body_text -> body_text NEWLINE .)
-    SCHEDULING      reduce using rule 72 (body_text -> body_text NEWLINE .)
-    COOKIE          reduce using rule 72 (body_text -> body_text NEWLINE .)
-    PRIORITY        reduce using rule 72 (body_text -> body_text NEWLINE .)
-    TODO            reduce using rule 72 (body_text -> body_text NEWLINE .)
-    COMMENT         reduce using rule 72 (body_text -> body_text NEWLINE .)
-    TAGS            reduce using rule 72 (body_text -> body_text NEWLINE .)
-    ATIMESTAMP      reduce using rule 72 (body_text -> body_text NEWLINE .)
-    ITIMESTAMP      reduce using rule 72 (body_text -> body_text NEWLINE .)
-    SEPARATOR       reduce using rule 72 (body_text -> body_text NEWLINE .)
-    STARS           reduce using rule 72 (body_text -> body_text NEWLINE .)
-    $end            reduce using rule 72 (body_text -> body_text NEWLINE .)
+    TEXT            reduce using rule 76 (body_text -> body_text METADATA .)
+    SPACE           reduce using rule 76 (body_text -> body_text METADATA .)
+    METADATA        reduce using rule 76 (body_text -> body_text METADATA .)
+    NEWLINE         reduce using rule 76 (body_text -> body_text METADATA .)
+    SCHEDULING      reduce using rule 76 (body_text -> body_text METADATA .)
+    COOKIE          reduce using rule 76 (body_text -> body_text METADATA .)
+    PRIORITY        reduce using rule 76 (body_text -> body_text METADATA .)
+    TODO            reduce using rule 76 (body_text -> body_text METADATA .)
+    COMMENT         reduce using rule 76 (body_text -> body_text METADATA .)
+    TAGS            reduce using rule 76 (body_text -> body_text METADATA .)
+    ATIMESTAMP      reduce using rule 76 (body_text -> body_text METADATA .)
+    ITIMESTAMP      reduce using rule 76 (body_text -> body_text METADATA .)
+    SEPARATOR       reduce using rule 76 (body_text -> body_text METADATA .)
+    STARS           reduce using rule 76 (body_text -> body_text METADATA .)
+    $end            reduce using rule 76 (body_text -> body_text METADATA .)
 
 
 state 79
 
-    (44) drawer_data -> drawer_data DRAWER NEWLINE .
+    (77) body_text -> body_text NEWLINE .
 
-    DRAWER          reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    TEXT            reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    SPACE           reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    METADATA        reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    SCHEDULING      reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    COOKIE          reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    PRIORITY        reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    TODO            reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    COMMENT         reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    TAGS            reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    ATIMESTAMP      reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    ITIMESTAMP      reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    SEPARATOR       reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    STARS           reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
-    $end            reduce using rule 44 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    TEXT            reduce using rule 77 (body_text -> body_text NEWLINE .)
+    SPACE           reduce using rule 77 (body_text -> body_text NEWLINE .)
+    METADATA        reduce using rule 77 (body_text -> body_text NEWLINE .)
+    NEWLINE         reduce using rule 77 (body_text -> body_text NEWLINE .)
+    SCHEDULING      reduce using rule 77 (body_text -> body_text NEWLINE .)
+    COOKIE          reduce using rule 77 (body_text -> body_text NEWLINE .)
+    PRIORITY        reduce using rule 77 (body_text -> body_text NEWLINE .)
+    TODO            reduce using rule 77 (body_text -> body_text NEWLINE .)
+    COMMENT         reduce using rule 77 (body_text -> body_text NEWLINE .)
+    TAGS            reduce using rule 77 (body_text -> body_text NEWLINE .)
+    ATIMESTAMP      reduce using rule 77 (body_text -> body_text NEWLINE .)
+    ITIMESTAMP      reduce using rule 77 (body_text -> body_text NEWLINE .)
+    SEPARATOR       reduce using rule 77 (body_text -> body_text NEWLINE .)
+    STARS           reduce using rule 77 (body_text -> body_text NEWLINE .)
+    $end            reduce using rule 77 (body_text -> body_text NEWLINE .)
 
 
 state 80
 
-    (45) drawer_data -> drawer_data DRAWER SEPARATOR .
+    (49) drawer_data -> drawer_data DRAWER NEWLINE .
 
-    DRAWER          reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    TEXT            reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    SPACE           reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    METADATA        reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    SCHEDULING      reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    COOKIE          reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    PRIORITY        reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    TODO            reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    COMMENT         reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    TAGS            reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    ATIMESTAMP      reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    ITIMESTAMP      reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    SEPARATOR       reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    STARS           reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
-    $end            reduce using rule 45 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    DRAWER          reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    TEXT            reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    SPACE           reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    METADATA        reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    SCHEDULING      reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    COOKIE          reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    PRIORITY        reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    TODO            reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    COMMENT         reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    TAGS            reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    ATIMESTAMP      reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    ITIMESTAMP      reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    SEPARATOR       reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    STARS           reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
+    $end            reduce using rule 49 (drawer_data -> drawer_data DRAWER NEWLINE .)
 
 
 state 81
 
-    (35) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp . NEWLINE
-    (36) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp . SEPARATOR
-    (37) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp . SPACE
-
-    NEWLINE         shift and go to state 89
-    SEPARATOR       shift and go to state 90
-    SPACE           shift and go to state 88
+    (50) drawer_data -> drawer_data DRAWER SEPARATOR .
+
+    DRAWER          reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    TEXT            reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    SPACE           reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    METADATA        reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    SCHEDULING      reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    COOKIE          reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    PRIORITY        reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    TODO            reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    COMMENT         reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    TAGS            reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    ATIMESTAMP      reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    ITIMESTAMP      reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    SEPARATOR       reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    STARS           reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
+    $end            reduce using rule 50 (drawer_data -> drawer_data DRAWER SEPARATOR .)
 
 
 state 82
 
-    (34) scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .
+    (40) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp . NEWLINE
+    (41) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp . SEPARATOR
+    (42) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp . SPACE
 
-    SCHEDULING      reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    DRAWER          reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    TEXT            reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    SPACE           reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    METADATA        reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    COOKIE          reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    PRIORITY        reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    TODO            reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    COMMENT         reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    TAGS            reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    ATIMESTAMP      reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    ITIMESTAMP      reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    SEPARATOR       reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    STARS           reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
-    $end            reduce using rule 34 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    NEWLINE         shift and go to state 92
+    SEPARATOR       shift and go to state 93
+    SPACE           shift and go to state 91
 
 
 state 83
 
-    (32) scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .
+    (39) scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .
 
-    SCHEDULING      reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    DRAWER          reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    TEXT            reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    SPACE           reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    METADATA        reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    COOKIE          reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    PRIORITY        reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    TODO            reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    COMMENT         reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    TAGS            reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    ATIMESTAMP      reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    ITIMESTAMP      reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    SEPARATOR       reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    STARS           reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
-    $end            reduce using rule 32 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    SCHEDULING      reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    DRAWER          reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    TEXT            reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    SPACE           reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    METADATA        reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    COOKIE          reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    PRIORITY        reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    TODO            reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    COMMENT         reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    TAGS            reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    ATIMESTAMP      reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    ITIMESTAMP      reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    SEPARATOR       reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    STARS           reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
+    $end            reduce using rule 39 (scheduling_data -> SCHEDULING SPACE any_timestamp SPACE .)
 
 
 state 84
 
-    (33) scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .
+    (37) scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .
 
-    SCHEDULING      reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    DRAWER          reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    TEXT            reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    SPACE           reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    METADATA        reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    COOKIE          reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    PRIORITY        reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    TODO            reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    COMMENT         reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    TAGS            reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    ATIMESTAMP      reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    ITIMESTAMP      reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    SEPARATOR       reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    STARS           reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
-    $end            reduce using rule 33 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    SCHEDULING      reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    DRAWER          reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    TEXT            reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    SPACE           reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    METADATA        reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    COOKIE          reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    PRIORITY        reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    TODO            reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    COMMENT         reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    TAGS            reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    ATIMESTAMP      reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    ITIMESTAMP      reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    SEPARATOR       reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    STARS           reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
+    $end            reduce using rule 37 (scheduling_data -> SCHEDULING SPACE any_timestamp NEWLINE .)
 
 
 state 85
 
-    (16) headline -> STARS SPACE comment todo priority title . cookie tags
-    (24) title -> title . SPACE TEXT
-    (25) title -> title . SPACE
-    (26) cookie -> . COOKIE SPACE
-    (27) cookie -> . COOKIE
-    (28) cookie -> . empty
-    (73) empty -> .
+    (38) scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .
 
-    SPACE           shift and go to state 91
-    COOKIE          shift and go to state 93
-    TAGS            reduce using rule 73 (empty -> .)
-    NEWLINE         reduce using rule 73 (empty -> .)
-    SEPARATOR       reduce using rule 73 (empty -> .)
+    SCHEDULING      reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    DRAWER          reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TEXT            reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    SPACE           reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    METADATA        reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    COOKIE          reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    PRIORITY        reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TODO            reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    COMMENT         reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TAGS            reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    ATIMESTAMP      reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    ITIMESTAMP      reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    SEPARATOR       reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    STARS           reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
+    $end            reduce using rule 38 (scheduling_data -> SCHEDULING SPACE any_timestamp SEPARATOR .)
 
-    cookie                         shift and go to state 92
-    empty                          shift and go to state 94
 
 state 86
 
-    (23) title -> TEXT .
-
-    SPACE           reduce using rule 23 (title -> TEXT .)
-    COOKIE          reduce using rule 23 (title -> TEXT .)
-    TAGS            reduce using rule 23 (title -> TEXT .)
-    NEWLINE         reduce using rule 23 (title -> TEXT .)
-    SEPARATOR       reduce using rule 23 (title -> TEXT .)
+    (18) headline -> STARS SPACE comment todo priority title . cookie tags
+    (27) title -> title . SPACE TEXT
+    (28) title -> title . SPACE TODO
+    (29) title -> title . SPACE
+    (31) cookie -> . COOKIE SPACE
+    (32) cookie -> . COOKIE
+    (33) cookie -> . empty
+    (78) empty -> .
+
+    SPACE           shift and go to state 94
+    COOKIE          shift and go to state 96
+    TAGS            reduce using rule 78 (empty -> .)
+    NEWLINE         reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
 
+    cookie                         shift and go to state 95
+    empty                          shift and go to state 97
 
 state 87
 
-    (21) priority -> PRIORITY SPACE .
+    (25) title -> TEXT .
 
-    TEXT            reduce using rule 21 (priority -> PRIORITY SPACE .)
+    SPACE           reduce using rule 25 (title -> TEXT .)
+    COOKIE          reduce using rule 25 (title -> TEXT .)
+    TAGS            reduce using rule 25 (title -> TEXT .)
+    NEWLINE         reduce using rule 25 (title -> TEXT .)
+    SEPARATOR       reduce using rule 25 (title -> TEXT .)
 
 
 state 88
 
-    (37) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .
+    (26) title -> TODO .
 
-    SCHEDULING      reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    DRAWER          reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    TEXT            reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    SPACE           reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    METADATA        reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    COOKIE          reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    PRIORITY        reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    TODO            reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    COMMENT         reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    TAGS            reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    ATIMESTAMP      reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    ITIMESTAMP      reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    SEPARATOR       reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    STARS           reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
-    $end            reduce using rule 37 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    SPACE           reduce using rule 26 (title -> TODO .)
+    COOKIE          reduce using rule 26 (title -> TODO .)
+    TAGS            reduce using rule 26 (title -> TODO .)
+    NEWLINE         reduce using rule 26 (title -> TODO .)
+    SEPARATOR       reduce using rule 26 (title -> TODO .)
 
 
 state 89
 
-    (35) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .
+    (30) title -> empty .
 
-    SCHEDULING      reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    DRAWER          reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    TEXT            reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    SPACE           reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    METADATA        reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    COOKIE          reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    PRIORITY        reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    TODO            reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    COMMENT         reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    TAGS            reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    ATIMESTAMP      reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    ITIMESTAMP      reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    SEPARATOR       reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    STARS           reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
-    $end            reduce using rule 35 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    SPACE           reduce using rule 30 (title -> empty .)
+    COOKIE          reduce using rule 30 (title -> empty .)
+    TAGS            reduce using rule 30 (title -> empty .)
+    NEWLINE         reduce using rule 30 (title -> empty .)
+    SEPARATOR       reduce using rule 30 (title -> empty .)
 
 
 state 90
 
-    (36) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .
+    (23) priority -> PRIORITY SPACE .
 
-    SCHEDULING      reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    DRAWER          reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    TEXT            reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    SPACE           reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    METADATA        reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    COOKIE          reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    PRIORITY        reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    TODO            reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    COMMENT         reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    TAGS            reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    ATIMESTAMP      reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    ITIMESTAMP      reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    SEPARATOR       reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    STARS           reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
-    $end            reduce using rule 36 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TEXT            reduce using rule 23 (priority -> PRIORITY SPACE .)
+    TODO            reduce using rule 23 (priority -> PRIORITY SPACE .)
+    SPACE           reduce using rule 23 (priority -> PRIORITY SPACE .)
+    COOKIE          reduce using rule 23 (priority -> PRIORITY SPACE .)
+    TAGS            reduce using rule 23 (priority -> PRIORITY SPACE .)
+    NEWLINE         reduce using rule 23 (priority -> PRIORITY SPACE .)
+    SEPARATOR       reduce using rule 23 (priority -> PRIORITY SPACE .)
 
 
 state 91
 
-    (24) title -> title SPACE . TEXT
-    (25) title -> title SPACE .
+    (42) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .
 
-    TEXT            shift and go to state 95
-    SPACE           reduce using rule 25 (title -> title SPACE .)
-    COOKIE          reduce using rule 25 (title -> title SPACE .)
-    TAGS            reduce using rule 25 (title -> title SPACE .)
-    NEWLINE         reduce using rule 25 (title -> title SPACE .)
-    SEPARATOR       reduce using rule 25 (title -> title SPACE .)
+    SCHEDULING      reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    DRAWER          reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    TEXT            reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    SPACE           reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    METADATA        reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    COOKIE          reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    PRIORITY        reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    TODO            reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    COMMENT         reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    TAGS            reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    ATIMESTAMP      reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    ITIMESTAMP      reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    SEPARATOR       reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    STARS           reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
+    $end            reduce using rule 42 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SPACE .)
 
 
 state 92
 
-    (16) headline -> STARS SPACE comment todo priority title cookie . tags
-    (29) tags -> . TAGS
-    (30) tags -> . empty
-    (73) empty -> .
-
-    TAGS            shift and go to state 97
-    NEWLINE         reduce using rule 73 (empty -> .)
-    SEPARATOR       reduce using rule 73 (empty -> .)
+    (40) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .
+
+    SCHEDULING      reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    DRAWER          reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    TEXT            reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    SPACE           reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    METADATA        reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    COOKIE          reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    PRIORITY        reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    TODO            reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    COMMENT         reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    TAGS            reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    ATIMESTAMP      reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    ITIMESTAMP      reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    SEPARATOR       reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    STARS           reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
+    $end            reduce using rule 40 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp NEWLINE .)
 
-    tags                           shift and go to state 96
-    empty                          shift and go to state 98
 
 state 93
 
-    (26) cookie -> COOKIE . SPACE
-    (27) cookie -> COOKIE .
+    (41) scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .
 
-    SPACE           shift and go to state 99
-    TAGS            reduce using rule 27 (cookie -> COOKIE .)
-    NEWLINE         reduce using rule 27 (cookie -> COOKIE .)
-    SEPARATOR       reduce using rule 27 (cookie -> COOKIE .)
+    SCHEDULING      reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    DRAWER          reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TEXT            reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    SPACE           reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    METADATA        reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    COOKIE          reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    PRIORITY        reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TODO            reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    COMMENT         reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    TAGS            reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    ATIMESTAMP      reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    ITIMESTAMP      reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    SEPARATOR       reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    STARS           reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
+    $end            reduce using rule 41 (scheduling_data -> scheduling_data SCHEDULING SPACE any_timestamp SEPARATOR .)
 
 
 state 94
 
-    (28) cookie -> empty .
-
-    TAGS            reduce using rule 28 (cookie -> empty .)
-    NEWLINE         reduce using rule 28 (cookie -> empty .)
-    SEPARATOR       reduce using rule 28 (cookie -> empty .)
+    (27) title -> title SPACE . TEXT
+    (28) title -> title SPACE . TODO
+    (29) title -> title SPACE .
+
+    TEXT            shift and go to state 98
+    TODO            shift and go to state 99
+    SPACE           reduce using rule 29 (title -> title SPACE .)
+    COOKIE          reduce using rule 29 (title -> title SPACE .)
+    TAGS            reduce using rule 29 (title -> title SPACE .)
+    NEWLINE         reduce using rule 29 (title -> title SPACE .)
+    SEPARATOR       reduce using rule 29 (title -> title SPACE .)
 
 
 state 95
 
-    (24) title -> title SPACE TEXT .
-
-    SPACE           reduce using rule 24 (title -> title SPACE TEXT .)
-    COOKIE          reduce using rule 24 (title -> title SPACE TEXT .)
-    TAGS            reduce using rule 24 (title -> title SPACE TEXT .)
-    NEWLINE         reduce using rule 24 (title -> title SPACE TEXT .)
-    SEPARATOR       reduce using rule 24 (title -> title SPACE TEXT .)
+    (18) headline -> STARS SPACE comment todo priority title cookie . tags
+    (34) tags -> . TAGS
+    (35) tags -> . empty
+    (78) empty -> .
+
+    TAGS            shift and go to state 101
+    NEWLINE         reduce using rule 78 (empty -> .)
+    SEPARATOR       reduce using rule 78 (empty -> .)
 
+    tags                           shift and go to state 100
+    empty                          shift and go to state 102
 
 state 96
 
-    (16) headline -> STARS SPACE comment todo priority title cookie tags .
+    (31) cookie -> COOKIE . SPACE
+    (32) cookie -> COOKIE .
 
-    NEWLINE         reduce using rule 16 (headline -> STARS SPACE comment todo priority title cookie tags .)
-    SEPARATOR       reduce using rule 16 (headline -> STARS SPACE comment todo priority title cookie tags .)
+    SPACE           shift and go to state 103
+    TAGS            reduce using rule 32 (cookie -> COOKIE .)
+    NEWLINE         reduce using rule 32 (cookie -> COOKIE .)
+    SEPARATOR       reduce using rule 32 (cookie -> COOKIE .)
 
 
 state 97
 
-    (29) tags -> TAGS .
+    (33) cookie -> empty .
 
-    NEWLINE         reduce using rule 29 (tags -> TAGS .)
-    SEPARATOR       reduce using rule 29 (tags -> TAGS .)
+    TAGS            reduce using rule 33 (cookie -> empty .)
+    NEWLINE         reduce using rule 33 (cookie -> empty .)
+    SEPARATOR       reduce using rule 33 (cookie -> empty .)
 
 
 state 98
 
-    (30) tags -> empty .
+    (27) title -> title SPACE TEXT .
 
-    NEWLINE         reduce using rule 30 (tags -> empty .)
-    SEPARATOR       reduce using rule 30 (tags -> empty .)
+    SPACE           reduce using rule 27 (title -> title SPACE TEXT .)
+    COOKIE          reduce using rule 27 (title -> title SPACE TEXT .)
+    TAGS            reduce using rule 27 (title -> title SPACE TEXT .)
+    NEWLINE         reduce using rule 27 (title -> title SPACE TEXT .)
+    SEPARATOR       reduce using rule 27 (title -> title SPACE TEXT .)
 
 
 state 99
 
-    (26) cookie -> COOKIE SPACE .
+    (28) title -> title SPACE TODO .
+
+    SPACE           reduce using rule 28 (title -> title SPACE TODO .)
+    COOKIE          reduce using rule 28 (title -> title SPACE TODO .)
+    TAGS            reduce using rule 28 (title -> title SPACE TODO .)
+    NEWLINE         reduce using rule 28 (title -> title SPACE TODO .)
+    SEPARATOR       reduce using rule 28 (title -> title SPACE TODO .)
+
+
+state 100
+
+    (18) headline -> STARS SPACE comment todo priority title cookie tags .
+
+    NEWLINE         reduce using rule 18 (headline -> STARS SPACE comment todo priority title cookie tags .)
+    SEPARATOR       reduce using rule 18 (headline -> STARS SPACE comment todo priority title cookie tags .)
+
+
+state 101
+
+    (34) tags -> TAGS .
+
+    NEWLINE         reduce using rule 34 (tags -> TAGS .)
+    SEPARATOR       reduce using rule 34 (tags -> TAGS .)
+
+
+state 102
+
+    (35) tags -> empty .
+
+    NEWLINE         reduce using rule 35 (tags -> empty .)
+    SEPARATOR       reduce using rule 35 (tags -> empty .)
+
+
+state 103
+
+    (31) cookie -> COOKIE SPACE .
 
-    TAGS            reduce using rule 26 (cookie -> COOKIE SPACE .)
-    NEWLINE         reduce using rule 26 (cookie -> COOKIE SPACE .)
-    SEPARATOR       reduce using rule 26 (cookie -> COOKIE SPACE .)
+    TAGS            reduce using rule 31 (cookie -> COOKIE SPACE .)
+    NEWLINE         reduce using rule 31 (cookie -> COOKIE SPACE .)
+    SEPARATOR       reduce using rule 31 (cookie -> COOKIE SPACE .)
 
 WARNING: 
 WARNING: Conflicts:
 WARNING: 
-WARNING: shift/reduce conflict for SCHEDULING in state 33 resolved as shift
-WARNING: shift/reduce conflict for SCHEDULING in state 41 resolved as shift
+WARNING: shift/reduce conflict for SCHEDULING in state 34 resolved as shift
+WARNING: shift/reduce conflict for SCHEDULING in state 42 resolved as shift
+WARNING: shift/reduce conflict for TODO in state 45 resolved as shift
```

### Comparing `orgmunge-0.2.0/src/orgmunge/parser.py` & `orgmunge-0.2.1/src/orgmunge/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,33 @@
     def __init__(self, lexer):
         self.tokens = lexer.tokens
         self.lexer = lexer
         self.parser = yacc.yacc(module=self)
     def p_org_file(self, p):
         '''org_file : metadata org_tree
                     | non_metadata_body_text SEPARATOR org_tree
+                    | non_metadata_body_text SEPARATOR
                     | metadata non_metadata_body_text SEPARATOR org_tree
                     | metadata non_metadata_body_text SEPARATOR 
                     | metadata
                     | org_tree
+                    | SEPARATOR
                     | empty'''
         if len(p) == 5:
             p[0] = (p[1], p[2], p[4])
         elif len(p) == 4:
-            if p[3] != '\n': 
+            if type(p[3]) is not str: 
                 p[0] = ('', p[1], p[3])
             else:
                 p[0] = (p[1], p[2], None)
         elif len(p) == 3:
-            p[0] = (p[1], '', p[2])
+            if p[1].startswith('#+'):
+                p[0] = (p[1], '', p[2])
+            else:
+                p[0] = ('', p[1], None)
         else:
             if type(p[1]) is str:
                 p[0] = (p[1], '', None)
             else:
                 p[0] = ('', '', p[1])
 
     def p_metadata(self, p):
@@ -79,22 +84,26 @@
     def p_priority(self, p):
         '''priority : PRIORITY SPACE
                     | empty'''
         p[0] = p[1] if len(p) > 2 else None
 
     def p_title(self, p):
         """title : TEXT 
-                | title SPACE TEXT
-                | title SPACE"""
-        p[0] = reduce(add, p[1:]).strip()
+                 | TODO
+                 | title SPACE TEXT
+                 | title SPACE TODO
+                 | title SPACE
+                 | empty"""
+        none_to_empty = [x if x else "" for x in p[1:]]
+        p[0] = reduce(add, none_to_empty, "").strip()
 
     def p_cookie(self, p):
         '''cookie : COOKIE SPACE
-                | COOKIE
-                | empty'''
+                  | COOKIE
+                  | empty'''
         p[0] = p[1] if len(p) > 1 else None
 
     def p_tags(self, p):
         '''tags : TAGS
                 | empty''' 
         if p[1] is not None:
             p[0] = [x for x in p[1].split(':') if x != '']
@@ -192,7 +201,8 @@
     def p_empty(self, p):
         'empty :' 
         pass
 
     def p_error(self, p):
         if p is not None:
             print(f'Syntax error: {p}')
+            raise ValueError("Parser error!")
```

### Comparing `orgmunge-0.2.0/PKG-INFO` & `orgmunge-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: orgmunge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Programmatically modify Orgmode documents
 License: MIT
 Author: durableOne 
 Author-email: era31asj@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ply (>=3.11,<4.0)
 Description-Content-Type: text/plain
 
 #+title:Orgmunge
 * Motivation and scope
 Orgmunge was born out of the desire to modify Org documents
 programmatically from within Python. The wonderful [[https://github.com/karlicoss/orgparse][orgparse]] can read
@@ -306,14 +307,24 @@
 regex unless =exact= is set to =True=, in which case, the function will
 return headings whose title matches the search string
 exactly. =re_flags= are flags passed to =re.search=. This argument is
 ignored if =exact= is =True=.
 Uses =filter_headings= under the hood so will return a generator of
 matching headings.
 
+*** Search for Headings by Path
+Use =Org.get_heading_by_path= to search for a heading with the given path:
+#+begin_src python
+  Org.get_heading_by_path(path, exact=False, re_flags=0)
+#+end_src
+=path= is a list of heading titles. Each member is interpreted the same
+way the =search_string= argument of =get_headings_by_title= is
+interpreted. This function returns the first heading of the tree that
+matches the given path or =None= if no such heading is found.
+
 * License
 #+INCLUDE: ./LICENSE
 
 
 
 * Contributors
 :PROPERTIES:
```

