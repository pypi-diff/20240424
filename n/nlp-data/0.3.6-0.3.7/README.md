# Comparing `tmp/nlp_data-0.3.6.tar.gz` & `tmp/nlp_data-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_data-0.3.6.tar", max compression
+gzip compressed data, was "nlp_data-0.3.7.tar", max compression
```

## Comparing `nlp_data-0.3.6.tar` & `nlp_data-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4445 2024-02-21 08:13:09.155055 nlp_data-0.3.6/README.md
--rw-r--r--   0        0        0       69 2024-02-05 08:00:25.134574 nlp_data-0.3.6/nlp_data/__init__.py
--rw-r--r--   0        0        0       29 2023-09-07 05:38:28.176112 nlp_data-0.3.6/nlp_data/augment/__init__.py
--rw-r--r--   0        0        0    10505 2024-03-01 02:57:22.799778 nlp_data-0.3.6/nlp_data/augment/gpt.py
--rw-r--r--   0        0        0     2665 2023-10-20 09:37:59.968020 nlp_data-0.3.6/nlp_data/cli.py
--rw-r--r--   0        0        0      186 2023-09-12 23:32:47.410236 nlp_data-0.3.6/nlp_data/document/__init__.py
--rw-r--r--   0        0        0     3940 2023-11-15 10:30:38.549269 nlp_data-0.3.6/nlp_data/document/api.py
--rw-r--r--   0        0        0     2111 2023-11-15 12:20:30.863273 nlp_data-0.3.6/nlp_data/document/dialogue.py
--rw-r--r--   0        0        0     2561 2024-02-02 07:55:00.926673 nlp_data-0.3.6/nlp_data/document/embedding.py
--rw-r--r--   0        0        0    28905 2024-03-14 02:59:52.609343 nlp_data-0.3.6/nlp_data/document/nlu.py
--rw-r--r--   0        0        0      259 2023-10-12 09:35:14.295863 nlp_data-0.3.6/nlp_data/storage/__init__.py
--rw-r--r--   0        0        0      698 2024-02-22 06:16:36.239175 nlp_data-0.3.6/nlp_data/storage/api.py
--rw-r--r--   0        0        0     4338 2023-10-18 09:35:57.215122 nlp_data-0.3.6/nlp_data/storage/base.py
--rw-r--r--   0        0        0      737 2023-11-02 03:31:01.217994 nlp_data-0.3.6/nlp_data/storage/dialogue.py
--rw-r--r--   0        0        0      745 2023-11-02 03:32:52.423265 nlp_data-0.3.6/nlp_data/storage/embdding.py
--rw-r--r--   0        0        0     1069 2024-02-22 11:22:56.086356 nlp_data-0.3.6/nlp_data/storage/nlu.py
--rw-r--r--   0        0        0     9732 2023-11-01 10:04:19.272964 nlp_data-0.3.6/nlp_data/storage/s3.py
--rw-r--r--   0        0        0     2815 2024-03-01 02:59:47.274999 nlp_data-0.3.6/nlp_data/utils.py
--rw-r--r--   0        0        0      855 2024-03-14 03:01:11.601156 nlp_data-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 nlp_data-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     4806 2024-03-29 03:37:28.228914 nlp_data-0.3.7/README.md
+-rw-r--r--   0        0        0       69 2024-02-05 08:00:25.134574 nlp_data-0.3.7/nlp_data/__init__.py
+-rw-r--r--   0        0        0       29 2023-09-07 05:38:28.176112 nlp_data-0.3.7/nlp_data/augment/__init__.py
+-rw-r--r--   0        0        0    12244 2024-04-24 06:48:11.085254 nlp_data-0.3.7/nlp_data/augment/gpt.py
+-rw-r--r--   0        0        0     2665 2023-10-20 09:37:59.968020 nlp_data-0.3.7/nlp_data/cli.py
+-rw-r--r--   0        0        0      186 2023-09-12 23:32:47.410236 nlp_data-0.3.7/nlp_data/document/__init__.py
+-rw-r--r--   0        0        0     3940 2023-11-15 10:30:38.549269 nlp_data-0.3.7/nlp_data/document/api.py
+-rw-r--r--   0        0        0     2111 2023-11-15 12:20:30.863273 nlp_data-0.3.7/nlp_data/document/dialogue.py
+-rw-r--r--   0        0        0     2561 2024-02-02 07:55:00.926673 nlp_data-0.3.7/nlp_data/document/embedding.py
+-rw-r--r--   0        0        0    31950 2024-04-24 07:19:42.076479 nlp_data-0.3.7/nlp_data/document/nlu.py
+-rw-r--r--   0        0        0      323 2024-03-14 07:06:02.430192 nlp_data-0.3.7/nlp_data/storage/__init__.py
+-rw-r--r--   0        0        0      698 2024-02-22 06:16:36.239175 nlp_data-0.3.7/nlp_data/storage/api.py
+-rw-r--r--   0        0        0     4338 2023-10-18 09:35:57.215122 nlp_data-0.3.7/nlp_data/storage/base.py
+-rw-r--r--   0        0        0      737 2023-11-02 03:31:01.217994 nlp_data-0.3.7/nlp_data/storage/dialogue.py
+-rw-r--r--   0        0        0      745 2023-11-02 03:32:52.423265 nlp_data-0.3.7/nlp_data/storage/embdding.py
+-rw-r--r--   0        0        0     1221 2024-03-14 07:04:40.900752 nlp_data-0.3.7/nlp_data/storage/nlu.py
+-rw-r--r--   0        0        0     9732 2023-11-01 10:04:19.272964 nlp_data-0.3.7/nlp_data/storage/s3.py
+-rw-r--r--   0        0        0     2815 2024-03-01 02:59:47.274999 nlp_data-0.3.7/nlp_data/utils.py
+-rw-r--r--   0        0        0      855 2024-03-14 06:12:15.148248 nlp_data-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5661 1970-01-01 00:00:00.000000 nlp_data-0.3.7/PKG-INFO
```

### Comparing `nlp_data-0.3.6/README.md` & `nlp_data-0.3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,7 +123,17 @@
 # 下载文件,当xxx为一个s3中的文件夹时,会下载该文件夹下所有文件
 nlp-data download xxx.xxx --bucket xxx --save_path xxx
 # 上传文件, 当xxx为一个文件夹时,会上传该文件夹下所有文件
 nlp-data upload xxx --bucket xxx
 # 删除文件, 当xxx为一个文件夹时,会删除该文件夹下所有文件
 nlp-data delete xxx --bucket xxx
 ```
+</details>
+
+### 示例
+
+examples文件夹下有一些示例代码,可以参考,下面是翻译中文nlu文档然后保存英文nlu的示例
+
+```python
+python examples/translate_nlu.py --api_key xxx --doc_name schedule/train --save_name schedule/train --num_samples 5000
+```
+上述代码将nlu bucket里面的schedule/train文档翻译成英文,nlu-en bucket中
```

