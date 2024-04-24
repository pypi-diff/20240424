# Comparing `tmp/biobear-0.18.0.tar.gz` & `tmp/biobear-0.19.5.tar.gz`

## Comparing `biobear-0.18.0.tar` & `biobear-0.19.5.tar`

### file list

```diff
@@ -1,85 +1,101 @@
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 biobear-0.18.0/Cargo.toml
--rw-r--r--   0     1001      127       18 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127     3295 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/biobear.svg
--rw-r--r--   0     1001      127      100 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/dependabot.yml
--rw-r--r--   0     1001      127     4017 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1438 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      127      143 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/workflows/smoketest.py
--rw-r--r--   0     1001      127     1159 2024-03-27 18:28:32.000000 biobear-0.18.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4135 2024-03-27 18:28:32.000000 biobear-0.18.0/.gitignore
--rw-r--r--   0     1001      127     3819 2024-03-27 18:28:32.000000 biobear-0.18.0/CHANGELOG.md
--rw-r--r--   0     1001      127     1055 2024-03-27 18:28:32.000000 biobear-0.18.0/LICENSE
--rw-r--r--   0     1001      127      207 2024-03-27 18:28:32.000000 biobear-0.18.0/Makefile
--rw-r--r--   0     1001      127     7956 2024-03-27 18:28:32.000000 biobear-0.18.0/README.md
--rw-r--r--   0     1001      127      393 2024-03-27 18:28:32.000000 biobear-0.18.0/benchmarks/biobear-scan.py
--rw-r--r--   0     1001      127      467 2024-03-27 18:28:32.000000 biobear-0.18.0/benchmarks/biopython-scan.py
--rw-r--r--   0     1001      127      979 2024-03-27 18:28:32.000000 biobear-0.18.0/benchmarks/results.json
--rw-r--r--   0     1001      127     1569 2024-03-27 18:28:32.000000 biobear-0.18.0/bin/test.sh
--rw-r--r--   0     1001      127      285 2024-03-27 18:28:32.000000 biobear-0.18.0/cz.json
--rw-r--r--   0     1001      127      252 2024-03-27 18:28:32.000000 biobear-0.18.0/docs.bash
--rw-r--r--   0     1001      127     1752 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/__init__.py
--rw-r--r--   0     1001      127     1829 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/bam_reader.py
--rw-r--r--   0     1001      127     1883 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      127     1309 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/compression.py
--rw-r--r--   0     1001      127     1520 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      127     1516 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      127      858 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      127     1564 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/gff_reader.py
--rw-r--r--   0     1001      127     1566 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      127     1050 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/mzml_reader.py
--rw-r--r--   0     1001      127     2910 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/reader.py
--rw-r--r--   0     1001      127     1887 2024-03-27 18:28:32.000000 biobear-0.18.0/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      127   124562 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      127     6152 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      127     7608 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      127   339527 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/fake_fastq_file.fastq.gz
--rw-r--r--   0     1001      127     1749 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/file.vcf
--rw-r--r--   0     1001      127     9521 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/index.bcf
--rw-r--r--   0     1001      127      143 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      127     8638 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      127      213 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      127       41 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fa
--rw-r--r--   0     1001      127       55 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fa.gz
--rw-r--r--   0     1001      127       41 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fasta
--rw-r--r--   0     1001      127       22 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fasta.fai
--rw-r--r--   0     1001      127       58 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      127      286 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fastq
--rw-r--r--   0     1001      127      134 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      127      286 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fq
--rw-r--r--   0     1001      127      156 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.fq.gz
--rw-r--r--   0     1001      127      112 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.gff
--rw-r--r--   0     1001      127       91 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      127    17994 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.gtf
--rw-r--r--   0     1001      127     1478 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      127    17171 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.mzML
--rw-r--r--   0     1001      127     2845 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/test.mzML.gz
--rw-r--r--   0     1001      127     4302 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      127     1669 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      127      254 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      127      840 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      127     1758 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_bcf_reader.py
--rw-r--r--   0     1001      127     2175 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      127     1833 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      127      673 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_genbank_reader.py
--rw-r--r--   0     1001      127     1617 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      127     1620 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_gtf_reader.py
--rw-r--r--   0     1001      127      743 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_mzml_reader.py
--rw-r--r--   0     1001      127     7622 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_session.py
--rw-r--r--   0     1001      127     1144 2024-03-27 18:28:32.000000 biobear-0.18.0/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      127       47 2024-03-27 18:28:32.000000 biobear-0.18.0/requirements-dev.txt
--rw-r--r--   0     1001      127     3705 2024-03-27 18:28:32.000000 biobear-0.18.0/src/bam_reader.rs
--rw-r--r--   0     1001      127     3231 2024-03-27 18:28:32.000000 biobear-0.18.0/src/bcf_reader.rs
--rw-r--r--   0     1001      127     3395 2024-03-27 18:28:32.000000 biobear-0.18.0/src/datasources/fasta.rs
--rw-r--r--   0     1001      127     3486 2024-03-27 18:28:32.000000 biobear-0.18.0/src/datasources/fastq.rs
--rw-r--r--   0     1001      127      632 2024-03-27 18:28:32.000000 biobear-0.18.0/src/datasources/mod.rs
--rw-r--r--   0     1001      127     2625 2024-03-27 18:28:32.000000 biobear-0.18.0/src/error.rs
--rw-r--r--   0     1001      127     4365 2024-03-27 18:28:32.000000 biobear-0.18.0/src/execution_result.rs
--rw-r--r--   0     1001      127     3784 2024-03-27 18:28:32.000000 biobear-0.18.0/src/exon_reader.rs
--rw-r--r--   0     1001      127     3144 2024-03-27 18:28:32.000000 biobear-0.18.0/src/file_compression_type.rs
--rw-r--r--   0     1001      127     1873 2024-03-27 18:28:32.000000 biobear-0.18.0/src/lib.rs
--rw-r--r--   0     1001      127     1253 2024-03-27 18:28:32.000000 biobear-0.18.0/src/runtime.rs
--rw-r--r--   0     1001      127     3454 2024-03-27 18:28:32.000000 biobear-0.18.0/src/session_context.rs
--rw-r--r--   0     1001      127     3231 2024-03-27 18:28:32.000000 biobear-0.18.0/src/vcf_reader.rs
--rw-r--r--   0     1001      127   102476 2024-03-27 18:28:49.000000 biobear-0.18.0/Cargo.lock
--rw-r--r--   0     1001      127      725 2024-03-27 18:28:32.000000 biobear-0.18.0/pyproject.toml
--rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 biobear-0.19.5/Cargo.toml
+-rw-r--r--   0     1001      127       18 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     3295 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/biobear.svg
+-rw-r--r--   0     1001      127      100 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4104 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1441 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      127      143 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      127     1160 2024-04-24 03:28:00.000000 biobear-0.19.5/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4135 2024-04-24 03:28:00.000000 biobear-0.19.5/.gitignore
+-rw-r--r--   0     1001      127     4339 2024-04-24 03:28:00.000000 biobear-0.19.5/CHANGELOG.md
+-rw-r--r--   0     1001      127     1055 2024-04-24 03:28:00.000000 biobear-0.19.5/LICENSE
+-rw-r--r--   0     1001      127      207 2024-04-24 03:28:00.000000 biobear-0.19.5/Makefile
+-rw-r--r--   0     1001      127     7956 2024-04-24 03:28:00.000000 biobear-0.19.5/README.md
+-rw-r--r--   0     1001      127      393 2024-04-24 03:28:00.000000 biobear-0.19.5/benchmarks/biobear-scan.py
+-rw-r--r--   0     1001      127      467 2024-04-24 03:28:00.000000 biobear-0.19.5/benchmarks/biopython-scan.py
+-rw-r--r--   0     1001      127      979 2024-04-24 03:28:00.000000 biobear-0.19.5/benchmarks/results.json
+-rw-r--r--   0     1001      127     1569 2024-04-24 03:28:00.000000 biobear-0.19.5/bin/test.sh
+-rw-r--r--   0     1001      127      285 2024-04-24 03:28:00.000000 biobear-0.19.5/cz.json
+-rw-r--r--   0     1001      127      252 2024-04-24 03:28:00.000000 biobear-0.19.5/docs.bash
+-rw-r--r--   0     1001      127     2587 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/__init__.py
+-rw-r--r--   0     1001      127     2304 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      127     2087 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      127     4928 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/biobear.pyi
+-rw-r--r--   0     1001      127     1309 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/compression.py
+-rw-r--r--   0     1001      127     1762 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      127     1756 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      127      858 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      127     1564 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      127     1566 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      127     1050 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/mzml_reader.py
+-rw-r--r--   0     1001      127        0 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/py.typed
+-rw-r--r--   0     1001      127     2910 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/reader.py
+-rw-r--r--   0     1001      127     2129 2024-04-24 03:28:00.000000 biobear-0.19.5/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      127   124562 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      127     6152 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      127     7608 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      127      939 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/cram/0500_mapped.cram
+-rw-r--r--   0     1001      127     7275 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/cram/1404_index_multislice.cram
+-rw-r--r--   0     1001      127      156 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/cram/1404_index_multislice.cram.crai
+-rw-r--r--   0     1001      127  1060702 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/cram/ce.fa
+-rw-r--r--   0     1001      127      230 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/cram/ce.fa.fai
+-rw-r--r--   0     1001      127     3178 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/cram/test_input_1_a.cram
+-rw-r--r--   0     1001      127   339527 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/fake_fastq_file.fastq.gz
+-rw-r--r--   0     1001      127     1749 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/file.vcf
+-rw-r--r--   0     1001      127     9521 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/index.bcf
+-rw-r--r--   0     1001      127      143 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      127     8638 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      127      213 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      127       41 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fa
+-rw-r--r--   0     1001      127       55 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fa.gz
+-rw-r--r--   0     1001      127       41 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fasta
+-rw-r--r--   0     1001      127       22 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fasta.fai
+-rw-r--r--   0     1001      127       58 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      127      286 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fastq
+-rw-r--r--   0     1001      127      134 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      127      286 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fq
+-rw-r--r--   0     1001      127      156 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.fq.gz
+-rw-r--r--   0     1001      127      112 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.gff
+-rw-r--r--   0     1001      127       91 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      127    17994 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.gtf
+-rw-r--r--   0     1001      127     1478 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      127    17171 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.mzML
+-rw-r--r--   0     1001      127     2845 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/test.mzML.gz
+-rw-r--r--   0     1001      127     1025 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/two-cram/rand1k.fa
+-rw-r--r--   0     1001      127       20 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/two-cram/rand1k.fa.fai
+-rw-r--r--   0     1001      127     1029 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/two-cram/twolib.sorted.cram
+-rw-r--r--   0     1001      127       42 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/two-cram/twolib.sorted.cram.crai
+-rw-r--r--   0     1001      127     4302 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      127     1669 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127    13746 2024-04-24 03:28:00.000000 biobear-0.19.5/python/tests/test_session.py
+-rw-r--r--   0     1001      127       47 2024-04-24 03:28:00.000000 biobear-0.19.5/requirements-dev.txt
+-rw-r--r--   0     1001      127     3705 2024-04-24 03:28:00.000000 biobear-0.19.5/src/bam_reader.rs
+-rw-r--r--   0     1001      127     3590 2024-04-24 03:28:00.000000 biobear-0.19.5/src/bcf_reader.rs
+-rw-r--r--   0     1001      127     1397 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/bam.rs
+-rw-r--r--   0     1001      127     1631 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/bcf.rs
+-rw-r--r--   0     1001      127     1561 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/bed.rs
+-rw-r--r--   0     1001      127     2572 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/bigwig.rs
+-rw-r--r--   0     1001      127     1548 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/cram.rs
+-rw-r--r--   0     1001      127     3265 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/fasta.rs
+-rw-r--r--   0     1001      127     3322 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/fastq.rs
+-rw-r--r--   0     1001      127     1353 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/fcs.rs
+-rw-r--r--   0     1001      127     1380 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/genbank.rs
+-rw-r--r--   0     1001      127     1913 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/gff.rs
+-rw-r--r--   0     1001      127     1476 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/gtf.rs
+-rw-r--r--   0     1001      127     1322 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/hmm_dom_tab.rs
+-rw-r--r--   0     1001      127     1224 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/mod.rs
+-rw-r--r--   0     1001      127     1517 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/mzml.rs
+-rw-r--r--   0     1001      127     1071 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/sam.rs
+-rw-r--r--   0     1001      127     2036 2024-04-24 03:28:00.000000 biobear-0.19.5/src/datasources/vcf.rs
+-rw-r--r--   0     1001      127     2618 2024-04-24 03:28:00.000000 biobear-0.19.5/src/error.rs
+-rw-r--r--   0     1001      127     4180 2024-04-24 03:28:00.000000 biobear-0.19.5/src/execution_result.rs
+-rw-r--r--   0     1001      127     3784 2024-04-24 03:28:00.000000 biobear-0.19.5/src/exon_reader.rs
+-rw-r--r--   0     1001      127     3225 2024-04-24 03:28:00.000000 biobear-0.19.5/src/file_compression_type.rs
+-rw-r--r--   0     1001      127     2706 2024-04-24 03:28:00.000000 biobear-0.19.5/src/lib.rs
+-rw-r--r--   0     1001      127     1253 2024-04-24 03:28:00.000000 biobear-0.19.5/src/runtime.rs
+-rw-r--r--   0     1001      127    10798 2024-04-24 03:28:00.000000 biobear-0.19.5/src/session_context.rs
+-rw-r--r--   0     1001      127     3752 2024-04-24 03:28:00.000000 biobear-0.19.5/src/vcf_reader.rs
+-rw-r--r--   0     1001      127   110055 2024-04-24 03:28:04.000000 biobear-0.19.5/Cargo.lock
+-rw-r--r--   0     1001      127      725 2024-04-24 03:28:00.000000 biobear-0.19.5/pyproject.toml
+-rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.19.5/PKG-INFO
```

