# Comparing `tmp/django_simple_nav-0.5.1.tar.gz` & `tmp/django_simple_nav-0.6.0.tar.gz`

## Comparing `django_simple_nav-0.5.1.tar` & `django_simple_nav-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,61 @@
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/RELEASING.md
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/noxfile.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/.vscode/extensions.json
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/.vscode/settings.json.example
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/changelog.md
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/conf.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/getting-started.md
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/index.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/requirements.in
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/usage.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/development/contributing.md
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/development/just.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/docs/development/releasing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/__init__.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/demo.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/navigation.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/base.html
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/basic.html
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/bootstrap4.html
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/bootstrap5.html
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/extra_context.html
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/nested.html
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/permissions.html
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/picocss.html
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/tailwind.html
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/basic.html
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/bootstrap4.html
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/bootstrap5.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/example_list.html
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/extra_context.html
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/nested.html
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/picocss.html
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/tailwind_main.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/example/templates/navs/tailwind_profile.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/apps.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/conf.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/nav.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/permissions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/templatetags/__init__.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/src/django_simple_nav/templatetags/django_simple_nav.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/navs.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/settings.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/test_conf.py
--rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/test_nav.py
--rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/test_permissions.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/test_templatetags.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/test_version.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/urls.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/templates/tests/alternate.html
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/tests/templates/tests/dummy_nav.html
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/.gitignore
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/AUTHORS.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/LICENSE
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/README.md
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 django_simple_nav-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/RELEASING.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/noxfile.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/changelog.md
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/getting-started.md
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/usage.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/development/contributing.md
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/development/just.md
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/docs/development/releasing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/__init__.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/demo.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/navigation.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/base.html
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/basic.html
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/bootstrap4.html
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/bootstrap5.html
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/extra_context.html
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/nested.html
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/permissions.html
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/picocss.html
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/tailwind.html
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/basic.html
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/bootstrap4.html
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/bootstrap5.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/example_list.html
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/extra_context.html
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/nested.html
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/picocss.html
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/tailwind_main.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/example/templates/navs/tailwind_profile.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/apps.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/conf.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/nav.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/permissions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/templatetags/__init__.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/src/django_simple_nav/templatetags/django_simple_nav.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/navs.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/settings.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/test_conf.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/test_nav.py
+-rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/test_permissions.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/test_templatetags.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/test_version.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/urls.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/templates/tests/alternate.html
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/tests/templates/tests/dummy_nav.html
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/.gitignore
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/AUTHORS.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/README.md
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13636 2020-02-02 00:00:00.000000 django_simple_nav-0.6.0/PKG-INFO
```

### Comparing `django_simple_nav-0.5.1/CHANGELOG.md` & `django_simple_nav-0.6.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,95 +14,110 @@
 ### Fixed - for any bug fixes
 ### Security - in case of vulnerabilities
 [${version}]: https://github.com/westerveltco/django-simple-nav/releases/tag/v${version}
 -->
 
 ## [Unreleased]
 
+## [0.6.0]
+
+### Added
+
+-   Added two new methods to `Nav`: `get_items` and `get_template_name`. These should allow for further flexibility and customization of rendering the `Nav`.
+
+### Changed
+
+-   Now using v2024.16 of `django-twc-package`.
+
+### Fixed
+
+-   Active nav item matching is now correctly using the `url` property on `RenderedNavItem`.
+
 ## [0.5.1]
 
 ### Added
 
-- Added the requisite `py.typed` file to the package, so that it plays nicely when type-checking in projects using `django-simple-nav`.
+-   Added the requisite `py.typed` file to the package, so that it plays nicely when type-checking in projects using `django-simple-nav`.
 
 ## [0.5.0]
 
 ### Added
 
-- An number of examples have been added to a new `example` directory. These examples are intended to demonstrate various ways how to use `django-simple-nav` in a Django project and include basic usage and usage with some popular CSS frameworks.
+-   An number of examples have been added to a new `example` directory. These examples are intended to demonstrate various ways how to use `django-simple-nav` in a Django project and include basic usage and usage with some popular CSS frameworks.
 
 ### Changed
 
-- `check_item_permission` now takes a `request` argument instead of a `user` argument.
+-   `check_item_permission` now takes a `request` argument instead of a `user` argument.
 
 ### Fixed
 
