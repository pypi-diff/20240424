# Comparing `tmp/aecdata-0.0.2.tar.gz` & `tmp/aecdata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aecdata-0.0.2.tar", last modified: Fri Apr 19 12:57:45 2024, max compression
+gzip compressed data, was "aecdata-0.0.3.tar", last modified: Wed Apr 24 13:48:10 2024, max compression
```

## Comparing `aecdata-0.0.2.tar` & `aecdata-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.620832 aecdata-0.0.2/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.2/LICENSE
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16101 2024-04-19 12:57:45.620582 aecdata-0.0.2/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    15498 2024-04-17 08:11:11.000000 aecdata-0.0.2/README.md
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.619196 aecdata-0.0.2/aecdata/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.2/aecdata/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2402 2024-04-03 12:58:03.000000 aecdata-0.0.2/aecdata/auth.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9211 2024-04-05 12:23:40.000000 aecdata-0.0.2/aecdata/client.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    40812 2024-04-19 09:03:16.000000 aecdata-0.0.2/aecdata/productdata.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20904 2024-04-12 08:29:30.000000 aecdata-0.0.2/aecdata/utils.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.620348 aecdata-0.0.2/aecdata.egg-info/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16101 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/SOURCES.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/dependency_links.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       41 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/requires.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/top_level.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-04-19 12:57:45.620883 aecdata-0.0.2/setup.cfg
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      771 2024-04-19 12:57:11.000000 aecdata-0.0.2/setup.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.620199 aecdata-0.0.2/tests/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.2/tests/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.2/tests/test_client.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.149800 aecdata-0.0.3/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.3/LICENSE
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16348 2024-04-24 13:48:10.149489 aecdata-0.0.3/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    15745 2024-04-22 09:51:42.000000 aecdata-0.0.3/README.md
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.147967 aecdata-0.0.3/aecdata/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.3/aecdata/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2402 2024-04-03 12:58:03.000000 aecdata-0.0.3/aecdata/auth.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9211 2024-04-05 12:23:40.000000 aecdata-0.0.3/aecdata/client.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    40613 2024-04-24 13:34:47.000000 aecdata-0.0.3/aecdata/productdata.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20904 2024-04-12 08:29:30.000000 aecdata-0.0.3/aecdata/utils.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.149125 aecdata-0.0.3/aecdata.egg-info/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16348 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/SOURCES.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/dependency_links.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       41 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/requires.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/top_level.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-04-24 13:48:10.149846 aecdata-0.0.3/setup.cfg
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      771 2024-04-24 13:46:29.000000 aecdata-0.0.3/setup.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.148975 aecdata-0.0.3/tests/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.3/tests/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.3/tests/test_client.py
```

### Comparing `aecdata-0.0.2/LICENSE` & `aecdata-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.2/PKG-INFO` & `aecdata-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,28 +15,28 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 
 # AECData
 
-AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
+AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API (see documentation [here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api)). By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
 - **Flexible Data Retrieval**: Supports fetching data using customizable filters to meet diverse analysis needs.
 - **Data Manipulation and Analysis**: Offers tools for transforming, scaling, and statistically analyzing the data.
 - **Visualization Support**: Provides functionalities for visualizing data distributions and product contributions.
 
 ## Introduction and Outline
 
 The library is structured to guide the user through a seamless process from authentication to data analysis:
 
