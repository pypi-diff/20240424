# Comparing `tmp/django_img_optimizer-1.1.tar.gz` & `tmp/django_img_optimizer-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_img_optimizer-1.1.tar", last modified: Mon Apr 22 07:17:12 2024, max compression
+gzip compressed data, was "django_img_optimizer-1.2.tar", last modified: Wed Apr 24 05:46:28 2024, max compression
```

## Comparing `django_img_optimizer-1.1.tar` & `django_img_optimizer-1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.343988 django_img_optimizer-1.1/django_img_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/django_img_optimizer/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/django_img_optimizer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/management/commands/optimize_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/django_img_optimizer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/templatetags/image_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/django_img_optimizer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/django_img_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-22 07:17:12.000000 django_img_optimizer-1.1/django_img_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-22 07:17:12.000000 django_img_optimizer-1.1/django_img_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:17:12.000000 django_img_optimizer-1.1/django_img_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 07:17:12.000000 django_img_optimizer-1.1/django_img_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 07:17:12.000000 django_img_optimizer-1.1/django_img_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:17:12.347988 django_img_optimizer-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-22 07:17:03.000000 django_img_optimizer-1.1/tests/test_build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/management/commands/optimize_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/templatetags/image_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/tests/test_build.py
```

### Comparing `django_img_optimizer-1.1/LICENSE` & `django_img_optimizer-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.1/PKG-INFO` & `django_img_optimizer-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-img-optimizer
-Version: 1.1
+Version: 1.2
 Summary: Image optimizer for Django.
 Author: Peter Stavrou
 License: MIT
 Project-URL: Homepage, https://github.com/peterstavrou/django-img-optimizer
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow>=10.2.0
 
 # Django Image Optimizer
 
