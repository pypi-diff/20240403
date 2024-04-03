# Comparing `tmp/neon-skill-synonyms-1.0.2a1.tar.gz` & `tmp/neon-skill-synonyms-1.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-synonyms-1.0.2a1.tar", last modified: Tue Feb  6 01:08:32 2024, max compression
+gzip compressed data, was "neon-skill-synonyms-1.0.2a2.tar", last modified: Wed Feb  7 01:02:19 2024, max compression
```

## Comparing `neon-skill-synonyms-1.0.2a1.tar` & `neon-skill-synonyms-1.0.2a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:08:32.083702 neon-skill-synonyms-1.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-06 01:08:32.083702 neon-skill-synonyms-1.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:08:32.079702 neon-skill-synonyms-1.0.2a1/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:08:32.083702 neon-skill-synonyms-1.0.2a1/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/dialog/en-us/add_synonym_command.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/dialog/en-us/new_synonym_command.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/dialog/en-us/synonym_equals_command.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/dialog/en-us/synonym_pair_already_exists.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:08:32.083702 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-06 01:08:32.000000 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-06 01:08:32.000000 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:08:32.000000 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-06 01:08:32.000000 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 01:08:32.000000 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 01:08:32.000000 neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:08:32.083702 neon-skill-synonyms-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:08:32.079702 neon-skill-synonyms-1.0.2a1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:08:32.083702 neon-skill-synonyms-1.0.2a1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/vocab/en-us/for.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/vocab/en-us/particles.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/vocab/en-us/set.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-06 01:08:26.000000 neon-skill-synonyms-1.0.2a1/vocab/en-us/synonym.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:02:19.546207 neon-skill-synonyms-1.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-07 01:02:19.546207 neon-skill-synonyms-1.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:02:19.542207 neon-skill-synonyms-1.0.2a2/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:02:19.546207 neon-skill-synonyms-1.0.2a2/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/dialog/en-us/add_synonym_command.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/dialog/en-us/new_synonym_command.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/dialog/en-us/synonym_equals_command.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/dialog/en-us/synonym_pair_already_exists.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:02:19.546207 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-07 01:02:19.000000 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-07 01:02:19.000000 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 01:02:19.000000 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-07 01:02:19.000000 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-07 01:02:19.000000 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 01:02:19.000000 neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 01:02:19.546207 neon-skill-synonyms-1.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:02:19.542207 neon-skill-synonyms-1.0.2a2/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:02:19.546207 neon-skill-synonyms-1.0.2a2/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/vocab/en-us/for.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/vocab/en-us/particles.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/vocab/en-us/set.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-07 01:02:16.000000 neon-skill-synonyms-1.0.2a2/vocab/en-us/synonym.voc
```

### Comparing `neon-skill-synonyms-1.0.2a1/LICENSE.md` & `neon-skill-synonyms-1.0.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-synonyms-1.0.2a1/PKG-INFO` & `neon-skill-synonyms-1.0.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-synonyms
-Version: 1.0.2a1
+Version: 1.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-synonyms
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-synonyms-1.0.2a1/README.md` & `neon-skill-synonyms-1.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-synonyms-1.0.2a1/__init__.py` & `neon-skill-synonyms-1.0.2a2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         Parse synonym and add to configuration
         :param message: Message associated with request
         :param trigger_phrase: Phrase to listen for
         :param command_phrase: Command to execute when syn_phrase is heard
         :return:
         """
         try:
-            skill_prefs = self.preference_skill(message)
+            skill_prefs = self.settings
             if not skill_prefs.get("synonyms"):
                 skill_prefs["synonyms"] = {}
 
             # Check if spoken request is a valid synonym pair
             if trigger_phrase == command_phrase:
                 self.speak_dialog('synonym_equals_command',
                                   {"syn_phrase": trigger_phrase,
@@ -194,23 +194,23 @@
 
     def _check_utterance_is_synonym(self, message):
         """
         Handler that filters incoming messages and checks if a synonym should be
         emitted in place of incoming utterance
         :param message: Incoming payload object
         """
-        if len(self.preference_skill(message).get("synonyms", {})) == 0:
+        if len(self.settings.get("synonyms", {})) == 0:
             return False
         if message.data.get("utterances"):
             sentence = message.data.get('utterances')[0].lower()
             LOG.info(sentence)
 
-            syn_exec_phrase = [x for x, y in self.preference_skill(message).
-                               get("synonyms", {}).items() if sentence in
-                               [sentence.lower() for sentence in y]]
+            syn_exec_phrase = [x for x, y in
+                               self.settings.get("synonyms", {}).items() if
+                               sentence in [sentence.lower() for sentence in y]]
             LOG.debug(syn_exec_phrase)
         else:
             syn_exec_phrase = False
         LOG.info(syn_exec_phrase)
         if syn_exec_phrase and len(syn_exec_phrase) > 0:
             LOG.info(syn_exec_phrase)
             message.context["neon_should_respond"] = True
```

### Comparing `neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/PKG-INFO` & `neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-synonyms
-Version: 1.0.2a1
+Version: 1.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-synonyms
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-synonyms-1.0.2a1/neon_skill_synonyms.egg-info/SOURCES.txt` & `neon-skill-synonyms-1.0.2a2/neon_skill_synonyms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-synonyms-1.0.2a1/setup.py` & `neon-skill-synonyms-1.0.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-synonyms-1.0.2a1/skill.json` & `neon-skill-synonyms-1.0.2a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-synonyms-1.0.2a1/version.py` & `neon-skill-synonyms-1.0.2a2/version.py`

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