-1. **Initialization**: Start by creating a `User` instance with your developer token. This instance will manage your authentication and serve as your gateway to fetching data.
+1. **Initialization**: Start by creating a `User` instance with your developer token ([see how to get a token here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api#get-a-developer-token)). This instance will manage your authentication and serve as your gateway to fetching data.
    
 2. **Fetching Data**: Utilize the `User` class to retrieve data from the API. You can apply various filters to narrow down the data according to your needs.
    
 3. **Data Manipulation**: Once you have fetched the data, you can construct a `ProductData` object. This object allows for extensive manipulation and transformation of the data, enabling you to prepare it for analysis or visualization in a format that suits your requirements.
    
 4. **Statistical Analysis and Visualization**: For advanced data analysis, the `ProductStatistics` class extends `ProductData` to provide statistical insights. It enables outlier removal, distribution analysis, and more, coupled with visualization capabilities to help interpret the data effectively.
```

### Comparing `aecdata-0.0.2/README.md` & `aecdata-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # AECData
 
-AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
+AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API (see documentation [here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api)). By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
 - **Flexible Data Retrieval**: Supports fetching data using customizable filters to meet diverse analysis needs.
 - **Data Manipulation and Analysis**: Offers tools for transforming, scaling, and statistically analyzing the data.
 - **Visualization Support**: Provides functionalities for visualizing data distributions and product contributions.
 
 ## Introduction and Outline
 
 The library is structured to guide the user through a seamless process from authentication to data analysis:
 
-1. **Initialization**: Start by creating a `User` instance with your developer token. This instance will manage your authentication and serve as your gateway to fetching data.
+1. **Initialization**: Start by creating a `User` instance with your developer token ([see how to get a token here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api#get-a-developer-token)). This instance will manage your authentication and serve as your gateway to fetching data.
    
 2. **Fetching Data**: Utilize the `User` class to retrieve data from the API. You can apply various filters to narrow down the data according to your needs.
    
 3. **Data Manipulation**: Once you have fetched the data, you can construct a `ProductData` object. This object allows for extensive manipulation and transformation of the data, enabling you to prepare it for analysis or visualization in a format that suits your requirements.
    
 4. **Statistical Analysis and Visualization**: For advanced data analysis, the `ProductStatistics` class extends `ProductData` to provide statistical insights. It enables outlier removal, distribution analysis, and more, coupled with visualization capabilities to help interpret the data effectively.
```

### Comparing `aecdata-0.0.2/aecdata/auth.py` & `aecdata-0.0.3/aecdata/auth.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.2/aecdata/client.py` & `aecdata-0.0.3/aecdata/client.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.2/aecdata/productdata.py` & `aecdata-0.0.3/aecdata/productdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,27 @@
     @property
     def data(self):
         return self._data
 
     @data.setter
     def data(self, value):
         def add_scaling_factor(product):
-            # Check if 'material_facts' is a key in the product dictionary
+            # Ensure 'material_facts' exists and proceed if it does
             if 'material_facts' in product:
-                # Check if 'scaling_factor' is not a key in the 'material_facts' dictionary
-                if 'scaling_factor' not in product['material_facts']:
+                # Initialize 'material_facts' if not already present
+                if 'scaling_factors' not in product['material_facts']:
                     declared_unit = product['material_facts'].get('declared_unit', None)
                     if declared_unit:
                         product['material_facts']['scaling_factors'] = {
                             declared_unit: {'value': 1, 'estimated': False}
                         }
-            # In case 'material_facts' key is missing, do nothing (no error)
             return product
-        if 'scaling_factor' not in value:
-            products = []
-            for product in value:
-                products.append(add_scaling_factor(product))
-        else:
-            products = value.copy()
+
+        # Process each product to potentially add missing scaling factors
+        products = [add_scaling_factor(product) for product in value]
 
         self._data = products
         self._dataframe = self.to_dataframe(products).replace({np.nan: None})
 
     @property
     def dataframe(self):
         return self._dataframe
@@ -848,15 +844,15 @@
         else:
             df = self.dataframe
 
         if not include_estimated_values:
             df = df[df['estimated'] == False]
 
         if field not in self.get_available_fields():
-            raise ValueError(f"{field} is not available.")
+            return pd.DataFrame()
 
         df = df.dropna(subset=[field])
 
         if remove_outliers:
             df = self.remove_outliers_from_df(df, field, method, sqrt_tranf)
 
         return df.reset_index(drop=True)
```

### Comparing `aecdata-0.0.2/aecdata/utils.py` & `aecdata-0.0.3/aecdata/utils.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.2/aecdata.egg-info/PKG-INFO` & `aecdata-0.0.3/aecdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,28 +15,28 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 
 # AECData
 
-AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
+AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API (see documentation [here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api)). By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
 - **Flexible Data Retrieval**: Supports fetching data using customizable filters to meet diverse analysis needs.
 - **Data Manipulation and Analysis**: Offers tools for transforming, scaling, and statistically analyzing the data.
 - **Visualization Support**: Provides functionalities for visualizing data distributions and product contributions.
 
 ## Introduction and Outline
 
 The library is structured to guide the user through a seamless process from authentication to data analysis:
 
-1. **Initialization**: Start by creating a `User` instance with your developer token. This instance will manage your authentication and serve as your gateway to fetching data.
+1. **Initialization**: Start by creating a `User` instance with your developer token ([see how to get a token here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api#get-a-developer-token)). This instance will manage your authentication and serve as your gateway to fetching data.
    
 2. **Fetching Data**: Utilize the `User` class to retrieve data from the API. You can apply various filters to narrow down the data according to your needs.
    
 3. **Data Manipulation**: Once you have fetched the data, you can construct a `ProductData` object. This object allows for extensive manipulation and transformation of the data, enabling you to prepare it for analysis or visualization in a format that suits your requirements.
    
 4. **Statistical Analysis and Visualization**: For advanced data analysis, the `ProductStatistics` class extends `ProductData` to provide statistical insights. It enables outlier removal, distribution analysis, and more, coupled with visualization capabilities to help interpret the data effectively.
```

### Comparing `aecdata-0.0.2/setup.py` & `aecdata-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aecdata",
-    version="0.0.2",
+    version="0.0.3",
     author="2050 Materials",
     license="Apache License 2.0",
     author_email="nicodemos@2050-materials.com",
     description="A Python library designed to simplify access to the 2050-materials API",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/2050-Materials/aecdata",
```

