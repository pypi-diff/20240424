# Comparing `tmp/RagCLI-0.1.1-py3-none-any.whl.zip` & `tmp/RagCLI-0.1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 31211 bytes, number of entries: 32
+Zip file size: 31251 bytes, number of entries: 32
 -rw-rw-rw-  2.0 fat     3140 b- defN 24-Apr-23 08:48 RagAdhocQueryDoc.py
 -rw-rw-rw-  2.0 fat     3629 b- defN 24-Apr-23 08:48 RagChromaDB.py
 -rw-rw-rw-  2.0 fat     2833 b- defN 24-Apr-23 16:45 RagChunkText.py
 -rw-rw-rw-  2.0 fat     2204 b- defN 24-Apr-23 16:38 RagEmbeddings.py
 -rw-rw-rw-  2.0 fat     3854 b- defN 24-Apr-23 16:30 RagFaiss.py
 -rw-rw-rw-  2.0 fat     1439 b- defN 24-Apr-23 08:48 RagLLM.py
 -rw-rw-rw-  2.0 fat     1653 b- defN 24-Apr-23 08:48 RagPdf2Text.py
@@ -21,14 +21,14 @@
 -rw-rw-rw-  2.0 fat     2250 b- defN 24-Apr-24 13:39 rag/ragCLChromadb.py
 -rw-rw-rw-  2.0 fat     3165 b- defN 24-Apr-24 06:38 rag/ragCLFaiss.py
 -rw-rw-rw-  2.0 fat     4046 b- defN 24-Apr-24 07:30 utils/CONST.py
 -rw-rw-rw-  2.0 fat      867 b- defN 24-Apr-23 08:40 utils/FUNCTIONS.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 16:16 utils/__init__.py
 -rw-rw-rw-  2.0 fat     1857 b- defN 24-Apr-24 07:29 utils/log.py
 -rw-rw-rw-  2.0 fat     1907 b- defN 24-Apr-22 13:53 utils/milestone.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 13:45 RagCLI-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8530 b- defN 24-Apr-24 13:45 RagCLI-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 13:45 RagCLI-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      262 b- defN 24-Apr-24 13:45 RagCLI-0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat      122 b- defN 24-Apr-24 13:45 RagCLI-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2434 b- defN 24-Apr-24 13:45 RagCLI-0.1.1.dist-info/RECORD
-32 files, 77626 bytes uncompressed, 27389 bytes compressed:  64.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 13:53 RagCLI-0.1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8544 b- defN 24-Apr-24 13:53 RagCLI-0.1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 13:53 RagCLI-0.1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      262 b- defN 24-Apr-24 13:53 RagCLI-0.1.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat      122 b- defN 24-Apr-24 13:53 RagCLI-0.1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2446 b- defN 24-Apr-24 13:53 RagCLI-0.1.1.1.dist-info/RECORD
+32 files, 77652 bytes uncompressed, 27405 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -72,26 +72,26 @@
 
 Filename: utils/log.py
 Comment: 
 
 Filename: utils/milestone.py
 Comment: 
 
-Filename: RagCLI-0.1.1.dist-info/LICENSE
+Filename: RagCLI-0.1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: RagCLI-0.1.1.dist-info/METADATA
+Filename: RagCLI-0.1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: RagCLI-0.1.1.dist-info/WHEEL
+Filename: RagCLI-0.1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: RagCLI-0.1.1.dist-info/entry_points.txt
+Filename: RagCLI-0.1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: RagCLI-0.1.1.dist-info/top_level.txt
+Filename: RagCLI-0.1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: RagCLI-0.1.1.dist-info/RECORD
+Filename: RagCLI-0.1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `RagCLI-0.1.1.dist-info/LICENSE` & `RagCLI-0.1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RagCLI-0.1.1.dist-info/METADATA` & `RagCLI-0.1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: RagCLI
-Version: 0.1.1
-Summary: This solution manages a full RAG by using FAISS, Ollama and sentence_transformers for embeddings.
+Version: 0.1.1.1
+Summary: This solution manages a full RAG by using FAISS or ChromaDB, Ollama and sentence_transformers for embeddings.
 Author-email: Benoit Cayla <benoit@datacorner.fr>
 License: MIT License
         
         Copyright (c) 2023 Benoît Cayla
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

## Comparing `RagCLI-0.1.1.dist-info/RECORD` & `RagCLI-0.1.1.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 rag/ragCLChromadb.py,sha256=XCAOsQuhB0YwX3vqljqQA2G8FiTW0yK5L0VcaLHYpmM,2250
 rag/ragCLFaiss.py,sha256=Ncn-Bv4ey8isAaiVVDQl9Mvy7vBAUqHpegGf1_pJThU,3165
 utils/CONST.py,sha256=zM0pQqcJWfY87HrFInYQC-cCcuaqqXf1QS_5OvfdKuI,4046
 utils/FUNCTIONS.py,sha256=SxsDChfQwe50h7zCMXb6TqFcrhI6Pv45H9PeAUP-s6Y,867
 utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 utils/log.py,sha256=fqHYPfnMJyU2K-VWjIFAI51fXLJwSQRf4mBjPp0NurI,1857
 utils/milestone.py,sha256=dA5T_0QVWtHv3HaAFVZkKCEdRDS2SQSJsi7g0e_glGw,1907
-RagCLI-0.1.1.dist-info/LICENSE,sha256=BvMmeujpLDerNqzsA1gOET7mphtef9ebt_u8-bp4bNA,1091
-RagCLI-0.1.1.dist-info/METADATA,sha256=bSK2f5QjaKAk8R5iw3awEzfBr1FWAqHdrBk4hCputeI,8530
-RagCLI-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-RagCLI-0.1.1.dist-info/entry_points.txt,sha256=wxkL6gKZ9HCQ4K3BzxYurJdD0OQebf3rylGUKjYIofI,262
-RagCLI-0.1.1.dist-info/top_level.txt,sha256=NaU2WdHoZlDKupGLTbUdlcyE5T1MdjeUSaalQyep8xs,122
-RagCLI-0.1.1.dist-info/RECORD,,
+RagCLI-0.1.1.1.dist-info/LICENSE,sha256=BvMmeujpLDerNqzsA1gOET7mphtef9ebt_u8-bp4bNA,1091
+RagCLI-0.1.1.1.dist-info/METADATA,sha256=OboAlTyS9bHMW4s0Qbm7xTbnFZSGk1OA6xhafRwHXeQ,8544
+RagCLI-0.1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+RagCLI-0.1.1.1.dist-info/entry_points.txt,sha256=wxkL6gKZ9HCQ4K3BzxYurJdD0OQebf3rylGUKjYIofI,262
+RagCLI-0.1.1.1.dist-info/top_level.txt,sha256=NaU2WdHoZlDKupGLTbUdlcyE5T1MdjeUSaalQyep8xs,122
+RagCLI-0.1.1.1.dist-info/RECORD,,
```

