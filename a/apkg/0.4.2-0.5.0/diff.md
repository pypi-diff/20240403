# Comparing `tmp/apkg-0.4.2.tar.gz` & `tmp/apkg-0.5.0.tar.gz`

## Comparing `apkg-0.4.2.tar` & `apkg-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/CHANGELOG.md -> docs/news.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 apkg-0.4.2/requirements.txt
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apkg-0.4.2/setup.cfg
--rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 apkg-0.4.2/setup.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/__main__.py
--rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/adistro.py
--rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/cache.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/cli.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/compat.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/ex.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/log.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/parse.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyle.py
--rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgtemplate.py
--rw-r--r--   0        0        0    12761 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgtest.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/project.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/__init__.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/build.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/build_dep.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/clean.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/compat.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/get_archive.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/info.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/install.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/make_archive.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/srcpkg.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/status.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/system_setup.py
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/test.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/test_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/__init__.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/arch.py
--rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/deb.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/nix.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/rpm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/archive.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/common.py
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/git.py
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/run.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/shutil35.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/test.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/upstreamversion.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 apkg-0.4.2/scripts/make-archive.sh
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 apkg-0.4.2/scripts/upstream-version.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 apkg-0.4.2/.gitignore
--rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 apkg-0.4.2/COPYING
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 apkg-0.4.2/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 apkg-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 apkg-0.4.2/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.5.0/CHANGELOG.md -> docs/news.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 apkg-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apkg-0.5.0/setup.cfg
+-rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 apkg-0.5.0/setup.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/__main__.py
+-rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/adistro.py
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/cache.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/cli.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/compat.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/ex.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/log.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/parse.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgstyle.py
+-rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgtemplate.py
+-rw-r--r--   0        0        0    12761 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgtest.py
+-rw-r--r--   0        0        0    10412 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/project.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/__init__.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/build.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/build_dep.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/clean.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/compat.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/get_archive.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/info.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/install.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/make_archive.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/srcpkg.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/status.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/system_setup.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/test.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/commands/test_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgstyles/__init__.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgstyles/arch.py
+-rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgstyles/deb.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgstyles/nix.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/pkgstyles/rpm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/templatevars/__init__.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/templatevars/debseries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/archive.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/common.py
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/git.py
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/run.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/shutil35.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/test.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 apkg-0.5.0/apkg/util/upstreamversion.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 apkg-0.5.0/scripts/make-archive.sh
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 apkg-0.5.0/scripts/upstream-version.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 apkg-0.5.0/.gitignore
+-rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 apkg-0.5.0/COPYING
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 apkg-0.5.0/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 apkg-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 apkg-0.5.0/PKG-INFO
```

### Comparing `apkg-0.4.2/setup.cfg` & `apkg-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/setup.py` & `apkg-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/adistro.py` & `apkg-0.5.0/apkg/adistro.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/cache.py` & `apkg-0.5.0/apkg/cache.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/cli.py` & `apkg-0.5.0/apkg/cli.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/compat.py` & `apkg-0.5.0/apkg/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from apkg.util.upstreamversion import latest_apkg_version
 
 
 log = getLogger(__name__)
 
 
 # current apkg compatibility level
