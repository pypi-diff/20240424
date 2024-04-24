# Comparing `tmp/unofficial_ascend_tools-0.0.1-py3-none-any.whl.zip` & `tmp/unofficial_ascend_tools-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7742 bytes, number of entries: 8
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:20 unofficial_ascend_tools/__init__.py
--rw-rw-r--  2.0 unx       69 b- defN 24-Apr-18 09:19 unofficial_ascend_tools/embeddings/__init__.py
--rw-rw-r--  2.0 unx     3855 b- defN 24-Apr-18 09:17 unofficial_ascend_tools/embeddings/ascend.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-18 09:46 unofficial_ascend_tools-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      902 b- defN 24-Apr-18 09:46 unofficial_ascend_tools-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 09:46 unofficial_ascend_tools-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 24-Apr-18 09:46 unofficial_ascend_tools-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      757 b- defN 24-Apr-18 09:46 unofficial_ascend_tools-0.0.1.dist-info/RECORD
-8 files, 17056 bytes uncompressed, 6384 bytes compressed:  62.6%
+Zip file size: 7773 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:51 unofficial_ascend_tools/__init__.py
+-rw-r--r--  2.0 unx       69 b- defN 24-Apr-23 13:51 unofficial_ascend_tools/embeddings/__init__.py
+-rw-r--r--  2.0 unx     4239 b- defN 24-Apr-23 14:05 unofficial_ascend_tools/embeddings/ascend.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-23 14:06 unofficial_ascend_tools-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      906 b- defN 24-Apr-23 14:06 unofficial_ascend_tools-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 14:06 unofficial_ascend_tools-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-23 14:06 unofficial_ascend_tools-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      757 b- defN 24-Apr-23 14:06 unofficial_ascend_tools-0.0.2.dist-info/RECORD
+8 files, 17444 bytes uncompressed, 6415 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: unofficial_ascend_tools/embeddings/__init__.py
 Comment: 
 
 Filename: unofficial_ascend_tools/embeddings/ascend.py
 Comment: 
 
-Filename: unofficial_ascend_tools-0.0.1.dist-info/LICENSE
+Filename: unofficial_ascend_tools-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: unofficial_ascend_tools-0.0.1.dist-info/METADATA
+Filename: unofficial_ascend_tools-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: unofficial_ascend_tools-0.0.1.dist-info/WHEEL
+Filename: unofficial_ascend_tools-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: unofficial_ascend_tools-0.0.1.dist-info/top_level.txt
+Filename: unofficial_ascend_tools-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: unofficial_ascend_tools-0.0.1.dist-info/RECORD
+Filename: unofficial_ascend_tools-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## unofficial_ascend_tools/embeddings/ascend.py

