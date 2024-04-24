# Comparing `tmp/seqprocessor-0.1.3.tar.gz` & `tmp/seqprocessor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqprocessor-0.1.3.tar", max compression
+gzip compressed data, was "seqprocessor-0.1.4.tar", max compression
```

## Comparing `seqprocessor-0.1.3.tar` & `seqprocessor-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0       26 2024-04-15 06:48:57.446696 seqprocessor-0.1.3/README.md
--rwxr-xr-x   0        0        0      558 2024-04-23 08:24:17.798573 seqprocessor-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-04-15 06:48:18.998387 seqprocessor-0.1.3/seqprocessor/__init__.py
--rwxr-xr-x   0        0        0      876 2024-04-23 07:01:19.617116 seqprocessor-0.1.3/seqprocessor/main.py
--rwxr-xr-x   0        0        0     7780 2024-04-23 08:20:27.288637 seqprocessor-0.1.3/seqprocessor/mutation/mutation.py
--rwxr-xr-x   0        0        0      118 2024-04-15 06:48:18.999386 seqprocessor-0.1.3/seqprocessor/options.py
--rwxr-xr-x   0        0        0        0 2024-04-15 06:48:19.000405 seqprocessor-0.1.3/seqprocessor/seq/__init__.py
--rwxr-xr-x   0        0        0     2224 2024-04-23 03:31:01.215902 seqprocessor-0.1.3/seqprocessor/seq/align.py
--rwxr-xr-x   0        0        0     3148 2024-04-23 03:29:33.163762 seqprocessor-0.1.3/seqprocessor/seq/info.py
--rwxr-xr-x   0        0        0     2097 2024-04-23 03:29:46.414749 seqprocessor-0.1.3/seqprocessor/seq/phylo.py
--rwxr-xr-x   0        0        0     8850 2024-04-23 03:30:40.022099 seqprocessor-0.1.3/seqprocessor/seq/pretreat.py
--rwxr-xr-x   0        0        0      937 2024-04-23 06:17:18.723606 seqprocessor-0.1.3/seqprocessor/seq/translate.py
--rwxr-xr-x   0        0        0     3000 2024-04-23 06:01:40.600670 seqprocessor-0.1.3/seqprocessor/utils.py
--rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 seqprocessor-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2024-04-15 06:48:57.446696 seqprocessor-0.1.4/README.md
+-rwxr-xr-x   0        0        0      558 2024-04-24 05:59:20.637950 seqprocessor-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-04-15 06:48:18.998387 seqprocessor-0.1.4/seqprocessor/__init__.py
+-rwxr-xr-x   0        0        0      876 2024-04-23 07:01:19.617116 seqprocessor-0.1.4/seqprocessor/main.py
+-rwxr-xr-x   0        0        0    10036 2024-04-24 05:56:47.509595 seqprocessor-0.1.4/seqprocessor/mutation/mutation.py
+-rwxr-xr-x   0        0        0      118 2024-04-15 06:48:18.999386 seqprocessor-0.1.4/seqprocessor/options.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 06:48:19.000405 seqprocessor-0.1.4/seqprocessor/seq/__init__.py
+-rwxr-xr-x   0        0        0     2224 2024-04-23 03:31:01.215902 seqprocessor-0.1.4/seqprocessor/seq/align.py
+-rwxr-xr-x   0        0        0     3148 2024-04-23 03:29:33.163762 seqprocessor-0.1.4/seqprocessor/seq/info.py
+-rwxr-xr-x   0        0        0     2097 2024-04-23 03:29:46.414749 seqprocessor-0.1.4/seqprocessor/seq/phylo.py
+-rwxr-xr-x   0        0        0     8850 2024-04-23 03:30:40.022099 seqprocessor-0.1.4/seqprocessor/seq/pretreat.py
+-rwxr-xr-x   0        0        0      937 2024-04-23 06:17:18.723606 seqprocessor-0.1.4/seqprocessor/seq/translate.py
+-rwxr-xr-x   0        0        0     3767 2024-04-24 05:55:00.487419 seqprocessor-0.1.4/seqprocessor/utils.py
+-rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 seqprocessor-0.1.4/PKG-INFO
```

### Comparing `seqprocessor-0.1.3/seqprocessor/main.py` & `seqprocessor-0.1.4/seqprocessor/main.py`

 * *Files identical despite different names*

### Comparing `seqprocessor-0.1.3/seqprocessor/mutation/mutation.py` & `seqprocessor-0.1.4/seqprocessor/mutation/mutation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typer
 
 from Bio import SeqIO
 from collections import Counter
 from matplotlib.backends.backend_pdf import PdfPages
 import matplotlib.pyplot as plt
 import pandas as pd
