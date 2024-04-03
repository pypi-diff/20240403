# Comparing `tmp/schubmult-1.2.9.tar.gz` & `tmp/schubmult-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.2.9.tar", last modified: Mon Jan 15 18:30:45 2024, max compression
+gzip compressed data, was "schubmult-1.3.0.tar", last modified: Wed Apr  3 18:42:23 2024, max compression
```

## Comparing `schubmult-1.2.9.tar` & `schubmult-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-01-15 18:30:45.239000 schubmult-1.2.9/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    35149 2023-09-24 17:08:26.000000 schubmult-1.2.9/LICENSE
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     3949 2024-01-15 18:30:45.189000 schubmult-1.2.9/PKG-INFO
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     3567 2023-11-08 17:08:40.000000 schubmult-1.2.9/README.md
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-01-15 18:30:43.564000 schubmult-1.2.9/schubmult/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2023-09-24 17:08:26.000000 schubmult-1.2.9/schubmult/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    13839 2023-12-24 16:32:39.000000 schubmult-1.2.9/schubmult/perm_lib.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-01-15 18:30:44.386000 schubmult-1.2.9/schubmult/schubmult_double/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       41 2023-09-25 01:39:08.000000 schubmult-1.2.9/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       97 2023-09-26 17:55:50.000000 schubmult-1.2.9/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     4586 2023-12-24 14:56:44.000000 schubmult-1.2.9/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-01-15 18:30:44.751000 schubmult-1.2.9/schubmult/schubmult_py/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       36 2023-09-25 01:39:03.000000 schubmult-1.2.9/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       94 2023-09-26 17:55:38.000000 schubmult-1.2.9/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     4248 2023-12-24 14:56:50.000000 schubmult-1.2.9/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-01-15 18:30:45.111000 schubmult-1.2.9/schubmult/schubmult_yz/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       27 2023-09-25 01:38:28.000000 schubmult-1.2.9/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       93 2023-09-26 17:55:32.000000 schubmult-1.2.9/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    38444 2024-01-15 17:04:53.000000 schubmult-1.2.9/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-01-15 18:30:44.055000 schubmult-1.2.9/schubmult.egg-info/
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     3949 2024-01-15 18:30:42.000000 schubmult-1.2.9/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)      623 2024-01-15 18:30:42.000000 schubmult-1.2.9/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        1 2024-01-15 18:30:42.000000 schubmult-1.2.9/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)      183 2024-01-15 18:30:42.000000 schubmult-1.2.9/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       83 2024-01-15 18:30:42.000000 schubmult-1.2.9/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       10 2024-01-15 18:30:42.000000 schubmult-1.2.9/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       79 2024-01-15 18:30:45.223000 schubmult-1.2.9/setup.cfg
--rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     1064 2024-01-15 18:30:13.000000 schubmult-1.2.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:23.392000 schubmult-1.3.0/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 18:42:23.344000 schubmult-1.3.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3745 2024-04-03 18:41:26.000000 schubmult-1.3.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:21.434000 schubmult-1.3.0/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.0/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15144 2024-04-03 18:11:49.000000 schubmult-1.3.0/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:22.209000 schubmult-1.3.0/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.0/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.0/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4586 2023-12-24 14:56:44.000000 schubmult-1.3.0/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:22.543000 schubmult-1.3.0/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.0/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.0/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4248 2023-12-24 14:56:50.000000 schubmult-1.3.0/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:22.904000 schubmult-1.3.0/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.0/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.0/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2819 2024-04-03 18:35:54.000000 schubmult-1.3.0/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:23.272000 schubmult-1.3.0/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.0/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.0/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42129 2024-03-18 16:03:30.000000 schubmult-1.3.0/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 18:42:21.877000 schubmult-1.3.0/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 18:42:19.000000 schubmult-1.3.0/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-03 18:42:20.000000 schubmult-1.3.0/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-03 18:42:23.377000 schubmult-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1117 2024-04-03 18:19:55.000000 schubmult-1.3.0/setup.py
```

### Comparing `schubmult-1.2.9/LICENSE` & `schubmult-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.2.9/PKG-INFO` & `schubmult-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.2.9
+Version: 1.3.0
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.0, it also handles quantum Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
 schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6
