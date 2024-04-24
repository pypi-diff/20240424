# Comparing `tmp/dseqmap4nlp-0.0.2.tar.gz` & `tmp/dseqmap4nlp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dseqmap4nlp-0.0.2.tar", last modified: Fri Apr 19 19:32:47 2024, max compression
+gzip compressed data, was "dseqmap4nlp-0.0.3.tar", last modified: Wed Apr 24 01:07:49 2024, max compression
```

## Comparing `dseqmap4nlp-0.0.2.tar` & `dseqmap4nlp-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:47.219865 dseqmap4nlp-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-19 19:32:47.219865 dseqmap4nlp-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:32:47.219865 dseqmap4nlp-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:47.215865 dseqmap4nlp-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:47.219865 dseqmap4nlp-0.0.2/src/dseqmap4nlp/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/annotationset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/basemapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/charmapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/labelloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/raggedmapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-19 19:32:43.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp/spacymapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:47.219865 dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-19 19:32:47.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 19:32:47.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:47.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 19:32:47.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 19:32:47.000000 dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:07:49.445458 dseqmap4nlp-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-24 01:07:49.445458 dseqmap4nlp-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:07:49.445458 dseqmap4nlp-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:07:49.441458 dseqmap4nlp-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:07:49.441458 dseqmap4nlp-0.0.3/src/dseqmap4nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/annotationset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/basemapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/charmapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/labelloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/raggedmapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-24 01:07:44.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp/spacymapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:07:49.445458 dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-24 01:07:49.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 01:07:49.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:07:49.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 01:07:49.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 01:07:49.000000 dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/top_level.txt
```

### Comparing `dseqmap4nlp-0.0.2/LICENSE` & `dseqmap4nlp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dseqmap4nlp-0.0.2/PKG-INFO` & `dseqmap4nlp-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dseqmap4nlp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small tool to parse and process annotated text corpora
 Author-email: Johann Frei <johann_frei@yahoo.de>
 Project-URL: Homepage, https://github.com/j-frei/DSeqMap4NLP
 Project-URL: Issues, https://github.com/j-frei/DSeqMap4NLP/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,27 +35,44 @@
         (6,8, "b")
     ]}
 ]
 
 for sample in samples:
     text = sample["text"]
     anns = sample["label"]
+    # Mapper @ Chars <-> SpaCy Tokens
     mapper = SpacySequenceMapper(text, nlp="de")
+    # (trivial) Mapper @ Chars <-> Chars
     charmapper = CharSequenceMapper(text=text)
 
+    # Load annotation data
+    # assuming the format: [ (start_idx, stop_idx, label_class), ...]
+    # and merge it with to a certain (char <-> discrete sequence) mapper
     annotationset = LabelLoader.from_text_spans(anns, mapper)
+    
+    # Determine number fo overlaps
     print("Overlaps:", annotationset.countOverlaps())
 
+    # Apply the following transformations to the annotation data:
+    # - transform char-based labels onto discretized sequence items (e.g. tokens)
+    #   -> Expand if a label's char bounds are not exactly at token bounds
+    # - Remove shorter spans in case of overlapping spans
+    #   -> Note: New overlaps could also be introduced by span expansion!
     filtered_spans = annotationset\
         .toDSeqSpans(strategy=["expand"])\
         .withoutOverlaps(strategy="prefer_longest", merge_same_classes=True)
+
+    # Check overlaps again (No overlap should exist anymore!)
     print("Overlaps:", filtered_spans.countOverlaps())
 
+    # Transform annotation data into IOB2-formatted sequence.
     print("Sequence:")
     print(filtered_spans.toFormattedSequence(schema="IOB2"))
-    print("Previous sequence:")
+
+    # Try to generate an IOB2 sequence with overlaps. (It should fail!)
+    print("Previous sequence (should fail):")
     try:
         # Should raise an error...
         print(annotationset.toFormattedSequence(schema="IOB2"))
-    except Exception as e:
+    except ValueError as e:
         print("Error raised: " + repr(e))
 ```
```

### Comparing `dseqmap4nlp-0.0.2/README.md` & `dseqmap4nlp-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -18,27 +18,44 @@
         (6,8, "b")
     ]}
 ]
 
 for sample in samples:
     text = sample["text"]
     anns = sample["label"]
+    # Mapper @ Chars <-> SpaCy Tokens
     mapper = SpacySequenceMapper(text, nlp="de")
+    # (trivial) Mapper @ Chars <-> Chars
     charmapper = CharSequenceMapper(text=text)
 
+    # Load annotation data
+    # assuming the format: [ (start_idx, stop_idx, label_class), ...]
+    # and merge it with to a certain (char <-> discrete sequence) mapper
     annotationset = LabelLoader.from_text_spans(anns, mapper)
+    
+    # Determine number fo overlaps
     print("Overlaps:", annotationset.countOverlaps())
 
+    # Apply the following transformations to the annotation data:
+    # - transform char-based labels onto discretized sequence items (e.g. tokens)
+    #   -> Expand if a label's char bounds are not exactly at token bounds
+    # - Remove shorter spans in case of overlapping spans
+    #   -> Note: New overlaps could also be introduced by span expansion!
     filtered_spans = annotationset\
         .toDSeqSpans(strategy=["expand"])\
         .withoutOverlaps(strategy="prefer_longest", merge_same_classes=True)
+
+    # Check overlaps again (No overlap should exist anymore!)
     print("Overlaps:", filtered_spans.countOverlaps())
 
+    # Transform annotation data into IOB2-formatted sequence.
     print("Sequence:")
     print(filtered_spans.toFormattedSequence(schema="IOB2"))
-    print("Previous sequence:")
+
+    # Try to generate an IOB2 sequence with overlaps. (It should fail!)
+    print("Previous sequence (should fail):")
     try:
         # Should raise an error...
         print(annotationset.toFormattedSequence(schema="IOB2"))