```diff
@@ -28,26 +28,30 @@
     query_instruction: str = ""
     """Unstruntion to used for embedding document."""
     document_instruction: str = ""
     use_fp16: bool = True
     pooling_method: Optional[str] = 'cls'
     model: Any
     tokenizer: Any
+    is_npu_avaiable: bool = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         try:
             from transformers import AutoTokenizer, AutoModel
         except ImportError as e:
             raise ImportError(
                 "Unable to import transformers, please install with "
                 "`pip install -U transformers`."
             ) from e
         try:
-            self.model = AutoModel.from_pretrained(self.model_path).npu().eval()
+            if self.is_npu_avaiable:
+                self.model = AutoModel.from_pretrained(self.model_path).npu().eval()
+            else:
+                self.model = AutoModel.from_pretrained(self.model_path).eval()
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_path)
         except Exception as e:
             raise Exception(f"Failed to load model [self.model_path], due to following error:{e}")
 
         if self.use_fp16:
             self.model.half()
         self.encode([f"warmup {i} times" for i in range(10)])
@@ -55,15 +59,16 @@
     @root_validator
     def validate_environment(cls, values: Dict) -> Dict:
         if not os.access(values['model_path'], os.F_OK):
             raise FileNotFoundError(f"Unabled to find valid model path in [{values['model_path']}]")
         try:
             import torch_npu
         except ImportError:
-            raise ModuleNotFoundError("torch_npu not found, please install torch_npu")
+            values['is_npu_avaiable'] = False
+            return values
         except Exception as e:
             raise e
         try:
             torch_npu.npu.set_device(values['device_id'])
         except Exception as e:
             raise Exception(f"set device failed due to {e}")
         return values
@@ -76,16 +81,20 @@
             max_length=512)
         try:
             import torch
         except ImportError as e:
             raise ImportError("Unable to import torch, please install with "
                 "`pip install -U torch`."
             ) from e
-        last_hidden_state = self.model(inputs.input_ids.npu(), return_dict=True).last_hidden_state
-        tmp = self.pooling(last_hidden_state, inputs['attention_mask'].npu())
+        if self.is_npu_avaiable:
+            last_hidden_state = self.model(inputs.input_ids.npu(), return_dict=True).last_hidden_state
+            tmp = self.pooling(last_hidden_state, inputs['attention_mask'].npu())
+        else:
+            last_hidden_state = self.model(inputs.input_ids, return_dict=True).last_hidden_state
+            tmp = self.pooling(last_hidden_state, inputs['attention_mask'])
         embeddings = torch.nn.functional.normalize(tmp, dim=-1)
         return embeddings.cpu().detach().numpy()
 
 
     def pooling(self,
             last_hidden_state: Any,
             attention_mask: Any = None):
```

## Comparing `unofficial_ascend_tools-0.0.1.dist-info/LICENSE` & `unofficial_ascend_tools-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unofficial_ascend_tools-0.0.1.dist-info/METADATA` & `unofficial_ascend_tools-0.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unofficial-ascend-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: unofficial-ascend-tools
 Home-page: https://gitee.com/yuncliu/unofficial-ascend-tools
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.7
@@ -22,13 +22,13 @@
 source /usr/local/Ascend/ascend-toolkit/env.sh
 ```
 
 2. install torch and torch_npu
 
 3. now use like bellow
 ```python
-from langchain_community.embeddings import AscendEmbeddings
+from unofficial_ascend_tools.embeddings import AscendEmbeddings
 model = AscendEmbeddings(model_path=<path_to_model>,
     device_id=0,
     query_instruction="Represend this sentence for searching relevant passages: "
 )
 ```
```

## Comparing `unofficial_ascend_tools-0.0.1.dist-info/RECORD` & `unofficial_ascend_tools-0.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 unofficial_ascend_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unofficial_ascend_tools/embeddings/__init__.py,sha256=sLiUPg91TiPreUo35A-gHFcPC4171KZjTy_0YPQ0nf4,69
-unofficial_ascend_tools/embeddings/ascend.py,sha256=NB4Ze4XB245Z8dksRZVfxp6Tq--Zhe6MvQvNV8Sdl5o,3855
-unofficial_ascend_tools-0.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-unofficial_ascend_tools-0.0.1.dist-info/METADATA,sha256=4a6mnmfPYkEjgLwC1X9u0oBX4W-d9zY_11IZtq3XX70,902
-unofficial_ascend_tools-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-unofficial_ascend_tools-0.0.1.dist-info/top_level.txt,sha256=TX3n2FFt32LXdFEL1VjYp4742pYURPNhMC-d4lZTkzM,24
-unofficial_ascend_tools-0.0.1.dist-info/RECORD,,
+unofficial_ascend_tools/embeddings/ascend.py,sha256=jC8icWrdOlUdz1qKfHPmPhGetM8sBqqtK5dYB71hJRI,4239
+unofficial_ascend_tools-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+unofficial_ascend_tools-0.0.2.dist-info/METADATA,sha256=xuTRaZ9_Ff4J1Av9l5Vz_ACsr3LwpT7lNCXPjjYfT7U,906
+unofficial_ascend_tools-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+unofficial_ascend_tools-0.0.2.dist-info/top_level.txt,sha256=TX3n2FFt32LXdFEL1VjYp4742pYURPNhMC-d4lZTkzM,24
+unofficial_ascend_tools-0.0.2.dist-info/RECORD,,
```

