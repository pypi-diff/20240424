# Comparing `tmp/django_ninja_extra-0.20.5.tar.gz` & `tmp/django_ninja_extra-0.20.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_extra-0.20.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ninja_extra-0.20.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ninja_extra-0.20.5.tar` & `django_ninja_extra-0.20.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     4290 2024-04-01 07:01:41.186999 django_ninja_extra-0.20.5/README.md
--rw-r--r--   0        0        0     1554 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/apps.py
--rw-r--r--   0        0        0      440 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/compatible.py
--rw-r--r--   0        0        0       55 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/conf/__init__.py
--rw-r--r--   0        0        0     3560 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/conf/settings.py
--rw-r--r--   0        0        0      575 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/constants.py
--rw-r--r--   0        0        0     1159 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/__init__.py
--rw-r--r--   0        0        0    19025 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/base.py
--rw-r--r--   0        0        0      476 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/__init__.py
--rw-r--r--   0        0        0     6976 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/builder.py
--rw-r--r--   0        0        0    26945 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/endpoints.py
--rw-r--r--   0        0        0     1813 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/interfaces.py
--rw-r--r--   0        0        0     5466 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/path_resolver.py
--rw-r--r--   0        0        0     8116 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/schemas.py
--rw-r--r--   0        0        0     3774 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/model/service.py
--rw-r--r--   0        0        0     1286 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/registry.py
--rw-r--r--   0        0        0      854 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/response.py
--rw-r--r--   0        0        0    25873 2024-04-01 07:01:41.222999 django_ninja_extra-0.20.5/ninja_extra/controllers/route/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/controllers/route/context.py
--rw-r--r--   0        0        0     7875 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/controllers/route/route_functions.py
--rw-r--r--   0        0        0     1434 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/dependency_resolver.py
--rw-r--r--   0        0        0     1879 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/details.py
--rw-r--r--   0        0        0     8927 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/exceptions.py
--rw-r--r--   0        0        0     1775 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/generic.py
--rw-r--r--   0        0        0      597 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/helper.py
--rw-r--r--   0        0        0      670 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/lazy.py
--rw-r--r--   0        0        0       61 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/logger.py
--rw-r--r--   0        0        0     4782 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/main.py
--rw-r--r--   0        0        0     1099 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/modules.py
--rw-r--r--   0        0        0    12921 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/operation.py
--rw-r--r--   0        0        0     8137 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/ordering.py
--rw-r--r--   0        0        0     8354 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/pagination.py
--rw-r--r--   0        0        0      281 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/permissions/__init__.py
--rw-r--r--   0        0        0     5632 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/permissions/base.py
--rw-r--r--   0        0        0     1622 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/permissions/common.py
--rw-r--r--   0        0        0        0 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/py.typed
--rw-r--r--   0        0        0     2195 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/router.py
--rw-r--r--   0        0        0      430 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/schemas/__init__.py
--rw-r--r--   0        0        0     2230 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/schemas/response.py
--rw-r--r--   0        0        0     9223 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/searching.py
--rw-r--r--   0        0        0      748 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/security/__init__.py
--rw-r--r--   0        0        0      880 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/security/api_key.py
--rw-r--r--   0        0        0     1696 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/security/http.py
--rw-r--r--   0        0        0      542 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/security/session.py
--rw-r--r--   0        0        0     2503 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/shortcuts.py
--rw-r--r--   0        0        0      163 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/signals.py
--rw-r--r--   0        0        0     2515 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/status.py
--rw-r--r--   0        0        0      112 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/testing/__init__.py
--rw-r--r--   0        0        0     2089 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/testing/client.py
--rw-r--r--   0        0        0      318 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/throttling/__init__.py
--rw-r--r--   0        0        0     3931 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/throttling/decorator.py
--rw-r--r--   0        0        0     8242 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/throttling/model.py
--rw-r--r--   0        0        0      267 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/types.py
--rw-r--r--   0        0        0     1104 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/ninja_extra/urls.py
--rw-r--r--   0        0        0     2695 2024-04-01 07:01:41.226999 django_ninja_extra-0.20.5/pyproject.toml
--rw-r--r--   0        0        0     6195 1970-01-01 00:00:00.000000 django_ninja_extra-0.20.5/PKG-INFO
+-rw-r--r--   0        0        0     4290 2024-04-24 17:36:28.085167 django_ninja_extra-0.20.6/README.md
+-rw-r--r--   0        0        0     1554 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/apps.py
+-rw-r--r--   0        0        0      440 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/compatible.py
+-rw-r--r--   0        0        0       55 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/conf/__init__.py
+-rw-r--r--   0        0        0     3560 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/conf/settings.py
+-rw-r--r--   0        0        0      577 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/constants.py
+-rw-r--r--   0        0        0     1159 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/__init__.py
+-rw-r--r--   0        0        0    19313 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/base.py
+-rw-r--r--   0        0        0      476 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/__init__.py
+-rw-r--r--   0        0        0     6976 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/builder.py
+-rw-r--r--   0        0        0    26945 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/endpoints.py
+-rw-r--r--   0        0        0     1813 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/interfaces.py
+-rw-r--r--   0        0        0     5466 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/path_resolver.py
+-rw-r--r--   0        0        0     8116 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/schemas.py
+-rw-r--r--   0        0        0     3774 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/service.py
+-rw-r--r--   0        0        0     1286 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/registry.py
+-rw-r--r--   0        0        0      854 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/response.py
+-rw-r--r--   0        0        0    25873 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/route/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/route/context.py
+-rw-r--r--   0        0        0     7875 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/route/route_functions.py
+-rw-r--r--   0        0        0     1434 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/dependency_resolver.py
+-rw-r--r--   0        0        0     1879 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/details.py
+-rw-r--r--   0        0        0     8928 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/exceptions.py
+-rw-r--r--   0        0        0     1775 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/generic.py
+-rw-r--r--   0        0        0      597 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/helper.py
+-rw-r--r--   0        0        0      670 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/lazy.py
+-rw-r--r--   0        0        0       61 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/logger.py
+-rw-r--r--   0        0        0     4782 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/main.py
+-rw-r--r--   0        0        0     1099 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/modules.py
+-rw-r--r--   0        0        0    12921 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/operation.py
+-rw-r--r--   0        0        0     8121 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/ordering.py
+-rw-r--r--   0        0        0     8354 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/pagination.py
+-rw-r--r--   0        0        0      281 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/permissions/__init__.py
+-rw-r--r--   0        0        0     5633 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/permissions/base.py
+-rw-r--r--   0        0        0     1622 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/permissions/common.py
+-rw-r--r--   0        0        0        0 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/py.typed
+-rw-r--r--   0        0        0     2195 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/router.py
+-rw-r--r--   0        0        0      430 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/schemas/__init__.py
+-rw-r--r--   0        0        0     2230 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/schemas/response.py
+-rw-r--r--   0        0        0     9207 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/searching.py
+-rw-r--r--   0        0        0      748 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/__init__.py
+-rw-r--r--   0        0        0      880 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/api_key.py
+-rw-r--r--   0        0        0     1696 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/http.py
+-rw-r--r--   0        0        0      542 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/session.py
+-rw-r--r--   0        0        0     2503 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/shortcuts.py
+-rw-r--r--   0        0        0      163 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/signals.py
+-rw-r--r--   0        0        0     2515 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/status.py
+-rw-r--r--   0        0        0      112 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2089 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/testing/client.py
+-rw-r--r--   0        0        0      318 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/throttling/__init__.py
+-rw-r--r--   0        0        0     3931 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/throttling/decorator.py
+-rw-r--r--   0        0        0     8243 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/throttling/model.py
+-rw-r--r--   0        0        0      267 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/types.py
+-rw-r--r--   0        0        0     1104 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/urls.py
+-rw-r--r--   0        0        0     2695 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/pyproject.toml
+-rw-r--r--   0        0        0     6195 1970-01-01 00:00:00.000000 django_ninja_extra-0.20.6/PKG-INFO
```

### Comparing `django_ninja_extra-0.20.5/README.md` & `django_ninja_extra-0.20.6/README.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/__init__.py` & `django_ninja_extra-0.20.6/ninja_extra/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)"""
 
-__version__ = "0.20.5"
+__version__ = "0.20.6"
 
 import django
 
 from ninja_extra.controllers import (
     ControllerBase,
     ModelAsyncEndpointFactory,
     ModelConfig,
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/apps.py` & `django_ninja_extra-0.20.6/ninja_extra/apps.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/conf/settings.py` & `django_ninja_extra-0.20.6/ninja_extra/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/constants.py` & `django_ninja_extra-0.20.6/ninja_extra/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 HEAD = "HEAD"
 OPTIONS = "OPTIONS"
 TRACE = "TRACE"
 ROUTE_METHODS = [POST, PUT, PATCH, DELETE, GET, HEAD, OPTIONS, TRACE]
 THROTTLED_FUNCTION = "__throttled_endpoint__"
 ROUTE_FUNCTION = "__route_function__"
 
-ROUTE_CONTEXT_VAR: contextvars.ContextVar[
-    t.Optional["RouteContext"]
-] = contextvars.ContextVar("ROUTE_CONTEXT_VAR")
+ROUTE_CONTEXT_VAR: contextvars.ContextVar[t.Optional["RouteContext"]] = (
+    contextvars.ContextVar("ROUTE_CONTEXT_VAR")
+)
 ROUTE_CONTEXT_VAR.set(None)
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/__init__.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/base.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
+    TypeVar,
     Union,
     cast,
     overload,
 )
 
 from django.db.models import Model, QuerySet
 from django.http import HttpResponse
@@ -50,14 +51,16 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from ninja_extra import NinjaExtraAPI
     from ninja_extra.throttling import BaseThrottle
 
     from .route.context import RouteContext
 
+T = TypeVar("T")
+
 
 class MissingAPIControllerDecoratorException(Exception):
     pass
 
 
 def get_route_functions(cls: Type) -> Iterable[RouteFunction]:
     for method in cls.__dict__.values():
@@ -238,14 +241,20 @@
     ```
     """
 
     service: ModelService
     model_config: Optional[ModelConfig] = None
 
 
