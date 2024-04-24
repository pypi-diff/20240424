# Comparing `tmp/pailettes-0.1.2.tar.gz` & `tmp/pailettes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pailettes-0.1.2.tar", max compression
+gzip compressed data, was "pailettes-0.1.3.tar", max compression
```

## Comparing `pailettes-0.1.2.tar` & `pailettes-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-03-27 18:50:12.067866 pailettes-0.1.2/LICENSE
--rw-r--r--   0        0        0     1040 2024-04-11 15:28:34.260155 pailettes-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-27 19:37:48.611302 pailettes-0.1.2/pailettes/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-11 15:33:15.361423 pailettes-0.1.2/pailettes/main.py
--rw-r--r--   0        0        0      403 2024-04-11 15:46:47.071880 pailettes-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 pailettes-0.1.2/setup.py
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 pailettes-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-27 18:50:12.067866 pailettes-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1040 2024-04-11 15:28:34.260155 pailettes-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 19:37:48.611302 pailettes-0.1.3/pailettes/__init__.py
+-rw-r--r--   0        0        0     3105 2024-04-24 18:44:17.822526 pailettes-0.1.3/pailettes/main.py
+-rw-r--r--   0        0        0      517 2024-04-24 19:09:39.556182 pailettes-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 pailettes-0.1.3/setup.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 pailettes-0.1.3/PKG-INFO
```

### Comparing `pailettes-0.1.2/LICENSE` & `pailettes-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pailettes-0.1.2/README.md` & `pailettes-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pailettes-0.1.2/pailettes/main.py` & `pailettes-0.1.3/pailettes/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich import print
 
 
 app = typer.Typer()
 
 
 @app.command()
-def generate(theme: str, palette_count: int = 1, color_count: int = 4):
+def generate(theme: str, palette_count: int = 1, color_count: int = 4, to_json: bool = False, json_file: str = None):
     api_key = os.getenv('OPENAI_KEY')
     if not api_key:
         raise typer.BadParameter("Please set your OpenAI API KEY as an env var named 'OPENAI_KEY'.")
     try:
         client = OpenAI(api_key=api_key)
         session = client.chat.completions.create(
             model="gpt-3.5-turbo",
@@ -48,12 +48,22 @@
         )
     except AuthenticationError:
         raise typer.BadParameter("Your API key was not valid - we could not authenticate with OpenAI.")
     response = session.choices[0].message.content
 
     json_list = json.loads(response)
 
+    if to_json is True:
+        pretty_json = json.dumps(json_list, indent=4)
+        if json_file:
+            with open(json_file, "w") as fh:
+                fh.write(pretty_json)
+            print(f"Palette data saved in {json_file}.")
+        else:
+            print(pretty_json)
+        return
+
     for json_resp in json_list:
         print(json_resp["name"])
         for c in json_resp["colors"]:
             print(f"[on {c}]{c}        [/]")
         print()
```

### Comparing `pailettes-0.1.2/setup.py` & `pailettes-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['openai>=1.14.3,<2.0.0', 'rich>=13.7.1,<14.0.0', 'typer[all]>=0.11.0,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['pailettes = pailettes.main:app']}
 
 setup_kwargs = {
     'name': 'pailettes',
-    'version': '0.1.2',
-    'description': '',
+    'version': '0.1.3',
+    'description': 'Generate color palettes using artificial intelligence (OpenAI).',
     'long_description': '# Pailettes\n\nGenerate color palettes using artificial intelligence. The OpenAI API is used for this, so you will require an account.\n\n![Pailettes](https://raw.githubusercontent.com/psyonara/pailettes/master/imgs/headline.jpg)\n\n## Installation\n\n### Pipx\n\n```shell\npipx install pailettes\n```\n\n### Pip\n\n```shell\npip install pailettes\n```\n\n## Configuration\n\nTo configure your OpenAI API key, create an environment variable as follows.\n\n### Windows\nTODO\n\n### MacOS\nTODO\n\n### Linux\n```shell\nexport OPENAI_KEY="your-key-goes-here"\n```\n\nThis will set your OpenAI key for that terminal session. If you would like to permanently set the environment variable, consult the documentation of your OS/shell.\n\n## Usage\n\n### Quick Start\n\n```shell\npailettes retro\n```\n\nThis creates a color palette with a "retro" theme.\n\n### Number of colors\n\nTo specify the number of colors in your palette:\n\n```shell\npailettes retro --color-count=6\n```\n\n### Number of palettes\n\nTo specify the number of palettes to generate:\n\n```shell\npailettes retro --palette-count=3\n```\n',
     'author': 'Helmut Irle',
     'author_email': 'me@helmut.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/psyonara/pailettes',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `pailettes-0.1.2/PKG-INFO` & `pailettes-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pailettes
-Version: 0.1.2
-Summary: 
+Version: 0.1.3
+Summary: Generate color palettes using artificial intelligence (OpenAI).
+Home-page: https://github.com/psyonara/pailettes
 Author: Helmut Irle
 Author-email: me@helmut.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=1.14.3,<2.0.0)
```