-COMPAT_LEVEL = 3
+COMPAT_LEVEL = 4
 
 
 COMPAT_LEVEL_NOTES = {
+    4: ('0.5.0', """Forward compatible update, no action required."""),
     3: ('0.4.0', """Forward compatible update, no action required."""),
     2: ('0.3.0', """Forward compatible update for most users.
 
 ## new flexible template selection mechanism
 
 Make sure each template dir in distro/pkg/ matches name
 of a respective pkgstyle such as deb, rpm, arch, or nix.
```

### Comparing `apkg-0.4.2/apkg/ex.py` & `apkg-0.5.0/apkg/ex.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,19 @@
         " apkg compat level {apkg}.\n\n"
         "Run `apkg compat` for more information.\n\n"
         "Please upgrade apkg to work with this project."
     )
     returncode = 20
 
 
+class InvalidVariablesSource(ApkgException):
+    msg_fmt = "Invalid variables source: {src}"
+    returncode = 26
+
+
 # 30-39: Missing and NotFound
 class MissingRequiredArgument(ApkgException):
     msg_fmt = "Missing required argument: {arg}"
     returncode = 30
 
 
 class MissingRequiredConfigOption(ApkgException):
```

### Comparing `apkg-0.4.2/apkg/log.py` & `apkg-0.5.0/apkg/log.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/parse.py` & `apkg-0.5.0/apkg/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from apkg import ex
 
 
 # subgroups:
 # 1) name
 # 2) name-version separator ('-' or '_')
 # 3) version (including release)
-RE_NVR = r'^(.+?)([-_])(v?\d+(?:\.\d+)+(?:.+?)?)$'
+RE_NVR = r'^(.+?)([-_])(v?\d+(?:\.\d+)*(?:.+?)?)$'
 
 
 def split_archive_ext(archive_fn):
     """
     split archive file into base name and extension such as '.tar.gz'
 
     return (name, extension)
```

### Comparing `apkg-0.4.2/apkg/pkgstyle.py` & `apkg-0.5.0/apkg/pkgstyle.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/pkgtemplate.py` & `apkg-0.5.0/apkg/pkgtemplate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """
 module for handling and rendering apkg package templates
 """
+from collections import UserDict
 import glob
+import importlib.util
 import os
 
 from pathlib import Path
 import jinja2
 import jinja2.ext
 from markupsafe import Markup
 
+from apkg import ex
 from apkg import adistro
 from apkg.log import getLogger
 from apkg import pkgstyle as _pkgstyle
+from apkg.pkgstyle import call_pkgstyle_fun
 from apkg.util import common
 import apkg.util.shutil35 as shutil
 
 
 log = getLogger(__name__)
 
 
 DUMMY_VARS = {
     'name': 'PKGNAME',
     'version': '0.VERSION',
     'release': '0.RELEASE',
-    'nvr': 'NVR',
+    'nvr': 'NAME-VERSION-RELEASE',
     'distro': 'DISTRO',
 }
 
 # package template selection types ordered by priority
 TS_ALIAS, TS_DISTRO, TS_PKGSTYLE = range(3)
 TEMPLATE_SELECTION_STR = {
     TS_ALIAS: 'distro alias',
@@ -63,28 +67,30 @@
         src = self.environment.loader.get_source(self.environment, filename)[0]
         return Markup(src.rstrip('\n'))
 
 
 # pylint: disable=too-many-instance-attributes
 class PackageTemplate:
     def __init__(self, path, style=None, selection=TS_DISTRO,
-                 ignore_files=None, plain_copy_files=None):
+                 ignore_files=None, plain_copy_files=None,
+                 variables_sources=None):
         self.path = Path(path)
         self.style = style
         self.selection = selection
         self.distro_rules = None
 
         if ignore_files is None:
             self.ignore_files = DEFAULT_IGNORE_FILES
         else:
             self.ignore_files = ignore_files
         if plain_copy_files is None:
             self.plain_copy_files = DEFAULT_PLAIN_COPY_FILES
         else:
             self.plain_copy_files = plain_copy_files
+        self.variables_sources = variables_sources
 
         self.setup_env()
 
     def setup_env(self):
         self.env = jinja2.Environment(
             loader=jinja2.FileSystemLoader('.'),
             extensions=[IncludeRawExtension])
@@ -112,29 +118,53 @@
         return TEMPLATE_SELECTION_STR.get(self.selection, 'INVALID')
 
     def match_distro(self, distro):
         return self.distro_rules.match(distro)
 
     def template_vars(self, tvars=None):
         """
-        get/update template variables from pkgstyle
+        get/update template variables
         """
+        vars_ = DUMMY_VARS.copy()
+
+        # package name from template
+        name = call_pkgstyle_fun(
+            self.pkgstyle, 'get_template_name', self.path)
+        vars_['name'] = name
         # static pkgstyle vars
-        result = getattr(self.pkgstyle, 'TEMPLATE_VARS', {})
+        vars_pkgstyle = getattr(self.pkgstyle, 'TEMPLATE_VARS', {})
+        vars_.update(vars_pkgstyle)
         # dynamic pkgstyle vars resolved at render time
-        tvars_dyn = getattr(self.pkgstyle, 'TEMPLATE_VARS_DYNAMIC', {})
-        if tvars_dyn:
-            _vars = {}
-            for name, fun in tvars_dyn.items():
-                _vars[name] = fun()
-            result.update(_vars)
-        # custom supplied vars
+        vars_dyn = getattr(self.pkgstyle, 'TEMPLATE_VARS_DYNAMIC', {})
+        if vars_dyn:
+            for name, fun in vars_dyn.items():
+                vars_[name] = fun()
+        # supplied vars
         if tvars:
-            result.update(tvars)
-        return result
+            vars_.update(tvars)
+        # custom variables
+        if self.variables_sources:
+            vars_ = self.custom_vars(vars_)
+
+        return vars_
+
+    def custom_vars(self, tvars):
+        """
+        get/update template variables from custom sources
+        """
+        for vsrc in self.variables_sources:
+            vsrc.validate()
+            log.info("custom variables from %s: %s",
+                     vsrc.src_attr, vsrc.src_val)
+            custom_tvars = vsrc.get_variables(tvars)
+            log.verbose("%s custom variables: %s",
+                        len(custom_tvars), custom_tvars)
+            tvars.update(custom_tvars)
+
+        return tvars
 
     def render(self, out_path, tvars):
         """
         render package template into specified output directory
 
         Args:
             out_path: output base path
@@ -187,24 +217,27 @@
     def __repr__(self):
         return "PackageTemplate<%s,%s>" % (self.name, self.pkgstyle.name)
 
 
 def load_templates(path,
                    distro_aliases=None,
                    ignore_files=None,
-                   plain_copy_files=None):
+                   plain_copy_files=None,
+                   variables_sources=None):
     """
     load package templates sorted by evaluation priority
 
     Params:
         path - templates base path (i.e.: distro/pkg)
         distro_aliases - distro aliases dict (optional)
         ignore_files - list of file patterns to ignore (optional)
         plain_copy_files - list of file patterns to copy
                            without templating (optional)
+        variables_sources - list of sources to define
+                            template variables (optional)
 
     Returns:
         list of PackageTemplates in order they should
         be evaluated (by selection type):
 
         1) distro alias templates
         2) distro-specific templates
