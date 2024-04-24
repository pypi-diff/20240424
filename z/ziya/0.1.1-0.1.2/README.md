# Comparing `tmp/ziya-0.1.1.tar.gz` & `tmp/ziya-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.1.tar", max compression
+gzip compressed data, was "ziya-0.1.2.tar", max compression
```

## Comparing `ziya-0.1.1.tar` & `ziya-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.1/LICENSE
--rw-r--r--   0        0        0     1714 2024-04-22 03:21:31.982461 ziya-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.1/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.1/app/agents/__init__.py
--rw-r--r--   0        0        0     4181 2024-04-22 03:14:43.793669 ziya-0.1.1/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.1/app/agents/prompts.py
--rw-r--r--   0        0        0     1359 2024-04-22 03:14:43.793879 ziya-0.1.1/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.1/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.1/app/utils/__init__.py
--rw-r--r--   0        0        0     2132 2024-04-22 03:14:43.794161 ziya-0.1.1/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.1/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.1/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.1/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      716 2024-04-22 03:16:37.495159 ziya-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-22 03:14:43.795533 ziya-0.1.1/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.1/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.1/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.1/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-22 03:14:43.796168 ziya-0.1.1/templates/index.html
--rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 ziya-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1714 2024-04-24 04:42:40.757902 ziya-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.2/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.2/app/agents/__init__.py
+-rw-r--r--   0        0        0     4266 2024-04-24 04:42:40.748800 ziya-0.1.2/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.2/app/agents/prompts.py
+-rw-r--r--   0        0        0     1688 2024-04-24 04:42:40.748995 ziya-0.1.2/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.2/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.2/app/utils/__init__.py
+-rw-r--r--   0        0        0     2278 2024-04-24 04:42:40.749189 ziya-0.1.2/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.2/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.2/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.2/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      716 2024-04-24 04:43:41.685380 ziya-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.2/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.2/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.2/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.2/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.2/templates/index.html
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 ziya-0.1.2/PKG-INFO
```

### Comparing `ziya-0.1.1/LICENSE` & `ziya-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/README.md` & `ziya-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/app/agents/agent.py` & `ziya-0.1.2/app/agents/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,42 +43,41 @@
 
 def get_combined_document_contents() -> str:
     user_codebase_dir: str = os.environ["ZIYA_USER_CODEBASE_DIR"]
     print(f"Reading user's current codebase: {user_codebase_dir}")
 
     combined_contents: str = ""
     ignored_patterns: List[str] = get_ignored_patterns(user_codebase_dir)
-    all_files: List[str] = get_complete_file_list(user_codebase_dir, ignored_patterns)
+    included_relative_dirs = [pattern.strip() for pattern in os.environ.get("ZIYA_ADDITIONAL_INCLUDE_DIRS", "").split(',')]
+    all_files: List[str] = get_complete_file_list(user_codebase_dir, ignored_patterns, included_relative_dirs)
 
     print_file_tree(all_files)
 
     seen_dirs: Set[str] = set()
     for file_path in all_files:
         try:
             docs = TextLoader(file_path).load()
             for doc in docs:
                 combined_contents += f"File: {file_path}\n{doc.page_content}\n\n"
             dir_path = os.path.dirname(file_path)
             if dir_path not in seen_dirs:
-                # print_file_tree(dir_path, ignored_patterns)
                 seen_dirs.add(dir_path)
         except Exception as e:
             print(f"Skipping file {file_path} due to error: {e}")
 
     print("--------------------------------------------------------")
     print(f"Ignoring following paths based on gitIgnore and other defaults: {ignored_patterns}")
     print("--------------------------------------------------------")
     print(f"Codebase word count: {len(combined_contents.split()):,}")
     token_count = len(tiktoken.get_encoding("cl100k_base").encode(combined_contents))
     print(f"Codebase token count: {token_count:,}")
     print(f"Max Claude Token limit: 200,000")
     print("--------------------------------------------------------")
     return combined_contents
 
