# Comparing `tmp/mergecraft-0.0.2.tar.gz` & `tmp/mergecraft-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergecraft-0.0.2.tar", last modified: Sat Aug 19 00:17:30 2023, max compression
+gzip compressed data, was "mergecraft-0.0.3.tar", last modified: Wed Apr 24 04:25:23 2024, max compression
```

## Comparing `mergecraft-0.0.2.tar` & `mergecraft-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-19 00:17:30.452825 mergecraft-0.0.2/
--rw-rw-rw-   0        0        0     1105 2023-08-16 16:20:24.000000 mergecraft-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      910 2023-08-19 00:17:30.451821 mergecraft-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-08-18 19:05:10.000000 mergecraft-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-19 00:17:30.440822 mergecraft-0.0.2/mergecraft/
--rw-rw-rw-   0        0        0        0 2023-08-18 17:33:08.000000 mergecraft-0.0.2/mergecraft/__init__.py
--rw-rw-rw-   0        0        0     5970 2023-08-19 00:14:47.000000 mergecraft-0.0.2/mergecraft/mergecraft.py
-drwxrwxrwx   0        0        0        0 2023-08-19 00:17:30.449822 mergecraft-0.0.2/mergecraft.egg-info/
--rw-rw-rw-   0        0        0      910 2023-08-19 00:17:30.000000 mergecraft-0.0.2/mergecraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-08-19 00:17:30.000000 mergecraft-0.0.2/mergecraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-19 00:17:30.000000 mergecraft-0.0.2/mergecraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-19 00:17:30.000000 mergecraft-0.0.2/mergecraft.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-08-19 00:17:30.000000 mergecraft-0.0.2/mergecraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-19 00:17:30.000000 mergecraft-0.0.2/mergecraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-19 00:17:30.452825 mergecraft-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-08-19 00:16:55.000000 mergecraft-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:23.785180 mergecraft-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 04:25:13.000000 mergecraft-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 04:25:23.785180 mergecraft-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 04:25:13.000000 mergecraft-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:23.785180 mergecraft-0.0.3/mergecraft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-24 04:25:13.000000 mergecraft-0.0.3/mergecraft/mergecraft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:25:23.785180 mergecraft-0.0.3/mergecraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 04:25:23.000000 mergecraft-0.0.3/mergecraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:25:23.785180 mergecraft-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 04:25:13.000000 mergecraft-0.0.3/setup.py
```

### Comparing `mergecraft-0.0.2/LICENSE` & `mergecraft-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 José Ângelo da Silva Nery
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 José Ângelo da Silva Nery
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mergecraft-0.0.2/mergecraft/mergecraft.py` & `mergecraft-0.0.3/mergecraft/mergecraft.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,171 +1,179 @@
-import os
-import tempfile
-import subprocess
-import pathspec
-import argparse
-import re
-
-
-def find_subdir(start_dir, subdir_name):
-    """Recursively search for a subdirectory within the start directory."""
-    for dirpath, dirnames, filenames in os.walk(start_dir):
-        for dirname in dirnames:
-            if subdir_name in dirname:
-                # print(f"Found directory: {os.path.join(dirpath, dirname)}")  # Debug
-                return os.path.join(dirpath, dirname)
-    # print(
-    #     f"Directory '{subdir_name}' not found from starting point: {start_dir}"
-    # )  # Debug
-    return None
-
-
-def read_file_content(filepath):
-    """Read the content of a file."""
-    with open(filepath, "rb") as file:
-        content_bytes = file.read()
-        content = content_bytes.decode("utf-8", errors="replace")
-        return content if content.strip() else "(empty)"
-
-
-def load_gitignore():
-    """Load the .gitignore specifications."""
-    with open(".gitignore", "r") as f:
-        gitignore = f.readlines()
-    return pathspec.PathSpec.from_lines("gitwildmatch", gitignore)
-
-
-def should_skip_directory(dirpath):
-    """Return True if the directory should be skipped based on certain criteria."""
-    skip_directories = ["bin", "obj", ".git"]
-    for skip_dir in skip_directories:
-        if skip_dir in dirpath.split(os.path.sep):
-            return True
-    return False
-
-
-def main():
-    # Parse command-line arguments
-    parser = argparse.ArgumentParser(
-        description="Merge files into a temporary file and open in VS Code."
-    )
-    parser.add_argument(
-        "-e",
-        "--extensions",
-        nargs="+",
-        default=None,  # Default para None, vamos tratar isso mais adiante
-        help="Specify the file extensions to process.",
-    )
-    parser.add_argument(
-        "--path",
-        default=".",
-        help="Specify the root path to start searching for files. Defaults to current directory.",
-    )
-    parser.add_argument(
-        "--filter",
-        help="A regex pattern to filter files based on their content or name. Only files matching this pattern will be included.",
-    )
-    args = parser.parse_args()
-
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
-    if args.extensions is None:
-        args.extensions = [".py"]
-
-    # Normalize the path and check if it exists
-    current_dir = os.getcwd()
-    full_path = os.path.normpath(os.path.join(current_dir, args.path))
-    if not os.path.exists(full_path):
-        # If the path doesn't exist directly, try to find it recursively
-        full_path = find_subdir(current_dir, args.path)
-
-    if not full_path or not os.path.exists(full_path):
-        print(
-            f"Error: The specified path '{args.path}' was not found in '{current_dir}' or its subdirectories!"
-        )
-        return
-
-    # Create a temporary file with a meaningful prefix
-    with tempfile.NamedTemporaryFile(prefix="mergecraft_", delete=False) as temp_file:
-        temp_path = temp_file.name
-
-    gitignore_spec = load_gitignore() if os.path.exists(".gitignore") else None
-
-    read_files = []
-    total_line_count = 0
-
-    for dirpath, dirnames, filenames in os.walk(full_path):
-        # Debug
-        # print(f"Checking directory: {dirpath}")
-
-        # Ignore the .git directory
-        if ".git" in dirpath:
-            # print("Skipping .git directory")  # Debug
-            continue
-
-        for filename in filenames:
-            # Filter by extensions
-            if not filename.endswith(tuple(args.extensions)):
-                continue
-
-            filepath = os.path.join(dirpath, filename)
-            relative_filepath = os.path.relpath(filepath)
-
-            # print(f"Checking file: {filepath}")  # Debug
-
-            # Check against gitignore rules
-            if gitignore_spec and gitignore_spec.match_file(relative_filepath):
-                # print(f"File {filepath} is ignored due to .gitignore rules.")  # Debug
-                continue  # Skip this file
-
-            # Apply the filter to both filename and content
-            content = read_file_content(filepath)
-            if args.filter and not (
-                re.search(args.filter, content) or re.search(args.filter, filename)
-            ):
-                # print(f"File {filepath} does not match the provided filter.")  # Debug
-                continue
-
-            line_count = len(content.split("\n"))
-            total_line_count += line_count
-            read_files.append((relative_filepath, line_count))
-
-            with open(temp_path, "a", encoding="utf-8") as temp_file:
-                temp_file.write(f"``` {filename}\n{content}\n```\n\n")
-
-    print("Editing in VS Code. Close to continue.")
-    subprocess.run(["cmd", "/c", "code", "-w", temp_path])
-
-    if not read_files:
-        print("No files were read!")
-        return
-
-    print("Editing completed. Continuing script execution...")
-    print("\nSummary:")
-    print(f"Total files read: {len(read_files)}")
-    print(f"Total lines: {total_line_count}")
-    print("\nFiles read:")
-    for file_path, line_count in read_files:
-        print(f"{file_path}: {line_count} lines")
-
-    os.remove(temp_path)
-
-
-if __name__ == "__main__":
-    main()
+import os
+import tempfile
+import subprocess
+import pathspec
+import argparse
+import re
+
+
+def find_subdir(start_dir, subdir_name):
+    """Recursively search for a subdirectory within the start directory."""
+    for dirpath, dirnames, filenames in os.walk(start_dir):
+        for dirname in dirnames:
+            if subdir_name in dirname:
+                # print(f"Found directory: {os.path.join(dirpath, dirname)}")  # Debug
+                return os.path.join(dirpath, dirname)
+    # print(
+    #     f"Directory '{subdir_name}' not found from starting point: {start_dir}"
+    # )  # Debug
+    return None
+
+
+def read_file_content(filepath):
+    """Read the content of a file."""
+    with open(filepath, "rb") as file:
+        content_bytes = file.read()
+        content = content_bytes.decode("utf-8", errors="replace")
+        return content if content.strip() else "(empty)"
+
+
+def load_gitignore():
+    """Load the .gitignore specifications."""
+    with open(".gitignore", "r") as f:
+        gitignore = f.readlines()
+    return pathspec.PathSpec.from_lines("gitwildmatch", gitignore)
+
+
+def should_skip_directory(dirpath):
+    """Return True if the directory should be skipped based on certain criteria."""
+    skip_directories = ["bin", "obj", ".git"]
+    for skip_dir in skip_directories:
+        if skip_dir in dirpath.split(os.path.sep):
+            return True
+    return False
+
+
+def main():
+    # Parse command-line arguments
+    parser = argparse.ArgumentParser(
+        description="Merge files into a temporary file and open in VS Code."
+    )
+    parser.add_argument(
+        "-e",
+        "--extensions",
+        nargs="+",
+        default=None,  # Default para None, vamos tratar isso mais adiante
+        help="Specify the file extensions to process.",
+    )
+    parser.add_argument(
+        "--path",
+        default=".",
+        help="Specify the root path to start searching for files. Defaults to current directory.",
+    )
+    parser.add_argument(
+        "--filter",
+        help="A regex pattern to filter files based on their content or name. Only files matching this pattern will be included.",
+    )
+    args = parser.parse_args()
+
+    # Se --path for fornecido e --extensions não for, leremos todos os arquivos
+    if args.path != "." and args.extensions is None:
+        args.extensions = [""]
+    elif args.filter != "" and args.extensions is None:
+        args.extensions = [""]
+    elif (
+        args.extensions is None
+    ):  # Se --extensions não for fornecido, vamos usar .py como padrão
+        args.extensions = [".py"]
+
+    # Validate Regex
+    if args.filter:
+        try:
+            re.compile(args.filter)
+        except re.error:
+            print("Error: Invalid regular expression provided!")
+            return
+
+    # If no extensions are explicitly provided, default to .py
+    if args.extensions is None:
+        args.extensions = [".py"]
+
+    # Normalize the path and check if it exists
+    current_dir = os.getcwd()
+    full_path = os.path.normpath(os.path.join(current_dir, args.path))
+    if not os.path.exists(full_path):
+        # If the path doesn't exist directly, try to find it recursively
+        full_path = find_subdir(current_dir, args.path)
+
+    if not full_path or not os.path.exists(full_path):
+        print(
+            f"Error: The specified path '{args.path}' was not found in '{current_dir}' or its subdirectories!"
+        )
+        return
+
+    # Create a temporary file with a meaningful prefix
+    with tempfile.NamedTemporaryFile(prefix="mergecraft_", delete=False) as temp_file:
+        temp_path = temp_file.name
+
+    gitignore_spec = load_gitignore() if os.path.exists(".gitignore") else None
+
+    read_files = []
+    total_line_count = 0
+
+    for dirpath, dirnames, filenames in os.walk(full_path):
+        # Debug
+        # print(f"Checking directory: {dirpath}")
+
+        # Ignore the .git directory
+        if ".git" in dirpath:
+            # print("Skipping .git directory")  # Debug
+            continue
+
+        for filename in filenames:
+            if filename.startswith("_"):
+                continue
+
+            # Check if filename is .gitignore
+            if filename in [".gitignore", "LICENSE", "README.md", "__init__.py"]:
+                continue
+
+            # Filter by extensions
+            if not filename.endswith(tuple(args.extensions)):
+                continue
+
+            filepath = os.path.join(dirpath, filename)
+            relative_filepath = os.path.relpath(filepath)
+
+            # Check against gitignore rules
+            if gitignore_spec and gitignore_spec.match_file(relative_filepath):
+                # print(f"File {filepath} is ignored due to .gitignore rules.")
+                continue
+
+            # Apply the filter to both filename and content
+            content = read_file_content(filepath)
+            if args.filter and not (
+                re.search(args.filter, content) or re.search(args.filter, filename)
+            ):
+                # print(f"File {filepath} does not match the provided filter.")  # Debug
+                continue
+
+            line_count = len(content.split("\n"))
+            total_line_count += line_count
+            read_files.append((relative_filepath, line_count))
+
+            with open(filepath, "r", encoding="utf-8") as original_file:
+                content = original_file.read()
+
+            with open(temp_path, "a", encoding="utf-8") as temp_file:
+                temp_file.write(f"# {filepath}\n{content}\n")
+
+    print("Editing in VS Code. Close to continue.")
+    subprocess.run(["cmd", "/c", "code", "-w", temp_path])
+
+    if not read_files:
+        print("No files were read!")
+        return
+
+    print("Editing completed. Continuing script execution...")
+    print("\nSummary:")
+    print(f"Total files read: {len(read_files)}")
+    print(f"Total lines: {total_line_count}")
+    print("\nFiles read:")
+    for file_path, line_count in read_files:
+        print(f"{file_path}: {line_count} lines")
+
+    os.remove(temp_path)
+
+
+if __name__ == "__main__":
+    main()
```

