# Comparing `tmp/pydeck-carto-0.1.0b9.tar.gz` & `tmp/pydeck-carto-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeck-carto-0.1.0b9.tar", last modified: Thu Nov  3 16:37:46 2022, max compression
+gzip compressed data, was "pydeck-carto-0.1.1b0.tar", last modified: Wed Apr 24 16:22:34 2024, max compression
```

## Comparing `pydeck-carto-0.1.0b9.tar` & `pydeck-carto-0.1.1b0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2022-11-03 16:37:46.659649 pydeck-carto-0.1.0b9/
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     3350 2022-11-03 16:37:46.659649 pydeck-carto-0.1.0b9/PKG-INFO
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     1950 2022-11-03 16:33:25.000000 pydeck-carto-0.1.0b9/README.md
-drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2022-11-03 16:37:46.659649 pydeck-carto-0.1.0b9/pydeck_carto/
--rw-rw-r--   0 jesus     (1000) jesus     (1000)      348 2022-11-03 16:13:36.000000 pydeck-carto-0.1.0b9/pydeck_carto/__init__.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       24 2022-11-03 16:08:43.000000 pydeck-carto-0.1.0b9/pydeck_carto/_version.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     2705 2022-11-03 16:12:33.000000 pydeck-carto-0.1.0b9/pydeck_carto/layer.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     3286 2022-11-03 14:14:11.000000 pydeck-carto-0.1.0b9/pydeck_carto/styles.py
-drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2022-11-03 16:37:46.659649 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     3350 2022-11-03 16:37:46.000000 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/PKG-INFO
--rw-rw-r--   0 jesus     (1000) jesus     (1000)      337 2022-11-03 16:37:46.000000 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/SOURCES.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)        1 2022-11-03 16:37:46.000000 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/dependency_links.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)        1 2022-11-03 16:37:46.000000 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/not-zip-safe
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       36 2022-11-03 16:37:46.000000 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/requires.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       13 2022-11-03 16:37:46.000000 pydeck-carto-0.1.0b9/pydeck_carto.egg-info/top_level.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       69 2022-11-03 16:37:46.659649 pydeck-carto-0.1.0b9/setup.cfg
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     1311 2022-11-03 13:17:28.000000 pydeck-carto-0.1.0b9/setup.py
+drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-04-24 16:22:34.462788 pydeck-carto-0.1.1b0/
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     1512 2023-11-13 16:22:18.000000 pydeck-carto-0.1.1b0/LICENSE
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     2810 2024-04-24 16:22:34.462883 pydeck-carto-0.1.1b0/PKG-INFO
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     1950 2024-04-22 21:08:37.000000 pydeck-carto-0.1.1b0/README.md
+drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-04-24 16:22:34.461867 pydeck-carto-0.1.1b0/pydeck_carto/
+-rw-r--r--   0 donmccurdy   (501) staff       (20)      348 2024-04-22 21:08:37.000000 pydeck-carto-0.1.1b0/pydeck_carto/__init__.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       24 2024-04-24 16:12:13.000000 pydeck-carto-0.1.1b0/pydeck_carto/_version.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     2742 2024-04-24 13:44:31.000000 pydeck-carto-0.1.1b0/pydeck_carto/layer.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     3286 2023-11-13 16:22:18.000000 pydeck-carto-0.1.1b0/pydeck_carto/styles.py
+drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-04-24 16:22:34.462684 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     2810 2024-04-24 16:22:34.000000 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/PKG-INFO
+-rw-r--r--   0 donmccurdy   (501) staff       (20)      345 2024-04-24 16:22:34.000000 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/SOURCES.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)        1 2024-04-24 16:22:34.000000 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/dependency_links.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)        1 2024-04-24 16:22:34.000000 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/not-zip-safe
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       32 2024-04-24 16:22:34.000000 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/requires.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       13 2024-04-24 16:22:34.000000 pydeck-carto-0.1.1b0/pydeck_carto.egg-info/top_level.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       69 2024-04-24 16:22:34.463106 pydeck-carto-0.1.1b0/setup.cfg
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     1320 2024-04-24 13:44:31.000000 pydeck-carto-0.1.1b0/setup.py
```

### Comparing `pydeck-carto-0.1.0b9/PKG-INFO` & `pydeck-carto-0.1.1b0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 Metadata-Version: 2.1
 Name: pydeck-carto
