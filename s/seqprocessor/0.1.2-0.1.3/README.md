# Comparing `tmp/seqprocessor-0.1.2.tar.gz` & `tmp/seqprocessor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqprocessor-0.1.2.tar", max compression
+gzip compressed data, was "seqprocessor-0.1.3.tar", max compression
```

## Comparing `seqprocessor-0.1.2.tar` & `seqprocessor-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rwxr-xr-x   0        0        0       26 2024-04-15 06:48:57.446696 seqprocessor-0.1.2/README.md
--rwxr-xr-x   0        0        0      519 2024-04-19 08:53:53.103154 seqprocessor-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-04-15 06:48:18.998387 seqprocessor-0.1.2/seqprocessor/__init__.py
--rwxr-xr-x   0        0        0      326 2024-04-15 08:59:31.839970 seqprocessor-0.1.2/seqprocessor/main.py
--rwxr-xr-x   0        0        0      118 2024-04-15 06:48:18.999386 seqprocessor-0.1.2/seqprocessor/options.py
--rwxr-xr-x   0        0        0        0 2024-04-15 06:48:19.000405 seqprocessor-0.1.2/seqprocessor/seq/__init__.py
--rwxr-xr-x   0        0        0     3098 2024-04-19 08:52:07.442757 seqprocessor-0.1.2/seqprocessor/seq/info.py
--rwxr-xr-x   0        0        0     7755 2024-04-19 05:18:20.464621 seqprocessor-0.1.2/seqprocessor/seq/pretreat.py
--rwxr-xr-x   0        0        0     1316 2024-04-15 11:30:12.162660 seqprocessor-0.1.2/seqprocessor/utils.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 seqprocessor-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2024-04-15 06:48:57.446696 seqprocessor-0.1.3/README.md
+-rwxr-xr-x   0        0        0      558 2024-04-23 08:24:17.798573 seqprocessor-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-04-15 06:48:18.998387 seqprocessor-0.1.3/seqprocessor/__init__.py
+-rwxr-xr-x   0        0        0      876 2024-04-23 07:01:19.617116 seqprocessor-0.1.3/seqprocessor/main.py
+-rwxr-xr-x   0        0        0     7780 2024-04-23 08:20:27.288637 seqprocessor-0.1.3/seqprocessor/mutation/mutation.py
+-rwxr-xr-x   0        0        0      118 2024-04-15 06:48:18.999386 seqprocessor-0.1.3/seqprocessor/options.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 06:48:19.000405 seqprocessor-0.1.3/seqprocessor/seq/__init__.py
+-rwxr-xr-x   0        0        0     2224 2024-04-23 03:31:01.215902 seqprocessor-0.1.3/seqprocessor/seq/align.py
+-rwxr-xr-x   0        0        0     3148 2024-04-23 03:29:33.163762 seqprocessor-0.1.3/seqprocessor/seq/info.py
+-rwxr-xr-x   0        0        0     2097 2024-04-23 03:29:46.414749 seqprocessor-0.1.3/seqprocessor/seq/phylo.py
+-rwxr-xr-x   0        0        0     8850 2024-04-23 03:30:40.022099 seqprocessor-0.1.3/seqprocessor/seq/pretreat.py
+-rwxr-xr-x   0        0        0      937 2024-04-23 06:17:18.723606 seqprocessor-0.1.3/seqprocessor/seq/translate.py
+-rwxr-xr-x   0        0        0     3000 2024-04-23 06:01:40.600670 seqprocessor-0.1.3/seqprocessor/utils.py
+-rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 seqprocessor-0.1.3/PKG-INFO
```

### Comparing `seqprocessor-0.1.2/pyproject.toml` & `seqprocessor-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqprocessor"
-version = "0.1.2"
+version = "0.1.3"
 description = "A sequence tool"
 authors = ["Ruichen Wang <wangruichen100@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 seqprocessor = "seqprocessor.main:app"
 
@@ -12,12 +12,13 @@
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.12.3"}
 pandas = "^2.2.2"
 xlrd = "^2.0.1"
 biopython = "^1.83"
 openpyxl = "^3.1.2"
 requests = "^2.31.0"
-
+matplotlib = "^3.7.2"
+tqdm = "^4.65.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seqprocessor-0.1.2/seqprocessor/seq/info.py` & `seqprocessor-0.1.3/seqprocessor/seq/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,8 +70,11 @@
             df.to_csv(out_path, index=False)
         elif out_format == OutputFormat.table:
             df.to_csv(out_path, sep="\t", index=False)
         elif out_format == OutputFormat.excel:
             df.to_excel(out_path, index=False)
     except Exception as e:
         typer.echo(f"Error writing output file: {e}")
-        raise typer.Abort()
+        raise typer.Abort()
+    
+if __name__ == "__main__":
+    info_app()
```

### Comparing `seqprocessor-0.1.2/seqprocessor/seq/pretreat.py` & `seqprocessor-0.1.3/seqprocessor/seq/pretreat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typer
 import pandas as pd
 
 from Bio import SeqIO
 from enum import Enum
+from collections import Counter
 
 from seqprocessor.utils import fasta_read, fasta_read2
 from seqprocessor.options import OutputFormat
 
 
 pretreat_app = typer.Typer(help="Sequence pretreatment")
 
@@ -197,8 +198,30 @@
     name_dict = dict(zip(old_name,new_name))
 
     with open(out_path, 'w') as outfile:
         for name, sequence in zip(names, sequences):
             name_ = name_dict[name]
             outfile.write(f'>{name_}\n{sequence}\n')
 
-            
+# Filtering low-quality sequences.
+@pretreat_app.command(name="quality_control", 
+                      help="Filtering low-quality sequences.")
+def quality_control(
+    file_path: str = typer.Option(..., "--input", "-i", help="Path to the input FASTA file."),
+    out_path: str = typer.Option(..., "--out", "-o", help="Path to the output file."),
+    qc_percentage: float = typer.Option(..., "--qc", "-q", help="Qc percentage, 0.0 to 1.0."),
+):
+
+    names, sequences = fasta_read2(file_path)
+
+    with open(out_path, 'w') as outfile:
+        for name, sequence in zip(names, sequences):
+            sequence = sequence.upper()
+            seq_length = len(sequence)
+            seq_count = Counter(sequence)
+            atcg_count = seq_count["A"]+seq_count["T"]+seq_count["C"]+seq_count["G"]
+            # Checking if percentage of A, T, C, and G bases is greater than or equal to qc_percentage
+            if atcg_count/seq_length >= qc_percentage:
+                outfile.write(f'>{name}\n{sequence}\n')
+
+if __name__ == "__main__":
+    pretreat_app()
```

### Comparing `seqprocessor-0.1.2/PKG-INFO` & `seqprocessor-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: seqprocessor
-Version: 0.1.2
+Version: 0.1.3
 Summary: A sequence tool
 Author: Ruichen Wang
 Author-email: wangruichen100@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: biopython (>=1.83,<2.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # SeqProcessor
 20240415
```