+ControllerClassType = TypeVar(
+    "ControllerClassType",
+    bound=Union[Type[ControllerBase], Type],
+)
+
+
 class APIController:
     _PATH_PARAMETER_COMPONENT_RE = r"{(?:(?P<converter>[^>:]+):)?(?P<parameter>[^>]+)}"
 
     """
     A class decorator
 
     Features
@@ -334,21 +343,21 @@
     @tags.setter
     def tags(self, value: Union[str, List[str], None]) -> None:
         tag: Optional[List[str]] = cast(Optional[List[str]], value)
         if tag and isinstance(value, str):
             tag = [value]
         self._tags = tag
 
-    def __call__(self, cls: Type) -> Type[ControllerBase]:
+    def __call__(self, cls: ControllerClassType) -> ControllerClassType:
         from ninja_extra.throttling import throttle
 
         self.auto_import = getattr(cls, "auto_import", self.auto_import)
         if not issubclass(cls, ControllerBase):
             # We force the cls to inherit from `ControllerBase` by creating another type.
-            cls = type(cls.__name__, (ControllerBase, cls), {"_api_controller": self})
+            cls = type(cls.__name__, (ControllerBase, cls), {"_api_controller": self})  # type:ignore[assignment]
         else:
             cls._api_controller = self
 
         assert isinstance(
             cls.throttling_classes, (list, tuple)
         ), f"Controller[{cls.__name__}].throttling_class must be a list or tuple"
         has_throttling_classes = len(cls.throttling_classes) > 0
@@ -383,15 +392,15 @@
                 )(v.route.view_func)
             self._add_operation_from_route_function(v)
 
         if not is_decorated_with_inject(cls.__init__):
             fail_silently(inject, constructor_or_class=cls)
 
         ControllerRegistry().add_controller(cls)
-        return cls
+        return cls  # type:ignore[return-value]
 
     @property
     def path_operations(self) -> Dict[str, PathView]:
         return self._path_operations
 
     def set_api_instance(self, api: "NinjaExtraAPI") -> None:
         self.controller_class.api = api
@@ -497,47 +506,47 @@
             openapi_extra=openapi_extra,
         )
         return operation
 
 
 @overload
 def api_controller(
-    prefix_or_class: Type,
-) -> Type[ControllerBase]:  # pragma: no cover
+    prefix_or_class: Type[T],
+) -> Union[Type[ControllerBase], Type[T]]:  # pragma: no cover
     ...
 
 
 @overload
 def api_controller(
     prefix_or_class: str = "",
     auth: Any = NOT_SET,
     tags: Union[Optional[List[str]], str] = None,
     permissions: Optional["PermissionType"] = None,
     auto_import: bool = True,
-) -> Callable[[Type], Type[ControllerBase]]:  # pragma: no cover
+) -> Callable[[Type[T]], Union[Type[ControllerBase], Type[T]]]:  # pragma: no cover
     ...
 
 
 def api_controller(
-    prefix_or_class: Union[str, Type] = "",
+    prefix_or_class: Union[str, ControllerClassType] = "",
     auth: Any = NOT_SET,
     tags: Union[Optional[List[str]], str] = None,
     permissions: Optional["PermissionType"] = None,
     auto_import: bool = True,
-) -> Union[Type[ControllerBase], Callable[[Type], Type[ControllerBase]]]:
+) -> Union[ControllerClassType, Callable[[ControllerClassType], ControllerClassType]]:
     if isinstance(prefix_or_class, type):
         return APIController(
             prefix="",
             auth=auth,
             tags=tags,
             permissions=permissions,
             auto_import=auto_import,
         )(prefix_or_class)
 
-    def _decorator(cls: Type) -> Type[ControllerBase]:
+    def _decorator(cls: ControllerClassType) -> ControllerClassType:
         return APIController(
             prefix=str(prefix_or_class),
             auth=auth,
             tags=tags,
             permissions=permissions,
             auto_import=auto_import,
         )(cls)
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/model/builder.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/model/builder.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/model/endpoints.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/model/endpoints.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/model/interfaces.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/model/interfaces.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/model/path_resolver.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/model/path_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/model/schemas.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/model/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     from ninja_schema.orm.model_schema import (
         ModelSchemaConfig as NinjaSchemaModelSchemaConfig,
     )
     from ninja_schema.orm.model_schema import (
         ModelSchemaConfigAdapter,
     )
 except Exception:  # pragma: no cover
-    ConfigError = (
-        NinjaSchemaModelSchemaConfig
-    ) = ModelSchemaConfigAdapter = SchemaFactory = None
+    ConfigError = NinjaSchemaModelSchemaConfig = ModelSchemaConfigAdapter = (
+        SchemaFactory
+    ) = None
 
 
 from ...pagination import PageNumberPaginationExtra, PaginatedResponseSchema
 
 
 class ModelPagination(PydanticModel):
     """
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/model/service.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/model/service.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/registry.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/registry.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/response.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/route/__init__.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/route/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/route/context.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/route/context.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/controllers/route/route_functions.py` & `django_ninja_extra-0.20.6/ninja_extra/controllers/route/route_functions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/dependency_resolver.py` & `django_ninja_extra-0.20.6/ninja_extra/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/details.py` & `django_ninja_extra-0.20.6/ninja_extra/details.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/exceptions.py` & `django_ninja_extra-0.20.6/ninja_extra/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 DRF Exceptions
 """
+
 import math
 from typing import Any, Dict, List, Optional, Type, Union, no_type_check
 
 from django.http import HttpRequest, HttpResponse, JsonResponse
 from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import ngettext
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/generic.py` & `django_ninja_extra-0.20.6/ninja_extra/generic.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/helper.py` & `django_ninja_extra-0.20.6/ninja_extra/helper.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/lazy.py` & `django_ninja_extra-0.20.6/ninja_extra/lazy.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/main.py` & `django_ninja_extra-0.20.6/ninja_extra/main.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/modules.py` & `django_ninja_extra-0.20.6/ninja_extra/modules.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/operation.py` & `django_ninja_extra-0.20.6/ninja_extra/operation.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/ordering.py` & `django_ninja_extra-0.20.6/ninja_extra/ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,25 @@
     "ordering",
     "OrderatorOperation",
     "AsyncOrderatorOperation",
 ]
 
 
 class OrderingBase(ABC):
-    class Input(Schema):
-        ...
+    class Input(Schema): ...
 
     InputSource = Query(...)
 
     def __init__(self, *, pass_parameter: Optional[str] = None, **kwargs: Any) -> None:
         self.pass_parameter = pass_parameter
 
     @abstractmethod
     def ordering_queryset(
         self, items: Union[QuerySet, List], ordering_input: Any
-    ) -> Union[QuerySet, List]:
-        ...
+    ) -> Union[QuerySet, List]: ...
 
 
 class Ordering(OrderingBase):
     class Input(Schema):
         ordering: Optional[str] = Field(None)
 
     def __init__(
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/pagination.py` & `django_ninja_extra-0.20.6/ninja_extra/pagination.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/permissions/base.py` & `django_ninja_extra-0.20.6/ninja_extra/permissions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Copied from DRF
 Provides a set of pluggable permission policies.
 """
