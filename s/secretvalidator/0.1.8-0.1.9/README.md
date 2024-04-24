# Comparing `tmp/secretvalidator-0.1.8.tar.gz` & `tmp/secretvalidator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidator-0.1.8.tar", last modified: Mon Apr 22 16:54:38 2024, max compression
+gzip compressed data, was "secretvalidator-0.1.9.tar", last modified: Tue Apr 23 08:53:54 2024, max compression
```

## Comparing `secretvalidator-0.1.8.tar` & `secretvalidator-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 16:54:38.001836 secretvalidator-0.1.8/
--rw-rw-rw-   0        0        0     1092 2024-04-22 08:47:45.000000 secretvalidator-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      107 2024-04-22 16:54:37.998834 secretvalidator-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       72 2024-04-22 08:47:45.000000 secretvalidator-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 16:54:37.940835 secretvalidator-0.1.8/secretvalidator/
--rw-rw-rw-   0        0        0       26 2024-04-22 10:41:30.000000 secretvalidator-0.1.8/secretvalidator/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-04-22 16:54:11.000000 secretvalidator-0.1.8/secretvalidator/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-22 16:54:37.992834 secretvalidator-0.1.8/secretvalidator.egg-info/
--rw-rw-rw-   0        0        0      107 2024-04-22 16:54:37.000000 secretvalidator-0.1.8/secretvalidator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-04-22 16:54:37.000000 secretvalidator-0.1.8/secretvalidator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 16:54:37.000000 secretvalidator-0.1.8/secretvalidator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-22 16:54:37.000000 secretvalidator-0.1.8/secretvalidator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-04-22 16:54:37.000000 secretvalidator-0.1.8/secretvalidator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-22 16:54:37.000000 secretvalidator-0.1.8/secretvalidator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 16:54:38.001836 secretvalidator-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      321 2024-04-22 16:54:31.000000 secretvalidator-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:53:54.636295 secretvalidator-0.1.9/
+-rw-rw-rw-   0        0        0     1092 2024-04-22 08:47:45.000000 secretvalidator-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      107 2024-04-23 08:53:54.628296 secretvalidator-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2024-04-22 08:47:45.000000 secretvalidator-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 08:53:54.544296 secretvalidator-0.1.9/secretvalidator/
+-rw-rw-rw-   0        0        0       26 2024-04-22 10:41:30.000000 secretvalidator-0.1.9/secretvalidator/__init__.py
+-rw-rw-rw-   0        0        0     2431 2024-04-23 08:53:06.000000 secretvalidator-0.1.9/secretvalidator/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:53:54.618294 secretvalidator-0.1.9/secretvalidator.egg-info/
+-rw-rw-rw-   0        0        0      107 2024-04-23 08:53:53.000000 secretvalidator-0.1.9/secretvalidator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-23 08:53:53.000000 secretvalidator-0.1.9/secretvalidator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:53:53.000000 secretvalidator-0.1.9/secretvalidator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-23 08:53:53.000000 secretvalidator-0.1.9/secretvalidator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-04-23 08:53:53.000000 secretvalidator-0.1.9/secretvalidator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 08:53:53.000000 secretvalidator-0.1.9/secretvalidator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:53:54.637295 secretvalidator-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      321 2024-04-23 08:53:30.000000 secretvalidator-0.1.9/setup.py
```

### Comparing `secretvalidator-0.1.8/LICENSE` & `secretvalidator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidator-0.1.8/secretvalidator/cli.py` & `secretvalidator-0.1.9/secretvalidator/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import click
 import requests
 import json
-import importlib.resources
 import os
 
 @click.command()
 @click.argument('service', nargs=1, type=click.Choice(['sonarcloud', 'snyk']))
 @click.argument('secret', nargs=1)
 @click.option('-r', '--response', is_flag=True, help='Print simple response (status/true/false).')
 def validate(service, secret, response):
     """Run secret validation checks."""
     click.echo("Running secret validation checks...")
-     
-     
-    # Get absolute path to urls.txt
+         # Get absolute path to urls.txt
     current_dir = os.path.abspath(os.path.dirname(__file__))
     urls_path = os.path.join(current_dir, 'urls.txt')
     
     # Check if urls.txt exists
     if not os.path.exists(urls_path):
         click.echo("Error: 'urls.txt' file not found.")
         return
@@ -25,15 +22,15 @@
     # Read file content
     with open(urls_path, 'r') as f:
         urls_content = f.read()
     
     urls = json.loads(urls_content)
     
     service_url = urls.get(service)
-    
+
     if not service_url:
         click.echo(f"Error: URL for service {service} not found.")
         return
     
     headers = {}
     
     # Set headers for Snyk or SonarCloud
```