### Comparing `nlp_data-0.3.6/nlp_data/augment/gpt.py` & `nlp_data-0.3.7/nlp_data/augment/gpt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from enum import Enum
 from openai import OpenAI
 import os
 from ..document import NLUDocList, NLUDoc, APIDocList, APIDoc, DialogueDoc, DialogueDocList, APIParam
+from ..document.nlu import Entity
 from ..document.dialogue import Message
+from docarray import DocList
 from pydantic import validate_arguments
 from tqdm import tqdm, trange
 from wasabi import msg
-from typing import Optional
+from typing import List
 
 
 class Localism(str, Enum):
     """方言
     """
     guangdong: str = '广东话'
     sichuan: str = '四川话'
@@ -19,15 +21,15 @@
     
 class GPTAugmentor:
     """基于ChatGPT的数据增强器
     """
     def __init__(self, 
                  api_key: str = None,
                  model: str = 'gpt-3.5-turbo-0613',
-                 api_base: str = 'https://record.pachira.cn/v1'):
+                 api_base: str = 'https://us-pachira-aiproxy.pachira.cn/v1'):
         
         api_key = api_key or os.environ.get('OPENAI_API_KEY')
         if not api_key:
             raise ValueError('请设置OPENAI_API_KEY环境变量')
         self.chat_model = model
         self.client = OpenAI(api_key=api_key, base_url=api_base)
         
@@ -120,15 +122,15 @@
                             assert turns[i+1].startswith('Bot:')
                             message = Message(role='user', content=turns[i][5:])
                             new_doc.conversation.append(message)
                             message = Message(role='assistant', content=turns[i+1][5:])
                             new_doc.conversation.append(message)
                         new_docs.append(new_doc)
                         retry = max_retry
-                    except:
+                    except Exception:
                         msg.fail(f'augment doc {doc.id} fail')
                         retry += 1
         return new_docs
     
     
     
     @validate_arguments