@@ -220,15 +253,16 @@
         if not os.path.isdir(entry_path):
             # ignore non-dirs
             continue
 
         template = PackageTemplate(
             entry_path,
             ignore_files=ignore_files,
-            plain_copy_files=plain_copy_files)
+            plain_copy_files=plain_copy_files,
+            variables_sources=variables_sources)
 
         if not template.pkgstyle:
             log.warning("ignoring unknown package style in %s", entry_path)
             continue
 
         alias_rules = aliases.get(template.name)
         if alias_rules:
@@ -263,7 +297,91 @@
     for da in distro_aliases:
         for at in alias_templates:
             if at.name == da:
                 result.append(at)
                 break
     assert len(alias_templates) == len(result)
     return result
+
+
+class VariablesSource(UserDict):
+    VARS_SOURCES = ['local_module', 'python_module']
+
+    def __init__(self, **kwargs):
+        super().__init__(kwargs)
+
+    @property
+    def local_module(self):
+        return self.get('local_module', None)
+
+    @property
+    def python_module(self):
+        return self.get('python_module', None)
+
+    @property
+    def src_attr(self):
+        for src in self.VARS_SOURCES:
+            if src in self.data:
+                return src
+        return None
+
+    @property
+    def src_val(self):
+        return self.data.get(self.src_attr, None)
+
+    def validate(self):
+        src_attrs = [src for src in self.VARS_SOURCES if self.get(src)]
+        n_src = len(src_attrs)
+        if n_src < 1:
+            raise ex.InvalidVariablesSource(
+                src="no source specified: %s" % self)
+        if n_src > 1:
+            raise ex.InvalidVariablesSource(
+                src="multiple conflicting sources: %s" % self)
+        return True
+
+    def exists(self):
+        if self.src_attr == 'local_module':
+            return Path(self.local_module).exists()
+        elif self.src_attr == 'python_module':
+            try:
+                spec = importlib.util.find_spec(self.python_module)
+                return spec is not None
+            except ModuleNotFoundError:
+                return False
+        else:
+            return False
+
+    def get_variables(self, tvars):
+        if self.local_module:
+            if not os.path.exists(self.local_module):
+                raise ex.InvalidVariablesSource(
+                    src='local_module not found: %s' % (self.local_module))
+
+            spec = importlib.util.spec_from_file_location(
+                "custom_variables", self.local_module)
+
+            custom_module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(custom_module)
+        elif self.python_module:
+            try:
+                custom_module = importlib.import_module(self.python_module)
+            except ModuleNotFoundError:
+                raise ex.InvalidVariablesSource(
+                    src='python_module not found: %s' % self.python_module)
+
+        custom_fun = getattr(custom_module, 'get_variables', None)
+        if not custom_fun:
+            raise ex.InvalidVariablesSource(
+                src='%s missing required get_variables function: %s'
+                % (self.src_val, custom_module))
+
+        custom_tvars = custom_fun(tvars)
+        return custom_tvars
+
+
+def parse_variables_sources(config):
+    sources = []
+    for vcfg in config:
+        vsrc = VariablesSource(**vcfg)
+        sources.append(vsrc)
+    return sources
```

### Comparing `apkg-0.4.2/apkg/pkgtest.py` & `apkg-0.5.0/apkg/pkgtest.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/project.py` & `apkg-0.5.0/apkg/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     """
     Project class serves as high level interface to projecs in need of
     packaging
     """
     name = None
     config = {}
     distro_aliases = {}
