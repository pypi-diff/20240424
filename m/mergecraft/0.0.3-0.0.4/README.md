# Comparing `tmp/mergecraft-0.0.3.tar.gz` & `tmp/mergecraft-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergecraft-0.0.3.tar", last modified: Wed Apr 24 04:25:23 2024, max compression
+gzip compressed data, was "mergecraft-0.0.4.tar", last modified: Wed Apr 24 10:00:54 2024, max compression
```

## Comparing `mergecraft-0.0.3.tar` & `mergecraft-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:23.785180 mergecraft-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 04:25:13.000000 mergecraft-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 04:25:23.785180 mergecraft-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 04:25:13.000000 mergecraft-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:23.785180 mergecraft-0.0.3/mergecraft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/gitignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/mergecraft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:23.785180 mergecraft-0.0.3/mergecraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:25:23.785180 mergecraft-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 04:25:13.000000 mergecraft-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:54.239794 mergecraft-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:00:43.000000 mergecraft-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-24 10:00:54.239794 mergecraft-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-24 10:00:43.000000 mergecraft-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:54.235794 mergecraft-0.0.4/mergecraft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:43.000000 mergecraft-0.0.4/mergecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:00:43.000000 mergecraft-0.0.4/mergecraft/mergecraft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:54.235794 mergecraft-0.0.4/mergecraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:00:54.239794 mergecraft-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 10:00:43.000000 mergecraft-0.0.4/setup.py
```

### Comparing `mergecraft-0.0.3/LICENSE` & `mergecraft-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.3/mergecraft/mergecraft.py` & `mergecraft-0.0.4/mergecraft/mergecraft.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,159 @@
 import os
 import tempfile
 import subprocess
 import pathspec
 import argparse
 import re
+import yaml
+
+
+def default_config():
+    """Return the default configuration."""
+    return {
+        "extensions": [".py", ".txt"],
+        "skip_files": [".gitignore", "LICENSE", "README.md", "__init__.py", "_*"],
+        "skip_directories": ["bin", "obj", ".git"],
+    }
+
+
+def save_default_config(config_path):
+    """Save the default configuration to a YAML file."""
+    with open(config_path, "w") as file:
+        yaml.dump(default_config(), file, default_flow_style=False)
+
+
+def load_config():
+    """Load configuration from a YAML file or create it if it doesn't exist."""
+    config_path = os.path.join(os.getcwd(), "mergecraft.config.yml")
+    if not os.path.exists(config_path):
+        save_default_config(config_path)
+    with open(config_path, "r") as file:
+        return yaml.safe_load(file)
+
+
+config = load_config()
 
 
 def find_subdir(start_dir, subdir_name):
     """Recursively search for a subdirectory within the start directory."""
     for dirpath, dirnames, filenames in os.walk(start_dir):
         for dirname in dirnames:
             if subdir_name in dirname:
-                # print(f"Found directory: {os.path.join(dirpath, dirname)}")  # Debug
                 return os.path.join(dirpath, dirname)
-    # print(
-    #     f"Directory '{subdir_name}' not found from starting point: {start_dir}"
-    # )  # Debug
     return None
 
 
 def read_file_content(filepath):
     """Read the content of a file."""
     with open(filepath, "rb") as file:
         content_bytes = file.read()
         content = content_bytes.decode("utf-8", errors="replace")
         return content if content.strip() else "(empty)"
 
 
 def load_gitignore():
     """Load the .gitignore specifications."""
-    with open(".gitignore", "r") as f:
-        gitignore = f.readlines()
-    return pathspec.PathSpec.from_lines("gitwildmatch", gitignore)
+    gitignore_path = os.path.join(os.getcwd(), ".gitignore")
+    if os.path.exists(gitignore_path):
+        with open(gitignore_path, "r") as f:
+            gitignore = f.readlines()
+        return pathspec.PathSpec.from_lines("gitwildmatch", gitignore)
+    return None
 
 
-def should_skip_directory(dirpath):
-    """Return True if the directory should be skipped based on certain criteria."""
-    skip_directories = ["bin", "obj", ".git"]
-    for skip_dir in skip_directories:
-        if skip_dir in dirpath.split(os.path.sep):
+def should_skip_filename(filename):
+    """Check if file should be skipped based on config."""
+    for pattern in config["skip_files"]:
+        if re.match(pattern.replace("*", ".*"), filename):
             return True
     return False
 
 
+def should_skip_directory(dirpath):
+    """Return True if the directory should be skipped based on config."""
+    return any(
+        skip_dir in dirpath.split(os.path.sep)
+        for skip_dir in config["skip_directories"]
+    )
+
+
 def main():
