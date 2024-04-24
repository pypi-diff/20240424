# Comparing `tmp/dogma_data-0.2.8.tar.gz` & `tmp/dogma_data-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogma_data-0.2.8.tar", last modified: Sat Apr 20 06:00:25 2024, max compression
+gzip compressed data
```

## Comparing `dogma_data-0.2.8.tar` & `dogma_data-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-20 06:00:25.050363 dogma_data-0.2.8/
--rw-r--r--   0 roed     (23269) root         (0)      628 2024-04-20 06:00:25.050363 dogma_data-0.2.8/PKG-INFO
--rw-r--r--   0 roed     (23269) root         (0)        0 2024-04-10 03:45:24.000000 dogma_data-0.2.8/README.md
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-20 06:00:25.050363 dogma_data-0.2.8/dogma_data/
--rw-r--r--   0 roed     (23269) root         (0)      235 2024-04-18 18:31:18.000000 dogma_data-0.2.8/dogma_data/__init__.py
--rw-r--r--   0 roed     (23269) root         (0)    11807 2024-04-19 18:41:42.000000 dogma_data-0.2.8/dogma_data/_dogma_data.py
--rw-r--r--   0 roed     (23269) root         (0)      450 2024-04-10 03:45:24.000000 dogma_data-0.2.8/dogma_data/dogma_torch.py
--rw-r--r--   0 roed     (23269) root         (0)     7292 2024-04-10 07:59:30.000000 dogma_data-0.2.8/dogma_data/fasta.py
--rw-r--r--   0 roed     (23269) root         (0)     3287 2024-04-18 18:25:24.000000 dogma_data-0.2.8/dogma_data/sharded_data.py
--rw-r--r--   0 roed     (23269) root         (0)      762 2024-04-10 03:45:24.000000 dogma_data-0.2.8/dogma_data/utils.py
-drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-20 06:00:25.050363 dogma_data-0.2.8/dogma_data.egg-info/
--rw-r--r--   0 roed     (23269) root         (0)      628 2024-04-20 06:00:25.000000 dogma_data-0.2.8/dogma_data.egg-info/PKG-INFO
--rw-r--r--   0 roed     (23269) root         (0)      335 2024-04-20 06:00:25.000000 dogma_data-0.2.8/dogma_data.egg-info/SOURCES.txt
--rw-r--r--   0 roed     (23269) root         (0)        1 2024-04-20 06:00:25.000000 dogma_data-0.2.8/dogma_data.egg-info/dependency_links.txt
--rw-r--r--   0 roed     (23269) root         (0)       93 2024-04-20 06:00:25.000000 dogma_data-0.2.8/dogma_data.egg-info/requires.txt
--rw-r--r--   0 roed     (23269) root         (0)       11 2024-04-20 06:00:25.000000 dogma_data-0.2.8/dogma_data.egg-info/top_level.txt
--rw-r--r--   0 roed     (23269) root         (0)     1067 2024-04-20 06:00:06.000000 dogma_data-0.2.8/pyproject.toml
--rw-r--r--   0 roed     (23269) root         (0)       38 2024-04-20 06:00:25.050363 dogma_data-0.2.8/setup.cfg
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_data-0.2.9/Cargo.toml
+-rw-r--r--   0    23269        0      134 2024-04-22 01:14:15.000000 dogma_data-0.2.9/.gitignore
+-rw-r--r--   0    23269        0        0 2024-04-22 00:55:04.000000 dogma_data-0.2.9/LICENSE
+-rw-r--r--   0    23269        0        0 2024-04-10 03:45:24.000000 dogma_data-0.2.9/README.md
+-rw-r--r--   0    23269        0     3526 2024-04-10 03:45:24.000000 dogma_data-0.2.9/dogma-rust/.github/workflows/CI.yml
+-rw-r--r--   0    23269        0      686 2024-04-10 03:45:24.000000 dogma_data-0.2.9/dogma-rust/.gitignore
+-rw-r--r--   0    23269        0    19526 2024-04-21 21:48:52.000000 dogma_data-0.2.9/dogma-rust/Cargo.lock
+-rw-r--r--   0    23269        0      472 2024-04-22 00:16:02.000000 dogma_data-0.2.9/dogma-rust/README.md
+-rw-r--r--   0    23269        0      538 2024-04-21 21:31:45.000000 dogma_data-0.2.9/dogma-rust/pyproject.toml
+-rw-r--r--   0    23269        0      235 2024-04-18 18:31:18.000000 dogma_data-0.2.9/dogma_data/__init__.py
+-rw-r--r--   0    23269        0    11807 2024-04-21 21:33:51.000000 dogma_data-0.2.9/dogma_data/_dogma_data.py
+-rw-r--r--   0    23269        0      450 2024-04-10 03:45:24.000000 dogma_data-0.2.9/dogma_data/dogma_torch.py
+-rw-r--r--   0    23269        0     7305 2024-04-22 01:00:17.000000 dogma_data-0.2.9/dogma_data/fasta.py
+-rw-r--r--   0    23269        0     3287 2024-04-18 18:25:24.000000 dogma_data-0.2.9/dogma_data/sharded_data.py
+-rw-r--r--   0    23269        0      762 2024-04-10 03:45:24.000000 dogma_data-0.2.9/dogma_data/utils.py
+-rw-r--r--   0    23269        0      499 2024-04-22 00:34:05.000000 dogma_data-0.2.9/dogma_rust.pyi
+-rw-r--r--   0    23269        0     9115 2024-04-10 03:46:52.000000 dogma_data-0.2.9/lightning_write_shuffled.py
+-rw-r--r--   0    23269        0     3997 2024-04-10 03:46:52.000000 dogma_data-0.2.9/make_packed.py
+-rw-r--r--   0    23269        0     3453 2024-04-11 03:27:15.000000 dogma_data-0.2.9/make_sharded.py
+-rw-r--r--   0    23269        0     1507 2024-04-10 08:31:56.000000 dogma_data-0.2.9/make_shuffled.py
+-rw-r--r--   0    23269        0      872 2024-04-10 03:45:24.000000 dogma_data-0.2.9/mds_convert.py
+-rw-r--r--   0    23269        0     7408 2024-04-10 08:22:28.000000 dogma_data-0.2.9/notebooks/fasta_parse.ipynb
+-rw-r--r--   0    23269        0     2395 2024-04-21 23:47:49.000000 dogma_data-0.2.9/src/data.rs
+-rw-r--r--   0    23269        0     5150 2024-04-21 23:48:09.000000 dogma_data-0.2.9/src/fasta.rs
+-rw-r--r--   0    23269        0     5714 2024-04-22 00:14:58.000000 dogma_data-0.2.9/src/lib.rs
+-rw-r--r--   0    23269        0     3254 2024-04-22 00:02:26.000000 dogma_data-0.2.9/src/parallel.rs
+-rw-r--r--   0    23269        0      492 2024-04-10 03:45:24.000000 dogma_data-0.2.9/write_blosc_to_ak.py
+-rw-r--r--   0    23269        0    19526 2024-04-22 00:55:33.000000 dogma_data-0.2.9/Cargo.lock
+-rw-r--r--   0    23269        0      784 2024-04-22 01:12:13.000000 dogma_data-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 dogma_data-0.2.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dogma_data-0.2.8/dogma_data/_dogma_data.py` & `dogma_data-0.2.9/dogma_data/_dogma_data.py`

 * *Files identical despite different names*

### Comparing `dogma_data-0.2.8/dogma_data/fasta.py` & `dogma_data-0.2.9/dogma_data/fasta.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,12 +176,12 @@
                     "<seq_protein_masked>",
                 ]
             ]
         ),
         specials=["<pad>", "<sos>", "<eos>", "<unk>"],
     )
     AA_VOCAB.set_default_index(AA_VOCAB["<aaunk>"])
-    fasta_lines = parse_fasta('fasta_data/result_rep_seq.fasta', AA_VOCAB)
+    fasta_lines = parse_fasta('rna_taxon_fastas/ccds_rna_aa_taxon.fa', AA_VOCAB, 'rna')
     # with open('fasta_data/result_rep_seq.fasta', 'r') as f:
     #     fasta_lines = parse_fasta(f.read(), AA_VOCAB)
     print(fasta_lines)
     breakpoint()
```

### Comparing `dogma_data-0.2.8/dogma_data/sharded_data.py` & `dogma_data-0.2.9/dogma_data/sharded_data.py`

 * *Files identical despite different names*

### Comparing `dogma_data-0.2.8/dogma_data/utils.py` & `dogma_data-0.2.9/dogma_data/utils.py`

 * *Files identical despite different names*

