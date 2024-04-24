# Comparing `tmp/gocodeo-0.0.9.1.tar.gz` & `tmp/gocodeo-0.0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocodeo-0.0.9.1.tar", last modified: Tue Apr  9 03:06:10 2024, max compression
+gzip compressed data, was "gocodeo-0.0.9.2.tar", last modified: Fri Apr 12 07:15:45 2024, max compression
```

## Comparing `gocodeo-0.0.9.1.tar` & `gocodeo-0.0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:06:10.587958 gocodeo-0.0.9.1/
--rw-rw-rw-   0        0        0      809 2024-04-09 03:06:10.582716 gocodeo-0.0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-03 14:58:55.000000 gocodeo-0.0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 03:06:10.549568 gocodeo-0.0.9.1/gocodeo/
--rw-rw-rw-   0        0        0       67 2024-04-04 07:06:34.000000 gocodeo-0.0.9.1/gocodeo/__init__.py
--rw-rw-rw-   0        0        0    27750 2024-04-08 05:16:56.000000 gocodeo-0.0.9.1/gocodeo/generator.py
--rw-rw-rw-   0        0        0     7224 2024-04-08 18:54:13.000000 gocodeo-0.0.9.1/gocodeo/train.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:06:10.582716 gocodeo-0.0.9.1/gocodeo.egg-info/
--rw-rw-rw-   0        0        0      809 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2024-03-03 14:59:37.000000 gocodeo-0.0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 03:06:10.587958 gocodeo-0.0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1255 2024-04-09 03:05:44.000000 gocodeo-0.0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:15:45.579891 gocodeo-0.0.9.2/
+-rw-rw-rw-   0        0        0      809 2024-04-12 07:15:45.578435 gocodeo-0.0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-03 14:58:55.000000 gocodeo-0.0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 07:15:45.559938 gocodeo-0.0.9.2/gocodeo/
+-rw-rw-rw-   0        0        0       67 2024-04-04 07:06:34.000000 gocodeo-0.0.9.2/gocodeo/__init__.py
+-rw-rw-rw-   0        0        0    27780 2024-04-11 19:20:56.000000 gocodeo-0.0.9.2/gocodeo/generator.py
+-rw-rw-rw-   0        0        0     7458 2024-04-12 07:06:19.000000 gocodeo-0.0.9.2/gocodeo/train.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:15:45.577417 gocodeo-0.0.9.2/gocodeo.egg-info/
+-rw-rw-rw-   0        0        0      809 2024-04-12 07:15:45.000000 gocodeo-0.0.9.2/gocodeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-04-12 07:15:45.000000 gocodeo-0.0.9.2/gocodeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:15:45.000000 gocodeo-0.0.9.2/gocodeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-04-12 07:15:45.000000 gocodeo-0.0.9.2/gocodeo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2024-04-12 07:15:45.000000 gocodeo-0.0.9.2/gocodeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 07:15:45.000000 gocodeo-0.0.9.2/gocodeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2024-03-03 14:59:37.000000 gocodeo-0.0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:15:45.580635 gocodeo-0.0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2024-04-12 07:15:17.000000 gocodeo-0.0.9.2/setup.py
```

### Comparing `gocodeo-0.0.9.1/PKG-INFO` & `gocodeo-0.0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gocodeo
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: A package to generate unit tests for a file
 Author: GoCodeo AI
 Description-Content-Type: text/markdown
 Requires-Dist: vertexai
 Requires-Dist: requests
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: google-auth
```

### Comparing `gocodeo-0.0.9.1/gocodeo/generator.py` & `gocodeo-0.0.9.2/gocodeo/generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -215,16 +215,16 @@
 
     if len(choices) == 0:
         raise Exception("Prompt did not return any answer")   
     message = choices[0].get("message", {}).get("content", "")
     # print(message, "message")
  
     return message
