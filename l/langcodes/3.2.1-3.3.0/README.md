# Comparing `tmp/langcodes-3.2.1.tar.gz` & `tmp/langcodes-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcodes-3.2.1.tar", last modified: Tue Oct  5 17:23:58 2021, max compression
+gzip compressed data, was "langcodes-3.3.0.tar", max compression
```

## Comparing `langcodes-3.2.1.tar` & `langcodes-3.3.0.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxrwxr-x   0 elia      (1000) elia      (1000)        0 2021-10-05 17:23:58.437632 langcodes-3.2.1/
--rw-rw-r--   0 elia      (1000) elia      (1000)     1090 2021-09-10 14:12:24.000000 langcodes-3.2.1/LICENSE.txt
--rw-rw-r--   0 elia      (1000) elia      (1000)      125 2021-10-04 20:46:17.000000 langcodes-3.2.1/MANIFEST.in
--rw-rw-r--   0 elia      (1000) elia      (1000)     1220 2021-10-05 17:23:58.437632 langcodes-3.2.1/PKG-INFO
--rw-rw-r--   0 elia      (1000) elia      (1000)    28326 2021-10-05 15:04:53.000000 langcodes-3.2.1/README.md
-drwxrwxr-x   0 elia      (1000) elia      (1000)        0 2021-10-05 17:23:58.437632 langcodes-3.2.1/langcodes/
--rw-rw-r--   0 elia      (1000) elia      (1000)    69111 2021-10-05 15:05:25.000000 langcodes-3.2.1/langcodes/__init__.py
--rw-rw-r--   0 elia      (1000) elia      (1000)     9965 2021-10-05 14:46:48.000000 langcodes-3.2.1/langcodes/build_data.py
-drwxrwxr-x   0 elia      (1000) elia      (1000)        0 2021-10-05 17:23:58.437632 langcodes-3.2.1/langcodes/data/
--rw-rw-r--   0 elia      (1000) elia      (1000)   715867 2021-10-01 19:19:56.000000 langcodes-3.2.1/langcodes/data/language-subtag-registry.txt
--rw-rw-r--   0 elia      (1000) elia      (1000)   110962 2021-10-04 21:54:54.000000 langcodes-3.2.1/langcodes/data_dicts.py
--rw-rw-r--   0 elia      (1000) elia      (1000)     5751 2021-09-10 14:12:24.000000 langcodes-3.2.1/langcodes/language_distance.py
--rw-rw-r--   0 elia      (1000) elia      (1000)     8650 2021-09-10 14:12:24.000000 langcodes-3.2.1/langcodes/language_lists.py
--rw-rw-r--   0 elia      (1000) elia      (1000)        0 2021-09-10 14:12:24.000000 langcodes-3.2.1/langcodes/py.typed
--rw-rw-r--   0 elia      (1000) elia      (1000)     1785 2021-09-10 14:12:24.000000 langcodes-3.2.1/langcodes/registry_parser.py
--rw-rw-r--   0 elia      (1000) elia      (1000)    14283 2021-10-05 15:15:20.000000 langcodes-3.2.1/langcodes/tag_parser.py
--rw-rw-r--   0 elia      (1000) elia      (1000)      182 2021-09-10 14:12:24.000000 langcodes-3.2.1/langcodes/util.py
-drwxrwxr-x   0 elia      (1000) elia      (1000)        0 2021-10-05 17:23:58.437632 langcodes-3.2.1/langcodes.egg-info/
--rw-rw-r--   0 elia      (1000) elia      (1000)     1220 2021-10-05 17:23:58.000000 langcodes-3.2.1/langcodes.egg-info/PKG-INFO
--rw-rw-r--   0 elia      (1000) elia      (1000)      511 2021-10-05 17:23:58.000000 langcodes-3.2.1/langcodes.egg-info/SOURCES.txt
--rw-rw-r--   0 elia      (1000) elia      (1000)        1 2021-10-05 17:23:58.000000 langcodes-3.2.1/langcodes.egg-info/dependency_links.txt
--rw-rw-r--   0 elia      (1000) elia      (1000)        1 2021-09-10 18:12:59.000000 langcodes-3.2.1/langcodes.egg-info/not-zip-safe
--rw-rw-r--   0 elia      (1000) elia      (1000)       29 2021-10-05 17:23:58.000000 langcodes-3.2.1/langcodes.egg-info/requires.txt
--rw-rw-r--   0 elia      (1000) elia      (1000)       10 2021-10-05 17:23:58.000000 langcodes-3.2.1/langcodes.egg-info/top_level.txt
--rw-rw-r--   0 elia      (1000) elia      (1000)       69 2021-10-05 17:23:58.437632 langcodes-3.2.1/setup.cfg
--rw-rw-r--   0 elia      (1000) elia      (1000)     1676 2021-10-04 22:59:31.000000 langcodes-3.2.1/setup.py
+-rw-r--r--   0        0        0     1090 2021-09-10 14:12:24.580176 langcodes-3.3.0/LICENSE.txt
+-rw-r--r--   0        0        0    28784 2021-11-11 20:49:06.996805 langcodes-3.3.0/README.md
+-rw-r--r--   0        0        0    69456 2021-11-11 20:49:06.996805 langcodes-3.3.0/langcodes/__init__.py
+-rw-r--r--   0        0        0    10120 2021-11-11 20:49:07.000805 langcodes-3.3.0/langcodes/build_data.py
+-rw-r--r--   0        0        0   715867 2021-10-01 19:19:56.746708 langcodes-3.3.0/langcodes/data/language-subtag-registry.txt
+-rw-r--r--   0        0        0   113788 2021-11-11 20:49:07.000805 langcodes-3.3.0/langcodes/data_dicts.py
+-rw-r--r--   0        0        0     5751 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/language_distance.py
+-rw-r--r--   0        0        0     8650 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/language_lists.py
+-rw-r--r--   0        0        0        0 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/py.typed
+-rw-r--r--   0        0        0     1785 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/registry_parser.py
+-rw-r--r--   0        0        0    14283 2021-11-11 20:49:07.000805 langcodes-3.3.0/langcodes/tag_parser.py
+-rw-r--r--   0        0        0      239 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/tests/README.md
+-rw-r--r--   0        0        0      797 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/tests/test_alpha3.py
+-rw-r--r--   0        0        0      227 2021-11-11 20:49:07.000805 langcodes-3.3.0/langcodes/tests/test_language_data.py
+-rw-r--r--   0        0        0      784 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/tests/test_wikt_languages.py
+-rw-r--r--   0        0        0      182 2021-09-10 14:12:24.584176 langcodes-3.3.0/langcodes/util.py
+-rw-r--r--   0        0        0      662 2021-11-11 20:49:07.000805 langcodes-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    30813 2021-11-11 20:50:55.528219 langcodes-3.3.0/setup.py
+-rw-r--r--   0        0        0    29520 2021-11-11 20:50:55.529740 langcodes-3.3.0/PKG-INFO
```

### Comparing `langcodes-3.2.1/LICENSE.txt` & `langcodes-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langcodes-3.2.1/README.md` & `langcodes-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -634,14 +634,28 @@
 
 [Code with documentation][code]
 
 [code]: https://github.com/rspeer/langcodes/blob/master/langcodes/__init__.py
 
 # Changelog
 
