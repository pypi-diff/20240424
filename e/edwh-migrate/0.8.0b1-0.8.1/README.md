# Comparing `tmp/edwh_migrate-0.8.0b1.tar.gz` & `tmp/edwh_migrate-0.8.1.tar.gz`

## Comparing `edwh_migrate-0.8.0b1.tar` & `edwh_migrate-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/migrations.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    37633 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/.ruff_cache/0.1.4/14106432868302123460
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/.ruff_cache/0.1.4/5683927022054931246
--rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/.ruff_cache/0.1.4/9948050529372631611
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/examples/Dockerfile
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/examples/docker-compose.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/examples/migrations.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    27515 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/src/edwh_migrate/py.typed
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/fixtures.py
--rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/test_basics.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/test_typedal.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/sqlite_empty/empty_sqlite.db
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/sqlite_empty/just_implemented_features.db
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/tests/sqlite_empty/just_implemented_features.sql
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/LICENSE.txt
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/README.md
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/pyproject.toml
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 edwh_migrate-0.8.0b1/PKG-INFO
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/migrations.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    37633 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/.ruff_cache/0.1.4/14106432868302123460
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/.ruff_cache/0.1.4/5683927022054931246
+-rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/.ruff_cache/0.1.4/9948050529372631611
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/examples/Dockerfile
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/examples/docker-compose.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/examples/migrations.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    27873 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/src/edwh_migrate/py.typed
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/fixtures.py
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/test_basics.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/test_import_migrations.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/test_postgres.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/test_redis.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/test_typedal.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/sqlite_empty/just_implemented_features.psql.sql
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/README.md
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 edwh_migrate-0.8.1/PKG-INFO
```

### Comparing `edwh_migrate-0.8.0b1/CHANGELOG.md` & `edwh_migrate-0.8.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.8.1 (2024-04-24)
+### Fix
+* Redis.from_url for better parsing + test valkey as drop-in redis replacement ([`6b842e8`](https://github.com/educationwarehouse/migrate/commit/6b842e81e43ec2874fefe29b7ee7d94115483ba1))
+* Support custom redis port + add test for it ([`228c72a`](https://github.com/educationwarehouse/migrate/commit/228c72afe689ed2b0845e33ee2d422f5851bb35d))
+
+## v0.8.0 (2024-03-21)
+
+
+
 ## v0.8.0-beta.1 (2024-03-20)
 
 ### Feature
 
 * **edwh_migrate:** Add list_migrations and mark_migration functions + fixes ([`a0be3da`](https://github.com/educationwarehouse/migrate/commit/a0be3daf3ef65f438f89a79a8182fcdb0268dce7))
 
 ### Fix
```

### Comparing `edwh_migrate-0.8.0b1/migrations.py` & `edwh_migrate-0.8.1/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/.ruff_cache/0.1.4/14106432868302123460` & `edwh_migrate-0.8.1/.ruff_cache/0.1.4/14106432868302123460`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/.ruff_cache/0.1.4/9948050529372631611` & `edwh_migrate-0.8.1/.ruff_cache/0.1.4/9948050529372631611`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/examples/migrations.py` & `edwh_migrate-0.8.1/examples/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/src/edwh_migrate/__init__.py` & `edwh_migrate-0.8.1/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/src/edwh_migrate/migrate.py` & `edwh_migrate-0.8.1/src/edwh_migrate/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,23 @@
 from configuraptor.errors import ConfigErrorMissingKey, IsPostponedError
 from dotenv import find_dotenv
 from pydal import DAL, Field
 from pydal.objects import Table
 
 try:
     from typedal import TypeDAL
-except ImportError:
+except ImportError:  # pragma: no cover
     TypeDAL = DAL  # type: ignore
 
 Migration: typing.TypeAlias = typing.Callable[[DAL], bool]
 
 registered_functions: OrderedDict[str, Migration] = OrderedDict()
 
+TEN_MINUTES = 600
+
 
 class BaseEDWHMigrateException(BaseException):
     """
     Most top-level exception class for this module.
 
     Not caught by `except Exception`.
     """
@@ -285,17 +287,19 @@
     )
 
     if is_postgres and long_running:
         # https://www.pgpool.net/docs/latest/en/html/sql-pgpool-set.html
         # make this connection able to live longer, because the functions can take over 30s
         # to perform the job.
         # db.executesql("PGPOOL SET client_idle_limit = 3600;")
-        with contextlib.suppress(Exception):
-            print("Setting up for long running connection")
+        print("Setting up for long running connection")
+        try:
             db.executesql(f"PGPOOL SET client_idle_limit = {long_running if str(long_running).isdigit() else 3600};")
+        except psycopg2.errors.Error:
+            # maybe not using PGPOOL, ignore
             db.rollback()
 
     if remove_migrate_tablefile:
         tablefile_path = Path(db._folder or ".") / f"{db._uri_hash}_ewh_implemented_features.table"
         tablefile_path.unlink(missing_ok=True)
 
     define_ewh_implemented_features(db, impl_feat_table_name or config.migrate_table)
@@ -447,15 +451,15 @@
     extension = prepared_sql_path.suffix.lower()
 
     cat_command = {
         ".sql": "cat",
         ".xz": "xzcat",
         ".gz": "zcat",
     }.get(extension, config.migrate_cat_command)
-    if not cat_command:
+    if not cat_command:  # pragma: no cover
         raise NotImplementedError(f"Extension {extension} not supported for {prepared_sql_path}")
     unpack = plumbum.local[cat_command][prepared_sql_path]
 
     # unpack is now the command to cat the sql to stdout
     # which is piped to psql to perform the recovery
 
     # parse the db uri to find hostname and port and such to
@@ -467,14 +471,15 @@
         psql = plumbum.local["psql"][config.migrate_uri]
         sql_consumer = psql
     else:
         filepath = uri.path
         if "///" not in config.migrate_uri:
             # else absolute path, don't strip!
             filepath = filepath.strip("/")
+
         sqlite_database_path = pathlib.Path(uri.netloc) / pathlib.Path(filepath)
         sql_consumer = plumbum.local["sqlite3"][sqlite_database_path]
     # combine both
     cmd = unpack | sql_consumer
 
     print("UNPACKING AND INSTALLING DATABASE:", cmd)
     # noinspection PyStatementEffect
@@ -485,28 +490,28 @@
     if is_postgres and set_schema:
         echo = plumbum.local["echo"]
         cmd = echo[f"SET search_path TO {set_schema};"] | sql_consumer
         print("For postgres: set schema to public:", cmd)
         cmd()
 
 
-def try_setup_db(config: Optional[Config] = None) -> typing.Optional[DAL]:
+def try_setup_db(config: Optional[Config] = None, max_time: int = TEN_MINUTES) -> typing.Optional[DAL]:
     """
     Handle multiple scenario's such as an existing db, a db that can be loaded from a backup or a fully new db.
     """
     started = time.time()
-    while time.time() - started < 600:
+    while time.time() - started < max_time:
         try:
             db = setup_db(config=config)
             print("activate_migrations connected after", time.time() - started, "seconds.")
 
             db.commit()
             # without an error, all *should* be well...
             return db
-        except DatabaseNotYetInitialized as e:
+        except DatabaseNotYetInitialized as e:  # pragma: no cover
             # the connection succeeded, but when encountering an empty databse,
             # the features table will not be found, and this will raise an exception
             # this error is to be expected, since the database is not yet recovered...
             print("table not found, starting database restore")
             # recover the erroneous database connection to start database recovery.
             _, db = e.args
             # clear the current connection from errors :
@@ -527,24 +532,24 @@
                 with contextlib.suppress(DatabaseNotYetInitialized):
                     print("RECOVER: Failed. Starting from scratch with new .table file.")
                     return setup_db(migrate=True, migrate_enabled=True, remove_migrate_tablefile=True)
 
             except Exception as e:
                 print("RECOVER: database recovery went wrong:", e)
             break  # don't retry
-        except Exception as e:
+        except Exception as e:  # pragma: no cover
             print(
                 "activate_migrations failed to connect to database. "
                 "sleeping and retrying in 3 seconds. will try for 10 min."
             )
             print(e)
             time.sleep(3)
 
     # shouldn't happen :(
-    return None
+    return None  # pragma: no cover
 
 
 def mark_migration(db: DAL, name: str, installed: bool) -> int | None:
     """
     Store the result of a migration in the implemented_features table.
     """
     new_id = db.ewh_implemented_features.update_or_insert(
@@ -552,21 +557,21 @@
         name=name,
         installed=installed,
         last_update_dttm=datetime.datetime.now(),
     )  # type: int | None
     return new_id
 
 
-def activate_migrations(config: Optional[Config] = None) -> bool:
+def activate_migrations(config: Optional[Config] = None, max_time: int = TEN_MINUTES) -> bool:
     """
     Start the migration process, don't wait for a lock.
     """
     config = config or get_config()
 
-    db = try_setup_db(config)
+    db = try_setup_db(config, max_time=max_time)
     if not db:
         raise ValueError("No db could be set up!")
 
     successes = []
     # perform migrations
     for name, function in registered_functions.items():
         print("test:", name)
@@ -600,15 +605,18 @@
             print("already installed. ")
 
     db.close()
 
     # clean redis whenever possible
     # reads REDIS_MASTER_HOST from the environment
     if redis_host := config.redis_host:
-        r = redis.Redis(redis_host)
+        if not redis_host.startswith("redis://"):
+            redis_host = f"redis://{redis_host}"
+
+        r = redis.Redis.from_url(redis_host)
         keys = r.keys()
         print(f"Removing {len(keys)} keys from redis.")
         for key in keys:
             del r[key]
         print("done")
     return all(successes)
```

### Comparing `edwh_migrate-0.8.0b1/tests/fixtures.py` & `edwh_migrate-0.8.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/tests/test_basics.py` & `edwh_migrate-0.8.1/tests/test_basics.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from src.edwh_migrate.__about__ import __version__
 from src.edwh_migrate.migrate import (
     MigrateLockExists,
     MigrationFailed,
     get_config,
     schema_versioned_lock_file,
 )
+
 from .fixtures import (  # noqa
     clean_migrate,
     fixture_temp_chdir,
     sqlite_empty,
     tmp_empty_sqlite_db_file,
     tmp_just_implemented_features_sqlite_db_file,
     tmp_just_implemented_features_sqlite_sql_file,
@@ -181,20 +182,32 @@
 
     fake_path.touch()
     with pytest.raises(FileNotFoundError):
         # even if the file doesn't exist but has invalid extension, not found error is raised.
         recover_database_from_backup()
 
     config.database_to_restore = str(tmp_just_implemented_features_sqlite_sql_file)
-    recover_database_from_backup()
+    recover_database_from_backup(config=config)  # sqlite:///tmp/.../empty_sqlite.db
 
     # no error anymore:
     assert migrate.setup_db(migrate=False)
 
 
+def test_recover_database_from_backup_relative(tmp_just_implemented_features_sqlite_sql_file, tmp_empty_sqlite_db_file):
+    config = get_config()
+
+    filepath = pathlib.Path(config.migrate_uri.split("://")[-1])
+    with chdir(filepath.parent):
+        config.migrate_uri = f"sqlite://{filepath.name}"  # sqlite://empty_sqlite.db
+        config.database_to_restore = str(tmp_just_implemented_features_sqlite_sql_file)
+        recover_database_from_backup(config=config)
+
+        assert migrate.setup_db(migrate=False)
+
+
 def test_config():
     config = get_config()
     assert config is get_config()  # singleton
 
     assert config.database_to_restore is get_config().database_to_restore
 
     assert "<Config{" in repr(config)
```

### Comparing `edwh_migrate-0.8.0b1/tests/test_typedal.py` & `edwh_migrate-0.8.1/tests/test_typedal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import pytest
 from typedal import TypeDAL
 
-from src.edwh_migrate import setup_db, activate_migrations
+from src.edwh_migrate import activate_migrations, setup_db
 
 from .fixtures import (  # noqa
     clean_migrate,
     fixture_temp_chdir,
     sqlite_empty,
     tmp_empty_sqlite_db_file,
     tmp_just_implemented_features_sqlite_db_file,
@@ -15,26 +15,26 @@
     tmp_sqlite_folder,
     tmp_sqlite_sql_file,
 )
 
 
 @pytest.fixture
 def env_use_typedal():
-    os.environ['USE_TYPEDAL'] = "1"
+    os.environ["USE_TYPEDAL"] = "1"
     yield
-    del os.environ['USE_TYPEDAL']
+    del os.environ["USE_TYPEDAL"]
 
 
 @pytest.fixture
 def tmp_typedal_env(fixture_temp_chdir):
-    os.environ['DB_URI'] = f"sqlite://{fixture_temp_chdir / 'some.sqlite'}"
-    os.environ['FOLDER'] = str(fixture_temp_chdir / "database")
+    os.environ["DB_URI"] = f"sqlite://{fixture_temp_chdir / 'some.sqlite'}"
+    os.environ["FOLDER"] = str(fixture_temp_chdir / "database")
     yield
-    del os.environ['DB_URI']
-    del os.environ['FOLDER']
+    del os.environ["DB_URI"]
+    del os.environ["FOLDER"]
 
 
 def test_setup_db(tmp_just_implemented_features_sqlite_db_file, clean_migrate):
     db = setup_db(dal_class=TypeDAL)
 
     assert isinstance(db, TypeDAL)
```

### Comparing `edwh_migrate-0.8.0b1/tests/sqlite_empty/empty_sqlite.db` & `edwh_migrate-0.8.1/tests/sqlite_empty/empty_sqlite.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/tests/sqlite_empty/just_implemented_features.db` & `edwh_migrate-0.8.1/tests/sqlite_empty/just_implemented_features.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/.gitignore` & `edwh_migrate-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/LICENSE.txt` & `edwh_migrate-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/README.md` & `edwh_migrate-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.8.0b1/pyproject.toml` & `edwh_migrate-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     "hatch",
     "python-semantic-release<8",
     "black",
     "isort",
     "pytest",
     "pytest-cov",
     "contextlib-chdir",
+    "testcontainers",
+    "SQLAlchemy-Utils", # for drop_database
 ]
 
 [template.plugins.default]
 src-layout = true
 
 [tool.setuptools.package-data]
 "edwh_migrate" = ["py.typed"]
@@ -159,33 +161,14 @@
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
-[tool.coverage.run]
-source_pkgs = ["_", "tests"]
-branch = true
-parallel = true
-omit = [
-    "src/_/__about__.py",
-]
-
-[tool.coverage.paths]
-_ = ["src/_", "*/-/src/_"]
-tests = ["tests", "*/-/tests"]
-
-[tool.coverage.report]
-exclude_lines = [
-    "no cov",
-    "if __name__ == .__main__.:",
-    "if TYPE_CHECKING:",
-]
-
 [tool.pytest.ini_options]
 pythonpath = [
     "src",
 ]
 
 [tool.pydocstyle]
 match-dir = '(?!venv)[^\.].*'
```

### Comparing `edwh_migrate-0.8.0b1/PKG-INFO` & `edwh_migrate-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-migrate
-Version: 0.8.0b1
+Version: 0.8.1
 Summary: Helps migrating database schema changes using pydal. 
 Project-URL: Documentation, https://github.com/educationwarehouse/migrate#readme
 Project-URL: Issues, https://github.com/educationwarehouse/migrate/issues
 Project-URL: Source, https://github.com/educationwarehouse/migrate
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -26,14 +26,16 @@
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: contextlib-chdir; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: python-semantic-release<8; extra == 'dev'
+Requires-Dist: sqlalchemy-utils; extra == 'dev'
+Requires-Dist: testcontainers; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Educationwarehouse's Migrate
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-migrate.svg)](https://pypi.org/project/edwh-migrate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-migrate.svg)](https://pypi.org/project/edwh-migrate)
```