+schubmult_q 5 1 4 3 2 - 2 1 3 5 4
 ```
 
 The same execution with the Lehmer code:
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
 schubmult_yz -code 0 1 1 2 - 1 0 2 3
+schubmult_q -code 4 0 2 1 - 1 0 0 1
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4
@@ -46,15 +48,15 @@
 
 
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Both have the same command line syntax as schubmult. schubmult_double displays the result with nonnegative coefficients in terms of the negative simple roots. Both are of course slower than schubmult_py, and expressing the result positively for schubmult_double slows it down even more.
 
-New in version 1.1.0, schubmult_py -coprod allows you to split Schubert polynomials along certain indices. It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
+New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6)) # outputs dictionary with results
```

### Comparing `schubmult-1.2.9/README.md` & `schubmult-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.0, it also handles quantum Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
 schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6
+schubmult_q 5 1 4 3 2 - 2 1 3 5 4
 ```
 
 The same execution with the Lehmer code:
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
 schubmult_yz -code 0 1 1 2 - 1 0 2 3
+schubmult_q -code 4 0 2 1 - 1 0 0 1
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4
@@ -33,15 +35,15 @@
 
 
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Both have the same command line syntax as schubmult. schubmult_double displays the result with nonnegative coefficients in terms of the negative simple roots. Both are of course slower than schubmult_py, and expressing the result positively for schubmult_double slows it down even more.
 
-New in version 1.1.0, schubmult_py -coprod allows you to split Schubert polynomials along certain indices. It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
+New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6)) # outputs dictionary with results
```

### Comparing `schubmult-1.2.9/schubmult/perm_lib.py` & `schubmult-1.3.0/schubmult/perm_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from symengine import *
 from functools import cache
 from itertools import chain
 from bisect import bisect_left
+import numpy as np
+
+n = 100
+
+q_var = symarray("q",n)
 
 def inv(perm):
 	L = len(perm)
 	v = [i for i in range(1,L+1)]
 	ans = 0
 	for i in range(L):
 		itr = bisect_left(v, perm[i])
@@ -82,14 +87,28 @@
 	if perm[i]<perm[j]:
 		return False
 	for p in range(i+1,j):
 		if perm[i]>perm[p] and perm[p]>perm[j]:
 			return False
 	return True
 
+def count_bruhat(perm,i,j):
+	up_amount = 0
+	if perm[i]<perm[j]:
+		up_amount = 1
+	else:
+		up_amount = -1
+	for k in range(i+1,j):
+		if perm[i]<perm[k] and perm[j]>perm[k]:
+			up_amount+=1
+		elif perm[i]>perm[k] and perm[j]<perm[k]:
+			up_amount-=1
+	return up_amount
+
+
 def has_bruhat_ascent(perm,i,j):
 	if perm[i]>perm[j]:
 		return False
 	for p in range(i+1,j):
 		if perm[i]<perm[p] and perm[p]<perm[j]:
 			return False
 	return True	
@@ -116,14 +135,41 @@
 						else:
 							new_perm_add = tuple(new_perm)
 						perm_list += [(new_perm_add,up_perm2[j])]
 						total_list+=[(new_perm_add,pp+1)]
 		up_perm_list = perm_list
 	return total_list
 
+
+def elem_sym_perms_q(orig_perm,p,k):	
+	total_list = [(orig_perm,0,1)]
+	up_perm_list = [(orig_perm,1,1000)]
+	for pp in range(p):
+		perm_list = []
+		for up_perm, last, last_j in up_perm_list:	
+			up_perm2 = [*up_perm,len(up_perm)+1]
+			if len(up_perm2) < k + 1:
+				up_perm2 += [i+1 for i in range(len(up_perm2),k+2)]
+			pos_list = [i for i in range(k) if i>=len(orig_perm) or up_perm2[i] == orig_perm[i]]
+			for j in range(min(last_j,len(up_perm2)-1),k-1,-1):
+				for i in pos_list:
+					ct = count_bruhat(up_perm2,i,j)
+					if ct == 1 or ct == 2*(i-j)+1:
+						new_perm = [*up_perm2]
+						new_perm[i],new_perm[j] = new_perm[j],new_perm[i]
+						new_perm_add = tuple(permtrim(new_perm))
+						new_last = last
+						if ct<0:
+							new_last *= np.prod([q_var[index] for index in range(i+1,j+1)])
+						perm_list += [(new_perm_add,new_last,j)]
+						total_list+=[(new_perm_add,pp+1,new_last)]
+		up_perm_list = perm_list
+	return total_list
+
+
 # perms and inversion diff
 def kdown_perms(perm,monoperm,p,k):	
 	inv_m = inv(monoperm)
 	inv_p = inv(perm)
 	full_perm_list = []
 	
 	if inv(mulperm(list(perm),monoperm)) == inv_m - inv_p:
