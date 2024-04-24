# Comparing `tmp/openai_messages_token_helper-0.0.4.tar.gz` & `tmp/openai_messages_token_helper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_messages_token_helper-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai_messages_token_helper-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai_messages_token_helper-0.0.4.tar` & `openai_messages_token_helper-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      880 2024-04-06 22:31:15.975017 openai_messages_token_helper-0.0.4/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.0.4/.gitignore
--rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      148 2024-04-21 22:10:10.823452 openai_messages_token_helper-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0      390 2024-04-21 22:14:21.177132 openai_messages_token_helper-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      238 2024-04-04 19:40:44.165440 openai_messages_token_helper-0.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.0.4/LICENSE
--rw-r--r--   0        0        0     3595 2024-04-21 22:12:13.742283 openai_messages_token_helper-0.0.4/README.md
--rw-r--r--   0        0        0     1314 2024-04-21 22:14:34.835118 openai_messages_token_helper-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      265 2024-04-04 20:03:54.128074 openai_messages_token_helper-0.0.4/src/openai_messages_token_helper/__init__.py
--rw-r--r--   0        0        0     2020 2024-04-04 19:40:09.278693 openai_messages_token_helper-0.0.4/src/openai_messages_token_helper/images_helper.py
--rw-r--r--   0        0        0     5118 2024-04-04 19:40:53.891278 openai_messages_token_helper-0.0.4/src/openai_messages_token_helper/message_builder.py
--rw-r--r--   0        0        0     3048 2024-04-21 22:10:10.832836 openai_messages_token_helper-0.0.4/src/openai_messages_token_helper/model_helper.py
--rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.0.4/tests/image_large.png
--rw-r--r--   0        0        0     1448 2024-04-21 22:10:10.836640 openai_messages_token_helper-0.0.4/tests/messages.py
--rw-r--r--   0        0        0     1105 2024-04-21 22:11:26.921768 openai_messages_token_helper-0.0.4/tests/test_imageshelper.py
--rw-r--r--   0        0        0     1729 2024-04-21 22:11:26.916047 openai_messages_token_helper-0.0.4/tests/test_messagebuilder.py
--rw-r--r--   0        0        0     2232 2024-04-21 22:11:26.914077 openai_messages_token_helper-0.0.4/tests/test_modelhelper.py
--rw-r--r--   0        0        0     1604 2024-04-21 22:10:10.850735 openai_messages_token_helper-0.0.4/tests/verify_openai.py
--rw-r--r--   0        0        0     4679 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      880 2024-04-06 22:31:15.975017 openai_messages_token_helper-0.0.5/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.0.5/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      148 2024-04-21 22:10:10.823452 openai_messages_token_helper-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0      731 2024-04-24 15:10:08.284117 openai_messages_token_helper-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      238 2024-04-04 19:40:44.165440 openai_messages_token_helper-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3860 2024-04-24 15:10:08.286590 openai_messages_token_helper-0.0.5/README.md
+-rw-r--r--   0        0        0     1314 2024-04-24 15:10:08.288520 openai_messages_token_helper-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-04-24 15:10:08.288991 openai_messages_token_helper-0.0.5/src/openai_messages_token_helper/__init__.py
+-rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.0.5/src/openai_messages_token_helper/images_helper.py
+-rw-r--r--   0        0        0     5118 2024-04-24 15:10:08.289805 openai_messages_token_helper-0.0.5/src/openai_messages_token_helper/message_builder.py
+-rw-r--r--   0        0        0     3784 2024-04-24 15:10:08.292471 openai_messages_token_helper-0.0.5/src/openai_messages_token_helper/model_helper.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.0.5/tests/image_large.png
+-rw-r--r--   0        0        0     1448 2024-04-21 22:10:10.836640 openai_messages_token_helper-0.0.5/tests/messages.py
+-rw-r--r--   0        0        0     1105 2024-04-24 15:10:08.294738 openai_messages_token_helper-0.0.5/tests/test_imageshelper.py
+-rw-r--r--   0        0        0     1729 2024-04-24 15:10:08.298351 openai_messages_token_helper-0.0.5/tests/test_messagebuilder.py
+-rw-r--r--   0        0        0     2782 2024-04-24 15:10:08.300364 openai_messages_token_helper-0.0.5/tests/test_modelhelper.py
+-rw-r--r--   0        0        0     1604 2024-04-21 22:10:10.850735 openai_messages_token_helper-0.0.5/tests/verify_openai.py
+-rw-r--r--   0        0        0     4944 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.0.5/PKG-INFO
```

### Comparing `openai_messages_token_helper-0.0.4/.github/workflows/python.yaml` & `openai_messages_token_helper-0.0.5/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/.gitignore` & `openai_messages_token_helper-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/LICENSE` & `openai_messages_token_helper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/README.md` & `openai_messages_token_helper-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 ### `count_tokens_for_message`
 
 Counts the number of tokens in a message.
 
 Arguments:
 
 * `model` (`str`): The model name to use for token calculation, like gpt-3.5-turbo.
