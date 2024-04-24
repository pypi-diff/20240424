# Comparing `tmp/dicebear-2.7.3.tar.gz` & `tmp/dicebear-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicebear-2.7.3.tar", last modified: Sat Mar  9 18:15:11 2024, max compression
+gzip compressed data, was "dicebear-2.7.4.tar", last modified: Wed Apr 24 17:27:16 2024, max compression
```

## Comparing `dicebear-2.7.3.tar` & `dicebear-2.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 18:15:11.831679 dicebear-2.7.3/
--rw-rw-rw-   0        0        0     1095 2024-03-09 17:35:16.000000 dicebear-2.7.3/LICENSE
--rw-rw-rw-   0        0        0    11077 2024-03-09 18:15:11.830678 dicebear-2.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     9011 2024-03-09 18:00:23.000000 dicebear-2.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 18:15:11.795502 dicebear-2.7.3/dicebear/
--rw-rw-rw-   0        0        0     1255 2024-03-09 18:09:46.000000 dicebear-2.7.3/dicebear/__init__.py
--rw-rw-rw-   0        0        0    17174 2024-03-09 18:09:41.000000 dicebear-2.7.3/dicebear/avatar.py
--rw-rw-rw-   0        0        0     3987 2024-03-09 18:09:52.000000 dicebear-2.7.3/dicebear/errors.py
--rw-rw-rw-   0        0        0    19860 2024-03-09 18:10:04.000000 dicebear-2.7.3/dicebear/models.py
--rw-rw-rw-   0        0        0     4455 2024-03-09 18:10:04.000000 dicebear-2.7.3/dicebear/utility.py
-drwxrwxrwx   0        0        0        0 2024-03-09 18:15:11.817022 dicebear-2.7.3/dicebear.egg-info/
--rw-rw-rw-   0        0        0    11077 2024-03-09 18:15:11.000000 dicebear-2.7.3/dicebear.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-03-09 18:15:11.000000 dicebear-2.7.3/dicebear.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 18:15:11.000000 dicebear-2.7.3/dicebear.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-09 18:15:11.000000 dicebear-2.7.3/dicebear.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-09 18:15:11.000000 dicebear-2.7.3/dicebear.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-02-22 11:00:24.000000 dicebear-2.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-09 18:15:11.831679 dicebear-2.7.3/setup.cfg
--rw-rw-rw-   0        0        0     3760 2024-03-09 18:12:49.000000 dicebear-2.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-09 18:15:11.829685 dicebear-2.7.3/tests/
--rw-rw-rw-   0        0        0       23 2023-03-13 12:13:43.000000 dicebear-2.7.3/tests/__init__.py
--rw-rw-rw-   0        0        0     5534 2023-12-12 13:42:18.000000 dicebear-2.7.3/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:27:16.656930 dicebear-2.7.4/
+-rw-rw-rw-   0        0        0     1095 2024-03-09 17:35:16.000000 dicebear-2.7.4/LICENSE
+-rw-rw-rw-   0        0        0    11048 2024-04-24 17:27:16.656930 dicebear-2.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8990 2024-04-24 17:18:09.000000 dicebear-2.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 17:27:16.619394 dicebear-2.7.4/dicebear/
+-rw-rw-rw-   0        0        0     1255 2024-04-24 14:31:28.000000 dicebear-2.7.4/dicebear/__init__.py
+-rw-rw-rw-   0        0        0    16613 2024-04-24 15:58:11.000000 dicebear-2.7.4/dicebear/avatar.py
+-rw-rw-rw-   0        0        0     3975 2024-04-24 15:21:58.000000 dicebear-2.7.4/dicebear/errors.py
+-rw-rw-rw-   0        0        0    19857 2024-04-24 16:13:48.000000 dicebear-2.7.4/dicebear/models.py
+-rw-rw-rw-   0        0        0     4492 2024-04-24 15:49:02.000000 dicebear-2.7.4/dicebear/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:27:16.649929 dicebear-2.7.4/dicebear.egg-info/
+-rw-rw-rw-   0        0        0    11048 2024-04-24 17:27:16.000000 dicebear-2.7.4/dicebear.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-24 17:27:16.000000 dicebear-2.7.4/dicebear.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 17:27:16.000000 dicebear-2.7.4/dicebear.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-24 17:27:16.000000 dicebear-2.7.4/dicebear.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 17:27:16.000000 dicebear-2.7.4/dicebear.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-04-24 17:03:15.000000 dicebear-2.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 17:27:16.657929 dicebear-2.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     3752 2024-04-24 15:46:16.000000 dicebear-2.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:27:16.655929 dicebear-2.7.4/tests/
+-rw-rw-rw-   0        0        0       23 2023-03-13 12:13:43.000000 dicebear-2.7.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     5749 2024-04-24 16:26:11.000000 dicebear-2.7.4/tests/test_main.py
```

### Comparing `dicebear-2.7.3/LICENSE` & `dicebear-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dicebear-2.7.3/PKG-INFO` & `dicebear-2.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dicebear
-Version: 2.7.3
+Version: 2.7.4
 Summary: A python wrapper for DiceBear's avatar generating API.
 Home-page: https://jvh.gitbook.io/dicebear
 Author: jvherck
-Author-email: contact@janvh.be
+Author-email: jan@vhjan.me
 Maintainer: jvherck
