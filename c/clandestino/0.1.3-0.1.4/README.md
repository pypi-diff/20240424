# Comparing `tmp/clandestino-0.1.3.tar.gz` & `tmp/clandestino-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clandestino-0.1.3.tar", max compression
+gzip compressed data, was "clandestino-0.1.4.tar", max compression
```

## Comparing `clandestino-0.1.3.tar` & `clandestino-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-02-28 19:30:44.612244 clandestino-0.1.3/LICENSE
--rw-r--r--   0        0        0     4645 2024-03-02 12:54:08.336124 clandestino-0.1.3/README.md
--rw-r--r--   0        0        0       74 2024-03-02 12:54:08.336124 clandestino-0.1.3/clandestino/__init__.py
--rwxr-xr-x   0        0        0     8615 2024-03-02 13:06:08.641605 clandestino-0.1.3/clandestino/clandestino.py
--rw-r--r--   0        0        0        0 2024-03-02 12:54:08.336124 clandestino-0.1.3/clandestino/src/__init__.py
--rw-r--r--   0        0        0      291 2024-03-02 12:54:08.336124 clandestino-0.1.3/clandestino/src/ref.py
--rw-r--r--   0        0        0     1093 2024-03-02 14:21:04.016689 clandestino-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 clandestino-0.1.3/setup.py
--rw-r--r--   0        0        0     5685 1970-01-01 00:00:00.000000 clandestino-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-28 19:30:44.612244 clandestino-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4648 2024-04-24 15:28:52.950517 clandestino-0.1.4/README.md
+-rw-r--r--   0        0        0       74 2024-03-02 12:54:08.336124 clandestino-0.1.4/clandestino/__init__.py
+-rwxr-xr-x   0        0        0     8513 2024-04-24 15:28:52.950517 clandestino-0.1.4/clandestino/clandestino.py
+-rw-r--r--   0        0        0        0 2024-03-02 12:54:08.336124 clandestino-0.1.4/clandestino/src/__init__.py
+-rw-r--r--   0        0        0      291 2024-03-02 12:54:08.336124 clandestino-0.1.4/clandestino/src/ref.py
+-rw-r--r--   0        0        0     1093 2024-04-24 15:28:52.950517 clandestino-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 clandestino-0.1.4/setup.py
+-rw-r--r--   0        0        0     5688 1970-01-01 00:00:00.000000 clandestino-0.1.4/PKG-INFO
```

### Comparing `clandestino-0.1.3/LICENSE` & `clandestino-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clandestino-0.1.3/README.md` & `clandestino-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 | MongoDB       | mongo               | [here](extras/mongo/README.md)          | CLANDESTINO_MONGO_CONNECTION_STRING         |
 
 How to install extra packages?
 
 ```shell
 poetry add clandestino -E postgres
 OR
-pip install 'romeways[postgres]'
+pip install 'clandestino[postgres]'
 ```
 
 ## Config
 
 Clandestino has some configurations that you can set as environment variables or in a `.env` file.
 
 - `CLANDESTINO_MIGRATION_REPO` If you are using any of the extra packages, you must set them with their respective values: `POSTGRES`, `ELASTICSEARCH`, `MONGO`
```

### Comparing `clandestino-0.1.3/clandestino/clandestino.py` & `clandestino-0.1.4/clandestino/clandestino.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 
 def print_sep():
     print("=" * 100)
 
 
 async def help_callback():
-
     clandestino_options = f"cldest [{'|'.join(available_options.keys())}] [params]"
     header = (
         """ Clandestino is a database migration tool\n"""
         f""" Migration repository mode is: {config('CLANDESTINO_MIGRATION_REPO')}\n"""
         f"  {clandestino_options}\n"
     )
     print(header)
@@ -110,23 +109,19 @@
     print_sep()
     for _, migration_name, _ in iter_modules([f"{os.getcwd()}{os.sep}migrations"]):
         if str(migration_name).startswith("migration"):
             print(migration_name)
 
 
 async def rollback_migration():
-    modules_list = [
-        (importer, migration_name, is_package)
-        for importer, migration_name, is_package in iter_modules(
-            [f"{os.getcwd()}{os.sep}migrations"]
-        )
-    ]
+    _path = f"{os.getcwd()}{os.sep}migrations"
+    sys.path.append(_path)
+    modules_list = [module for module in iter_modules([_path])]
     if modules_list:
