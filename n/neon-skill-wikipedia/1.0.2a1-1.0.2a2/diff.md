# Comparing `tmp/neon-skill-wikipedia-1.0.2a1.tar.gz` & `tmp/neon-skill-wikipedia-1.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-wikipedia-1.0.2a1.tar", last modified: Wed Feb  7 00:09:04 2024, max compression
+gzip compressed data, was "neon-skill-wikipedia-1.0.2a2.tar", last modified: Tue Apr  2 23:19:38 2024, max compression
```

## Comparing `neon-skill-wikipedia-1.0.2a1.tar` & `neon-skill-wikipedia-1.0.2a2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:04.358762 neon-skill-wikipedia-1.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-07 00:09:04.358762 neon-skill-wikipedia-1.0.2a1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5502 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:04.354762 neon-skill-wikipedia-1.0.2a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:04.354762 neon-skill-wikipedia-1.0.2a1/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/ca-es/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:04.354762 neon-skill-wikipedia-1.0.2a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/locale/en-us/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:04.358762 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-07 00:09:04.000000 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-07 00:09:04.000000 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 00:09:04.000000 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-07 00:09:04.000000 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-07 00:09:04.000000 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 00:09:04.000000 neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/pic.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 00:09:04.358762 neon-skill-wikipedia-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:04.358762 neon-skill-wikipedia-1.0.2a1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)   907480 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/ui/jumping.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-07 00:08:58.000000 neon-skill-wikipedia-1.0.2a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:19:38.443830 neon-skill-wikipedia-1.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-02 23:19:38.443830 neon-skill-wikipedia-1.0.2a2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5502 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:19:38.435830 neon-skill-wikipedia-1.0.2a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:19:38.439830 neon-skill-wikipedia-1.0.2a2/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/ca-es/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:19:38.439830 neon-skill-wikipedia-1.0.2a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/locale/en-us/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:19:38.439830 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-02 23:19:38.000000 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-02 23:19:38.000000 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:19:38.000000 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 23:19:38.000000 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 23:19:38.000000 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 23:19:38.000000 neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/pic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:19:38.443830 neon-skill-wikipedia-1.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:19:38.439830 neon-skill-wikipedia-1.0.2a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   907480 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/ui/jumping.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 23:19:33.000000 neon-skill-wikipedia-1.0.2a2/version.py
```

### Comparing `neon-skill-wikipedia-1.0.2a1/LICENSE` & `neon-skill-wikipedia-1.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/LICENSE.md` & `neon-skill-wikipedia-1.0.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/PKG-INFO` & `neon-skill-wikipedia-1.0.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-wikipedia
-Version: 1.0.2a1
+Version: 1.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-wikipedia
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-wikipedia-1.0.2a1/README.md` & `neon-skill-wikipedia-1.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/__init__.py` & `neon-skill-wikipedia-1.0.2a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/locale/ca-es/wikiroulette.intent` & `neon-skill-wikipedia-1.0.2a2/locale/ca-es/wikiroulette.intent`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/PKG-INFO` & `neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-wikipedia
-Version: 1.0.2a1
+Version: 1.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-wikipedia
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-wikipedia-1.0.2a1/neon_skill_wikipedia.egg-info/SOURCES.txt` & `neon-skill-wikipedia-1.0.2a2/neon_skill_wikipedia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/setup.py` & `neon-skill-wikipedia-1.0.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/skill.json` & `neon-skill-wikipedia-1.0.2a2/skill.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'requirements'": "{'python': {insert: [(2, 'ovos_utils~=0.0,>=0.0.28')], delete: [2]}}"}*

```diff
@@ -34,15 +34,15 @@
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-utils~=1.0",
             "ovos-workshop~=0.0.15",
-            "ovos_utils~=0.0.28",
+            "ovos_utils~=0.0,>=0.0.28",
             "wikipedia-api~=0.5.8",
             "wikipedia_for_humans~=0.2.3"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Wikipedia ![](./logo.png)",
```

### Comparing `neon-skill-wikipedia-1.0.2a1/ui/jumping.gif` & `neon-skill-wikipedia-1.0.2a2/ui/jumping.gif`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-1.0.2a1/version.py` & `neon-skill-wikipedia-1.0.2a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.2a1"
+__version__ = "1.0.2a2"
```

