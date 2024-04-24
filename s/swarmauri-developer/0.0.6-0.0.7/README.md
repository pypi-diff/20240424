# Comparing `tmp/swarmauri_developer-0.0.6.tar.gz` & `tmp/swarmauri_developer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri_developer-0.0.6.tar", last modified: Wed Apr 24 10:45:17 2024, max compression
+gzip compressed data, was "swarmauri_developer-0.0.7.tar", last modified: Wed Apr 24 17:18:57 2024, max compression
```

## Comparing `swarmauri_developer-0.0.6.tar` & `swarmauri_developer-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:45:17.745288 swarmauri_developer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 10:45:17.745288 swarmauri_developer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-24 10:45:06.000000 swarmauri_developer-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:45:17.749288 swarmauri_developer-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 10:45:06.000000 swarmauri_developer-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:45:17.745288 swarmauri_developer-0.0.6/swarmauri_developer/
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-24 10:45:06.000000 swarmauri_developer-0.0.6/swarmauri_developer/DeveloperAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-24 10:45:06.000000 swarmauri_developer-0.0.6/swarmauri_developer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:45:17.745288 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 10:45:17.000000 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 10:45:17.000000 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:45:17.000000 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 10:45:17.000000 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 10:45:17.000000 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 10:45:17.000000 swarmauri_developer-0.0.6/swarmauri_developer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:57.498545 swarmauri_developer-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 17:18:57.498545 swarmauri_developer-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-24 17:18:49.000000 swarmauri_developer-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:18:57.498545 swarmauri_developer-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 17:18:49.000000 swarmauri_developer-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:57.494545 swarmauri_developer-0.0.7/swarmauri_developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-24 17:18:49.000000 swarmauri_developer-0.0.7/swarmauri_developer/DeveloperAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-24 17:18:49.000000 swarmauri_developer-0.0.7/swarmauri_developer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:57.498545 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 17:18:57.000000 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 17:18:57.000000 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:18:57.000000 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 17:18:57.000000 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 17:18:57.000000 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 17:18:57.000000 swarmauri_developer-0.0.7/swarmauri_developer.egg-info/top_level.txt
```

### Comparing `swarmauri_developer-0.0.6/PKG-INFO` & `swarmauri_developer-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri_developer
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter.
 Home-page: http://github.com/swarmauri/developer_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri_developer-0.0.6/README.md` & `swarmauri_developer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `swarmauri_developer-0.0.6/setup.py` & `swarmauri_developer-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `swarmauri_developer-0.0.6/swarmauri_developer/DeveloperAssistant.py` & `swarmauri_developer-0.0.7/swarmauri_developer/DeveloperAssistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,18 @@
         
         with gr.Blocks(css=self.css) as code_interpreter:
             with gr.Row():
                 code_input = gr.Code(language="python", label="Enter your Python code here", elem_id='code-block')
                 output = gr.Textbox(label="Output")
             code_input.change(self.execute_code, inputs=code_input, outputs=output)
 
-        self.app = gr.TabbedInterface([chat_interface_stream, file_explorer, code_interpreter], ["Developer Assistant", "File Explorer", "Code Interpreter"], css=self.css)
+        self.app = gr.TabbedInterface([chat_interface_stream, file_explorer, code_interpreter], 
+            ["Developer Assistant", "File Explorer", "Code Interpreter"], 
+            css=self.css,
+            title="Swarmauri Developer Assistant")
 
     def launch(self):
         self.app.launch(share=True)
 
 def main():
     import argparse
     parser = argparse.ArgumentParser(description="Swarmauri Developer Assistant Command Line Tool")
```

### Comparing `swarmauri_developer-0.0.6/swarmauri_developer/__init__.py` & `swarmauri_developer-0.0.7/swarmauri_developer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __short_desc__ = """The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter."""
 __long_desc__ = """# Swarmauri Developer Assistant
 
 ## Overview
 The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter.
 
 ## Features
 - **AI-Powered Coding Assistance:** Utilize OpenAI's models for real-time coding help and documentation.
 - **File Management Interface:** Navigate and manage your project files within a robust Gradio interface.
 - **Code Execution Environment:** Execute Python code snippets directly from the interface.
 - **Database Integration:** Automatically log interactions in a SQLite database for analysis or record-keeping.
 - **Vector Store Integration:** Efficiently handle and retrieve data using the MLMVectorStore component.
 """
-__cdn__ = "https://cdn.swarmauri.com/assets/developer_assistant/0_0_5_vector_store_data.zip"
+__cdn__ = "https://cdn.swarmauri.com/assets/developer_assistant/0_0_7_vector_store_data.zip"
 __default_vector_store_path__ = "vector_store_data"
```

### Comparing `swarmauri_developer-0.0.6/swarmauri_developer.egg-info/PKG-INFO` & `swarmauri_developer-0.0.7/swarmauri_developer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri_developer
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter.
 Home-page: http://github.com/swarmauri/developer_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