-Version: 0.1.0b9
+Version: 0.1.1b0
 Summary: Pydeck wrapper for use with CARTO
 Home-page: https://github.com/visgl/deck.gl/tree/master/bindings/pydeck-carto
 Author: CARTO
 Author-email: jarroyo@carto.com
 License: BSD 3-Clause
-Description: # pydeck-carto
-        
-        [![PyPI version](https://badge.fury.io/py/pydeck-carto.svg)](https://badge.fury.io/py/pydeck-carto)
-        [![Documentation Status](https://readthedocs.org/projects/pydeck-carto/badge/?version=latest)](https://pydeck-carto.readthedocs.io)
-        
-        [Pydeck](https://pydeck.gl/) wrapper for use with [CARTO](carto.com).
-        
-        ## Install
-        
-        ```bash
-        pip install pydeck-carto
-        ```
-        
-        This also ensures [pydeck](https://pydeck.gl/) is installed. If you haven't previously enabled pydeck to be used with Jupyter, follow [its instructions](https://pydeck.gl/installation.html) to install.
-        
-        ### Installing from source
-        
-        ```bash
-        git clone https://github.com/visgl/deck.gl
-        cd deck.gl/bindings/pydeck-carto
-        pip install .
-        ```
-        
-        ## Usage
-        
-        ```py
-        import pydeck as pdk
-        import pydeck_carto as pdkc
-        from carto_auth import CartoAuth
-        
-        # Authentication with CARTO
-        carto_auth = CartoAuth.from_oauth()
-        
-        # Register CartoLayer in pydeck
-        pdkc.register_carto_layer()
-        
-        # Render CartoLayer in pydeck
-        layer = pdk.Layer(
-            "CartoLayer",
-            data="SELECT geom, name FROM carto-demo-data.demo_tables.airports",
-            type_=pdkc.MapType.QUERY,
-            connection=pdkc.CartoConnection.CARTO_DW,
-            credentials=pdkc.get_layer_credentials(carto_auth),
-            get_fill_color=[238, 77, 90],
-            point_radius_min_pixels=2.5,
-            pickable=True,
-        )
-        view_state = pdk.ViewState(latitude=0, longitude=0, zoom=1)
-        pdk.Deck(layer, map_style=pdk.map_styles.ROAD, initial_view_state=view_state)
-        ```
-        
-        For more information, check the [examples](./examples) section and the [documentation](https://pydeck-carto.readthedocs.io).
-        
-        ## Development
-        
-        Make commands:
-        
-        - init: create the environment and install dependencies
-        - lint: run linter (black + flake8)
-        - test: run tests (pytest)
-        - publish-pypi: publish package in pypi.org
-        - publish-test-pypi: publish package in test.pypi.org
-        - clean: remove the environment
-        
-        ## Contributors
-        
-        - [Jesús Arroyo](https://github.com/jesus89)
-        - [Óscar Ramírez](https://github.com/tuxskar)
-        
 Keywords: pydeck,carto,visualization,graphics,GIS,maps
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pydeck-carto
+
+[![PyPI version](https://badge.fury.io/py/pydeck-carto.svg)](https://badge.fury.io/py/pydeck-carto)
+[![Documentation Status](https://readthedocs.org/projects/pydeck-carto/badge/?version=latest)](https://pydeck-carto.readthedocs.io)
+
+[Pydeck](https://pydeck.gl/) wrapper for use with [CARTO](carto.com).
+
+## Install
+
+```bash
+pip install pydeck-carto
+```
+
+This also ensures [pydeck](https://pydeck.gl/) is installed. If you haven't previously enabled pydeck to be used with Jupyter, follow [its instructions](https://pydeck.gl/installation.html) to install.
+
+### Installing from source
+
+```bash
+git clone https://github.com/visgl/deck.gl
+cd deck.gl/bindings/pydeck-carto
+pip install .
+```
+
+## Usage
+
+```py
+import pydeck as pdk
+import pydeck_carto as pdkc
+from carto_auth import CartoAuth
+
+# Authentication with CARTO
+carto_auth = CartoAuth.from_oauth()
+
+# Register CartoLayer in pydeck
+pdkc.register_carto_layer()
+
+# Render CartoLayer in pydeck
+layer = pdk.Layer(
+    "CartoLayer",
+    data="SELECT geom, name FROM carto-demo-data.demo_tables.airports",
+    type_=pdkc.MapType.QUERY,
+    connection=pdkc.CartoConnection.CARTO_DW,
+    credentials=pdkc.get_layer_credentials(carto_auth),
+    get_fill_color=[238, 77, 90],
+    point_radius_min_pixels=2.5,
+    pickable=True,
+)
+view_state = pdk.ViewState(latitude=0, longitude=0, zoom=1)
+pdk.Deck(layer, map_style=pdk.map_styles.ROAD, initial_view_state=view_state)
+```
+
+For more information, check the [examples](./examples) section and the [documentation](https://pydeck-carto.readthedocs.io).
+
+## Development
+
+Make commands:
+
+- init: create the environment and install dependencies
+- lint: run linter (black + flake8)
+- test: run tests (pytest)
+- publish-pypi: publish package in pypi.org
+- publish-test-pypi: publish package in test.pypi.org
+- clean: remove the environment
+
+## Contributors
+
+- [Jesús Arroyo](https://github.com/jesus89)
+- [Óscar Ramírez](https://github.com/tuxskar)
```

### Comparing `pydeck-carto-0.1.0b9/README.md` & `pydeck-carto-0.1.1b0/README.md`

 * *Files identical despite different names*

### Comparing `pydeck-carto-0.1.0b9/pydeck_carto/layer.py` & `pydeck-carto-0.1.1b0/pydeck_carto/layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pydeck as pdk
 
 H3_VERSION = "~3.7.*"
-DECKGL_VERSION = "~8.8.*"
+DECKGL_VERSION = "~8.9.*"
 
 LIBRARIES_TO_INCLUDE = [
     f"npm/h3-js@{H3_VERSION}/dist/h3-js.umd.js",
     f"npm/@deck.gl/extensions@{DECKGL_VERSION}/dist.min.js",
     f"npm/@deck.gl/carto@{DECKGL_VERSION}/dist.min.js",
 ]
 SELECTED_LIBRARIES = ",".join(LIBRARIES_TO_INCLUDE)
@@ -78,13 +78,14 @@
 def get_layer_credentials(carto_auth) -> dict:
     """Get the layer credentials object to gather information
     from carto warehouses.
 
     The return object has the following structure:
     ``{"apiVersion": "v3", "apiBaseUrl": "...", "accessToken": "...",}``
     """
+    api_base_url = carto_auth.get_api_base_url()
     access_token = carto_auth.get_access_token()
     return {
         "apiVersion": "v3",
-        "apiBaseUrl": carto_auth._api_base_url,
+        "apiBaseUrl": api_base_url,
         "accessToken": access_token,
     }
```

### Comparing `pydeck-carto-0.1.0b9/pydeck_carto/styles.py` & `pydeck-carto-0.1.1b0/pydeck_carto/styles.py`

 * *Files identical despite different names*

### Comparing `pydeck-carto-0.1.0b9/pydeck_carto.egg-info/PKG-INFO` & `pydeck-carto-0.1.1b0/pydeck_carto.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 Metadata-Version: 2.1
 Name: pydeck-carto
-Version: 0.1.0b9
+Version: 0.1.1b0
 Summary: Pydeck wrapper for use with CARTO
 Home-page: https://github.com/visgl/deck.gl/tree/master/bindings/pydeck-carto
 Author: CARTO
 Author-email: jarroyo@carto.com
 License: BSD 3-Clause
-Description: # pydeck-carto
-        
-        [![PyPI version](https://badge.fury.io/py/pydeck-carto.svg)](https://badge.fury.io/py/pydeck-carto)
-        [![Documentation Status](https://readthedocs.org/projects/pydeck-carto/badge/?version=latest)](https://pydeck-carto.readthedocs.io)
-        
-        [Pydeck](https://pydeck.gl/) wrapper for use with [CARTO](carto.com).
-        
-        ## Install
-        
-        ```bash
-        pip install pydeck-carto
-        ```
-        
-        This also ensures [pydeck](https://pydeck.gl/) is installed. If you haven't previously enabled pydeck to be used with Jupyter, follow [its instructions](https://pydeck.gl/installation.html) to install.
-        
-        ### Installing from source
-        
-        ```bash
-        git clone https://github.com/visgl/deck.gl
-        cd deck.gl/bindings/pydeck-carto
-        pip install .
-        ```
-        
-        ## Usage
-        
-        ```py
-        import pydeck as pdk
-        import pydeck_carto as pdkc
-        from carto_auth import CartoAuth
-        
-        # Authentication with CARTO
-        carto_auth = CartoAuth.from_oauth()
-        
-        # Register CartoLayer in pydeck
-        pdkc.register_carto_layer()
-        
-        # Render CartoLayer in pydeck
-        layer = pdk.Layer(
-            "CartoLayer",
-            data="SELECT geom, name FROM carto-demo-data.demo_tables.airports",
-            type_=pdkc.MapType.QUERY,
-            connection=pdkc.CartoConnection.CARTO_DW,
-            credentials=pdkc.get_layer_credentials(carto_auth),
-            get_fill_color=[238, 77, 90],
-            point_radius_min_pixels=2.5,
-            pickable=True,
-        )
-        view_state = pdk.ViewState(latitude=0, longitude=0, zoom=1)
-        pdk.Deck(layer, map_style=pdk.map_styles.ROAD, initial_view_state=view_state)
-        ```
-        
-        For more information, check the [examples](./examples) section and the [documentation](https://pydeck-carto.readthedocs.io).
-        
-        ## Development
-        
-        Make commands:
-        
-        - init: create the environment and install dependencies
-        - lint: run linter (black + flake8)
-        - test: run tests (pytest)
-        - publish-pypi: publish package in pypi.org
-        - publish-test-pypi: publish package in test.pypi.org
-        - clean: remove the environment
-        
-        ## Contributors
-        
-        - [Jesús Arroyo](https://github.com/jesus89)
-        - [Óscar Ramírez](https://github.com/tuxskar)
-        
 Keywords: pydeck,carto,visualization,graphics,GIS,maps
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pydeck-carto
+
+[![PyPI version](https://badge.fury.io/py/pydeck-carto.svg)](https://badge.fury.io/py/pydeck-carto)
+[![Documentation Status](https://readthedocs.org/projects/pydeck-carto/badge/?version=latest)](https://pydeck-carto.readthedocs.io)
+
+[Pydeck](https://pydeck.gl/) wrapper for use with [CARTO](carto.com).
+
+## Install
+
+```bash
+pip install pydeck-carto
+```
+
+This also ensures [pydeck](https://pydeck.gl/) is installed. If you haven't previously enabled pydeck to be used with Jupyter, follow [its instructions](https://pydeck.gl/installation.html) to install.
+
+### Installing from source
+
+```bash
+git clone https://github.com/visgl/deck.gl
+cd deck.gl/bindings/pydeck-carto
+pip install .
+```
+
+## Usage
+
+```py
+import pydeck as pdk
+import pydeck_carto as pdkc
+from carto_auth import CartoAuth
+
+# Authentication with CARTO
+carto_auth = CartoAuth.from_oauth()
+
+# Register CartoLayer in pydeck
+pdkc.register_carto_layer()
+
+# Render CartoLayer in pydeck
+layer = pdk.Layer(
+    "CartoLayer",
+    data="SELECT geom, name FROM carto-demo-data.demo_tables.airports",
+    type_=pdkc.MapType.QUERY,
+    connection=pdkc.CartoConnection.CARTO_DW,
+    credentials=pdkc.get_layer_credentials(carto_auth),
+    get_fill_color=[238, 77, 90],
+    point_radius_min_pixels=2.5,
+    pickable=True,
+)
+view_state = pdk.ViewState(latitude=0, longitude=0, zoom=1)
+pdk.Deck(layer, map_style=pdk.map_styles.ROAD, initial_view_state=view_state)
+```
+
+For more information, check the [examples](./examples) section and the [documentation](https://pydeck-carto.readthedocs.io).
+
+## Development
+
+Make commands:
+
+- init: create the environment and install dependencies
+- lint: run linter (black + flake8)
+- test: run tests (pytest)
+- publish-pypi: publish package in pypi.org
+- publish-test-pypi: publish package in test.pypi.org
+- clean: remove the environment
+
+## Contributors
+
+- [Jesús Arroyo](https://github.com/jesus89)
+- [Óscar Ramírez](https://github.com/tuxskar)
```

### Comparing `pydeck-carto-0.1.0b9/setup.py` & `pydeck-carto-0.1.1b0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     author="CARTO",
     author_email="jarroyo@carto.com",
     url="https://github.com/visgl/deck.gl/tree/master/bindings/pydeck-carto",
     license="BSD 3-Clause",
     packages=find_packages(exclude=["examples", "tests"]),
     python_requires=">=3.7",
     install_requires=[
-        "pydeck>=0.8.0b4",
-        "carto-auth>=0.1.0b5",
+        "pydeck>=0.8.0",
+        "carto-auth>=0.1.0",
     ],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Jupyter",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

