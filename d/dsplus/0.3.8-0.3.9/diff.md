# Comparing `tmp/dsplus-0.3.8.tar.gz` & `tmp/dsplus-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.3.8.tar", last modified: Tue Apr  2 19:19:49 2024, max compression
+gzip compressed data, was "dsplus-0.3.9.tar", last modified: Tue Apr  2 23:01:33 2024, max compression
```

## Comparing `dsplus-0.3.8.tar` & `dsplus-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.470435 dsplus-0.3.8/
--rw-rw-rw-   0        0        0     1084 2024-03-29 14:28:34.000000 dsplus-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      690 2024-04-02 19:19:49.469864 dsplus-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      105 2024-03-29 14:28:34.000000 dsplus-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.429272 dsplus-0.3.8/dsplus/
--rw-rw-rw-   0        0        0      171 2024-04-02 19:19:36.000000 dsplus-0.3.8/dsplus/__init__.py
--rw-rw-rw-   0        0        0    24320 2024-04-02 19:06:51.000000 dsplus-0.3.8/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    41986 2024-03-29 14:28:34.000000 dsplus-0.3.8/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56679 2024-04-01 14:08:05.000000 dsplus-0.3.8/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    44406 2024-03-29 14:28:34.000000 dsplus-0.3.8/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.454275 dsplus-0.3.8/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 19:19:49.000000 dsplus-0.3.8/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 19:19:49.470955 dsplus-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1693 2024-03-29 18:38:45.000000 dsplus-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 19:19:49.468300 dsplus-0.3.8/tests/
--rw-rw-rw-   0        0        0    12143 2024-03-29 16:50:11.000000 dsplus-0.3.8/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:33.040650 dsplus-0.3.9/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-04-02 23:01:33.036460 dsplus-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:33.006629 dsplus-0.3.9/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-04-02 22:58:04.000000 dsplus-0.3.9/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24320 2024-04-02 22:58:04.000000 dsplus-0.3.9/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    41986 2024-03-29 02:59:14.000000 dsplus-0.3.9/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.3.9/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    44406 2024-03-29 03:03:20.000000 dsplus-0.3.9/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:33.026235 dsplus-0.3.9/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-04-02 23:01:32.000000 dsplus-0.3.9/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-04-02 23:01:32.000000 dsplus-0.3.9/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 23:01:32.000000 dsplus-0.3.9/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 23:01:32.000000 dsplus-0.3.9/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 23:01:33.040650 dsplus-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:33.028331 dsplus-0.3.9/tests/
+-rw-rw-rw-   0        0        0    12143 2024-03-29 17:35:19.000000 dsplus-0.3.9/tests/Test_pandas.py
```

### Comparing `dsplus-0.3.8/LICENSE` & `dsplus-0.3.9/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `dsplus-0.3.8/PKG-INFO` & `dsplus-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.3.8
+Version: 0.3.9
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.3.8/dsplus/pb_functions_general.py` & `dsplus-0.3.9/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.3.8/dsplus/pb_functions_pandas.py` & `dsplus-0.3.9/dsplus/pb_functions_pandas.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.3.8/dsplus/pb_functions_plotly.py` & `dsplus-0.3.9/dsplus/pb_functions_plotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,16 @@
                     kwargs['marginal_x']=self.marginal_x
                     kwargs['marginal_y']=self.marginal_y
                 elif marginal == '':
                     pass
                 else:
                     kwargs['marginal']=self.marginal_xy
 
+                kwargs = {k:v for k,v in kwargs.items() if v is not None}
+
                 # return func(self, *args, **kwargs)
 
                 trace = func(self, *args, **kwargs)
 
                 self._update_legend_show(trace, kwargs.get('legend_show'), kwargs.get('legend_name'))
 
                 self.add(trace)
@@ -867,14 +869,16 @@
                       linewidth = kwargs['border_width'],
                       linecolor = kwargs['border_color'],
                       mirror = kwargs['border_mirror'],
                       range = kwargs['value_range'],
                       categoryorder = kwargs.get('category_order'),
                       autorange = None if kwargs['value_rev'] is None else 'reversed')
 
+        kwargs = {k:v for k,v in kwargs.items() if v is not None}
+
         if axis=='x':
             fig.update_xaxes(**kwargs)
         elif axis=='y':
             fig.update_yaxes(**kwargs)
         else:
             fig.update_xaxes(**kwargs)
             fig.update_yaxes(**kwargs)
@@ -1058,14 +1062,16 @@
             kwargs: Set any other properties that can go into 'update_layout()'.
 
         Returns:
             Self: Self object.
         '''
         fig = self.fig
 
+        kwargs = {k:v for k,v in kwargs.items() if v is not None}
+
         if margins is not None:
             if isinstance(margins, list|tuple):
                 margin_l, margin_r, margin_t, margin_b = margins
             else:
                 margin_l = margins.get('l')
                 margin_r = margins.get('r')
                 margin_t = margins.get('t')
```

