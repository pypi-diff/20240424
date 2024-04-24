# Comparing `tmp/pypomes_core-0.8.7.tar.gz` & `tmp/pypomes_core-0.8.8.tar.gz`

## Comparing `pypomes_core-0.8.7.tar` & `pypomes_core-0.8.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27940 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23887 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/PKG-INFO
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.8/src/pypomes_core/.ruff.toml`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     "COM812",   # checks for the absence of trailing commas
     "COM819",   # prohibited trailing commas
     "D200",     # one-line docstring should fit on one line
     "D204",     # 1 blank line required after class docstring
     "D210",     # whitespaces surrounding docstring text
     "D212",     # multi-line docstring summary to start at the second line
     "DTZ005",   # the use of datetime.datetime.now() without tz argument is not allowed
+    "DTZ006",   # usage of 'datetime.datetime.fromtimestamp()' that do not specify a timezone
     "G004",     # logging statement uses 'f-string'
     "PGH004",   # use specific rule codes when using 'noqa'
     "PLR2004",  # magic value used in comparison, consider replacing it with a constant variable
     "PLW0603",  # using the global statement to update a variable is discouraged
     "PTH118",   # os.{module}.join() should be replaced by Path with / operator
     "RUF013",   # implicit Optional in type annotations when the default parameter value is None
     "S104",     # possible binding to all interfaces
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/__init__.py` & `pypomes_core-0.8.8/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.7/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/datetime_pomes.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 DATETIME_FORMAT_COMPACT: Final[str] = "%Y%m%d%H%M%S"
 DATETIME_FORMAT_INV: Final[str] = "%Y-%m-%d %H:%M:%S"
 
 TIMEZONE_LOCAL: pytz.BaseTzInfo = pytz.timezone(env_get_str(f"{APP_PREFIX}_TIMEZONE_LOCAL", "America/Sao_Paulo"))
 TIMEZONE_UTC: pytz.BaseTzInfo = pytz.UTC
 
 
-def date_reformat(dt_str: str, to_format: str, **kwargs: any) -> str:
+def date_reformat(dt_str: str,
+                  to_format: str,
+                  **kwargs: any) -> str:
     """
     Convert the date in *dt_str* to the format especified in *to_format*.
 
     The argument *dt_str* must represent a valid date, with or without time-of-day information.
     The argument *to_format* must be a valid format for *date* ou *datetime*.
 
     In *kwargs*, it may optionally be specified:
@@ -37,15 +39,16 @@
     ts: datetime = parser.parse(dt_str, **kwargs)
     if ts:
         result = datetime.strftime(ts, to_format)
 
     return result
 
 
-def date_parse(dt_str: str, **kwargs: any) -> date:
+def date_parse(dt_str: str,
+               **kwargs: any) -> date:
     """
     Obtain and return the *date* object corresponding to *dt_str*.
 
     In *kwargs*, it may optionally be specified:
         -   *dayfirst*, to signal that *day* comes before *month* in *dt_str*
         -   *fmt=<format>*, to force use of a specific format
     Return *None* se *dt_str* does not contain a valid date.
@@ -57,15 +60,16 @@
     result: date | None = None
     if dt_str:
         result = parser.parse(dt_str, **kwargs).date()
 
     return result
 
 
-def datetime_parse(dt_str: str, **kwargs: any) -> datetime:
+def datetime_parse(dt_str: str,
+                   **kwargs: any) -> datetime:
     """
     Obtain and return the *datetime* object corresponding to *dt_str*.
 
     In *kwargs*, it may optionally be specified:
         -   *dayfirst=True*, to signal that *day* comes before *month* in *dt_str*
         -   *fmt=<format>*, to force use of a specific format
    Return *None* se *dt_str* does not contain a valid date.
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/dict_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import types
 
 
-def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
+def dict_has_key_chain(source: dict,
+                       key_chain: list[str]) -> bool:
     """
     Indicate the existence of an element in *source*, pointed to by the nested key chain *[keys[0]: ... :keys[n]*.
 
     The path up to he last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
 
     :param source: the reference dict
@@ -47,15 +48,16 @@
         # success, if the parent element contains the last key in the chain
         else:
             result = key in parent
 
     return result
 
 
-def dict_get_value(source: dict, key_chain: list[str]) -> any:
+def dict_get_value(source: dict,
+                   key_chain: list[str]) -> any:
     """
     Obtain the value of the element in *source*, pointed to by the nested key chain *[keys[0]: ... :keys[n]*.
 
     The path up to the last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
     Return *None* if the sought after value is not found.
     Note that returning *None* might not be indicative of the absence of the element in *source*,
@@ -97,15 +99,17 @@
         else:
             # proceeding is not possible, the element corresponding to 'key' in the dictionary
             result = result.get(key)
 
     return result
 
 
-def dict_set_value(target: dict, key_chain: list[str], value: any) -> None:
+def dict_set_value(target: dict,
+                   key_chain: list[str],
+                   value: any) -> None:
     """
     Assign to an element of *source* the value *value*.
 
     The element in question is pointed to by the key chain *[keys[0]: ... :keys[n]*.
     If the element does not exist, it is created with the specified value.
     Any non-existing intermediate elements are created with the value of an empty *dict*.
     A key might indicate the position of the element within a list, using the format *<key>[<pos>]*.
@@ -159,15 +163,16 @@
                 # yes, do it
                 dict_item[inx] = value
         else:
             # no, assign 'value' to the element 'key' in the dictionary
             dict_item[key] = value
 
 
-def dict_pop_value(target: dict, key_chain: list[str]) -> any:
+def dict_pop_value(target: dict,
+                   key_chain: list[str]) -> any:
     """
     Obtain the value of the element in *source*, pointed to by the nested key chain *[keys[0]: ... :keys[n]*.
 
     The path up to the last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
     Return *None* if the sought after value is not found.
     Note that returning *None* might not be indicative of the absence of the element in *source*,
@@ -216,15 +221,17 @@
         elif key in parent:
             # yes, remove that element and return its value
             result = parent.pop(key)
 
     return result
 
 
-def dict_replace_value(target: dict, old_value: any, new_value: any) -> None:
+def dict_replace_value(target: dict,
+                       old_value: any,
+                       new_value: any) -> None:
     """
     Replace, in *target*, all occurrences of *old_value* with *new_value*.
 
     :param target: the reference dict
     :param old_value: the value to be replaced
     :param new_value: the new value
     """
@@ -257,15 +264,16 @@
 
         # is 'curr_value' a list ?
         elif isinstance(curr_value, list):
             # yes, process it recursively
             list_replace_value(curr_value, old_value, new_value)
 
 
-def dict_get_key(source: dict, value: any) -> any:
+def dict_get_key(source: dict,
+                 value: any) -> any:
     """
     Return the key in *source*, mapping the first occurrence of *value* found.
 
     Return *None*, if no key is found.
     No recursion is attempted; only the first-level attributes in *source* are inspected.
 
     :param source: dict to search
@@ -277,28 +285,30 @@
         if val == value:
             result = key
             break
 
     return result
 
 
-def dict_get_keys(source: dict, value: any) -> list[str]:
+def dict_get_keys(source: dict,
+                  value: any) -> list[str]:
     """
     Return all keys in *source*, mapping the value *value*.
 
     Return *[]* if no key is found.
 
     :param source: dict to search
     :param value: the reference value
     :return: list containing all keys mapping the reference value
     """
     return [key for key, val in source.items() if val == value]
 
 
-def dict_merge(target: dict, source: dict) -> None:
+def dict_merge(target: dict,
+               source: dict) -> None:
     """
     Traverse the elements in *source* to update *target*, according to the criteria presented herein.
 
     The criteria to be followed are:
       - add the element to *target*, if it does not exist
       - if the element exists in *target*:
 
@@ -332,15 +342,16 @@
                 # both elements are not lists or dictionarie, replace the value in target
                 target[skey] = svalue
         else:
             # the item is not in target, add it
             target[skey] = svalue
 
 
-def dict_coalesce(target: dict, key_chain: list[str]) -> None:
+def dict_coalesce(target: dict,
+                  key_chain: list[str]) -> None:
     """
     Coalesce the element of type *list* in *target* at the level *n* with the list at the level immediately above.
 
     This element is pointed to by the key chain *[keys[0]: ... :keys[n]*, and is processed as a sequence
     of multiple elements. The two last keys in *key_chain* must be associated with values of type *list*.
 
     :param target: the dictionary to be coalesced
@@ -424,15 +435,16 @@
                 # no, save it
                 penultimate_list.append(last_elem)
 
         # replace the original list with the coalesced new list
         curr_dict[key_chain[-2]] = penultimate_list
 
 
-def dict_reduce(target: dict, key_chain: list[str]) -> None:
+def dict_reduce(target: dict,
+                key_chain: list[str]) -> None:
     """
     Relocate the elements from *target* at level *n*, to the level immediately above.
 
     These elements are pointed to by the nested key chain *[keys[0]: ... :keys[n]*.
     The element at level *n* is removed at the end.
 
     :param target: the 'dict' to be reduced
@@ -473,15 +485,17 @@
            isinstance(curr_dict.get(last_key), dict):
             # sim, prossiga com a redução
             last: dict = curr_dict.pop(last_key)
             for key, value in last.items():
                 curr_dict[key] = value
 
 
-def dict_from_list(source: list[dict], key_chain: list[str], value: any) -> dict:
+def dict_from_list(source: list[dict],
+                   key_chain: list[str],
+                   value: any) -> dict:
     """
     Locate in *source*, and return, the element of type *dict* with value *value* in the key chain *key_chain*.
 
     :param source: the list to be inspected
     :param key_chain: the key chain used in the search process
     :param value: the value of the element pointed to by the key chain
     :return: the 'dict' wanted, or 'None' if not found
@@ -541,16 +555,18 @@
             else:
                 # no, proceed linearly
                 result[name] = value
 
     return result
 
 
-def dict_transform(source: dict, from_to_keys: list[tuple[str, str]],
-                   prefix_from: str = None, prefix_to: str = None) -> dict:
+def dict_transform(source: dict,
+                   from_to_keys: list[tuple[str, str]],
+                   prefix_from: str = None,
+                   prefix_to: str = None) -> dict:
     """
     Build a new *dict*, according to the rules presented herein.
 
     This dictionary is constructed by creating, for each element of the list of tuples in
     *from_to_keys*, the element indicated by the second term of the tuple, assigning to it
     the value of the *source* element indicated by the first term of the tuple. Both terms
     of the tuples are represented by a chain of nested keys.
@@ -604,15 +620,16 @@
 
             # atribui o valor transformado ao resultado
             dict_set_value(result, to_keys_deep, to_value)
 
     return result
 
 
-def dict_clone(source: dict, from_to_keys: list) -> dict:
+def dict_clone(source: dict,
+               from_to_keys: list) -> dict:
     """
     Build a new *dict*, according to the rules presented herein.
 
     This dictionary is constructed by creating a new element for each element in the list
     *from_to_keys*. When the element of this list is a tuple, the name indicated by its
     second term is used, and the value of the *source* element indicated by the tuple's
     first term is assigned. This first term can be represented by a chain of  nested keys.
@@ -635,15 +652,16 @@
         from_key: str = elem[0] if isinstance(elem, tuple) else elem
         to_key: str = (elem[1] if isinstance(elem, tuple) and len(elem) > 1 else None) or from_key
         result[to_key] = dict_get_value(source, list_unflatten(from_key))
 
     return result
 
 
-def dict_listify(target: dict, key_chain: list[str]) -> None:
+def dict_listify(target: dict,
+                 key_chain: list[str]) -> None:
     """
     Insert the value of the item pointed to by the key chain *[keys[0]: ... :keys[n]* in a list.
 
     This insertion will happen only if such a value is not itself a list.
     All lists eventually found, up to the penultimate key in the chain, will be processed recursively.
 
     :param target: the dictionary to be modified
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/email_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 
 EMAIL_ACCOUNT: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_ACCOUNT")
 EMAIL_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_PWD")
 EMAIL_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_EMAIL_PORT")
 EMAIL_SERVER: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_SERVER")
 
 
-def email_send(errors: list[str] | None, user_email: str,
-               subject: str, content: str, logger: Logger = None) -> None:
+def email_send(errors: list[str] | None,
+               user_email: str,
+               subject: str,
+               content: str,
+               logger: Logger = None) -> None:
     """
     Send email to *user_email", with *subject* as the email subject, and *content* as the email message.
 
     :param errors: incidental error messages
     :param user_email: the address to send the email to
     :param subject: the email subject
     :param content: the email message
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.7/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/env_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from pathlib import Path
 from typing import Final
 
 # the prefix for the names of the environment variables
 APP_PREFIX: Final[str] = os.environ["PYPOMES_APP_PREFIX"]
 
 
-def env_get_str(key: str, def_value: str = None) -> str:
+def env_get_str(key: str,
+                def_value: str = None) -> str:
     """
     Retrieve and return the string value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The str value associated with the key
     """
@@ -19,15 +20,16 @@
         result = os.environ[key]
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
-def env_get_bool(key: str, def_value: bool = None) -> bool:
+def env_get_bool(key: str,
+                 def_value: bool = None) -> bool:
     """
     Retrieve and return the boolean value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The bool value associated with the key
     """
@@ -36,15 +38,16 @@
         result = bool(int(os.environ[key]))
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
-def env_get_int(key: str, def_value: int = None) -> int:
+def env_get_int(key: str,
+                def_value: int = None) -> int:
     """
     Retrieve and return the int value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The int value associated with the key
     """
@@ -53,15 +56,16 @@
         result = int(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
-def env_get_float(key: str, def_value: float = None) -> float:
+def env_get_float(key: str,
+                  def_value: float = None) -> float:
     """
     Retrieve and return the float value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The float value associated with the key
     """
@@ -70,15 +74,16 @@
         result = int(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
-def env_get_path(key: str, def_value: Path = None) -> Path:
+def env_get_path(key: str,
+                 def_value: Path = None) -> Path:
     """
     Retrieve and return the path value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The path value associated with the key
     """
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/exception_pomes.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from types import TracebackType
 import os
 import traceback
+from types import TracebackType
 
 
 def exc_format(exc: Exception,
                exc_info: tuple[type[BaseException], BaseException, TracebackType]) -> str:
     """
     Format the error message resulting from the exception raised in execution time.
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/file_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from werkzeug.datastructures import FileStorage
 
 from .env_pomes import APP_PREFIX, env_get_path
 
 TEMP_DIR: Final[Path] = env_get_path(f"{APP_PREFIX}_TEMP_DIR", Path(gettempdir()))
 
 
-def file_from_request(request: Request, file_name: str = None, file_seq: int = 0) -> bytes:
+def file_from_request(request: Request,
+                      file_name: str = None,
+                      file_seq: int = 0) -> bytes:
     """
     Retrieve and return the contents of the file returned in the response to a request.
 
     The file may be referred to by its name (*file_name*), or if no name is specified,
     by its sequence number (*file_seq*).
 
     :param request: the request
     :param file_name: optional name for the file
-    :param file_seq:  sequence number for the file, defaults to the first file
+    :param file_seq: sequence number for the file, defaults to the first file
     :return: the contents retrieved from the file
     """
     # inicialize the return variable
     result: bytes | None = None
 
     count: int = len(request.files)
     # has a file been found ?
@@ -39,28 +41,28 @@
             result: bytes = file.stream.read()
 
     return result
 
 
 def file_get_data(file_data: Path | str | bytes) -> bytes:
     """
-    Retrieve and return the data in *file_data* (typeipo *bytes*), or in a file in path *file_data* (type *str*).
+    Retrieve and return the data in *file_data* (type *bytes*), or in a file in path *file_data* (type *Path* or *str*).
 
     :param file_data: file data, or the path to locate the file
-    :return: the data
+    :return: the data, or None if the file data could not be obtained
     """
-    # declare the return variable
-    result: bytes
+    # initialize the return variable
+    result: bytes | None = None
 
     # what is the argument type ?
     if isinstance(file_data, bytes):
         # argument is type 'bytes'
         result = file_data
 
-    else:  # isinstance(file_data, Path) or isinstance(file_data, str)
+    elif isinstance(file_data, Path | str):
         # argument is a file path
         buf_size: int = 128 * 1024
         file_path: Path = file_data if isinstance(file_data, Path) else Path(file_data)
         with file_path.open("rb") as f:
             file_bytes: bytearray = bytearray()
             while True:
                 in_bytes: bytes = f.read(buf_size)
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.7/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/list_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-def list_compare(list1: list[any], list2: list[any]) -> bool:
+def list_compare(list1: list[any],
+                 list2: list[any]) -> bool:
     """
     Compare the contents of the two lists *list1* e *list2*.
 
     Return *True* if all the elements in *list1* are also in *list2*, and vice-versa, with the same cardinality.
 
     :param list1: the first list
     :param list2: the second list
@@ -61,15 +62,16 @@
     """
     # import the needed function
     from .str_pomes import str_split_on_mark
 
     return str_split_on_mark(source, ".")
 
 
-def list_find_coupled(coupled_elements: list[tuple[str, str]], primary_element: str) -> str:
+def list_find_coupled(coupled_elements: list[tuple[str, str]],
+                      primary_element: str) -> str:
     """
     Locate in *coupled_elements*, and return, the element coupled to *primary_element*.
 
     If *primary_element* contains an index indication (denoted by *[<pos>]*), this indication is removed.
     This function is used in the transformation of *dicts* (*dict_transform*) and *lists* (*list_transform*),
     from sequences of key pairs.
 
@@ -94,16 +96,18 @@
             # yes, return the corresponding coupled element
             result = coupled
             break
 
     return result
 
 
-def list_transform(source: list[any], from_to_keys: list[tuple[str, str]],
-                   prefix_from: str = None, prefix_to: str = None) -> list[any]:
+def list_transform(source: list[any],
+                   from_to_keys: list[tuple[str, str]],
+                   prefix_from: str = None,
+                   prefix_to: str = None) -> list[any]:
     """
     Construct a new *list*, transforming elements of type *list* and *dict* found in *source*.
 
     The conversion of *dict* type elements is documented in the *dict_transform* function.
 
     The prefixes for the source and destination keys, if defined, have different treatments.
     They are added when searching for values in *Source*, and removed when assigning values
@@ -139,15 +143,16 @@
         # added the value transformed to 'result'
         result.append(to_value)
 
     return result
 
 
 def list_elem_starting_with(source: list[str | bytes],
-                            prefix: str | bytes, keep_prefix: bool = True) -> str | bytes:
+                            prefix: str | bytes,
+                            keep_prefix: bool = True) -> str | bytes:
     """
     Locate and return the first element in *source* prefixed by *prefix*.
 
     Retorna *None* se esse elemento não for encontrado.
 
     :param source: the list to be inspected
     :param prefix: the data prefixing the element to be returned
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/str_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     cleaned: str = target_str.replace("\\", "") \
                              .replace('"', "'") \
                              .replace("\n", " ") \
                              .replace("\t", " ")
     return " ".join(cleaned.split())
 
 
-def str_split_on_mark(source: str, mark: str) -> list[str]:
+def str_split_on_mark(source: str,
+                      mark: str) -> list[str]:
     """
     Extract from *source* the text segments separated by *mark*, and return them in a *list*.
 
     The separator itself will not be in the returned list.
 
     :param source: the string to be inspected
     :param mark: the separator
@@ -61,15 +62,17 @@
         if char.isspace():
             result = inx
             break
 
     return result
 
 
-def str_get_between(source: str, from_str: str, to_str: str) -> str:
+def str_get_between(source: str,
+                    from_str: str,
+                    to_str: str) -> str:
     """
     Extract and return the *substring* in *source* located between the delimiters *from_str* and *to_str*.
 
     :param source: the string to be inspected
     :param from_str: the initial delimiter
     :param to_str: the final delimiter
     :return: the extracted substring, or None if no substring was obtained
@@ -83,15 +86,17 @@
         pos2: int = source.find(to_str, pos1)
         if pos2 >= pos1:
             result = source[pos1:pos2]
 
     return result
 
 
-def str_get_positional(source: str, list_origin: list[str], list_dest: list[str]) -> str:
+def str_get_positional(source: str,
+                       list_origin: list[str],
+                       list_dest: list[str]) -> str:
     """
     Locate the position of *source* within *list_origin*, and return the element in the same position in *list_dest*.
 
     :param source: the source string
     :param list_origin: the list to be inspected
     :param list_dest: the list containing the positionally corresponding values
     :return: the value positionally corresponding to the source string, or None if not found
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.8/src/pypomes_core/validation_msgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,16 @@
     _ERR_MSGS_EN[key] = value["en"]
 
 _ERR_MSGS_PT: dict = {}
 for key, value in __ERR_MSGS.items():
     _ERR_MSGS_PT[key] = value["pt"]
 
 
-def validate_add_msgs(msgs: dict, lang: Literal["en", "pt"] = "en") -> None:
+def validate_add_msgs(msgs: dict,
+                      lang: Literal["en", "pt"] = "en") -> None:
     """
     Add the messages in *msgs* to the standard validation messages list for language *lang".
 
     If applicable, this operation should be performed at the start of the application importing this module,
     before any attempt to read from *_ERR_MSGS_EN* or *_ERR_MSGS_PT*.
 
     :param msgs: list of messages to be added
@@ -113,15 +114,16 @@
     match lang:
         case "en":
             _ERR_MSGS_EN.update(msgs)
         case "pt":
             _ERR_MSGS_PT.update(msgs)
 
 
-def validate_set_msgs(msgs: dict, lang: Literal["en", "pt"] = "en") -> None:
+def validate_set_msgs(msgs: dict,
+                      lang: Literal["en", "pt"] = "en") -> None:
     """
     Set  the standard validation messages list for language *lang* to the messages in *msgs*.
 
     If applicable, this operation should be performed at the start of the application importing this module,
     before any attempt to read from *_ERR_MSGS_EN* or *_ERR_MSGS_PT*.
 
     :param msgs: list of messages to set the standard validation messages to
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/validation_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 from .env_pomes import APP_PREFIX, env_get_str
 from .str_pomes import str_sanitize, str_find_whitespace
 
 VALIDATE_MSG_LANGUAGE: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_LANGUAGE", "pt")
 VALIDATE_MSG_PREFIX: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_PREFIX", APP_PREFIX)
 
 
-def validate_value(attr: str, val: str | int | float, min_val: int = None,
-                   max_val: int = None, default: bool | list[any] = None) -> str:
+def validate_value(attr: str,
+                   val: str | int | float,
+                   min_val: int = None,
+                   max_val: int = None,
+                   default: bool | list[any] = None) -> str:
     """
     Validate *val* according to value, range, or membership in values list, as specified.
 
     :param attr: the name of the attribute
     :param val: the value to be validated
     :param min_val: if val is a string, specifies its minimum length; otherwise, specifies its minimum value
     :param max_val: if val is a string, specifies its maximum length; otherwise, specifies its maximum value
@@ -37,15 +40,15 @@
                     result = validate_format_error(125, val, default[0], f"@{attr}")
                 else:
                     # is 'None' the last element in list ?
                     if default[-1] is None:
                         # yes, omit it from the message
                         length -= 1
                     # 126: Invalid value {}: must be one of {}
-                    result = validate_format_error(126, val, [default[:length]], f"@{attr}")
+                    result = validate_format_error(126, val, default[:length], f"@{attr}")
     elif val is None:
         if isinstance(default, bool) and default:
             # 112: Required attribute
             result = validate_format_error(112, f"@{attr}")
     elif isinstance(val, str):
         length: int = len(val)
         if min_val is not None and max_val == min_val and length != min_val:
@@ -61,16 +64,20 @@
          (max_val is not None and val > max_val):
         # 127: Invalid value {}: must be in the range {}
         result = validate_format_error(127, val, [min_val, max_val], f"@{attr}")
 
     return result
 
 
-def validate_bool(errors: list[str] | None, scheme: dict, attr: str,
-                  default: bool = None, mandatory: bool = False, logger: Logger = None) -> bool:
+def validate_bool(errors: list[str] | None,
+                  scheme: dict,
+                  attr: str,
+                  default: bool = None,
+                  mandatory: bool = False,
+                  logger: Logger = None) -> bool:
     """
     Validate the boolean value associated with *attr* in *scheme*.
 
     If provided, this value must be a *bool*, or the string *t*, *true*, *f*, or *false*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
@@ -105,17 +112,21 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_int(errors: list[str] | None, scheme: dict, attr: str,
-                 min_val: int = None, max_val: int = None,
-                 default: bool | int | list[int] = None, logger: Logger = None) -> int:
+def validate_int(errors: list[str] | None,
+                 scheme: dict,
+                 attr: str,
+                 min_val: int = None,
+                 max_val: int = None,
+                 default: bool | int | list[int] = None,
+                 logger: Logger = None) -> int:
     """
     Validate the *int* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *int*, or a valid string representation of a *int*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
@@ -156,17 +167,21 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_float(errors: list[str] | None, scheme: dict, attr: str,
-                   min_val: float = None, max_val: float = None,
-                   default: bool | int | float | list[float | int] = None, logger: Logger = None) -> float:
+def validate_float(errors: list[str] | None,
+                   scheme: dict,
+                   attr: str,
+                   min_val: float = None,
+                   max_val: float = None,
+                   default: bool | int | float | list[float | int] = None,
+                   logger: Logger = None) -> float:
     """
     Validate the *float* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *float*, or a valid string representation of a *float*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
@@ -209,17 +224,21 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_str(errors: list[str] | None, scheme: dict, attr: str,
-                 min_length: int = None, max_length: int = None,
-                 default: bool | str | list[str] = None, logger: Logger = None) -> str:
+def validate_str(errors: list[str] | None,
+                 scheme: dict,
+                 attr: str,
+                 min_length: int = None,
+                 max_length: int = None,
+                 default: bool | str | list[str] = None,
+                 logger: Logger = None) -> str:
     """
     Validate the *str* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *str*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
@@ -252,16 +271,20 @@
     if stat:
         result = None
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_date(errors: list[str] | None, scheme: dict, attr: str,
-                  day_first: bool = False, default: bool | date = None, logger: Logger = None) -> date:
+def validate_date(errors: list[str] | None,
+                  scheme: dict,
+                  attr: str,
+                  day_first: bool = False,
+                  default: bool | date = None,
+                  logger: Logger = None) -> date:
     """
     Validate the *date* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *date*, or a valid string representation of a *date*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
@@ -301,16 +324,20 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_datetime(errors: list[str] | None, scheme: dict, attr: str,
-                      day_first: bool = True, default: bool | datetime = None, logger: Logger = None) -> datetime:
+def validate_datetime(errors: list[str] | None,
+                      scheme: dict,
+                      attr: str,
+                      day_first: bool = True,
+                      default: bool | datetime = None,
+                      logger: Logger = None) -> datetime:
     """
     Validate the *datetime* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *date*, or a valid string representation of a *date*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
@@ -350,17 +377,21 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_ints(errors: list[str] | None, scheme: dict, attr: str,
-                  min_val: int = None, max_val: int = None,
-                  mandatory: bool = False, logger: Logger = None) -> list[int]:
+def validate_ints(errors: list[str] | None,
+                  scheme: dict,
+                  attr: str,
+                  min_val: int = None,
+                  max_val: int = None,
+                  mandatory: bool = False,
+                  logger: Logger = None) -> list[int]:
     """
     Validate the list of *int* values associated with *attr* in *scheme*.
 
     If provided, this list must contain *ints*, or valid string representations of *ints*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the list of values to be validated
@@ -402,17 +433,21 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_strs(errors: list[str] | None, scheme: dict,
-                  attr: str, min_length: int, max_length: int,
-                  mandatory: bool = False, logger: Logger = None) -> list[str]:
+def validate_strs(errors: list[str] | None,
+                  scheme: dict,
+                  attr: str,
+                  min_length: int,
+                  max_length: int,
+                  mandatory: bool = False,
+                  logger: Logger = None) -> list[str]:
     """
     Validate the list of *str* values associated with *attr* in *scheme*.
 
     If provided, this list must contain *strs*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the list of values to be validated
@@ -454,15 +489,16 @@
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
-def validate_format_error(error_id: int, *args) -> str:
+def validate_format_error(error_id: int,
+                          *args: any) -> str:
     """
     Format and return the error message identified by *err_id* in the standard messages list.
 
     The message is built from the message element in the standard messages list, identified by *err_id*.
     The occurrences of '{}' in the element are sequentially replaced by the given *args*.
 
     :param error_id: the identification of the message element
@@ -567,15 +603,17 @@
             result.append(f"{error.get(name)}: {str_sanitize(error.get(desc))}")
         else:
             result.append(error)
 
     return result
 
 
-def __validate_log(errors: list[str], err_msg: str, logger: Logger) -> None:
+def __validate_log(errors: list[str],
+                   err_msg: str,
+                   logger: Logger) -> None:
     """
     LOg *err_msg* using *logger*, and add it to the error messages list *errors*.
 
     :param errors: the error messages list
     :param err_msg: the message to log
     :param logger: the logger
     """
```

### Comparing `pypomes_core-0.8.7/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.8/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.7/LICENSE` & `pypomes_core-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.7/pyproject.toml` & `pypomes_core-0.8.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.7/PKG-INFO` & `pypomes_core-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.7
+Version: 0.8.8
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

