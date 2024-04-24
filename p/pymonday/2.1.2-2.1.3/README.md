# Comparing `tmp/pymonday-2.1.2.tar.gz` & `tmp/pymonday-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonday-2.1.2.tar", last modified: Tue Apr 16 14:58:52 2024, max compression
+gzip compressed data, was "pymonday-2.1.3.tar", last modified: Wed Apr 24 11:16:56 2024, max compression
```

## Comparing `pymonday-2.1.2.tar` & `pymonday-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:52.128334 pymonday-2.1.2/
--rw-rw-rw-   0        0        0    35823 2024-02-26 11:34:44.000000 pymonday-2.1.2/LICENSE
--rw-rw-rw-   0        0        0      344 2024-04-16 14:58:52.127334 pymonday-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      112 2024-02-26 12:54:28.000000 pymonday-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:52.115832 pymonday-2.1.2/pymonday/
--rw-rw-rw-   0        0        0       56 2024-02-26 11:40:39.000000 pymonday-2.1.2/pymonday/__init__.py
--rw-rw-rw-   0        0        0     1259 2024-02-26 11:40:48.000000 pymonday-2.1.2/pymonday/columns.py
--rw-rw-rw-   0        0        0    48791 2024-04-16 14:54:25.000000 pymonday-2.1.2/pymonday/monday_api_client.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:52.125834 pymonday-2.1.2/pymonday.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 14:58:52.128834 pymonday-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      451 2024-04-16 14:56:38.000000 pymonday-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:16:56.983894 pymonday-2.1.3/
+-rw-rw-rw-   0        0        0    35823 2024-02-26 11:34:44.000000 pymonday-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0      344 2024-04-24 11:16:56.982394 pymonday-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2024-02-26 12:54:28.000000 pymonday-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 11:16:56.970392 pymonday-2.1.3/pymonday/
+-rw-rw-rw-   0        0        0       56 2024-02-26 11:40:39.000000 pymonday-2.1.3/pymonday/__init__.py
+-rw-rw-rw-   0        0        0     1259 2024-02-26 11:40:48.000000 pymonday-2.1.3/pymonday/columns.py
+-rw-rw-rw-   0        0        0    50323 2024-04-24 11:16:16.000000 pymonday-2.1.3/pymonday/monday_api_client.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:16:56.980894 pymonday-2.1.3/pymonday.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 11:16:56.983894 pymonday-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      451 2024-04-24 11:16:33.000000 pymonday-2.1.3/setup.py
```

### Comparing `pymonday-2.1.2/LICENSE` & `pymonday-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonday-2.1.2/pymonday/columns.py` & `pymonday-2.1.3/pymonday/columns.py`

 * *Files identical despite different names*

### Comparing `pymonday-2.1.2/pymonday/monday_api_client.py` & `pymonday-2.1.3/pymonday/monday_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -737,23 +737,51 @@
         column_string = column_string[:-2]
         column_string = f"[{column_string}]"
         item_attributes = f'''name id parent_item{{id name }} column_values(ids: {column_string}) {{text value
         column{{id title}}
         ... on BoardRelationValue {{display_value linked_items {{id}}}}
         ... on MirrorValue {{display_value}}}}'''
 
-        initial_query = f'''{{boards(ids: {board_id}) {{groups(ids: "{group_id}") {{items_page(limit: 100 
+        initial_query = f'''{{boards(ids: {board_id}) {{groups(ids: "{group_id}") {{items_page(limit: 8 
         query_params: {{rules: {{column_id: "{column_id}", compare_value: [{index_value}]}}}}) {{
         cursor
         items {{{item_attributes}}}}}}}}}}}'''
         data = {'query': initial_query}
         response = self.__send_post_request(data)
         if not response:
             return None
         items = [item for item in response['data']['boards'][0]['groups'][0]['items_page']['items']]
+        cursor = response['data']['boards'][0]['groups'][0]['items_page']['cursor']
+        if cursor is None:
+            return items
+        all_items = self.__get_next_page(cursor, items, item_attributes)
+        return all_items
+
+    ####################################################################################################################
+    def get_items_page_between(self, board_id, group_id, columns, column_id, start_date, end_date):
+        column_string = ""
+        for column in columns:
+            column_string = column_string + f"\"{column}\", "
+        column_string = column_string[:-2]
+        column_string = f"[{column_string}]"
+        item_attributes = f'''name id parent_item{{id name }} column_values(ids: {column_string}) {{text value
+        column{{id title}}
+        ... on BoardRelationValue {{display_value linked_items {{id}}}}
+        ... on MirrorValue {{display_value}}}}'''
+
+        initial_query = f'''{{boards(ids: {board_id}) {{groups(ids: "{group_id}") {{items_page(limit: 8 
+        query_params: {{rules: {{column_id: "{column_id}", compare_value: ["{start_date}", "{end_date}"], 
+        compare_attribute: "START_DATE", operator: between}}}}) {{
+        cursor
+        items {{{item_attributes}}}}}}}}}}}'''
+        data = {'query': initial_query}
+        response = self.__send_post_request(data)
+        if not response:
+            return None
+        items = [item for item in response['data']['boards'][0]['groups'][0]['items_page']['items']]
         cursor = response['data']['boards'][0]['groups'][0]['items_page']['cursor']
         if cursor is None:
             return items
         all_items = self.__get_next_page(cursor, items, item_attributes)
         return all_items
 
     ####################################################################################################################
```

