# Comparing `tmp/schubmult-1.3.1.tar.gz` & `tmp/schubmult-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.1.tar", last modified: Wed Apr  3 19:26:08 2024, max compression
+gzip compressed data, was "schubmult-1.3.2.tar", last modified: Wed Apr  3 21:06:44 2024, max compression
```

## Comparing `schubmult-1.3.1.tar` & `schubmult-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:08.023000 schubmult-1.3.1/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 19:26:07.984000 schubmult-1.3.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3745 2024-04-03 18:41:26.000000 schubmult-1.3.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:06.147000 schubmult-1.3.1/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.1/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15283 2024-04-03 19:24:23.000000 schubmult-1.3.1/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:06.864000 schubmult-1.3.1/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.1/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.1/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4586 2023-12-24 14:56:44.000000 schubmult-1.3.1/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:07.236000 schubmult-1.3.1/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.1/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.1/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4248 2023-12-24 14:56:50.000000 schubmult-1.3.1/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:07.561000 schubmult-1.3.1/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.1/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.1/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     2851 2024-04-03 19:24:31.000000 schubmult-1.3.1/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:07.909000 schubmult-1.3.1/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.1/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.1/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42129 2024-03-18 16:03:30.000000 schubmult-1.3.1/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 19:26:06.579000 schubmult-1.3.1/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-03 19:26:05.000000 schubmult-1.3.1/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-03 19:26:04.000000 schubmult-1.3.1/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-03 19:26:08.017000 schubmult-1.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1117 2024-04-03 19:25:07.000000 schubmult-1.3.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.764000 schubmult-1.3.2/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 21:06:44.722000 schubmult-1.3.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3745 2024-04-03 18:41:26.000000 schubmult-1.3.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:43.020000 schubmult-1.3.2/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.2/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15361 2024-04-03 21:04:46.000000 schubmult-1.3.2/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:43.729000 schubmult-1.3.2/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.2/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.2/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4586 2023-12-24 14:56:44.000000 schubmult-1.3.2/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.030000 schubmult-1.3.2/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.2/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.2/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4248 2023-12-24 14:56:50.000000 schubmult-1.3.2/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.326000 schubmult-1.3.2/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.2/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.2/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2817 2024-04-03 21:05:09.000000 schubmult-1.3.2/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.649000 schubmult-1.3.2/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.2/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.2/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42129 2024-03-18 16:03:30.000000 schubmult-1.3.2/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:43.447000 schubmult-1.3.2/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-03 21:06:42.000000 schubmult-1.3.2/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-03 21:06:44.758000 schubmult-1.3.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1117 2024-04-03 21:06:00.000000 schubmult-1.3.2/setup.py
```

### Comparing `schubmult-1.3.1/LICENSE` & `schubmult-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.1/PKG-INFO` & `schubmult-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.1
+Version: 1.3.2
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.1/README.md` & `schubmult-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.1/schubmult/perm_lib.py` & `schubmult-1.3.2/schubmult/perm_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,17 +94,17 @@
 def count_bruhat(perm,i,j):
 	up_amount = 0
 	if perm[i]<perm[j]:
 		up_amount = 1
 	else:
 		up_amount = -1
 	for k in range(i+1,j):
-		if perm[i]<perm[k] and perm[j]>perm[k]:
+		if perm[i]<perm[k] and perm[k]<perm[j]:
 			up_amount+=2
-		elif perm[i]>perm[k] and perm[j]<perm[k]:
+		elif perm[i]>perm[k] and perm[k]>perm[j]:
 			up_amount-=2
 	return up_amount
 
 
 def has_bruhat_ascent(perm,i,j):
 	if perm[i]>perm[j]:
 		return False
@@ -141,34 +141,35 @@
 
 
 def elem_sym_perms_q(orig_perm,p,k):	
 	total_list = [(orig_perm,0,1)]
 	up_perm_list = [(orig_perm,1,1000)]
 	for pp in range(p):
 		perm_list = []
-		for up_perm, last, last_j in up_perm_list:	
+		for up_perm, val, last_j in up_perm_list:	
 			up_perm2 = [*up_perm,len(up_perm)+1]
 			if len(up_perm2) < k + 1:
 				up_perm2 += [i+1 for i in range(len(up_perm2),k+2)]