-[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.1/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
+[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.2/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
 
 Django Image Optimizer converts images to WebP format while allowing you to specify the quality of the image. Optimized images that are larger than their originals are automatically deleted.
 
 ## Installation
     pip install django-img-optimizer
 
 ## Configuration
@@ -103,14 +103,22 @@
     <picture>
         <source srcset="/static/images/logo.webp" type="image/webp">
         <img loading="lazy" decoding="async" src="/static/images/logo.jpg" alt="Logo" class="img-fluid">
     </picture>
 
 Pass in any `<img>` attribute by wrapping it between  single quotes `'`.
 
+You can use `auto` to generated the value of the `alt` and `title` attribute automatically using its filename.
+
+**Example:**
+
+    {% optimized_image 'src="images/logo-auto-attributes.jpg"' 'alt="auto"' 'title="auto"' %}
+
+This will render `alt="Logo Auto Attributes"` and `title="Logo Auto Attributes"`.
+
 You can use variables with the `optimize_image` template tag that have been passed through `include` by using the built-in Django filter <a href="https://docs.djangoproject.com/en/5.0/ref/templates/builtins/#add" target="_blank">add</a>.
 
 **Example:**
 
 index.html
 
     {% include 'partials/include.html' with image_name='logo'  %}
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.1 Summary: Image
+Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.2 Summary: Image
 optimizer for Django. Author: Peter Stavrou License: MIT Project-URL: Homepage,
 https://github.com/peterstavrou/django-img-optimizer Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pillow>=10.2.0 # Django Image
 Optimizer [![pytest](https://github.com/peterstavrou/django-img-optimizer/
 actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-
 img-optimizer/actions)   [![pypi](https://img.shields.io/badge/dynamic/
 toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/
 main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)]
-(https://pypi.org/project/django-img-optimizer/1.1/)   [![mit-license](https://
+(https://pypi.org/project/django-img-optimizer/1.2/)   [![mit-license](https://
 img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/
 django-img-optimizer/blob/main/LICENSE) Django Image Optimizer converts images
 to WebP format while allowing you to specify the quality of the image.
 Optimized images that are larger than their originals are automatically
 deleted. ## Installation pip install django-img-optimizer ## Configuration Add
 django_img_optimizer to `INSTALLED_APPS` in your projects `settings.py` file:
 ``` INSTALLED_APPS = [ ... 'django_img_optimizer', ... ] ``` Set
@@ -32,19 +32,23 @@
 OPTIMIZE_IMAGE_EXCLUDED_FOLDERS = ['backup-larger-versions'] ## Usage ###
 Command line Optimize all images: python manage.py optimize_images Delete all
 optimized images: python manage.py optimize_images --delete ### Django
 templates Load the optimized images in Django templates: {% load
 image_optimizer %} {% optimized_image 'loading="lazy"' 'decoding="async"'
 'src="images/logo.jpg"' 'alt="Logo"' 'class="img-fluid"' %} This will render:
 [Logo]Pass in any `[Image]` attribute by wrapping it between single quotes `'`.
-You can use variables with the `optimize_image` template tag that have been
-passed through `include` by using the built-in Django filter _a_d_d. **Example:**
-index.html {% include 'partials/include.html' with image_name='logo' %}
-include.html {% with src='"images/'|add:image_name|add:'.jpg"' %} {%
-optimized_image 'src='|add:src %} {% endwith %} This will render: [/static/
-images/logo.jpg]**Code Breakdown:** src is set to: `src='"images/'` The single
-quotes `'` around `"images/` indicates that it is a string. `|add:image_name`
-adds the `image_name` variable to the string, resulting in: `src="images/logo`
-`|add:'.jpg"'` adds `.jpg"` to the string, resulting in: `src="images/
-logo.jpg"` ## AVIF Image Support django_img_optimizer utilizes `python-pillow`
-which currently lacks official support for AVIF files. However, a _p_u_l_l_ _r_e_q_u_e_s_t
-is in progress to enable this.
+You can use `auto` to generated the value of the `alt` and `title` attribute
+automatically using its filename. **Example:** {% optimized_image 'src="images/
+logo-auto-attributes.jpg"' 'alt="auto"' 'title="auto"' %} This will render
+`alt="Logo Auto Attributes"` and `title="Logo Auto Attributes"`. You can use
+variables with the `optimize_image` template tag that have been passed through
+`include` by using the built-in Django filter _a_d_d. **Example:** index.html {%
+include 'partials/include.html' with image_name='logo' %} include.html {% with
+src='"images/'|add:image_name|add:'.jpg"' %} {% optimized_image 'src='|add:src
+%} {% endwith %} This will render: [/static/images/logo.jpg]**Code Breakdown:**
+src is set to: `src='"images/'` The single quotes `'` around `"images/
+` indicates that it is a string. `|add:image_name` adds the `image_name`
+variable to the string, resulting in: `src="images/logo` `|add:'.jpg"'` adds
+`.jpg"` to the string, resulting in: `src="images/logo.jpg"` ## AVIF Image
+Support django_img_optimizer utilizes `python-pillow` which currently lacks
+official support for AVIF files. However, a _p_u_l_l_ _r_e_q_u_e_s_t is in progress to
+enable this.
```

### Comparing `django_img_optimizer-1.1/README.md` & `django_img_optimizer-1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Django Image Optimizer
 
-[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.1/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
+[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.2/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
 
 Django Image Optimizer converts images to WebP format while allowing you to specify the quality of the image. Optimized images that are larger than their originals are automatically deleted.
 
 ## Installation
     pip install django-img-optimizer
 
 ## Configuration
@@ -90,14 +90,22 @@
     <picture>
         <source srcset="/static/images/logo.webp" type="image/webp">
         <img loading="lazy" decoding="async" src="/static/images/logo.jpg" alt="Logo" class="img-fluid">
     </picture>
 
 Pass in any `<img>` attribute by wrapping it between  single quotes `'`.
 
+You can use `auto` to generated the value of the `alt` and `title` attribute automatically using its filename.
+
+**Example:**
+
+    {% optimized_image 'src="images/logo-auto-attributes.jpg"' 'alt="auto"' 'title="auto"' %}
+
+This will render `alt="Logo Auto Attributes"` and `title="Logo Auto Attributes"`.
+
 You can use variables with the `optimize_image` template tag that have been passed through `include` by using the built-in Django filter <a href="https://docs.djangoproject.com/en/5.0/ref/templates/builtins/#add" target="_blank">add</a>.
 
 **Example:**
 
 index.html
 
     {% include 'partials/include.html' with image_name='logo'  %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # Django Image Optimizer [![pytest](https://github.com/peterstavrou/django-img-
 optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/
 peterstavrou/django-img-optimizer/actions)   [![pypi](https://img.shields.io/
 badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-
 img-optimizer/main/
 pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://
-pypi.org/project/django-img-optimizer/1.1/)   [![mit-license](https://
+pypi.org/project/django-img-optimizer/1.2/)   [![mit-license](https://
 img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/
 django-img-optimizer/blob/main/LICENSE) Django Image Optimizer converts images
 to WebP format while allowing you to specify the quality of the image.
 Optimized images that are larger than their originals are automatically
 deleted. ## Installation pip install django-img-optimizer ## Configuration Add
 django_img_optimizer to `INSTALLED_APPS` in your projects `settings.py` file:
 ``` INSTALLED_APPS = [ ... 'django_img_optimizer', ... ] ``` Set
@@ -28,19 +28,23 @@
 OPTIMIZE_IMAGE_EXCLUDED_FOLDERS = ['backup-larger-versions'] ## Usage ###
 Command line Optimize all images: python manage.py optimize_images Delete all
 optimized images: python manage.py optimize_images --delete ### Django
 templates Load the optimized images in Django templates: {% load
 image_optimizer %} {% optimized_image 'loading="lazy"' 'decoding="async"'
 'src="images/logo.jpg"' 'alt="Logo"' 'class="img-fluid"' %} This will render:
 [Logo]Pass in any `[Image]` attribute by wrapping it between single quotes `'`.
-You can use variables with the `optimize_image` template tag that have been
-passed through `include` by using the built-in Django filter _a_d_d. **Example:**
-index.html {% include 'partials/include.html' with image_name='logo' %}
-include.html {% with src='"images/'|add:image_name|add:'.jpg"' %} {%
-optimized_image 'src='|add:src %} {% endwith %} This will render: [/static/
-images/logo.jpg]**Code Breakdown:** src is set to: `src='"images/'` The single
-quotes `'` around `"images/` indicates that it is a string. `|add:image_name`
-adds the `image_name` variable to the string, resulting in: `src="images/logo`
-`|add:'.jpg"'` adds `.jpg"` to the string, resulting in: `src="images/
-logo.jpg"` ## AVIF Image Support django_img_optimizer utilizes `python-pillow`
-which currently lacks official support for AVIF files. However, a _p_u_l_l_ _r_e_q_u_e_s_t
-is in progress to enable this.
+You can use `auto` to generated the value of the `alt` and `title` attribute
+automatically using its filename. **Example:** {% optimized_image 'src="images/
+logo-auto-attributes.jpg"' 'alt="auto"' 'title="auto"' %} This will render
+`alt="Logo Auto Attributes"` and `title="Logo Auto Attributes"`. You can use
+variables with the `optimize_image` template tag that have been passed through
+`include` by using the built-in Django filter _a_d_d. **Example:** index.html {%
+include 'partials/include.html' with image_name='logo' %} include.html {% with
+src='"images/'|add:image_name|add:'.jpg"' %} {% optimized_image 'src='|add:src
+%} {% endwith %} This will render: [/static/images/logo.jpg]**Code Breakdown:**
+src is set to: `src='"images/'` The single quotes `'` around `"images/
+` indicates that it is a string. `|add:image_name` adds the `image_name`
+variable to the string, resulting in: `src="images/logo` `|add:'.jpg"'` adds
+`.jpg"` to the string, resulting in: `src="images/logo.jpg"` ## AVIF Image
+Support django_img_optimizer utilizes `python-pillow` which currently lacks
+official support for AVIF files. However, a _p_u_l_l_ _r_e_q_u_e_s_t is in progress to
+enable this.
```

### Comparing `django_img_optimizer-1.1/django_img_optimizer/management/commands/optimize_images.py` & `django_img_optimizer-1.2/django_img_optimizer/management/commands/optimize_images.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.1/django_img_optimizer/templatetags/image_optimizer.py` & `django_img_optimizer-1.2/django_img_optimizer/templatetags/image_optimizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         str: A html picture tag with an optimized webp image if it exists, or just the original image if no optimized image is found.
 
     Args:
         *args: Variable number of arguments representing the attributes for the image tag.
     """
     attributes = ' '.join(args)
 
-
     # Get src attribute value
     match_src = re.search(r'src="([^"]+)"', attributes)
     # print(match_src)
     # print('************')
     relative_image_path = match_src.group(1) if match_src.group(1) is not None else "src could not be found"
 
     # Get django static path
@@ -36,14 +35,19 @@
 
     if optimized_image_webp_absolute_path:
         optimized_image_static_src = static(f'{relative_image_path_without_extension}.webp')
         optimized_image_webp = f'<source srcset="{optimized_image_static_src}" type="image/webp">'
     else:
         optimized_image_webp = ''
 
+    # Create alt and/or title attribute using image name
+    if 'alt="auto"' in attributes_output or 'title="auto"' in attributes_output:
+        image_name = relative_image_path_without_extension.split('/')[-1].replace('-', ' ').title()
+        attributes_output = attributes_output.replace('="auto"', f'="{image_name}"')
+
     # Create html picture tag
     picture_tag = f'''
     <picture>
         {optimized_image_webp}
         <img {attributes_output}>
     </picture>
     '''
```

### Comparing `django_img_optimizer-1.1/django_img_optimizer/utils.py` & `django_img_optimizer-1.2/django_img_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.1/django_img_optimizer.egg-info/PKG-INFO` & `django_img_optimizer-1.2/django_img_optimizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-img-optimizer
-Version: 1.1
+Version: 1.2
 Summary: Image optimizer for Django.
 Author: Peter Stavrou
 License: MIT
 Project-URL: Homepage, https://github.com/peterstavrou/django-img-optimizer
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow>=10.2.0
 
 # Django Image Optimizer
 
-[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.1/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
+[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.2/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
 
 Django Image Optimizer converts images to WebP format while allowing you to specify the quality of the image. Optimized images that are larger than their originals are automatically deleted.
 
 ## Installation
     pip install django-img-optimizer
 
 ## Configuration
@@ -103,14 +103,22 @@
     <picture>
         <source srcset="/static/images/logo.webp" type="image/webp">
         <img loading="lazy" decoding="async" src="/static/images/logo.jpg" alt="Logo" class="img-fluid">
     </picture>
 
 Pass in any `<img>` attribute by wrapping it between  single quotes `'`.
 
+You can use `auto` to generated the value of the `alt` and `title` attribute automatically using its filename.
+
+**Example:**
+
+    {% optimized_image 'src="images/logo-auto-attributes.jpg"' 'alt="auto"' 'title="auto"' %}
+
+This will render `alt="Logo Auto Attributes"` and `title="Logo Auto Attributes"`.
+
 You can use variables with the `optimize_image` template tag that have been passed through `include` by using the built-in Django filter <a href="https://docs.djangoproject.com/en/5.0/ref/templates/builtins/#add" target="_blank">add</a>.
 
 **Example:**
 
 index.html
 
     {% include 'partials/include.html' with image_name='logo'  %}
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.1 Summary: Image
+Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.2 Summary: Image
 optimizer for Django. Author: Peter Stavrou License: MIT Project-URL: Homepage,
 https://github.com/peterstavrou/django-img-optimizer Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pillow>=10.2.0 # Django Image
 Optimizer [![pytest](https://github.com/peterstavrou/django-img-optimizer/
 actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-
 img-optimizer/actions)   [![pypi](https://img.shields.io/badge/dynamic/
 toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/
 main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)]
-(https://pypi.org/project/django-img-optimizer/1.1/)   [![mit-license](https://
+(https://pypi.org/project/django-img-optimizer/1.2/)   [![mit-license](https://
 img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/
 django-img-optimizer/blob/main/LICENSE) Django Image Optimizer converts images
 to WebP format while allowing you to specify the quality of the image.
 Optimized images that are larger than their originals are automatically
 deleted. ## Installation pip install django-img-optimizer ## Configuration Add
 django_img_optimizer to `INSTALLED_APPS` in your projects `settings.py` file:
 ``` INSTALLED_APPS = [ ... 'django_img_optimizer', ... ] ``` Set
@@ -32,19 +32,23 @@
 OPTIMIZE_IMAGE_EXCLUDED_FOLDERS = ['backup-larger-versions'] ## Usage ###
 Command line Optimize all images: python manage.py optimize_images Delete all
 optimized images: python manage.py optimize_images --delete ### Django
 templates Load the optimized images in Django templates: {% load
 image_optimizer %} {% optimized_image 'loading="lazy"' 'decoding="async"'
 'src="images/logo.jpg"' 'alt="Logo"' 'class="img-fluid"' %} This will render:
 [Logo]Pass in any `[Image]` attribute by wrapping it between single quotes `'`.
-You can use variables with the `optimize_image` template tag that have been
-passed through `include` by using the built-in Django filter _a_d_d. **Example:**
-index.html {% include 'partials/include.html' with image_name='logo' %}
-include.html {% with src='"images/'|add:image_name|add:'.jpg"' %} {%
-optimized_image 'src='|add:src %} {% endwith %} This will render: [/static/
-images/logo.jpg]**Code Breakdown:** src is set to: `src='"images/'` The single
-quotes `'` around `"images/` indicates that it is a string. `|add:image_name`
-adds the `image_name` variable to the string, resulting in: `src="images/logo`
-`|add:'.jpg"'` adds `.jpg"` to the string, resulting in: `src="images/
-logo.jpg"` ## AVIF Image Support django_img_optimizer utilizes `python-pillow`
-which currently lacks official support for AVIF files. However, a _p_u_l_l_ _r_e_q_u_e_s_t
-is in progress to enable this.
+You can use `auto` to generated the value of the `alt` and `title` attribute
+automatically using its filename. **Example:** {% optimized_image 'src="images/
+logo-auto-attributes.jpg"' 'alt="auto"' 'title="auto"' %} This will render
+`alt="Logo Auto Attributes"` and `title="Logo Auto Attributes"`. You can use
+variables with the `optimize_image` template tag that have been passed through
+`include` by using the built-in Django filter _a_d_d. **Example:** index.html {%
+include 'partials/include.html' with image_name='logo' %} include.html {% with
+src='"images/'|add:image_name|add:'.jpg"' %} {% optimized_image 'src='|add:src
+%} {% endwith %} This will render: [/static/images/logo.jpg]**Code Breakdown:**
+src is set to: `src='"images/'` The single quotes `'` around `"images/
+` indicates that it is a string. `|add:image_name` adds the `image_name`
+variable to the string, resulting in: `src="images/logo` `|add:'.jpg"'` adds
+`.jpg"` to the string, resulting in: `src="images/logo.jpg"` ## AVIF Image
+Support django_img_optimizer utilizes `python-pillow` which currently lacks
+official support for AVIF files. However, a _p_u_l_l_ _r_e_q_u_e_s_t is in progress to
+enable this.
```

### Comparing `django_img_optimizer-1.1/django_img_optimizer.egg-info/SOURCES.txt` & `django_img_optimizer-1.2/django_img_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.1/tests/test_build.py` & `django_img_optimizer-1.2/tests/test_build.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,40 +28,49 @@
 def test_raise_exception_no_OPTIMIZE_IMAGE_root_set_in_settings():
     settings.OPTIMIZE_IMAGE_ROOT = None
 
     with pytest.raises(Exception, match="Set OPTIMIZE_IMAGE_ROOT in settings.py"):
         optimize_images()
 
 def test_optimize_all_images(settings_config):
-
         optimize_images()
+
         # Assert webp image optimization
         assert os.path.exists(f'{settings.OPTIMIZE_IMAGE_ROOT}/logo.webp')
 
         # Assert that subdirectories are traversed
         assert os.path.exists(f'{settings.OPTIMIZE_IMAGE_ROOT}/subdirectory/subdirectory-logo.webp')
 
         # Assert that the OPTIMIZE_IMAGE_EXCLUDED_FOLDERS setting works
         assert not os.path.exists(f'{settings.OPTIMIZE_IMAGE_ROOT}/excluded_folder/exclude.webp')
 
         # Assert that the delete_if_optimized_image_is_smaller_or_equal function works
         assert not os.path.exists(f'{settings.OPTIMIZE_IMAGE_ROOT}/small.webp')
 
-def test_no_optimized_webp_image(client):
+def test_optimized_image_template_tag(client):
     response = client.get('/')
 
     # Assert that the the template tag created a html picture tag containing the optimized webp image
     optimized_image = '''
     <picture>
         <source srcset="/static/images/logo.webp" type="image/webp">
         <img loading="lazy" decoding="async" src="/static/images/logo.jpg" alt="Logo" class="img-fluid">
     </picture>
     '''
     assert optimized_image in response.content.decode()
 
+    # Assert that the the template tag created an alt and title attribute from the image name
+    optimized_image_with_auto_alt_and_title_attributes = '''
+    <picture>
+        <source srcset="/static/images/logo-auto-attributes.webp" type="image/webp">
+        <img loading="lazy" decoding="async" src="/static/images/logo-auto-attributes.jpg" alt="Logo Auto Attributes" title="Logo Auto Attributes">
+    </picture>
+    '''
+    assert optimized_image_with_auto_alt_and_title_attributes in response.content.decode()
+
     # Assert that the template tag created an html picture tag that does not contain a webp image as the optimized size is larger than the original
     not_optimized_image = '''
     <picture>
         <source srcset="/static/images/small.webp" type="image/webp">
         <img loading="lazy" decoding="async" src="/static/images/small.jpg" alt="Logo Small">
     </picture>
     '''
```

