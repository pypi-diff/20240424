# Comparing `tmp/unimernet-0.0.2-py2.py3-none-any.whl.zip` & `tmp/unimernet-0.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2226225 bytes, number of entries: 69
+Zip file size: 2226268 bytes, number of entries: 69
 -rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 test.py
 -rw-r--r--  2.0 unx     2750 b- defN 80-Jan-01 00:00 train.py
 -rw-r--r--  2.0 unx      950 b- defN 80-Jan-01 00:00 unimernet/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/common/__init__.py
 -rw-r--r--  2.0 unx    15074 b- defN 80-Jan-01 00:00 unimernet/common/config.py
 -rw-r--r--  2.0 unx     3614 b- defN 80-Jan-01 00:00 unimernet/common/dist_utils.py
 -rw-r--r--  2.0 unx      815 b- defN 80-Jan-01 00:00 unimernet/common/gradcam.py
@@ -59,13 +59,13 @@
 -rw-r--r--  2.0 unx    11292 b- defN 80-Jan-01 00:00 unimernet/processors/randaugment.py
 -rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 unimernet/runners/__init__.py
 -rw-r--r--  2.0 unx    23307 b- defN 80-Jan-01 00:00 unimernet/runners/runner_base.py
 -rw-r--r--  2.0 unx    11842 b- defN 80-Jan-01 00:00 unimernet/runners/runner_iter.py
 -rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 unimernet/tasks/__init__.py
 -rw-r--r--  2.0 unx     9180 b- defN 80-Jan-01 00:00 unimernet/tasks/base_task.py
 -rw-r--r--  2.0 unx     6318 b- defN 80-Jan-01 00:00 unimernet/tasks/unimernet_train.py
--rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     7646 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6544 b- defN 16-Jan-01 00:00 unimernet-0.0.2.dist-info/RECORD
-69 files, 2620078 bytes uncompressed, 2215619 bytes compressed:  15.4%
+-rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7905 b- defN 80-Jan-01 00:00 unimernet-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 unimernet-0.0.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6543 b- defN 16-Jan-01 00:00 unimernet-0.0.3.dist-info/RECORD
+69 files, 2620304 bytes uncompressed, 2215662 bytes compressed:  15.4%
```

## zipnote {}

```diff
@@ -186,23 +186,23 @@
 
 Filename: unimernet/tasks/base_task.py
 Comment: 
 
 Filename: unimernet/tasks/unimernet_train.py
 Comment: 
 
