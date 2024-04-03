# Comparing `tmp/pairlist-0.5.1.2.tar.gz` & `tmp/pairlist-0.5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pairlist-0.5.1.2.tar", max compression
+gzip compressed data, was "pairlist-0.5.1.3.tar", max compression
```

## Comparing `pairlist-0.5.1.2.tar` & `pairlist-0.5.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3020 2023-12-11 03:26:44.107996 pairlist-0.5.1.2/README.md
--rw-r--r--   0        0        0     1233 2023-12-11 03:59:08.553024 pairlist-0.5.1.2/build.py
--rw-r--r--   0        0        0     4743 2021-03-23 12:44:02.423984 pairlist-0.5.1.2/csource/cpairlist.c
--rw-r--r--   0        0        0    15048 2021-03-15 05:17:26.373669 pairlist-0.5.1.2/csource/pairlist.c
--rw-r--r--   0        0        0      378 2018-04-06 23:30:44.000000 pairlist-0.5.1.2/csource/pairlist.h
--rw-r--r--   0        0        0    13055 2023-12-11 02:01:49.054144 pairlist-0.5.1.2/pairlist.py
--rw-r--r--   0        0        0      652 2023-12-11 04:06:25.214600 pairlist-0.5.1.2/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 pairlist-0.5.1.2/setup.py
--rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 pairlist-0.5.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3020 2023-12-11 03:26:44.107996 pairlist-0.5.1.3/README.md
+-rw-r--r--   0        0        0     1233 2024-04-03 14:52:00.104074 pairlist-0.5.1.3/build.py
+-rw-r--r--   0        0        0     4743 2021-03-23 12:44:02.423984 pairlist-0.5.1.3/csource/cpairlist.c
+-rw-r--r--   0        0        0    15048 2021-03-15 05:17:26.373669 pairlist-0.5.1.3/csource/pairlist.c
+-rw-r--r--   0        0        0      378 2018-04-06 23:30:44.000000 pairlist-0.5.1.3/csource/pairlist.h
+-rw-r--r--   0        0        0    13055 2024-04-03 14:57:18.815810 pairlist-0.5.1.3/pairlist.py
+-rw-r--r--   0        0        0      682 2024-04-03 14:59:36.074665 pairlist-0.5.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 pairlist-0.5.1.3/setup.py
+-rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 pairlist-0.5.1.3/PKG-INFO
```

### Comparing `pairlist-0.5.1.2/README.md` & `pairlist-0.5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pairlist-0.5.1.2/build.py` & `pairlist-0.5.1.3/build.py`

 * *Files identical despite different names*

### Comparing `pairlist-0.5.1.2/csource/cpairlist.c` & `pairlist-0.5.1.3/csource/cpairlist.c`

 * *Files identical despite different names*

### Comparing `pairlist-0.5.1.2/csource/pairlist.c` & `pairlist-0.5.1.3/csource/pairlist.c`

 * *Files identical despite different names*

### Comparing `pairlist-0.5.1.2/pairlist.py` & `pairlist-0.5.1.3/pairlist.py`

 * *Files identical despite different names*

### Comparing `pairlist-0.5.1.2/pyproject.toml` & `pairlist-0.5.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pairlist"
-version = "0.5.1.2"
+version = "0.5.1.3"
 description = "Generate neighbor list for the particles in a periodic boundary cell."
 authors = ["vitroid <vitroid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = [{path = "csource/"}]
 
 [tool.poetry.build]
@@ -15,15 +15,17 @@
 python = "^3.9"
 numpy = "^1.26.2"
 
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^69.0.2"
 networkx = "^3.2.1"
-genice = {path = "../GenIce2"}
+genice2 = "^2.2"
 jinja2 = "^3.1.2"
 toml = "^0.10.2"
 pdoc = "^14.1.0"
+ipykernel = "^6.29.4"
+matplotlib = "^3.8.3"
 
 [build-system]
 requires = ["poetry-core", "setuptools", "numpy"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pairlist-0.5.1.2/setup.py` & `pairlist-0.5.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['pairlist']
 install_requires = \
 ['numpy>=1.26.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'pairlist',
-    'version': '0.5.1.2',
+    'version': '0.5.1.3',
     'description': 'Generate neighbor list for the particles in a periodic boundary cell.',
     'long_description': '# pairlist\nGenerates the pair list of atoms that are closer to each other than the\ngiven threshold under the periodic boundary conditions.\n\nversion 0.5.1.1\n\n## Usage\n\nSee `pairlist.h` for the function definition and `pairlist-test.c` for usage.\n\nPython API is served in pairlist.py. The API document is [here](https://vitroid.github.io/PairList/pairlist.html).\n\nTo find the neighbors in a face-centered cubic lattice of size 10x10x10 on a MacBook Air 2021 (Apple Silicon),\n\n```shell\n$ python benchmark.py\nINFO crude: Neighboring pair list by a crude double loop.\nINFO crude: 18024 ms\nINFO crude: end.\n24000 pairs\nINFO numpyish: Neighboring pair list by numpy fancy array.\nINFO numpyish: 741 ms\nINFO numpyish: end.\n24000.0 pairs\nINFO pairlist_py: Neighboring pair list by pairlist in pure python.\nINFO pairlist_py: 125 ms\nINFO pairlist_py: end.\n24000 pairs\nINFO pairlist_c: Neighboring pair list by pairlist in c.\nINFO pairlist_c: end.\nINFO pairlist_c: 16 ms\n24000 pairs\n```\n\n```python\nimport pairlist as pl\nfrom fcc import FaceCenteredCubic\nfrom logging import getLogger, basicConfig, INFO, DEBUG\nfrom decorator import timeit, banner\nimport numpy as np\nfrom pairlist import pairs_py, pairs2_py\n\n\nbasicConfig(level=INFO, format="%(levelname)s %(message)s")\nlogger = getLogger()\nlogger.debug("Debug mode.")\n\n\n@banner\n@timeit\ndef crude(lattice, cell, rc=1.1):\n    "Neighboring pair list by a crude double loop."\n    rc2 = rc**2\n    count = 0\n    for i in range(len(lattice)):\n        for j in range(i):\n            d = lattice[i] - lattice[j]\n            d -= np.floor(d + 0.5)\n            d = d @ cell\n            if d @ d < rc2:\n                count += 1\n    return count\n\n\n@banner\n@timeit\ndef numpyish(lattice, cell, rc=1.1):\n    "Neighboring pair list by numpy fancy array."\n    # cross-differences\n    M = lattice[:, None, :] - lattice[None, :, :]\n    # wrap\n    M -= np.floor(M + 0.5)\n    # in absolute coordinate\n    M = M @ cell\n    d = (M * M).sum(2)\n    return d[(d < rc**2) & (0 < d)].shape[0] / 2\n\n\n@banner\n@timeit\ndef pairlist_py(lattice, cell, rc=1.1):\n    "Neighboring pair list by pairlist in pure python."\n    count = 0\n    for i, j, d in pl.pairs_iter(\n        lattice, maxdist=rc, cell=cell, _engine=(pairs_py, pairs2_py)\n    ):\n        count += 1\n    return count\n\n\n@timeit\n@banner\ndef pairlist_c(lattice, cell, rc=1.1):\n    "Neighboring pair list by pairlist in c."\n    count = 0\n    for i, j, d in pl.pairs_iter(lattice, maxdist=rc, cell=cell):\n        count += 1\n    return count\n\n\nlattice, cell = FaceCenteredCubic(10)\n\nprint(crude(lattice, cell), "pairs")\nprint(numpyish(lattice, cell), "pairs")\nprint(pairlist_py(lattice, cell), "pairs")\nprint(pairlist_c(lattice, cell), "pairs")\n\n```\n\n![benchmark](https://github.com/vitroid/PairList/raw/master/benchmark/benchmark.png)\n\n## Algorithm\n\nA simple cell division algorithm is implemented.\n\n## Demo\n\nIt requires [GenIce](https://github.com/vitroid/GenIce) to make the test data.\n\n```shell\n% make test\n```\n\n## Requirements\n\n* python\n* numpy\n\n\n## Bugs\n\n',
     'author': 'vitroid',
     'author_email': 'vitroid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pairlist-0.5.1.2/PKG-INFO` & `pairlist-0.5.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pairlist
-Version: 0.5.1.2
+Version: 0.5.1.3
 Summary: Generate neighbor list for the particles in a periodic boundary cell.
 License: MIT
 Author: vitroid
 Author-email: vitroid@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

