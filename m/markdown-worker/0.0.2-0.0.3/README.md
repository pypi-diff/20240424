# Comparing `tmp/markdown_worker-0.0.2.tar.gz` & `tmp/markdown_worker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_worker-0.0.2.tar", last modified: Thu Jul 27 06:10:31 2023, max compression
+gzip compressed data, was "markdown_worker-0.0.3.tar", last modified: Wed Apr 24 16:02:20 2024, max compression
```

## Comparing `markdown_worker-0.0.2.tar` & `markdown_worker-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-27 06:10:31.244736 markdown_worker-0.0.2/
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1073 2023-07-26 09:18:13.000000 markdown_worker-0.0.2/LICENSE
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1785 2023-07-27 06:10:31.244620 markdown_worker-0.0.2/PKG-INFO
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1222 2023-07-27 06:09:38.000000 markdown_worker-0.0.2/README.md
-drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-27 06:10:31.243733 markdown_worker-0.0.2/markdown_worker/
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)       58 2023-07-26 09:56:36.000000 markdown_worker-0.0.2/markdown_worker/__init__.py
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     5357 2023-07-27 05:59:02.000000 markdown_worker-0.0.2/markdown_worker/markdown_worker.py
-drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-27 06:10:31.244428 markdown_worker-0.0.2/markdown_worker.egg-info/
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1785 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/PKG-INFO
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)      283 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/SOURCES.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)        1 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/dependency_links.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)        6 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/requires.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)       16 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/top_level.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)       38 2023-07-27 06:10:31.244773 markdown_worker-0.0.2/setup.cfg
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1084 2023-07-27 06:05:54.000000 markdown_worker-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:02:20.857853 markdown_worker-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 16:02:16.000000 markdown_worker-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-24 16:02:20.857853 markdown_worker-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-24 16:02:16.000000 markdown_worker-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:02:20.857853 markdown_worker-0.0.3/markdown_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 16:02:16.000000 markdown_worker-0.0.3/markdown_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-24 16:02:16.000000 markdown_worker-0.0.3/markdown_worker/markdown_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:02:20.857853 markdown_worker-0.0.3/markdown_worker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-24 16:02:20.000000 markdown_worker-0.0.3/markdown_worker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 16:02:20.000000 markdown_worker-0.0.3/markdown_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:02:20.000000 markdown_worker-0.0.3/markdown_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 16:02:20.000000 markdown_worker-0.0.3/markdown_worker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 16:02:20.000000 markdown_worker-0.0.3/markdown_worker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:02:20.857853 markdown_worker-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-24 16:02:16.000000 markdown_worker-0.0.3/setup.py
```

### Comparing `markdown_worker-0.0.2/LICENSE` & `markdown_worker-0.0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Mantresh Khurana
+Copyright (c) 2024 Mantresh Khurana
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `markdown_worker-0.0.2/markdown_worker/markdown_worker.py` & `markdown_worker-0.0.3/markdown_worker/markdown_worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import re
 
 class MarkdownParser:
     def __init__(self, filename=None):
         self.filename = filename
         self.markdown_text = self.read_markdown_file() if filename else ""
 
+        self.lines = self.markdown_text.split('\n')
+
     def read_markdown_file(self):
         if self.filename and self.filename.endswith('.md'):
-            with open(self.filename, 'r', encoding='utf-8') as file:
-                markdown_text = file.read()
+            try:
+                with open(self.filename, 'r', encoding='utf-8') as file:
+                    markdown_text = file.read()
                 return markdown_text
+            except IOError:
+                return "Error: unable to read the markdown file."
         else:
-            return "File is not a Markdown file."
+            return "Error: file is not a markdown file."
 
     def extract_headers_and_paragraphs(self):
         header_pattern = r'^#{1,6}\s(.+)$'
         paragraph_pattern = r'^([^#\n].+)$'
 
         headers = []
         paragraphs = []
         header_indices = []
 
-        lines = self.markdown_text.split('\n')
-        for index, line in enumerate(lines):
+        for index, line in enumerate(self.lines):
             header_match = re.match(header_pattern, line)
             paragraph_match = re.match(paragraph_pattern, line)
             
             if header_match:
                 headers.append(header_match.group(1))
                 header_indices.append(index)
             elif paragraph_match:
@@ -39,81 +43,75 @@
 
         if heading_to_search in headers:
             heading_index = headers.index(heading_to_search)
             start_index = header_indices[heading_index]
             if heading_index + 1 < len(header_indices):
                 end_index = header_indices[heading_index + 1]
             else:
-                end_index = len(self.markdown_text.split('\n'))
+                end_index = len(self.lines)
 
-            content = '\n'.join(self.markdown_text.split('\n')[start_index:end_index])
+            content = '\n'.join(self.lines[start_index:end_index])
             result = content
         else:
-            result = "Heading not found in the Markdown file."
+            result = "Heading not found in the markdown file."
 
         return result
     
     def read_complete_file(self):
         return self.markdown_text
     
     def read_line(self, line_number):
-        lines = self.markdown_text.split('\n')
-        if line_number < len(lines):
-            return lines[line_number]
+        if line_number < len(self.lines):
+            return self.lines[line_number]
         else:
             return "Line number out of range."
         
     def read_word(self, line_number, word_number):
-        lines = self.markdown_text.split('\n')
-        if line_number < len(lines):
-            words = lines[line_number].split(' ')
+        if line_number < len(self.lines):
+            words = self.lines[line_number].split(' ')
             if word_number < len(words):
                 return words[word_number]
             else:
                 return "Word number out of range."
         else:
             return "Line number out of range."
         
     def read_character(self, line_number, word_number, character_number):
-        lines = self.markdown_text.split('\n')
-        if line_number < len(lines):
-            words = lines[line_number].split(' ')
+        if line_number < len(self.lines):
+            words = self.lines[line_number].split(' ')
             if word_number < len(words):
                 characters = list(words[word_number])
                 if character_number < len(characters):
                     return characters[character_number]
                 else:
                     return "Character number out of range."
             else:
                 return "Word number out of range."
         else:
             return "Line number out of range."
         
     def read_character_from_line(self, line_number, character_number):
-        lines = self.markdown_text.split('\n')
-        if line_number < len(lines):
-            characters = list(lines[line_number])
+        if line_number < len(self.lines):
+            characters = list(self.lines[line_number])
             if character_number < len(characters):
                 return characters[character_number]
             else:
                 return "Character number out of range."
         else:
             return "Line number out of range."
         
     def read_character_from_file(self, character_number):
-        characters = list(self.markdown_text)
-        if character_number < len(characters):
-            return characters[character_number]
+        if character_number < len(self.markdown_text):
+            return self.markdown_text[character_number]
         else:
             return "Character number out of range."
         
     def read_word_from_line(self, line_number, word_number):
-        lines = self.markdown_text.split('\n')
-        if line_number < len(lines):
-            words = lines[line_number].split(' ')
+        if line_number < len(self.lines):
+            words = self.lines[line_number].split(' ')
             if word_number < len(words):
                 return words[word_number]
             else:
                 return "Word number out of range."
         else:
             return "Line number out of range."
 
@@ -129,12 +127,14 @@
 
         markdown_text = re.sub(r'^\d+\.\s(.*)$', r'<li>\1</li>', markdown_text, flags=re.MULTILINE)
         markdown_text = re.sub(r'(<li>.*<\/li>)+', r'<ol>\g<0></ol>', markdown_text)
 
         markdown_text = re.sub(r'`([^`]+)`', r'<code>\1</code>', markdown_text)
 
         if output_filename:
-            with open(output_filename, 'w', encoding='utf-8') as output_file:
-                output_file.write(markdown_text)
+            try:
+                with open(output_filename, 'w', encoding='utf-8') as output_file:
+                    output_file.write(markdown_text)
+            except IOError:
+                return "Error: unable to write to the output file."
 
         return markdown_text
-
```

### Comparing `markdown_worker-0.0.2/setup.py` & `markdown_worker-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A simple markdown parsing package.'
-LONG_DESCRIPTION = 'A package that allows to parse, read and write markdown files.'
+LONG_DESCRIPTION = 'Markdown Worker is a versatile Python module for parsing, reading, and writing Markdown files. It simplifies the process of working with Markdown documents by providing a convenient interface for common tasks.'
 
 # Setting up
 setup(
-    name="markdown_worker",
+    name="markdown-worker",
     version=VERSION,
     author="Mantresh Khurana",
     author_email="<mantreshkhurana@spyxpo.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
@@ -27,8 +27,8 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