+    variables_sources = []
 
     def __init__(
             self,
             base_path=None,
             input_path=None,
             output_path=None,
             auto_load=True,
@@ -101,14 +102,15 @@
     def load(self):
         """
         load project config and update attributes
         """
         self.load_config()
         self.update_attrs()
         self.update_distro_aliases()
+        self.update_variables_sources()
         if self.auto_compat:
             self.ensure_compat()
 
     def reload(self,
                base_path=None,
                input_path=None,
                output_path=None):
@@ -165,14 +167,21 @@
     def update_distro_aliases(self):
         """
         load distro aliases from project config
         """
         conf = self.config_get('distro.aliases', [])
         self.distro_aliases = adistro.parse_distro_aliases(conf)
 
+    def update_variables_sources(self):
+        """
+        load custom variables sources from project config
+        """
+        conf = self.config_get('template.variables', [])
+        self.variables_sources = pkgtemplate.parse_variables_sources(conf)
+
     @cached_property
     def vcs(self):
         """
         Version Control System used in project
 
         possible outputs: 'git', None
         """
@@ -252,15 +261,16 @@
         if self.path.templates.exists():
             ignore_files = self.config_get('template.ignore_files')
             plain_copy_files = self.config_get('template.plain_copy_files')
             return pkgtemplate.load_templates(
                 self.path.templates,
                 distro_aliases=self.distro_aliases,
                 ignore_files=ignore_files,
-                plain_copy_files=plain_copy_files)
+                plain_copy_files=plain_copy_files,
+                variables_sources=self.variables_sources)
         else:
             return []
 
     def get_template_for_distro_(self, distro):
         for t in self.templates:
             if t.match_distro(distro):
                 return t
```

### Comparing `apkg-0.4.2/apkg/terminal.py` & `apkg-0.5.0/apkg/terminal.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/build.py` & `apkg-0.5.0/apkg/commands/build.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/build_dep.py` & `apkg-0.5.0/apkg/commands/build_dep.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/clean.py` & `apkg-0.5.0/apkg/commands/clean.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/compat.py` & `apkg-0.5.0/apkg/commands/compat.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/get_archive.py` & `apkg-0.5.0/apkg/commands/get_archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/install.py` & `apkg-0.5.0/apkg/commands/install.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/make_archive.py` & `apkg-0.5.0/apkg/commands/make_archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/srcpkg.py` & `apkg-0.5.0/apkg/commands/srcpkg.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/status.py` & `apkg-0.5.0/apkg/commands/status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 
 from apkg import adistro
 from apkg import compat
+from apkg import ex
 from apkg.log import getLogger, T
 from apkg.project import Project
 
 
 log = getLogger(__name__)
 
 
@@ -49,14 +50,15 @@
     if compat_ok:
         msg += " ({t.green}{state}{t.normal})"
     else:
         msg += (" ({t.warn}{state}"
                 " -> run {t.command}apkg compat{t.normal})")
     print(msg.format(level=level, state=compat_state, t=T))
 
+    print()
     msg = "package templates path:  {t.bold}{path}{t.normal}"
     if proj.path.templates.exists():
         msg += " ({t.green}exists{t.normal})"
     else:
         msg += " ({t.red}doesn't exist{t.normal})"
     print(msg.format(path=proj.path.templates, t=T))
 
