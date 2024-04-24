# Comparing `tmp/Quanthon-0.3.5.3.tar.gz` & `tmp/Quanthon-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.5.3.tar", last modified: Wed Apr 10 00:57:11 2024, max compression
+gzip compressed data, was "Quanthon-0.3.6.tar", last modified: Wed Apr 24 11:09:56 2024, max compression
```

## Comparing `Quanthon-0.3.5.3.tar` & `Quanthon-0.3.6.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:57:11.591304 Quanthon-0.3.5.3/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.5.3/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:57:11.591085 Quanthon-0.3.5.3/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:57:11.589211 Quanthon-0.3.5.3/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.5.3/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      319 2024-04-10 00:27:46.000000 Quanthon-0.3.5.3/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     6876 2024-04-10 00:56:44.000000 Quanthon-0.3.5.3/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-10 00:49:28.000000 Quanthon-0.3.5.3/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 Quanthon-0.3.5.3/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.5.3/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.5.3/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.5.3/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.5.3/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.5.3/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.5.3/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     6159 2024-04-10 00:03:37.000000 Quanthon-0.3.5.3/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:57:11.590872 Quanthon-0.3.5.3/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:57:11.000000 Quanthon-0.3.5.3/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      533 2024-04-10 00:57:11.000000 Quanthon-0.3.5.3/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-10 00:57:11.000000 Quanthon-0.3.5.3/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-10 00:57:11.000000 Quanthon-0.3.5.3/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-10 00:57:11.000000 Quanthon-0.3.5.3/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1506 2024-04-10 00:23:56.000000 Quanthon-0.3.5.3/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-10 00:57:11.591349 Quanthon-0.3.5.3/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-10 00:56:52.000000 Quanthon-0.3.5.3/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:57:11.590582 Quanthon-0.3.5.3/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.5.3/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)      331 2024-04-10 00:24:57.000000 Quanthon-0.3.5.3/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 Quanthon-0.3.5.3/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.460278 Quanthon-0.3.6/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.6/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2519 2024-04-24 11:09:56.460089 Quanthon-0.3.6/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.457578 Quanthon-0.3.6/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.6/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-22 07:48:46.000000 Quanthon-0.3.6/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6876 2024-04-10 00:56:44.000000 Quanthon-0.3.6/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-10 00:49:28.000000 Quanthon-0.3.6/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 Quanthon-0.3.6/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.6/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4796 2024-04-24 11:09:30.000000 Quanthon-0.3.6/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6714 2024-04-24 11:09:39.000000 Quanthon-0.3.6/Quanthon/mappers_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 Quanthon-0.3.6/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.6/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.6/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.6/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6569 2024-04-18 11:08:36.000000 Quanthon-0.3.6/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.459907 Quanthon-0.3.6/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2519 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      581 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 Quanthon-0.3.6/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-24 11:09:56.460316 Quanthon-0.3.6/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-04-22 07:50:01.000000 Quanthon-0.3.6/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.459439 Quanthon-0.3.6/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.6/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)      626 2024-04-18 11:24:53.000000 Quanthon-0.3.6/tests/test_mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 Quanthon-0.3.6/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 Quanthon-0.3.6/tests/test_vqes.py
```

### Comparing `Quanthon-0.3.5.3/PKG-INFO` & `Quanthon-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.5.3
+Version: 0.3.6
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -97,11 +97,19 @@
 ```python
 # Perform a CNOT operation between the first and second qubit
 two_qubits.CONT(0, 1)
 
 two_qubits.SWAP(0, 1)
 ```
 
+## New in 0.3.6:
+Added pauli_decomposition for matrices of size $2^n \times 2^n$.
 
-## NEW IN VERSION 0.3.5:
-- VQE now supports non-Hermitian 'Hamiltonian's, but why would you ever need it?
+```py
+from Quanthon import pauli_decomposition
+```
+
+## Previous Version Releases
+
+### 0.3.5:
+- VQE now supports non-Hermitian 'Hamiltonians', but why would you ever need it?
```

### Comparing `Quanthon-0.3.5.3/Quanthon/Models.py` & `Quanthon-0.3.6/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/algorithms.py` & `Quanthon-0.3.6/Quanthon/algorithms.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/ansatzs.py` & `Quanthon-0.3.6/Quanthon/ansatzs.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/base.py` & `Quanthon-0.3.6/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/expectation.py` & `Quanthon-0.3.6/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/mappers.py` & `Quanthon-0.3.6/Quanthon/mappers_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -177,146 +177,25 @@
         new_op = ''.join(new_op)
         all_tb_op.append((new_op, factor * coeff))
         # print(new_op, coeff)
 
     return all_tb_op 
 
 
