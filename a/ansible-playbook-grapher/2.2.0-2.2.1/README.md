# Comparing `tmp/ansible_playbook_grapher-2.2.0-py2.py3-none-any.whl.zip` & `tmp/ansible_playbook_grapher-2.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 51198 bytes, number of entries: 18
--rw-r--r--  2.0 unx       60 b- defN 24-Apr-21 18:32 ansibleplaybookgrapher/__init__.py
+Zip file size: 51197 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-24 18:39 ansibleplaybookgrapher/__init__.py
 -rw-r--r--  2.0 unx    12252 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/cli.py
 -rw-r--r--  2.0 unx    15624 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/graph_model.py
 -rw-r--r--  2.0 unx     2679 b- defN 24-Mar-23 05:55 ansibleplaybookgrapher/grapher.py
 -rw-r--r--  2.0 unx    20440 b- defN 24-Apr-21 17:53 ansibleplaybookgrapher/parser.py
 -rw-r--r--  2.0 unx     7031 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/utils.py
 -rw-r--r--  2.0 unx      358 b- defN 23-May-11 14:42 ansibleplaybookgrapher/data/graph.css
 -rw-r--r--  2.0 unx     5458 b- defN 23-May-11 14:42 ansibleplaybookgrapher/data/highlight-hover.js
 -rw-r--r--  2.0 unx     8709 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/renderer/__init__.py
--rw-r--r--  2.0 unx    13229 b- defN 24-Apr-18 20:30 ansibleplaybookgrapher/renderer/mermaid.py
+-rw-r--r--  2.0 unx    13225 b- defN 24-Apr-24 18:39 ansibleplaybookgrapher/renderer/mermaid.py
 -rw-r--r--  2.0 unx    12104 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/renderer/graphviz/__init__.py
 -rw-r--r--  2.0 unx     7367 b- defN 23-May-13 12:42 ansibleplaybookgrapher/renderer/graphviz/postprocessor.py
--rw-r--r--  2.0 unx    35148 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    23247 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1745 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/RECORD
-18 files, 165661 bytes uncompressed, 48260 bytes compressed:  70.9%
+-rw-r--r--  2.0 unx    35148 b- defN 24-Apr-24 18:44 ansible_playbook_grapher-2.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23247 b- defN 24-Apr-24 18:44 ansible_playbook_grapher-2.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-24 18:44 ansible_playbook_grapher-2.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-24 18:44 ansible_playbook_grapher-2.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-24 18:44 ansible_playbook_grapher-2.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1745 b- defN 24-Apr-24 18:44 ansible_playbook_grapher-2.2.1.dist-info/RECORD
+18 files, 165657 bytes uncompressed, 48259 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: ansibleplaybookgrapher/renderer/graphviz/__init__.py
 Comment: 
 
 Filename: ansibleplaybookgrapher/renderer/graphviz/postprocessor.py
 Comment: 
 
-Filename: ansible_playbook_grapher-2.2.0.dist-info/LICENSE
+Filename: ansible_playbook_grapher-2.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: ansible_playbook_grapher-2.2.0.dist-info/METADATA
+Filename: ansible_playbook_grapher-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: ansible_playbook_grapher-2.2.0.dist-info/WHEEL
+Filename: ansible_playbook_grapher-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: ansible_playbook_grapher-2.2.0.dist-info/entry_points.txt
+Filename: ansible_playbook_grapher-2.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ansible_playbook_grapher-2.2.0.dist-info/top_level.txt
+Filename: ansible_playbook_grapher-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ansible_playbook_grapher-2.2.0.dist-info/RECORD
+Filename: ansible_playbook_grapher-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ansibleplaybookgrapher/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 __prog__ = "ansible-playbook-grapher"
```

## ansibleplaybookgrapher/renderer/mermaid.py

```diff
@@ -141,15 +141,15 @@
         }
 
         compressed = zlib.compress(json.dumps(graph_state).encode("utf-8"), level=9)
 
         url_path = f'pako:{urlsafe_b64encode(compressed).decode("utf-8")}'
         url = f"https://mermaid.live/edit#{url_path}"
 
-        display.display(f"Mermaid live editor URL: {url}")
+        display.vvv(f"Mermaid live editor URL: {url}")
 
         # Display url using the default browser in a new tag
         webbrowser.open(url, new=2)
 
 
 class MermaidFlowChartPlaybookBuilder(PlaybookBuilder):
     def __init__(
```

## Comparing `ansible_playbook_grapher-2.2.0.dist-info/LICENSE` & `ansible_playbook_grapher-2.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ansible_playbook_grapher-2.2.0.dist-info/METADATA` & `ansible_playbook_grapher-2.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ansible-playbook-grapher
-Version: 2.2.0
+Version: 2.2.1
 Summary: A command line tool to create a graph representing your Ansible playbook tasks and roles
 Home-page: https://github.com/haidaraM/ansible-playbook-grapher
-Download-URL: https://github.com/haidaraM/ansible-playbook-grapher/archive/v2.2.0.tar.gz
+Download-URL: https://github.com/haidaraM/ansible-playbook-grapher/archive/v2.2.1.tar.gz
 Author: HAIDARA Mohamed El Mouctar
 Author-email: elmhaidara@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ansible-core <2.16.5,>=2.15
+Requires-Dist: ansible-core <2.16.6,>=2.15
 Requires-Dist: graphviz <1,>=0.18
 Requires-Dist: colour <1
 Requires-Dist: lxml <6
 Requires-Dist: svg.path <7
 
 # Ansible Playbook Grapher
```