-
 def get_child_paths(directory: str) -> Generator[str, None, None]:
     for entry in os.listdir(directory):
         child_path = os.path.join(directory, entry)
         yield child_path
 
 
 prompt = conversational_prompt.partial(
```

### Comparing `ziya-0.1.1/app/agents/prompts.py` & `ziya-0.1.2/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/app/main.py` & `ziya-0.1.2/app/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 
 def main():
     os.environ["ZIYA_USER_CODEBASE_DIR"] = os.getcwd()
 
     parser = argparse.ArgumentParser(description="Run with custom options")
     parser.add_argument("--exclude", default=[], type=lambda x: x.split(','),
                         help="List of files or directories to exclude (e.g., --exclude 'tst,build,*.py')")
+    parser.add_argument("--include-dirs", default=[], type=lambda x: x.split(','),
+                        help="List of directories to include (e.g., --include 'src,static')")
     parser.add_argument("--profile", type=str, default=None,
                         help="AWS profile to use (e.g., --profile ziya)")
     parser.add_argument("--model", type=str, choices=["sonnet", "haiku", "opus"], default="haiku",
                         help="AWS Bedrock Model to use  (e.g., --model sonnet)")
     parser.add_argument("--port", type=int, default=6969,
                         help="Port number to run Ziya frontend on (e.g., --port 8080)")
     args = parser.parse_args()
 
     additional_excluded_dirs = ','.join([item for item in args.exclude])
     os.environ["ZIYA_ADDITIONAL_EXCLUDE_DIRS"] = additional_excluded_dirs
 
+    additional_included_dirs = ','.join([item for item in args.include_dirs])
+    os.environ["ZIYA_ADDITIONAL_INCLUDE_DIRS"] = additional_included_dirs
+
     if args.profile:
         os.environ["ZIYA_AWS_PROFILE"] = args.profile
     if args.model:
         os.environ["ZIYA_AWS_MODEL"] = args.model
 
     langchain_serve_directory = os.path.dirname(os.path.abspath(__file__))
     os.chdir(langchain_serve_directory)
     serve(port=args.port)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `ziya-0.1.1/app/server.py` & `ziya-0.1.2/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/app/utils/directory_util.py` & `ziya-0.1.2/app/utils/directory_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 
         return patterns
 
     ignored_patterns.extend(get_patterns_recursive(directory))
     return ignored_patterns
 
 
-def get_complete_file_list(user_codebase_dir: str, ignored_patterns: List[str]) -> List[str]:
+def get_complete_file_list(user_codebase_dir: str, ignored_patterns: List[str], included_relative_dirs: List[str]) -> List[str]:
     should_ignore = parse_gitignore_patterns(ignored_patterns, base_dir=user_codebase_dir)
     file_set: Set[str] = set()
-
-    for root, dirs, files in os.walk(user_codebase_dir):
-        # Filter out ignored directories
-        dirs[:] = [d for d in dirs if not should_ignore(os.path.join(root, d))]
-
-        for file in files:
-            file_path = os.path.join(root, file)
-            if not should_ignore(file_path):
-                file_set.add(file_path)
+    for pattern in included_relative_dirs:
+        for root, dirs, files in os.walk(os.path.normpath(os.path.join(user_codebase_dir, pattern))):
+            # Filter out ignored directories
+            dirs[:] = [d for d in dirs if not should_ignore(os.path.join(root, d))]
+
+            for file in files:
+                file_path = os.path.join(root, file)
+                if not should_ignore(file_path):
+                    file_set.add(file_path)
 
     return list(file_set)
```

### Comparing `ziya-0.1.1/app/utils/gitignore_parser.py` & `ziya-0.1.2/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/app/utils/print_tree_util.py` & `ziya-0.1.2/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/pyproject.toml` & `ziya-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.1/static/app.js` & `ziya-0.1.2/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/static/favicon.ico` & `ziya-0.1.2/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/static/sendPayload.js` & `ziya-0.1.2/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/static/ziya.css` & `ziya-0.1.2/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/templates/index.html` & `ziya-0.1.2/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.1/PKG-INFO` & `ziya-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

