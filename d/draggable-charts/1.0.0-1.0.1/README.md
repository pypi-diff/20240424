# Comparing `tmp/draggable-charts-1.0.0.tar.gz` & `tmp/draggable-charts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-charts-1.0.0.tar", last modified: Tue Apr 23 23:41:26 2024, max compression
+gzip compressed data, was "draggable-charts-1.0.1.tar", last modified: Wed Apr 24 01:22:29 2024, max compression
```

## Comparing `draggable-charts-1.0.0.tar` & `draggable-charts-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.829672 draggable-charts-1.0.0/
--rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-charts-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6119 2024-04-23 23:41:26.825936 draggable-charts-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5617 2024-04-23 23:36:04.000000 draggable-charts-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.653994 draggable-charts-1.0.0/draggable_charts/
--rw-rw-rw-   0        0        0       41 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/__init__.py
--rw-rw-rw-   0        0        0     2680 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/example.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.602130 draggable-charts-1.0.0/draggable_charts/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.720814 draggable-charts-1.0.0/draggable_charts/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-23 23:24:32.000000 draggable-charts-1.0.0/draggable_charts/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-23 23:24:32.000000 draggable-charts-1.0.0/draggable_charts/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.604155 draggable-charts-1.0.0/draggable_charts/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.751443 draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/
--rw-rw-rw-   0        0        0   591514 2024-04-23 23:24:32.000000 draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js
--rw-rw-rw-   0        0        0     1831 2024-04-23 23:24:32.000000 draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2534740 2024-04-23 23:24:32.000000 draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.map
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.780906 draggable-charts-1.0.0/draggable_charts/utils/
--rw-rw-rw-   0        0        0      117 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/utils/__init__.py
--rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/utils/component_func.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.816521 draggable-charts-1.0.0/draggable_charts/widgets/
--rw-rw-rw-   0        0        0      113 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/widgets/__init__.py
--rw-rw-rw-   0        0        0     3887 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/widgets/bezierchart.py
--rw-rw-rw-   0        0        0     4332 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/widgets/linechart.py
--rw-rw-rw-   0        0        0     2310 2024-04-23 23:20:49.000000 draggable-charts-1.0.0/draggable_charts/widgets/scatterchart.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:26.692976 draggable-charts-1.0.0/draggable_charts.egg-info/
--rw-rw-rw-   0        0        0     6119 2024-04-23 23:41:26.000000 draggable-charts-1.0.0/draggable_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2024-04-23 23:41:26.000000 draggable-charts-1.0.0/draggable_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 23:41:26.000000 draggable-charts-1.0.0/draggable_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-23 23:41:26.000000 draggable-charts-1.0.0/draggable_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-23 23:41:26.000000 draggable-charts-1.0.0/draggable_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 23:41:26.832082 draggable-charts-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1124 2024-04-23 23:41:15.000000 draggable-charts-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:29.142028 draggable-charts-1.0.1/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-charts-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6115 2024-04-24 01:22:29.136043 draggable-charts-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:28.899281 draggable-charts-1.0.1/draggable_charts/
+-rw-rw-rw-   0        0        0       41 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/draggable_charts/__init__.py
+-rw-rw-rw-   0        0        0     2680 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/draggable_charts/example.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:28.824992 draggable-charts-1.0.1/draggable_charts/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:28.985611 draggable-charts-1.0.1/draggable_charts/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-24 01:21:16.000000 draggable-charts-1.0.1/draggable_charts/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/draggable_charts/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-24 01:21:16.000000 draggable-charts-1.0.1/draggable_charts/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:28.828980 draggable-charts-1.0.1/draggable_charts/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:29.025289 draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   591514 2024-04-24 01:21:16.000000 draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js
+-rw-rw-rw-   0        0        0     1831 2024-04-24 01:21:16.000000 draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2534740 2024-04-24 01:21:16.000000 draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.map
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:29.067614 draggable-charts-1.0.1/draggable_charts/utils/
+-rw-rw-rw-   0        0        0      117 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/draggable_charts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/draggable_charts/utils/component_func.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:29.124076 draggable-charts-1.0.1/draggable_charts/widgets/
+-rw-rw-rw-   0        0        0      113 2024-04-23 23:20:49.000000 draggable-charts-1.0.1/draggable_charts/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3893 2024-04-24 01:15:58.000000 draggable-charts-1.0.1/draggable_charts/widgets/bezierchart.py
+-rw-rw-rw-   0        0        0     4334 2024-04-24 01:15:50.000000 draggable-charts-1.0.1/draggable_charts/widgets/linechart.py
+-rw-rw-rw-   0        0        0     2316 2024-04-24 01:16:47.000000 draggable-charts-1.0.1/draggable_charts/widgets/scatterchart.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:22:28.951653 draggable-charts-1.0.1/draggable_charts.egg-info/
+-rw-rw-rw-   0        0        0     6115 2024-04-24 01:22:28.000000 draggable-charts-1.0.1/draggable_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2024-04-24 01:22:28.000000 draggable-charts-1.0.1/draggable_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 01:22:28.000000 draggable-charts-1.0.1/draggable_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-24 01:22:28.000000 draggable-charts-1.0.1/draggable_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-24 01:22:28.000000 draggable-charts-1.0.1/draggable_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 01:22:29.144993 draggable-charts-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2024-04-24 01:17:24.000000 draggable-charts-1.0.1/setup.py
```

### Comparing `draggable-charts-1.0.0/LICENSE` & `draggable-charts-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/PKG-INFO` & `draggable-charts-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -13,15 +13,15 @@
 # draggable-charts
 
 Streamlit component that displays a interactive charts with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 
 ## Installation instructions
 
 ```sh
-pip install draggable-line-chart
+pip install draggable-charts
 ```
 
 
 ## Usage
 
 ## Line Chart:
