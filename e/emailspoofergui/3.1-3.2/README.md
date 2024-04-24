# Comparing `tmp/emailspoofergui-3.1.tar.gz` & `tmp/emailspoofergui-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailspoofergui-3.1.tar", last modified: Wed Apr  3 08:34:51 2024, max compression
+gzip compressed data, was "emailspoofergui-3.2.tar", last modified: Wed Apr 24 08:59:16 2024, max compression
```

## Comparing `emailspoofergui-3.1.tar` & `emailspoofergui-3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.661453 emailspoofergui-3.1/
--rw-r--r--   0 kali      (1000) kali      (1000)     1076 2024-04-03 08:34:32.000000 emailspoofergui-3.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-04-03 08:34:51.661453 emailspoofergui-3.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1160 2024-04-03 08:34:32.000000 emailspoofergui-3.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.657453 emailspoofergui-3.1/emailspoofergui/
--rw-r--r--   0 kali      (1000) kali      (1000)      143 2024-04-03 08:34:32.000000 emailspoofergui-3.1/emailspoofergui/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.661453 emailspoofergui-3.1/emailspoofergui/data/
--rw-r--r--   0 kali      (1000) kali      (1000)      112 2024-04-03 08:34:32.000000 emailspoofergui-3.1/emailspoofergui/data/config.json
--rw-r--r--   0 kali      (1000) kali      (1000)     5428 2024-04-03 08:34:32.000000 emailspoofergui-3.1/emailspoofergui/emailspoofergui.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.661453 emailspoofergui-3.1/emailspoofergui.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      358 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       79 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-03 08:34:51.661453 emailspoofergui-3.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1145 2024-04-03 08:34:32.000000 emailspoofergui-3.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-24 08:59:16.894779 emailspoofergui-3.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1076 2024-04-24 08:58:11.000000 emailspoofergui-3.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-04-24 08:59:16.890779 emailspoofergui-3.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1160 2024-04-24 08:58:11.000000 emailspoofergui-3.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-24 08:59:16.890779 emailspoofergui-3.2/emailspoofergui/
+-rw-r--r--   0 kali      (1000) kali      (1000)      143 2024-04-24 08:58:11.000000 emailspoofergui-3.2/emailspoofergui/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-24 08:59:16.890779 emailspoofergui-3.2/emailspoofergui/data/
+-rw-r--r--   0 kali      (1000) kali      (1000)      112 2024-04-24 08:58:11.000000 emailspoofergui-3.2/emailspoofergui/data/config.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     6998 2024-04-24 08:58:11.000000 emailspoofergui-3.2/emailspoofergui/emailspoofergui.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-24 08:59:16.890779 emailspoofergui-3.2/emailspoofergui.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-04-24 08:59:16.000000 emailspoofergui-3.2/emailspoofergui.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      358 2024-04-24 08:59:16.000000 emailspoofergui-3.2/emailspoofergui.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-04-24 08:59:16.000000 emailspoofergui-3.2/emailspoofergui.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       79 2024-04-24 08:59:16.000000 emailspoofergui-3.2/emailspoofergui.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-04-24 08:59:16.000000 emailspoofergui-3.2/emailspoofergui.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2024-04-24 08:59:16.000000 emailspoofergui-3.2/emailspoofergui.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-24 08:59:16.894779 emailspoofergui-3.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1145 2024-04-24 08:58:11.000000 emailspoofergui-3.2/setup.py
```

### Comparing `emailspoofergui-3.1/LICENSE` & `emailspoofergui-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emailspoofergui-3.1/PKG-INFO` & `emailspoofergui-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailspoofergui
-Version: 3.1
+Version: 3.2
 Summary: A graphical email spoofing tool
 Home-page: https://github.com/IMApurbo/emailspoofergui
 Author: AKM Korishee Apurbo
 Author-email: bandinvisible8@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emailspoofergui-3.1/README.md` & `emailspoofergui-3.2/README.md`

 * *Files identical despite different names*

### Comparing `emailspoofergui-3.1/emailspoofergui/emailspoofergui.py` & `emailspoofergui-3.2/emailspoofergui/emailspoofergui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 import subprocess
 import json
 import pkg_resources
 import os
 import customtkinter as ctk
 from CTkMessagebox import CTkMessagebox
+from tkinter import filedialog
+
 
 def send_email():
     # Function to send the email
     def send():
         sender_name = sender_entry.get()
         receiver_email = receiver_entry.get()
         subject = subject_entry.get()
         message = message_entry.get("1.0", "end-1c")
+        attachment = attachment_entry.get()
+        tls = tls_var.get()
 