```

### Comparing `schubmult-1.2.9/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.0/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.2.9/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.0/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.2.9/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.0/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files 7% similar despite different names*

```diff
@@ -732,24 +732,51 @@
 			done = True
 		if started and cd[i] == 0:
 			found_zero_after = True
 	if started or done:
 		return True
 	return False
 
-@cached(cache={}, key=lambda val, u2,v2,w2,var2=var2,var3=var3,msg=False,do_pos_neg=True: hashkey(u2,v2,w2,var2,var3,msg,do_pos_neg))
-def posify(val,u2,v2,w2,var2=var2,var3=var3,msg=False,do_pos_neg=True):
-	if inv(u2)+inv(v2) - inv(w2)<=1:
-		return expand(val)
+def div_diff(i,poly):
+	return sympify(sympy.div(sympy.sympify(poly - permy(poly,i)),sympy.sympify(var2[i]-var2[i+1]))[0])
+
+def skew_div_diff(u,w,poly):
+	d = -1
+	for i in range(len(w)-1):
+		if w[i]>w[i+1]:
+			d = i
+			break
+	d2 = -1
+	for i in range(len(u)-1):
+		if u[i]>u[i+1]:
+			d2 = i
+			break
+	if d == -1:
+		if d2 == -1:
+			return poly
+		return 0
+	w2 = [*w]
+	w2[d], w2[d+1] = w2[d+1], w2[d]
+	if d<len(u)-1 and u[d]>u[d+1]:		
+		u2 = [*u]		
+		u2[d], u2[d+1] = u2[d+1], u2[d]
+		return skew_div_diff(u2,w2,permy(poly,d+1))
+	else:
+		return skew_div_diff(u,w2,div_diff(d+1,poly))
+
+@cached(cache={}, key=lambda val, u2,v2,w2,var2=var2,var3=var3,msg=False,do_pos_neg=True,sign_only=False: hashkey(u2,v2,w2,var2,var3,msg,do_pos_neg,sign_only))
+def posify(val,u2,v2,w2,var2=var2,var3=var3,msg=False,do_pos_neg=True,sign_only=False):
+	if inv(u2)+inv(v2) - inv(w2) == 0:
+		return val
 	cdv = code(v2)	
-	if set(cdv) == set([0,1]):		
+	if set(cdv) == set([0,1]) and do_pos_neg:	
 		return val
 	#if is_hook(cdv):
 	#	print(f"Could've {cdv}")
-	if expand(val) == 0:
+	if not sign_only and expand(val) == 0:
 		return 0
 	
 	u, v, w = try_reduce_v(u2, v2, w2)
 	if is_coeff_irreducible(u,v,w):
 		u, v, w = try_reduce_u(u2, v2, w2)
 		if is_coeff_irreducible(u,v,w):
 			u, v, w = [*u2], [*v2], [*w2]
@@ -763,41 +790,50 @@
 							w0 = w
 							u, v, w = reduce_descents(u,v,w)						
 							if is_coeff_irreducible(u,v,w):	
 								u, v, w = reduce_coeff(u,v,w)
 	u = tuple(u)
 	v = tuple(v)	
 	w = tuple(w)
+	
+	if w != w2 and sign_only:
+		return 0
 			
 	if is_coeff_irreducible(u,v,w):
 		u3, v3, w3 = try_reduce_v(u, v, w)
 		if not is_coeff_irreducible(u3,v3,w3):
 			u, v, w = u3, v3, w3
 		else:
 			u3, v3, w3 = try_reduce_u(u, v, w)		
 			if not is_coeff_irreducible(u3,v3,w3):
 				u, v, w = u3, v3, w3
 	split_two_b, split_two = is_split_two(u,v,w)
-
+	
 	if len([i for i in code(v) if i !=0]) == 1:
+		if sign_only:
+			return 0
 		cv = code(v)
 		for i in range(len(cv)):
 			if cv[i]!=0:
 				k = i+1
 				p = cv[i]
 				break					
 		inv_u = inv(u)
 		r = inv(w) - inv_u
 		val = 0
 		w2 = w
 		hvarset = [w2[i] for i in range(min(len(w2),k))]+[i+1 for i in range(len(w2),k)] + [w2[b] for b in range(k,len(u)) if u[b]!=w2[b]]+[w2[b] for b in range(len(u),len(w2))]
 		val = elem_sym_poly(p-r,k+p-1,[-var3[i] for i in range(1,n)],[-var2[i] for i in hvarset])	
 	elif (will_formula_work(v,u) or dominates(u,w)):
+		if sign_only:
+			return 0
 		val = dualcoeff(u,v,w,var2,var3)
 	elif inv(w) - inv(u) == 1:	
+		if sign_only:
+			return 0
 		a, b = -1, -1
 		for i in range(len(w)):
 			if a == -1 and u[i] != w[i]:
 				a = i
 			elif i>=len(u) and w[i] != i+1:
 				b = i
 			elif b == -1 and u[i] != w[i]:
@@ -843,14 +879,16 @@
 				else:
 					yv = w[i]
 				for j in range(len(oaf)):				
 					toadd*= var2[yv] - var3[oaf[j]]
 			toadd *= schubpoly(v3,[0,var2[w[a]],var2[w[b]]],var3)
 			val += toadd
 	elif split_two_b:
+		if sign_only:
+			return 0
 		cycles = split_two
 		a1, b1 = cycles[0]
 		a2, b2 = cycles[1]
 		a1-=1
 		b1-=1
 		a2-=1
 		b2-=1
@@ -996,38 +1034,88 @@
 			if doschubpoly:
 				toadd *= schubpoly(v3,varo,var3)
 			else:
 				subs_dict3 = {var2[i]: varo[i] for i in range(len(varo))}
 				toadd*=tomul.subs(subs_dict3)
 			val += toadd
 	elif will_formula_work(u,v):
+		if sign_only:
+			return 0
 		val = forwardcoeff(u,v,w,var2,var3)
+	#elif inv(w) - inv(u) == 2:
+	#	indices = []
+	#	for i in range(len(w)):
+	#		if i>=len(u) or u[i]!=w[i]:
+	#			indices += [i+1]
+	#	arr = [[[],v]]
+	#	d = -1
+	#	for i in range(len(v)-1):
+	#		if v[i]>v[i+1]:
+	#			d = i + 1
+	#	for i in range(d):
+	#		arr2 = []
+	#					
+	#		if i+1 in indices:
+	#			continue
+	#		i2 = 1
+	#		i2 += len([aa for aa in indices if i+1>aa])
+	#		for vr, v2 in arr:
+	#			dpret = pull_out_var(i2,[*v2])
+	#			for v3r, v3 in dpret:
+	#				arr2 += [[vr + [(v3r,i+1)],v3]]
+	#		arr = arr2
+	#	val = 0
+	#	
+	#	for L in arr:
+	#		v3 = [*L[-1]]
+	#		tomul = 1
+	#		pooly = skew_div_diff(u,w,schubpoly(v3,[0,*[var2[a] for a in indices]],var3))
+	#		coeff = compute_positive_rep(pooly,var2,var3,msg,False)
+	#		if coeff == -1:
+	#			return -1
+	#		tomul = sympify(coeff)
+	#		toadd = 1
+	#		for i in range(len(L[0])):
+	#			var_index = L[0][i][1]
+	#			oaf = L[0][i][0]
+	#			if var_index-1>=len(w):
+	#				yv = var_index
+	#			else:
+	#				yv = w[var_index-1]
+	#			for j in range(len(oaf)):				
+	#				toadd*= var2[yv] - var3[oaf[j]]
+	#		toadd*=tomul#.subs(subs_dict3)
+	#		val += toadd		
 	else:
 		c01 = code(u)
 		c02 = code(w)
 		c03 = code(v)
 		
 		c1 = code(inverse(u))
 		c2 = code(inverse(w))
 		
 		if one_dominates(u,w):
+			if sign_only:
+				return 0
 			while c1[0] != c2[0]:				
 				w = [*w]
 				v = [*v]
 				w[c2[0]-1], w[c2[0]] = w[c2[0]], w[c2[0]-1]
 				v[c2[0]-1], v[c2[0]] = v[c2[0]], v[c2[0]-1]
 				w = tuple(w)
 				v = tuple(v)
 				c2 = code(inverse(w))
 				c03 = code(v)
 				c01 = code(u)
 				c02 = code(w)				
 				
 		
 		if is_reducible(v):
+			if sign_only:
+				return 0
 			newc = []
 			elemc = []
 			for i in range(len(c03)):
 				if c03[i]>0:
 					newc += [c03[i]-1]
 					elemc += [1]
 				else:
@@ -1037,41 +1125,109 @@
 			val = 0
 			for new_w in coeff_dict:
 				tomul = coeff_dict[new_w]
 				newval = schubmult_one(new_w,tuple(permtrim(uncode(newc))),var2,var3).get(tuple(permtrim([*w])),0)
 				newval = posify(newval,new_w,tuple(permtrim(uncode(newc))),w,var2,var3,msg,do_pos_neg)
 				val += tomul*shiftsubz(newval)
 		elif c01[0] == c02[0] and c01[0] != 0:
+			if sign_only:
+				return 0
 			varl = c01[0]
 			u3 = uncode([0] + c01[1:])
 			w3 = uncode([0] + c02[1:])
 			val = 0
 			val = schubmult_one(tuple(permtrim(u3)),tuple(permtrim([*v])),var2,var3).get(tuple(permtrim(w3)),0)
 			val = posify(val,tuple(permtrim(u3)),tuple(permtrim([*v])),tuple(permtrim(w3)),var2,var3,msg,do_pos_neg)
 			for i in range(varl):
 				val = permy(val,i+1)			
 		elif c1[0] == c2[0]:
+			if sign_only:
+				return 0
 			vp = pull_out_var(c1[0]+1,[*v])
 			u3 = tuple(permtrim(phi1(u)))
 			w3 = tuple(permtrim(phi1(w)))
 			c3 = code(inverse(u3))
 			c4 = code(inverse(w3))
 			val = 0
 			for arr, v3 in vp:
 				tomul = 1
 				for i in range(len(arr)):
 					tomul*=var2[1] - var3[arr[i]]
 				
 				val2 = schubmult_one(tuple(permtrim(u3)),tuple(permtrim(v3)),var2,var3).get(tuple(permtrim(w3)),0)
 				val2 = posify(val2,u3,tuple(permtrim(v3)),w3,var2,var3,msg,do_pos_neg)
 				val += tomul*shiftsub(val2)
+		elif inv(w)-inv(u)==2:
+			indices = []
+			for i in range(len(w)):
+				if i>=len(u) or u[i]!=w[i]:
+					indices += [i+1]
+			arr = [[[],v]]
+			d = -1
+			for i in range(len(v)-1):
+				if v[i]>v[i+1]:
+					d = i + 1
+			for i in range(d):
+				arr2 = []
+							
+				if i+1 in indices:
+					continue
+				i2 = 1
+				i2 += len([aa for aa in indices if i+1>aa])
+				for vr, v2 in arr:
+					dpret = pull_out_var(i2,[*v2])
+					for v3r, v3 in dpret:
+						arr2 += [[vr + [(v3r,i+1)],v3]]
+				arr = arr2
+			val = 0
+			
+			for L in arr:
+				v3 = [*L[-1]]
+				tomul = 1						
+				toadd = 1
+				for i in range(len(L[0])):
+					var_index = L[0][i][1]
+					oaf = L[0][i][0]
+					if var_index-1>=len(w):
+						yv = var_index
+					else:
+						yv = w[var_index-1]
+					for j in range(len(oaf)):				
+						toadd*= var2[yv] - var3[oaf[j]]
+				pooly = skew_div_diff(u,w,schubpoly(v3,[0,*[var2[a] for a in indices]],var3))
+				if toadd == 0:
+					continue
+				if pooly !=0:
+					coeff = compute_positive_rep(pooly,var2,var3,msg,False)
+				else:
+					coeff = 0
+				if coeff == -1:
+					return -1
+				tomul = sympify(coeff)
+				toadd*=tomul#.subs(subs_dict3)
+				val += toadd						
 		else:
-			val2 = compute_positive_rep(val,var2,var3,msg,do_pos_neg)
-			if val2 is not None:
-				val = val2
+			if not sign_only:
+				if inv(u)+inv(v)-inv(w)==1:
+					val2 = compute_positive_rep(val,var2,var3,msg,False)
+				else:
+					val2 = compute_positive_rep(val,var2,var3,msg,do_pos_neg)					
+				if val2 is not None:				
+					val = val2							
+			else:
+				#st = str(expand(val))
+				#if st.find("-")!=-1:
+				#	return -1
+				#else:
+				#	return val
+				d = expand(val).as_coefficients_dict()
+				for v in d.values():
+					if v<0:
+						return -1
+				return 1
 	return val
 
 def split_perms(perms):
 	perms2 = [perms[0]]
 	for perm in perms[1:]:
 		cd = code(perm)
 		index = -1
@@ -1302,23 +1458,22 @@
 				size = len(perms)
 				perms = split_perms(perms)
 			
 			coeff_dict = {perms[0]: 1}
 			check_coeff_dict = {perms[0]: 1}
 			for perm in orig_perms[1:]:
 				check_coeff_dict = schubmult(check_coeff_dict,perm)
-			if display_positive and len(perms)==2 and will_formula_work(perms[0],perms[1]) and perms[0]:
+			if display_positive and len(perms)==2 and will_formula_work(perms[0],perms[1]):
 				coeff_dict = {}
 				th = theta(perms[1])
 				muv = uncode(th)
 				muvn1v = mulperm(inverse(muv),perms[1])
 				coeff_dict2 = {perms[0]: 1}
 				coeff_dict2 = schubmult(coeff_dict2,muv)
-				
-				for perm, val in coeff_dict2.items():		
+				for perm, val in coeff_dict2.items():					
 					w = mulperm([*perm],muvn1v)
 					if inv(w)+inv(muvn1v) == inv(perm):
 						coeff_dict[tuple(permtrim(w))] = val
 				posified = True
 				
 			if display_positive and len(perms)>2:
 				coeff_dict2 = dict(coeff_dict)
@@ -1329,15 +1484,15 @@
 						coeff_dict4 = schubmult(coeff_dict4,perm)
 						for w in coeff_dict4:
 							coeff_dict4[w] = coeff_dict2[u]*posify(coeff_dict4[w],u,perm,w,var2,var3,msg)
 						coeff_dict3 = add_perm_dict(coeff_dict4,coeff_dict3)					
 					coeff_dict2 = coeff_dict3
 				coeff_dict = coeff_dict2
 				posified = True
-			else:				
+			elif not posified:	
 				coeff_dict = check_coeff_dict
 					
 			if pr:
 				if ascode:
 					width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys()])
 				else:
 					width = max([len(str(perm)) for perm in coeff_dict.keys()])
```