+## Version 3.3 (November 2021)
+
+- Updated to CLDR v40.
+
+- Updated the IANA subtag registry to version 2021-08-06.
+
+- Bug fix: recognize script codes that appear in the IANA registry even if
+  they're missing from CLDR for some reason. 'cu-Cyrs' is valid, for example.
+
+- Switched the build system from `setuptools` to `poetry`.
+
+To install the package in editable mode before PEP 660 is better supported, use
+`poetry install` instead of `pip install -e .`.
+
 ## Version 3.2 (October 2021)
 
 - Supports Python 3.6 through 3.10.
 
 - Added the top-level function `tag_is_valid(tag)`, for determining if a string
   is a valid language tag without having to parse it first.
```

### Comparing `langcodes-3.2.1/langcodes/__init__.py` & `langcodes-3.3.0/langcodes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import Any, List, Tuple, Dict, Sequence, Iterable, Optional, Mapping, Union
 import warnings
 import sys
 
 from langcodes.tag_parser import LanguageTagError, parse_tag, normalize_characters
 from langcodes.language_distance import tuple_distance_cached
 from langcodes.data_dicts import (
+    ALL_SCRIPTS,
     DEFAULT_SCRIPTS,
     LANGUAGE_REPLACEMENTS,
     LANGUAGE_ALPHA3,
     LANGUAGE_ALPHA3_BIBLIOGRAPHIC,
     TERRITORY_REPLACEMENTS,
     NORMALIZED_MACROLANGUAGES,
     LIKELY_SUBTAGS,
@@ -726,15 +727,15 @@
 
     def is_valid(self) -> bool:
         """
         Checks whether the language, script, territory, and variants
         (if present) are all tags that have meanings assigned by IANA.
         For example, 'ja' (Japanese) is a valid tag, and 'jp' is not.
 
-        The data is current as of CLDR 38.1.
+        The data is current as of CLDR 40.
 
         >>> Language.get('ja').is_valid()
         True
         >>> Language.get('jp').is_valid()
         False
         >>> Language.get('en-001').is_valid()
         True
@@ -749,14 +750,22 @@
         >>> Language.get('en-GB-oxendict').is_valid()
         True
         >>> Language.get('en-GB-oxenfree').is_valid()
         False
         >>> Language.get('x-heptapod').is_valid()
         True
 
+        Some scripts are, confusingly, not included in CLDR's 'validity' pattern.
+        If a script appears in the IANA registry, we consider it valid.
+
+        >>> Language.get('ur-Aran').is_valid()
+        True
+        >>> Language.get('cu-Cyrs').is_valid()
+        True
+
         A language tag with multiple extlangs will parse, but is not valid.
         The only allowed example is 'zh-min-nan', which normalizes to the
         language 'nan'.
 
         >>> Language.get('zh-min-nan').is_valid()
         True
         >>> Language.get('sgn-ase-bfi').is_valid()
@@ -791,15 +800,16 @@
         checked_subtags = []
         if self.variants is not None:
             subtags.extend(self.variants)
         for subtag in subtags:
             if subtag is not None:
                 checked_subtags.append(subtag)
                 if not subtag.startswith('x-') and not VALIDITY.match(subtag):
-                    return False
+                    if subtag not in ALL_SCRIPTS:
+                        return False
 
         # We check extensions for validity by ensuring that there aren't
         # two extensions introduced by the same letter. For example, you can't
         # have two 'u-' extensions.
         if self.extensions:
             checked_subtags.extend([extension[:2] for extension in self.extensions])
         if len(set(checked_subtags)) != len(checked_subtags):
```

### Comparing `langcodes-3.2.1/langcodes/build_data.py` & `langcodes-3.3.0/langcodes/build_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import json
 import xml.etree.ElementTree as ET
-import sys
-import os
-from pathlib import Path
-from collections import defaultdict, Counter
-
-import langcodes
 from langcodes.util import data_filename
-from langcodes.language_lists import CLDR_LANGUAGES
 from langcodes.registry_parser import parse_registry
 
 
 def read_cldr_supplemental(dataname):
     cldr_supp_path = data_filename('cldr-json/cldr-json/cldr-core/supplemental')
     filename = data_filename(f'{cldr_supp_path}/{dataname}.json')
     fulldata = json.load(open(filename, encoding='utf-8'))
     if dataname == 'aliases':
         data = fulldata['supplemental']['metadata']['alias']
     else:
         data = fulldata['supplemental'][dataname]
     return data
 
 
-def read_iana_registry_scripts():
+def read_iana_registry_suppress_scripts():
     scripts = {}
     for entry in parse_registry():
         if entry['Type'] == 'language' and 'Suppress-Script' in entry:
             scripts[entry['Subtag']] = entry['Suppress-Script']
     return scripts
 
 
+def read_iana_registry_scripts():
+    scripts = set()
+    for entry in parse_registry():
+        if entry['Type'] == 'script':
+            scripts.add(entry['Subtag'])
+    return scripts
+
+
 def read_iana_registry_macrolanguages():
     macros = {}
     for entry in parse_registry():
         if entry['Type'] == 'language' and 'Macrolanguage' in entry:
             macros[entry['Subtag']] = entry['Macrolanguage']
     return macros
 
@@ -132,15 +133,16 @@
                         desired_distance = tag_distances.setdefault(desired, {})
                         desired_distance[supported] = int(attribs['distance']) + 1
 
     return tag_distances
 
 
 def build_data():
-    lang_scripts = read_iana_registry_scripts()
+    lang_scripts = read_iana_registry_suppress_scripts()
+    all_scripts = read_iana_registry_scripts()
     macrolanguages = read_iana_registry_macrolanguages()
     iana_replacements = read_iana_registry_replacements()
     language_distances = read_language_distances()
 
     alias_data = read_cldr_supplemental('aliases')
     likely_subtags = read_cldr_supplemental('likelySubtags')
     replacements = {}
@@ -221,14 +223,15 @@
         write_python_dict(outfile, 'DEFAULT_SCRIPTS', lang_scripts)
         write_python_dict(
             outfile, 'LANGUAGE_REPLACEMENTS', replacements['languageAlias']
         )
         write_python_dict(outfile, 'LANGUAGE_ALPHA3', alpha3_mapping)
         write_python_dict(outfile, 'LANGUAGE_ALPHA3_BIBLIOGRAPHIC', alpha3_biblio)
         write_python_dict(outfile, 'SCRIPT_REPLACEMENTS', replacements['scriptAlias'])
+        write_python_set(outfile, 'ALL_SCRIPTS', all_scripts)
         write_python_dict(
             outfile, 'TERRITORY_REPLACEMENTS', replacements['territoryAlias']
         )
         write_python_dict(outfile, 'MACROLANGUAGES', macrolanguages)
         write_python_dict(outfile, 'NORMALIZED_MACROLANGUAGES', norm_macrolanguages)
         write_python_dict(outfile, 'LIKELY_SUBTAGS', likely_subtags)
         write_python_dict(outfile, 'LANGUAGE_DISTANCES', language_distances)
```

### Comparing `langcodes-3.2.1/langcodes/data/language-subtag-registry.txt` & `langcodes-3.3.0/langcodes/data/language-subtag-registry.txt`

 * *Files identical despite different names*

### Comparing `langcodes-3.2.1/langcodes/data_dicts.py` & `langcodes-3.3.0/langcodes/data_dicts.py`

 * *Files 1% similar despite different names*

```diff
@@ -777,14 +777,225 @@
     'sk': 'slo',
     'sq': 'alb',
     'zh': 'chi',
 }
 SCRIPT_REPLACEMENTS = {
     'qaai': 'Zinh',
 }
+ALL_SCRIPTS = {
+    'Adlm',
+    'Afak',
+    'Aghb',
+    'Ahom',
+    'Arab',
+    'Aran',
+    'Armi',
+    'Armn',
+    'Avst',
+    'Bali',
+    'Bamu',
+    'Bass',
+    'Batk',
+    'Beng',
+    'Bhks',
+    'Blis',
+    'Bopo',
+    'Brah',
+    'Brai',
+    'Bugi',
+    'Buhd',
+    'Cakm',
+    'Cans',
+    'Cari',
+    'Cham',
+    'Cher',
+    'Chrs',
+    'Cirt',
+    'Copt',
+    'Cpmn',
+    'Cprt',
+    'Cyrl',
+    'Cyrs',
+    'Deva',
+    'Diak',
+    'Dogr',
+    'Dsrt',
+    'Dupl',
+    'Egyd',
+    'Egyh',
+    'Egyp',
+    'Elba',
+    'Elym',
+    'Ethi',
+    'Geok',
+    'Geor',
+    'Glag',
+    'Gong',
+    'Gonm',
+    'Goth',
+    'Gran',
+    'Grek',
+    'Gujr',
+    'Guru',
+    'Hanb',
+    'Hang',
+    'Hani',
+    'Hano',
+    'Hans',
+    'Hant',
+    'Hatr',
+    'Hebr',
+    'Hira',
+    'Hluw',
+    'Hmng',
+    'Hmnp',
+    'Hrkt',
+    'Hung',
+    'Inds',
+    'Ital',
+    'Jamo',
+    'Java',
+    'Jpan',
+    'Jurc',
+    'Kali',
+    'Kana',
+    'Khar',
+    'Khmr',
+    'Khoj',
+    'Kitl',
+    'Kits',
+    'Knda',
+    'Kore',
+    'Kpel',
+    'Kthi',
+    'Lana',
+    'Laoo',
+    'Latf',
+    'Latg',
+    'Latn',
+    'Leke',
+    'Lepc',
+    'Limb',
+    'Lina',
+    'Linb',
+    'Lisu',
+    'Loma',
+    'Lyci',
+    'Lydi',
+    'Mahj',
+    'Maka',
+    'Mand',
+    'Mani',
+    'Marc',
+    'Maya',
+    'Medf',
+    'Mend',
+    'Merc',
+    'Mero',
+    'Mlym',
+    'Modi',
+    'Mong',
+    'Moon',
+    'Mroo',
+    'Mtei',
+    'Mult',
+    'Mymr',
+    'Nand',
+    'Narb',
+    'Nbat',
+    'Newa',
+    'Nkdb',
+    'Nkgb',
+    'Nkoo',
+    'Nshu',
+    'Ogam',
+    'Olck',
+    'Orkh',
+    'Orya',
+    'Osge',
+    'Osma',
+    'Ougr',
+    'Palm',
+    'Pauc',
+    'Pcun',
+    'Pelm',
+    'Perm',
+    'Phag',
+    'Phli',
+    'Phlp',
+    'Phlv',
+    'Phnx',
+    'Piqd',
+    'Plrd',
+    'Prti',
+    'Psin',
+    'Qaaa..Qabx',
+    'Ranj',
+    'Rjng',
+    'Rohg',
+    'Roro',
+    'Runr',
+    'Samr',
+    'Sara',
+    'Sarb',
+    'Saur',
+    'Sgnw',
+    'Shaw',
+    'Shrd',
+    'Shui',
+    'Sidd',
+    'Sind',
+    'Sinh',
+    'Sogd',
+    'Sogo',
+    'Sora',
+    'Soyo',
+    'Sund',
+    'Sylo',
+    'Syrc',
+    'Syre',
+    'Syrj',
+    'Syrn',
+    'Tagb',
+    'Takr',
+    'Tale',
+    'Talu',
+    'Taml',
+    'Tang',
+    'Tavt',
+    'Telu',
+    'Teng',
+    'Tfng',
+    'Tglg',
+    'Thaa',
+    'Thai',
+    'Tibt',
+    'Tirh',
+    'Tnsa',
+    'Toto',
+    'Ugar',
+    'Vaii',
+    'Visp',
+    'Vith',
+    'Wara',
+    'Wcho',
+    'Wole',
+    'Xpeo',
+    'Xsux',
+    'Yezi',
+    'Yiii',
+    'Zanb',
+    'Zinh',
+    'Zmth',
+    'Zsye',
+    'Zsym',
+    'Zxxx',
+    'Zyyy',
+    'Zzzz',
+}
 TERRITORY_REPLACEMENTS = {
     '004': 'AF',
     '008': 'AL',
     '010': 'AQ',
     '012': 'DZ',
     '016': 'AS',
     '020': 'AD',
@@ -2098,14 +2309,15 @@
     'bjt': 'bjt-Latn-SN',
     'bjz': 'bjz-Latn-ZZ',
     'bkc': 'bkc-Latn-ZZ',
     'bkm': 'bkm-Latn-CM',
     'bkq': 'bkq-Latn-ZZ',
     'bku': 'bku-Latn-PH',
     'bkv': 'bkv-Latn-ZZ',
+    'blg': 'blg-Latn-MY',
     'blt': 'blt-Tavt-VN',
     'bm': 'bm-Latn-ML',
     'bmh': 'bmh-Latn-ZZ',
     'bmk': 'bmk-Latn-ZZ',
     'bmq': 'bmq-Latn-ML',
     'bmu': 'bmu-Latn-ZZ',
     'bn': 'bn-Beng-BD',
@@ -2409,15 +2621,15 @@
     'hil': 'hil-Latn-PH',
     'hla': 'hla-Latn-ZZ',
     'hlu': 'hlu-Hluw-TR',
     'hmd': 'hmd-Plrd-CN',
     'hmt': 'hmt-Latn-ZZ',
     'hnd': 'hnd-Arab-PK',
     'hne': 'hne-Deva-IN',
-    'hnj': 'hnj-Hmng-LA',
+    'hnj': 'hnj-Hmnp-US',
     'hnn': 'hnn-Latn-PH',
     'hno': 'hno-Arab-PK',
     'ho': 'ho-Latn-PG',
     'hoc': 'hoc-Deva-IN',
     'hoj': 'hoj-Deva-IN',
     'hot': 'hot-Latn-ZZ',
     'hr': 'hr-Latn-HR',
@@ -2499,15 +2711,15 @@
     'kbx': 'kbx-Latn-ZZ',
     'kby': 'kby-Arab-NE',
     'kcg': 'kcg-Latn-NG',
     'kck': 'kck-Latn-ZW',
     'kcl': 'kcl-Latn-ZZ',
     'kct': 'kct-Latn-ZZ',
     'kde': 'kde-Latn-TZ',
-    'kdh': 'kdh-Arab-TG',
+    'kdh': 'kdh-Latn-TG',
     'kdl': 'kdl-Latn-ZZ',
     'kdt': 'kdt-Thai-TH',
     'kea': 'kea-Latn-CV',
     'ken': 'ken-Latn-CM',
     'kez': 'kez-Latn-ZZ',
     'kfo': 'kfo-Latn-CI',
     'kfr': 'kfr-Deva-IN',
@@ -2867,14 +3079,15 @@
     'nqo': 'nqo-Nkoo-GN',
     'nr': 'nr-Latn-ZA',
     'nrb': 'nrb-Latn-ZZ',
     'nsk': 'nsk-Cans-CA',
     'nsn': 'nsn-Latn-ZZ',
     'nso': 'nso-Latn-ZA',
     'nss': 'nss-Latn-ZZ',
+    'nst': 'nst-Tnsa-IN',
     'ntm': 'ntm-Latn-ZZ',
     'ntr': 'ntr-Latn-ZZ',
     'nui': 'nui-Latn-ZZ',
     'nup': 'nup-Latn-ZZ',
     'nus': 'nus-Latn-SS',
     'nuv': 'nuv-Latn-ZZ',
     'nux': 'nux-Latn-ZZ',
@@ -2898,14 +3111,15 @@
     'or': 'or-Orya-IN',
     'oro': 'oro-Latn-ZZ',
     'oru': 'oru-Arab-ZZ',
     'os': 'os-Cyrl-GE',
     'osa': 'osa-Osge-US',
     'ota': 'ota-Arab-ZZ',
     'otk': 'otk-Orkh-MN',
+    'oui': 'oui-Ougr-143',
     'ozm': 'ozm-Latn-ZZ',
     'pa': 'pa-Guru-IN',
     'pa-Arab': 'pa-Arab-PK',
     'pa-PK': 'pa-Arab-PK',
     'pag': 'pag-Latn-PH',
     'pal': 'pal-Phli-IR',
     'pal-Phlp': 'pal-Phlp-CN',
@@ -2952,15 +3166,15 @@
     'raj': 'raj-Deva-IN',
     'rao': 'rao-Latn-ZZ',
     'rcf': 'rcf-Latn-RE',
     'rej': 'rej-Latn-ID',
     'rel': 'rel-Latn-ZZ',
     'res': 'res-Latn-ZZ',
     'rgn': 'rgn-Latn-IT',
-    'rhg': 'rhg-Arab-MM',
+    'rhg': 'rhg-Rohg-MM',
     'ria': 'ria-Latn-IN',
     'rif': 'rif-Tfng-MA',
     'rif-NL': 'rif-Latn-NL',
     'rjs': 'rjs-Deva-NP',
     'rkt': 'rkt-Beng-BD',
     'rm': 'rm-Latn-CH',
     'rmf': 'rmf-Latn-FI',
@@ -3176,14 +3390,15 @@
     'tuq': 'tuq-Latn-ZZ',
     'tvd': 'tvd-Latn-ZZ',
     'tvl': 'tvl-Latn-TV',
     'tvu': 'tvu-Latn-ZZ',
     'twh': 'twh-Latn-ZZ',
     'twq': 'twq-Latn-NE',
     'txg': 'txg-Tang-CN',
+    'txo': 'txo-Toto-IN',
     'ty': 'ty-Latn-PF',
     'tya': 'tya-Latn-ZZ',
     'tyv': 'tyv-Cyrl-RU',
     'tzm': 'tzm-Latn-MA',
     'ubu': 'ubu-Latn-ZZ',
     'udi': 'udi-Aghb-RU',
     'udm': 'udm-Cyrl-RU',
@@ -3308,14 +3523,16 @@
     'und-Cakm': 'ccp-Cakm-BD',
     'und-Cans': 'cr-Cans-CA',
     'und-Cari': 'xcr-Cari-TR',
     'und-Cham': 'cjm-Cham-VN',
     'und-Cher': 'chr-Cher-US',
     'und-Chrs': 'xco-Chrs-UZ',
     'und-Copt': 'cop-Copt-EG',
+    'und-Cpmn': 'und-Cpmn-CY',
+    'und-Cpmn-CY': 'und-Cpmn-CY',
     'und-Cprt': 'grc-Cprt-CY',
     'und-Cyrl': 'ru-Cyrl-RU',
     'und-Cyrl-AL': 'mk-Cyrl-AL',
     'und-Cyrl-BA': 'sr-Cyrl-BA',
     'und-Cyrl-GE': 'os-Cyrl-GE',
     'und-Cyrl-GR': 'mk-Cyrl-GR',
     'und-Cyrl-MD': 'uk-Cyrl-MD',
@@ -3392,15 +3609,15 @@
     'und-Hebr-GB': 'yi-Hebr-GB',
     'und-Hebr-SE': 'yi-Hebr-SE',
     'und-Hebr-UA': 'yi-Hebr-UA',
     'und-Hebr-US': 'yi-Hebr-US',
     'und-Hira': 'ja-Hira-JP',
     'und-Hluw': 'hlu-Hluw-TR',
     'und-Hmng': 'hnj-Hmng-LA',
-    'und-Hmnp': 'mww-Hmnp-US',
+    'und-Hmnp': 'hnj-Hmnp-US',
     'und-Hung': 'hu-Hung-HU',
     'und-IC': 'es-Latn-IC',
     'und-ID': 'id-Latn-ID',
     'und-IL': 'he-Hebr-IL',
     'und-IN': 'hi-Deva-IN',
     'und-IQ': 'ar-Arab-IQ',
     'und-IR': 'fa-Arab-IR',
@@ -3519,14 +3736,15 @@
     'und-OM': 'ar-Arab-OM',
     'und-Ogam': 'sga-Ogam-IE',
     'und-Olck': 'sat-Olck-IN',
     'und-Orkh': 'otk-Orkh-MN',
     'und-Orya': 'or-Orya-IN',
     'und-Osge': 'osa-Osge-US',
     'und-Osma': 'so-Osma-SO',
+    'und-Ougr': 'oui-Ougr-143',
     'und-PA': 'es-Latn-PA',
     'und-PE': 'es-Latn-PE',
     'und-PF': 'fr-Latn-PF',
     'und-PG': 'tpi-Latn-PG',
     'und-PH': 'fil-Latn-PH',
     'und-PK': 'ur-Arab-PK',
     'und-PL': 'pl-Latn-PL',
@@ -3612,24 +3830,27 @@
     'und-Thaa': 'dv-Thaa-MV',
     'und-Thai': 'th-Thai-TH',
     'und-Thai-CN': 'lcp-Thai-CN',
     'und-Thai-KH': 'kdt-Thai-KH',
     'und-Thai-LA': 'kdt-Thai-LA',
     'und-Tibt': 'bo-Tibt-CN',
     'und-Tirh': 'mai-Tirh-IN',
+    'und-Tnsa': 'nst-Tnsa-IN',
+    'und-Toto': 'txo-Toto-IN',
     'und-UA': 'uk-Cyrl-UA',
     'und-UG': 'sw-Latn-UG',
     'und-UY': 'es-Latn-UY',
     'und-UZ': 'uz-Latn-UZ',
     'und-Ugar': 'uga-Ugar-SY',
     'und-VA': 'it-Latn-VA',
     'und-VE': 'es-Latn-VE',
     'und-VN': 'vi-Latn-VN',
     'und-VU': 'bi-Latn-VU',
     'und-Vaii': 'vai-Vaii-LR',
+    'und-Vith': 'sq-Vith-AL',
     'und-WF': 'fr-Latn-WF',
     'und-WS': 'sm-Latn-WS',
     'und-Wara': 'hoc-Wara-IN',
     'und-Wcho': 'nnp-Wcho-IN',
     'und-XK': 'sq-Latn-XK',
     'und-Xpeo': 'peo-Xpeo-IR',
     'und-Xsux': 'akk-Xsux-IQ',
```

### Comparing `langcodes-3.2.1/langcodes/language_distance.py` & `langcodes-3.3.0/langcodes/language_distance.py`

 * *Files identical despite different names*

### Comparing `langcodes-3.2.1/langcodes/language_lists.py` & `langcodes-3.3.0/langcodes/language_lists.py`

 * *Files identical despite different names*

### Comparing `langcodes-3.2.1/langcodes/registry_parser.py` & `langcodes-3.3.0/langcodes/registry_parser.py`

 * *Files identical despite different names*

### Comparing `langcodes-3.2.1/langcodes/tag_parser.py` & `langcodes-3.3.0/langcodes/tag_parser.py`

 * *Files identical despite different names*