@@ -197,15 +199,15 @@
                         assert turns[i+1].startswith('Bot:')
                         message = Message(role='user', content=turns[i][5:])
                         doc.conversation.append(message)
                         message = Message(role='assistant', content=turns[i+1][5:])
                         doc.conversation.append(message)
                     docs.append(doc)
                     retry = max_retry
-                except:
+                except Exception:  # noqa: E722
                     retry += 1
                     msg.fail(f'generate doc {j} fail. retry {retry}')
                 
         return docs
     
     def translate_nlu_en(self, docs: NLUDocList) -> NLUDocList:
         """将文档的文本翻译为英文
@@ -217,8 +219,43 @@
             translated_text = self.get_chatgpt_response(query=prompt)
             translated_doc = NLUDoc(text=translated_text)
             if doc.domain:
                 translated_doc.set_domain(text=doc.domain.text)
             if doc.intention:
                 translated_doc.set_intention(text=doc.intention.text)
             translated_docs.append(translated_doc)
-        return translated_docs
+        return translated_docs
+    
+    def augment_nlu_prior_ents(self, docs: NLUDocList, prior_ent_labels: List[str], max_retry: int = 5) -> NLUDocList:
+        """为nlu文档添加先验的实体信息,当做外部词典信息的替代方案.
+        """
+        labels = set(docs.traverse_flat("slots__label"))
+        for label in prior_ent_labels:
+            if label not in labels:
+                raise ValueError(f"prior ent label {label} not in docs. all labels: {labels}")
+        prompt_template = """找出下面的文本中的实体信息,并标注实体类型,实体类型包括: {ent_labels}.
+        文本: 
+        {text}
+        
+        要求:
+        
+        1. 以下面的格式返回: [(实体1, 实体1类型), (实体2, 实体2类型), ...]
+        2. 如果没有实体,只返回空列表`[]`,不要返回无用的信息.
+        """
+        for doc in tqdm(docs):
+            prompt = prompt_template.format(ent_labels=prior_ent_labels, text=doc.text)
+            retry = 0
+            while retry < max_retry:
+                try:
+                    response = self.get_chatgpt_response(query=prompt)
+                    ents = eval(response)
+                    if len(ents) == 0:
+                        doc.prior_ents = DocList[Entity]()
+                    else:
+                        for ent, label in ents:
+                            doc.set_prior_ent(text=ent, label=label)
+                    retry = max_retry
+                except Exception as e:
+                    print(e)
+                    msg.fail(f"augment doc {doc.id} fail, retry: {retry} / {max_retry}")
+                    retry += 1
+        return docs
```

### Comparing `nlp_data-0.3.6/nlp_data/cli.py` & `nlp_data-0.3.7/nlp_data/cli.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/document/api.py` & `nlp_data-0.3.7/nlp_data/document/api.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/document/dialogue.py` & `nlp_data-0.3.7/nlp_data/document/dialogue.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/document/embedding.py` & `nlp_data-0.3.7/nlp_data/document/embedding.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/document/nlu.py` & `nlp_data-0.3.7/nlp_data/document/nlu.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     language: Optional[str] = None
     domain: Optional[Domain] = None
     intention: Optional[Intention] = None
     slots: DocList[Entity] = DocList[Entity]()
     abnf_output: Optional[str] = None
     screen: Optional[Literal["driver", "passenger"]] = None
     hicar: Optional[Hicar] = None
+    prior_ents: DocList[Entity] = DocList[Entity]()
     
     @validator('text')
     def validate_text(cls, v: str, values: dict):
         return v.strip().replace('\n', '')
     
     @validator('hicar', always=True)
     def validate_hicar(cls, v: Optional[Hicar], values: dict):
@@ -150,18 +151,22 @@
                 return hicar
             else:
                 return v
             
     @validator('screen', always=True)
     def validate_screen(cls, v: Optional[Literal["driver", "passenger"]], values: dict):
         if v is None:
-            if re.search(r'主驾屏|主驾驶屏幕|主驾驶屏|主驾屏幕|主驾', values['text']):
+            driver_res =  re.search(r'主驾屏|主驾驶屏幕|主驾驶屏|主驾屏幕|主驾', values['text'])
+            passenger_res =  re.search(r'副驾屏|副驾驶屏幕|副驾视屏|副驾屏幕|副驾', values['text'])
+            if driver_res and not passenger_res:
                 return 'driver'
-            elif re.search(r'副驾屏|副驾驶屏幕|副驾视屏|副驾屏幕|副驾', values['text']):
+            elif passenger_res and not driver_res:
                 return 'passenger'
+            else:
+                return v
         else:
             return v
             
     
     @validate_arguments
     def set_slot(self, text: constr(strip_whitespace=True, min_length=1, strict=True), label: Label, indices: Optional[List[Index]] = None, score: Optional[Score] = None):
         if not indices:
@@ -170,14 +175,27 @@
             indices = list(range(start, end))
         slot = Entity(text=text, indices=indices, label=label, score=score)
         if self.slots is None:
             self.slots = DocList[Entity]()
         if slot not in self.slots:
             assert_span_text_in_doc(doc_text=self.text, span_text=text, span_indices=indices)
             self.slots.append(slot)
+            
+    @validate_arguments
+    def set_prior_ent(self, text: constr(strip_whitespace=True, min_length=1), label: Label, indices: Optional[List[Index]] = None, score: Optional[Score] = None):
+        if not indices:
+            start = self.text.index(text)
+            end = start + len(text)
+            indices = list(range(start, end))
+        slot = Entity(text=text, indices=indices, label=label, score=score)
+        if not hasattr(self, 'prior_ents'):
+            self.prior_ents = DocList[Entity]()
+        if slot not in self.prior_ents:
+            assert_span_text_in_doc(doc_text=self.text, span_text=text, span_indices=indices)
+            self.prior_ents.append(slot)
     
     @validate_arguments
     def set_domain(self, text: constr(strip_whitespace=True, min_length=1), score: Optional[Score] = None):
         self.domain = Domain(text=text, score=score)
     
     @validate_arguments
     def set_intention(self, text: constr(strip_whitespace=True, min_length=1), score: Optional[Score] = None):
@@ -249,14 +267,28 @@
         return doc
     
     def __hash__(self) -> int:
         return hash(self.text)
     
     def __eq__(self, __value: object) -> bool:
         return self.text == __value.text
+    
+    def __hasattr__(self, name: str):
+        return name in self.__dict__
+    
+    def __getattr__(self, item: str):
+        if item in self._docarray_fields().keys():
+            if item in  self.__dict__:
+                return self.__dict__[item]
+            else:
+                if item == 'prior_ents':
+                    self.__dict__['prior_ents'] =  DocList[Entity]()
+                    return self.__dict__[item]
+        else:
+            return super().__getattribute__(item)
         
         
 class NLUExample(BaseDoc):
     """存放NLU文档对, 主要用于存放NLU文档对的评估结果
     """
     id: ID = None
     x: NLUDoc
@@ -356,14 +388,54 @@
             for line in tqdm(lines):
                 doc = NLUDoc(text=line)
                 doc.set_domain(text=domain)
                 docs.append(doc)
         return docs
     
     @classmethod
+    def from_ner_dataset(cls, dataset_dir: Union[str, Path]) -> 'NLUDocList':
+        """将NLUDocList.convert_slots_to_ner_dataset保存的数据集转换为NLUDocList
+
+        Args:
+            dataset_dir (Union[str, Path]): 数据集目录
+
+        Raises:
+            ImportError: datasets未安装
+
+        Returns:
+            NLUDocList: NLU文档列表
+        """
+        if not datsets_requirement:
+            raise ImportError('datasets not installed, please install datasets first, pip install datasets')
+        else:
+            from datasets import load_from_disk, DatasetDict, Dataset
+        
+        def convert_to_nlu_doc(example: Dict[str, Any]) -> NLUDoc:
+            text = example['text']
+            doc = NLUDoc(text=text)
+            for ent in example['ents']:
+                doc.set_slot(text=ent['text'], label=ent['label'], indices=ent['indices'])
+            return doc
+        
+        ds = load_from_disk(dataset_dir)
+        if isinstance(ds, DatasetDict):
+            docs = NLUDocList()
+            for split in ['train', 'validation']:
+                if split in ds:
+                    for example in tqdm(ds[split]):
+                        doc = convert_to_nlu_doc(example)
+                        docs.append(doc)
+                else:
+                    print(f'{split}数据集不存在')
+        if isinstance(ds, Dataset):
+            docs = NLUDocList([convert_to_nlu_doc(example) for example in tqdm(ds)])
+        return docs
+                
+    
+    @classmethod
     def from_v1_ner_dataset(cls, file_path: Union[str, Path], end_char: str = '。', split_char: str = '\t') -> 'NLUDocList':
         """将旧版本的NER数据集转换为NLUDocList,需要文件如下格式:
         麻	O
         烦	O
         向	B-VERB
         大	I-VERB
         调	I-VERB