@@ -70,14 +72,35 @@
                 % (short_path, template.pkgstyle.name,
                    template.selection_str(), template.distro_rules))
         msg = "\n".join(msg_lines)
     else:
         msg = "    {t.red}no package templates found{t.normal}"
     print(msg.format(dir=proj.path.templates, t=T))
 
+    print("template variables sources:")
+    if proj.variables_sources:
+        msg_lines = []
+        for vsrc in proj.variables_sources:
+            try:
+                vsrc.validate()
+                line = ("%s: {t.bold}%s{t.normal}"
+                        % (vsrc.src_attr, vsrc.src_val))
+                if vsrc.exists():
+                    line += " ({t.green}exists{t.normal})"
+                else:
+                    line += " ({t.red}doesn't exist{t.normal})"
+                line = line.format(t=T)
+            except ex.InvalidVariablesSource as e:
+                line = "{t.red}%s{t.normal}".format(t=T) % e
+            msg_lines.append("    %s" % line)
+        msg = "\n".join(msg_lines)
+    else:
+        msg = "    no custom variables sources defined"
+    print(msg)
+
     print()
     if distro:
         # target distro status
         distro = adistro.Distro(distro)
         msg = "target distro: {t.cyan}{id}{t.normal}"
         print(msg.format(id=distro, t=T))
     else:
```

### Comparing `apkg-0.4.2/apkg/commands/system_setup.py` & `apkg-0.5.0/apkg/commands/system_setup.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/test.py` & `apkg-0.5.0/apkg/commands/test.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/commands/test_dep.py` & `apkg-0.5.0/apkg/commands/test_dep.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/pkgstyles/arch.py` & `apkg-0.5.0/apkg/pkgstyles/arch.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/pkgstyles/deb.py` & `apkg-0.5.0/apkg/pkgstyles/deb.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,15 @@
  * core: `devscripts`
  * isolated build: `pbuilder`
 
 **template variables:**
 
  * `now`: current date in Debian changelog format (RFC 2822)
 """
+import email
 import email.utils
 import glob
 import os
 from pathlib import Path
 import re
 import sys
 import tempfile
@@ -92,25 +93,56 @@
 
 
 def get_srcpkg_nvr(path):
     nvr, _, _ = str(path.name).rpartition('.')
     return nvr
 
 
-def copy_srcpkg_files(src_path, dst_path):
-    # not part of pkgstyle interface yet but probably should be
-    for pattern in [
-            '*.dsc',
-            '*_source.*',  # questionable, some tools need these
-            '*.debian.tar.*',
-            '*.orig.tar.*',
-            '*.diff.*']:
-        for f in glob.iglob('%s/%s' % (src_path, pattern)):
-            srcp = Path(f)
-            shutil.copyfile(f, dst_path / srcp.name)
+def copy_pkg_files(src_path, dst_path):
+    """
+    copy package files at src_path to dst_path
+
+    Find a single *.changes file at src_path
+    and copy it and all files it references to dst_path.
+
+    Return a list of all files copied.
+
+    This isn't a part of pkgstyle interface as it's fairly specific to Debian
+    """
+    changes = list(glob.iglob('%s/*.changes' % (src_path)))
+    if not changes:
+        raise ex.UnexpectedCommandOutput(
+            msg="no *.changes files found when copying package")
+    if len(changes) > 1:
+        raise ex.UnexpectedCommandOutput(
+            msg="multiple *.changes files found when copying package")
+
+    changes_path = Path(changes[0])
+    changes_dst_path = dst_path / changes_path.name
+    result = []
+    shutil.copyfile(changes_path, changes_dst_path)
+    result.append(changes_dst_path)
+
+    parser = email.parser.HeaderParser()
+    parsed = parser.parsestr(changes_path.read_text())
+    for entry in parsed['Files'].split('\n'):
+        if not entry:
+            # first line is empty
+            continue
+        items = re.split(r'\s+', entry.strip(), 5)
+        if len(items) < 5:
+            log.warning("Invalid *.changes line: %s", entry)
+            continue
+        name = items[4]
+        src = src_path / name
+        dst = dst_path / name
+        shutil.copyfile(src, dst)
+        result.append(dst)
+
+    return result
 
 
 def build_srcpkg(
         build_path,
         out_path,
         archive_paths,
         template,
@@ -146,25 +178,20 @@
             '-nc',  # do not pre clean source tree
             '-us',  # unsigned source package.
             '-uc',  # unsigned .changes file.
             )
 
     log.info("copying source package to result dir: %s", out_path)
     out_path.mkdir(parents=True)
-    copy_srcpkg_files(build_path, out_path)
-    fns = glob.glob('%s/*' % out_path)
-    # make sure .dsc is first
-    for i, fn in enumerate(fns):
-        if fn.endswith('.dsc'):
-            fns = [fns.pop(i)] + fns
-            break
-    else:
+    copied = copy_pkg_files(build_path, out_path)
+    dscs = [path for path in copied if path.suffix == '.dsc']
+    if not dscs:
         raise ex.UnexpectedCommandOutput(
-            msg="no *.dsc found after moving built source package")
-    return list(map(Path, fns))
+            msg="no *.dsc files found after source package build")
+    return dscs
 
 
 def build_packages(
         build_path,
         out_path,
         srcpkg_paths,
         **kwargs):
@@ -201,21 +228,20 @@
         with cd(source_path):
             # build
             run('dpkg-buildpackage',
                 '-us',  # unsigned source package.
                 '-uc',  # unsigned .changes file.
                 )
 
-    pkgs = []
     log.info("copying built packages to result dir: %s", out_path)
-    for src_pkg in glob.iglob('%s/*.deb' % build_path):
-        dst_pkg = out_path / Path(src_pkg).name
-        shutil.copyfile(src_pkg, dst_pkg)
-        pkgs.append(dst_pkg)
-
+    copied = copy_pkg_files(build_path, out_path)
+    pkgs = [path for path in copied if path.suffix in ['.deb', '.ddeb']]
+    if not pkgs:
+        raise ex.UnexpectedCommandOutput(
+            msg="no *.deb packages found after build")
     return pkgs
 
 
 def install_distro_packages(
         packages,
         **kwargs):
     interactive = kwargs.get('interactive', False)
```

### Comparing `apkg-0.4.2/apkg/pkgstyles/nix.py` & `apkg-0.5.0/apkg/pkgstyles/nix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
-apkg package style for **Nix** (NixOS.org).
+apkg package style for **Nix** ([NixOS.org](https://nixos.org)).
 
 **source template:**
- - `default.nix` as-if in https://github.com/NixOS/nixpkgs
- - `top-level.nix` that simply wraps it to work outside that official tree,
+
+- `default.nix` as-if in [https://github.com/NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)
+- `top-level.nix` that simply wraps it to work outside that official tree,
    in particular it should substitute the source archive;
-   e.g. see ../../distro/pkg/nix/top-level.nix
+   e.g. see `apkg/distro/pkg/nix/top-level.nix`
 
 **source package:** the same, just with templates substituted
 
 **packages:** symlink to your local nix store (for the primary package output)
 """
 import os
 import re