-
-def jordan_wigner(hamiltonian):
-    
-    '''
-    Perform the Jordan-Wigner transform for which maps second quantisation Hamiltonian to qubit Hamiltonians.
-    N.B. 0th qubit to the left, always.
-    arg:
-        hamiltonian: Hamiltonian, the second quantisation Hamiltonian containing the overlap integrals.
-    
-    return:
-        h_pauli: list of tuples, the qubit Hamiltonian in terms of Pauli strings.'''
-    h_pauli = []
-    n = hamiltonian.one_body_coeffs.shape[0]
-
-    # one body
-    for i in range(n):
-        for j in range(n):
-
-            if np.allclose(hamiltonian.one_body_coeffs[i, j],0):
-                continue
-
-            # diagnol terms
-            if i == j:
-                # II...III - I...IZ...I
-
-                all_i = n * 'I'
-                h_pauli.append((all_i, 0.5 * hamiltonian.one_body_coeffs[i, j]))
-
-                z_term = list(all_i)
-                # z_term[n-i-1] = 'Z'
-                z_term[i] = 'Z'
-                z_term = ''.join(z_term)
-
-                h_pauli.append((z_term, -0.5 * hamiltonian.one_body_coeffs[i, j]))
-
-            else:
-                ob_op = get_ob_op(n, i, j, hamiltonian.one_body_coeffs[i, j])
-                h_pauli.extend(ob_op)
-     
-                
-    # two body
-                
-    # print("unhealthy terms after one body", _check_health_jw(h_pauli, n))
-    # return h_pauli
-
-    for p in range(n):
-        for q in range(n):
-            if p == q:
-                continue
-            for r in range(n):
-                for s in range(n):
-                    if r == s:
-                        continue
-
-
-                    coeff = hamiltonian.two_body_coeffs[p, q, r, s]
-
-                    if np.allclose(coeff,0):
-                        continue
-                    
-                    # print(f'pqrs: {p}{q}{r}{s}, coeff: {coeff}')
-
-                    
-                    # if the outer indices are not all greater than the inner indices
-                    if (p > q and r > s) or (p < q and r < s):
-                        coeff *= -1
-                        # print(coeff)
-
-                    if (p == r and q == s) or (p == s and q == r):
-
-                        # print(p, q, r, s)
-                        all_i = n*'I'
-
-                        pz = list(n*'I')
-                        pz[p] = 'Z'
-                        pz = ''.join(pz)
-
-                        qz = list(n*'I')
-                        qz[q] = 'Z'
-                        qz = ''.join(qz)
-
-                        qpz = list(n*'I')
-                        qpz[p] = 'Z'
-                        qpz[q] = 'Z'
-                        qpz = ''.join(qpz)
-
-                        # print(p, q, r, s, coeff)
-                        # print(all_i, pz, qz, qpz)
-                        # print()
-                        # print("all_i", all_i)
-                        # print("pz", pz)
-                        # print("qz", qz)
-                        # print("qpz", qpz)
-
-                        h_pauli.append((all_i, 0.25 * coeff))
-                        h_pauli.append((pz, -0.25 * coeff))
-                        h_pauli.append((qz, -0.25 * coeff))
-                        h_pauli.append((qpz, 0.25 * coeff))
-
-                        
-                    elif len({p, q, r, s}) == 4:
-                        # if they are all different
-
-                        tb_op = get_tb_4u(n, p, q, r, s, coeff)
-                        h_pauli.extend(tb_op)
-
-                    elif len({p, q, r, s}) == 3:
-                        # 0223
-                        tb_op = get_tb_3u(n, p, q, r, s, coeff)
-                        h_pauli.extend(tb_op)
-
-
-    if _check_health_jw(h_pauli, n):
-        raise ValueError("There are terms whose length is not equal to the number of qubits.")
-    
-    h_pauli = _simplify_pauli_terms(h_pauli)
-    return h_pauli
-
-
-
-def _check_health_jw(h_pauli, n):
+def check_health_jw(h_pauli, n):
     count = 0
     for term in h_pauli:
         if len(term[0]) != n:
             print(term)
             count += 1
     
     return count
     
 