-Maintainer-email: contact@janvh.be
+Maintainer-email: jan@vhjan.me
 License: MIT License
 Project-URL: Documentation, https://jvh.gitbook.io/dicebear
 Project-URL: Source, https://github.com/jvherck/dicebear
 Project-URL: Tracker, https://github.com/jvherck/dicebear/issues
 Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,notionists,notionists-neutral,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -43,36 +43,36 @@
 ![PyPI](https://img.shields.io/pypi/v/dicebear)
 ![GitHub issues](https://img.shields.io/github/issues/jvherck/dicebear)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicebear)
 ![GitHub](https://img.shields.io/github/license/jvherck/dicebear)
 ![Maintenance](https://img.shields.io/maintenance/yes/2024)
 ![PyPI - Status](https://img.shields.io/pypi/status/dicebear)
 
-Always keep an eye on https://jvh.gitbook.io/dicebear/ for updates and warnings about this packages!
+Always keep an eye on https://dicebear.vhjan.me/ for updates and warnings about this packages!
 
-[`dicebear`](https://pypi.org/project/dicebear/) is an API wrapper for https://dicebear.com. Using this wrapper you can get custom avatars for your program. \
+[`dicebear`](https://pypi.org/project/dicebear/) is a Python API wrapper for https://dicebear.com. Using this wrapper you can get custom avatars for your program. \
 For an example go to [`examples/dicebear.py`](https://github.com/jvherck/dicebear/tree/main/examples).
 
 
 ---
 
 
 ## Useful links  
-* Docs: https://jvh.gitbook.io/dicebear/  
+* Official Dicebear: https://dicebear.com/
+* Docs: https://dicebear.vhjan.me/  
 * PyPI: https://pypi.org/project/dicebear/  
 * GitHub: https://github.com/jvherck/dicebear  
-* Dicebear: https://dicebear.com/  
-- Dicebear CLI: https://github.com/jvherck/dicebear-cli  
+* Dicebear Python CLI: https://github.com/jvherck/dicebear-cli  
 
 
 ---
 
 
 ## Changelog
-Find the changelog here: https://github.com/jvherck/dicebear/blob/main/CHANGELOG.md
+Find the changelog here: https://dicebear.vhjan.me/changelog
 
 
 ---
 
 
 ## How to install  
 Run `pip install -U dicebear` \
@@ -273,14 +273,14 @@
 
 
 ---
 
 
 ## Credits  
 Special thanks to [DiceBear](https://github.com/dicebear) ([Florian Körner](https://github.com/FlorianKoerner)) for 
-making this amazing API and to [all artists](https://dicebear.com/licenses) that helped making avatars!  
+making this amazing API and to [all artists](https://dicebear.com/licenses) for creating these avatars!  
 
 
 ## Licenses and privacy policy  
 - Dicebear **Licenses**: https://dicebear.com/licenses  
 - Dicebear **Privacy Policy**: https://dicebear.com/legal/privacy-policy  
-- Dicebear Python API wrapper (this project): https://jvh.gitbook.io/dicebear/license
+- Dicebear Python API wrapper (this project): https://dicebear.vhjan.me/license
```

### Comparing `dicebear-2.7.3/README.md` & `dicebear-2.7.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 ![PyPI](https://img.shields.io/pypi/v/dicebear)
 ![GitHub issues](https://img.shields.io/github/issues/jvherck/dicebear)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicebear)
 ![GitHub](https://img.shields.io/github/license/jvherck/dicebear)
 ![Maintenance](https://img.shields.io/maintenance/yes/2024)
 ![PyPI - Status](https://img.shields.io/pypi/status/dicebear)
 
-Always keep an eye on https://jvh.gitbook.io/dicebear/ for updates and warnings about this packages!
+Always keep an eye on https://dicebear.vhjan.me/ for updates and warnings about this packages!
 
-[`dicebear`](https://pypi.org/project/dicebear/) is an API wrapper for https://dicebear.com. Using this wrapper you can get custom avatars for your program. \
+[`dicebear`](https://pypi.org/project/dicebear/) is a Python API wrapper for https://dicebear.com. Using this wrapper you can get custom avatars for your program. \
 For an example go to [`examples/dicebear.py`](https://github.com/jvherck/dicebear/tree/main/examples).
 
 
 ---
 
 
 ## Useful links  
-* Docs: https://jvh.gitbook.io/dicebear/  
+* Official Dicebear: https://dicebear.com/
+* Docs: https://dicebear.vhjan.me/  
 * PyPI: https://pypi.org/project/dicebear/  
 * GitHub: https://github.com/jvherck/dicebear  
-* Dicebear: https://dicebear.com/  
-- Dicebear CLI: https://github.com/jvherck/dicebear-cli  
+* Dicebear Python CLI: https://github.com/jvherck/dicebear-cli  
 
 
 ---
 
 
 ## Changelog
-Find the changelog here: https://github.com/jvherck/dicebear/blob/main/CHANGELOG.md
+Find the changelog here: https://dicebear.vhjan.me/changelog
 
 
 ---
 
 
 ## How to install  
 Run `pip install -U dicebear` \
@@ -234,14 +234,14 @@
 
 
 ---
 
 
 ## Credits  
 Special thanks to [DiceBear](https://github.com/dicebear) ([Florian Körner](https://github.com/FlorianKoerner)) for 
-making this amazing API and to [all artists](https://dicebear.com/licenses) that helped making avatars!  
+making this amazing API and to [all artists](https://dicebear.com/licenses) for creating these avatars!  
 
 
 ## Licenses and privacy policy  
 - Dicebear **Licenses**: https://dicebear.com/licenses  
 - Dicebear **Privacy Policy**: https://dicebear.com/legal/privacy-policy  
-- Dicebear Python API wrapper (this project): https://jvh.gitbook.io/dicebear/license
+- Dicebear Python API wrapper (this project): https://dicebear.vhjan.me/license
```

### Comparing `dicebear-2.7.3/dicebear/__init__.py` & `dicebear-2.7.4/dicebear/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 # SOFTWARE.
 
 from .avatar import *
 from .errors import *
 from .models import *
 from .utility import *
 
-__version__ = "2.7.3"
+__version__ = "2.7.4"
```

### Comparing `dicebear-2.7.3/dicebear/avatar.py` & `dicebear-2.7.4/dicebear/avatar.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,60 +16,55 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import requests as r
+import io
 import os
 import pathlib
-import io
 import re as regex
-
-from urllib.parse import quote
-from string import ascii_lowercase, digits
 from ast import literal_eval
-from typing import Union
 from random import choices
+from string import ascii_lowercase, digits
+from typing import Union
+from urllib.parse import quote
+
+import requests as r
 
-from .models import *
 from .errors import *
-from .models import _FindPil, _pilcheck, _statsIncrease
+from .models import *
+from .models import _FindPil, _pilcheck, _statsIncrease, _x
 
 __all__ = ('DAvatar',)
 __filename__ = "avatar.py"
 
 try:
-    from PIL import Image as i
+    from PIL import Image as Im
 except Exception:
-    class i:
+    class Im:
         class Image:
             def show(self): pass
 
-
     _FindPil.found = False
 
-_x = "https://api.dicebear.com/7.x/{}/svg?seed={}&"
+
+_y = _x + "/{}/svg?seed={}&"
 
 
 class DAvatar:
     """
     Base class for the avatar generator.
     """
     default_options: dict = default_options
     all_options: list = options
 
-    def __init__(self,
-                 style: Union[str, DStyle] = None,
-                 seed: str = None,
-                 *,
-                 options: DOptions = None,
-                 custom: dict = None
-                 ) -> None:
+    def __init__(self, style: Union[str, DStyle] = None, seed: str = None, *, options: DOptions = None,
+                 custom: dict = None) -> None:
         """
         Create a new avatar object.
 
         :param style: class `dicebear.models.DStyle` :: the style of avatar you want to create; check the whole list at https://github.com/jvherck/dicebear#styles
         :type style: dicebear.models.DStyle
         :param seed: class `str` :: the seed for the avatar; the avatar will be edited according to the seed
         :type seed: str
@@ -86,15 +81,14 @@
         if options is None: options = DOptions.empty
         if custom is None: custom = {}
         self.__style: DStyle = style
         self.__seed: str = seed
         self.__options: DOptions = options
         self.__specific: dict = custom
         self.__url_svg: str
-        self.__schema: dict = r.get(f"https://api.dicebear.com/7.x/{style}/schema.json").json()
         self.__update()
         _statsIncrease(__filename__, self.__class__.__name__, ".__init__()")
 
     @property
     def style(self) -> DStyle:
         """
         :return: the style of the avatar
@@ -114,17 +108,17 @@
     def options(self) -> DOptions:
         """
         :return: the options of the avatar
         """
         _statsIncrease(__filename__, self.__class__.__name__, ".options")
         _option_list = {}
         for key in self.__options:
-            if self.__options[key] != DAvatar.default_options[key]:
+            if self.__options[key] != default_options[key]:
                 _option_list.update({key: self.__options[key]})
-        return DOptions(fromdict=_option_list)
+        return DOptions.from_dict(_option_list)
 
     @property
     def customisations(self) -> dict:
         """
         :return: the customisations of the avatar
         """
         _statsIncrease(__filename__, self.__class__.__name__, ".customisations")
@@ -165,15 +159,15 @@
         return self.__url_svg.replace("/svg?", "/json?")
 
     @property
     def schema(self) -> dict:
         """
         :return: dict object containing the schema of the avatar style
         """
-        return self.__schema
+        return r.get(_x + f"/{self.style}/schema.json").json()
 
     def text(self, format: DFormat = DFormat.svg) -> str:
         """
         :param format: class `dicebear.models.DFormat` :: which format to use
         :return: returns the avatar's request's full text/file in str format
         """
         _statsIncrease(__filename__, self.__class__.__name__, ".text()")
@@ -194,46 +188,46 @@
     def __repr__(self):
         return f"DAvatar(style=DStyle.{self.style}, seed=\"{self.seed}\", *, options={self.options}, custom={self.customizations})"
 
     def __str__(self):
         return self.__url_svg
 
     def __eq__(self, other):
-        if type(other) == DAvatar: return self.__url_svg == other.__url_svg
+        if type(other) is DAvatar: return self.__url_svg == other.__url_svg
         return self.__url_svg == other
 
     def __ne__(self, other):
-        if type(other) == DAvatar: return self.__url_svg != other.__url_svg
+        if type(other) is DAvatar: return self.__url_svg != other.__url_svg
         return self.__url_svg != other
 
     def __le__(self, other):
-        if type(other) == DAvatar:
+        if type(other) is DAvatar:
             return self.options["size"] <= other.options["size"]
-        elif type(other) == dict:
+        elif type(other) is dict:
             return self.options["size"] <= other["size"]
         return self.options["size"] <= other
 
     def __lt__(self, other):
-        if type(other) == DAvatar:
+        if type(other) is DAvatar:
             return self.options["size"] < other.options["size"]
-        elif type(other) == dict:
+        elif type(other) is dict:
             return self.options["size"] < other["size"]
         return self.options["size"] < other
 
     def __ge__(self, other):
-        if type(other) == DAvatar:
+        if type(other) is DAvatar:
             return self.options["size"] >= other.options["size"]
-        elif type(other) == dict:
+        elif type(other) is dict:
             return self.options["size"] >= other["size"]
         return self.options["size"] >= other
 
     def __gt__(self, other):
-        if type(other) == DAvatar:
+        if type(other) is DAvatar:
             return self.options["size"] > other.options["size"]
-        elif type(other) == dict:
+        elif type(other) is dict:
             return self.options["size"] > other["size"]
         return self.options["size"] > other
 
     def __dict__(self):
         return {"style": self.style, "seed": self.seed, "options": self.options, "custom": self.customisations}
 
     def __contains__(self, key: str):
@@ -243,57 +237,53 @@
         return key in self.options.keys() or key in self.customisations.keys()
 
     @staticmethod
     def __checkLinkError(text: str) -> None:
         """
         :param text: requests.Response.text
         """
-        status = ""
         try:
             status = literal_eval(text)
         except (ValueError, SyntaxError):
-            pass
-        if type(status) == dict and "statusCode" in status: raise HTTPError(status)
+            status = ""
+        if type(status) is dict and "statusCode" in status: raise HTTPError(status)
 
     def __update(self) -> None:
-        _link = _x
+        _link = _y
         _options, _specoptions, status = [], [], ""
         for item in self.__options:
-            if item in all_options:
-                _options.append(
-                    "{}={}".format(
-                        quote(item),
-                        str(self.__options[item]).replace("False", "false").replace("True", "true")))
-        for item in self.__specific:
-            _specoptions.append(
-                "{}={}".format(
+            if item in all_options and self.__options[item] != default_options[item]:
+                _options.append("{}={}".format(
                     quote(item),
-                    str(self.__specific[item]).replace("False", "false").replace("True", "true")))
+                    str(self.__options[item])
+                    .replace("False", "false")
+                    .replace("True", "true")))
+        for item in self.__specific:
+            _specoptions.append("{}={}".format(
+                quote(item),
+                str(self.__specific[item])
+                .replace("False", "false")
+                .replace("True", "true")))
         _link += "&".join(_options + _specoptions)
         _link = _link.format(quote(str(self.__style)), quote(self.__seed))
         req = r.get(_link)
         self.__checkLinkError(req.text)
         self.__url_svg = req.url
 
     @staticmethod
     def __uniquify(path) -> str:
         filename, extension = os.path.splitext(path)
-        counter = 1
+        counter = 0
         while os.path.exists(path):
-            path = filename + "(" + str(counter) + ")" + extension
             counter += 1
+            path = filename + "(" + str(counter) + ")" + extension
         return path
 
-    def edit(self,
-             *,
-             style: DStyle = None,
-             seed: str = None,
-             extra_options: DOptions = None,
-             blank_options: DOptions = None
-             ) -> str:
+    def edit(self, *, style: DStyle = None, seed: str = None, extra_options: DOptions = None,
+             blank_options: DOptions = None) -> str:
         """
         Edit an already existing avatar.
 
         :param style: class `DStyle` :: edit the avatar's style (style of drawing)
         :type style: dicebear.models.DStyle
         :param seed: class `str` :: edit the avatar's seed (string to determine its looks)
         :type seed: str
@@ -309,19 +299,15 @@
         if extra_options:
             self.__options.update(extra_options)
         elif blank_options:
             self.__options = blank_options
         self.__update()
         return self.__url_svg
 
-    def customise(self,
-                  *,
-                  extra_options: dict = None,
-                  blank_options: dict = None
-                  ) -> str:
+    def customise(self, *, extra_options: dict = None, blank_options: dict = None) -> str:
         """
         Customise the specific options for an already existing avatar.
 
         :param extra_options: class `DOptions` :: edit the avatar's specific options (old options stay, these get added) -- cannot be used at the same time with `blank_options` !
         :type extra_options: dicebear.models.DOptions
         :param blank_options: class `DOptions` :: reset old specific options and set these options as new ones (new options) -- cannot be used at the same with `extra_options` !
         :type blank_options: dicebear.models.DOptions
@@ -333,22 +319,16 @@
         elif blank_options:
             self.__specific = blank_options
         self.__update()
         return self.__url_svg
 
     customize: callable = customise
 
-    def save(self,
-             *,
-             location: Union[pathlib.Path, str] = None,
-             file_name: str = "dicebear_avatar",
-             file_format: DFormat = DFormat.svg,
-             overwrite: bool = False,
-             open_after_save: bool = False
-             ) -> str:
+    def save(self, *, location: Union[pathlib.Path, str] = None, file_name: str = "dicebear_avatar",
+             file_format: DFormat = DFormat.svg, overwrite: bool = False, open_after_save: bool = False) -> str:
         """
         Save the avatar to your device.
 
         :param location: class `pathlib.Path` :: the folder to save the file in. (default is `None` which saves it in the current directory `os.getcwd()`)
         :type location: pathlib.Path
         :param file_name: class `str` :: the name of the file to save. (default is "dicebear_avatar")
         :type file_name: str
@@ -367,48 +347,42 @@
         if location is None: location = pathlib.Path(os.getcwd())
         _location = os.path.join(location, "{}.{}".format(file_name, file_format))
         _location = self.__uniquify(_location) if overwrite is False else _location
         ret = -1
         try:
             if file_format in [DFormat.svg, DFormat.json]:
                 with open(_location, "w", encoding="UTF-8") as f:
-                    f.write(self.text(DFormat.json if file_format == DFormat.json else DFormat.svg))
+                    f.write(self.text(file_format))
                 f.close()
             else:
                 with open(_location, "wb") as f:
-                    f.write(self.bytes(DFormat.jpg if file_format == DFormat.jpg else DFormat.png).read())
+                    f.write(self.bytes(file_format).read())
                 f.close()
             ret = _location
         except ValueError:
             raise ImageValueError(_location)
         except OSError as e:
             raise ImageOSError(str(e))
-        except Exception as e:
-            raise e
         if open_after_save: self.view(use_pil=False)
         return ret
 
     @_pilcheck
-    def pillow(self) -> i.Image:
+    def pillow(self) -> Im.Image:
         """
         Convert a :py:class:`DAvatar` to a :py:class:`PIL.Image.Image` object.
 
         :return: :py:class:`PIL.Image.Image`
         :raise `dicebear.errors.PILError`:
         """
         _statsIncrease(__filename__, self.__class__.__name__, ".pillow()")
-        raw_img = i.open(self.bytes(DFormat.png)).tobytes()
-        img: i.Image = i.frombytes("RGBA", (256, 256), raw_img)
+        raw_img = Im.open(self.bytes(DFormat.png)).tobytes()
+        img: Im.Image = Im.frombytes("RGBA", (256, 256), raw_img)
         return img
 
-    def view(self,
-             *,
-             format: DFormat = DFormat.svg,
-             use_pil: bool = True
-             ) -> None:
+    def view(self, *, format: DFormat = DFormat.svg, use_pil: bool = True) -> None:
         """
         Open and view the avatar on your device.
 
         :param format: class `DFormat` :: what format to use when opening the DAvatar image
         :type format: dicebear.models.DFormat
         :param use_pil: class `bool` :: whether to use Pillow module to open the avatar image
         :type use_pil: bool
@@ -417,14 +391,14 @@
         """
         _statsIncrease(__filename__, self.__class__.__name__, ".view()")
         if use_pil and _FindPil.found is True:
             self.__view_pil()
         elif use_pil and _FindPil.found is False:
             log_error(ModuleNotFoundError("Module `Pillow` is not found or installed"), True)
         else:
-            os.startfile(self.__getattribute__("url_" + str(format)), "open")
+            os.startfile(getattr(self, "url_" + str(format)), "open")
 
     open: callable = view
 
     @_pilcheck
     def __view_pil(self) -> None:
         self.pillow().show("Dicebear Avatar")
```

### Comparing `dicebear-2.7.3/dicebear/errors.py` & `dicebear-2.7.4/dicebear/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,24 @@
 class InvalidOption(Exception):
     """Invalid option"""
     def __init__(self, wrong_option: str = None):
         super().__init__('Invalid option given: "{}" is not an existing option! (use `Avatar.options` to get all possible options)'.format(
             wrong_option))
 
 
-
 class Error(Exception):
     """General error"""
     def __init__(self, error_type: str = "", message: str = ""):
         super().__init__('{}{}'.format(error_type + (': ' if error_type else ''), message))
 
 
 class HTTPError(Error):
     """HTTP error"""
-    def __init__(self, dic: dict):
-        super().__init__(message=str(dic))
-
+    def __init__(self, d: dict):
+        super().__init__(message=str(d))
 
 
 class ImageError(Exception):
     """General image error"""
     def __init__(self, message: str = None):
         super().__init__(message)
 
@@ -83,15 +81,14 @@
 
 class PILError(ImageError):
     """Pillow error"""
     def __init__(self, message: str = "To use this function you need to install Pillow."):
         super().__init__('Module "PIL (=Pillow)" is not found! {}'.format(message))
 
 
-
 _error_logger = logging.getLogger()
 _error_handler = logging.StreamHandler()
 _error_logger.setLevel(logging.ERROR)
 _error_handler.setLevel(logging.ERROR)
 _error_logger.addHandler(_error_handler)
 
 def log_error(exception: Union[Exception, str], raise_error: bool = False) -> None:
@@ -103,9 +100,8 @@
     :param raise_error: class `bool` :: whether to raise this exception or not (default: False)
     :type raise_error: bool
     """
     if raise_error is False:
         _error_handler.setFormatter(logging.Formatter(f"%(levelname)s: {exception.__class__.__name__}: %(message)s"))
         _error_logger.error(exception)
         return
-    raise Exception(exception) if type(exception) == str else exception
-
+    raise Exception(exception) if type(exception) is str else exception
```

### Comparing `dicebear-2.7.3/dicebear/models.py` & `dicebear-2.7.4/dicebear/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 class _FindPil:
     """Not important for you, just makes things easier for me on the back-end ;)"""
     found: bool = True
 
 
 _ascii_lowercase = "abcdef"
-_incorrect_lowercase = "ghijklmnopqrstuvwxyz"
 _digits = "0123456789"
-_y = "https://api.dicebear.com/7.x/{}/schema.json"
+_x = "https://api.dicebear.com/8.x"
+_y = _x + "/{}/schema.json"
 
 options = all_options = ["flip", "rotate", "scale", "radius", "size", "backgroundColor", "backgroundType",
                          "backgroundRotation", "translateX", "translateY", "randomizeIds"]
 style_metadata = {
     "adventurer": {
         "title": "Adventurer",
         "creator": "Lisa Wischofsky",
@@ -332,14 +332,16 @@
             "name": "CC0 1.0",
             "url": "https://creativecommons.org/publicdomain/zero/1.0/",
         },
     },
 }
 
 styles = list(style_metadata.keys())
+
+
 # styles_depricated = ["female", "gridy", "human", "jdenticon", "male"]
 
 
 class DColor:
     """
     Base class for DAvatar's colors.
     """
@@ -350,37 +352,47 @@
 
         :param html_code: :py:class:`str` :: the html color code to use as color. This can be a list of strings if `backgroundType` has been set to "gradientLinear". (default: transparent)
         :type html_code: str
         :raise dicebear.errors.IncorrectColor: if the given html_code is an invalid hex color
         """
         code_list: list = []
         hex_list: list = []
-        if type(html_code) == str:
+        if type(html_code) is str:
             code_list = html_code.replace(" ", "").split(",")
-        elif type(html_code) == list and all(type(x) == str for x in html_code):
+        elif type(html_code) is list and all(type(x) is str for x in html_code):
             code_list = html_code
         for code in code_list:
-            if code.startswith("#"): code = code.replace("#", "")
-            if (len(code) != 6 or any(x in code for x in _incorrect_lowercase)) and code != "transparent":
+            code = code.replace("#", "")
+            if (len(code) != 6 or any(x not in (_ascii_lowercase+_digits) for x in code)) and code != "transparent":
                 raise IncorrectColor(str(code))
             hex_list.append(code)
-        self.html_code: str = ",".join(hex_list)
+        self._html_code: str = ",".join(hex_list)
+
+    @property
+    def html_code(self) -> str:
+        """Returns the validated and formatted html/hex color codes."""
+        return str(self._html_code)
+
+    hex_code = html_code
 
     def __str__(self):
         return str(self.html_code)
 
     def __repr__(self):
         return str(self.html_code)
 
+    def __hash__(self):
+        return hash(self.html_code)
+
     def __eq__(self, other):
-        if type(other) == DColor: return self.html_code == other.html_code
+        if type(other) is DColor: return self.html_code == other.html_code
         return self.html_code == other
 
     def __ne__(self, other):
-        if type(other) == DColor: return self.html_code != other.html_code
+        if type(other) is DColor: return self.html_code != other.html_code
         return self.html_code != other
 
     @staticmethod
     def random() -> "DColor":
         """
         Get a random html code.
 
@@ -451,23 +463,23 @@
         """
         Get a random style.
 
         :return: a random style
         """
         return choice(styles)
 
-    @classmethod
-    def from_str(cls, style_str: str) -> str:
+    @staticmethod
+    def from_str(style_str: str) -> str:
         """
         Get an avatar style from a string.
 
         :param style_str: :py:class:`str` :: the string to convert to a DStyle
         :type style_str: str
         """
-        return getattr(cls, style_str.replace("-", "_"))
+        return getattr(DStyle, style_str.replace("-", "_"))
 
 
 class DFormat:
     """
     All possible image formats for saving or converting avatars.
     - Note: Only works with attributes!
     """
@@ -477,23 +489,23 @@
     jpg = "jpg"
     json = "json"
 
     def __init__(self):
         """Only use `.attribute` to use a format."""
         raise NotImplementedError("DFormat should not be initialized.")
 
-    @classmethod
-    def from_str(cls, format_str: str) -> str:
+    @staticmethod
+    def from_str(format_str: str) -> str:
         """
         Get an avatar format from a string
 
         :param format_str: :py:class:`str` :: the string to convert to a DFormat
         :type format_str: str
         """
-        return getattr(cls, format_str.replace("DFormat.", ""))
+        return getattr(DFormat, format_str.lower().replace("dformat.", ""))
 
 
 default_options: dict = {options[0]: False, options[1]: 0, options[2]: 100, options[3]: 0, options[4]: 0,
                          options[5]: DColor(), options[6]: "solid", options[7]: 0, options[8]: 0, options[9]: 0,
                          options[10]: False}
 
 
@@ -502,38 +514,37 @@
     The options class for :py:class:`dicebear.avatar.DAvatar`
     """
     empty: dict = {}
     default_options = default = default_options
 
     def __init__(self, *, flip: bool = False, rotate: int = 0, scale: int = 100, radius: int = 0, size: int = 0,
                  backgroundColor: Union[DColor, List[DColor]] = DColor(), backgroundType: str = "solid",
-                 backgroundRotation: int = 0,
-                 translateX: int = 0, translateY: int = 0, randomizeIds: bool = False, **kwargs):
+                 backgroundRotation: int = 0, translateX: int = 0, translateY: int = 0, randomizeIds: bool = False):
         """
         Go to https://github.com/jvherck/dicebear#base-options to see all info (important for minimum and maximum values for each option!)
-
-        :param kwargs: `fromdict` to use a custom dict instead of args (if you use this kwarg all other args will be neglected)
         """
-        dic = kwargs.get("fromdict", {})
-        current: dict = {"flip": flip, "rotate": rotate, "scale": scale, "radius": radius, "size": size,
-                         "backgroundColor": backgroundColor, "backgroundType": backgroundType,
-                         "backgroundRotation": backgroundRotation,
-                         "translateX": translateX, "translateY": translateY, "randomizeIds": randomizeIds}
-        if dic:
-            for item in dic:
-                if item not in default_options.keys() or dic[item] == default_options[item]: dic.pop(item, None)
-        else:  # if not dic
-            for item in current:
-                if item in default_options and current[item] != default_options[item]: dic.update({item: current[item]})
-        if "size" in dic and dic["size"] == 0: dic.pop("size")
-        super().__init__(dic)
+        d = {"flip": flip, "rotate": rotate, "scale": scale, "radius": radius, "size": size,
+             "backgroundColor": backgroundColor, "backgroundType": backgroundType,
+             "backgroundRotation": backgroundRotation, "translateX": translateX, "translateY": translateY,
+             "randomizeIds": randomizeIds}
+        self.update(d.items() - default_options.items())
+        if "size" in self and self["size"] == 0:
+            self.pop("size")
+        super().__init__(self)
 
-    @property
-    def _ver(self):
-        return type(self)
+    @classmethod
+    def from_dict(cls, d: dict) -> "DOptions":
+        """Return a new instance of DOptions from a dict."""
+        for item in d:
+            if item not in default_options.keys() or d[item] == default_options[item]:
+                d.pop(item, None)
+        self = cls()
+        self.clear()
+        self.update(d)
+        return self
 
 
 def _statsIncrease(_file: str, _class: str, _function: str, *, _test: bool = False) -> None:
     """
     Pings an API to update this package's usage stats. This will be used to analyse Dicebear's usage and improve your overall experience.
     """
     if environ.get('ENABLE_PYTHON_DICEBEAR_USAGE_STATS', '').lower() != 'true':
```

### Comparing `dicebear-2.7.3/dicebear/utility.py` & `dicebear-2.7.4/dicebear/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'create_random',
     'bulk_create',
 )
 __filename__ = "utility.py"
 
 
 def create_avatar(
-        style: DStyle,
+        style: Union[str, DStyle],
         seed: str,
         options: Union[DOptions, None] = None,
         customisations: Union[dict, None] = None
 ) -> DAvatar:
     """
     Creates a DAvatar object and returns it.
 
@@ -64,22 +64,23 @@
     :return: DAvatar object
     """
     _statsIncrease(__filename__, "/", ".create_random()")
     options = None
     if randomOptions:
         _type = choice(["solid", "gradientLinear"])
         _color = [DColor.random()]
-        if _type == "gradientLinear": _color.append(DColor.random())
+        if _type == "gradientLinear":
+            _color.append(DColor.random())
         options = DOptions(flip=choice([True, False]), backgroundColor=DColor([str(x) for x in _color]),
                            backgroundType=_type, backgroundRotation=randint(0, 360))
     return DAvatar(DStyle.random(), "".join(choices(ascii_lowercase + digits, k=20)), options=options)
 
 
 def bulk_create(
-        style: DStyle = DStyle.random(),
+        style: Union[str, DStyle] = DStyle.random(),
         amount: Annotated[int, "Min: 1, Max: 50"] = 2,
         *,
         options: DOptions = None,
         custom: dict = None,
 ) -> List[DAvatar]:
     """
     Creates a list of :py:class:`DAvatar` objects. Easy way to make multiple of the same style (but different randomly generated seeds) at once.
```

### Comparing `dicebear-2.7.3/dicebear.egg-info/PKG-INFO` & `dicebear-2.7.4/dicebear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dicebear
-Version: 2.7.3
+Version: 2.7.4
 Summary: A python wrapper for DiceBear's avatar generating API.
 Home-page: https://jvh.gitbook.io/dicebear
 Author: jvherck
-Author-email: contact@janvh.be
+Author-email: jan@vhjan.me
 Maintainer: jvherck
-Maintainer-email: contact@janvh.be
+Maintainer-email: jan@vhjan.me
 License: MIT License
 Project-URL: Documentation, https://jvh.gitbook.io/dicebear
 Project-URL: Source, https://github.com/jvherck/dicebear
 Project-URL: Tracker, https://github.com/jvherck/dicebear/issues
 Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,notionists,notionists-neutral,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -43,36 +43,36 @@
 ![PyPI](https://img.shields.io/pypi/v/dicebear)
 ![GitHub issues](https://img.shields.io/github/issues/jvherck/dicebear)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicebear)
 ![GitHub](https://img.shields.io/github/license/jvherck/dicebear)
 ![Maintenance](https://img.shields.io/maintenance/yes/2024)
 ![PyPI - Status](https://img.shields.io/pypi/status/dicebear)
 
-Always keep an eye on https://jvh.gitbook.io/dicebear/ for updates and warnings about this packages!
+Always keep an eye on https://dicebear.vhjan.me/ for updates and warnings about this packages!
 
-[`dicebear`](https://pypi.org/project/dicebear/) is an API wrapper for https://dicebear.com. Using this wrapper you can get custom avatars for your program. \
+[`dicebear`](https://pypi.org/project/dicebear/) is a Python API wrapper for https://dicebear.com. Using this wrapper you can get custom avatars for your program. \
 For an example go to [`examples/dicebear.py`](https://github.com/jvherck/dicebear/tree/main/examples).
 
 
 ---
 
 
 ## Useful links  
-* Docs: https://jvh.gitbook.io/dicebear/  
+* Official Dicebear: https://dicebear.com/
+* Docs: https://dicebear.vhjan.me/  
 * PyPI: https://pypi.org/project/dicebear/  
 * GitHub: https://github.com/jvherck/dicebear  
-* Dicebear: https://dicebear.com/  
-- Dicebear CLI: https://github.com/jvherck/dicebear-cli  
+* Dicebear Python CLI: https://github.com/jvherck/dicebear-cli  
 
 
 ---
 
 
 ## Changelog
-Find the changelog here: https://github.com/jvherck/dicebear/blob/main/CHANGELOG.md
+Find the changelog here: https://dicebear.vhjan.me/changelog
 
 
 ---
 
 
 ## How to install  
 Run `pip install -U dicebear` \
@@ -273,14 +273,14 @@
 
 
 ---
 
 
 ## Credits  
 Special thanks to [DiceBear](https://github.com/dicebear) ([Florian Körner](https://github.com/FlorianKoerner)) for 
-making this amazing API and to [all artists](https://dicebear.com/licenses) that helped making avatars!  
+making this amazing API and to [all artists](https://dicebear.com/licenses) for creating these avatars!  
 
 
 ## Licenses and privacy policy  
 - Dicebear **Licenses**: https://dicebear.com/licenses  
 - Dicebear **Privacy Policy**: https://dicebear.com/legal/privacy-policy  
-- Dicebear Python API wrapper (this project): https://jvh.gitbook.io/dicebear/license
+- Dicebear Python API wrapper (this project): https://dicebear.vhjan.me/license
```

### Comparing `dicebear-2.7.3/setup.py` & `dicebear-2.7.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     long_description = fh.read()
 
 setup(
     name="dicebear",
     version=__version__,
     license="MIT License",
     author="jvherck",
-    author_email="contact@janvh.be",
+    author_email="jan@vhjan.me",
     maintainer="jvherck",
-    maintainer_email="contact@janvh.be",
+    maintainer_email="jan@vhjan.me",
     url="https://jvh.gitbook.io/dicebear",
     project_urls={"Documentation": "https://jvh.gitbook.io/dicebear", "Source": "https://github.com/jvherck/dicebear", "Tracker": "https://github.com/jvherck/dicebear/issues"},
     description="A python wrapper for DiceBear's avatar generating API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['requests', 'urllib3'],
```

### Comparing `dicebear-2.7.3/tests/test_main.py` & `dicebear-2.7.4/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,22 @@
 class TAvatar(unittest.TestCase):
     def testBase(self):
         style = models.DStyle.random()
         seed = "John Apple"
         options = models.DOptions(flip=True, rotate=90, backgroundType="gradientLinear")
         av = avatar.DAvatar(style, seed, options=options)
         self.assertEqual(
-            av,
-            avatar._x.format(quote(style), quote(seed)) + "flip=true&rotate=90&backgroundType=gradientLinear"
+            str(av)[:-49],
+            avatar._y.format(quote(style), quote(seed))
         )
+        urlparams = str(av)[-68:]
+        self.assertIn("?seed=John%20Apple&", urlparams)
+        self.assertIn("flip=true", urlparams)
+        self.assertIn("rotate=90", urlparams)
+        self.assertIn("backgroundType=gradientLinear", urlparams)
 
     def test2(self):
         style = "John Apple"
         seed = "John Apple"
         options = models.DOptions(flip=True, rotate=90, backgroundType="gradientLinear")
         self.assertRaises(
             errors.Error,
@@ -103,29 +108,29 @@
         custom = {
             "eyes": "dizzy",
             "texture": "camo01",
             "somethingWrong": "doesNotMatter"
         }
         av = avatar.DAvatar(style, seed, options=options, custom=custom)
         self.assertEqual(
-            av,
-            avatar._x.format(quote(style), quote(seed)) + "flip=true&eyes=dizzy&texture=camo01&somethingWrong=doesNotMatter"
+            str(av),
+            avatar._y.format(quote(style), quote(seed)) + "flip=true&eyes=dizzy&texture=camo01&somethingWrong=doesNotMatter"
         )
 
 
 class TUtil(unittest.TestCase):
     def testSingle(self):
         style = models.DStyle.random()
         seed = "John Apple"
         options = models.DOptions(rotate=90)
         custom = {"scale": "52"}
         av = utility.create_avatar(style, seed, options, custom)
         self.assertEqual(
             av,
-            avatar._x.format(quote(style), quote(seed)) + "rotate=90&scale=52"
+            avatar._y.format(quote(style), quote(seed)) + "rotate=90&scale=52"
         )
 
     def testRandom(self):
         av = utility.create_random(True)
         _url_svg = av.url_svg
         self.assertEqual(av.url_svg, _url_svg)
```