-			pos_list = [i for i in range(k) if i>=len(orig_perm) or up_perm2[i] == orig_perm[i]]
+			pos_list = [i for i in range(k) if (i>=len(orig_perm) and up_perm2[i]==i+1) or (i<len(orig_perm) and up_perm2[i] == orig_perm[i])]
 			for j in range(min(len(up_perm2)-1,last_j),k-1,-1):
 				for i in pos_list:
 					ct = count_bruhat(up_perm2,i,j)
 					#print(f"{up_perm2=} {ct=} {i=} {j=} {k=} {pp=}")
 					if ct == 1 or ct == 2*(i-j)+1:
 						new_perm = [*up_perm2]
 						new_perm[i],new_perm[j] = new_perm[j],new_perm[i]
 						new_perm_add = tuple(permtrim(new_perm))
-						#print(f"{ct=} {i=} {j=} {k=} {last_j=} {pp=} {up_perm2=} {new_perm_add=}")
-						new_last = last
+						new_val = val
 						if ct<0:
-							new_last *= np.prod([q_var[index] for index in range(i+1,j+1)])
-						perm_list += [(new_perm_add,new_last,j)]
-						total_list+=[(new_perm_add,pp+1,new_last)]
+							new_val *= np.prod([q_var[index] for index in range(i+1,j+1)])
+						#print(f"{ct=} {i=} {j=} {k=} {last_j=} {pp=} {up_perm2=} {new_perm_add=} {new_val=}")
+						perm_list += [(new_perm_add,new_val,j)]
+						total_list+=[(new_perm_add,pp+1,new_val)]
 		up_perm_list = perm_list
+	#print(f"{total_list=}")
 	return total_list
 
 
 # perms and inversion diff
 def kdown_perms(perm,monoperm,p,k):	
 	inv_m = inv(monoperm)
 	inv_p = inv(perm)
```

### Comparing `schubmult-1.3.1/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.2/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.1/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.2/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.1/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.2/schubmult/schubmult_q/schubmult_q.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import cache
 from itertools import chain
 from schubmult.perm_lib import *
 import sys
 
 def schubmult(perm_dict,v):
 	vn1 = inverse(v)
-	th = [len(v)-i for i in range(1,len(v))]	
+	th = [len(v)-i for i in range(1,len(v)+1)]	
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	#print(f"{th=} {mu=} {vmu=}")
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
@@ -26,25 +26,24 @@
 			for vp in vpathdicts[index]:
 				for v2,vdiff,s in vpathdicts[index][vp]:
 					if th[index]-vdiff > mx_th:
 						mx_th = th[index] - vdiff					
 			newpathsums = {}
 			for up in vpathsums:
 				newperms = elem_sym_perms_q(up,mx_th,th[index])
-				for vp in vpathsums[up]:
-					sumval = vpathsums[up][vp]
-					if sumval == 0:
-						continue
-					for v2,vdiff,s in vpathdicts[index][vp]:
-						addsumval = s*sumval
-						for up2, udiff, mul_val in newperms:					
-							if vdiff + udiff == th[index]:								
-								if up2 not in newpathsums:
-									newpathsums[up2]={}
-								newpathsums[up2][v2] = newpathsums[up2].get(v2,0)+mul_val*addsumval
+				for up2, udiff, mul_val in newperms:
+					if up2 not in newpathsums:
+						newpathsums[up2]={}
+					for v in vpathdicts[index]:
+						sumval = vpathsums[up].get(v,zero)
+						if sumval == 0:
+							continue
+						for v2,vdiff,s in vpathdicts[index][v]:
+							if udiff+vdiff==th[index]:
+								newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*mul_val
 			vpathsums = newpathsums
 		toget = tuple(vmu)
 		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
 	return ret_dict
 
 
 def main():
```

### Comparing `schubmult-1.3.1/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.2/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.1/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.2/schubmult.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.1
+Version: 1.3.2
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.1/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.2/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.1/setup.py` & `schubmult-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.1",
+    version="1.3.2",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