-        sendemail_command = f"sendemail -xu {config['username']} -xp {config['password']} -s {config['smtp_server']} -f '{sender_name}' -t {receiver_email} -u '{subject}' -m '{message}'"
+        sendemail_command = f"sendemail -xu {config['username']} -xp {config['password']} -s {config['smtp_server']} -o tls={tls} -f '{sender_name}' -t {receiver_email} -u '{subject}' -m '{message}'"
+        
+        if attachment:
+            sendemail_command += f" -a '{attachment}'"
 
         try:
             subprocess.run(sendemail_command, shell=True, check=True)
             CTkMessagebox(title="Success", message="Email sent successfully!", icon="info", option_1="ok")
         except subprocess.CalledProcessError as e:
             CTkMessagebox(title="Error", message=f"\n{e}", icon="warning", option_1="ok")
 
+    def select_attachment():
+        filename = filedialog.askopenfilename()
+        if filename:  # Check if a file was selected
+            basename = os.path.basename(filename)  # Extract the filename from the full path
+            attachment_entry.delete(0, ctk.END)
+            attachment_entry.insert(0, basename)  # Display only the filename
+            attachment_entry.filename = filename  # Store the full path in a new attribute
+
 
     # Function to open dialog box to edit config
     def edit_config():
         edit_window = ctk.CTkToplevel(root)
         edit_window.title("Edit Configuration")
 
         # Read configuration from file
@@ -48,15 +63,15 @@
             config = load_config()
 
         save_button = ctk.CTkButton(edit_window, text="Save", command=save_config)
         save_button.grid(row=1, column=0, pady=10)
 
     root = ctk.CTk()
     root.title("Email Spoofer from AKM KORISHEE APURBO")
-    root.geometry("800x500+500+0")
+    root.geometry("800x550+500+0")
     root.resizable(False, False)
 
     # Read configuration from file
     global config
     config = load_config()
 
     if config:
@@ -86,16 +101,37 @@
 
         message_label = ctk.CTkLabel(root, text="Message:  ",font=("Latin Modern Mono Slanted", 16))
         message_label.grid(row=4, column=0, sticky="w")
 
         message_entry = ctk.CTkTextbox(root, width=600, height=250,font=("TeX Gyre Pagella", 14,"bold"))
         message_entry.grid(row=4, column=1, sticky="e")
 
+        # Add attachment entry and button
+        attachment_label = ctk.CTkLabel(root, text="Attachment: ", font=("Latin Modern Mono Slanted", 16))
+        attachment_label.grid(row=5, column=0, sticky="w")
+        
+        attachment_entry = ctk.CTkEntry(root, width=500, border_color="blue",text_color="red", font=("Latin Modern Mono Slanted", 16))
+        attachment_entry.grid(row=5, column=1, sticky="w")
+
+        attachment_button = ctk.CTkButton(root,width=100,border_color="red",hover_color="black", border_width=3,fg_color="blue", text="📎", command=select_attachment)
+        attachment_button.grid(row=5, column=1, sticky="e")
+        
         send_button = ctk.CTkButton(root, text="Send Email",font=("MathJax_Main", 16,"italic"),fg_color="blue",hover_color="purple",command=send)
-        send_button.grid(row=5, column=0, columnspan=2, pady=10)
+        send_button.grid(row=7, column=0, columnspan=2, pady=10)
+
+
+
+
+
+
+        
+        # Add TLS toggle
+        tls_var = ctk.StringVar(value="no")  # Default to TLS on
+        tls_checkbutton = ctk.CTkCheckBox(root, text="Use TLS", variable=tls_var, onvalue="yes", offvalue="no")
+        tls_checkbutton.grid(row=6, column=1, sticky="w")
 
     
 
         # Button to edit config
         edit_button = ctk.CTkButton(root, text="Edit Config",text_color="black", font=("MathJax_Main", 16, "italic"),fg_color="red",hover_color="green", command=edit_config)
         edit_button.grid(row=6, column=0, columnspan=2, pady=10,sticky="se")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emailspoofergui-3.1/emailspoofergui.egg-info/PKG-INFO` & `emailspoofergui-3.2/emailspoofergui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailspoofergui
-Version: 3.1
+Version: 3.2
 Summary: A graphical email spoofing tool
 Home-page: https://github.com/IMApurbo/emailspoofergui
 Author: AKM Korishee Apurbo
 Author-email: bandinvisible8@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emailspoofergui-3.1/setup.py` & `emailspoofergui-3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emailspoofergui',
-    version='3.1',
+    version='3.2',
     packages=find_packages(),
     package_data={'emailspoofergui': ['data/config.json']},
     install_requires=[
         'customtkinter',  # Example of a required package with a minimum version
         'CTkMessagebox',  # Example of a required package with an exact version 
     ],
     entry_points={
```

