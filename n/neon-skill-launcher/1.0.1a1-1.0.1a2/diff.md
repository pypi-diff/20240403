# Comparing `tmp/neon-skill-launcher-1.0.1a1.tar.gz` & `tmp/neon-skill-launcher-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-launcher-1.0.1a1.tar", last modified: Tue Feb  6 02:27:03 2024, max compression
+gzip compressed data, was "neon-skill-launcher-1.0.1a2.tar", last modified: Wed Apr  3 19:00:04 2024, max compression
```

## Comparing `neon-skill-launcher-1.0.1a1.tar` & `neon-skill-launcher-1.0.1a2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.479361 neon-skill-launcher-1.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.479361 neon-skill-launcher-1.0.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/launch_program.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/launch_website.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/mobile_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/on.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/dialog/website_not_found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/regex/website.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/vocab/browse.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/vocab/launch.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/locale/en-us/vocab/launch_program.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-06 02:27:03.000000 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-06 02:27:03.000000 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 02:27:03.000000 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-06 02:27:03.000000 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-06 02:27:03.000000 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 02:27:03.000000 neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 02:27:03.483361 neon-skill-launcher-1.0.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 02:26:55.000000 neon-skill-launcher-1.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.805920 neon-skill-launcher-1.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.805920 neon-skill-launcher-1.0.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/launch_program.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/launch_website.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/mobile_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/on.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/dialog/website_not_found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/regex/website.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/browse.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/launch.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/locale/en-us/vocab/launch_program.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 19:00:04.000000 neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:00:04.809919 neon-skill-launcher-1.0.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 18:59:50.000000 neon-skill-launcher-1.0.1a2/version.py
```

### Comparing `neon-skill-launcher-1.0.1a1/LICENSE.md` & `neon-skill-launcher-1.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/PKG-INFO` & `neon-skill-launcher-1.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-launcher
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-launcher
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-launcher-1.0.1a1/README.md` & `neon-skill-launcher-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/__init__.py` & `neon-skill-launcher-1.0.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/PKG-INFO` & `neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-launcher
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-launcher
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-launcher-1.0.1a1/neon_skill_launcher.egg-info/SOURCES.txt` & `neon-skill-launcher-1.0.1a2/neon_skill_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/setup.py` & `neon-skill-launcher-1.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/skill.json` & `neon-skill-launcher-1.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/test/test_skill.py` & `neon-skill-launcher-1.0.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-launcher-1.0.1a1/version.py` & `neon-skill-launcher-1.0.1a2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a1"
+__version__ = "1.0.1a2"
```