-    except Exception as e:
+    except ValueError as e:
         print("Error raised: " + repr(e))
 ```
```

### Comparing `dseqmap4nlp-0.0.2/pyproject.toml` & `dseqmap4nlp-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dseqmap4nlp"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Johann Frei", email="johann_frei@yahoo.de" },
 ]
 description = "A small tool to parse and process annotated text corpora"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp/annotationset.py` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp/annotationset.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,16 +174,14 @@
             if self.mapper.getText() != mapper.getText():
                 raise Exception("Text of mappers do not match.")
         else:
             print("Cannot validate text of annotation data because no previous mapper was set.", file=sys.stderr)
         return AnnotationSet(self.entries, self.level, mapper)
 
     def toFormattedSequence(self, schema: Literal["IOB2", "plain"] = "IOB2"):
-        if self.level != "dseq":
-            raise ValueError("Convert to dseq spans first.")
         if self.mapper is None:
             raise ValueError("No mapper is set.")
         if not schema in ["IOB2", "plain"]:
             raise ValueError("Unknown schema: {}, one of {}".format(
                 schema,
                 ["IOB2", "plain"]
             ))
@@ -214,8 +212,9 @@
 
     def toEntities(self, with_text: bool = None):
         if self.entries is None:
             raise ValueError("Entries are None.")
         if with_text:
             if self.mapper is None:
                 raise ValueError("No mapper assigned.")
-            {"text": self.mapper.getText(), "label": self.entries}
+            return {"text": self.mapper.getText(), "label": self.entries}
+        return self.entries
```

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp/basemapper.py` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp/basemapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         text_start = self.seq2txt[start]
         # use end of previous dseq entry
         text_stop = self.seq2txt[stop-1] + len(self.dseq[stop-1])
         return (text_start, text_stop)
 
 
-    def mapTextSpanToDSeqSpan(self, text_span: tuple[int,int], mode: Literal["strict", "contract", "expand"] = "strict") -> Optional[Tuple[int,int]]:
+    def mapTextSpanToDSeqSpan(self, text_span: Tuple[int,int], mode: Literal["strict", "contract", "expand"] = "strict") -> Optional[Tuple[int,int]]:
         if mode not in ["strict", "contract", "expand"]:
             raise ValueError("Unknown mode {}. Use one of: {}".format(
                 repr(mode),
                 repr(["strict", "contract", "expand"])
             ))
 
         start, stop = text_span
```

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp/charmapper.py` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp/charmapper.py`

 * *Files identical despite different names*

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp/labelloader.py` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp/labelloader.py`

 * *Files identical despite different names*

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp/raggedmapper.py` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp/raggedmapper.py`

 * *Files identical despite different names*

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp/spacymapper.py` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp/spacymapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import sys
 import spacy
 from spacy.language import Language
+from typing import Union
 from dseqmap4nlp import BaseMapper
 
 class SpacySequenceMapper(BaseMapper):
     spacy_cache = {}
 
-    def __init__(self, text: str, nlp: str | Language = None):
+    def __init__(self, text: str, nlp: Union[str, Language] = None):
         if text is None:
             raise ValueError("Parameter text is None.")
 
         if nlp is None:
             print("Assuming English NLP object...", file=sys.stderr)
             nlp = "en"
```

### Comparing `dseqmap4nlp-0.0.2/src/dseqmap4nlp.egg-info/PKG-INFO` & `dseqmap4nlp-0.0.3/src/dseqmap4nlp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dseqmap4nlp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small tool to parse and process annotated text corpora
 Author-email: Johann Frei <johann_frei@yahoo.de>
 Project-URL: Homepage, https://github.com/j-frei/DSeqMap4NLP
 Project-URL: Issues, https://github.com/j-frei/DSeqMap4NLP/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,27 +35,44 @@
         (6,8, "b")
     ]}
 ]
 
 for sample in samples:
     text = sample["text"]
     anns = sample["label"]
+    # Mapper @ Chars <-> SpaCy Tokens
     mapper = SpacySequenceMapper(text, nlp="de")
+    # (trivial) Mapper @ Chars <-> Chars
     charmapper = CharSequenceMapper(text=text)
 
+    # Load annotation data
+    # assuming the format: [ (start_idx, stop_idx, label_class), ...]
+    # and merge it with to a certain (char <-> discrete sequence) mapper
     annotationset = LabelLoader.from_text_spans(anns, mapper)
+    
+    # Determine number fo overlaps
     print("Overlaps:", annotationset.countOverlaps())
 
+    # Apply the following transformations to the annotation data:
+    # - transform char-based labels onto discretized sequence items (e.g. tokens)
+    #   -> Expand if a label's char bounds are not exactly at token bounds
+    # - Remove shorter spans in case of overlapping spans
+    #   -> Note: New overlaps could also be introduced by span expansion!
     filtered_spans = annotationset\
         .toDSeqSpans(strategy=["expand"])\
         .withoutOverlaps(strategy="prefer_longest", merge_same_classes=True)
+
+    # Check overlaps again (No overlap should exist anymore!)
     print("Overlaps:", filtered_spans.countOverlaps())
 
+    # Transform annotation data into IOB2-formatted sequence.
     print("Sequence:")
     print(filtered_spans.toFormattedSequence(schema="IOB2"))
-    print("Previous sequence:")
+
+    # Try to generate an IOB2 sequence with overlaps. (It should fail!)
+    print("Previous sequence (should fail):")
     try:
         # Should raise an error...
         print(annotationset.toFormattedSequence(schema="IOB2"))
-    except Exception as e:
+    except ValueError as e:
         print("Error raised: " + repr(e))
 ```
```

