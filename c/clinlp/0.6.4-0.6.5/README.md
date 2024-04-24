# Comparing `tmp/clinlp-0.6.4.tar.gz` & `tmp/clinlp-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.6.4.tar", max compression
+gzip compressed data, was "clinlp-0.6.5.tar", max compression
```

## Comparing `clinlp-0.6.4.tar` & `clinlp-0.6.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2024-02-13 10:08:44.902416 clinlp-0.6.4/LICENSE
--rw-r--r--   0        0        0    14976 2024-02-13 10:08:44.902416 clinlp-0.6.4/README.md
--rw-r--r--   0        0        0      309 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/__init__.py
--rw-r--r--   0        0        0     7962 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/entity.py
--rw-r--r--   0        0        0       48 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/exceptions.py
--rw-r--r--   0        0        0     9019 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/language.py
--rw-r--r--   0        0        0     1656 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/normalizer.py
--rw-r--r--   0        0        0      361 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/qualifier/__init__.py
--rw-r--r--   0        0        0    12368 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/qualifier/context_algorithm.py
--rw-r--r--   0        0        0     4014 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/qualifier/qualifier.py
--rw-r--r--   0        0        0     5300 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/qualifier/transformer.py
--rw-r--r--   0        0        0        0 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/resources/__init__.py
--rw-r--r--   0        0        0    26538 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/resources/context_rules.json
--rw-r--r--   0        0        0     2412 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/sentencizer.py
--rw-r--r--   0        0        0     1939 2024-02-13 10:08:44.902416 clinlp-0.6.4/clinlp/util.py
--rw-r--r--   0        0        0     1033 2024-02-13 10:08:44.906416 clinlp-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    15754 1970-01-01 00:00:00.000000 clinlp-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-24 11:34:44.395123 clinlp-0.6.5/LICENSE
+-rw-r--r--   0        0        0    17270 2024-04-24 11:34:44.395123 clinlp-0.6.5/README.md
+-rw-r--r--   0        0        0      309 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/__init__.py
+-rw-r--r--   0        0        0     7962 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/entity.py
+-rw-r--r--   0        0        0       48 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/exceptions.py
+-rw-r--r--   0        0        0     9019 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/language.py
+-rw-r--r--   0        0        0     1656 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/normalizer.py
+-rw-r--r--   0        0        0      440 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/qualifier/__init__.py
+-rw-r--r--   0        0        0    12368 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/qualifier/context_algorithm.py
+-rw-r--r--   0        0        0     4014 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/qualifier/qualifier.py
+-rw-r--r--   0        0        0     7214 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/qualifier/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    26538 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/resources/context_rules.json
+-rw-r--r--   0        0        0     2412 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/sentencizer.py
+-rw-r--r--   0        0        0     1939 2024-04-24 11:34:44.395123 clinlp-0.6.5/clinlp/util.py
+-rw-r--r--   0        0        0     1033 2024-04-24 11:34:44.399123 clinlp-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    18048 1970-01-01 00:00:00.000000 clinlp-0.6.5/PKG-INFO
```

### Comparing `clinlp-0.6.4/LICENSE` & `clinlp-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/README.md` & `clinlp-0.6.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+[![test](https://github.com/umcu/clinlp/actions/workflows/test.yml/badge.svg)](https://github.com/umcu/clinlp/actions/workflows/test.yml)
+[![pypi version](https://img.shields.io/pypi/v/clinlp?color=blue)](https://pypi.org/project/clinlp/)
+[![pypi python versions](https://img.shields.io/pypi/pyversions/clinlp)](https://pypi.org/project/clinlp/)
+[![license](https://img.shields.io/github/license/umcu/clinlp?color=blue)](https://github.com/umcu/clinlp/blob/main/LICENSE)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # clinlp
 
 ![clinlp](media/clinlp.png)
 
 * :hospital: `clinical` + :netherlands: `nl` + :clipboard: `NLP` = :sparkles: `clinlp`
 * :star: Performant and production-ready NLP pipelines for clinical text written in Dutch
 * :rocket: Open source, created and maintained by the Dutch Clinical NLP community
 * :triangular_ruler: Useful out of the box, but customization highly recommended
 
-Read the [principles and goals](#principles-and-goals), futher down :arrow_down:
-
-## Contact and contributing
+If you are enthusiastic about using or contributing to `clinlp`, please don't hesitate to get in touch (via [e-mail](mailto:analytics@umcutrecht.nl) or by creating an [issue](https://github.com/umcu/clinlp/issues/new)). `clinlp` is intended as a community project, and we would love to hear from you. 
 
-`clinlp` is very much still being shaped, so if you are enthusiastic about using or contributing to `clinlp`, please don't hesitate to get in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new)). We would be very happy to discuss your ideas and needs, whether its from the perspective of an (end) user, engineer or clinician, and formulate a roadmap with next steps together. 
+This readme contains information on [getting started](#getting-started), how to [cite](#citing) this work, some basic [documentation](#documentation), the [roadmap](#roadmap), the overarching [principles and goals](#principles-and-goals) and how to [contribute](#contributing) :arrow_down:.
 
 ## Getting started
 
 ### Installation
 ```bash
 pip install clinlp
 ```
@@ -310,40 +314,49 @@
 
 A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/context_rules.json`](clinlp/resources/context_rules.json) for an example, and load it as follows:
 
 ```python
 cm = nlp.add_pipe("clinlp_context_algorithm", config={"rules": "/path/to/my_own_ruleset.json"})
 ```
 
-#### Transformer based negation detection
+#### Transformer based detection
 
-`clinlp` also includes a wrapper around the transformer based negation detector, as described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformer can be found on [huggingface](https://huggingface.co/UMCU/MedRoBERTa.nl_NegationDetection). It is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
+`clinlp` also includes a wrapper around some trained transformer models for detector qualifiers, including the negation detector described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformers can be found on [huggingface](https://huggingface.co/UMCU/). The negation detector for instnace is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
 
 First, install the additional dependencies:
 
 ```bash
 pip install "clinlp[transformers]"
 ```
 
-Then add it using:
+Currently, the following components are available:
 
 ```python
-tn = nlp.add_pipe("clinlp_negation_transformer")
+_ = nlp.add_pipe("clinlp_negation_transformer")
+_ = nlp.add_pipe("clinlp_experiencer_transformer")
 ```
 
 Some configuration options, like the number of tokens to consider, can be specified in the `config` argument. 
 
 
 ### Where to go from here
 
 We hope to extend `clinlp` with new functionality and more complete documentation in the near future. In the meantime, if any questions or problems arise, we recommend:
 
 * Checking the source code 
 * Getting in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new))
 
+## Roadmap
+
+We keep track of work being done on `clinlp` (now and in the future) using GitHub Projects, on this page: [clinlp development roadmap](https://github.com/orgs/umcu/projects/3/views/1). All issues created automatically appear on the roadmap, where they will be triaged and assigned. 
+
+A more high-level overview of the types of NLP tasks that might be implemented in `clinlp`, with those in the current release marked in green, can be found below. This list is non-exhaustive. 
+
+![clinlp-features](media/clinlp-features-v0.6.png)
+
 ## Principles and goals
 
 Functional:
 
 * Provides NLP pipelines optimized for Dutch clinical text
   * Performant and production-ready
   * Useful out-of-the-box, but highly configurable
@@ -363,7 +376,16 @@
 
 Overarching goals:
 
 * Improve the quality of Dutch Clinical NLP pipelines
 * Enable easier (re)use/valorization of efforts
 * Help mature the field of Dutch Clinical NLP
 * Help develop the Dutch Clinical NLP community
+
+## Contributing
+
+`clinlp` is intended as a community project, and as such your contribution is very welcome. We hope to set up some more extensive contributing guidelines in the near future. For now, here is some basic information for starters: 
+
+* PRs are welcome, but if you are planning extensive changes, please do get in touch beforehand. This holds both for your own ideas, and for items already on our roadmap. 
+* Keep in mind that `clinlp` consists of **generic** components that process **clinical** text written in **Dutch**. If your contribution does not meet those three criteria, a separate release might be a better option. 
+* We aim for production ready code, that is well tested, scalable, maintainable, SOLID, etc., but we can help with refactoring code to reach that point. 
+* We try to use [issues](https://github.com/umcu/clinlp/issues/new) for communication as much as possible, but you can reach the maintainers by [e-mail](mailto:analytics@umcutrecht.nl) if that doesn't work.
```

### Comparing `clinlp-0.6.4/clinlp/entity.py` & `clinlp-0.6.5/clinlp/entity.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/language.py` & `clinlp-0.6.5/clinlp/language.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/normalizer.py` & `clinlp-0.6.5/clinlp/normalizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/qualifier/context_algorithm.py` & `clinlp-0.6.5/clinlp/qualifier/context_algorithm.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/qualifier/qualifier.py` & `clinlp-0.6.5/clinlp/qualifier/qualifier.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/resources/context_rules.json` & `clinlp-0.6.5/clinlp/resources/context_rules.json`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/sentencizer.py` & `clinlp-0.6.5/clinlp/sentencizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/clinlp/util.py` & `clinlp-0.6.5/clinlp/util.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.4/pyproject.toml` & `clinlp-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinlp"
-version = "0.6.4"
+version = "0.6.5"
 description = "Performant and production-ready NLP pipelines for clinical text written in Dutch"
 authors = ["UMCU DIT Analytics <analytics@umcutrecht.nl>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 spacy = "^3.5.3"
```

### Comparing `clinlp-0.6.4/PKG-INFO` & `clinlp-0.6.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.6.4
+Version: 0.6.5
 Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
 Author: UMCU DIT Analytics
 Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,28 +14,32 @@
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: transformers[torch] (>=4.30.2,<5.0.0) ; extra == "transformers"
 Description-Content-Type: text/markdown
 
+[![test](https://github.com/umcu/clinlp/actions/workflows/test.yml/badge.svg)](https://github.com/umcu/clinlp/actions/workflows/test.yml)
+[![pypi version](https://img.shields.io/pypi/v/clinlp?color=blue)](https://pypi.org/project/clinlp/)
+[![pypi python versions](https://img.shields.io/pypi/pyversions/clinlp)](https://pypi.org/project/clinlp/)
+[![license](https://img.shields.io/github/license/umcu/clinlp?color=blue)](https://github.com/umcu/clinlp/blob/main/LICENSE)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 # clinlp
 
 ![clinlp](media/clinlp.png)
 
 * :hospital: `clinical` + :netherlands: `nl` + :clipboard: `NLP` = :sparkles: `clinlp`
 * :star: Performant and production-ready NLP pipelines for clinical text written in Dutch
 * :rocket: Open source, created and maintained by the Dutch Clinical NLP community
 * :triangular_ruler: Useful out of the box, but customization highly recommended
 
-Read the [principles and goals](#principles-and-goals), futher down :arrow_down:
-
-## Contact and contributing
+If you are enthusiastic about using or contributing to `clinlp`, please don't hesitate to get in touch (via [e-mail](mailto:analytics@umcutrecht.nl) or by creating an [issue](https://github.com/umcu/clinlp/issues/new)). `clinlp` is intended as a community project, and we would love to hear from you. 
 
-`clinlp` is very much still being shaped, so if you are enthusiastic about using or contributing to `clinlp`, please don't hesitate to get in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new)). We would be very happy to discuss your ideas and needs, whether its from the perspective of an (end) user, engineer or clinician, and formulate a roadmap with next steps together. 
+This readme contains information on [getting started](#getting-started), how to [cite](#citing) this work, some basic [documentation](#documentation), the [roadmap](#roadmap), the overarching [principles and goals](#principles-and-goals) and how to [contribute](#contributing) :arrow_down:.
 
 ## Getting started
 
 ### Installation
 ```bash
 pip install clinlp
 ```
@@ -330,40 +334,49 @@
 
 A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/context_rules.json`](clinlp/resources/context_rules.json) for an example, and load it as follows:
 
 ```python
 cm = nlp.add_pipe("clinlp_context_algorithm", config={"rules": "/path/to/my_own_ruleset.json"})
 ```
 
-#### Transformer based negation detection
+#### Transformer based detection
 
-`clinlp` also includes a wrapper around the transformer based negation detector, as described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformer can be found on [huggingface](https://huggingface.co/UMCU/MedRoBERTa.nl_NegationDetection). It is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
+`clinlp` also includes a wrapper around some trained transformer models for detector qualifiers, including the negation detector described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformers can be found on [huggingface](https://huggingface.co/UMCU/). The negation detector for instnace is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
 
 First, install the additional dependencies:
 
 ```bash
 pip install "clinlp[transformers]"
 ```
 
-Then add it using:
+Currently, the following components are available:
 
 ```python
-tn = nlp.add_pipe("clinlp_negation_transformer")
+_ = nlp.add_pipe("clinlp_negation_transformer")
+_ = nlp.add_pipe("clinlp_experiencer_transformer")
 ```
 
 Some configuration options, like the number of tokens to consider, can be specified in the `config` argument. 
 
 
 ### Where to go from here
 
 We hope to extend `clinlp` with new functionality and more complete documentation in the near future. In the meantime, if any questions or problems arise, we recommend:
 
 * Checking the source code 
 * Getting in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new))
 
+## Roadmap
+
+We keep track of work being done on `clinlp` (now and in the future) using GitHub Projects, on this page: [clinlp development roadmap](https://github.com/orgs/umcu/projects/3/views/1). All issues created automatically appear on the roadmap, where they will be triaged and assigned. 
+
+A more high-level overview of the types of NLP tasks that might be implemented in `clinlp`, with those in the current release marked in green, can be found below. This list is non-exhaustive. 
+
+![clinlp-features](media/clinlp-features-v0.6.png)
+
 ## Principles and goals
 
 Functional:
 
 * Provides NLP pipelines optimized for Dutch clinical text
   * Performant and production-ready
   * Useful out-of-the-box, but highly configurable
@@ -384,7 +397,16 @@
 Overarching goals:
 
 * Improve the quality of Dutch Clinical NLP pipelines
 * Enable easier (re)use/valorization of efforts
 * Help mature the field of Dutch Clinical NLP
 * Help develop the Dutch Clinical NLP community
 
+## Contributing
+
+`clinlp` is intended as a community project, and as such your contribution is very welcome. We hope to set up some more extensive contributing guidelines in the near future. For now, here is some basic information for starters: 
+
+* PRs are welcome, but if you are planning extensive changes, please do get in touch beforehand. This holds both for your own ideas, and for items already on our roadmap. 
+* Keep in mind that `clinlp` consists of **generic** components that process **clinical** text written in **Dutch**. If your contribution does not meet those three criteria, a separate release might be a better option. 
+* We aim for production ready code, that is well tested, scalable, maintainable, SOLID, etc., but we can help with refactoring code to reach that point. 
+* We try to use [issues](https://github.com/umcu/clinlp/issues/new) for communication as much as possible, but you can reach the maintainers by [e-mail](mailto:analytics@umcutrecht.nl) if that doesn't work.
+
```