### Comparing `biobear-0.18.0/.github/biobear.svg` & `biobear-0.19.5/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/.github/workflows/release.yml` & `biobear-0.19.5/.github/workflows/release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,28 @@
   #       target: [aarch64, armv7, ppc64]
 
   #   steps:
   #     - uses: actions/checkout@v4
   #       with:
   #         ref: ${{ github.event.inputs.tag || github.ref }}
 
-  #     - uses: actions/setup-python@v4
+  #     - uses: actions/setup-python@v5
   #       with:
-  #         python-version: 3.9
+  #         python-version: '3.10'
 
   #     - name: Build wheels
   #       uses: PyO3/maturin-action@v1
   #       with:
   #         target: ${{ matrix.target }}
   #         args: --release --out dist --find-interpreter
   #         sccache: 'true'
   #         manylinux: auto
 
   #     - name: Upload wheels
-  #       uses: actions/upload-artifact@v3
+  #       uses: actions/upload-artifact@v4
   #       with:
   #         name: wheels
   #         path: dist
 
   linux:
     runs-on: ubuntu-latest
     strategy:
@@ -51,17 +51,17 @@
         target: [x86_64, aarch64]
 
     steps:
       - uses: actions/checkout@v4
         with:
           ref: ${{ github.event.inputs.tag || github.ref }}
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
-          python-version: 3.9
+          python-version: '3.10'
 
       - name: Build wheels (x86_64)
         if: matrix.target == 'x86_64'
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
@@ -74,94 +74,92 @@
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: 2_28
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-linux-${{ matrix.target }}
           path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ github.event.inputs.tag || github.ref }}
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-windows-${{ matrix.target }}
           path: dist
 
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ github.event.inputs.tag || github.ref }}
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-macos-${{ matrix.target }}
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ github.event.inputs.tag || github.ref }}
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           args: --out dist
       - name: Upload sdist
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-sdist
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: [linux, windows, macos, sdist]
     steps:
-      - uses: actions/download-artifact@v3
-        with:
-          name: wheels
+      - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         with:
           command: upload