```

### Comparing `apkg-0.4.2/apkg/pkgstyles/rpm.py` & `apkg-0.5.0/apkg/pkgstyles/rpm.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/archive.py` & `apkg-0.5.0/apkg/util/archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/common.py` & `apkg-0.5.0/apkg/util/common.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/git.py` & `apkg-0.5.0/apkg/util/git.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/run.py` & `apkg-0.5.0/apkg/util/run.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/shutil35.py` & `apkg-0.5.0/apkg/util/shutil35.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/test.py` & `apkg-0.5.0/apkg/util/test.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/apkg/util/upstreamversion.py` & `apkg-0.5.0/apkg/util/upstreamversion.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/scripts/make-archive.sh` & `apkg-0.5.0/scripts/make-archive.sh`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/COPYING` & `apkg-0.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/README.md` & `apkg-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/pyproject.toml` & `apkg-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apkg-0.4.2/PKG-INFO` & `apkg-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: apkg
-Version: 0.4.2
+Version: 0.5.0
 Summary: cross-distro upstream packaging automation tool
 Project-URL: Documentation, https://gitlab.nic.cz/packaging/apkg/-/blob/master/README.md
 Project-URL: Issues, https://gitlab.nic.cz/packaging/apkg/-/issues
 Project-URL: Source, https://gitlab.nic.cz/packaging/apkg
 Author-email: Jakub Ružička <jakub.ruzicka@nic.cz>
 License: MIT
 License-File: COPYING
```

