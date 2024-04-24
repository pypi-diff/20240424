# Comparing `tmp/formulaic_ai-0.1.0.4.tar.gz` & `tmp/formulaic_ai-0.1.0.5.tar.gz`

## Comparing `formulaic_ai-0.1.0.4.tar` & `formulaic_ai-0.1.0.5.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/examples/motivator.json
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/examples/quickstart.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/src/formulaic_ai/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/src/formulaic_ai/formulaic_ai.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/src/formulaic_ai/motivator.json
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/src/formulaic_ai/openclient.py
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/LICENSE
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/README.md
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/pyproject.toml
--rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/examples/motivator.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/examples/quickstart.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/src/formulaic_ai/__init__.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/src/formulaic_ai/formulaic_ai.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/LICENSE
+-rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/README.md
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 formulaic_ai-0.1.0.5/PKG-INFO
```

### Comparing `formulaic_ai-0.1.0.4/examples/motivator.json` & `formulaic_ai-0.1.0.5/examples/motivator.json`

 * *Files identical despite different names*

### Comparing `formulaic_ai-0.1.0.4/src/formulaic_ai/formulaic_ai.py` & `formulaic_ai-0.1.0.5/src/formulaic_ai/formulaic_ai.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
-import json, sys
+import json, sys, copy, requests
 from string import Template
 
 
+
 ''' 
 Formula Class for enabling the opening, parsing of Formulas
 Gets them ready to send to various LLMs
 
 This will grow to support system prompts, few shot 
 examples, etc. 
 
 Formula Class works with OpenClient, which is a wrapper on top of 
 OpenAI and can send our Formula prompts to many LLMs
 
 :render(): Formula method for rendering usable prompts by substituting variable values
 into the template placeholders
 
-:inputs(): Helpful CLI tool for testing only. Prompts user for new variables on command line
 
 FormulaTemplate Class - extends Template for basic template rendering of curly
 brace tenplates. Consider changing format to support either mustache or 
 jinja formats
 
 Helper functions Also contains helper functions for opening json Formula files from disc
 And saving processed outputs back to disc
@@ -35,36 +35,26 @@
 
 '''
 
 
 # Helpers
 # open and read JSON file passed by CLI, return dict
 def load_formula(file_name):
+    """Load a JSON Formula from disk"""
     try:
         
         file_name = sys.argv[1] if len(sys.argv) > 1 else file_name
         with open(file_name, "r") as my_file:
             contents = my_file.read()
             return json.loads(contents) # load the JSON Formula into a dict
     except Exception as e:
         print(f"An unexpected error occurred: {e}")
 
 
-# saves our output file to disk 
-# filename is the full file path to disk plus extension
-def save_output(output, filename='export.txt'):
-    # convert dict to json string
-    json_str = json.dumps(output, indent=4)
-
-    with open(filename, 'w') as f:
-        f.write(json_str)
-    
-
-
-class Formula:
+class Formulaic:
     # blank Formula for embedded publishing in apps
     default_formula_json = {
         'name': '',
         'description': '',
         'created_at': '',
         'updated_at': '',
         'author': '',
@@ -73,48 +63,84 @@
         'script': {
             'model': {'id': '', 'name': '', 'vendor': '', 'provider': ''},
             'sequences': [],
             'variables': {}
         }
     }
 
-    
-    def __init__(self, formula_json=None): 
-        # formula_json is actually a dict. CONSIDER RENAMING!
+
+    def __init__(self, api_key=None, formula_json=None, options=None): 
+
         # Use the default_formula_json template if none is given
         if formula_json is None:
-            formula_json = Formula.default_formula_json        
+           formula_json = copy.deepcopy(Formulaic.default_formula_json)
+
+        if api_key is not None:
+            self.api_key = api_key
+
+        # set default options to include base_url
+        self.options = {"base_url": "https://formulaic.app/api/"}
         
-        # store the json as a hack for republishing, to be implemented later
-        self.formula_json = formula_json
+        # add user options, including overriding base_url. api_key expected
+        if options is not None:
+            self.options.update(options)
+
+        self.script = formula_json 
+
+     
+    @property
+    def script(self):
+        return self._script
+
+    @script.setter
+    def script(self, formula_json):
+        if formula_json is not None:
+            self._script = formula_json 
+            #self.script = formula_json
 
         # individual properties
+
         self.name = formula_json.get('name', '')
         self.description = formula_json.get('description', '')
         self.created = formula_json.get('created_at', '')
         self.updated = formula_json.get('updated_at', '')
         self.author = formula_json.get('author', '')  # ['author']
         self.source = formula_json.get ('source') #['source']
         self.license = formula_json.get('license', {}) #['license']['canonical_link']
         self.model = formula_json.get('script', {}).get('model', {}) #['script']['model']