-    # Parse command-line arguments
     parser = argparse.ArgumentParser(
         description="Merge files into a temporary file and open in VS Code."
     )
     parser.add_argument(
         "-e",
         "--extensions",
         nargs="+",
-        default=None,  # Default para None, vamos tratar isso mais adiante
+        default=config.get("extensions", [".py"]),
         help="Specify the file extensions to process.",
     )
     parser.add_argument(
         "--path",
         default=".",
         help="Specify the root path to start searching for files. Defaults to current directory.",
     )
     parser.add_argument(
         "--filter",
-        help="A regex pattern to filter files based on their content or name. Only files matching this pattern will be included.",
+        help="A regex pattern to filter files based on their content or name.",
     )
     args = parser.parse_args()
 
-    # Se --path for fornecido e --extensions não for, leremos todos os arquivos
-    if args.path != "." and args.extensions is None:
-        args.extensions = [""]
-    elif args.filter != "" and args.extensions is None:
-        args.extensions = [""]
-    elif (
-        args.extensions is None
-    ):  # Se --extensions não for fornecido, vamos usar .py como padrão
-        args.extensions = [".py"]
-
-    # Validate Regex
-    if args.filter:
-        try:
-            re.compile(args.filter)
-        except re.error:
-            print("Error: Invalid regular expression provided!")
-            return
-
-    # If no extensions are explicitly provided, default to .py
     if args.extensions is None:
-        args.extensions = [".py"]
+        print("No file extensions provided; no files will be processed.")
+        return
 
-    # Normalize the path and check if it exists
-    current_dir = os.getcwd()
-    full_path = os.path.normpath(os.path.join(current_dir, args.path))
+    full_path = os.path.normpath(os.path.join(os.getcwd(), args.path))
     if not os.path.exists(full_path):
-        # If the path doesn't exist directly, try to find it recursively
-        full_path = find_subdir(current_dir, args.path)
+        full_path = find_subdir(os.getcwd(), args.path)
 
     if not full_path or not os.path.exists(full_path):
-        print(
-            f"Error: The specified path '{args.path}' was not found in '{current_dir}' or its subdirectories!"
-        )
+        print(f"Error: The specified path '{args.path}' was not found.")
         return
 
-    # Create a temporary file with a meaningful prefix
     with tempfile.NamedTemporaryFile(prefix="mergecraft_", delete=False) as temp_file:
         temp_path = temp_file.name
 
-    gitignore_spec = load_gitignore() if os.path.exists(".gitignore") else None
-
+    gitignore_spec = load_gitignore()
     read_files = []
     total_line_count = 0
 
     for dirpath, dirnames, filenames in os.walk(full_path):
-        # Debug
-        # print(f"Checking directory: {dirpath}")
-
-        # Ignore the .git directory
-        if ".git" in dirpath:
-            # print("Skipping .git directory")  # Debug
+        if ".git" in dirpath or should_skip_directory(dirpath):
             continue
 
         for filename in filenames:
-            if filename.startswith("_"):
-                continue
-
-            # Check if filename is .gitignore
-            if filename in [".gitignore", "LICENSE", "README.md", "__init__.py"]:
+            if should_skip_filename(filename):
                 continue
 
-            # Filter by extensions
-            if not filename.endswith(tuple(args.extensions)):
+            if not any(filename.endswith(ext) for ext in args.extensions):
                 continue
 
             filepath = os.path.join(dirpath, filename)
-            relative_filepath = os.path.relpath(filepath)
-
-            # Check against gitignore rules
-            if gitignore_spec and gitignore_spec.match_file(relative_filepath):
-                # print(f"File {filepath} is ignored due to .gitignore rules.")
+            if gitignore_spec and gitignore_spec.match_file(
+                os.path.relpath(filepath, start=os.getcwd())
+            ):
                 continue
 
-            # Apply the filter to both filename and content
             content = read_file_content(filepath)
             if args.filter and not (
                 re.search(args.filter, content) or re.search(args.filter, filename)
             ):
-                # print(f"File {filepath} does not match the provided filter.")  # Debug
                 continue
 
             line_count = len(content.split("\n"))
             total_line_count += line_count
-            read_files.append((relative_filepath, line_count))
+            read_files.append((filepath, line_count))
 
             with open(filepath, "r", encoding="utf-8") as original_file:
-                content = original_file.read()
+                file_content = original_file.read()
 
             with open(temp_path, "a", encoding="utf-8") as temp_file:
-                temp_file.write(f"# {filepath}\n{content}\n")
+                temp_file.write(f"# {filepath}\n{file_content}\n")
 
     print("Editing in VS Code. Close to continue.")
     subprocess.run(["cmd", "/c", "code", "-w", temp_path])
 
     if not read_files:
         print("No files were read!")
         return
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mergecraft-0.0.3/setup.py` & `mergecraft-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mergecraft",
-    version="0.0.3",
+    version="0.0.4",
     description="A command-line tool to merge files into a temporary file and open in VS Code.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="José Nery",
     author_email="josenerydev@gmail.com",
     url="https://github.com/josenerydev/mergecraft",
     packages=find_packages(),
```