+
 from abc import ABC, ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, Any, Generic, Tuple, Type, TypeVar, Union
 
 from django.http import HttpRequest
 from ninja.types import DictStrAny
 
 if TYPE_CHECKING:  # pragma: no cover
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/permissions/common.py` & `django_ninja_extra-0.20.6/ninja_extra/permissions/common.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/router.py` & `django_ninja_extra-0.20.6/ninja_extra/router.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/schemas/response.py` & `django_ninja_extra-0.20.6/ninja_extra/schemas/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/searching.py` & `django_ninja_extra-0.20.6/ninja_extra/searching.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,27 +52,25 @@
 
 
 def _isicontains(a: str, b: str) -> bool:
     return b.lower() in a.lower()
 
 
 class SearchingBase(ABC):
-    class Input(Schema):
-        ...
+    class Input(Schema): ...
 
     InputSource = Query(...)
 
     def __init__(self, *, pass_parameter: Optional[str] = None, **kwargs: Any) -> None:
         self.pass_parameter = pass_parameter
 
     @abstractmethod
     def searching_queryset(
         self, items: Union[QuerySet, List], searching_input: Any
-    ) -> Union[QuerySet, List]:
-        ...
+    ) -> Union[QuerySet, List]: ...
 
 
 class Searching(SearchingBase):
     class Input(Schema):
         search: Optional[str] = Field(None)
 
     lookup_prefixes = {
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/security/__init__.py` & `django_ninja_extra-0.20.6/ninja_extra/security/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/security/api_key.py` & `django_ninja_extra-0.20.6/ninja_extra/security/api_key.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/security/http.py` & `django_ninja_extra-0.20.6/ninja_extra/security/http.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/security/session.py` & `django_ninja_extra-0.20.6/ninja_extra/security/session.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/shortcuts.py` & `django_ninja_extra-0.20.6/ninja_extra/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/status.py` & `django_ninja_extra-0.20.6/ninja_extra/status.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/testing/client.py` & `django_ninja_extra-0.20.6/ninja_extra/testing/client.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/throttling/decorator.py` & `django_ninja_extra-0.20.6/ninja_extra/throttling/decorator.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/ninja_extra/throttling/model.py` & `django_ninja_extra-0.20.6/ninja_extra/throttling/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Provides various throttling policies.
 From DjangoRestFramework - https://github.com/encode/django-rest-framework/blob/master/rest_framework/throttling.py
 """
+
 import time
 from typing import Any, Callable, Dict, List, Optional, Tuple, cast
 
 from django.core.cache import cache as default_cache
 from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpRequest
```

### Comparing `django_ninja_extra-0.20.5/ninja_extra/urls.py` & `django_ninja_extra-0.20.6/ninja_extra/urls.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/pyproject.toml` & `django_ninja_extra-0.20.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.5/PKG-INFO` & `django_ninja_extra-0.20.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-extra
-Version: 0.20.5
+Version: 0.20.6
 Summary: Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)
 Home-page: https://github.com/eadwinCode/django-ninja-extra
 Author: Ezeudoh Tochukwu
 Author-email: tochukwu.ezeudoh@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