+import numpy as np
 import os
-from tqdm import tqdm
 
-from seqprocessor.utils import fasta_read, fasta_read2
+from seqprocessor.utils import fasta_read, fasta_read2, tab21_black
 from seqprocessor.options import OutputFormat
 
 mutation_app = typer.Typer(help="Mutation analysis")
 
 @mutation_app.command(name="pair_mutation", help="Compare pair mutations by ref sequence.")
 def pair_mutation(
     file_path: str = typer.Option(..., "--input", "-i", help="A FASTA file"),
@@ -64,120 +64,199 @@
     differences = []
     for i, (letter1, letter2) in enumerate(zip(ref_seq, seq)):
         if letter1 != letter2:
             differences.append([i+1, letter1, letter2, name])
     return differences
 
 
-
 @mutation_app.command(name="group_aamutation", help="Compare amino acid mutations in different classifications.")
 def group_aamutation(
     file_path: str = typer.Option(..., "--input", "-i", help="A FASTA file"),
     info_path: str = typer.Option(..., "--info", "-info", help="Information file path"),
     out_path: str = typer.Option(..., "--out", "-o", help="Output file path"),
     id_column: str = typer.Option("id", "--id", "-id", help="ID column"),
     type_column: str = typer.Option("type", "--type", "-type", help="Classification column"),
     picture_type: str = typer.Option("bar", "--ptype", "-pt", help="Picture format"),
 ):
     seq_record = fasta_read(file_path)
     df = pd.read_excel(info_path)
+    seq_type = sorted(set(df[type_column].to_list()))
+    os.makedirs(f"./{out_path}/{type_column}", exist_ok=True)
 
-    os.makedirs(f"{out_path}/{type_column}", exist_ok=True)
-
-    for _, group_df in df.groupby(type_column):
-        group_name = group_df.iloc[0][type_column]
-        group_fasta_path = f"{out_path}/{type_column}/{group_name}.fas"
+    for seq_type_ in seq_type:
+        df_type = df[df[type_column]==seq_type_]
+        # print(seq_type_)
+        with open(f"./{out_path}/{type_column}/{seq_type_}.fas", "w") as f:
+            for name_ in df_type[id_column].to_list():          
+                f.write(f">{name_}\n{seq_record[name_]}\n")
+
+    pdf = f"{out_path}/{type_column}/{type_column}.pdf"
+    file_path = f"{out_path}/{type_column}"
+    file_name = seq_type
+
+    site_all = []
+    aa_all = []
+    stat_df_all = []
+    freq_df_all = []
+    group_all = []
+
+    for name_ in file_name:
+        print(name_)
+        site, aa, stat_df, freq_df, group_ = aatj("{0}/{1}.fas".format(file_path, name_), name_)
+
+        site_all += site
+        aa_all += aa
+        stat_df_all += stat_df
+        freq_df_all += freq_df
+        group_all += group_
+
+    df = pd.DataFrame()
+    df["site"] = site_all
+    df["aa"] = aa_all
+    df["stat"] = stat_df_all
+    df["freq"] = freq_df_all
+    df["group"] = group_all
+    df = df.fillna(0)
+    df.to_csv(f"{out_path}/{type_column}/{type_column}.csv",index = False)
+
+    with PdfPages(pdf) as pdf:
+        for i_ in range(df["site"].min(), df["site"].max() + 1):
+            print(i_ + 1)
+            df_site = df[df["site"] == i_]
 
-        with open(group_fasta_path, "w") as f:
-            for seq_id in group_df[id_column]:
-                f.write(f">{seq_id}\n{seq_record[seq_id]}\n")
+            pivot_df = df_site.pivot(index='group', columns='aa', values='freq')
+            if picture_type == "bar":
+                pivot_df.plot(kind='bar', stacked=True, colormap=tab21_black(), yticks=[0.5, 1])
+            elif picture_type == "line":
+                pivot_df.plot(kind='line', colormap=tab21_black(), yticks=[0.5, 1])
+            plt.ylim((0, 1.1))
+            plt.legend(prop={'size': 8}, bbox_to_anchor=(1.12, 1),loc='upper right', fontsize=5)
+            plt.title('Site' + str(i_+1))
+            plt.xlabel(None)
+            # plt.show()
+            pdf.savefig()
+            plt.clf()
+            plt.close('all')
 
-        create_plots_aa(group_fasta_path, group_name, out_path, picture_type)
+def aatj(input_fasta, group):
+    site = []
+    aa = []
+    stat_df = []
+    freq_df = []
 
-def create_plots_aa(input_fasta, group_name, out_path, picture_type):
-    pdf_path = f"{out_path}/{group_name}.pdf"
+    seq_data = [list(i.seq) for i in SeqIO.parse(input_fasta, "fasta")]
+    df = pd.DataFrame(seq_data)
 
-    if os.path.exists(pdf_path):
-        os.remove(pdf_path)
+    for column in df.columns:
+        aa_ = ['G', 'A', 'V', 'L', 'I', 'F', 'W', 'Y', 'D', 'N', 'E', 'K', 'Q', 'M', 'S', 'T', 'C', 'P', 'H', 'R', "-"]
+        aa += aa_
+        site += [column] * len(aa_)
 
-    seq_data = [list(seq.seq) for seq in SeqIO.parse(input_fasta, "fasta")]
-    df = pd.DataFrame(seq_data)
+        stat = Counter(df[column])
+        aa_dict = {aa: stat.get(aa, 0) for aa in aa_}
+        stat_df.extend(aa_dict.values())
 
-    freq_df = []
-    for col in df.columns:
-        stat = Counter(df[col])
-        freq = [stat.get(aa, 0) / len(df) for aa in 'GAVLIFWYDNKEQMSTCPHR']
-        freq_df.append(freq)
+        freq = np.array(list(aa_dict.values())) / sum(aa_dict.values())
+        freq_df.extend(freq)
 
-    freq_df = pd.DataFrame(freq_df, columns=list('GAVLIFWYDNKEQMSTCPHR'))
+    group_ = [group] * len(site)
 
-    with PdfPages(pdf_path) as pdf:
-        for i, row in tqdm(freq_df.iterrows(), desc="Plotting"):
-            if picture_type == "bar":
-                row.plot(kind='bar', stacked=True, colormap='tab20', yticks=[0.5, 1])
-            elif picture_type == "line":
-                row.plot(kind='line', colormap='tab20', yticks=[0.5, 1])
+    return site, aa, stat_df, freq_df, group_
 
-            plt.ylim((0, 1.1))
-            plt.legend(prop={'size': 8}, bbox_to_anchor=(1.12, 1), loc='upper right', fontsize=5)
-            plt.title(f'Site {i + 1}')
-            plt.xlabel(None)
-            pdf.savefig()
-            plt.clf()
 
-@mutation_app.command(name="group_ntmutation", help="Compare nucleotide mutations in different classifications.")
-def group_ntmutation(
+@mutation_app.command(name="group_ntmutation", help="Compare amino acid mutations in different classifications.")
+def group_aamutation(
     file_path: str = typer.Option(..., "--input", "-i", help="A FASTA file"),
     info_path: str = typer.Option(..., "--info", "-info", help="Information file path"),
     out_path: str = typer.Option(..., "--out", "-o", help="Output file path"),
     id_column: str = typer.Option("id", "--id", "-id", help="ID column"),
     type_column: str = typer.Option("type", "--type", "-type", help="Classification column"),
     picture_type: str = typer.Option("bar", "--ptype", "-pt", help="Picture format"),
 ):
     seq_record = fasta_read(file_path)
     df = pd.read_excel(info_path)
+    seq_type = sorted(set(df[type_column].to_list()))
+    os.makedirs(f"./{out_path}/{type_column}", exist_ok=True)
 
-    os.makedirs(f"{out_path}/{type_column}", exist_ok=True)
-
-    for _, group_df in df.groupby(type_column):
-        group_name = group_df.iloc[0][type_column]
-        group_fasta_path = f"{out_path}/{type_column}/{group_name}.fas"
+    for seq_type_ in seq_type:
+        df_type = df[df[type_column]==seq_type_]
+        # print(seq_type_)
+        with open(f"./{out_path}/{type_column}/{seq_type_}.fas", "w") as f:
+            for name_ in df_type[id_column].to_list():          
+                f.write(f">{name_}\n{seq_record[name_].upper()}\n")
+
+    pdf = f"{out_path}/{type_column}/{type_column}.pdf"
+    file_path = f"{out_path}/{type_column}"
+    file_name = seq_type
+
+    site_all = []
+    nt_all = []
+    stat_df_all = []
+    freq_df_all = []
+    group_all = []
+
+    for name_ in file_name:
+        print(name_)
+        site, nt, stat_df, freq_df, group_ = nttj("{0}/{1}.fas".format(file_path, name_), name_)
+
+        site_all += site
+        nt_all += nt
+        stat_df_all += stat_df
+        freq_df_all += freq_df
+        group_all += group_
+
+    df = pd.DataFrame()
+    df["site"] = site_all
+    df["nt"] = nt_all
+    df["stat"] = stat_df_all
+    df["freq"] = freq_df_all
+    df["group"] = group_all
+    df = df.fillna(0)
+    df.to_csv(f"{out_path}/{type_column}/{type_column}.csv",index = False)
+
+    with PdfPages(pdf) as pdf:
+        for i_ in range(df["site"].min(), df["site"].max() + 1):
+            print(i_ + 1)
+            df_site = df[df["site"] == i_]
 
-        with open(group_fasta_path, "w") as f:
-            for seq_id in group_df[id_column]:
-                f.write(f">{seq_id}\n{seq_record[seq_id]}\n")
+            pivot_df = df_site.pivot(index='group', columns='nt', values='freq')
+            if picture_type == "bar":
+                pivot_df.plot(kind='bar', stacked=True, colormap="Set1", yticks=[0.5, 1])
+            elif picture_type == "line":
+                pivot_df.plot(kind='line', colormap="Set1", yticks=[0.5, 1])
+            plt.ylim((0, 1.1))
+            plt.legend(prop={'size': 8}, bbox_to_anchor=(1.12, 1),loc='upper right', fontsize=5)
+            plt.title('Site' + str(i_+1))
+            plt.xlabel(None)
+            # plt.show()
+            pdf.savefig()
+            plt.clf()
+            plt.close('all')
 
-        create_plots_nt(group_fasta_path, group_name, out_path, picture_type)
+def nttj(input_fasta, group):
+    site = []
+    nt = []
+    stat_df = []
+    freq_df = []
 
-def create_plots_nt(input_fasta, group_name, out_path, picture_type):
-    pdf_path = f"{out_path}/{group_name}.pdf"
+    seq_data = [list(i.seq) for i in SeqIO.parse(input_fasta, "fasta")]
+    df = pd.DataFrame(seq_data)
 
-    if os.path.exists(pdf_path):
-        os.remove(pdf_path)
+    for column in df.columns:
+        nt_ = ['A',"T","C","G","-"]
+        nt += nt_
+        site += [column] * len(nt_)
 
-    seq_data = [list(seq.seq) for seq in SeqIO.parse(input_fasta, "fasta")]
-    df = pd.DataFrame(seq_data)
+        stat = Counter(df[column])
+        nt_dict = {nt: stat.get(nt, 0) for nt in nt_}
+        stat_df.extend(nt_dict.values())
 
-    freq_df = []
-    for col in df.columns:
-        stat = Counter(df[col])
-        freq = [stat.get(aa, 0) / len(df) for aa in 'ATCG']
-        freq_df.append(freq)
+        freq = np.array(list(nt_dict.values())) / sum(nt_dict.values())
+        freq_df.extend(freq)
 
-    freq_df = pd.DataFrame(freq_df, columns=list('ATCG'))
+    group_ = [group] * len(site)
 
-    with PdfPages(pdf_path) as pdf:
-        for i, row in tqdm(freq_df.iterrows(), desc="Plotting"):
-            if picture_type == "bar":
-                row.plot(kind='bar', stacked=True, colormap='Set2', yticks=[0.5, 1])
-            elif picture_type == "line":
-                row.plot(kind='line', colormap='Set2', yticks=[0.5, 1])
+    return site, nt, stat_df, freq_df, group_
 
-            plt.ylim((0, 1.1))
-            plt.legend(prop={'size': 8}, bbox_to_anchor=(1.12, 1), loc='upper right', fontsize=5)
-            plt.title(f'Site {i + 1}')
-            plt.xlabel(None)
-            pdf.savefig()
-            plt.clf()
 
 if __name__ == "__main__":
     mutation_app()
```

### Comparing `seqprocessor-0.1.3/seqprocessor/seq/align.py` & `seqprocessor-0.1.4/seqprocessor/seq/align.py`

 * *Files identical despite different names*

### Comparing `seqprocessor-0.1.3/seqprocessor/seq/info.py` & `seqprocessor-0.1.4/seqprocessor/seq/info.py`

 * *Files identical despite different names*

### Comparing `seqprocessor-0.1.3/seqprocessor/seq/phylo.py` & `seqprocessor-0.1.4/seqprocessor/seq/phylo.py`

 * *Files identical despite different names*

### Comparing `seqprocessor-0.1.3/seqprocessor/seq/pretreat.py` & `seqprocessor-0.1.4/seqprocessor/seq/pretreat.py`

 * *Files identical despite different names*

### Comparing `seqprocessor-0.1.3/seqprocessor/seq/translate.py` & `seqprocessor-0.1.4/seqprocessor/seq/translate.py`

 * *Files identical despite different names*

### Comparing `seqprocessor-0.1.3/PKG-INFO` & `seqprocessor-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqprocessor
-Version: 0.1.3
+Version: 0.1.4
 Summary: A sequence tool
 Author: Ruichen Wang
 Author-email: wangruichen100@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