+        
         # shortcut because model_id seems useful
         self.model_id = self.model.get('id', '')  #['script']['model']['id']
         self.sequences = formula_json.get('script', {}).get('sequences', []) #['script']['sequences']
 
 
         
         # full variables with all attributes
         self.variables = formula_json.get('script', {}).get('variables', {}) #['script']['variables']
 
         # storedefault variables in simple format. Useful for testing locally
-        self.default_values = Formula.simple_variables(self.variables)
+        self.default_values = Formulaic.simple_variables(self.variables)
 
         # auto-render the default values or fail when they're called before rendering?
         #self.prompts = Formula.render(self.sequences, self.defaults)
 
+    def get_formula(self, formula_id):
+        """Get a Formula from the Formulaic API"""
+        url = self.options['base_url'] + "recipes/" + formula_id + "/scripts"
+        headers = {
+            "Accept": "*/*",
+            "Authorization": "Bearer " + self.api_key,
+        }
+        
+        response = requests.get(url, headers=headers, timeout=10)
+        formula_dict = response.json()
+        self.script = formula_dict
+        return formula_dict
+
+
 
     @staticmethod 
     def simple_variables(data):
         # reformat our variables into k/v pairs for use in the template
         simple_data = {variable['name']: variable['value'] for variable in data}
         return simple_data
     
@@ -138,42 +164,22 @@
 
                 try:
                     rendered.append(prompt_template.substitute(simple_data))
 
                 except:
                     print(f"Templating error, the JSON you submitted has incorrect keys.")
         
+        #consider format here -- do we use OpenAI format for messages?
         #think about whether we want to return prompts or set a property
         self.prompts = rendered
-        #return rendered
-
-    # Convenient for testing user variable inputs in CLI
-    # Loops over Formula.variables simple object
-    # creates a new
-
-    def inputs(self, variables=None):
-
-        if variables is None:
-            variables = self.variables 
-
-        new_inputs = variables
+  
 
-        for i in variables:
-            answer = input(i['description'] + "\n> ")
+ 
 