-Filename: unimernet-0.0.2.dist-info/LICENSE
+Filename: unimernet-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: unimernet-0.0.2.dist-info/METADATA
+Filename: unimernet-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: unimernet-0.0.2.dist-info/WHEEL
+Filename: unimernet-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: unimernet-0.0.2.dist-info/entry_points.txt
+Filename: unimernet-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: unimernet-0.0.2.dist-info/RECORD
+Filename: unimernet-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `unimernet-0.0.2.dist-info/LICENSE` & `unimernet-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unimernet-0.0.2.dist-info/METADATA` & `unimernet-0.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unimernet
-Version: 0.0.2
+Version: 0.0.3
 Summary: UniMERNet: A Universal Network for Real-World Mathematical Expression Recognition
-Home-page: https://github.com/xxx
+Home-page: https://github.com/opendatalab/UniMERNet
 License: Apache-2.0
 Keywords: MER,latex,markdown,pdf
 Author: Bin Wang
 Author-email: ictwangbin@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -22,29 +22,32 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: albumentations (>=1.4.4,<2.0.0)
 Requires-Dist: eva-decord (>=0.6.1,<0.7.0)
 Requires-Dist: evaluate (>=0.4.1,<0.5.0)
 Requires-Dist: fairscale (>=0.4.13,<0.5.0)
 Requires-Dist: ftfy (>=6.2.0,<7.0.0)
 Requires-Dist: iopath (>=0.1.10,<0.2.0)
+Requires-Dist: jupyterlab (>=4.1.6,<5.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: opencv-python (>=4.9.0,<5.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: timm (>=0.9.16,<0.10.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: torchtext (>=0.17.2,<0.18.0)
 Requires-Dist: torchvision (>=0.17.2,<0.18.0)
 Requires-Dist: transformers (>=4.40.0,<5.0.0)
 Requires-Dist: wand (>=0.6.13,<0.7.0)
 Requires-Dist: webdataset (>=0.2.86,<0.3.0)
-Project-URL: Repository, https://github.com/xxx
+Project-URL: Repository, https://github.com/opendatalab/UniMERNet
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1>UniMERNet: A Universal Network for Real-World Mathematical Expression Recognition</h1>
 
 [![Paper](https://img.shields.io/badge/Paper-arxiv)]()
 [![Hugging Face Spaces](https://img.shields.io/badge/🤗%20Hugging%20Face-Community%20Space-blue)]()
@@ -53,21 +56,28 @@
 
 This is the official repository for UniMERNet, a math recogition model that can be used for image to LaTeX conversion for a wide range of senarios.
 
 Project page: https://gitlab.pjlab.org.cn/fdc/mllm/unimernet
 
 ## Installation
 
+``` bash 
+conda create -n unimernet python=3.10
+
+conda activate unimernet
+
+pip install unimernet
+```
+
 ### For Mac
 ```bash
 brew install freetype imagemagick
 export MAGICK_HOME=/opt/homebrew/opt/imagemagick
 ```
 
-
 ## Quickstart
 
 ### Try the Streamlit Demo
 
 ### Write MER Code in less than 10 lines of code
```

## Comparing `unimernet-0.0.2.dist-info/RECORD` & `unimernet-0.0.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -58,12 +58,12 @@
 unimernet/processors/randaugment.py,sha256=mNaXux-SCMNBYIubeG9k9YRxIkv7p6JMecTJqq4AabM,11292
 unimernet/runners/__init__.py,sha256=RXvSvxFZ2_Q5Lq_0OHe8x53uiLC6vO-SgVmtiKZnEeY,368
 unimernet/runners/runner_base.py,sha256=XN1OLAq5t68u5-BCVnALXnhZSVFDLur7z0CyIpSSti8,23307
 unimernet/runners/runner_iter.py,sha256=tz88ZTLymApeEe5A-wVynscWuc7uTymQFngCxI2Tqes,11842
 unimernet/tasks/__init__.py,sha256=5_T40TR9RVIURJDppFO-fgQjUxygtlvEtZpoZFEKLp4,717
 unimernet/tasks/base_task.py,sha256=FujbWh9o6a4tnDIR3pSYPqSnkTppGPhmdg9648AsVcE,9180
 unimernet/tasks/unimernet_train.py,sha256=ut8QUVOPgnLbiuGfIpHbM4SJwbmVr2SbVvR_q46AzjQ,6318
-unimernet-0.0.2.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
-unimernet-0.0.2.dist-info/METADATA,sha256=BrwJVMOHVVCt6Zz3STpe9pNQKaPqHobkrizGTukgc6c,7646
-unimernet-0.0.2.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
-unimernet-0.0.2.dist-info/entry_points.txt,sha256=_OsnCi4ChrM_8ss-TzUkaPxwqMLI2I5ve5SoCcCKc-w,104
-unimernet-0.0.2.dist-info/RECORD,,
+unimernet-0.0.3.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
+unimernet-0.0.3.dist-info/METADATA,sha256=DbMcPeEQVNwV1B2O-oDrMHfIfRnlGnhCBerttA8m8_M,7905
+unimernet-0.0.3.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
+unimernet-0.0.3.dist-info/entry_points.txt,sha256=zISHJOfWynQr_VgZmV7Z6LBRwjH8VmuNjU1rFXeGbSk,72
+unimernet-0.0.3.dist-info/RECORD,,
```