```

### Comparing `draggable-charts-1.0.0/README.md` & `draggable-charts-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # draggable-charts
 
 Streamlit component that displays a interactive charts with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 
 ## Installation instructions
 
 ```sh
-pip install draggable-line-chart
+pip install draggable-charts
 ```
 
 
 ## Usage
 
 ## Line Chart:
```

### Comparing `draggable-charts-1.0.0/draggable_charts/example.py` & `draggable-charts-1.0.1/draggable_charts/example.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/draggable_charts/frontend/build/bootstrap.min.css` & `draggable-charts-1.0.1/draggable_charts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js` & `draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.LICENSE.txt` & `draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.map` & `draggable-charts-1.0.1/draggable_charts/frontend/build/static/js/main.f3ea7fdc.js.map`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/draggable_charts/utils/component_func.py` & `draggable-charts-1.0.1/draggable_charts/utils/component_func.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/draggable_charts/widgets/bezierchart.py` & `draggable-charts-1.0.1/draggable_charts/widgets/bezierchart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from utils import component, get_func_name
 from typing import Literal
+
 import numpy as np
 
+from ..utils import component, get_func_name
+
 DEFAULT_OPTIONS = {
     "x_grid": True,
     "y_grid": True,
     "tension": 0.3,
     "line": False,
 }
```

### Comparing `draggable-charts-1.0.0/draggable_charts/widgets/linechart.py` & `draggable-charts-1.0.1/draggable_charts/widgets/linechart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import Any, Dict, Union
 
 import numpy as np
 import pandas as pd
-from utils import component, get_func_name
+
+from ..utils import component, get_func_name
 
 DEFAULT_OPTIONS = {
     "x_grid": True,
     "y_grid": True,
     "tension": 0.3
 }
 
+
 def line_chart(
     data: Union[pd.DataFrame, pd.Series],
     options: Dict[str, Any] = {},
     key: str = None
 ) -> Union[pd.DataFrame, pd.Series]:
     """
     Displays a line chart with draggable points.
@@ -60,14 +62,15 @@
         kw={"data": dict_data, "options": options},
         default=data,
         key=key
     )
     new_df = postprocess_data(data, new_data)
     return new_df
 
+
 def validate_data(data):
     if isinstance(data, pd.Series):
         return
     elif isinstance(data, pd.DataFrame):
         non_numeric_columns = data.select_dtypes(exclude='number').columns
         if len(non_numeric_columns) > 0:
             raise ValueError(
@@ -75,25 +78,27 @@
                 "Expected a DataFrame with only numeric columns."
             )
     else:
         raise ValueError(
             f"Invalid data type: {type(data).__name__}. "
             "Expected a pandas Series or DataFrame."
         )
-        
+
+
 def transform_data(data) -> dict:
     if isinstance(data, pd.Series):
         if not data.name:
             data.name = "data"
         return {data.name: data.replace({np.nan: None}).to_dict()}
     elif isinstance(data, pd.DataFrame):
         return data.replace({np.nan: None}).to_dict()
-    
+
+
 def postprocess_data(data, new_data) -> pd.DataFrame:
     if isinstance(data, pd.Series) and isinstance(new_data, pd.Series):
         return pd.Series(new_data)
     elif isinstance(data, pd.Series):
         new_series = pd.Series(new_data[data.name])
         new_series.name = data.name
         return new_series
     elif isinstance(data, pd.DataFrame):
-        return pd.DataFrame(new_data)
+        return pd.DataFrame(new_data)
```

### Comparing `draggable-charts-1.0.0/draggable_charts/widgets/scatterchart.py` & `draggable-charts-1.0.1/draggable_charts/widgets/scatterchart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from utils import component, get_func_name
 from typing import Literal
+
 import numpy as np
 
+from ..utils import component, get_func_name
+
 DEFAULT_OPTIONS = {
     "x_grid": True,
     "y_grid": True,
     "tension": 0.3,
     "line": False,
 }
```

### Comparing `draggable-charts-1.0.0/draggable_charts.egg-info/PKG-INFO` & `draggable-charts-1.0.1/draggable_charts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -13,15 +13,15 @@
 # draggable-charts
 
 Streamlit component that displays a interactive charts with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 
 ## Installation instructions
 
 ```sh
-pip install draggable-line-chart
+pip install draggable-charts
 ```
 
 
 ## Usage
 
 ## Line Chart:
```

### Comparing `draggable-charts-1.0.0/draggable_charts.egg-info/SOURCES.txt` & `draggable-charts-1.0.1/draggable_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.0.0/setup.py` & `draggable-charts-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-charts",
-    version="1.0.0",
+    version="1.0.1",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/draggable-charts",
     packages=setuptools.find_packages(),
```

