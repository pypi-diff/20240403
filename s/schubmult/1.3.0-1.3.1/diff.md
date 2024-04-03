# Comparing `tmp/schubmult-1.3.0.tar.gz` & `tmp/schubmult-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.0.tar", last modified: Wed Apr  3 18:42:23 2024, max compression
+gzip compressed data, was "schubmult-1.3.1.tar", last modified: Wed Apr  3 19:26:08 2024, max compression
```

## Comparing `schubmult-1.3.0.tar` & `schubmult-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:23.392000 schubmult-1.3.0/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 18:42:23.344000 schubmult-1.3.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3745 2024-04-03 18:41:26.000000 schubmult-1.3.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:21.434000 schubmult-1.3.0/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.0/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15144 2024-04-03 18:11:49.000000 schubmult-1.3.0/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:22.209000 schubmult-1.3.0/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.0/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.0/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4586 2023-12-24 14:56:44.000000 schubmult-1.3.0/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:22.543000 schubmult-1.3.0/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.0/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.0/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4248 2023-12-24 14:56:50.000000 schubmult-1.3.0/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:22.904000 schubmult-1.3.0/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.0/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.0/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     2819 2024-04-03 18:35:54.000000 schubmult-1.3.0/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:23.272000 schubmult-1.3.0/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.0/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.0/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42129 2024-03-18 16:03:30.000000 schubmult-1.3.0/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:21.877000 schubmult-1.3.0/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 18:42:19.000000 schubmult-1.3.0/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-03 18:42:23.377000 schubmult-1.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1117 2024-04-03 18:19:55.000000 schubmult-1.3.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:08.023000 schubmult-1.3.1/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 19:26:07.984000 schubmult-1.3.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3745 2024-04-03 18:41:26.000000 schubmult-1.3.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:06.147000 schubmult-1.3.1/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.1/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15283 2024-04-03 19:24:23.000000 schubmult-1.3.1/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:06.864000 schubmult-1.3.1/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.1/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.1/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4586 2023-12-24 14:56:44.000000 schubmult-1.3.1/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:07.236000 schubmult-1.3.1/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.1/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.1/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4248 2023-12-24 14:56:50.000000 schubmult-1.3.1/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:07.561000 schubmult-1.3.1/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.1/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.1/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2851 2024-04-03 19:24:31.000000 schubmult-1.3.1/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:07.909000 schubmult-1.3.1/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.1/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.1/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42129 2024-03-18 16:03:30.000000 schubmult-1.3.1/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:06.579000 schubmult-1.3.1/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-03 19:26:05.000000 schubmult-1.3.1/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-03 19:26:08.017000 schubmult-1.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1117 2024-04-03 19:25:07.000000 schubmult-1.3.1/setup.py
```

### Comparing `schubmult-1.3.0/LICENSE` & `schubmult-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.0/PKG-INFO` & `schubmult-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.0
+Version: 1.3.1
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.0/README.md` & `schubmult-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.0/schubmult/perm_lib.py` & `schubmult-1.3.1/schubmult/perm_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,17 @@
 	up_amount = 0
 	if perm[i]<perm[j]:
 		up_amount = 1
 	else:
 		up_amount = -1
 	for k in range(i+1,j):
 		if perm[i]<perm[k] and perm[j]>perm[k]:
-			up_amount+=1
+			up_amount+=2
 		elif perm[i]>perm[k] and perm[j]<perm[k]:
-			up_amount-=1
+			up_amount-=2
 	return up_amount
 
 
 def has_bruhat_ascent(perm,i,j):
 	if perm[i]>perm[j]:
 		return False
 	for p in range(i+1,j):
@@ -146,21 +146,23 @@
 	for pp in range(p):
 		perm_list = []
 		for up_perm, last, last_j in up_perm_list:	
 			up_perm2 = [*up_perm,len(up_perm)+1]
 			if len(up_perm2) < k + 1:
 				up_perm2 += [i+1 for i in range(len(up_perm2),k+2)]
 			pos_list = [i for i in range(k) if i>=len(orig_perm) or up_perm2[i] == orig_perm[i]]
-			for j in range(min(last_j,len(up_perm2)-1),k-1,-1):
+			for j in range(min(len(up_perm2)-1,last_j),k-1,-1):
 				for i in pos_list:
 					ct = count_bruhat(up_perm2,i,j)
+					#print(f"{up_perm2=} {ct=} {i=} {j=} {k=} {pp=}")
 					if ct == 1 or ct == 2*(i-j)+1:
 						new_perm = [*up_perm2]
 						new_perm[i],new_perm[j] = new_perm[j],new_perm[i]
 						new_perm_add = tuple(permtrim(new_perm))
+						#print(f"{ct=} {i=} {j=} {k=} {last_j=} {pp=} {up_perm2=} {new_perm_add=}")
 						new_last = last
 						if ct<0:
 							new_last *= np.prod([q_var[index] for index in range(i+1,j+1)])
 						perm_list += [(new_perm_add,new_last,j)]
 						total_list+=[(new_perm_add,pp+1,new_last)]
 		up_perm_list = perm_list
 	return total_list
```

### Comparing `schubmult-1.3.0/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.1/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.0/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.1/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.0/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.1/schubmult/schubmult_q/schubmult_q.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 
 def schubmult(perm_dict,v):
 	vn1 = inverse(v)
 	th = [len(v)-i for i in range(1,len(v))]	
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
+	#print(f"{th=} {mu=} {vmu=}")
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
 	while th[-1] == 0:
 		th.pop()
 	thL = len(th)
```

### Comparing `schubmult-1.3.0/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.1/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.0/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.1/schubmult.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.0
+Version: 1.3.1
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.0/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.1/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.0/setup.py` & `schubmult-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.0",
+    version="1.3.1",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