+* `message` (`dict`): The message to count tokens for.
+* `default_to_cl100k` (`bool`): Whether to default to the CL100k token limit if the model is not found.
 
 Returns:
 
 * `int`: The number of tokens in the message.
 
 Example:
 
@@ -125,14 +127,15 @@
 ### `get_token_limit`
 
 Get the token limit for a given GPT model name (OpenAI.com or Azure OpenAI supported).
 
 Arguments:
 
 * `model` (`str`): The model name to use for token calculation, like gpt-3.5-turbo (OpenAI.com) or gpt-35-turbo (Azure).
+* `default_to_minimum` (`bool`): Whether to default to the minimum token limit if the model is not found.
 
 Returns:
 
 * `int`: The token limit for the model.
 
 Example:
```

### Comparing `openai_messages_token_helper-0.0.4/pyproject.toml` & `openai_messages_token_helper-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "openai-messages-token-helper"
 description = "A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API."
-version = "0.0.4"
+version = "0.0.5"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "openai",
     "tiktoken",
```

### Comparing `openai_messages_token_helper-0.0.4/src/openai_messages_token_helper/images_helper.py` & `openai_messages_token_helper-0.0.5/src/openai_messages_token_helper/images_helper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/src/openai_messages_token_helper/message_builder.py` & `openai_messages_token_helper-0.0.5/src/openai_messages_token_helper/message_builder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/tests/image_large.png` & `openai_messages_token_helper-0.0.5/tests/image_large.png`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/tests/messages.py` & `openai_messages_token_helper-0.0.5/tests/messages.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/tests/test_imageshelper.py` & `openai_messages_token_helper-0.0.5/tests/test_imageshelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/tests/test_messagebuilder.py` & `openai_messages_token_helper-0.0.5/tests/test_messagebuilder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/tests/test_modelhelper.py` & `openai_messages_token_helper-0.0.5/tests/test_modelhelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
 
 def test_get_token_limit_error():
     with pytest.raises(ValueError, match="Called with unknown model name: gpt-3"):
         get_token_limit("gpt-3")
 
 
+def test_get_token_limit_default(caplog):
+    with caplog.at_level("WARNING"):
+        assert get_token_limit("gpt-3", default_to_minimum=True) == 4000
+        assert "Model gpt-3 not found, defaulting to minimum token limit 4000" in caplog.text
+
+
 # parameterize the model and the expected number of tokens
 @pytest.mark.parametrize(
     "model",
     [
         "gpt-35-turbo",
         "gpt-3.5-turbo",
         "gpt-35-turbo-16k",
@@ -54,18 +60,21 @@
         "content": {"key": "value"},
     }
     model = "gpt-35-turbo"
     with pytest.raises(ValueError, match="Could not encode unsupported message value type"):
         count_tokens_for_message(model, message)
 
 
-def test_get_oai_chatmodel_tiktok_error():
-    message = {
-        "role": "user",
-        "content": "hello",
-    }
+def test_count_tokens_for_message_model_error():
     with pytest.raises(ValueError, match="Expected valid OpenAI GPT model name"):
-        count_tokens_for_message("", message)
+        count_tokens_for_message("", user_message["message"])
     with pytest.raises(ValueError, match="Expected valid OpenAI GPT model name"):
-        count_tokens_for_message(None, message)
+        count_tokens_for_message(None, user_message["message"])
     with pytest.raises(ValueError, match="Expected valid OpenAI GPT model name"):
-        count_tokens_for_message("gpt44", message)
+        count_tokens_for_message("gpt44", user_message["message"])
+
+
+def test_count_tokens_for_message_model_default(caplog):
+    model = "phi-3"
+    with caplog.at_level("WARNING"):
+        assert count_tokens_for_message(model, user_message["message"], default_to_cl100k=True) == user_message["count"]
+        assert "Model phi-3 not found, defaulting to CL100k encoding" in caplog.text
```

### Comparing `openai_messages_token_helper-0.0.4/tests/verify_openai.py` & `openai_messages_token_helper-0.0.5/tests/verify_openai.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.4/PKG-INFO` & `openai_messages_token_helper-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-messages-token-helper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API.
 Author: Pamela Fox
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -103,14 +103,16 @@
 ### `count_tokens_for_message`
 
 Counts the number of tokens in a message.
 
 Arguments:
 
 * `model` (`str`): The model name to use for token calculation, like gpt-3.5-turbo.
+* `message` (`dict`): The message to count tokens for.
+* `default_to_cl100k` (`bool`): Whether to default to the CL100k token limit if the model is not found.
 
 Returns:
 
 * `int`: The number of tokens in the message.
 
 Example:
 
@@ -153,14 +155,15 @@
 ### `get_token_limit`
 
 Get the token limit for a given GPT model name (OpenAI.com or Azure OpenAI supported).
 
 Arguments:
 
 * `model` (`str`): The model name to use for token calculation, like gpt-3.5-turbo (OpenAI.com) or gpt-35-turbo (Azure).
+* `default_to_minimum` (`bool`): Whether to default to the minimum token limit if the model is not found.
 
 Returns:
 
 * `int`: The token limit for the model.
 
 Example:
```