@@ -495,15 +567,17 @@
             raise ImportError('datasets not installed, please install datasets first, pip install datasets')
         else:
             from datasets import Dataset, DatasetDict
         if not pandas_requirement:
             raise ImportError('pandas not installed, please install pandas first, pip install pandas')
         else:
             import pandas as pd
-        data = {'text': self.text, 'ents': [[ent.dict(exclude={"id"}) for ent in ent_ls] for ent_ls in self.slots]}
+        data = {'text': self.text, 
+                'ents': [[ent.dict(exclude={"id"}) for ent in ent_ls] for ent_ls in self.slots],
+                'prior_ents': [[ent.dict(exclude={"id"}) for ent in ent_ls] for ent_ls in self.prior_ents]}
         df = pd.DataFrame(data)
         train_df = df.sample(frac=train_ratio)
         if not split_test:
             val_df = df.drop(train_df.index)
             ds = DatasetDict({'train': Dataset.from_pandas(train_df, preserve_index=False), 'validation': Dataset.from_pandas(val_df, preserve_index=False)})
         else:
             val_ratio = (1 - train_ratio) / 2
```

### Comparing `nlp_data-0.3.6/nlp_data/storage/api.py` & `nlp_data-0.3.7/nlp_data/storage/api.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/storage/base.py` & `nlp_data-0.3.7/nlp_data/storage/base.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/storage/dialogue.py` & `nlp_data-0.3.7/nlp_data/storage/dialogue.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/storage/embdding.py` & `nlp_data-0.3.7/nlp_data/storage/embdding.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/storage/nlu.py` & `nlp_data-0.3.7/nlp_data/storage/nlu.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,8 +23,17 @@
         _ = DocList[NLUDoc].push_stream(docs, url=f's3://{cls.bucket_name}/{name}', show_progress=show_progress)
         return
 
     @classmethod
     def pull_stream(cls, name: str, show_progress: bool = True) -> Iterator[NLUDoc]:
         name = name.strip()
         for doc in DocList[NLUDoc].pull_stream(url=f's3://{cls.bucket_name}/{name}', show_progress=show_progress):