-        last_migration = modules_list[-1]
-        importer, migration_name, is_package = last_migration
+        importer, migration_name, is_package = modules_list[-1]
         if not is_package:
             answer = input(
                 f"You relly want to roll back this migration '{migration_name}'? Y/n: "
             )
             if answer == "Y":
                 print(
                     "Roll back migrations: "
```

### Comparing `clandestino-0.1.3/pyproject.toml` & `clandestino-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clandestino"
-version = "0.1.3"
+version = "0.1.4"
 description = "Simple migration tool for your python project"
 authors = ["XimitGaia <im.ximit@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-decouple = "^3.8"
```

### Comparing `clandestino-0.1.3/setup.py` & `clandestino-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'postgres': ['clandestino_postgres>=0.1.1,<0.2.0']}
 
 entry_points = \
 {'console_scripts': ['cdt = clandestino.clandestino:main']}
 
 setup_kwargs = {
     'name': 'clandestino',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Simple migration tool for your python project',
-    'long_description': '# Clandestino\n\n![banner](docs/banner.jpeg)\n\n```\nBy: CenturyBoys\n```\n\nThis package provides a migration tool. It includes a command-line interface (CLI) for easy execution and a single asynchronous function that can be imported and used in your code.\n\n## Install\n\nThe main package does not have any database implementation and uses only the interfaces and abstractions from the `clandestino_interfaces` package. In other words, you are free to create your own implementations. We will explain the details later.\n\n| Database Type | Install using extra | description                             | Environment parameter                       |\n|---------------|---------------------|-----------------------------------------|---------------------------------------------|\n| PostgreSQL    | postgres            | [here](extras/postgres/README.md)       | CLANDESTINO_POSTGRES_CONNECTION_STRING      |\n| Elasticsearch | elasticsearch       | [here](extras/elasticsearch/README.md)  | CLANDESTINO_ELASTICSEARCH_CONNECTION_STRING |\n| MongoDB       | mongo               | [here](extras/mongo/README.md)          | CLANDESTINO_MONGO_CONNECTION_STRING         |\n\nHow to install extra packages?\n\n```shell\npoetry add clandestino -E postgres\nOR\npip install \'romeways[postgres]\'\n```\n\n## Config\n\nClandestino has some configurations that you can set as environment variables or in a `.env` file.\n\n- `CLANDESTINO_MIGRATION_REPO` If you are using any of the extra packages, you must set them with their respective values: `POSTGRES`, `ELASTICSEARCH`, `MONGO`\n\n## CLI\n\n### [-h] Help command\n\n```bash\n$cdt -h         \n Clandestino is a database migration tool\n Migration repository mode is: ELASTICSEARCH\n  cldest [-h|-m|-lm|-rm|-cm] [params]\n\n    -h: Display help\n    -m: Migrate database\n    -lm: List migrations\n    -rm: Rollback last migration\n    -cm: Create database migration - params [name type]\n```\n\n### [-m] Migrate database\n\nMigrate databases using the files within the `./migrations` folder. Each migration checks if it\'s already run. If not, the migration is applied, the information is saved, and the async def up(self) -> None method is called. No migration will be executed twice.\n\nThe system will display the migration status:\n- OK = ✅\n- ERROR = ⚠️\n- SKIPPED = ⏭️\n\n### [-lm] List migrations\n\nList all migration within the `./migrations` folder\n\n### [-rm] Rollback migration\n\nRollback the last database migration using the latest file in the `./migrations` folder. The `async def down(self) -> None` method within the file will be called.\n\nThe system will display the rollback status:\n- OK = ✅\n- ERROR = ⚠️\n- SKIPPED = ⏭️\n\n### [-cm] Create migration\n\nCreate a migration within the `./migrations` folder, if the folder not exists create it to. \n\nThis command receive two parameters:\n\n- Migration name \n- Migration type, if not filled will use default migration template.\n\nThe migration file will be like this `migration_{datetime_reference}_{migration_name}.py`\n\n## Migration file\n\nThe migration file inherit the abstract class `AbstractMigration` and need declare two fundtions:\n\n- `async def up(self) -> None`. This method will be called on migration command\n- `async def down(self) -> None`. This method will be called on rollback command\n\nSee bellow an empty template file\n\n```python\nfrom clandestino_interfaces import AbstractMigration\n\nclass Migration(AbstractMigration):\n\n    infra = None\n\n    async def up(self) -> None:\n        """Do modifications in database"""\n        pass\n\n    async def down(self) -> None:\n        """Undo modifications in database"""\n        pass\n```\n\n## Self Implementation\n\nTo create your own Clandestino implementation, simply create a file named `repository.py` inside the `./migrations` folder. This file should contain a class named `MigrateRepository` that inherits from `clandestino_interfaces.IMigrateRepository`.\n\nObservation: Your migrations need to handler the database connections by your self.\n\nSee bellow the interface:\n\n```python\nfrom abc import ABC, abstractmethod\n\nclass IMigrateRepository(ABC):\n    @classmethod\n    @abstractmethod\n    async def create_control_table(cls) -> None:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def control_table_exists(cls) -> bool:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def register_migration_execution(cls, migration_name: str) -> None:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def migration_already_executed(cls, migration_name: str) -> bool:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def remove_migration_execution(cls, migration_name: str) -> None:\n        pass\n```',
+    'long_description': '# Clandestino\n\n![banner](docs/banner.jpeg)\n\n```\nBy: CenturyBoys\n```\n\nThis package provides a migration tool. It includes a command-line interface (CLI) for easy execution and a single asynchronous function that can be imported and used in your code.\n\n## Install\n\nThe main package does not have any database implementation and uses only the interfaces and abstractions from the `clandestino_interfaces` package. In other words, you are free to create your own implementations. We will explain the details later.\n\n| Database Type | Install using extra | description                             | Environment parameter                       |\n|---------------|---------------------|-----------------------------------------|---------------------------------------------|\n| PostgreSQL    | postgres            | [here](extras/postgres/README.md)       | CLANDESTINO_POSTGRES_CONNECTION_STRING      |\n| Elasticsearch | elasticsearch       | [here](extras/elasticsearch/README.md)  | CLANDESTINO_ELASTICSEARCH_CONNECTION_STRING |\n| MongoDB       | mongo               | [here](extras/mongo/README.md)          | CLANDESTINO_MONGO_CONNECTION_STRING         |\n\nHow to install extra packages?\n\n```shell\npoetry add clandestino -E postgres\nOR\npip install \'clandestino[postgres]\'\n```\n\n## Config\n\nClandestino has some configurations that you can set as environment variables or in a `.env` file.\n\n- `CLANDESTINO_MIGRATION_REPO` If you are using any of the extra packages, you must set them with their respective values: `POSTGRES`, `ELASTICSEARCH`, `MONGO`\n\n## CLI\n\n### [-h] Help command\n\n```bash\n$cdt -h         \n Clandestino is a database migration tool\n Migration repository mode is: ELASTICSEARCH\n  cldest [-h|-m|-lm|-rm|-cm] [params]\n\n    -h: Display help\n    -m: Migrate database\n    -lm: List migrations\n    -rm: Rollback last migration\n    -cm: Create database migration - params [name type]\n```\n\n### [-m] Migrate database\n\nMigrate databases using the files within the `./migrations` folder. Each migration checks if it\'s already run. If not, the migration is applied, the information is saved, and the async def up(self) -> None method is called. No migration will be executed twice.\n\nThe system will display the migration status:\n- OK = ✅\n- ERROR = ⚠️\n- SKIPPED = ⏭️\n\n### [-lm] List migrations\n\nList all migration within the `./migrations` folder\n\n### [-rm] Rollback migration\n\nRollback the last database migration using the latest file in the `./migrations` folder. The `async def down(self) -> None` method within the file will be called.\n\nThe system will display the rollback status:\n- OK = ✅\n- ERROR = ⚠️\n- SKIPPED = ⏭️\n\n### [-cm] Create migration\n\nCreate a migration within the `./migrations` folder, if the folder not exists create it to. \n\nThis command receive two parameters:\n\n- Migration name \n- Migration type, if not filled will use default migration template.\n\nThe migration file will be like this `migration_{datetime_reference}_{migration_name}.py`\n\n## Migration file\n\nThe migration file inherit the abstract class `AbstractMigration` and need declare two fundtions:\n\n- `async def up(self) -> None`. This method will be called on migration command\n- `async def down(self) -> None`. This method will be called on rollback command\n\nSee bellow an empty template file\n\n```python\nfrom clandestino_interfaces import AbstractMigration\n\nclass Migration(AbstractMigration):\n\n    infra = None\n\n    async def up(self) -> None:\n        """Do modifications in database"""\n        pass\n\n    async def down(self) -> None:\n        """Undo modifications in database"""\n        pass\n```\n\n## Self Implementation\n\nTo create your own Clandestino implementation, simply create a file named `repository.py` inside the `./migrations` folder. This file should contain a class named `MigrateRepository` that inherits from `clandestino_interfaces.IMigrateRepository`.\n\nObservation: Your migrations need to handler the database connections by your self.\n\nSee bellow the interface:\n\n```python\nfrom abc import ABC, abstractmethod\n\nclass IMigrateRepository(ABC):\n    @classmethod\n    @abstractmethod\n    async def create_control_table(cls) -> None:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def control_table_exists(cls) -> bool:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def register_migration_execution(cls, migration_name: str) -> None:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def migration_already_executed(cls, migration_name: str) -> bool:\n        pass\n\n    @classmethod\n    @abstractmethod\n    async def remove_migration_execution(cls, migration_name: str) -> None:\n        pass\n```',
     'author': 'XimitGaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clandestino-0.1.3/PKG-INFO` & `clandestino-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clandestino
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple migration tool for your python project
 Author: XimitGaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: elasticsearch
@@ -42,15 +42,15 @@
 | MongoDB       | mongo               | [here](extras/mongo/README.md)          | CLANDESTINO_MONGO_CONNECTION_STRING         |
 
 How to install extra packages?
 
 ```shell
 poetry add clandestino -E postgres
 OR
-pip install 'romeways[postgres]'
+pip install 'clandestino[postgres]'
 ```
 
 ## Config
 
 Clandestino has some configurations that you can set as environment variables or in a `.env` file.
 
 - `CLANDESTINO_MIGRATION_REPO` If you are using any of the extra packages, you must set them with their respective values: `POSTGRES`, `ELASTICSEARCH`, `MONGO`
```

