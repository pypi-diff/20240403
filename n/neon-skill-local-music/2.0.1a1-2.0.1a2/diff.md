# Comparing `tmp/neon-skill-local_music-2.0.1a1.tar.gz` & `tmp/neon-skill-local_music-2.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-local_music-2.0.1a1.tar", last modified: Tue Feb  6 00:01:10 2024, max compression
+gzip compressed data, was "neon-skill-local_music-2.0.1a2.tar", last modified: Wed Apr  3 00:02:13 2024, max compression
```

## Comparing `neon-skill-local_music-2.0.1a1.tar` & `neon-skill-local_music-2.0.1a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 00:01:06.000000 neon-skill-local_music-2.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-06 00:01:06.000000 neon-skill-local_music-2.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-02-06 00:01:06.000000 neon-skill-local_music-2.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.755479 neon-skill-local_music-2.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.755479 neon-skill-local_music-2.0.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 00:01:06.000000 neon-skill-local_music-2.0.1a1/locale/en-us/vocab/local.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-06 00:01:10.000000 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-06 00:01:10.000000 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 00:01:10.000000 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 00:01:10.000000 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-06 00:01:10.000000 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-06 00:01:10.000000 neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-02-06 00:01:06.000000 neon-skill-local_music-2.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-06 00:01:06.000000 neon-skill-local_music-2.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-02-06 00:01:07.000000 neon-skill-local_music-2.0.1a1/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-06 00:01:07.000000 neon-skill-local_music-2.0.1a1/ui/music-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:01:10.759479 neon-skill-local_music-2.0.1a1/util/
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-02-06 00:01:07.000000 neon-skill-local_music-2.0.1a1/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 00:01:07.000000 neon-skill-local_music-2.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.960772 neon-skill-local_music-2.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 00:02:13.960772 neon-skill-local_music-2.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/locale/en-us/vocab/local.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:02:13.960772 neon-skill-local_music-2.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/ui/music-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/version.py
```

### Comparing `neon-skill-local_music-2.0.1a1/LICENSE.md` & `neon-skill-local_music-2.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a1/PKG-INFO` & `neon-skill-local_music-2.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-local_music
-Version: 2.0.1a1
+Version: 2.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-2.0.1a1/README.md` & `neon-skill-local_music-2.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a1/__init__.py` & `neon-skill-local_music-2.0.1a2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,19 @@
                                    requires_gui=False,
                                    no_internet_fallback=True,
                                    no_network_fallback=True,
                                    no_gui_fallback=True)
 
     @property
     def demo_url(self) -> Optional[str]:
-        # default_url = "https://2222.us/app/files/neon_music/music.zip"
         return self.settings.get("demo_url")
 
     @property
     def music_dir(self) -> str:
-        # default_path = "/media"
-        return expanduser(self.settings.get('music_dir', ""))
+        return expanduser(self.settings.get('music_dir') or "~/Music")
 
     @property
     def music_library(self):
         if not self._music_library:
             LOG.info(f"Initializing music library at: {self.music_dir}")
             self._music_library = MusicLibrary(self.music_dir,
                                                self.file_system.path)
```

### Comparing `neon-skill-local_music-2.0.1a1/neon_skill_local_music.egg-info/PKG-INFO` & `neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-local-music
-Version: 2.0.1a1
+Version: 2.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-2.0.1a1/setup.py` & `neon-skill-local_music-2.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a1/skill.json` & `neon-skill-local_music-2.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a1/test/test_skill.py` & `neon-skill-local_music-2.0.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a1/util/__init__.py` & `neon-skill-local_music-2.0.1a2/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,17 @@
         a cached index at the specified `cache_file` path.
         :param library_path: path to scan for music files
         :param cache_path: path to cache directory for library and temp files
         """
         # Hidden files (starting with `.`) are always ignored
         self._ignored_files = ("desktop.ini", "desktop", "Attribution.pdf")
         self._update_lock = RLock()
-        self.library_paths = [expanduser(library_path)]
+        library_path = expanduser(library_path)
+        assert library_path is not None
+        self.library_paths = [library_path]
         self.cache_path = expanduser(cache_path)
         if not isdir(self.cache_path):
             makedirs(self.cache_path)
         self._songs = dict()
         self._db_file = join(self.cache_path, "library.pickle")
         with self._update_lock:
             try:
```

### Comparing `neon-skill-local_music-2.0.1a1/version.py` & `neon-skill-local_music-2.0.1a2/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1a1"
+__version__ = "2.0.1a2"
```