### Comparing `schubmult-1.2.9/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.0/schubmult.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.2.9
+Version: 1.3.0
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.0, it also handles quantum Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
 schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6
+schubmult_q 5 1 4 3 2 - 2 1 3 5 4
 ```
 
 The same execution with the Lehmer code:
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
 schubmult_yz -code 0 1 1 2 - 1 0 2 3
+schubmult_q -code 4 0 2 1 - 1 0 0 1
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4
@@ -46,15 +48,15 @@
 
 
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Both have the same command line syntax as schubmult. schubmult_double displays the result with nonnegative coefficients in terms of the negative simple roots. Both are of course slower than schubmult_py, and expressing the result positively for schubmult_double slows it down even more.
 
-New in version 1.1.0, schubmult_py -coprod allows you to split Schubert polynomials along certain indices. It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
+New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6)) # outputs dictionary with results
```

### Comparing `schubmult-1.2.9/setup.py` & `schubmult-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.2.9",
+    version="1.3.0",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
@@ -26,10 +26,11 @@
 		"sympy>=1.12",
 		"psutil",
 		"cachetools",
 		"sortedcontainers"
     ],
     entry_points={"console_scripts": ["schubmult_py=schubmult.schubmult_py.__main__:main",
 	"schubmult_double=schubmult.schubmult_double.__main__:main",
-	"schubmult_yz=schubmult.schubmult_yz.__main__:main"
+	"schubmult_yz=schubmult.schubmult_yz.__main__:main",
+	"schubmult_q=schubmult.schubmult_q.__main__:main"
 	]},
 )
```

