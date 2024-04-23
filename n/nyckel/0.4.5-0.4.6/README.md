# Comparing `tmp/nyckel-0.4.5.tar.gz` & `tmp/nyckel-0.4.6.tar.gz`

## Comparing `nyckel-0.4.5.tar` & `nyckel-0.4.6.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.5/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.5/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.5/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.5/.vscode/extensions.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.5/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/credentials.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/image_classification.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/image_tags.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/merge_labels.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/data_classes.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/image_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    14225 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/image_tags.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tabular_tags.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/conftest.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_field_handler.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_image_decoder.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_image_tags_function.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_sample_handler.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_tabular_tags_function.py
--rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_tags_shared.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_text_classification_function.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_white_background.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/fixtures/flower.jpg
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/fixtures/mixed-alpha-background.png
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.5/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.5/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 nyckel-0.4.6/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.6/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.6/.vscode/extensions.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.6/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/credentials.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/image_classification.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/image_tags.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/merge_labels.md
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/tabular_classification.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/tabular_tags.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.6/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/image_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    14225 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/image_tags.py
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/tabular_tags.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.6/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_image_tags_function.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_tabular_tags_function.py
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_tags_shared.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.6/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.6/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.6/PKG-INFO
```

### Comparing `nyckel-0.4.5/mkdocs.yml` & `nyckel-0.4.6/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     - Merge labels: merge_labels.md
     - Delete samples: delete_samples.md
     - Multimodal classification: multimodal_classification.md
   - Reference:
     - Image Classification: image_classification.md
     - Text Classification: text_classification.md
     - Tabular Classification: tabular_classification.md
-    - Text Tags: text_tags.md
     - Image Tags: image_tags.md
+    - Text Tags: text_tags.md
+    - Tabular Tags: tabular_tags.md
     - Credentials: credentials.md
     - Data classes: data_classes.md
 theme: 
   name: 'material'
   features:
     - content.code.copy
   logo: assets/nyckel-logo.png
```

### Comparing `nyckel-0.4.5/.github/workflows/build.yml` & `nyckel-0.4.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/.github/workflows/docs.yml` & `nyckel-0.4.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/.github/workflows/test.yml` & `nyckel-0.4.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/.vscode/settings.json` & `nyckel-0.4.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/copy_function.md` & `nyckel-0.4.6/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/delete_label.md` & `nyckel-0.4.6/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/delete_samples.md` & `nyckel-0.4.6/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/index.md` & `nyckel-0.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/merge_labels.md` & `nyckel-0.4.6/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/quickstart.md` & `nyckel-0.4.6/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/assets/favicon.ico` & `nyckel-0.4.6/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/docs/assets/nyckel-logo.png` & `nyckel-0.4.6/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/__init__.py` & `nyckel-0.4.6/src/nyckel/__init__.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/auth.py` & `nyckel-0.4.6/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/image_processing.py` & `nyckel-0.4.6/src/nyckel/image_processing.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/request_utils.py` & `nyckel-0.4.6/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/utils.py` & `nyckel-0.4.6/src/nyckel/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.6/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.6/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.6/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.6/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.6/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.6/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.6/src/nyckel/functions/classification/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.6/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/image_tags.py` & `nyckel-0.4.6/src/nyckel/functions/tags/image_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     func = ImageTagsFunction.create("ClothingColor", credentials)
     func.create_samples([
         ImageTagsSample(data="t-shirt1.jpg", annotation=[TagsAnnotation("White"), TagsAnnotation("Blue")]),
         ImageTagsSample(data="t=shirt2.jpg", annotation=[TagsAnnotation("Red"), TagsAnnotation("White")]),
         ImageTagsSample(data="jacket.jpg", annotation=[TagsAnnotation("Black")]),
         ImageTagsSample(data="jeans.jpg", annotation=[TagsAnnotation("Blue")]),
     ])
+
     predictions = func.invoke(["new-jacket.jpg"])
     ```
     """
 
     def __init__(self, function_id: NyckelId, credentials: Credentials):
         self._function_id = function_id
```

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/tabular_tags.py` & `nyckel-0.4.6/src/nyckel/functions/tags/tabular_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,14 +120,38 @@
 
     @abc.abstractmethod
     def delete_samples(self, sample_ids: List[NyckelId]) -> None:
         pass
 
 
 class TabularTagsFunction(TabularTagsFunctionInterface):
+    """
+    Example:
+
+    ```py
+
+    from nyckel import Credentials, TabularTagsFunction, TabularTagsSample, TagsAnnotation, TabularFunctionField
+
+    credentials = Credentials(client_id="...", client_secret="...")
+
+    func = TabularTagsFunction.create("NewsTopics", credentials)
+    func.create_fields([
+        TabularFunctionField(type="Text", name="Title"),
+        TabularFunctionField(type="Text", name="Abstract")
+    ])
+    func.create_samples([
+        TabularTagsSample(data={"Title": "New restaurant in SOHO", "Abstract": "This is the best..."}, annotation=[TagsAnnotation("Food"), TagsAnnotation("Reviews")]),
+        TabularTagsSample(data={"Title": "Belly-up still going strong", "Abstract": "The Belly-Up tavern in Solana..."}, annotation=[TagsAnnotation("Music"), TagsAnnotation("Reviews")]),
+        TabularTagsSample(data={"Title": "Carbonara at its best", "Abstract": "Here is how to make the best..."}, annotation=[TagsAnnotation("Food")]),
+        TabularTagsSample(data={"Title": "New album out!", "Abstract": "Taylor swift just released ..."}, annotation=[TagsAnnotation("Music")]),
+    ])
+
+    predictions = func.invoke([{"Title": "Swedish meatballs: the best recipe", "Abstract": "This age-old Swedish classic ..."}])
+    ```
+    """
 
     def __init__(self, function_id: NyckelId, credentials: Credentials):
         self._function_id = function_id
 
         self._function_handler = TagsFunctionHandler(function_id, credentials)
         self._label_handler = ClassificationLabelHandler(function_id, credentials)
         self._url_handler = TagsFunctionURLHandler(function_id, credentials.server_url)
```

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.6/src/nyckel/functions/tags/tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.6/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.6/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.6/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.6/src/nyckel/functions/tags/text_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/conftest.py` & `nyckel-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_duplicates_handling.py` & `nyckel-0.4.6/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_field_handler.py` & `nyckel-0.4.6/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_image_classification_function.py` & `nyckel-0.4.6/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_image_decoder.py` & `nyckel-0.4.6/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_image_tags_function.py` & `nyckel-0.4.6/tests/test_image_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_label_handler.py` & `nyckel-0.4.6/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_sample_handler.py` & `nyckel-0.4.6/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_tabular_classification_function.py` & `nyckel-0.4.6/tests/test_tabular_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_tabular_tags_function.py` & `nyckel-0.4.6/tests/test_tabular_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_tags_shared.py` & `nyckel-0.4.6/tests/test_tags_shared.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_text_classification_function.py` & `nyckel-0.4.6/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/test_white_background.py` & `nyckel-0.4.6/tests/test_white_background.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/fixtures/flower.jpg` & `nyckel-0.4.6/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/tests/fixtures/mixed-alpha-background.png` & `nyckel-0.4.6/tests/fixtures/mixed-alpha-background.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/.gitignore` & `nyckel-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/LICENSE` & `nyckel-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/README.md` & `nyckel-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.5/pyproject.toml` & `nyckel-0.4.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.4.5"
+version = "0.4.6"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.4.5/PKG-INFO` & `nyckel-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