-          args: --skip-existing *
+          args: --non-interactive --skip-existing wheels-*/*
```

### Comparing `biobear-0.18.0/.github/workflows/smoke-test.yml` & `biobear-0.19.5/.github/workflows/smoke-test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 jobs:
   test-package-conda:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.8']
+        python-version: ['3.10']
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
       - name: Set up Python
         uses: conda-incubator/setup-miniconda@v2
         with:
           python-version: ${{ matrix.python-version }}
           channels: conda-forge
           activate-environment: biobear
@@ -32,21 +32,21 @@
           conda run -n biobear python ./.github/workflows/smoketest.py
 
   test-package-pip:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.11]
+        python-version: ['3.10']
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install biobear
         run: |
           python -m pip install --upgrade pip
           pip install biobear polars
```

### Comparing `biobear-0.18.0/.github/workflows/test.yml` & `biobear-0.19.5/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     branches:
       - main
 
 jobs:
   test:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
 
       - uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
         with:
-          python-version: '3.9'
+          python-version: '3.10'
 
       - name: Run clippy
         run: cargo clippy --all-targets --all-features -- -D warnings
 
       # setup a virtual environment
       - name: Setup Python and Run Tests
         env:
```

### Comparing `biobear-0.18.0/.gitignore` & `biobear-0.19.5/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/CHANGELOG.md` & `biobear-0.19.5/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,51 @@
+## v0.19.5 (2024-04-23)
+
+### Fix
+
+- update other parts of build
+
+## v0.19.4 (2024-04-23)
+
+### Fix
+
+- update other parts of build
+
+## v0.19.3 (2024-04-23)
+
+### Fix
+
+- update version
+
+## v0.19.2 (2024-04-23)
+
+### Fix
+
+- update version
+
+## v0.19.1 (2024-04-23)
+
+### Fix
+
+- update python versions
+
+## v0.19.0 (2024-04-23)
+
+### Feat
+
+- add cram and fcs (#127)
+- add bed and bigwig (#124)
+- add bam and sam reader methods (#123)
+- add vcf read (#121)
+- add type annotations (#120)
+
+### Refactor
+
+- better obj creation (#117)
+
 ## v0.18.0 (2024-03-27)
 
 ## v0.17.16 (2024-03-21)
 
 ## v0.17.15 (2024-03-20)
 
 ## v0.17.14 (2024-03-20)
```

### Comparing `biobear-0.18.0/LICENSE` & `biobear-0.19.5/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/README.md` & `biobear-0.19.5/README.md`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/benchmarks/results.json` & `biobear-0.19.5/benchmarks/results.json`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/bin/test.sh` & `biobear-0.19.5/bin/test.sh`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/biobear/bam_reader.py` & `biobear-0.19.5/python/biobear/bam_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """BAM File Readers."""
 
 import os
 
 import pyarrow as pa
+import warnings
 
 from biobear.reader import Reader
 from .biobear import _BamIndexedReader, _ExonReader
 
 
 class BamReader(Reader):
     """A BAM File Reader."""
@@ -28,14 +29,19 @@
     def __init__(self, path: os.PathLike):
         """Initialize the BamReader.
 
         Args:
             path (Path): Path to the BAM file.
 
         """
+        warnings.warn(
+            "The BamReader class is deprecated and will be removed in a future release. "
+            "Please use BioBearSessionContext.read_bam_file instead.",
+            DeprecationWarning,
+        )
         self._bam_reader = _ExonReader(str(path), "BAM", None)
 
     @property
     def inner(self):
         """Return the inner reader."""
         return self._bam_reader
 
@@ -47,14 +53,19 @@
         """Initialize the BamIndexedReader.
 
         Args:
             path (Path): Path to the BAM file.
             index (Path): Path to the BAM index file.
 
         """
+        warnings.warn(
+            "The BamIndexedReader class is deprecated and will be removed in a future release. "
+            "Please use BioBearSessionContext.read_bam_file instead.",
+            DeprecationWarning,
+        )
         self._bam_reader = _BamIndexedReader(str(path))
 
     @property
     def inner(self):
         """Return the inner reader."""
         return self._bam_reader
```

### Comparing `biobear-0.18.0/python/biobear/bcf_reader.py` & `biobear-0.19.5/python/biobear/bcf_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,33 +15,41 @@
 
 """BCF File Readers."""
 
 import os
 
 import pyarrow as pa
 
-
 from biobear.reader import Reader
 
 from .biobear import _ExonReader, _BCFIndexedReader
 
+from warnings import warn
+
 
 class BCFReader(Reader):
     """A BCF File Reader.
 
     This class is used to read a BCF file and convert it to a polars DataFrame.
     """
 
     def __init__(self, path: os.PathLike):
         """Initialize the BCFReader.
 
         Args:
             path (Path): Path to the BCF file.
 
         """
+
+        # show a warning that this is deprecated
+        warn(
+            "BCFReader is deprecated, use ExonSessionContext instead",
+            DeprecationWarning,
+        )
+
         self._bcf_reader = _ExonReader(str(path), "BCF", None)
 
     @property
     def inner(self):
         """Return the inner reader."""
         return self._bcf_reader
```

### Comparing `biobear-0.18.0/python/biobear/compression.py` & `biobear-0.19.5/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/biobear/fasta_reader.py` & `biobear-0.19.5/python/biobear/fastq_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,43 +8,49 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""FASTA file reader."""
+"""FASTQ reader."""
 import os
+import warnings
 
 from biobear.reader import Reader
 from biobear.compression import Compression
 
 from .biobear import _ExonReader
 
 
-class FastaReader(Reader):
-    """FASTA file reader."""
+class FastqReader(Reader):
+    """FASTQ file reader."""
 
     def __init__(
         self, path: os.PathLike, compression: Compression = Compression.INFERRED
     ):
-        """Read a fasta file.
+        """Read a fastq file.
 
         Args:
-            path (Path): Path to the fasta file.
+            path (Path): Path to the fastq file.
 
         Kwargs:
             compression (Compression): Compression type of the file. Defaults to
                 Compression.INFERRED.
 
         """
+        warnings.warn(
+            "The FastaReader class is deprecated and will be removed in a future release. "
+            "Please use BioBearSessionContext.read_fasta instead.",
+            DeprecationWarning,
+        )
         self.compression = compression.infer_or_use(path)
 
         if self.compression == Compression.GZIP:
-            self._fasta_reader = _ExonReader(str(path), "FASTA", "GZIP")
+            self._fastq_reader = _ExonReader(str(path), "FASTQ", "GZIP")
         else:
-            self._fasta_reader = _ExonReader(str(path), "FASTA", None)
+            self._fastq_reader = _ExonReader(str(path), "FASTQ", None)
 
     @property
     def inner(self):
         """Return the inner reader."""
-        return self._fasta_reader
+        return self._fastq_reader
```

### Comparing `biobear-0.18.0/python/biobear/genbank_reader.py` & `biobear-0.19.5/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/biobear/gff_reader.py` & `biobear-0.19.5/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/biobear/gtf_reader.py` & `biobear-0.19.5/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/biobear/mzml_reader.py` & `biobear-0.19.5/python/biobear/mzml_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/biobear/reader.py` & `biobear-0.19.5/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/BGC0000404.gbk` & `biobear-0.19.5/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/bedcov.bam` & `biobear-0.19.5/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/bedcov.bam.bai` & `biobear-0.19.5/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/fake_fastq_file.fastq.gz` & `biobear-0.19.5/python/tests/data/fake_fastq_file.fastq.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/file.vcf` & `biobear-0.19.5/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/index.bcf` & `biobear-0.19.5/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/index.vcf.gz` & `biobear-0.19.5/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/test.gtf` & `biobear-0.19.5/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/test.gtf.gz` & `biobear-0.19.5/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/test.mzML` & `biobear-0.19.5/python/tests/data/test.mzML`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/test.mzML.gz` & `biobear-0.19.5/python/tests/data/test.mzML.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/vcf_file.vcf` & `biobear-0.19.5/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/python/tests/data/vcf_file.vcf.gz` & `biobear-0.19.5/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/src/bam_reader.rs` & `biobear-0.19.5/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/src/bcf_reader.rs` & `biobear-0.19.5/src/vcf_reader.rs`

 * *Files 7% similar despite different names*

```diff
@@ -10,34 +10,38 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use arrow::ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream};
 use arrow::pyarrow::IntoPyArrow;
-use datafusion::prelude::{SessionConfig, SessionContext};
+use datafusion::datasource::file_format::file_compression_type::FileCompressionType;
+use datafusion::prelude::SessionContext;
+use exon::datasources::vcf::ListingVCFTableOptions;
 use exon::ffi::DataFrameRecordBatchStream;
+use noodles::core::Region;
 use pyo3::prelude::*;
 use tokio::runtime::Runtime;
 
-use exon::ExonSessionExt;
+use exon::{new_exon_config, ExonSessionExt};
 
 use std::io;
+use std::str::FromStr;
 use std::sync::Arc;
 
 use crate::error::BioBearError;
 
-#[pyclass(name = "_BCFIndexedReader")]
-pub struct BCFIndexedReader {
+#[pyclass(name = "_VCFIndexedReader")]
+pub struct VCFIndexedReader {
     path: String,
     batch_size: Option<usize>,
     _runtime: Arc<Runtime>,
 }
 
-impl BCFIndexedReader {
+impl VCFIndexedReader {
     fn open(path: &str, batch_size: Option<usize>) -> io::Result<Self> {
         // Check the path exists
         if !std::path::Path::new(path).exists() {
             return Err(io::Error::new(
                 io::ErrorKind::NotFound,
                 format!("File not found: {path}"),
             ));
@@ -50,34 +54,44 @@
             batch_size,
             _runtime: rt,
         })
     }
 }
 
 #[pymethods]
-impl BCFIndexedReader {
+impl VCFIndexedReader {
     #[new]
     fn new(path: &str, batch_size: Option<usize>) -> PyResult<Self> {
         Self::open(path, batch_size).map_err(PyErr::new::<pyo3::exceptions::PyValueError, _>)
     }
 
     fn query(&mut self, region: &str) -> PyResult<PyObject> {
-        let mut config = SessionConfig::new();
+        let mut config = new_exon_config();
         if let Some(batch_size) = self.batch_size {
             config = config.with_batch_size(batch_size);
         }
 
-        let ctx = SessionContext::new_with_config(config);
+        let ctx = SessionContext::with_config_exon(config);
+
+        let region = Region::from_str(region).map_err(|e| {
+            io::Error::new(
+                io::ErrorKind::InvalidInput,
+                format!("Error parsing region: {e}"),
+            )
+        })?;
+
+        let options =
+            ListingVCFTableOptions::new(FileCompressionType::GZIP, true).with_regions(vec![region]);
 
         let df = self._runtime.block_on(async {
-            match ctx.query_bcf_file(self.path.as_str(), region).await {
+            match ctx.read_vcf(self.path.as_str(), options).await {
                 Ok(df) => Ok(df),
                 Err(e) => Err(io::Error::new(
                     io::ErrorKind::Other,
-                    format!("Error reading BCF file: {e}"),
+                    format!("Error reading VCF file: {e}"),
                 )),
             }
         })?;
 
         let mut stream_ptr = self._runtime.block_on(async {
             let stream = df.execute_stream().await?;
             let dataset_record_batch_stream =
```

### Comparing `biobear-0.18.0/src/datasources/fasta.rs` & `biobear-0.19.5/src/datasources/fasta.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use crate::{error::BioBearResult, file_compression_type::FileCompressionType};
-use datafusion::datasource::file_format::file_compression_type::FileCompressionType as DFFileCompressionType;
 use exon::datasources::fasta::table_provider::ListingFASTATableOptions;
 use pyo3::{pyclass, pymethods};
 
 const DEFAULT_FASTA_FILE_EXTENSION: &str = "fasta";
 
 #[pyclass]
 #[derive(Debug, Clone)]
@@ -43,30 +42,30 @@
 /// use exon::datasources::fasta::FASTAReadOptions;
 ///
 /// let options = FASTAReadOptions::default();
 /// assert_eq!(options.file_extension, "fasta");
 /// ```
 pub struct FASTAReadOptions {
     file_extension: String,
-    file_compression_type: DFFileCompressionType,
+    file_compression_type: FileCompressionType,
 }
 
 impl Default for FASTAReadOptions {
     fn default() -> Self {
         Self {
             file_extension: String::from(DEFAULT_FASTA_FILE_EXTENSION),
-            file_compression_type: DFFileCompressionType::UNCOMPRESSED,
+            file_compression_type: FileCompressionType::UNCOMPRESSED,
         }
     }
 }
 
 #[pymethods]
 impl FASTAReadOptions {
     #[new]
-    #[pyo3(signature = (*, file_extension=None, file_compression_type=None))]
+    #[pyo3(signature = (/, file_extension=None, file_compression_type=None))]
     /// Create a new FASTAReadOptions instance.
     ///
     /// # Arguments
     ///
     /// * `file_extension` - The file extension to use for the FASTA file.
     /// * `file_compression_type` - The file compression type to use for the FASTA file.
     ///
@@ -77,24 +76,23 @@
     /// # Note
     ///
     /// The arguments are optional in Python, but if passed, must be passed as kwargs.
     pub fn new(
         file_extension: Option<String>,
         file_compression_type: Option<FileCompressionType>,
     ) -> BioBearResult<Self> {
-        let df_compression = file_compression_type
-            .unwrap_or(FileCompressionType::UNCOMPRESSED)
-            .try_into()?;
+        let file_compression_type =
+            file_compression_type.unwrap_or(FileCompressionType::UNCOMPRESSED);
 
         Ok(Self {
-            file_compression_type: df_compression,
+            file_compression_type,
             file_extension: file_extension.unwrap_or(DEFAULT_FASTA_FILE_EXTENSION.to_string()),
         })
     }
 }
 
 impl From<FASTAReadOptions> for ListingFASTATableOptions {
     fn from(options: FASTAReadOptions) -> Self {
-        ListingFASTATableOptions::new(options.file_compression_type)
-            .with_file_extension(options.file_extension)
+        ListingFASTATableOptions::new(options.file_compression_type.into())
+            .with_some_file_extension(Some(&options.file_extension))
     }
 }
```

### Comparing `biobear-0.18.0/src/datasources/fastq.rs` & `biobear-0.19.5/src/datasources/fastq.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-use crate::{error::BioBearResult, file_compression_type::FileCompressionType};
-use datafusion::datasource::file_format::file_compression_type::FileCompressionType as DFFileCompressionType;
+use crate::file_compression_type::FileCompressionType;
 use exon::datasources::fastq::table_provider::ListingFASTQTableOptions;
 use pyo3::{pyclass, pymethods};
 
 const DEFAULT_FASTQ_FILE_EXTENSION: &str = "fastq";
 
 #[pyclass]
 #[derive(Debug, Clone)]
@@ -43,30 +42,30 @@
 /// use exon::datasources::fastq::FASTQReadOptions;
 ///
 /// let options = FASTQReadOptions::default();
 /// assert_eq!(options.file_extension, "fastq");
 /// ```
 pub struct FASTQReadOptions {
     file_extension: String,
-    file_compression_type: DFFileCompressionType,
+    file_compression_type: FileCompressionType,
 }
 
 impl Default for FASTQReadOptions {
     fn default() -> Self {
         Self {
             file_extension: DEFAULT_FASTQ_FILE_EXTENSION.to_string(),
-            file_compression_type: DFFileCompressionType::UNCOMPRESSED,
+            file_compression_type: FileCompressionType::UNCOMPRESSED,
         }
     }
 }
 
 #[pymethods]
 impl FASTQReadOptions {
     #[new]
-    #[pyo3(signature = (*, file_extension=None, file_compression_type=None))]
+    #[pyo3(signature = (/, file_extension=None, file_compression_type=None))]
     /// Create a new FASTQReadOptions instance.
     ///
     /// # Arguments
     ///
     /// * `file_extension` - The file extension to use for the FASTQ file.
     /// * `file_compression_type` - The file compression type to use for the FASTQ file.
     ///
@@ -76,31 +75,30 @@
     ///
     /// # Note
     ///
     /// The arguments are optional in Python, but if passed, must be passed as kwargs.
     pub fn new(
         file_extension: Option<String>,
         file_compression_type: Option<FileCompressionType>,
-    ) -> BioBearResult<Self> {
-        let file_compression_type = file_compression_type
-            .unwrap_or(FileCompressionType::UNCOMPRESSED)
-            .try_into()?;
+    ) -> Self {
+        let file_compression_type =
+            file_compression_type.unwrap_or(FileCompressionType::UNCOMPRESSED);
 
         let file_extension = file_extension.unwrap_or(DEFAULT_FASTQ_FILE_EXTENSION.to_string());
 
-        Ok(Self {
+        Self {
             file_extension,
             file_compression_type,
-        })
+        }
     }
 
     fn __repr__(&self) -> String {
         format!("{:?}", self)
     }
 }
 
 impl From<FASTQReadOptions> for ListingFASTQTableOptions {
     fn from(options: FASTQReadOptions) -> Self {
-        ListingFASTQTableOptions::new(options.file_compression_type)
-            .with_file_extension(options.file_extension)
+        ListingFASTQTableOptions::new(options.file_compression_type.into())
+            .with_some_file_extension(Some(&options.file_extension))
     }
 }
```

### Comparing `biobear-0.18.0/src/error.rs` & `biobear-0.19.5/src/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use arrow::error::ArrowError;
 use datafusion::{error::DataFusionError, sql::sqlparser::parser::ParserError};
-use exon::error::ExonError;
+use exon::ExonError;
 use pyo3::PyErr;
 
 #[derive(Debug)]
 pub enum BioBearError {
     IOError(String),
     Other(String),
     InvalidCompressionType(String),
```

### Comparing `biobear-0.18.0/src/execution_result.rs` & `biobear-0.19.5/src/execution_result.rs`

 * *Files 3% similar despite different names*

```diff
@@ -77,50 +77,44 @@
 
         let runtime = Arc::new(Runtime::new()?);
 
         let dataframe_record_batch_stream = DataFrameRecordBatchStream::new(stream, runtime);
 
         let mut stream = FFI_ArrowArrayStream::new(Box::new(dataframe_record_batch_stream));
 
-        Python::with_gil(|py| unsafe {
-            let stream_reader =
-                ArrowArrayStreamReader::from_raw(&mut stream).map_err(BioBearError::from)?;
+        let stream_reader =
+            unsafe { ArrowArrayStreamReader::from_raw(&mut stream).map_err(BioBearError::from) }?;
 
-            stream_reader.into_pyarrow(py)
-        })
+        stream_reader.into_pyarrow(py)
     }
 
     /// Convert to Arrow Table
     fn to_arrow(&self, py: Python) -> PyResult<PyObject> {
         let batches = self.collect(py)?.to_object(py);
         let schema = self.schema().into_py(py);
 
-        Python::with_gil(|py| {
-            // Instantiate pyarrow Table object and use its from_batches method
-            let table_class = py.import("pyarrow")?.getattr("Table")?;
-
-            let args = PyTuple::new(py, &[batches, schema]);
-            let table: PyObject = table_class.call_method1("from_batches", args)?.into();
-            Ok(table)
-        })
+        // Instantiate pyarrow Table object and use its from_batches method
+        let table_class = py.import("pyarrow")?.getattr("Table")?;
+
+        let args = PyTuple::new(py, &[batches, schema]);
+        let table: PyObject = table_class.call_method1("from_batches", args)?.into();
+        Ok(table)
     }
 
     /// Convert to a Polars DataFrame
     fn to_polars(&self, py: Python) -> PyResult<PyObject> {
         let batches = self.collect(py)?.to_object(py);
         let schema = self.schema().into_py(py);
 
         let schema = schema.into_py(py);
 
-        Python::with_gil(|py| {
-            let table_class = py.import("pyarrow")?.getattr("Table")?;
-            let args = (batches, schema);
-            let table: PyObject = table_class.call_method1("from_batches", args)?.into();
-
-            let module = py.import("polars")?;
-            let args = (table,);
-            let result = module.call_method1("from_arrow", args)?.into();
+        let table_class = py.import("pyarrow")?.getattr("Table")?;
+        let args = (batches, schema);
+        let table: PyObject = table_class.call_method1("from_batches", args)?.into();
+
+        let module = py.import("polars")?;
+        let args = (table,);
+        let result = module.call_method1("from_arrow", args)?.into();
 
-            Ok(result)
-        })
+        Ok(result)
     }
 }
```

### Comparing `biobear-0.18.0/src/exon_reader.rs` & `biobear-0.19.5/src/exon_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/src/runtime.rs` & `biobear-0.19.5/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.18.0/src/vcf_reader.rs` & `biobear-0.19.5/src/bcf_reader.rs`

 * *Files 5% similar despite different names*

```diff
@@ -10,34 +10,37 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use arrow::ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream};
 use arrow::pyarrow::IntoPyArrow;
-use datafusion::prelude::SessionContext;
+use datafusion::prelude::{SessionConfig, SessionContext};
+use exon::datasources::bcf::table_provider::ListingBCFTableOptions;
 use exon::ffi::DataFrameRecordBatchStream;
+use noodles::core::Region;
 use pyo3::prelude::*;
 use tokio::runtime::Runtime;
 
-use exon::{new_exon_config, ExonSessionExt};
+use exon::ExonSessionExt;
 
 use std::io;
+use std::str::FromStr;
 use std::sync::Arc;
 
 use crate::error::BioBearError;
 
-#[pyclass(name = "_VCFIndexedReader")]
-pub struct VCFIndexedReader {
+#[pyclass(name = "_BCFIndexedReader")]
+pub struct BCFIndexedReader {
     path: String,
     batch_size: Option<usize>,
     _runtime: Arc<Runtime>,
 }
 
-impl VCFIndexedReader {
+impl BCFIndexedReader {
     fn open(path: &str, batch_size: Option<usize>) -> io::Result<Self> {
         // Check the path exists
         if !std::path::Path::new(path).exists() {
             return Err(io::Error::new(
                 io::ErrorKind::NotFound,
                 format!("File not found: {path}"),
             ));
@@ -50,34 +53,40 @@
             batch_size,
             _runtime: rt,
         })
     }
 }
 
 #[pymethods]
-impl VCFIndexedReader {
+impl BCFIndexedReader {
     #[new]
     fn new(path: &str, batch_size: Option<usize>) -> PyResult<Self> {
         Self::open(path, batch_size).map_err(PyErr::new::<pyo3::exceptions::PyValueError, _>)
     }
 
     fn query(&mut self, region: &str) -> PyResult<PyObject> {
-        let mut config = new_exon_config();
+        let mut config = SessionConfig::new();
         if let Some(batch_size) = self.batch_size {
             config = config.with_batch_size(batch_size);
         }
 
-        let ctx = SessionContext::with_config_exon(config);
+        let ctx = SessionContext::new_with_config(config);
+
+        let region = Region::from_str(region).map_err(|e| {
+            io::Error::new(io::ErrorKind::Other, format!("Error parsing region: {e}"))
+        })?;
+
+        let options = ListingBCFTableOptions::default().with_regions(vec![region]);
 
         let df = self._runtime.block_on(async {
-            match ctx.query_vcf_file(self.path.as_str(), region).await {
+            match ctx.read_bcf(self.path.as_str(), options).await {
                 Ok(df) => Ok(df),
                 Err(e) => Err(io::Error::new(
                     io::ErrorKind::Other,
-                    format!("Error reading VCF file: {e}"),
+                    format!("Error reading BCF file: {e}"),
                 )),
             }
         })?;
 
         let mut stream_ptr = self._runtime.block_on(async {
             let stream = df.execute_stream().await?;
             let dataset_record_batch_stream =
```

### Comparing `biobear-0.18.0/Cargo.lock` & `biobear-0.19.5/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
@@ -73,30 +73,78 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anstream"
+version = "0.6.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+dependencies = [
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "3.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+dependencies = [
+ "anstyle",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "arrow"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa285343fba4d829d49985bdc541e3789cf6000ed0e84be7c039438df4a4e78c"
+checksum = "219d05930b81663fd3b32e3bde8ce5bff3c4d23052a99f11a8fa50a3b47b2658"
 dependencies = [
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
  "arrow-data",
@@ -108,79 +156,81 @@
  "arrow-select",
  "arrow-string",
  "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "753abd0a5290c1bcade7c6623a556f7d1659c5f4148b140b5b63ce7bd1a45705"
+checksum = "0272150200c07a86a390be651abdd320a2d12e84535f0837566ca87ecd8f95e0"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d390feeb7f21b78ec997a4081a025baef1e2e0d6069e181939b61864c9779609"
+checksum = "8010572cf8c745e242d1b632bd97bd6d4f40fefed5ed1290a8f433abaa686fea"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "chrono-tz",
  "half",
  "hashbrown",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69615b061701bcdffbc62756bc7e85c827d5290b472b580c972ebbbf690f5aa4"
+checksum = "0d0a2432f0cba5692bf4cb757469c66791394bac9ec7ce63c1afe74744c37b27"
 dependencies = [
  "bytes",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e448e5dd2f4113bf5b74a1f26531708f5edcacc77335b7066f9398f4bcf4cdef"
+checksum = "9abc10cd7995e83505cc290df9384d6e5412b207b79ce6bdff89a10505ed2cba"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
- "base64 0.21.7",
+ "atoi",
+ "base64 0.22.0",
  "chrono",
  "comfy-table",
  "half",
  "lexical-core",
  "num",
+ "ryu",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46af72211f0712612f5b18325530b9ad1bfbdc87290d5fbfd32a7da128983781"
+checksum = "95cbcba196b862270bf2a5edb75927380a7f3a163622c61d40cbba416a6305f2"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -189,44 +239,44 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67d644b91a162f3ad3135ce1184d0a31c28b816a581e08f29e8e9277a574c64e"
+checksum = "2742ac1f6650696ab08c88f6dd3f0eb68ce10f8c253958a18c943a68cd04aec5"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03dea5e79b48de6c2e04f03f62b0afea7105be7b77d134f6c5414868feefb80d"
+checksum = "a42ea853130f7e78b9b9d178cb4cd01dee0f78e64d96c2949dc0a915d6d9e19d"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
  "lz4_flex",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8950719280397a47d37ac01492e3506a8a724b3fb81001900b866637a829ee0f"
+checksum = "eaafb5714d4e59feae964714d724f880511500e3569cc2a94d02456b403a2a49"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -236,86 +286,87 @@
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ed9630979034077982d8e74a942b7ac228f33dd93a93b615b4d02ad60c260be"
+checksum = "e3e6b61e3dc468f503181dccc2fc705bdcc5f2f146755fa5b56d0a6c5943f412"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "007035e17ae09c4e8993e4cb8b5b96edf0afb927cd38e2dff27189b274d83dcf"
+checksum = "848ee52bb92eb459b811fb471175ea3afcf620157674c8794f539838920f9228"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
  "hashbrown",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ff3e9c01f7cd169379d269f926892d0e622a704960350d09d331be3ec9e0029"
+checksum = "02d9483aaabe910c4781153ae1b6ae0393f72d9ef757d38d09d450070cf2e528"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "arrow-select"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce20973c1912de6514348e064829e50947e35977bb9d7fb637dc99ea9ffd78c"
+checksum = "849524fa70e0e3c5ab58394c770cb8f514d0122d20de08475f7b472ed8075830"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00f3b37f2aeece31a2636d1b037dabb69ef590e03bdc7eb68519b51ec86932a7"
+checksum = "9373cb5a021aee58863498c37eb484998ef13377f69989c6c5ccfbd258236cdb"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "memchr",
  "num",
  "regex",
  "regex-syntax",
 ]
 
 [[package]]
 name = "async-compression"
-version = "0.4.6"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a116f46a969224200a0a97f29cfd4c50e7534e4b4826bd23ea2c3c533039c82c"
+checksum = "07dbbf24db18d609b1462965249abdf49129ccad073ec257da372adc83259c60"
 dependencies = [
  "bzip2",
  "flate2",
  "futures-core",
  "futures-io",
  "memchr",
  "pin-project-lite",
@@ -323,34 +374,57 @@
  "xz2",
  "zstd",
  "zstd-safe",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.79"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
+]
+
+[[package]]
+name = "atoi"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "attohttpc"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e57d6e7a84f33ff3316e97af3180fe7f86597a6a60161c0be70c0e45f382620"
+dependencies = [
+ "http 0.2.12",
+ "log",
+ "rustls",
+ "rustls-native-certs",
+ "url",
+ "webpki",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "aws-config"
-version = "1.1.9"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "297b64446175a73987cedc3c438d79b2a654d0fff96f65ff530fbe039347644c"
+checksum = "b2a4707646259764ab59fd9a50e9de2e92c637b28b36285d6f6fa030e915fbd9"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-sdk-sso",
  "aws-sdk-ssooidc",
  "aws-sdk-sts",
  "aws-smithy-async",
@@ -371,52 +445,52 @@
  "tracing",
  "url",
  "zeroize",
 ]
 
 [[package]]
 name = "aws-credential-types"
-version = "1.1.8"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa8587ae17c8e967e4b05a62d495be2fb7701bec52a97f7acfe8a29f938384c8"
+checksum = "e16838e6c9e12125face1c1eff1343c75e3ff540de98ff7ebd61874a89bcfeb9"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "zeroize",
 ]
 
 [[package]]
 name = "aws-runtime"
-version = "1.1.8"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b13dc54b4b49f8288532334bba8f87386a40571c47c37b1304979b556dc613c8"
+checksum = "f4963ac9ff2d33a4231b3806c1c69f578f221a9cabb89ad2bde62ce2b442c8a7"
 dependencies = [
  "aws-credential-types",
  "aws-sigv4",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "aws-types",
  "bytes",
  "fastrand",
  "http 0.2.12",
- "http-body",
+ "http-body 0.4.6",
  "percent-encoding",
  "pin-project-lite",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "aws-sdk-sso"
-version = "1.18.0"
+version = "1.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "019a07902c43b03167ea5df0182f0cb63fae89f9a9682c44d18cf2e4a042cb34"
+checksum = "3d70fb493f4183f5102d8a8d0cc9b57aec29a762f55c0e7bf527e0f7177bb408"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-json",
  "aws-smithy-runtime",
@@ -428,17 +502,17 @@
  "once_cell",
  "regex-lite",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sdk-ssooidc"
-version = "1.18.0"
+version = "1.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04c46ee08a48a7f4eaa4ad201dcc1dd537b49c50859d14d4510e00ad9d3f9af2"
+checksum = "de3f37549b3e38b7ea5efd419d4d7add6ea1e55223506eb0b4fef9d25e7cc90d"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-json",
  "aws-smithy-runtime",
@@ -450,17 +524,17 @@
  "once_cell",
  "regex-lite",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sdk-sts"
-version = "1.18.0"
+version = "1.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f752ac730125ca6017f72f9db5ec1772c9ecc664f87aa7507a7d81b023c23713"
+checksum = "3b2ff219a5d4b795cd33251c19dbe9c4b401f2b2cbe513e07c76ada644eaf34e"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-json",
  "aws-smithy-query",
@@ -473,17 +547,17 @@
  "once_cell",
  "regex-lite",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sigv4"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11d6f29688a4be9895c0ba8bef861ad0c0dac5c15e9618b9b7a6c233990fc263"
+checksum = "58b56f1cbe6fd4d0c2573df72868f20ab1c125ca9c9dbce17927a463433a2e57"
 dependencies = [
  "aws-credential-types",
  "aws-smithy-http",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "bytes",
  "form_urlencoded",
@@ -496,36 +570,36 @@
  "sha2",
  "time",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-async"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7a41ccd6b74401a49ca828617049e5c23d83163d330a4f90a8081aadee0ac45"
+checksum = "62220bc6e97f946ddd51b5f1361f78996e704677afc518a4ff66b7a72ea1378c"
 dependencies = [
  "futures-util",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "aws-smithy-http"
-version = "0.60.7"
+version = "0.60.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f10fa66956f01540051b0aa7ad54574640f748f9839e843442d99b970d3aff9"
+checksum = "4a7de001a1b9a25601016d8057ea16e31a45fdca3751304c8edf4ad72e706c08"
 dependencies = [
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "bytes",
  "bytes-utils",
  "futures-core",
  "http 0.2.12",
- "http-body",
+ "http-body 0.4.6",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
  "pin-utils",
  "tracing",
 ]
 
@@ -546,42 +620,43 @@
 dependencies = [
  "aws-smithy-types",
  "urlencoding",
 ]
 
 [[package]]
 name = "aws-smithy-runtime"
-version = "1.1.8"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec81002d883e5a7fd2bb063d6fb51c4999eb55d404f4fff3dd878bf4733b9f01"
+checksum = "44e7945379821074549168917e89e60630647e186a69243248f08c6d168b975a"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "bytes",
  "fastrand",
  "h2",
  "http 0.2.12",
- "http-body",
+ "http-body 0.4.6",
+ "http-body 1.0.0",
  "hyper",
  "hyper-rustls",
  "once_cell",
  "pin-project-lite",
  "pin-utils",
  "rustls",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-runtime-api"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9acb931e0adaf5132de878f1398d83f8677f90ba70f01f65ff87f6d7244be1c5"
+checksum = "4cc56a5c96ec741de6c5e6bf1ce6948be969d6506dfa9c39cffc284e31e4979b"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-types",
  "bytes",
  "http 0.2.12",
  "http 1.1.0",
  "pin-project-lite",
@@ -596,38 +671,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abe14dceea1e70101d38fbf2a99e6a34159477c0fb95e68e05c66bd7ae4c3729"
 dependencies = [
  "base64-simd",
  "bytes",
  "bytes-utils",
  "http 0.2.12",
- "http-body",
+ "http 1.1.0",
+ "http-body 0.4.6",
+ "http-body 1.0.0",
+ "http-body-util",
  "itoa",
  "num-integer",
  "pin-project-lite",
  "pin-utils",
  "ryu",
  "serde",
  "time",
 ]
 
 [[package]]
 name = "aws-smithy-xml"
-version = "0.60.7"
+version = "0.60.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "872c68cf019c0e4afc5de7753c4f7288ce4b71663212771bf5e4542eb9346ca9"
+checksum = "d123fbc2a4adc3c301652ba8e149bf4bc1d1725affb9784eb20c953ace06bf55"
 dependencies = [
  "xmlparser",
 ]
 
 [[package]]
 name = "aws-types"
-version = "1.1.8"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0dbf2f3da841a8930f159163175cf6a3d16ddde517c1b0fba7aa776822800f40"
+checksum = "5a43b56df2c529fe44cb4d92bd64d0479883fb9608ff62daede4df5405381814"
 dependencies = [
  "aws-credential-types",
  "aws-smithy-async",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "http 0.2.12",
  "rustc_version",
@@ -668,20 +746,56 @@
 checksum = "339abbe78e73178762e23bea9dfd08e697eb3f3301cd4be981c0f78ba5859195"
 dependencies = [
  "outref",
  "vsimd",
 ]
 
 [[package]]
+name = "bigtools"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2e7e3e2801e665559947318628677a989ee986fd6f18ac572e332127e72e27aa"
+dependencies = [
+ "attohttpc",
+ "bincode",
+ "byteorder",
+ "byteordered",
+ "bytes",
+ "clap",
+ "crossbeam-channel",
+ "crossbeam-utils",
+ "futures",
+ "itertools 0.10.5",
+ "libdeflater",
+ "ryu",
+ "serde",
+ "smallvec",
+ "tempfile",
+ "thiserror",
+ "tokio",
+ "ufmt",
+]
+
+[[package]]
+name = "bincode"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "biobear"
-version = "0.18.0"
+version = "0.19.5"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
+ "noodles",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "bit-vec"
 version = "0.6.3"
@@ -760,25 +874,34 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
+name = "byteordered"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bbf2cd9424f5ff404aba1959c835cbc448ee8b689b870a9981c76c0fd46280e6"
+dependencies = [
+ "byteorder",
+]
+
+[[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "bytes-utils"
@@ -809,39 +932,40 @@
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "serde",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "chrono-tz"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
@@ -865,21 +989,73 @@
 [[package]]
 name = "circular"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fc239e0f6cb375d2402d48afb92f76f5404fd1df208a41930ec81eda078bea"
 
 [[package]]
+name = "clap"
+version = "4.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
+dependencies = [
+ "clap_builder",
+ "clap_derive",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "clap_lex",
+ "strsim",
+]
+
+[[package]]
+name = "clap_derive"
+version = "4.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
+dependencies = [
+ "heck 0.5.0",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
+
+[[package]]
+name = "coitrees"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "240f9610db0e586042f50260506972820ef10d5eb9a0e867a00f8cfe0a238be3"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "comfy-table"
-version = "7.1.0"
+version = "7.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c64043d6c7b7a4c58e39e7efccfdea7b93d885a795d0c054a69dbbf4dd52686"
+checksum = "b34115915337defe99b2aff5c2ce6771e5fbc4079f4b506301f5cf394c8452f7"
 dependencies = [
- "strum 0.25.0",
- "strum_macros 0.25.3",
+ "strum",
+ "strum_macros",
  "unicode-width",
 ]
 
 [[package]]
 name = "const-random"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1002,30 +1178,31 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2b360b692bf6c6d6e6b6dbaf41a3be0020daeceac0f406aed54c75331e50dbb"
+checksum = "85069782056753459dc47e386219aa1fdac5b731f26c28abb8c0ffd4b7c5ab11"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-ipc",
  "arrow-schema",
  "async-compression",
  "async-trait",
  "bytes",
  "bzip2",
  "chrono",
  "dashmap",
  "datafusion-common",
+ "datafusion-common-runtime",
  "datafusion-execution",
  "datafusion-expr",
  "datafusion-functions",
  "datafusion-functions-array",
  "datafusion-optimizer",
  "datafusion-physical-expr",
  "datafusion-physical-plan",
@@ -1052,37 +1229,47 @@
  "uuid",
  "xz2",
  "zstd",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37f343ccc298f440e25aa38ff82678291a7acc24061c7370ba6c0ff5cc811412"
+checksum = "309d9040751f6dc9e33c85dce6abb55a46ef7ea3644577dd014611c379447ef3"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
  "chrono",
  "half",
+ "instant",
  "libc",
  "num_cpus",
  "object_store",
  "parquet",
  "sqlparser",
 ]
 
 [[package]]
+name = "datafusion-common-runtime"
+version = "37.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e4a44d8ef1b1e85d32234e6012364c411c3787859bb3bba893b0332cb03dfd"
+dependencies = [
+ "tokio",
+]
+
+[[package]]
 name = "datafusion-execution"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9c93043081487e335399a21ebf8295626367a647ac5cb87d41d18afad7d0f7"
+checksum = "06a3a29ae36bcde07d179cc33b45656a8e7e4d023623e320e48dcf1200eeee95"
 dependencies = [
  "arrow",
  "chrono",
  "dashmap",
  "datafusion-common",
  "datafusion-expr",
  "futures",
@@ -1093,62 +1280,79 @@
  "rand",
  "tempfile",
  "url",
 ]
 
 [[package]]
 name = "datafusion-expr"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e204d89909e678846b6a95f156aafc1ee5b36cb6c9e37ec2e1449b078a38c818"
+checksum = "2a3542aa322029c2121a671ce08000d4b274171070df13f697b14169ccf4f628"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
+ "chrono",
  "datafusion-common",
  "paste",
  "sqlparser",
- "strum 0.26.2",
- "strum_macros 0.26.2",
+ "strum",
+ "strum_macros",
 ]
 
 [[package]]
 name = "datafusion-functions"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98f1c73f7801b2b8ba2297b3ad78ffcf6c1fc6b8171f502987eb9ad5cb244ee7"
+checksum = "dd221792c666eac174ecc09e606312844772acc12cbec61a420c2fca1ee70959"
 dependencies = [
  "arrow",
- "base64 0.21.7",
+ "base64 0.22.0",
+ "blake2",
+ "blake3",
+ "chrono",
  "datafusion-common",
  "datafusion-execution",
  "datafusion-expr",
+ "datafusion-physical-expr",
  "hex",
+ "itertools 0.12.1",
  "log",
+ "md-5",
+ "regex",
+ "sha2",
+ "unicode-segmentation",
+ "uuid",
 ]
 
 [[package]]
 name = "datafusion-functions-array"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42d16a0ddf2c991526f6ffe2f47a72c6da0b7354d6c32411dd20631fe2e38937"
+checksum = "e501801e84d9c6ef54caaebcda1b18a6196a24176c12fb70e969bc0572e03c55"
 dependencies = [
  "arrow",
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-ord",
+ "arrow-schema",
  "datafusion-common",
  "datafusion-execution",
  "datafusion-expr",
+ "datafusion-functions",
+ "itertools 0.12.1",
  "log",
  "paste",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ae27e07bf1f04d327be5c2a293470879801ab5535204dc3b16b062fda195496"
+checksum = "76bd7f5087817deb961764e8c973d243b54f8572db414a8f0a8f33a48f991e0a"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
@@ -1156,26 +1360,26 @@
  "itertools 0.12.1",
  "log",
  "regex-syntax",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dde620cd9ef76a3bca9c754fb68854bd2349c49f55baf97e08001f9e967f6d6b"
+checksum = "5cabc0d9aaa0f5eb1b472112f16223c9ffd2fb04e58cbf65c0a331ee6e993f96"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-ord",
  "arrow-schema",
  "arrow-string",
- "base64 0.21.7",
+ "base64 0.22.0",
  "blake2",
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-execution",
  "datafusion-expr",
  "half",
@@ -1187,60 +1391,61 @@
  "md-5",
  "paste",
  "petgraph",
  "rand",
  "regex",
  "sha2",
  "unicode-segmentation",
- "uuid",
 ]
 
 [[package]]
 name = "datafusion-physical-plan"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a4c75fba9ea99d64b2246cbd2fcae2e6fc973e6616b1015237a616036506dd4"
+checksum = "17c0523e9c8880f2492a88bbd857dde02bed1ed23f3e9211a89d3d7ec3b44af9"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
  "async-trait",
  "chrono",
  "datafusion-common",
+ "datafusion-common-runtime",
  "datafusion-execution",
  "datafusion-expr",
  "datafusion-physical-expr",
  "futures",
  "half",
  "hashbrown",
  "indexmap",
  "itertools 0.12.1",
  "log",
  "once_cell",
  "parking_lot",
  "pin-project-lite",
  "rand",
  "tokio",
- "uuid",
 ]
 
 [[package]]
 name = "datafusion-sql"
-version = "36.0.0"
+version = "37.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21474a95c3a62d113599d21b439fa15091b538bac06bd20be0bb2e7d22903c09"
+checksum = "49eb54b42227136f6287573f2434b1de249fe1b8e6cd6cc73a634e4a3ec29356"
 dependencies = [
  "arrow",
+ "arrow-array",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
+ "strum",
 ]
 
 [[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
@@ -1263,23 +1468,23 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
@@ -1308,25 +1513,27 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "exon"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb9f441544608fdec1eda67c5c44a8100d6e12f7404fa13cacb2a34bf28950e9"
+checksum = "6fa0bc4dd82d6ec6f8953d209f6d114d61ac9cbfc9d401306e1d052deae68f97"
 dependencies = [
  "arrow",
  "async-trait",
  "bytes",
+ "coitrees",
  "datafusion",
  "exon-bam",
  "exon-bcf",
  "exon-bed",
+ "exon-bigwig",
  "exon-common",
  "exon-cram",
  "exon-fasta",
  "exon-fastq",
  "exon-fcs",
  "exon-genbank",
  "exon-gff",
@@ -1336,209 +1543,225 @@
  "exon-sam",
  "exon-vcf",
  "futures",
  "fxhash",
  "itertools 0.12.1",
  "lazy_static",
  "noodles",
- "noodles-bgzf",
  "num_cpus",
  "object_store",
  "pin-project",
  "regex",
  "serde",
  "tokio",
  "tokio-util",
  "tracing",
  "tracing-subscriber",
  "url",
 ]
 
 [[package]]
 name = "exon-bam"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6cd27cb3ac89233fc7f68bc96aef96bd6a788ee2d171adf2db8919008b6c0ec1"
+checksum = "36c3dd44c11b39a6f687aef3b183c3b041cf11e548842812cd454828a4210f0d"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-sam",
  "futures",
  "itertools 0.12.1",
  "noodles",
- "noodles-bgzf",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bcf"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b95237feb37c730c1737f4a032249e1cba5e46b3a641d21ba4da6d96cc4d344f"
+checksum = "37bac04538dce4ecf6a9896b95ce94b9c890d6d241f6c667698241b48939935b"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-vcf",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bed"
-version = "0.15.0"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ddef33fe52445d563cbdca3a29decf0c09b340e32046be5865c5fffb263dde8"
+dependencies = [
+ "arrow",
+ "exon-common",
+ "futures",
+ "noodles",
+ "object_store",
+ "tokio",
+ "tokio-util",
+]
+
+[[package]]
+name = "exon-bigwig"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d099f7a2324f6be5c8f0d762a927381ac37d76adf4b2c8308d882fae0b869884"
+checksum = "4672edb009c25f9e21ee477da20afc9df18693839dab7b56e1ca7cb3d9053886"
 dependencies = [
  "arrow",
+ "bigtools",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-common"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75706213ddc22d1b3a0908025d901a54d34f6525a3fa2850f6a3e045f47de71f"
+checksum = "9a937e7a0b277eda0ff02d7aaf2d0da883d3aedbc39c0c5e6e2a1bd43a373bac"
 dependencies = [
  "arrow",
  "datafusion",
  "futures",
  "glob",
  "object_store",
  "url",
 ]
 
 [[package]]
 name = "exon-cram"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8b732904c2420ffec3a11076681b5801e13a8cb5f03477893b78f6badaa3bf7"
+checksum = "586985a4a2d623e0f65005ffb0e82e5e3387e1f32649646434cca0376e213a7c"
 dependencies = [
  "arrow",
+ "coitrees",
  "exon-common",
  "exon-sam",
  "futures",
  "noodles",
  "object_store",
  "tokio",
+ "tracing",
 ]
 
 [[package]]
 name = "exon-fasta"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67b08cb394b3c2680cfdeecb3884c3dd3a6cba456e32a4181ec1f7111fb49166"
+checksum = "c3617480f7c8d671099cc96f2e2353aecbb3c98cd75c24d6205655a90630cc67"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fastq"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d6c8b14809bbdaba18728fc29442e4fcd6677942aca956844678907f8b87eea"
+checksum = "eb694d477d75dd5fdd0518ad3f94872d9e8ec8d2ca46a0b27f3c06eadafc4fcc"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fcs"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0dc90fa7bf274a51b74336cbf776f57f3c6e131fd019df854e8a2448c9b33fe7"
+checksum = "75936579cf7d9ea383e05fcb0753d71d770d86436b30c0a1c1348207829a474d"
 dependencies = [
  "arrow",
  "byteorder",
  "exon-common",
  "futures",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-genbank"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "114869ce479b773bfbe3db6d628604b228d79d882a667c1fe45cfcf22e9b6e36"
+checksum = "8501cc2951e7547d1be6d16d39332c0e0d41872092ae38034c2810e3e1bc8342"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "gb-io",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-gff"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c8c3e0c69ad847e4d827368b6f9a8449454d832654ba94475b2786117385b72"
+checksum = "647d164a26a3c070bbe9a560f7101a34f41894356d331d43fd33c0e1740f16ed"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-gtf"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70b947f811db1ef733a70753f560a368390ef3bc29fe4d1ad0cbd7709a8dd968"
+checksum = "955bc3d05bbbb5d59efe5b6da25c0e123d577e7002472512c38befe2c764d097"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-io"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3822e0487ffb9fba79aa68d565fc678dbc350d056081428013c373f17a93c98"
+checksum = "9a925701c2da63b34e529206a8f4e64fa7fe35ec80b54580eb1f83754fb6745d"
 dependencies = [
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "object_store",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "exon-mzml"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5d4059e0dadab6e63f525df274c566e2318b7dba59cfa752c6e20f7bfc5fbec"
+checksum = "d38acb5706f38f2d55ddc98382bae052a09e89043368ec94cbffa6bed3e182e6"
 dependencies = [
  "arrow",
  "base64 0.22.0",
  "byteorder",
  "exon-common",
  "flate2",
  "futures",
@@ -1546,39 +1769,37 @@
  "quick-xml",
  "serde",
  "tokio",
 ]
 
 [[package]]
 name = "exon-sam"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4587e6f37c5199a902b1d4678839f7ef1bb6faa51dd37c1f645e2386025631"
+checksum = "88ce1dc3243e1c3b9683680bdfaebd9130089c915275679340508c752209afbc"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "itertools 0.12.1",
  "noodles",
- "noodles-bgzf",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-vcf"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85005bdc1e29e25d428cb7fe5cf279ab2603f6b0ed93771426e869144b5ad16b"
+checksum = "d36092b522a08122746c5ca19fed73d2f16674a8b4b7670f5267679ffd009cc3"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
- "noodles-bgzf",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "fastrand"
 version = "2.0.2"
@@ -1662,14 +1883,15 @@
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
+ "num_cpus",
 ]
 
 [[package]]
 name = "futures-io"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
@@ -1678,15 +1900,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1749,17 +1971,17 @@
 dependencies = [
  "typenum",
  "version_check 0.9.4",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -1772,17 +1994,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.25"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http 0.2.12",
@@ -1791,17 +2013,17 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
@@ -1817,14 +2039,20 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
@@ -1871,14 +2099,37 @@
 dependencies = [
  "bytes",
  "http 0.2.12",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "http-body"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http 1.1.0",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "pin-project-lite",
+]
+
+[[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "httpdate"
@@ -1900,15 +2151,15 @@
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http 0.2.12",
- "http-body",
+ "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
@@ -1978,14 +2229,26 @@
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
+name = "instant"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
 name = "ipnet"
@@ -2015,17 +2278,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -2109,26 +2372,26 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libdeflate-sys"
-version = "1.19.3"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc9caa76c8cc6ee8c4efcf8f4514a812ebcad3aa7d3b548efe4d26da1203f177"
+checksum = "c301042beb41d94bc0f8dc667712f8fa8c42d3ea058dd7a71bed3fee8370c75e"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "libdeflater"
-version = "1.19.3"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "265a985bd31e5f22e2b2ac107cbed44c6ccf40ae236e46963cd00dd213e4bd03"
+checksum = "ea90e8df8addcafac4c8737aabf1597f2e83320d58552d8594a52f74cbf24d2e"
 dependencies = [
  "libdeflate-sys",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
@@ -2155,17 +2418,17 @@
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lz4_flex"
-version = "0.11.2"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "912b45c753ff5f7f5208307e8ace7d2a2e30d024e26d3509f3dce546c044ce15"
+checksum = "75761162ae2b0e580d7e7c390558127e5f01b4194debd6221fd8c207fc80e3f5"
 dependencies = [
  "twox-hash",
 ]
 
 [[package]]
 name = "lzma-sys"
 version = "0.1.20"
@@ -2185,17 +2448,17 @@
 dependencies = [
  "cfg-if",
  "digest",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
@@ -2242,17 +2505,17 @@
 dependencies = [
  "memchr",
  "version_check 0.1.5",
 ]
 
 [[package]]
 name = "noodles"
-version = "0.66.0"
+version = "0.70.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f806040f810a3f911dd67246d9361b9e3d149e2b5ed02da43f909835b25fa26"
+checksum = "e5c7777c4301ec50202f778c15d73b88c30f9240a074f9b9a98fe7babfa5bfc8"
 dependencies = [
  "noodles-bam",
  "noodles-bcf",
  "noodles-bed",
  "noodles-bgzf",
  "noodles-core",
  "noodles-cram",
@@ -2264,17 +2527,17 @@
  "noodles-sam",
  "noodles-tabix",
  "noodles-vcf",
 ]
 
 [[package]]
 name = "noodles-bam"
-version = "0.57.0"
+version = "0.60.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a7ece1f74b93a96246c881a9e5710a6d2d1ff23f6503ac1c3ba04819c5f459"
+checksum = "880f71c52dab49e073361e0427610e07eccea07ff48a2ecd8f133c648cb115d8"
 dependencies = [
  "bit-vec",
  "bstr",
  "byteorder",
  "bytes",
  "futures",
  "indexmap",
@@ -2283,17 +2546,17 @@
  "noodles-csi",
  "noodles-sam",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-bcf"
-version = "0.47.0"
+version = "0.51.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7a534e7baf782919cfcf06b10b63df1f821fff75e352027e65e8006b1fe3a1b"
+checksum = "8d58b4cf86ba61cecf9a26b598c2889a28ad7db4a2c0dc1bc5e2c6d7a1858305"
 dependencies = [
  "byteorder",
  "futures",
  "indexmap",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
@@ -2308,40 +2571,39 @@
 checksum = "c116ff14e3dd3ffa6c58771d1a2ee1205690e1c0fe78b0a3456402eebf44ad27"
 dependencies = [
  "noodles-core",
 ]
 
 [[package]]
 name = "noodles-bgzf"
-version = "0.27.0"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43ce62d1e012aa3793e17be1c286b8b71dad5a902a19524eb21729ed16113a9b"
+checksum = "eff82b0fb78c11947b29ef50e8ddf0093813fa9e613af0e13dc53fc12b2dc3ea"
 dependencies = [
  "byteorder",
  "bytes",
  "crossbeam-channel",
  "flate2",
  "futures",
- "libdeflater",
  "pin-project-lite",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "noodles-core"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7336c3be652de4e05444c9b12a32331beb5ba3316e8872d92bfdd8ef3b06c282"
 
 [[package]]
 name = "noodles-cram"
-version = "0.57.0"
+version = "0.60.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4d34fb825a0bcffc231ceda3b4efc216feba4cc7ca9557e6f31c7ecd267715"
+checksum = "0f7ea5956fad57e0c09a0dc84bb0536606434ef82112035d113745215ba71ebc"
 dependencies = [
  "async-compression",
  "bitflags 2.5.0",
  "bstr",
  "byteorder",
  "bytes",
  "bzip2",
@@ -2356,31 +2618,31 @@
  "pin-project-lite",
  "tokio",
  "xz2",
 ]
 
 [[package]]
 name = "noodles-csi"
-version = "0.31.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "512e6c224fcffe4586e408b75f3f5e46fa6d5fe77a2db2afad6b3d085f6cd53a"
+checksum = "938d7d865a3fbb079c7855e76eb1ef0be5d285dc039fa7776622225c7f708411"
 dependencies = [
  "bit-vec",
  "byteorder",
  "indexmap",
  "noodles-bgzf",
  "noodles-core",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-fasta"
-version = "0.34.0"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a838081c9f88c96c7a2c14c8c8a3303f282964b9e91fb53de2f3f9ef8c272b21"
+checksum = "59f7006eff28b06d2c2b1129f9dd2ba637163b92068617060433f22f557e6ce2"
 dependencies = [
  "bytes",
  "memchr",
  "noodles-bgzf",
  "noodles-core",
  "tokio",
 ]
@@ -2394,41 +2656,41 @@
  "futures",
  "memchr",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-gff"
-version = "0.28.0"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a7b22b0e56f109d205a7684eb47e92e9e3dbf65818f0d104281a117ed8ec719"
+checksum = "9216634517bf888abb425b10f3df7857ee3f584d4e46c8d6a2bb2c84acc4e10e"
 dependencies = [
  "indexmap",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "percent-encoding",
 ]
 
 [[package]]
 name = "noodles-gtf"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63d563aee968881bc73f634cd6df96cc0e97590b25f49ee737de068143ed176d"
+checksum = "99d4fabc2e574e80c00341685e8f4df37ae0b5a00a6fecccfd7c99eb45d5a4cf"
 dependencies = [
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
 ]
 
 [[package]]
 name = "noodles-sam"
-version = "0.54.0"
+version = "0.57.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8e1cf471985956a9cd12a8f363f2e8d3069dd843bc11f2920a82bb190f8c122"
+checksum = "6b0598e959a0e56fc60f11b3bc63bf11c332a530cb54883196c0eab1bd0d4b8a"
 dependencies = [
  "bitflags 2.5.0",
  "bstr",
  "futures",
  "indexmap",
  "lexical-core",
  "memchr",
@@ -2436,32 +2698,32 @@
  "noodles-core",
  "noodles-csi",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-tabix"
-version = "0.37.0"
+version = "0.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3cb9ee8ea6d8b4aa9a26a7d29fc1a22dc9afcedb95683f340236ce415f66e531"
+checksum = "8678ba994f92170f6675ad9b839c0163ba10c866ef1a942e6ea83d4ec2ca052a"
 dependencies = [
  "bit-vec",
  "byteorder",
  "indexmap",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-vcf"
-version = "0.50.0"
+version = "0.54.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0de3ecab40d63e5eabd2c64e34b84eb92d54e7a9e64d17f7ca2a3143f48a095c"
+checksum = "010d7057634a154feaf4db8dcc50ef522f5ad7201b6b598e20fb53a5c19ecd3f"
 dependencies = [
  "futures",
  "indexmap",
  "memchr",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
@@ -2478,17 +2740,17 @@
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -2665,27 +2927,27 @@
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "parquet"
-version = "50.0.0"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "547b92ebf0c1177e3892f44c8f79757ee62e678d564a9834189725f2c5b7a750"
+checksum = "096795d4f47f65fd3ee1ec5a98b77ab26d602f2cc785b0e4be5443add17ecc32"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
  "arrow-schema",
  "arrow-select",
- "base64 0.21.7",
+ "base64 0.22.0",
  "brotli",
  "bytes",
  "chrono",
  "flate2",
  "futures",
  "half",
  "hashbrown",
@@ -2803,22 +3065,22 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -2874,17 +3136,17 @@
  "proc-macro2",
  "quote",
  "version_check 0.9.4",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -2928,28 +3190,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
@@ -2957,17 +3219,17 @@
  "memchr",
  "serde",
  "tokio",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -3051,15 +3313,15 @@
  "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http 0.2.12",
- "http-body",
+ "http-body 0.4.6",
  "hyper",
  "hyper-rustls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
@@ -3113,30 +3375,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -3169,17 +3431,17 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -3215,30 +3477,30 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -3250,17 +3512,17 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.14"
@@ -3268,28 +3530,28 @@
 checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3322,17 +3584,17 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "siphasher"
 version = "0.3.11"
@@ -3366,15 +3628,15 @@
 
 [[package]]
 name = "snafu-derive"
 version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "990079665f075b699031e9c08fd3ab99be5029b96f3b78dc0709e8f77e4efebf"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "snap"
@@ -3396,31 +3658,31 @@
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
 [[package]]
 name = "sqlparser"
-version = "0.43.1"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f95c4bae5aba7cd30bd506f7140026ade63cff5afd778af8854026f9606bf5d4"
+checksum = "aaf9c7ff146298ffda83a200f8d5084f08dcee1edfc135fcc1d646a45d50ffd6"
 dependencies = [
  "log",
  "sqlparser_derive",
 ]
 
 [[package]]
 name = "sqlparser_derive"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01b2e185515564f15375f593fb966b5718bc624ba77fe49fa4616ad619690554"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -3448,52 +3710,39 @@
  "phf_generator 0.10.0",
  "phf_shared 0.10.0",
  "proc-macro2",
  "quote",
 ]
 
 [[package]]
-name = "strum"
-version = "0.25.0"
+name = "strsim"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "strum"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 dependencies = [
- "strum_macros 0.26.2",
-]
-
-[[package]]
-name = "strum_macros"
-version = "0.25.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
-dependencies = [
- "heck",
- "proc-macro2",
- "quote",
- "rustversion",
- "syn 2.0.55",
+ "strum_macros",
 ]
 
 [[package]]
 name = "strum_macros"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -3507,17 +3756,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3574,14 +3823,34 @@
  "cfg-if",
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "thiserror"
+version = "1.0.59"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.59"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
+
+[[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
@@ -3596,17 +3865,17 @@
  "byteorder",
  "integer-encoding",
  "ordered-float",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
  "time-macros",
@@ -3616,17 +3885,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
@@ -3650,17 +3919,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
@@ -3674,15 +3943,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -3727,15 +3996,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3788,14 +4057,41 @@
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
+name = "ufmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a64846ec02b57e9108d6469d98d1648782ad6bb150a95a9baac26900bbeab9d"
+dependencies = [
+ "ufmt-macros",
+ "ufmt-write",
+]
+
+[[package]]
+name = "ufmt-macros"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d337d3be617449165cb4633c8dece429afd83f84051024079f97ad32a9663716"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "ufmt-write"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e87a2ed6b42ec5e28cc3b94c09982969e9227600b2e3dcbc1db927a84c06bd69"
+
+[[package]]
 name = "unicode-bidi"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
@@ -3856,14 +4152,20 @@
 [[package]]
 name = "urlencoding"
 version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "daf8dba3b7eb870caf1ddeed7bc9d2a049f3cfdfae7cb521b087cc33ae4c49da"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
@@ -3934,15 +4236,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3968,15 +4270,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -4003,14 +4305,24 @@
 checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "webpki"
+version = "0.22.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed63aea5ce73d0ff405984102c42de94fc55a6b75765d621c65262469b3c9b53"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -4020,34 +4332,34 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "134306a13c5647ad6453e8deaec55d3a44d6021970129e6188735e74bf546697"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -4057,15 +4369,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -4077,110 +4389,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
@@ -4216,15 +4535,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `biobear-0.18.0/pyproject.toml` & `biobear-0.19.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 dependencies = ["pyarrow>=15"]
 license = { file = "LICENSE" }
 name = "biobear"
 readme = "README.md"
 requires-python = ">=3.8"
 description = "A package for working with Bioinformatics data with SQL and Arrow"
 summary = "A package for working with Bioinformatics data with SQL and Arrow"
-version = "0.18.0"
+version = "0.19.5"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
```

### Comparing `biobear-0.18.0/PKG-INFO` & `biobear-0.19.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: biobear
-Version: 0.18.0
+Version: 0.19.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=15
 License-File: LICENSE
 Summary: A package for working with Bioinformatics data with SQL and Arrow
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
```

