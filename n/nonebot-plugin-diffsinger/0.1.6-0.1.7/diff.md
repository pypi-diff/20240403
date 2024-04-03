# Comparing `tmp/nonebot_plugin_diffsinger-0.1.6.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.6.tar", last modified: Wed Apr  3 09:18:40 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.7.tar", last modified: Wed Apr  3 09:51:12 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.6.tar` & `nonebot_plugin_diffsinger-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:18:40.024602 nonebot_plugin_diffsinger-0.1.6/
--rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2049 2024-04-03 09:18:40.023605 nonebot_plugin_diffsinger-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1263 2024-04-03 04:10:04.000000 nonebot_plugin_diffsinger-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:18:40.014469 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger/
--rw-rw-rw-   0        0        0     3235 2024-04-03 09:16:09.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger/__init__.py
--rw-rw-rw-   0        0        0       97 2024-04-03 08:27:42.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger/config.py
--rw-rw-rw-   0        0        0     1438 2024-04-03 07:44:09.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger/data_source.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:18:40.022400 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger.egg-info/
--rw-rw-rw-   0        0        0     2049 2024-04-03 09:18:39.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-04-03 09:18:39.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:18:39.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-03 09:18:39.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 09:18:39.000000 nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:18:40.024602 nonebot_plugin_diffsinger-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     3806 2024-04-03 09:18:22.000000 nonebot_plugin_diffsinger-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.6/LICENSE` & `nonebot_plugin_diffsinger-0.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 zhzhongshi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2024 zhzhongshi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `nonebot_plugin_diffsinger-0.1.6/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.6/setup.py` & `nonebot_plugin_diffsinger-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'nonebot_plugin_diffsinger'
-DESCRIPTION = '用DiffSinger让bot唱歌'
-URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
-EMAIL = 'zhzhongshi@qq.com'
-AUTHOR = 'zhzhongshi'
-REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.6'
-REQUIRED = [
-    "nonebot2","nonebot-adapter-onebot","httpx","librosa"
-]
-# What packages are optional?
-EXTRAS = {
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license='MIT',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'nonebot_plugin_diffsinger'
+DESCRIPTION = '用DiffSinger让bot唱歌'
+URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
+EMAIL = 'zhzhongshi@qq.com'
+AUTHOR = 'zhzhongshi'
+REQUIRES_PYTHON = '>=3.8.0'
+VERSION = '0.1.7'
+REQUIRED = [
+    "nonebot2","nonebot-adapter-onebot","httpx","librosa"
+]
+# What packages are optional?
+EXTRAS = {
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license='MIT',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
 )
```

