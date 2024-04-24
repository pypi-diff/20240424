# Comparing `tmp/amorprot-0.0.4.tar.gz` & `tmp/amorprot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amorprot-0.0.4.tar", last modified: Wed Apr 24 04:57:01 2024, max compression
+gzip compressed data, was "amorprot-0.0.5.tar", last modified: Wed Apr 24 05:00:21 2024, max compression
```

## Comparing `amorprot-0.0.4.tar` & `amorprot-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mhlee     (1014) users      (100)        0 2024-04-24 04:57:01.032170 amorprot-0.0.4/
--rw-r--r--   0 mhlee     (1014) users      (100)      307 2024-04-24 04:57:01.032170 amorprot-0.0.4/PKG-INFO
--rw-r--r--   0 mhlee     (1014) users      (100)      790 2023-01-21 13:41:58.000000 amorprot-0.0.4/README.md
-drwxr-xr-x   0 mhlee     (1014) users      (100)        0 2024-04-24 04:57:01.029170 amorprot-0.0.4/amorprot/
--rw-r--r--   0 mhlee     (1014) users      (100)     4420 2024-04-24 04:55:57.000000 amorprot-0.0.4/amorprot/AmorProt.py
--rw-r--r--   0 mhlee     (1014) users      (100)       94 2023-03-25 15:29:29.000000 amorprot-0.0.4/amorprot/__init__.py
-drwxr-xr-x   0 mhlee     (1014) users      (100)        0 2024-04-24 04:57:01.032170 amorprot-0.0.4/amorprot.egg-info/
--rw-r--r--   0 mhlee     (1014) users      (100)      307 2024-04-24 04:57:00.000000 amorprot-0.0.4/amorprot.egg-info/PKG-INFO
--rw-r--r--   0 mhlee     (1014) users      (100)      219 2024-04-24 04:57:00.000000 amorprot-0.0.4/amorprot.egg-info/SOURCES.txt
--rw-r--r--   0 mhlee     (1014) users      (100)        1 2024-04-24 04:57:00.000000 amorprot-0.0.4/amorprot.egg-info/dependency_links.txt
--rw-r--r--   0 mhlee     (1014) users      (100)       31 2024-04-24 04:57:00.000000 amorprot-0.0.4/amorprot.egg-info/requires.txt
--rw-r--r--   0 mhlee     (1014) users      (100)        9 2024-04-24 04:57:00.000000 amorprot-0.0.4/amorprot.egg-info/top_level.txt
--rw-r--r--   0 mhlee     (1014) users      (100)       38 2024-04-24 04:57:01.032170 amorprot-0.0.4/setup.cfg
--rw-r--r--   0 mhlee     (1014) users      (100)      549 2024-04-24 04:56:46.000000 amorprot-0.0.4/setup.py
+drwxr-xr-x   0 mhlee     (1014) users      (100)        0 2024-04-24 05:00:21.627275 amorprot-0.0.5/
+-rw-r--r--   0 mhlee     (1014) users      (100)      307 2024-04-24 05:00:21.627275 amorprot-0.0.5/PKG-INFO
+-rw-r--r--   0 mhlee     (1014) users      (100)      790 2023-01-21 13:41:58.000000 amorprot-0.0.5/README.md
+drwxr-xr-x   0 mhlee     (1014) users      (100)        0 2024-04-24 05:00:21.626275 amorprot-0.0.5/amorprot/
+-rw-r--r--   0 mhlee     (1014) users      (100)     4417 2024-04-24 04:59:47.000000 amorprot-0.0.5/amorprot/AmorProt.py
+-rw-r--r--   0 mhlee     (1014) users      (100)       94 2023-03-25 15:29:29.000000 amorprot-0.0.5/amorprot/__init__.py
+drwxr-xr-x   0 mhlee     (1014) users      (100)        0 2024-04-24 05:00:21.627275 amorprot-0.0.5/amorprot.egg-info/
+-rw-r--r--   0 mhlee     (1014) users      (100)      307 2024-04-24 05:00:21.000000 amorprot-0.0.5/amorprot.egg-info/PKG-INFO
+-rw-r--r--   0 mhlee     (1014) users      (100)      219 2024-04-24 05:00:21.000000 amorprot-0.0.5/amorprot.egg-info/SOURCES.txt
+-rw-r--r--   0 mhlee     (1014) users      (100)        1 2024-04-24 05:00:21.000000 amorprot-0.0.5/amorprot.egg-info/dependency_links.txt
+-rw-r--r--   0 mhlee     (1014) users      (100)       31 2024-04-24 05:00:21.000000 amorprot-0.0.5/amorprot.egg-info/requires.txt
+-rw-r--r--   0 mhlee     (1014) users      (100)        9 2024-04-24 05:00:21.000000 amorprot-0.0.5/amorprot.egg-info/top_level.txt
+-rw-r--r--   0 mhlee     (1014) users      (100)       38 2024-04-24 05:00:21.627275 amorprot-0.0.5/setup.cfg
+-rw-r--r--   0 mhlee     (1014) users      (100)      549 2024-04-24 05:00:14.000000 amorprot-0.0.5/setup.py
```

### Comparing `amorprot-0.0.4/README.md` & `amorprot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `amorprot-0.0.4/amorprot/AmorProt.py` & `amorprot-0.0.5/amorprot/AmorProt.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             self.rdkit_dict = {}
             for aa in self.AA_dict.keys():
                 mol = Chem.MolFromSmiles(self.AA_dict[aa])
                 self.rdkit_dict[aa] = np.array(AllChem.RDKFingerprint(mol)).tolist()
     
     # the smoothed trigonometric function 
     def T(self, fp, p, W=10, A=10, R=0.85):
-        return (((np.sin(p[i]/W))/A)+R)*np.array(fp)
+        return (((np.sin(p/W))/A)+R)*np.array(fp)
     
     def fingerprint(self, seq):
         
         pos = np.arange(1, len(seq)+1)/(len(seq))
         arrays = []
         
         if self.maccs:
```

### Comparing `amorprot-0.0.4/setup.py` & `amorprot-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(name='amorprot',
-      version="0.0.4",
+      version="0.0.5",
       url='https://github.com/mhlee216/AmorProt',
       packages=find_packages(),
       author='Myeonghun Lee',
       author_email="leemh216@gmail.com",
       description='AmorProt',
       long_description='AmorProt: Amino Acid Molecular Fingerprints Repurposing-based Protein Fingerprint',
       install_requires=["numpy >= 1.19.0", "rdkit >= 2021.09.2"],
```

