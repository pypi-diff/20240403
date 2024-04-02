# Comparing `tmp/neon-skill-free_music_archive-1.0.1a1.tar.gz` & `tmp/neon-skill-free_music_archive-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-free_music_archive-1.0.1a1.tar", last modified: Mon Feb  5 22:41:24 2024, max compression
+gzip compressed data, was "neon-skill-free_music_archive-1.0.1a2.tar", last modified: Tue Apr  2 23:31:41 2024, max compression
```

## Comparing `neon-skill-free_music_archive-1.0.1a1.tar` & `neon-skill-free_music_archive-1.0.1a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:41:24.012667 neon-skill-free_music_archive-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-05 22:41:24.012667 neon-skill-free_music_archive-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:41:24.008667 neon-skill-free_music_archive-1.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:41:24.012667 neon-skill-free_music_archive-1.0.1a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/locale/en-us/articles.voc
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/locale/en-us/genre.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:41:24.012667 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-05 22:41:23.000000 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-05 22:41:24.000000 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 22:41:23.000000 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-05 22:41:23.000000 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-05 22:41:23.000000 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 22:41:23.000000 neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 22:41:24.012667 neon-skill-free_music_archive-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:41:24.012667 neon-skill-free_music_archive-1.0.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 22:41:21.000000 neon-skill-free_music_archive-1.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/locale/en-us/articles.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/locale/en-us/genre.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 23:31:41.000000 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 23:31:41.000000 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:31:41.000000 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 23:31:41.000000 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 23:31:41.000000 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 23:31:41.000000 neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:31:41.546043 neon-skill-free_music_archive-1.0.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 23:31:38.000000 neon-skill-free_music_archive-1.0.1a2/version.py
```

### Comparing `neon-skill-free_music_archive-1.0.1a1/LICENSE.md` & `neon-skill-free_music_archive-1.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-free_music_archive-1.0.1a1/PKG-INFO` & `neon-skill-free_music_archive-1.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-free_music_archive
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-free_music_archive
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-free_music_archive-1.0.1a1/README.md` & `neon-skill-free_music_archive-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-free_music_archive-1.0.1a1/__init__.py` & `neon-skill-free_music_archive-1.0.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-free_music_archive-1.0.1a1/neon_skill_free_music_archive.egg-info/PKG-INFO` & `neon-skill-free_music_archive-1.0.1a2/neon_skill_free_music_archive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-free-music-archive
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-free_music_archive
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-free_music_archive-1.0.1a1/setup.py` & `neon-skill-free_music_archive-1.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-free_music_archive-1.0.1a1/skill.json` & `neon-skill-free_music_archive-1.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-free_music_archive-1.0.1a1/test/test_skill.py` & `neon-skill-free_music_archive-1.0.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-free_music_archive-1.0.1a1/version.py` & `neon-skill-free_music_archive-1.0.1a2/version.py`

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