-- `check_item_permission` now explicitly checks if `django.contrib.auth` is installed before attempting to check if a user has a permission. If it is not, it will return `True` by default and log a warning.
-- The `request` object is now passed to `render_to_string` when rendering the navigation template, so that the `request` object is available in the template context. This allows for nesting the `django_simple_nav` template tag within another `django_simple_nav` template tag, and having the `request` object available in the nested template.
+-   `check_item_permission` now explicitly checks if `django.contrib.auth` is installed before attempting to check if a user has a permission. If it is not, it will return `True` by default and log a warning.
+-   The `request` object is now passed to `render_to_string` when rendering the navigation template, so that the `request` object is available in the template context. This allows for nesting the `django_simple_nav` template tag within another `django_simple_nav` template tag, and having the `request` object available in the nested template.
 
 ## [0.4.0]
 
 ### Added
 
-- The `Nav` class now has two new methods: `get_context_data` and `render`. These methods are used to render the navigation to a template. These new methods give greater flexibility for customizing the rendering of the navigation, as they can be overridden when defining a new `Nav`.
-  - `Nav.get_context_data` method takes a Django `HttpRequest` object and returns a dictionary of context data that can be used to render the navigation to a template.
-  - `Nav.render` method takes a Django `HttpRequest` object and an optional template name and renders the navigation to a template, returning the rendered template as a string.
+-   The `Nav` class now has two new methods: `get_context_data` and `render`. These methods are used to render the navigation to a template. These new methods give greater flexibility for customizing the rendering of the navigation, as they can be overridden when defining a new `Nav`.
+    -   `Nav.get_context_data` method takes a Django `HttpRequest` object and returns a dictionary of context data that can be used to render the navigation to a template.
+    -   `Nav.render` method takes a Django `HttpRequest` object and an optional template name and renders the navigation to a template, returning the rendered template as a string.
 
 ### Removed
 
-- `Nav.render_from_request` method has been removed. This was only used within the template tag to render a `Nav` template from an `HttpRequest` object. It has been removed in favor of the new `Nav.get_context_data` and `Nav.render` methods.
+-   `Nav.render_from_request` method has been removed. This was only used within the template tag to render a `Nav` template from an `HttpRequest` object. It has been removed in favor of the new `Nav.get_context_data` and `Nav.render` methods.
 
 ## [0.3.0]
 
 ### Added
 
-- `NavGroup` and `NavItem` now has a new `extra_context` attribute. This allows for passing additional context to the template when rendering the navigation, either via the extra attribute (`item.foo`) or the `extra_context` attribute itself (`item.extra_context.foo`).
+-   `NavGroup` and `NavItem` now has a new `extra_context` attribute. This allows for passing additional context to the template when rendering the navigation, either via the extra attribute (`item.foo`) or the `extra_context` attribute itself (`item.extra_context.foo`).
 
 ### Changed
 
-- Now using v2024.13 of `django-twc-package`.
+-   Now using v2024.13 of `django-twc-package`.
 
 ### Fixed
 
-- `RenderedNavItem.items` property now correctly returns a list of `RenderedNavItem` objects, rather than a list of `NavItem` objects. This fixes a bug where the properties that should be available (e.g. `active`, `url`, etc.) were not available when iterating over the `RenderedNavItem.items` list if the item was a `NavGroup` object with child items.
+-   `RenderedNavItem.items` property now correctly returns a list of `RenderedNavItem` objects, rather than a list of `NavItem` objects. This fixes a bug where the properties that should be available (e.g. `active`, `url`, etc.) were not available when iterating over the `RenderedNavItem.items` list if the item was a `NavGroup` object with child items.
 
 ## [0.2.0]
 
 ### Added
 
-- The `django_simple_nav` template tag can now take an instance of a `Nav` class, in addition to a `Nav` dotted path string. This should give greater flexibility for rendering a `Nav`, as it can now be overridden on a per-view/template basis.
+-   The `django_simple_nav` template tag can now take an instance of a `Nav` class, in addition to a `Nav` dotted path string. This should give greater flexibility for rendering a `Nav`, as it can now be overridden on a per-view/template basis.
 
 ### Changed
 
