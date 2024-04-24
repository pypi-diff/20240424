# Comparing `tmp/schubmult-1.3.4.tar.gz` & `tmp/schubmult-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.4.tar", last modified: Mon Apr 15 14:05:56 2024, max compression
+gzip compressed data, was "schubmult-1.3.5.tar", last modified: Wed Apr 24 11:35:51 2024, max compression
```

## Comparing `schubmult-1.3.4.tar` & `schubmult-1.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:56.285000 schubmult-1.3.4/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-15 14:05:56.236000 schubmult-1.3.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4853 2024-04-15 14:05:16.000000 schubmult-1.3.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:54.059000 schubmult-1.3.4/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.4/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16003 2024-04-12 18:48:00.000000 schubmult-1.3.4/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:54.734000 schubmult-1.3.4/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.4/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.4/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.4/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.025000 schubmult-1.3.4/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.4/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.4/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.4/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.307000 schubmult-1.3.4/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.4/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.4/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     9008 2024-04-08 20:08:59.000000 schubmult-1.3.4/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.590000 schubmult-1.3.4/schubmult/schubmult_q_double/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.4/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.4/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.4/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.879000 schubmult-1.3.4/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.4/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.4/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5854 2024-04-15 13:59:54.000000 schubmult-1.3.4/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:56.171000 schubmult-1.3.4/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.4/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.4/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.4/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:54.472000 schubmult-1.3.4/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      978 2024-04-15 14:05:53.000000 schubmult-1.3.4/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      353 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-15 14:05:56.272000 schubmult-1.3.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1243 2024-04-15 14:05:23.000000 schubmult-1.3.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:51.663000 schubmult-1.3.5/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-24 11:35:51.611000 schubmult-1.3.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4853 2024-04-15 14:05:16.000000 schubmult-1.3.5/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:48.869000 schubmult-1.3.5/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.5/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16003 2024-04-12 18:48:00.000000 schubmult-1.3.5/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:49.723000 schubmult-1.3.5/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.5/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.5/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.5/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:50.094000 schubmult-1.3.5/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.5/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.5/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.5/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:50.444000 schubmult-1.3.5/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.5/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.5/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9067 2024-04-21 14:28:57.000000 schubmult-1.3.5/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:50.790000 schubmult-1.3.5/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.5/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.5/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.5/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:51.160000 schubmult-1.3.5/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.5/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.5/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5863 2024-04-21 14:35:53.000000 schubmult-1.3.5/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:51.536000 schubmult-1.3.5/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.5/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.5/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.5/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:49.362000 schubmult-1.3.5/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-04-24 11:35:48.000000 schubmult-1.3.5/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-24 11:35:51.645000 schubmult-1.3.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-04-24 11:35:16.000000 schubmult-1.3.5/setup.py
```

### Comparing `schubmult-1.3.4/LICENSE` & `schubmult-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/PKG-INFO` & `schubmult-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.4
+Version: 1.3.5
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.4/README.md` & `schubmult-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/schubmult/perm_lib.py` & `schubmult-1.3.5/schubmult/perm_lib.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.5/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.5/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.5/schubmult/schubmult_q/schubmult_q.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 			mx_th = 0
 			for vp in vpathdicts[index]:
 				for v2,vdiff,s in vpathdicts[index][vp]:
 					if th[index]-vdiff > mx_th:
 						mx_th = th[index] - vdiff					
 			newpathsums = {}
 			for up in vpathsums:
-				newperms = elem_sym_perms_q(up,mx_th,th[index])
+				inv_up = inv(up)
+				newperms = elem_sym_perms_q(up,min(mx_th,(inv_mu-(inv_up-inv_u))-inv_vmu),th[index])
 				for up2, udiff, mul_val in newperms:
 					if up2 not in newpathsums:
 						newpathsums[up2]={}
 					for v in vpathdicts[index]:
 						sumval = vpathsums[up].get(v,zero)
 						if sumval == 0:
 							continue
```

### Comparing `schubmult-1.3.4/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.3.5/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.3.5/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 	
 
 	
 
 	
 def schubmult(perm_dict,v,var2=var2,var3=var3):
-	vn1 = inverse(v)
 	th = [len(v)-i for i in range(1,len(v))]
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
@@ -35,15 +34,15 @@
 			for vp in vpathdicts[index]:
 				for v2,vdiff,s in vpathdicts[index][vp]:
 					if th[index]-vdiff > mx_th:
 						mx_th = th[index] - vdiff					
 			newpathsums = {}
 			for up in vpathsums:
 				inv_up = inv(up)
-				newperms = elem_sym_perms_q(up,mx_th,th[index])
+				newperms = elem_sym_perms_q(up,min(mx_th,(inv_mu-(inv_up-inv_u))-inv_vmu),th[index])
 				for up2, udiff,mul_val in newperms:
 					if up2 not in newpathsums:
 						newpathsums[up2]={}
 					for v in vpathdicts[index]:
 						sumval = vpathsums[up].get(v,zero)*mul_val
 						if sumval == 0:
 							continue
@@ -89,14 +88,15 @@
 			if key in q_var2:
 				q_part *= key
 			else:
 				yz_part*=key
 			
 		ret[q_part] = ret.get(q_part,0) + yz_part
 	return ret
+	
 def main():
 	global var2
 	try:
 		sys.setrecursionlimit(1000000)
 	
 		perms=[]
 		curperm = []
@@ -166,16 +166,16 @@
 			else:
 				width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			
 			coeff_perms = list(coeff_dict.keys())
 			coeff_perms.sort(key=lambda x: (inv(x),*x))
 			
 			for perm in coeff_perms:
-				val = sympify(coeff_dict[perm]).simplify()
-				if val != 0:
+				val = coeff_dict[perm]
+				if expand(val) != 0:
 					notint = False
 					try:
 						int(val)
 					except Exception:
 						notint = True
 						val2 = 0
 						if display_positive:
```

### Comparing `schubmult-1.3.4/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.5/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.5/schubmult.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.4
+Version: 1.3.5
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.4/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.5/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.4/setup.py` & `schubmult-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.4",
+    version="1.3.5",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