-def generate_api_request(code, context, type, number,import_lines,imported_code):
-    prompt = f"You are angularjs unit testing expert. Your job is to write {number} numbers high quality unit test code using jasmine and karma framework only, for given angular code: {code} for the given {type} scenarios in the context: {context}. Strictly go through the context and generate at least {number} numbers high quality unit test code with description including assertions covering all scenarios in one file. Please mock all the services and data where ever necessary. Please Make sure to import all the dependencies at the top for execution of tests & the imports are {import_lines}.Import all these dependencies as per given if they are present.{imported_code}these are the code of imported classes or functions.Take context from here also & try to generate more accurate & executable unit test cases."
+def generate_api_request(code, context, type, number,import_lines,imported_code,src_path,test_path):
+    prompt = f"You are angularjs unit testing expert. Your job is to write {number} numbers high quality unit test code  using jasmine and karma framework only, for given angular code: {code} for the given {type} scenarios in the context: {context}. Strictly go through the context and generate at least {number} numbers high quality unit test code with description including assertions covering all scenarios in one file. Please mock all the services and data where ever necessary. You have to  make sure to import all the necessary dependencies at the top for execution of tests . For your reference the imports are {import_lines} in the source code file present at {src_path} location.Take more information from here also{imported_code},these are the code of imported classes or function which is imported in {import_lines}. It is mandatory that the imported elements generated by you should be valid,precise & accurate as they will be directly used in production. Try to generate more accurate & executable unit test cases.keep in mind that the unit test cases written by you will be written on {test_path} location."
 
     payload = {
         "model": "gpt-3.5-turbo-16k",
         "messages": [
             {
                 "role": "user",
                 "content": prompt
@@ -392,49 +392,36 @@
 
         # Check if the file exists
         if not os.path.exists(file_path):
             print(f"File not found: {file_path}")
             continue
 
         # Read the content of the file
-        with open(file_path, 'r') as file:
+        with open(file_path, 'r', encoding='utf-8') as file:
             file_content = file.read()
 
-            # Split import symbols into individual imports
-            import_symbols_list = [symbol.strip() for symbol in import_symbols.split(',')]
+            # Extract the symbols from the import statement
+            imported_symbols = [sym.strip() for sym in import_symbols.split(',')]
 
-            # Iterate through individual imports
-            for symbol in import_symbols_list:
-                # Check if the imported item is a class or a function
-                is_class = re.search(rf'\bclass\s+{symbol}\b', file_content)
-                is_function = re.search(rf'\bfunction\s+{symbol}\b', file_content)
-
-                # Extract the code of the imported item
-                imported_item_code = None
-                if is_class:
-                    class_code_pattern = rf'\bexport\s+class\s+{symbol}\b[\s\S]*?(?=export\s+class|\Z)'
-                    class_code_match = re.search(class_code_pattern, file_content)
-                    if class_code_match:
-                        imported_item_code = class_code_match.group(0).strip()
-                elif is_function:
-                    function_code_pattern = rf'\bexport\s+function\s+{symbol}\b[\s\S]*?(?=export\s+function|\Z)'
-                    function_code_match = re.search(function_code_pattern, file_content)
-                    if function_code_match:
-                        imported_item_code = function_code_match.group(0).strip()
+            # Construct the regular expression pattern to match export statements for the imported symbols
+            export_pattern = r'\b(?:export\s+(?:class|function|const|interface|type|enum)\s+(?:' + '|'.join(imported_symbols) + r')\b[\s\S]*?)(?=\n\s*export\s+(?:class|function|const|interface|type|enum)|\Z)'
 
-                if imported_item_code:
-                    imported_code.append(imported_item_code)
-                else:
-                    print(f"Class or function '{symbol}' not found in file: {file_path}")
+            # Find all export statements for the imported symbols using regex
+            export_statements = re.findall(export_pattern, file_content)
+
+            # Add the matched export statements to the imported code list
+            for statement in export_statements:
+                # Remove trailing comments from the matched export statement
+                cleaned_export_statement = re.sub(r'/\*.*?\*/', '', statement, flags=re.DOTALL)
+                imported_code.append(cleaned_export_statement.strip())
 
     # Join all the imported code strings into a single string
     all_imported_code = '\n\n'.join(imported_code)
 
     return all_imported_code
-
 # for gettting code of happy path & negative cases scenarios
 def generate_tests(file_name):
     try:
         with open(file_name, 'r', encoding='utf-8') as file:
             file_content = file.read()
 
             file_size = os.path.getsize(file_name)
@@ -490,18 +477,18 @@
 
                             directory_path = os.path.dirname(file_name)
                             test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
                             function_test_folder_path = os.path.join(test_folder_path, function_name)
                             output_file_path = os.path.join(function_test_folder_path, f'test_{function_name}_{type}.spec.ts')
 
                             retrived_context=fetch_imported_code(new_imports,function_test_folder_path)
-                            # print(retrived_context)
+                            print(retrived_context)
                                 
 
-                            test_response = generate_api_request(function_code, api_response, obj['type'], obj['number'],import_lines,retrived_context)
+                            test_response = generate_api_request(function_code, api_response, obj['type'], obj['number'],import_lines,retrived_context,file_name,output_file_path)
                             test_response1 = generate_api_request1(function_code, test_response,obj['type'], obj['number'])
         
                         
                             if test_response1:
                                 directory_path = os.path.dirname(file_name)
                                 test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
                                 os.makedirs(test_folder_path,exist_ok=True)
@@ -519,14 +506,15 @@
                                 match = re.search(combined_pattern, test_response1, re.DOTALL)
 
                                 if match:
                                     content = match.group(1) or match.group(2) or match.group(3) or match.group(4)
                                     content=content.strip()
                                 else:
                                     content=test_response1
+                                new_imports=extract_user_defined_imports(content)
                                 updated_code=replace_string_imports(content, new_imports)
                                 with open(output_file_path, 'w') as output_file:
                                     output_file.write(updated_code)
                                     print(f"Test cases for '{function_name}' written to {output_file_path}")
                             else:
                                 print(f"Failed to fetch test cases from API for function '{function_name}'.")        
                             
@@ -547,17 +535,17 @@
                         api_response = open_api_request(file_content, obj['type'], obj['number'], explain_response)
                     
                         directory_path = os.path.dirname(file_name)
                         test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
                         output_file_path = os.path.join(test_folder_path, f'test_{File_name}_{type}.spec.ts')
 
                         retrived_context=fetch_imported_code(new_imports,test_folder_path)
-                        # print(retrived_context)
+                        print(retrived_context)
 
-                        test_response = generate_api_request(file_content, api_response, obj['type'], obj['number'],import_lines,retrived_context)
+                        test_response = generate_api_request(file_content, api_response, obj['type'], obj['number'],import_lines,retrived_context,file_name,output_file_path)
                         
                         test_response1 = generate_api_request1(file_content, test_response,obj['type'], obj['number'])  
                         if test_response1:
 
                             directory_path = os.path.dirname(file_name)
                             test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
                             os.makedirs(test_folder_path,exist_ok=True)
@@ -573,14 +561,15 @@
                             match = re.search(combined_pattern, test_response1, re.DOTALL)
 
                             if match:
                                 content = match.group(1) or match.group(2) or match.group(3) or match.group(4)
                                 content=content.strip()
                             else:
                                 content=test_response1
+                            new_imports=extract_user_defined_imports(content)
                             updated_code=replace_string_imports(content, new_imports)
                             with open(output_file_path, 'w') as output_file:
                                 output_file.write(updated_code)
                                 print(f"Test cases on '{type}' scenarios written to file:{output_file_path}")
                         else:
                             print(f"Failed to fetch test cases from API for function '{function_name}'.")        
             else:
```

### Comparing `gocodeo-0.0.9.1/gocodeo/train.py` & `gocodeo-0.0.9.2/gocodeo/train.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,20 +69,21 @@
                     continue
                 if '.git' in dirs:
                     dirs.remove('.git')  # Skip .git directory and its contents
                     continue
                 for file in files:
                     file_path = os.path.join(root, file)
                     zipf.write(file_path, os.path.relpath(file_path, directory))
-
+    
     zip_filename = os.path.basename(directory) + ".zip"  # Name of the zip file will be the current directory name
 
     # Create a temporary directory to copy files, excluding node_modules and .git
     temp_dir = os.path.join(directory, "__temp_zip_dir__")
     shutil.copytree(directory, temp_dir, ignore=shutil.ignore_patterns('node_modules', '.git', zip_filename))
+    
 
     # Animation: Print "Training started" with animation dots
     
 
     zip_directory(temp_dir, zip_filename)
 
     # Clean up the temporary directory
@@ -116,41 +117,49 @@
     animation_stop_event = threading.Event()
 
     # Fetch the current working directory
     current_dir = os.getcwd()
 
     # Extract the directory name from the current directory path
     dir_name = os.path.basename(os.path.normpath(current_dir))
-
+    temp_name=dir_name
+    if '.' in temp_name:
+        dir_name = dir_name.replace('.', '_')
+    
     # Sanitize the directory name to adhere to bucket naming rules
     bucket_name = dir_name.lower().replace(" ", "-")
+    
 
     # Ensure the bucket name meets length requirements
     bucket_name = bucket_name[:63]+"-gocodeo"
     # print(bucket_name)
 
     # Create the bucket
     create_bucket(bucket_name)
 
     # Start animation thread
     animation_thread = threading.Thread(target=start_animation)
     animation_thread.start()
 
     # Create a zip file of the directory contents
-    zip_file_path = os.path.join(current_dir, f'{dir_name}.zip')
+    zip_file_path = os.path.join(current_dir, f'{temp_name}.zip')
+    
 
     # Zip the directory contents
     zip_directory_with_exclusions(current_dir)
 
     # Stop animation
     
     animation_stop_event.set()
     animation_thread.join()
     # Upload the zip file to the bucket
-    upload_file(bucket_name, zip_file_path, f'{dir_name}.zip')
+    if '.' in temp_name:
+        upload_file(bucket_name, zip_file_path, f'{dir_name}.zip')
+    else:
+        upload_file(bucket_name, zip_file_path, f'{temp_name}.zip')
 
     # Remove the zip file from the local filesystem
     os.remove(zip_file_path)
     
     print("Training Completed")
 
 if __name__ == "__main__":
```

### Comparing `gocodeo-0.0.9.1/gocodeo.egg-info/PKG-INFO` & `gocodeo-0.0.9.2/gocodeo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gocodeo
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: A package to generate unit tests for a file
 Author: GoCodeo AI
 Description-Content-Type: text/markdown
 Requires-Dist: vertexai
 Requires-Dist: requests
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: google-auth
```

### Comparing `gocodeo-0.0.9.1/setup.py` & `gocodeo-0.0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gocodeo',
-    version='0.0.9.1',
+    version='0.0.9.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'gocodeo-generate = gocodeo.generator:generate_tests_cli',
             'gocodeo-train = gocodeo.train:start'
         
         ]
```