-            # no validation here...
-            i['value'] = answer
-
-        new_inputs = Formula.simple_variables(new_inputs)
-
-        return new_inputs
-
-
-
-        
+# This allows us to extend templating or replace w/ Jinja2        
 class FormulaTemplate(Template):
     delimiter = '{{{'
     idpattern = r'\w+'
     
     pattern = r'''
     \{{3}                           # matches 3 opening braces 
     (?:
```

### Comparing `formulaic_ai-0.1.0.4/.gitignore` & `formulaic_ai-0.1.0.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Personal testing sripts
 /ignore
 open.py
 example.py
+test.py
+.DS_store
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `formulaic_ai-0.1.0.4/LICENSE` & `formulaic_ai-0.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `formulaic_ai-0.1.0.4/README.md` & `formulaic_ai-0.1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,24 @@
 # Formulaic Python Library 
-_**NOTE: This is a project in active development. It is not stable and changes frequently. It is not ready for production use.**_
+_**NOTE: This is a project in active development and changes frequently. It is not yet intended for production use.**_
 
-The Formulaic library makes it easy to use Formulas inside your generative AI applications. Formulas are open-licensed JSON scripts that contain AI prompts, template variables, and model configuration.  You can browse the library of existing Formulas for many popular language models at [Formulaic.app](https://formulaic.app). 
+The [Formulaic Python library](https://github.com/Mozilla-Ocho/formulaic-python) makes it easy to use Formulas inside your generative AI applications. Formulas are open-licensed JSON scripts that contain AI prompts, template variables, and model configuration.  You can browse the library of existing Formulas for many popular language models at [Formulaic.app](https://formulaic.app). 
 
 ## Installation
-This repo is currently private inside Mozilla until we release it as open source. 
 
-### (Recommended) Create a virtual environment
-Create a new directory on your local machine and open a terminal in that directory. Run this command:
+Install the Formulaic Python library
 
+```python
+pip install formulaic-ai
 ```
-python -m venv venv
-```
-
-Note, on your machine you may have to specify python3 if "python" is not setup as a shortcut to your current version:
-
-```
-python3 -m venv venv
-```
-
-This command creates a 'venv' virtual environment under `./venv` in the current directory. You're not ready to activate your virtual environment. Run this into the command line:
-
-```
-source venv/bin/activate
-```
-
-### Install the dev build of `formulaic` package
-Note: You must already be setup to use ssh with Mozilla repos in Github*. 
-
-Install the dev package as hosted here on Github:
-
-```
-pip install git+ssh://git@github.com/Mozilla-Ocho/formulaic-python.git
-```
-
-*_If you're not setup for SSH see [Setup Git to use SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?platform=mac&tool=webui) and [Generate SSH keys locally](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)_
-
-### Alternately: download the files and run directly
-You can also download this repo to your local machine and run all of the files inside `/src/formulaic/` to take a quick spin. **Note: the tutorial below is written for installing via `pip`.** 
-
-If you download and run all of the files inside [/src/formulaic/](https://github.com/Mozilla-Ocho/formulaic-python/tree/main/src/formulaic), use the [example.py](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/src/formulaic/example.py) file located there as your script file. This file only works if it is in the same directory as the other three files: `motivator.json`, `formulaic.py`, and `openclient.py`. 
-
 
 ## Quick Start
 We're going to build [this script](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/quickstart.py) step-by-step below, using a [Formula JSON file](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/motivator.json) we downloaded from [Formulaic.app](http://formulaic.app). If you download both this script and the JSON file to your working directory, you can run them right away. You will need a  llamafile server running at `localhost:8080`. You can also substitute in an  OpenAI key and get going that way. We're going to break the entire thing down step-by-step in a moment. 
 
-```
+```python
 from formulaic_ai import Formula, load_formula, OpenClient
  
 
 
 model_config = { "llamafile" :  {"url" : "http://localhost:8080/v1",
                                  "key":"sk-no-key-required", 
                                  "name": "LLaMA_CPP"}, 
@@ -93,26 +62,26 @@
 
 ## Step-by-step
 
 ### Do our imports
 
 Import `Formula` which is what we'll use to work with our Formulas, `OpenClient` a wrapper on the OpenAI library to make it seamless to send Formula prompts to any OpenAI compatible API, and a helper function `load_formula` to open Formula files. 
 
-```
+```python
 from formulaic_ai import Formula, OpenClient, load_formula
 ```
 
 ### Load and create our Formula instance
-All Formulas on [Formulaic.app](https://formulaic.app) JSON files that you can download to your local machine. We're providing one called `motivator.json` for you to use for this tutorial, which you can [download here](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/motivator.json). 
+All Formulas on [Formulaic.app](https://formulaic.app) are JSON files that you can download to your local machine. We're providing one called `motivator.json` for you to use for this tutorial, which you can [download here](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/motivator.json). 
 
 - Run `load_formula()` with a single argument of the the filepath+filename to `motivator.json`. That opens the Formula's JSON file and loads it into a Python dictionary
 - Create an instance of the `Formula` class by passing it the dictionary we just created. I combined these two steps and saved my `Formula` instance as `my_formula`
 - Now let's print the Formula name and description.
   
-```
+```python
 # load our Formula
 my_formula = Formula(load_formula("motivator.json")) 
 
 print(f"{my_formula.name}: {my_formula.description}")
 
 ```
 We see:
@@ -120,48 +89,53 @@
 ```
 Daily Motivator: Generates a motivational slogan based on your occasion.
 ```
 
 ### Render prompts
 Our Formula is loaded correctly. Now let's call the `.render()` method. Downloaded Formula prompts often contain templating variables. When we render, we replace the template variables with values and generate prompts that are stored in the `.prompts` property. If we don't pass new values to `.render()`, it will render prompts using the Formula's default values. Render and then print again. 
 
-```
+```python
 # render prompts. 
 my_formula.render()
 print(f"\nMy starting prompts: {my_formula.prompts}")
 ```
 Printed in the terminal we see we see: 
 
 ```
-My starting prompts: ['You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of first day of a new job', 'Now translate that slogan into French ']
+My starting prompts: ['You are a personal motivator assistant who is direct and 
+believes that everyone can be their best. Generate a motivating slogan for the 
+occasion of first day of a new job', 'Now translate that slogan into French ']
 ```
 Our prompts are in a Python list. The occasion is "first day of a new job" and the "French". 
 
 Now let's pass in new data, re-render our prompts, and print again.
-```
+```python
 #our new variables here. 
 data = {"occasion": "I'm scared of heights and climbing a mountain", 'language': 'German'}
 
 # render and print our prompts
 my_formula.render(data)
 print(f"\nMy new prompts: {my_formula.prompts}")
 ```
 Now we see our prompt list, available at `.prompts` contains the new occasion and new translation language.
 
 ```
-My new prompts: ["You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of I'm scared of heights and climbing a mountain", 'Now translate that slogan into German']
+My new prompts: ["You are a personal motivator assistant who is direct and 
+believes that everyone can be their best. Generate a motivating slogan for 
+the occasion of I'm scared of heights and climbing a mountain", 'Now 
+translate that slogan into German']
 ```
 
 ### Setup our model endpoint configuration
-We have prompts that are ready to be sent off to a language model. I'm going to use llamafile for this tutorial. [llamafile](https://github.com/Mozilla-Ocho/llamafile) is free, runs on your local machine, and easy to get going to run a local REST endpoint. I used the mistral 7B instruct llamafile. To get it running, download the file (5GB) and run it from the command line to start the local REST server. Please see the full [llamafile documentation](https://github.com/Mozilla-Ocho/llamafile). 
+We have prompts that are ready to be sent off to a language model. I'm going to use llamafile for this tutorial. [llamafile](https://github.com/Mozilla-Ocho/llamafile) is free, runs on your local machine, and makes it easy to deploy a local API endpoint. I chose the [mistral 7B instruct llamafile](https://huggingface.co/jartine/Mistral-7B-Instruct-v0.2-llamafile). To get it running, download the file (5GB) and run it from the command line to start the local HTTP server. Please see the full [llamafile documentation](https://github.com/Mozilla-Ocho/llamafile) for instructions on how to download and get started. 
 
 
-I went ahead and created a `model_config` dictionary to hold my model config variables to make it simpler. Beyond llamafile, I added placeholders for OpenAI and Anyscale. We can use the Formulaic Library to send our prompts to any language model API that supports the OpenAI format, so I included OpenAI and Anyscale. Anyscale provides hosting for many open source language models with an OpenAI compatible endpoint. You would have to create keys for OpenAI and Anyscale and substitute them in below. 
+I went ahead and created a `model_config` dictionary to hold my model config variables to make it simpler. We can use the Formulaic Library to send our prompts to any language model API that supports the OpenAI format, so I included OpenAI and Anyscale. Anyscale provides hosting for many open source language models with an OpenAI compatible endpoint. You would have to create keys for OpenAI and Anyscale and substitute them in below. 
 
-```
+```python
 
 model_config = { "llamafile" :  {"url" : "http://localhost:8080/v1",
                                  "key":"sk-no-key-required", 
                                  "name": "LLaMA_CPP"}, 
                   "OpenAI" :    {"url" :  "https://api.openai.com/v1",
                                  "key": "OPENAI_KEY_GOES_HERE", 
                                  "name": "gpt-3.5-turbo"},
@@ -169,35 +143,36 @@
                                  "key": "ANYSCALE_KEY_GOES_HERE", 
                                  "name": "mistralai/Mistral-7B-Instruct-v0.1"}  
                    
 }
 ```
 
 ### Create our OpenClient and start our chat
-Now we're ready to create our `OpenClient` instance, which is a class that extends `OpenAI`
-- We call `OpenClass` and pass two arguments:
--- The first is our Formula, `my_formula`.
--- The second is a dictionary that contains valid values for the `url`, `key`, and `name` of the model endpoing we're going to use. In this case, we pass it the `llamafile` dictionary from our `model_config`.
+Now we're ready to create our `OpenClient` instance, which is a class that extends `OpenAI`. 
 
-We're going to call it using a `with` statement so that OpenClient's content manager will clean up for us:
+* We call `OpenClass` and pass two arguments:
+    - The first is our Formula, `my_formula`.
+    -  The second is a dictionary that contains valid values for the `url`, `key`, and `name` of the model endpoing we're going to use. In this case, we pass it the `llamafile` dictionary from our `model_config`.
 
-```
+We're going to call it using a `with` statement so that OpenClient's context manager will clean up for us:
+
+```python
 with OpenClient(my_formula, model_config["llamafile"]) as client:
 
 ```
 
 We now have two options. We can just iterate over the 2 prompts we have in our Formula and await their responses. We do that by calling `.run()`. Instead, we are going to have an ongoing chat by calling `.chat()`. Both `.run` and `.chat` have a single optional argument to print out all user propmts and assistant responses to terminal. The default is `False` but we are using the command line to iteract, so we pass `True`
 
-```
+```python
 client.chat(True)
 ```
 
 And we're also going to add `print(client.messages)` so that we can see the full list of all messages we sent to the model and the model sent back. Our whole block looks like this:
 
-```
+```python
 # Create an OpenClient instance for llamafile
 with OpenClient(my_formula, model_config["llamafile"]) as client:
 
     # start our chat. True = print to terminal
     client.chat(True)
     
     # print our message log.  
@@ -215,25 +190,31 @@
 ```
 
 
 
 It takes a moment because we're running on our local hardware using llamafile. Here's what we see:
 
 ```
-User: You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of I'm scared of heights and climbing a mountain
-
-Assistant: Absolutely, I understand that fear of heights can be a significant challenge. But remember, every mountain peak is within your reach if you believe in yourself and take it one step at a time. Here's a motivating slogan for you:
+User: You are a personal motivator assistant who is direct and believes that 
+everyone can be their best. Generate a motivating slogan for the occasion of 
+I'm scared of heights and climbing a mountain
+
+Assistant: Absolutely, I understand that fear of heights can be a significant 
+challenge. But remember, every mountain peak is within your reach if you believe 
+in yourself and take it one step at a time. Here's a motivating slogan for you:
 
 "Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!"
 
 User: Now translate that slogan into German
 
-Assistant: Of course! The German translation of "Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!" would be:
+Assistant: Of course! The German translation of "Conquer the Mountain Within: 
+Your Fear is Just a Stepping Stone to New Heights!" would be:
 
-"Berge Innerhalb von Dir besiegen: Deine Angst ist nur ein Stufenstein zu neuen Gipfeln!"
+"Berge Innerhalb von Dir besiegen: Deine Angst ist nur ein Stufenstein zu 
+neuen Gipfeln!"
 
 > 
 ```
 
 Notice that we have iterated over both of our two prompts and received two answers from the llamafile model. The cursor is awaiting our input. Let's tell it to translate to Latin and hit Return. 
 
 ```
@@ -249,15 +230,28 @@
 
 ### See the message log printed
 Our Formula instance saved every message we sent to the model and every message the assistant sent back. This is what we accessed above by printing `client.messages`
 
 
 and now we see:
 ```
-[{'role': 'user', 'content': "You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of I'm scared of heights and climbing a mountain"}, {'role': 'assistant', 'content': 'Absolutely, I understand that fear of heights can be a significant challenge. But remember, every mountain peak is within your reach if you believe in yourself and take it one step at a time. Here\'s a motivating slogan for you:\n\n"Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!"'}, {'role': 'user', 'content': 'Now translate that slogan into German'}, {'role': 'assistant', 'content': 'Of course! The German translation of "Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!" would be:\n\n"Berge Innerhalb von Dir besiegen: Deine Angst ist nur ein Stufenstein zu neuen Gipfeln!"'}, {'role': 'user', 'content': 'Now translate to Latin'}, {'role': 'assistant', 'content': 'In Latin, the phrase could be:\n\n"Montes Intus Vincere: Timor Tuum Nec Nisi Gradus Ad Novos Culmines!"'}]
+[{'role': 'user', 'content': "You are a personal motivator assistant who is 
+direct and believes that everyone can be their best. Generate a motivating 
+slogan for the occasion of I'm scared of heights and climbing a mountain"}, 
+{'role': 'assistant', 'content': 'Absolutely, I understand that fear of heights 
+can be a significant challenge. But remember, every mountain peak is within your 
+reach if you believe in yourself and take it one step at a time. Here\'s a 
+motivating slogan for you:\n\n"Conquer the Mountain Within: Your Fear is 
+Just a Stepping Stone to New Heights!"'}, {'role': 'user', 'content': 'Now 
+translate that slogan into German'}, {'role': 'assistant', 'content': 'Of course! 
+The German translation of "Conquer the Mountain Within: Your Fear is Just a Stepping 
+Stone to New Heights!" would be:\n\n"Berge Innerhalb von Dir besiegen: Deine Angst 
+\ist nur ein Stufenstein zu neuen Gipfeln!"'}, {'role': 'user', 'content': 'Now 
+translate to Latin'}, {'role': 'assistant', 'content': 'In Latin, the phrase could 
+be:\n\n"Montes Intus Vincere: Timor Tuum Nec Nisi Gradus Ad Novos Culmines!"'}]
 
 ```
 
 That's the gist! You've parsed your first Formula and sent it off to a local language model. You can send it off to other model endpoints just as easily.  
 
 You can see [the entire script](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/quickstart.py) we just produced here.
```

### Comparing `formulaic_ai-0.1.0.4/pyproject.toml` & `formulaic_ai-0.1.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "formulaic-ai"
-version = "0.1.0.4"
-description = "The official Formulaic python library for working with generative AI prompts."
+version = "0.1.0.5"
+description = "The official Formulaic Python library"
 authors = [
-    {name = "Javaun Moradi", email = "formulaic@mozilla.com"}
+    {name = "Javaun Moradi", email = "formulaic@mozilla.com"},
+    {name = "Gabriel Habayeb", email = "formulaic@mozilla.com"}
     ]
 license = "Apache-2.0"
 readme = "README.md"
-keywords = ["prompt engineering", "prompt scripts" , "LLM", "language models", "generative ai", "openai", "api", ]
+keywords = ["prompt engineering", "prompt scripts" , "LLM", "language models", "llama", "mistral", "generative ai", "openai", "api", ]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "openai>=1.0"
+    "requests>=2.31.0"
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 homepage = "https:formulaic.app"
 repository = "https://github.com/Mozilla-Ocho/formulaic-python"
 documentation = "https://docs.formulaic.app"
```

### Comparing `formulaic_ai-0.1.0.4/PKG-INFO` & `formulaic_ai-0.1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,50 @@
 Metadata-Version: 2.3
 Name: formulaic-ai
-Version: 0.1.0.4
-Summary: The official Formulaic python library for working with generative AI prompts.
+Version: 0.1.0.5
+Summary: The official Formulaic Python library
 Project-URL: homepage, https:formulaic.app
 Project-URL: repository, https://github.com/Mozilla-Ocho/formulaic-python
 Project-URL: documentation, https://docs.formulaic.app
-Author-email: Javaun Moradi <formulaic@mozilla.com>
+Author-email: Javaun Moradi <formulaic@mozilla.com>, Gabriel Habayeb <formulaic@mozilla.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
-Keywords: LLM,api,generative ai,language models,openai,prompt engineering,prompt scripts
+Keywords: LLM,api,generative ai,language models,llama,mistral,openai,prompt engineering,prompt scripts
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.8
-Requires-Dist: openai>=1.0
+Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # Formulaic Python Library 
-_**NOTE: This is a project in active development. It is not stable and changes frequently. It is not ready for production use.**_
+_**NOTE: This is a project in active development and changes frequently. It is not yet intended for production use.**_
 
-The Formulaic library makes it easy to use Formulas inside your generative AI applications. Formulas are open-licensed JSON scripts that contain AI prompts, template variables, and model configuration.  You can browse the library of existing Formulas for many popular language models at [Formulaic.app](https://formulaic.app). 
+The [Formulaic Python library](https://github.com/Mozilla-Ocho/formulaic-python) makes it easy to use Formulas inside your generative AI applications. Formulas are open-licensed JSON scripts that contain AI prompts, template variables, and model configuration.  You can browse the library of existing Formulas for many popular language models at [Formulaic.app](https://formulaic.app). 
 
 ## Installation
-This repo is currently private inside Mozilla until we release it as open source. 
 
-### (Recommended) Create a virtual environment
-Create a new directory on your local machine and open a terminal in that directory. Run this command:
+Install the Formulaic Python library
 
+```python
+pip install formulaic-ai
 ```
-python -m venv venv
-```
-
-Note, on your machine you may have to specify python3 if "python" is not setup as a shortcut to your current version:
-
-```
-python3 -m venv venv
-```
-
-This command creates a 'venv' virtual environment under `./venv` in the current directory. You're not ready to activate your virtual environment. Run this into the command line:
-
-```
-source venv/bin/activate
-```
-
-### Install the dev build of `formulaic` package
-Note: You must already be setup to use ssh with Mozilla repos in Github*. 
-
-Install the dev package as hosted here on Github:
-
-```
-pip install git+ssh://git@github.com/Mozilla-Ocho/formulaic-python.git
-```
-
-*_If you're not setup for SSH see [Setup Git to use SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?platform=mac&tool=webui) and [Generate SSH keys locally](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)_
-
-### Alternately: download the files and run directly
-You can also download this repo to your local machine and run all of the files inside `/src/formulaic/` to take a quick spin. **Note: the tutorial below is written for installing via `pip`.** 
-
-If you download and run all of the files inside [/src/formulaic/](https://github.com/Mozilla-Ocho/formulaic-python/tree/main/src/formulaic), use the [example.py](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/src/formulaic/example.py) file located there as your script file. This file only works if it is in the same directory as the other three files: `motivator.json`, `formulaic.py`, and `openclient.py`. 
-
 
 ## Quick Start
 We're going to build [this script](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/quickstart.py) step-by-step below, using a [Formula JSON file](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/motivator.json) we downloaded from [Formulaic.app](http://formulaic.app). If you download both this script and the JSON file to your working directory, you can run them right away. You will need a  llamafile server running at `localhost:8080`. You can also substitute in an  OpenAI key and get going that way. We're going to break the entire thing down step-by-step in a moment. 
 
-```
+```python
 from formulaic_ai import Formula, load_formula, OpenClient
  
 
 
 model_config = { "llamafile" :  {"url" : "http://localhost:8080/v1",
                                  "key":"sk-no-key-required", 
                                  "name": "LLaMA_CPP"}, 
@@ -119,26 +88,26 @@
 
 ## Step-by-step
 
 ### Do our imports
 
 Import `Formula` which is what we'll use to work with our Formulas, `OpenClient` a wrapper on the OpenAI library to make it seamless to send Formula prompts to any OpenAI compatible API, and a helper function `load_formula` to open Formula files. 
 
-```
+```python
 from formulaic_ai import Formula, OpenClient, load_formula
 ```
 
 ### Load and create our Formula instance
-All Formulas on [Formulaic.app](https://formulaic.app) JSON files that you can download to your local machine. We're providing one called `motivator.json` for you to use for this tutorial, which you can [download here](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/motivator.json). 
+All Formulas on [Formulaic.app](https://formulaic.app) are JSON files that you can download to your local machine. We're providing one called `motivator.json` for you to use for this tutorial, which you can [download here](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/motivator.json). 
 
 - Run `load_formula()` with a single argument of the the filepath+filename to `motivator.json`. That opens the Formula's JSON file and loads it into a Python dictionary
 - Create an instance of the `Formula` class by passing it the dictionary we just created. I combined these two steps and saved my `Formula` instance as `my_formula`
 - Now let's print the Formula name and description.
   
-```
+```python
 # load our Formula
 my_formula = Formula(load_formula("motivator.json")) 
 
 print(f"{my_formula.name}: {my_formula.description}")
 
 ```
 We see:
@@ -146,48 +115,53 @@
 ```
 Daily Motivator: Generates a motivational slogan based on your occasion.
 ```
 
 ### Render prompts
 Our Formula is loaded correctly. Now let's call the `.render()` method. Downloaded Formula prompts often contain templating variables. When we render, we replace the template variables with values and generate prompts that are stored in the `.prompts` property. If we don't pass new values to `.render()`, it will render prompts using the Formula's default values. Render and then print again. 
 
-```
+```python
 # render prompts. 
 my_formula.render()
 print(f"\nMy starting prompts: {my_formula.prompts}")
 ```
 Printed in the terminal we see we see: 
 
 ```
-My starting prompts: ['You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of first day of a new job', 'Now translate that slogan into French ']
+My starting prompts: ['You are a personal motivator assistant who is direct and 
+believes that everyone can be their best. Generate a motivating slogan for the 
+occasion of first day of a new job', 'Now translate that slogan into French ']
 ```
 Our prompts are in a Python list. The occasion is "first day of a new job" and the "French". 
 
 Now let's pass in new data, re-render our prompts, and print again.
-```
+```python
 #our new variables here. 
 data = {"occasion": "I'm scared of heights and climbing a mountain", 'language': 'German'}
 
 # render and print our prompts
 my_formula.render(data)
 print(f"\nMy new prompts: {my_formula.prompts}")
 ```
 Now we see our prompt list, available at `.prompts` contains the new occasion and new translation language.
 
 ```
-My new prompts: ["You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of I'm scared of heights and climbing a mountain", 'Now translate that slogan into German']
+My new prompts: ["You are a personal motivator assistant who is direct and 
+believes that everyone can be their best. Generate a motivating slogan for 
+the occasion of I'm scared of heights and climbing a mountain", 'Now 
+translate that slogan into German']
 ```
 
 ### Setup our model endpoint configuration
-We have prompts that are ready to be sent off to a language model. I'm going to use llamafile for this tutorial. [llamafile](https://github.com/Mozilla-Ocho/llamafile) is free, runs on your local machine, and easy to get going to run a local REST endpoint. I used the mistral 7B instruct llamafile. To get it running, download the file (5GB) and run it from the command line to start the local REST server. Please see the full [llamafile documentation](https://github.com/Mozilla-Ocho/llamafile). 
+We have prompts that are ready to be sent off to a language model. I'm going to use llamafile for this tutorial. [llamafile](https://github.com/Mozilla-Ocho/llamafile) is free, runs on your local machine, and makes it easy to deploy a local API endpoint. I chose the [mistral 7B instruct llamafile](https://huggingface.co/jartine/Mistral-7B-Instruct-v0.2-llamafile). To get it running, download the file (5GB) and run it from the command line to start the local HTTP server. Please see the full [llamafile documentation](https://github.com/Mozilla-Ocho/llamafile) for instructions on how to download and get started. 
 
 
-I went ahead and created a `model_config` dictionary to hold my model config variables to make it simpler. Beyond llamafile, I added placeholders for OpenAI and Anyscale. We can use the Formulaic Library to send our prompts to any language model API that supports the OpenAI format, so I included OpenAI and Anyscale. Anyscale provides hosting for many open source language models with an OpenAI compatible endpoint. You would have to create keys for OpenAI and Anyscale and substitute them in below. 
+I went ahead and created a `model_config` dictionary to hold my model config variables to make it simpler. We can use the Formulaic Library to send our prompts to any language model API that supports the OpenAI format, so I included OpenAI and Anyscale. Anyscale provides hosting for many open source language models with an OpenAI compatible endpoint. You would have to create keys for OpenAI and Anyscale and substitute them in below. 
 
-```
+```python
 
 model_config = { "llamafile" :  {"url" : "http://localhost:8080/v1",
                                  "key":"sk-no-key-required", 
                                  "name": "LLaMA_CPP"}, 
                   "OpenAI" :    {"url" :  "https://api.openai.com/v1",
                                  "key": "OPENAI_KEY_GOES_HERE", 
                                  "name": "gpt-3.5-turbo"},
@@ -195,35 +169,36 @@
                                  "key": "ANYSCALE_KEY_GOES_HERE", 
                                  "name": "mistralai/Mistral-7B-Instruct-v0.1"}  
                    
 }
 ```
 
 ### Create our OpenClient and start our chat
-Now we're ready to create our `OpenClient` instance, which is a class that extends `OpenAI`
-- We call `OpenClass` and pass two arguments:
--- The first is our Formula, `my_formula`.
--- The second is a dictionary that contains valid values for the `url`, `key`, and `name` of the model endpoing we're going to use. In this case, we pass it the `llamafile` dictionary from our `model_config`.
+Now we're ready to create our `OpenClient` instance, which is a class that extends `OpenAI`. 
 
-We're going to call it using a `with` statement so that OpenClient's content manager will clean up for us:
+* We call `OpenClass` and pass two arguments:
+    - The first is our Formula, `my_formula`.
+    -  The second is a dictionary that contains valid values for the `url`, `key`, and `name` of the model endpoing we're going to use. In this case, we pass it the `llamafile` dictionary from our `model_config`.
 
-```
+We're going to call it using a `with` statement so that OpenClient's context manager will clean up for us:
+
+```python
 with OpenClient(my_formula, model_config["llamafile"]) as client:
 
 ```
 
 We now have two options. We can just iterate over the 2 prompts we have in our Formula and await their responses. We do that by calling `.run()`. Instead, we are going to have an ongoing chat by calling `.chat()`. Both `.run` and `.chat` have a single optional argument to print out all user propmts and assistant responses to terminal. The default is `False` but we are using the command line to iteract, so we pass `True`
 
-```
+```python
 client.chat(True)
 ```
 
 And we're also going to add `print(client.messages)` so that we can see the full list of all messages we sent to the model and the model sent back. Our whole block looks like this:
 
-```
+```python
 # Create an OpenClient instance for llamafile
 with OpenClient(my_formula, model_config["llamafile"]) as client:
 
     # start our chat. True = print to terminal
     client.chat(True)
     
     # print our message log.  
@@ -241,25 +216,31 @@
 ```
 
 
 
 It takes a moment because we're running on our local hardware using llamafile. Here's what we see:
 
 ```
-User: You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of I'm scared of heights and climbing a mountain
-
-Assistant: Absolutely, I understand that fear of heights can be a significant challenge. But remember, every mountain peak is within your reach if you believe in yourself and take it one step at a time. Here's a motivating slogan for you:
+User: You are a personal motivator assistant who is direct and believes that 
+everyone can be their best. Generate a motivating slogan for the occasion of 
+I'm scared of heights and climbing a mountain
+
+Assistant: Absolutely, I understand that fear of heights can be a significant 
+challenge. But remember, every mountain peak is within your reach if you believe 
+in yourself and take it one step at a time. Here's a motivating slogan for you:
 
 "Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!"
 
 User: Now translate that slogan into German
 
-Assistant: Of course! The German translation of "Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!" would be:
+Assistant: Of course! The German translation of "Conquer the Mountain Within: 
+Your Fear is Just a Stepping Stone to New Heights!" would be:
 
-"Berge Innerhalb von Dir besiegen: Deine Angst ist nur ein Stufenstein zu neuen Gipfeln!"
+"Berge Innerhalb von Dir besiegen: Deine Angst ist nur ein Stufenstein zu 
+neuen Gipfeln!"
 
 > 
 ```
 
 Notice that we have iterated over both of our two prompts and received two answers from the llamafile model. The cursor is awaiting our input. Let's tell it to translate to Latin and hit Return. 
 
 ```
@@ -275,15 +256,28 @@
 
 ### See the message log printed
 Our Formula instance saved every message we sent to the model and every message the assistant sent back. This is what we accessed above by printing `client.messages`
 
 
 and now we see:
 ```
-[{'role': 'user', 'content': "You are a personal motivator assistant who is direct and believes that everyone can be their best. Generate a motivating slogan for the occasion of I'm scared of heights and climbing a mountain"}, {'role': 'assistant', 'content': 'Absolutely, I understand that fear of heights can be a significant challenge. But remember, every mountain peak is within your reach if you believe in yourself and take it one step at a time. Here\'s a motivating slogan for you:\n\n"Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!"'}, {'role': 'user', 'content': 'Now translate that slogan into German'}, {'role': 'assistant', 'content': 'Of course! The German translation of "Conquer the Mountain Within: Your Fear is Just a Stepping Stone to New Heights!" would be:\n\n"Berge Innerhalb von Dir besiegen: Deine Angst ist nur ein Stufenstein zu neuen Gipfeln!"'}, {'role': 'user', 'content': 'Now translate to Latin'}, {'role': 'assistant', 'content': 'In Latin, the phrase could be:\n\n"Montes Intus Vincere: Timor Tuum Nec Nisi Gradus Ad Novos Culmines!"'}]
+[{'role': 'user', 'content': "You are a personal motivator assistant who is 
+direct and believes that everyone can be their best. Generate a motivating 
+slogan for the occasion of I'm scared of heights and climbing a mountain"}, 
+{'role': 'assistant', 'content': 'Absolutely, I understand that fear of heights 
+can be a significant challenge. But remember, every mountain peak is within your 
+reach if you believe in yourself and take it one step at a time. Here\'s a 
+motivating slogan for you:\n\n"Conquer the Mountain Within: Your Fear is 
+Just a Stepping Stone to New Heights!"'}, {'role': 'user', 'content': 'Now 
+translate that slogan into German'}, {'role': 'assistant', 'content': 'Of course! 
+The German translation of "Conquer the Mountain Within: Your Fear is Just a Stepping 
+Stone to New Heights!" would be:\n\n"Berge Innerhalb von Dir besiegen: Deine Angst 
+\ist nur ein Stufenstein zu neuen Gipfeln!"'}, {'role': 'user', 'content': 'Now 
+translate to Latin'}, {'role': 'assistant', 'content': 'In Latin, the phrase could 
+be:\n\n"Montes Intus Vincere: Timor Tuum Nec Nisi Gradus Ad Novos Culmines!"'}]
 
 ```
 
 That's the gist! You've parsed your first Formula and sent it off to a local language model. You can send it off to other model endpoints just as easily.  
 
 You can see [the entire script](https://github.com/Mozilla-Ocho/formulaic-python/blob/main/examples/quickstart.py) we just produced here.
```