### Comparing `dsplus-0.3.8/dsplus/pb_functions_spatial.py` & `dsplus-0.3.9/dsplus/pb_functions_spatial.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.3.8/dsplus.egg-info/PKG-INFO` & `dsplus-0.3.9/dsplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.3.8
+Version: 0.3.9
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.3.8/setup.py` & `dsplus-0.3.9/setup.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from setuptools import setup, find_packages
-from dsplus.__init__ import __version__
-
-setup(
-    name='dsplus',
-    version=__version__,
-    author='Prashana Bajracharya',
-    author_email='pajracharya713@gmail.com',
-    description='Helper functions for data science applications.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    # author=httpimport.__author__,
-    # license='MIT',
-    # url=httpimport.__github__,
-    # py_modules=['dsplus'],
-    packages=find_packages(),
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    # python_requires='>=3.6',
-    # classifiers=[
-    #     'Development Status :: 6 - Mature',
-    #     'Programming Language :: Python :: 3.4',
-    #     'Programming Language :: Python :: 3.7',
-    #     'Programming Language :: Python :: 3.9',
-    #     'Programming Language :: Python :: 3.11',
-    #     'Programming Language :: Python :: Implementation :: CPython',
-    #     'Programming Language :: Python :: Implementation :: PyPy',
-    #     'Intended Audience :: Developers',
-    #     'Intended Audience :: Information Technology',
-    #     'Topic :: Software Development :: Libraries :: Python Modules',
-    #     'Topic :: Software Development :: Build Tools',
-    #     'Topic :: Software Development :: Testing',
-    # ],
-    keywords=[
-        'data science',
-        'pandas'],
-)
+from setuptools import setup, find_packages
+from dsplus.__init__ import __version__
+
+setup(
+    name='dsplus',
+    version=__version__,
+    author='Prashana Bajracharya',
+    author_email='pajracharya713@gmail.com',
+    description='Helper functions for data science applications.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    # author=httpimport.__author__,
+    # license='MIT',
+    # url=httpimport.__github__,
+    # py_modules=['dsplus'],
+    packages=find_packages(),
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    # python_requires='>=3.6',
+    # classifiers=[
+    #     'Development Status :: 6 - Mature',
+    #     'Programming Language :: Python :: 3.4',
+    #     'Programming Language :: Python :: 3.7',
+    #     'Programming Language :: Python :: 3.9',
+    #     'Programming Language :: Python :: 3.11',
+    #     'Programming Language :: Python :: Implementation :: CPython',
+    #     'Programming Language :: Python :: Implementation :: PyPy',
+    #     'Intended Audience :: Developers',
+    #     'Intended Audience :: Information Technology',
+    #     'Topic :: Software Development :: Libraries :: Python Modules',
+    #     'Topic :: Software Development :: Build Tools',
+    #     'Topic :: Software Development :: Testing',
+    # ],
+    keywords=[
+        'data science',
+        'pandas'],
+)
```

### Comparing `dsplus-0.3.8/tests/Test_pandas.py` & `dsplus-0.3.9/tests/Test_pandas.py`

 * *Files identical despite different names*