-            yield doc
+            yield doc
+            
+class NLUDocStoreZH(NLUDocStore):
+    
+    bucket_name = 'nlu'
+    
+    
+class NLUDocStoreEN(NLUDocStore):
+    
+    bucket_name = 'nlu-en'
```

### Comparing `nlp_data-0.3.6/nlp_data/storage/s3.py` & `nlp_data-0.3.7/nlp_data/storage/s3.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/nlp_data/utils.py` & `nlp_data-0.3.7/nlp_data/utils.py`

 * *Files identical despite different names*

### Comparing `nlp_data-0.3.6/pyproject.toml` & `nlp_data-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-data"
-version = "0.3.6"
+version = "0.3.7"
 description = "普强内部NLP数据存储分享处理工具"
 authors = ["wang mengdi <wangmengdi@pachiratech.com>"]
 readme = "README.md"
 packages = [{include = "nlp_data"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nlp_data-0.3.6/PKG-INFO` & `nlp_data-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-data
-Version: 0.3.6
+Version: 0.3.7
 Summary: 普强内部NLP数据存储分享处理工具
 Author: wang mengdi
 Author-email: wangmengdi@pachiratech.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -147,8 +147,18 @@
 # 下载文件,当xxx为一个s3中的文件夹时,会下载该文件夹下所有文件
 nlp-data download xxx.xxx --bucket xxx --save_path xxx
 # 上传文件, 当xxx为一个文件夹时,会上传该文件夹下所有文件
 nlp-data upload xxx --bucket xxx
 # 删除文件, 当xxx为一个文件夹时,会删除该文件夹下所有文件
 nlp-data delete xxx --bucket xxx
 ```
+</details>
+
+### 示例
+
+examples文件夹下有一些示例代码,可以参考,下面是翻译中文nlu文档然后保存英文nlu的示例
+
+```python
+python examples/translate_nlu.py --api_key xxx --doc_name schedule/train --save_name schedule/train --num_samples 5000
+```
+上述代码将nlu bucket里面的schedule/train文档翻译成英文,nlu-en bucket中
```

