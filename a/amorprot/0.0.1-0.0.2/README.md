# Comparing `tmp/amorprot-0.0.1-py3-none-any.whl.zip` & `tmp/amorprot-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2502 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4402 b- defN 23-Aug-14 08:52 amorprot/AmorProt.py
+Zip file size: 2505 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4422 b- defN 24-Apr-24 04:08 amorprot/AmorProt.py
 -rw-r--r--  2.0 unx       94 b- defN 23-Mar-25 15:29 amorprot/__init__.py
--rw-r--r--  2.0 unx      374 b- defN 23-Aug-14 09:00 amorprot-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-14 09:00 amorprot-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Aug-14 09:00 amorprot-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      452 b- defN 23-Aug-14 09:00 amorprot-0.0.1.dist-info/RECORD
-6 files, 5423 bytes uncompressed, 1680 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx      374 b- defN 24-Apr-24 04:22 amorprot-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 04:22 amorprot-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-24 04:22 amorprot-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      452 b- defN 24-Apr-24 04:22 amorprot-0.0.2.dist-info/RECORD
+6 files, 5443 bytes uncompressed, 1683 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: amorprot/AmorProt.py
 Comment: 
 
 Filename: amorprot/__init__.py
 Comment: 
 
-Filename: amorprot-0.0.1.dist-info/METADATA
+Filename: amorprot-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: amorprot-0.0.1.dist-info/WHEEL
+Filename: amorprot-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: amorprot-0.0.1.dist-info/top_level.txt
+Filename: amorprot-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: amorprot-0.0.1.dist-info/RECORD
+Filename: amorprot-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## amorprot/AmorProt.py

```diff
@@ -72,39 +72,39 @@
         pos = np.arange(1, len(seq)+1)/(len(seq))
         arrays = []
         
         if self.maccs:
             maccs_list = []
             for i in range(len(seq)):
                 aa = seq[i]
-                maccs_list.append(T(self.maccs_list[aa], pos[i], W=self.W, A=self.A, R=self.R))
+                maccs_list.append(self.T(self.maccs_list[aa], pos[i], W=self.W, A=self.A, R=self.R))
             maccs_array = np.array(maccs_list, dtype=np.float32)
             arrays.append(maccs_array)
         
         if self.ecfp4:
             ecfp4_list = []
             for i in range(len(seq)):
                 aa = seq[i]
-                ecfp4_list.append(T(self.ecfp4_dict[aa], pos[i], W=self.W, A=self.A, R=self.R))
+                ecfp4_list.append(self.T(self.ecfp4_dict[aa], pos[i], W=self.W, A=self.A, R=self.R))
             ecfp4_array = np.array(ecfp4_list, dtype=np.float32)
             arrays.append(ecfp4_array)
         
         if self.ecfp6:
             ecfp6_list = []
             for i in range(len(seq)):
                 aa = seq[i]
-                ecfp6_list.append(T(self.ecfp6_dict[aa], pos[i], W=self.W, A=self.A, R=self.R))
+                ecfp6_list.append(self.T(self.ecfp6_dict[aa], pos[i], W=self.W, A=self.A, R=self.R))
             ecfp6_array = np.array(ecfp6_list, dtype=np.float32)
             arrays.append(ecfp6_array)
         
         if self.rdkit:
             rdkit_list = []
             for i in range(len(seq)):
                 aa = seq[i]
-                rdkit_list.append(T(self.rdkit_dict[aa], pos[i], W=self.W, A=self.A, R=self.R))
+                rdkit_list.append(self.T(self.rdkit_dict[aa], pos[i], W=self.W, A=self.A, R=self.R))
             rdkit_array = np.array(rdkit_list, dtype=np.float32)
             arrays.append(rdkit_array)
         
         profp = np.concatenate(arrays, axis=1)
         profp = profp.sum(axis=0)
         profp = profp/profp.max()
```