-
-def _simplify_pauli_terms(terms):
+def simplify_pauli_terms(terms):
 
     '''
         Simplify the pauli sums by collecting like terms.
         
         
         return: list, pauli sum equal to the input with like terms collected and sorted.
     
@@ -330,7 +209,37 @@
             simplified_terms[pauli_string] = coeff
     
     simplified_terms_list = [(pauli_string, coeff) for pauli_string, coeff in simplified_terms.items() if coeff != 0]
     
     # will sort alphabetically
     return sorted(simplified_terms_list)
 
+
+def is_power_of_two(n):
+    return n > 0 and (2 ** (n.bit_length() - 1)) == n
+
+
+def expand_h_mat(h_mat):
+
+    '''For matrices that are not a power of 2, expand the matrix to the nearest power of 2.
+    
+    args:
+        h_mat: 2d numpy array, the matrix to be expanded.
+
+    return:
+        new_h_mat: 2d numpy array, the expanded matrix to size of smallest power of 2 possible. 
+        The original matrix is at the top left corner.
+    '''
+
+    n = h_mat.shape[0]
+    pow = 1
+    while True:
+        if n <= 2 ** pow:
+           break 
+        pow += 1
+    
+    new_h_mat = np.zeros((2 ** pow, 2 ** pow))
+    new_h_mat[:n, :n] = h_mat
+
+    return new_h_mat
+        
+
```

### Comparing `Quanthon-0.3.5.3/Quanthon/ut_pyscf_mel.py` & `Quanthon-0.3.6/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/ut_qiskit_hamiltonian.py` & `Quanthon-0.3.6/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/ut_test_jw.py` & `Quanthon-0.3.6/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/Quanthon/utils.py` & `Quanthon-0.3.6/Quanthon/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Utils
 import numpy as np
-
+from itertools import product
 def get_pauli(basis_name):
     pauli_matrices = {'I': np.eye(2, dtype=np.complex128), 
                       'X': np.array([[0, 1], [1, 0]], dtype=np.complex128), 
                       'Y': np.array([[0, -1j], [1j, 0]]), 
                       'Z': np.array([[1, 0], [0, -1]],dtype=np.complex128)}
 
     # Check if basis_name is a valid combination
@@ -127,14 +127,30 @@
     if (val >> i) & 1 != (val >> j) & 1:
         mask = (1 << i) | (1 << j)
         val ^= mask
 
     return val
 
 
+def get_all_paulis(n):
+    '''
+    args: 
+        n: the number of qubits.
+    
+    return: list of all the possible Pauli strings of length n.
+    '''
+    paulis = 'IXYZ'
+    return [''.join(p) for p in product(paulis, repeat=n)] 
+
+
+def is_hermitian(mat):
+    return np.allclose(mat, mat.T.conj())
+
+def is_unitary(mat):
+    return np.allclose(mat @ mat.T.conj(), np.eye(len(mat)))
 
     
 if __name__ == "__main__":
     # Test Pauli operators
     # pauli_ops = [('IZZZ', 3), ('ZXYI', 2)]
     qubit_op = [('IIIIII', 0.1875), ('IIIIIZ', -0.5625), 
                     ('IIIIZI', -0.0625), ('IIIZII', 0.4375), 
@@ -178,8 +194,7 @@
         i = int(i, 2)
         flipped_i = flip_bit(int(i), c) 
         print(f'{flipped_i:0{n}b}')
         if f'{flipped_i:0{n}b}'[-(c+1)] != '0':
             raise Exception('WRONG')
 
 
-
```

### Comparing `Quanthon-0.3.5.3/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.6/Quanthon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.5.3
+Version: 0.3.6
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -97,11 +97,19 @@
 ```python
 # Perform a CNOT operation between the first and second qubit
 two_qubits.CONT(0, 1)
 
 two_qubits.SWAP(0, 1)
 ```
 
+## New in 0.3.6:
+Added pauli_decomposition for matrices of size $2^n \times 2^n$.
 
-## NEW IN VERSION 0.3.5:
-- VQE now supports non-Hermitian 'Hamiltonian's, but why would you ever need it?
+```py
+from Quanthon import pauli_decomposition
+```
+
+## Previous Version Releases
+
+### 0.3.5:
+- VQE now supports non-Hermitian 'Hamiltonians', but why would you ever need it?
```

### Comparing `Quanthon-0.3.5.3/setup.py` & `Quanthon-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.5.3" #####
+version = "0.3.6" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.5.3/tests/test_cmp_qk.py` & `Quanthon-0.3.6/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.3/tests/test_vqes.py` & `Quanthon-0.3.6/tests/test_vqes.py`

 * *Files identical despite different names*

