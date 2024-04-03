# Comparing `tmp/neon-skill-translation-1.0.1a2.tar.gz` & `tmp/neon-skill-translation-1.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-translation-1.0.1a2.tar", last modified: Tue Feb  6 01:46:06 2024, max compression
+gzip compressed data, was "neon-skill-translation-1.0.1a3.tar", last modified: Wed Apr  3 19:57:43 2024, max compression
```

## Comparing `neon-skill-translation-1.0.1a2.tar` & `neon-skill-translation-1.0.1a3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.963680 neon-skill-translation-1.0.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/locale/en-us/dialog/language_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/locale/en-us/dialog/phrase_in_language.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/locale/en-us/languages.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/locale/en-us/vocab/female.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/locale/en-us/vocab/male.voc
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/locale/en-us/vocab/translate_phrase.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-06 01:46:06.000000 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-06 01:46:06.000000 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:46:06.000000 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-06 01:46:06.000000 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-06 01:46:06.000000 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-06 01:46:06.000000 neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:46:06.967680 neon-skill-translation-1.0.1a2/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/ui/Translation.qml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:46:02.000000 neon-skill-translation-1.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/locale/en-us/dialog/language_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/locale/en-us/dialog/phrase_in_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/locale/en-us/languages.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/locale/en-us/vocab/female.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/locale/en-us/vocab/male.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/locale/en-us/vocab/translate_phrase.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 19:57:43.000000 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 19:57:43.000000 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:57:43.000000 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:57:43.000000 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 19:57:43.000000 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 19:57:43.000000 neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:57:43.653806 neon-skill-translation-1.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:57:43.649806 neon-skill-translation-1.0.1a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/ui/Translation.qml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 19:57:40.000000 neon-skill-translation-1.0.1a3/version.py
```

### Comparing `neon-skill-translation-1.0.1a2/LICENSE.md` & `neon-skill-translation-1.0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/PKG-INFO` & `neon-skill-translation-1.0.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-translation
-Version: 1.0.1a2
+Version: 1.0.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-translation
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-translation-1.0.1a2/README.md` & `neon-skill-translation-1.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/__init__.py` & `neon-skill-translation-1.0.1a3/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/PKG-INFO` & `neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-translation
-Version: 1.0.1a2
+Version: 1.0.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-translation
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-translation-1.0.1a2/neon_skill_translation.egg-info/SOURCES.txt` & `neon-skill-translation-1.0.1a3/neon_skill_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/setup.py` & `neon-skill-translation-1.0.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/skill.json` & `neon-skill-translation-1.0.1a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/test/test_skill.py` & `neon-skill-translation-1.0.1a3/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/ui/Translation.qml` & `neon-skill-translation-1.0.1a3/ui/Translation.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-1.0.1a2/version.py` & `neon-skill-translation-1.0.1a3/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a2"
+__version__ = "1.0.1a3"
```