-- Now using [`django-twc-package`](https://github.com/westerveltco/django-twc-package) template for repository and package structure.
+-   Now using [`django-twc-package`](https://github.com/westerveltco/django-twc-package) template for repository and package structure.
 
 ## [0.1.0]
 
 Initial release! 🎉
 
 ### Added
 
-- A group of navigation classes -- `Nav`, `NavGroup`, and `NavItem` -- that can be used together to build a simple navigation structure.
-  - `Nav` is the main container for a navigation structure.
-  - `NavGroup` is a container for a group of `NavItem` objects.
-  - `NavItem` is a single navigation item.
-- A `django_simple_nav` template tag that renders a `Nav` object to a template. The template tag takes a string represented the dotted path to a `Nav` object and renders it to the template.
-- Navigation item urls can be either a URL string (e.g. `https://example.com/about/` or `/about/`) or a Django URL name (e.g. `about-view`). When rendering out to the template, the template tag will resolve the URL name to the actual URL.
-- Navigation items also can take a list of permissions to control the visibility of the item. The permissions can be user attributes (e.g. `is_staff`, `is_superuser`, etc.) or a specific permission (e.g. `auth.add_user`).
-- Navigation items are marked as `active` if the current request path matches the item's URL. This is can be useful for highlighting the current page in the navigation.
-- A `Nav` object's template can either be set as a class attribute (`template_name`) or passed in as a keyword argument when rendering the template tag. This allows for easy customization of the navigation structure on a per-template or per-view basis.
-- Initial documentation.
-- Initial tests.
-- Initial CI/CD (GitHub Actions).
+-   A group of navigation classes -- `Nav`, `NavGroup`, and `NavItem` -- that can be used together to build a simple navigation structure.
+    -   `Nav` is the main container for a navigation structure.
+    -   `NavGroup` is a container for a group of `NavItem` objects.
+    -   `NavItem` is a single navigation item.
+-   A `django_simple_nav` template tag that renders a `Nav` object to a template. The template tag takes a string represented the dotted path to a `Nav` object and renders it to the template.
+-   Navigation item urls can be either a URL string (e.g. `https://example.com/about/` or `/about/`) or a Django URL name (e.g. `about-view`). When rendering out to the template, the template tag will resolve the URL name to the actual URL.
+-   Navigation items also can take a list of permissions to control the visibility of the item. The permissions can be user attributes (e.g. `is_staff`, `is_superuser`, etc.) or a specific permission (e.g. `auth.add_user`).
+-   Navigation items are marked as `active` if the current request path matches the item's URL. This is can be useful for highlighting the current page in the navigation.
+-   A `Nav` object's template can either be set as a class attribute (`template_name`) or passed in as a keyword argument when rendering the template tag. This allows for easy customization of the navigation structure on a per-template or per-view basis.
+-   Initial documentation.
+-   Initial tests.
+-   Initial CI/CD (GitHub Actions).
 
 ### New Contributors
 
-- Josh Thomas <josh@joshthomas.dev> (maintainer)
-- Jeff Triplett [@jefftriplett](https://github.com/jefftriplett)
+-   Josh Thomas <josh@joshthomas.dev> (maintainer)
+-   Jeff Triplett [@jefftriplett](https://github.com/jefftriplett)
 
-[unreleased]: https://github.com/westerveltco/django-simple-nav/compare/v0.5.1...HEAD
+[unreleased]: https://github.com/westerveltco/django-simple-nav/compare/v0.6.0...HEAD
 [0.1.0]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.1.0
 [0.2.0]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.2.0
 [0.3.0]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.3.0
 [0.4.0]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.4.0
 [0.5.0]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.5.0
 [0.5.1]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.5.1
+[0.6.0]: https://github.com/westerveltco/django-simple-nav/releases/tag/v0.6.0
```

### Comparing `django_simple_nav-0.5.1/CONTRIBUTING.md` & `django_simple_nav-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/RELEASING.md` & `django_simple_nav-0.6.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/noxfile.py` & `django_simple_nav-0.6.0/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,15 +72,18 @@
     if django == DJMAIN:
         session.install(
             "django @ https://github.com/django/django/archive/refs/heads/main.zip"
         )
     else:
         session.install(f"django=={django}")
 
-    session.run("python", "-m", "pytest")
+    if session.posargs:
+        session.run("python", "-m", "pytest", *session.posargs)
+    else:
+        session.run("python", "-m", "pytest")
 
 
 @nox.session
 def coverage(session):
     session.install("django-simple-nav[dev] @ .")
     session.run("python", "-m", "pytest", "--cov=django_simple_nav")
```

### Comparing `django_simple_nav-0.5.1/docs/conf.py` & `django_simple_nav-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/docs/development/just.md` & `django_simple_nav-0.6.0/docs/development/just.md`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/demo.py` & `django_simple_nav-0.6.0/example/demo.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/navigation.py` & `django_simple_nav-0.6.0/example/navigation.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/base.html` & `django_simple_nav-0.6.0/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/bootstrap4.html` & `django_simple_nav-0.6.0/example/templates/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/bootstrap5.html` & `django_simple_nav-0.6.0/example/templates/bootstrap5.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/basic.html` & `django_simple_nav-0.6.0/example/templates/navs/basic.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/bootstrap4.html` & `django_simple_nav-0.6.0/example/templates/navs/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/bootstrap5.html` & `django_simple_nav-0.6.0/example/templates/navs/bootstrap5.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/example_list.html` & `django_simple_nav-0.6.0/example/templates/navs/example_list.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/extra_context.html` & `django_simple_nav-0.6.0/example/templates/navs/extra_context.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/nested.html` & `django_simple_nav-0.6.0/example/templates/navs/nested.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/picocss.html` & `django_simple_nav-0.6.0/example/templates/navs/picocss.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/example/templates/navs/tailwind_main.html` & `django_simple_nav-0.6.0/example/templates/navs/tailwind_main.html`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/src/django_simple_nav/nav.py` & `django_simple_nav-0.6.0/src/django_simple_nav/nav.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Any
 
+from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpRequest
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 from django.utils.safestring import mark_safe
 
 from django_simple_nav.permissions import check_item_permissions
 
 
 @dataclass(frozen=True)
 class Nav:
-    template_name: str = field(init=False)
-    items: list[NavGroup | NavItem] = field(init=False)
+    template_name: str | None = field(init=False, default=None)
+    items: list[NavGroup | NavItem] | None = field(init=False, default=None)
+
+    def get_template_name(self) -> str:
+        if self.template_name is not None:
+            return self.template_name
+
+        msg = f"{self.__class__!r} must define 'template_name' or override 'get_template_name()'"
+        raise ImproperlyConfigured(msg % self.__class__.__name__)
+
+    def get_items(self, request: HttpRequest) -> list[RenderedNavItem]:
+        if self.items is not None:
+            return [
+                RenderedNavItem(item, request)
+                for item in self.items
+                if check_item_permissions(item, request)
+            ]
+
+        msg = f"{self.__class__!r} must define 'items' or override 'get_items()'"
+        raise ImproperlyConfigured(msg)
 
     def get_context_data(self, request: HttpRequest) -> dict[str, Any]:
-        items = [
-            RenderedNavItem(item, request)
-            for item in self.items
-            if check_item_permissions(item, request)
-        ]
-        return {"items": items}
+        return {
+            "items": self.get_items(request),
+            "request": request,
+        }
 
     def render(self, request: HttpRequest, template_name: str | None = None) -> str:
         context = self.get_context_data(request)
-        context["request"] = request
         return render_to_string(
-            template_name=template_name or self.template_name,
+            template_name=template_name or self.get_template_name(),
             context=context,
             request=request,
         )
 
 
 @dataclass(frozen=True)
 class NavGroup:
@@ -88,14 +104,14 @@
             url = reverse(self.item.url)
         except NoReverseMatch:
             url = self.item.url
         return url
 
     @property
     def active(self) -> bool:
-        if not self.item.url:
+        if not self.url:
             return False
         return (
-            self.request.path.startswith(self.item.url)
-            and self.item.url != "/"
-            or self.request.path == self.item.url
+            self.request.path.startswith(self.url)
+            and self.url != "/"
+            or self.request.path == self.url
         )
```

### Comparing `django_simple_nav-0.5.1/src/django_simple_nav/permissions.py` & `django_simple_nav-0.6.0/src/django_simple_nav/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 
 class User(Protocol):
     is_authenticated: bool
     is_staff: bool
     is_superuser: bool
 
-    def has_perm(self, perm: str) -> bool:
-        ...  # pragma: no cover
+    def has_perm(self, perm: str) -> bool: ...  # pragma: no cover
 
 
 def check_item_permissions(item: NavGroup | NavItem, request: HttpRequest) -> bool:
     if not apps.is_installed("django.contrib.auth"):
         logger.warning(
             "The 'django.contrib.auth' app is not installed, so no permissions will be checked."
         )
```

### Comparing `django_simple_nav-0.5.1/src/django_simple_nav/templatetags/django_simple_nav.py` & `django_simple_nav-0.6.0/src/django_simple_nav/templatetags/django_simple_nav.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/tests/conftest.py` & `django_simple_nav-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/tests/navs.py` & `django_simple_nav-0.6.0/tests/navs.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/tests/settings.py` & `django_simple_nav-0.6.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/tests/test_nav.py` & `django_simple_nav-0.6.0/tests/test_nav.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,13 +229,22 @@
 
     req.path = "/test/"
     rendered_item = RenderedNavItem(item, req)
 
     assert rendered_item.active is True
 
 
-def test_rendered_nav_item_active_no_url(req):
+def test_rendered_nav_group_active_no_url(req):
     item = NavGroup(title="Test", items=[NavItem(title="Test", url="/test/")])
 
     rendered_item = RenderedNavItem(item, req)
 
     assert rendered_item.active is False
+
+
+def test_rendered_nav_item_active_named_url(req):
+    item = NavItem(title="Test", url="fake-view")
+
+    req.path = "/fake-view/"
+    rendered_item = RenderedNavItem(item, req)
+
+    assert rendered_item.active is True
```

### Comparing `django_simple_nav-0.5.1/tests/test_permissions.py` & `django_simple_nav-0.6.0/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/tests/test_templatetags.py` & `django_simple_nav-0.6.0/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/.gitignore` & `django_simple_nav-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/LICENSE` & `django_simple_nav-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/README.md` & `django_simple_nav-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django_simple_nav-0.5.1/pyproject.toml` & `django_simple_nav-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   "coverage[toml]",
   "django-stubs",
   "django-stubs-ext",
   "faker",
   "hatch",
   "mypy",
   "model-bakery",
-  "nox[uv]>=2024.03.02",
+  "nox[uv]",
   "pytest",
   "pytest-cov",
   "pytest-django",
   "pytest-randomly",
   "pytest-reverse",
   "pytest-xdist"
 ]
@@ -67,15 +67,15 @@
 Documentation = "https://django-simple-nav.westervelt.dev/"
 Issues = "https://github.com/westerveltco/django-simple-nav/issues"
 Source = "https://github.com/westerveltco/django-simple-nav"
 
 [tool.bumpver]
 commit = true
 commit_message = ":bookmark: bump version {old_version} -> {new_version}"
-current_version = "0.5.1"
+current_version = "0.6.0"
 push = false  # set to false for CI
 tag = false
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 
 [tool.bumpver.file_patterns]
 ".copier/package.yml" = [
   'current_version: {version}'
@@ -169,15 +169,15 @@
   "node_modules",
   "venv"
 ]
 extend-include = ["*.pyi?"]
 indent-width = 4
 # Same as Black.
 line-length = 88
-# Assume Python >3.8.
+# Assume Python >3.8
 target-version = "py38"
 
 [tool.ruff.format]
 # Like Black, indent with spaces, rather than tabs.
 indent-style = "space"
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
```

### Comparing `django_simple_nav-0.5.1/PKG-INFO` & `django_simple_nav-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: django-simple-nav
-Version: 0.5.1
+Version: 0.6.0
 Summary: A simple, flexible, and extensible navigation menu for Django.
 Project-URL: Documentation, https://django-simple-nav.westervelt.dev/
 Project-URL: Issues, https://github.com/westerveltco/django-simple-nav/issues
 Project-URL: Source, https://github.com/westerveltco/django-simple-nav
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License: MIT License
         
@@ -42,15 +42,15 @@
 Requires-Dist: coverage[toml]; extra == 'dev'
 Requires-Dist: django-stubs; extra == 'dev'
 Requires-Dist: django-stubs-ext; extra == 'dev'
 Requires-Dist: faker; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: model-bakery; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: nox[uv]>=2024.03.02; extra == 'dev'
+Requires-Dist: nox[uv]; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-django; extra == 'dev'
 Requires-Dist: pytest-randomly; extra == 'dev'
 Requires-Dist: pytest-reverse; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
 Provides-Extra: docs
```

