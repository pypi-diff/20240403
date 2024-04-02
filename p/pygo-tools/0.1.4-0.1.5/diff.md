# Comparing `tmp/pygo-tools-0.1.4.tar.gz` & `tmp/pygo-tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygo-tools-0.1.4.tar", last modified: Sun Mar 31 15:49:16 2024, max compression
+gzip compressed data, was "pygo-tools-0.1.5.tar", last modified: Tue Apr  2 22:32:32 2024, max compression
```

## Comparing `pygo-tools-0.1.4.tar` & `pygo-tools-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:49:16.105512 pygo-tools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-03-31 15:49:16.105512 pygo-tools-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:49:16.101512 pygo-tools-0.1.4/pygo_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/build_ffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:49:16.101512 pygo-tools-0.1.4/pygo_tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/util/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pygo_tools/util/pathlib_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:49:16.101512 pygo-tools-0.1.4/pygo_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-03-31 15:49:16.000000 pygo-tools-0.1.4/pygo_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-31 15:49:16.000000 pygo-tools-0.1.4/pygo_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 15:49:16.000000 pygo-tools-0.1.4/pygo_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 15:49:16.000000 pygo-tools-0.1.4/pygo_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-31 15:49:16.000000 pygo-tools-0.1.4/pygo_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 15:49:16.000000 pygo-tools-0.1.4/pygo_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-31 15:48:54.000000 pygo-tools-0.1.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 15:49:16.105512 pygo-tools-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/pygo_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/build_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/pygo_tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/util/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/util/pathlib_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/pygo_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/setup.cfg
```

### Comparing `pygo-tools-0.1.4/PKG-INFO` & `pygo-tools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygo-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simplify Python-Go integration for Libraries with Precompiled Extensions
 Author-email: Rajan Khullar <rkhullar03@gmail.com>
 License: MIT NON-AI License
 Project-URL: Repository, https://github.com/rkhullar/python-libraries/tree/main/pygo-tools
 Keywords: python,golang,cffi
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pygo-tools-0.1.4/pygo_tools/backend.py` & `pygo-tools-0.1.5/pygo_tools/backend.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.4/pygo_tools/build_ffi.py` & `pygo-tools-0.1.5/pygo_tools/build_ffi.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.4/pygo_tools/config.py` & `pygo-tools-0.1.5/pygo_tools/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     def extension_path(self) -> Path:
         return self.project_path / self.package / f'{self.extension}.abi3.so'
 
     @property
     def library_source_path(self) -> Path:
         return self.project_path / self.package / 'go'
 
+    @property
+    def library_target_path(self) -> Path:
+        return self.library_source_path / 'local'
+
     @classmethod
     def from_json(cls) -> 'Config':
         setup_path = cls.get_path('setup.py')
         config_path = cls.get_path('config.json')
         if setup_path.exists() and config_path.exists():
             with config_path.open('r') as f:
                 data = json.load(f)
```

### Comparing `pygo-tools-0.1.4/pygo_tools/setup.py` & `pygo-tools-0.1.5/pygo_tools/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 
 from .config import Config
 
 
 def precompile(config: Config):
     subprocess.run('make', cwd=config.library_source_path)
+    if not config.library_path.exists():
+        config.library_path.symlink_to(config.library_target_path)
 
 
-def find_wheel(config: Config) -> Path | None:
-    dist_path = config.project_path / 'dist'
+def find_wheel(config: Config, dist_path: Path = None) -> Path | None:
+    dist_path = dist_path or config.project_path / 'dist'
     for path in dist_path.rglob('*.whl'):
         return path
 
 
 def build_ffi(config: Config, target: str = None, rename: bool = True) -> Path | None:
     command = ['build-ffi']
     if target:
@@ -37,37 +39,39 @@
         commands = [
             ['zip', '-j', str(wheel_path), str(path)],
         ]
         for command in commands:
             subprocess.run(command, cwd=dist_path)
 
 
-def patch_wheel_darwin(config: Config):
-    if wheel_path := find_wheel(config):
-        dist_path = wheel_path.parent
-        lib_file, ext_file = f'lib{config.library}.so', f'{config.extension}.abi3.so'
-        commands = [
-            ['unzip', str(wheel_path), ext_file],
-            ['install_name_tool', '-change', lib_file, f'@loader_path/{config.package}/lib/{lib_file}', ext_file],
-            ['otool', '-L', ext_file],
-            ['zip', '-d', str(wheel_path), ext_file],
-            ['zip', '-u', str(wheel_path), ext_file],
-            ['rm', '-rf', ext_file]
-        ]
-        for command in commands:
-            subprocess.run(command, cwd=dist_path)
+def patch_wheel_darwin(config: Config, wheel_path: Path):
+    dist_path = wheel_path.parent
+    lib_file, ext_file = f'lib{config.library}.so', f'{config.extension}.abi3.so'
+    commands = [
+        ['unzip', str(wheel_path), ext_file],
+        ['install_name_tool', '-change', lib_file, f'@loader_path/{config.package}/lib/{lib_file}', ext_file],
+        ['otool', '-L', ext_file],
+        ['zip', '-d', str(wheel_path), ext_file],
+        ['zip', '-u', str(wheel_path), ext_file],
+        ['rm', '-rf', ext_file]
+    ]
+    for command in commands:
+        subprocess.run(command, cwd=dist_path)
 
 
 class BuildGoWheel(_bdist_wheel):
     def run(self):
         config = Config.from_json()
         precompile(config)
         _bdist_wheel.run(self)
         if config.platform == 'darwin':
-            patch_wheel_darwin(config)
+            wheel_path = find_wheel(config, dist_path=Path(self.dist_dir))
+            if not wheel_path:
+                raise FileNotFoundError(f'could not find wheel to patch')
+            patch_wheel_darwin(config, wheel_path=wheel_path)
 
 
 def setup(cffi: str = 'cffi', config_path: str = None, **kwargs):
     if config_path:
         os.environ['PYGO_CONFIG_PATH'] = config_path
     cmdclass = kwargs.pop('cmdclass', dict())
     install_requires = kwargs.get('install_requires', list())
```

### Comparing `pygo-tools-0.1.4/pygo_tools/util/monkey_patch.py` & `pygo-tools-0.1.5/pygo_tools/util/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.4/pygo_tools.egg-info/PKG-INFO` & `pygo-tools-0.1.5/pygo_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygo-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simplify Python-Go integration for Libraries with Precompiled Extensions
 Author-email: Rajan Khullar <rkhullar03@gmail.com>
 License: MIT NON-AI License
 Project-URL: Repository, https://github.com/rkhullar/python-libraries/tree/main/pygo-tools
 Keywords: python,golang,cffi
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pygo-tools-0.1.4/pyproject.toml` & `pygo-tools-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.4/readme.md` & `pygo-tools-0.1.5/readme.md`

 * *Files identical despite different names*

