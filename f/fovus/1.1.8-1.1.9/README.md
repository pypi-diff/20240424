# Comparing `tmp/fovus-1.1.8-py3-none-any.whl.zip` & `tmp/fovus-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 58011 bytes, number of entries: 46
+Zip file size: 58421 bytes, number of entries: 46
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 23-Jul-17 01:48 fovus/root_config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/adapter/__init__.py
 -rw-r--r--  2.0 unx    26500 b- defN 23-Aug-31 07:14 fovus/adapter/fovus_api_adapter.py
--rw-r--r--  2.0 unx    19619 b- defN 23-Aug-31 10:07 fovus/adapter/fovus_s3_adapter.py
+-rw-r--r--  2.0 unx    21490 b- defN 23-Aug-31 19:29 fovus/adapter/fovus_s3_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/cli/__init__.py
--rw-r--r--  2.0 unx    15658 b- defN 23-Aug-31 10:07 fovus/cli/cli_action_runner.py
+-rw-r--r--  2.0 unx    15750 b- defN 23-Aug-31 19:29 fovus/cli/cli_action_runner.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Jul-17 01:48 fovus/cli/documenter.py
--rw-r--r--  2.0 unx      997 b- defN 23-Aug-30 20:05 fovus/cli/fovus_cli.py
+-rw-r--r--  2.0 unx     1656 b- defN 23-Aug-31 19:29 fovus/cli/fovus_cli.py
 -rw-r--r--  2.0 unx    31421 b- defN 23-Aug-31 08:56 fovus/cli/fovus_cli_argument_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/config/__init__.py
--rw-r--r--  2.0 unx      840 b- defN 23-Aug-31 10:07 fovus/config/config.py
+-rw-r--r--  2.0 unx      840 b- defN 23-Aug-31 19:29 fovus/config/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/constants/__init__.py
 -rw-r--r--  2.0 unx     1658 b- defN 23-Jul-26 20:54 fovus/constants/benchmark_constants.py
 -rw-r--r--  2.0 unx      485 b- defN 23-Jul-17 01:48 fovus/constants/cli_action_runner_constants.py
--rw-r--r--  2.0 unx     9584 b- defN 23-Aug-31 08:56 fovus/constants/cli_constants.py
+-rw-r--r--  2.0 unx     9641 b- defN 23-Aug-31 19:29 fovus/constants/cli_constants.py
 -rw-r--r--  2.0 unx     2001 b- defN 23-Aug-30 01:37 fovus/constants/fovus_api_constants.py
--rw-r--r--  2.0 unx      194 b- defN 23-Jul-17 01:48 fovus/constants/util_constants.py
+-rw-r--r--  2.0 unx      194 b- defN 23-Aug-31 18:29 fovus/constants/util_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/exception/__init__.py
 -rw-r--r--  2.0 unx      291 b- defN 23-Jul-17 01:48 fovus/exception/status_code_exception.py
 -rw-r--r--  2.0 unx      183 b- defN 23-Jul-17 01:48 fovus/exception/system_exception.py
 -rw-r--r--  2.0 unx      174 b- defN 23-Jul-17 01:48 fovus/exception/user_exception.py
 -rw-r--r--  2.0 unx     1191 b- defN 23-Aug-28 07:52 fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json
 -rw-r--r--  2.0 unx     1249 b- defN 23-Jul-17 01:48 fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json
 -rw-r--r--  2.0 unx      949 b- defN 23-Aug-30 01:37 fovus/fovus_provided_configs/FOVUS_job_template_containerized.json
@@ -35,14 +35,14 @@
 -rw-r--r--  2.0 unx     9310 b- defN 23-Aug-30 19:46 fovus/util/file_util.py
 -rw-r--r--  2.0 unx    15335 b- defN 23-Aug-22 22:37 fovus/util/fovus_api_util.py
 -rw-r--r--  2.0 unx     1956 b- defN 23-Jul-17 01:48 fovus/util/fovus_cli_argument_parser_util.py
 -rw-r--r--  2.0 unx     1198 b- defN 23-Aug-30 01:37 fovus/util/fovus_s3_adapter_util.py
 -rw-r--r--  2.0 unx     1240 b- defN 23-Jul-17 01:48 fovus/util/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 01:48 fovus/validator/__init__.py
 -rw-r--r--  2.0 unx     4793 b- defN 23-Aug-30 01:37 fovus/validator/fovus_api_validator.py
--rw-r--r--  2.0 unx    14101 b- defN 23-Aug-31 10:08 fovus-1.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    12427 b- defN 23-Aug-31 10:08 fovus-1.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-31 10:08 fovus-1.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Aug-31 10:08 fovus-1.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Aug-31 10:08 fovus-1.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4096 b- defN 23-Aug-31 10:08 fovus-1.1.8.dist-info/RECORD
-46 files, 194928 bytes uncompressed, 51351 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx    14101 b- defN 23-Aug-31 19:53 fovus-1.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    12427 b- defN 23-Aug-31 19:53 fovus-1.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-31 19:53 fovus-1.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Aug-31 19:53 fovus-1.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Aug-31 19:53 fovus-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4097 b- defN 23-Aug-31 19:53 fovus-1.1.9.dist-info/RECORD
+46 files, 197608 bytes uncompressed, 51761 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -114,26 +114,26 @@
 
 Filename: fovus/validator/__init__.py
 Comment: 
 
 Filename: fovus/validator/fovus_api_validator.py
 Comment: 
 
-Filename: fovus-1.1.8.dist-info/LICENSE.txt
+Filename: fovus-1.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fovus-1.1.8.dist-info/METADATA
+Filename: fovus-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: fovus-1.1.8.dist-info/WHEEL
+Filename: fovus-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: fovus-1.1.8.dist-info/entry_points.txt
+Filename: fovus-1.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: fovus-1.1.8.dist-info/top_level.txt
+Filename: fovus-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fovus-1.1.8.dist-info/RECORD
+Filename: fovus-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fovus/adapter/fovus_s3_adapter.py

```diff
@@ -1,17 +1,16 @@
 import concurrent.futures
 import json
+import logging
 import os
 import random
 import time
-import traceback
 from http import HTTPStatus
 from typing import Any, Callable, Optional, ParamSpec, Type, TypedDict, TypeVar, Union
 
-import boto3
 from mypy_boto3_s3 import S3Client
 from mypy_boto3_s3.type_defs import ObjectTypeDef
 from tqdm import tqdm
 
 from fovus.adapter.fovus_api_adapter import FovusApiAdapter
 from fovus.constants.cli_constants import (
     CLI_ARGUMENTS,
@@ -109,15 +108,15 @@
             )
             return
 
         job_data = {
             "job_id": self.job_id,
         }
         fovus_job_info_directory_path = os.path.join(self.local_root_directory_path, FOVUS_JOB_INFO_FOLDER)
-        os.makedirs(fovus_job_info_directory_path)
+        os.makedirs(fovus_job_info_directory_path, exist_ok=True)
         job_data_filepath = os.path.join(fovus_job_info_directory_path, JOB_DATA_FILENAME)
         with FileUtil.open(job_data_filepath, "w") as job_data_file:
             json.dump(job_data, job_data_file)
 
     def download_files(self):
         print("Retrieving file list from server...")
         s3_object_list = self._get_s3_object_list()
@@ -162,80 +161,60 @@
     Out = TypeVar("Out")
 
     def exponential_backoff_retry(
         self,
         function: Callable[Param, Out],
         max_retries=5,
         exceptions_to_raise: Union[list[Type[BaseException]], None] = None,
-        print_function: Callable[[str], None] = print,
         base=2,
         multiplier=1,
         randomize_sleep=True,
     ) -> Callable[Param, Out]:
         def wrapper(*args, **kwargs):
-            retry = 0
+            retry_count = 0
             while True:
                 try:
                     return function(*args, **kwargs)
-                except BaseException as error:  # pylint: disable=broad-except
-                    print_function(traceback.format_exc())
-                    print_function("Retrying...")
-                    if retry >= max_retries - 1 or (
+                except BaseException as exc:  # pylint: disable=broad-except
+                    logging.error("Exception caught by exponential_backoff_retry.")
+                    logging.exception(exc)
+
+                    if retry_count >= max_retries - 1 or (
                         isinstance(exceptions_to_raise, list)
-                        and any(isinstance(error, exception) for exception in exceptions_to_raise)
+                        and any(isinstance(exc, exception) for exception in exceptions_to_raise)
                     ):
-                        raise error
-                    time.sleep((base**retry) * multiplier * (random.random() if randomize_sleep else 1))  # nosec B311
-                    retry += 1
+                        raise exc
+
+                    time.sleep(
+                        (base**retry_count) * multiplier * (random.random() if randomize_sleep else 1)  # nosec B311
+                    )
+                    retry_count += 1
+
+                    logging.info("Retrying function.")
 
         return wrapper
 
     def _try_operate_on_file_list(
         self,
         file_operation: Callable[[Any, tqdm], Any],
         executor: concurrent.futures.ThreadPoolExecutor,
         remaining_objects: Union[list[str], list[ObjectTypeDef]],
         progress_bar: tqdm,
     ):
-        s3_client = None
-
-        if self.download_s3_info:
-            s3_client = self.download_s3_info["s3_client"]
-
-        if self.upload_s3_info:
-            s3_client = self.upload_s3_info["s3_client"]
-
-        if not s3_client:
-            s3_client = boto3.client("s3")
-
-        s3_exceptions = s3_client.exceptions
-
-        wrapped_file_operation = self.exponential_backoff_retry(
-            file_operation,
-            exceptions_to_raise=[s3_exceptions.NoSuchKey, s3_exceptions.NoSuchBucket],
-            print_function=progress_bar.write,
-        )
-
-        futures_to_obj = {executor.submit(wrapped_file_operation, obj, progress_bar): obj for obj in remaining_objects}
+        futures_to_obj = {executor.submit(file_operation, obj, progress_bar): obj for obj in remaining_objects}
 
         for future in concurrent.futures.as_completed(futures_to_obj):
             obj = futures_to_obj[future]
             key = obj if isinstance(obj, str) else obj["Key"]
 
             try:
                 future.result()
-            except s3_exceptions.NoSuchKey:
-                progress_bar.write(traceback.format_exc())
-                progress_bar.write("File not found: " + key)
-            except s3_exceptions.NoSuchBucket:
-                progress_bar.write(traceback.format_exc())
-                progress_bar.write("Bucket not found")
-            except Exception:  # pylint: disable=broad-except
-                progress_bar.write(traceback.format_exc())
-                progress_bar.write(f"An unknown error occured while downloading {key}")
+            except BaseException as exc:  # pylint: disable=broad-except
+                logging.error("Exception caught in _try_operate_on_file_list for %s.", key)
+                logging.exception(exc)
 
     def _instantiate_upload_instance_variables(self):
         print("Preparing to upload files.")
         self.local_filepath_list, self.task_count, self.total_file_size_bytes = FileUtil.get_files_in_directory(
             self.local_root_directory_path, self.cli_dict[INCLUDE_INPUT], self.cli_dict[EXCLUDE_INPUT]
         )
         self._validate_upload_job()
@@ -249,68 +228,114 @@
         if errors:
             raise UserException(
                 HTTPStatus.BAD_REQUEST,
                 self.__class__.__name__,
                 f"No {' or '.join(errors)} found to upload. Please check your include/exclude filters.",
             )
 
-    def _initiate_multipart_upload(self, bucket_name: str, key: str) -> str:
+    def _s3_initiate_multipart_upload(self, bucket_name: str, key: str) -> str:
+        def file_operation() -> str:
+            s3_info = self._get_upload_s3_info()
+            response = s3_info["s3_client"].create_multipart_upload(Bucket=bucket_name, Key=key)
+            return response["UploadId"]
+
         s3_info = self._get_upload_s3_info()
-        response = s3_info["s3_client"].create_multipart_upload(Bucket=bucket_name, Key=key)
-        return response["UploadId"]
+        s3_exceptions = s3_info["s3_client"].exceptions
+
+        wrapped_file_operation = self.exponential_backoff_retry(
+            file_operation,
+            exceptions_to_raise=[s3_exceptions.NoSuchBucket],
+        )
+
+        return wrapped_file_operation()
+
+    def _s3_upload_multipart_part(
+        self, data: bytes, upload_id: str, bucket_name: str, key: str, part_number: int
+    ) -> Any:
+        def file_operation() -> Any:
+            s3_info = self._get_upload_s3_info()
+            response = s3_info["s3_client"].upload_part(
+                Bucket=bucket_name, Key=key, PartNumber=part_number, UploadId=upload_id, Body=data
+            )
+            part = {"PartNumber": part_number, "ETag": response["ETag"]}
+            return part
 
-    def _upload_multipart_part(self, data: bytes, upload_id: str, bucket_name: str, key: str, part_number: int) -> Any:
         s3_info = self._get_upload_s3_info()
-        response = s3_info["s3_client"].upload_part(
-            Bucket=bucket_name, Key=key, PartNumber=part_number, UploadId=upload_id, Body=data
+        s3_exceptions = s3_info["s3_client"].exceptions
+
+        wrapped_file_operation = self.exponential_backoff_retry(
+            file_operation,
+            exceptions_to_raise=[s3_exceptions.NoSuchBucket],
         )
-        part = {"PartNumber": part_number, "ETag": response["ETag"]}
 
-        return part
+        return wrapped_file_operation()
+
+    def _s3_complete_multipart_upload(self, upload_id: str, bucket_name: str, key: str, parts: list) -> None:
+        def file_operation() -> None:
+            s3_info = self._get_upload_s3_info()
+            s3_info["s3_client"].complete_multipart_upload(
+                Bucket=bucket_name, Key=key, UploadId=upload_id, MultipartUpload={"Parts": parts}
+            )
 
-    def _complete_multipart_upload(self, upload_id: str, bucket_name: str, key: str, parts: list) -> None:
         s3_info = self._get_upload_s3_info()
-        s3_info["s3_client"].complete_multipart_upload(
-            Bucket=bucket_name, Key=key, UploadId=upload_id, MultipartUpload={"Parts": parts}
+        s3_exceptions = s3_info["s3_client"].exceptions
+
+        wrapped_file_operation = self.exponential_backoff_retry(
+            file_operation,
+            exceptions_to_raise=[s3_exceptions.NoSuchBucket],
         )
 
+        wrapped_file_operation()
+
     def _s3_multipart_upload(
         self,
         bucket_name: str,
         file_path: str,
         key: str,
         callback: Optional[Callable[[int], None]],
         chunk_size: int,
     ) -> None:
-        upload_id = self._initiate_multipart_upload(bucket_name, key)
+        upload_id = self._s3_initiate_multipart_upload(bucket_name, key)
 
         part_number = 1
         parts = []
 
         with open(file_path, "rb") as file:
             while True:
                 data = file.read(chunk_size)
                 if not data:
                     break
 
-                part = self._upload_multipart_part(data, upload_id, bucket_name, key, part_number)
+                part = self._s3_upload_multipart_part(data, upload_id, bucket_name, key, part_number)
                 parts.append(part)
                 part_number += 1
 
                 if callback:
                     callback(len(data))
 
-        self._complete_multipart_upload(upload_id, bucket_name, key, parts)
+        self._s3_complete_multipart_upload(upload_id, bucket_name, key, parts)
 
     def _s3_put_object(
         self, bucket_name: str, file_path: str, key: str, callback: Optional[Callable[[int], None]]
     ) -> None:
         with open(file_path, "rb") as file:
+
+            def file_operation() -> None:
+                s3_info = self._get_upload_s3_info()
+                s3_info["s3_client"].put_object(Bucket=bucket_name, Key=key, Body=file)
+
             s3_info = self._get_upload_s3_info()
-            s3_info["s3_client"].put_object(Bucket=bucket_name, Key=key, Body=file)
+            s3_exceptions = s3_info["s3_client"].exceptions
+
+            wrapped_file_operation = self.exponential_backoff_retry(
+                file_operation,
+                exceptions_to_raise=[s3_exceptions.NoSuchBucket],
+            )
+
+            wrapped_file_operation()
 
             if callback:
                 callback(os.path.getsize(file_path))
 
     def _s3_upload_file(
         self,
         bucket_name: str,
@@ -323,23 +348,28 @@
 
         if file_size > multipart_threshold:
             self._s3_multipart_upload(bucket_name, file_path, key, callback, chunk_size=multipart_threshold)
         else:
             self._s3_put_object(bucket_name, file_path, key, callback)
 
     def _upload_file(self, local_filepath: str, progress_bar: tqdm):
-        local_relative_filepath = os.path.relpath(local_filepath, self.local_root_directory_path)
-        s3_info = self._get_upload_s3_info()
-        s3_path = os.path.join(s3_info["s3_prefix"], local_relative_filepath)
-        if Util.is_windows():
-            s3_path = FileUtil.windows_to_unix_path(s3_path)
+        try:
+            local_relative_filepath = os.path.relpath(local_filepath, self.local_root_directory_path)
+            s3_info = self._get_upload_s3_info()
+            s3_path = os.path.join(s3_info["s3_prefix"], local_relative_filepath)
+            if Util.is_windows():
+                s3_path = FileUtil.windows_to_unix_path(s3_path)
 
-        self._s3_upload_file(
-            bucket_name=s3_info["s3_bucket"], file_path=local_filepath, key=s3_path, callback=progress_bar.update
-        )
+            self._s3_upload_file(
+                bucket_name=s3_info["s3_bucket"], file_path=local_filepath, key=s3_path, callback=progress_bar.update
+            )
+        except BaseException as exc:  # pylint: disable=broad-except
+            progress_bar.write(f"Failed to upload {local_filepath}.")
+            logging.error("Failed to upload %s.", local_filepath)
+            logging.exception(exc)
 
     def _get_s3_object_list(self) -> list[ObjectTypeDef]:
         s3_info = self._get_download_s3_info()
         response = s3_info["s3_client"].list_objects_v2(Bucket=s3_info["s3_bucket"], Prefix=s3_info["s3_prefix"])
 
         if "Contents" not in response:
             return []
@@ -384,26 +414,37 @@
             "s3_client": s3_client,
             "s3_bucket": s3_bucket,
             "s3_prefix": s3_prefix,
             "expires_at": expires_at,
         }
         return self.upload_s3_info
 
-    def _download_multipart_part(
+    def _s3_download_multipart_part(
         self, bucket_name: str, key: str, part_number: int, part_size: int, file_size: int
     ) -> bytes:
-        start_byte = (part_number - 1) * part_size
-        end_byte = min(part_number * part_size - 1, file_size)
-        range_header = f"bytes={start_byte}-{end_byte}"
+        def file_operation() -> bytes:
+            start_byte = (part_number - 1) * part_size
+            end_byte = min(part_number * part_size - 1, file_size)
+            range_header = f"bytes={start_byte}-{end_byte}"
+
+            s3_info = self._get_download_s3_info()
+            response = s3_info["s3_client"].get_object(Bucket=bucket_name, Key=key, Range=range_header)
+            part_data = response["Body"].read()
+
+            return part_data
 
         s3_info = self._get_download_s3_info()
-        response = s3_info["s3_client"].get_object(Bucket=bucket_name, Key=key, Range=range_header)
-        part_data = response["Body"].read()
+        s3_exceptions = s3_info["s3_client"].exceptions
+
+        wrapped_file_operation = self.exponential_backoff_retry(
+            file_operation,
+            exceptions_to_raise=[s3_exceptions.NoSuchKey, s3_exceptions.NoSuchBucket],
+        )
 
-        return part_data
+        return wrapped_file_operation()
 
     def _s3_download_file(
         self,
         bucket_name: str,
         key: str,
         local_path: str,
         file_size: int,
@@ -412,62 +453,70 @@
     ) -> None:
         total_parts = (file_size + part_size - 1) // part_size
 
         download_path = local_path + DOWNLOAD_FILE_EXTENSION
 
         with open(download_path, "wb") as file:
             for part_number in range(1, total_parts + 1):
-                part_data = self._download_multipart_part(bucket_name, key, part_number, part_size, file_size)
+                part_data = self._s3_download_multipart_part(bucket_name, key, part_number, part_size, file_size)
                 file.write(part_data)
 
                 if callback:
                     callback(len(part_data))
 
         os.rename(download_path, local_path)
 
     def _download_file(self, s3_object: ObjectTypeDef, progress_bar: tqdm):
-        if not AwsUtil.s3_object_is_directory(s3_object):
-            s3_info = self._get_download_s3_info()
-
-            local_filepath = self._get_local_filepath(s3_object, s3_info["s3_prefix"])
-
-            if FileUtil.include_exclude_allows_path(
-                os.path.relpath(local_filepath, self.local_root_directory_path),
-                self.cli_dict[INCLUDE_OUTPUT],
-                self.cli_dict[EXCLUDE_OUTPUT],
-            ) and self._should_download_file(local_filepath, s3_object):
-                os.makedirs(os.path.dirname(local_filepath), exist_ok=True)
-
+        try:
+            if not AwsUtil.s3_object_is_directory(s3_object):
                 s3_info = self._get_download_s3_info()
-                refreshed_s3_object = s3_info["s3_client"].get_object(Bucket=s3_info["s3_bucket"], Key=s3_object["Key"])
-                s3_object["ETag"] = refreshed_s3_object["ETag"]
+                local_filepath = self._get_local_filepath(s3_object, s3_info["s3_prefix"])
 
-                self._s3_download_file(
-                    bucket_name=s3_info["s3_bucket"],
-                    key=s3_object["Key"],
-                    local_path=local_filepath,
-                    file_size=s3_object["Size"],
-                    callback=progress_bar.update,
-                )
-
-                self._cache_file_data(local_filepath, s3_object)
-            else:
-                progress_bar.update(s3_object["Size"])
+                if FileUtil.include_exclude_allows_path(
+                    os.path.relpath(local_filepath, self.local_root_directory_path),
+                    self.cli_dict[INCLUDE_OUTPUT],
+                    self.cli_dict[EXCLUDE_OUTPUT],
+                ) and self._should_download_file(local_filepath, s3_object):
+                    os.makedirs(os.path.dirname(local_filepath), exist_ok=True)
+
+                    s3_info = self._get_download_s3_info()
+                    refreshed_s3_object = s3_info["s3_client"].get_object(
+                        Bucket=s3_info["s3_bucket"], Key=s3_object["Key"]
+                    )
+                    s3_object["ETag"] = refreshed_s3_object["ETag"]
+
+                    self._s3_download_file(
+                        bucket_name=s3_info["s3_bucket"],
+                        key=s3_object["Key"],
+                        local_path=local_filepath,
+                        file_size=s3_object["Size"],
+                        callback=progress_bar.update,
+                    )
+
+                    self._cache_file_data(local_filepath, s3_object)
+                else:
+                    progress_bar.update(s3_object["Size"])
+        except BaseException as exc:  # pylint: disable=broad-except
+            progress_bar.write(f"Failed to download {s3_object['Key']}.")
+            logging.error("Failed to download %s.", s3_object["Key"])
+            logging.exception(exc)
 
     def _load_cached_file_data(self):
         cached_file_data_filepath = os.path.join(
             self.local_root_directory_path, FOVUS_JOB_INFO_FOLDER, "cached_file_data.json"
         )
         if not os.path.isfile(cached_file_data_filepath):
             return {}
 
         try:
             with FileUtil.open(cached_file_data_filepath, "r") as cached_file_data_file:
                 return json.load(cached_file_data_file)
-        except Exception:  # pylint: disable=broad-except
+        except Exception as exc:  # pylint: disable=broad-except
+            logging.error("Failed to load cached file data.")
+            logging.exception(exc)
             return {}
 
     def _cache_file_data(self, local_filepath: str, s3_object: ObjectTypeDef):
         self.cached_file_data[s3_object["Key"]] = self._retrieve_file_data(local_filepath, s3_object)
         self._save_cached_file_data()
 
     def _save_cached_file_data(self):
```

## fovus/cli/cli_action_runner.py

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import os
 import shutil
 from http import HTTPStatus
 
 import pkg_resources  # type: ignore
 import requests
 from packaging import version
@@ -59,14 +60,15 @@
 
 class CliActionRunner:  # pylint: disable=too-few-public-methods
     def __init__(self, args_dict):
         self.args_dict = args_dict
 
     def run_actions(self):
         try:
+            logging.info("CLI Arguments: %s", self.args_dict)
             self._confirm_latest_version()
             self._run_actions()
         except StatusException as exception:
             print(exception)
 
     def _run_actions(self):
         self._confirm_nonconflicting_argument_sets(CONFLICTING_CLI_ARGUMENT_SETS)
@@ -335,15 +337,15 @@
         fovus_s3_adapter = FovusS3Adapter(fovus_api_adapter, self.args_dict, self.args_dict[JOB_FILE_ROOT_DIRECTORY])
         fovus_s3_adapter.download_files()
 
     def _create_missing_directories(self):
         print("Creating missing config directories (if any)")
         for directory in (PATH_TO_CONFIG_ROOT, PATH_TO_JOB_CONFIGS, PATH_TO_USER_CONFIGS, PATH_TO_JOB_LOGS):
             if not os.path.exists(os.path.expanduser(directory)):
-                os.makedirs(os.path.expanduser(directory))
+                os.makedirs(os.path.expanduser(directory), exist_ok=True)
 
     def _create_missing_empty_config_files(self):
         print("Creating missing empty config files (if any)")
         for config in FOVUS_PROVIDED_CONFIGS.values():
             empty_config_json_file_path = os.path.abspath(os.path.join(ROOT_DIR, config[PATH_TO_CONFIG_FILE_IN_REPO]))
             shutil.copy(empty_config_json_file_path, config[PATH_TO_CONFIG_FILE_LOCAL])
```

## fovus/cli/fovus_cli.py

```diff
@@ -1,40 +1,64 @@
 #!/usr/bin/env python3
+import logging
+import os
 import sys
-import traceback
+import time
 
 from fovus.cli.cli_action_runner import CliActionRunner
 from fovus.cli.fovus_cli_argument_parser import FovusCliArgumentParser
+from fovus.constants.cli_constants import PATH_TO_LOGS
+from fovus.constants.util_constants import UTF8
 
 OK_RETURN_STATUS = 0
 ERROR_RETURN_STATUS = 1
 
+BASIC_FORMATTER = logging.Formatter("%(asctime)s %(levelname)s %(message)s")
+
 
 def main():
     return_status = OK_RETURN_STATUS
-    debug = False
+
+    logger = logging.getLogger()
+
+    log_path = os.path.join(PATH_TO_LOGS, time.strftime("%Y-%m-%d_%H-%M-%S.log"))
+    os.makedirs(os.path.dirname(log_path), exist_ok=True)
+
+    file_handler = logging.FileHandler(log_path, mode="a", encoding=UTF8)
+    file_handler.setFormatter(BASIC_FORMATTER)
+
+    log_level = logging.INFO
+
     if "--debug" in sys.argv:
-        debug = True
         sys.argv.remove("--debug")
+        log_level = logging.DEBUG
+
+    logger.setLevel(log_level)
+    file_handler.setLevel(log_level)
+
+    logger.addHandler(file_handler)
+
     try:
         _main()
-    except Exception as exception:  # pylint: disable=broad-except
-        if debug:
-            print(traceback.format_exc())
-        else:
-            print(exception)
+    except Exception as exc:  # pylint: disable=broad-except
+        print(exc)
+        logging.critical("An unhandled exception occurred in main.")
+        logging.exception(exc)
         return_status = ERROR_RETURN_STATUS
     finally:
         return return_status  # pylint: disable=lost-exception
 
 
 def _main():
     parser = FovusCliArgumentParser()
     parser.parse_args()
     parser.merge_args_with_config()
     parser.update_overridden_configs()
-    cli_action_runner = CliActionRunner(parser.get_args_dict())
+
+    args = parser.get_args_dict()
+
+    cli_action_runner = CliActionRunner(args)
     cli_action_runner.run_actions()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

## fovus/constants/cli_constants.py

```diff
@@ -154,14 +154,15 @@
 GPU_INTERNAL_REPRESENTATION = "gpu"
 
 PASSWORD_ENVIRONMENT_VARIABLE_KEY = "FOVUS_CLI_PASSWORD"  # nosec
 PATH_TO_CONFIG_ROOT = os.path.join(os.path.expanduser("~"), ".fovus")
 PATH_TO_JOB_CONFIGS = os.path.join(PATH_TO_CONFIG_ROOT, "job_configs")
 PATH_TO_USER_CONFIGS = os.path.join(PATH_TO_CONFIG_ROOT, "user_configs")
 PATH_TO_JOB_LOGS = os.path.join(PATH_TO_CONFIG_ROOT, "job_logs")
+PATH_TO_LOGS = os.path.join(PATH_TO_CONFIG_ROOT, "logs")
 UNIX_OPEN = "open"
 WINDOWS_EXPLORER = "explorer"
 
 DEFAULT_USER_CONFIG_FILE_NAME = "FOVUS_default_user_config.json"
 DEFAULT_USER_CONFIG_FILE_PATH = os.path.join(PATH_TO_USER_CONFIGS, DEFAULT_USER_CONFIG_FILE_NAME)
 
 FOVUS_PROVIDED_CONFIGS_FOLDER_REPO = "fovus_provided_configs"
```

## Comparing `fovus-1.1.8.dist-info/LICENSE.txt` & `fovus-1.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fovus-1.1.8.dist-info/METADATA` & `fovus-1.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fovus
-Version: 1.1.8
+Version: 1.1.9
 Summary: The Fovus Python CLI
 Author: Fovus Corporation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3 >=1.28.36
 Requires-Dist: mypy-boto3-s3 >=1.28.36
```

## Comparing `fovus-1.1.8.dist-info/RECORD` & `fovus-1.1.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 fovus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/root_config.py,sha256=onsSNaAhzMvRK8o82IkASh4EVkyMxVMPBlUXcUq1Lcg,65
 fovus/adapter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/adapter/fovus_api_adapter.py,sha256=ISG6Ax0kEkIP9F61hhFhOcnGUNMQUZZn_c0L53f9yA0,26500
-fovus/adapter/fovus_s3_adapter.py,sha256=3ZF3fkh0TMAVM30eOaJPc8_CU5cY_Vui5OQoG6Q1p5I,19619
+fovus/adapter/fovus_s3_adapter.py,sha256=urCZGCbAPBMxz1DMFFoghyM2WvgCW0lYRARI4-7CoTY,21490
 fovus/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/cli/cli_action_runner.py,sha256=FApWPcUl6BFy4LEgrp2wJVPF75y7Kh1AtE2RE8SYhSo,15658
+fovus/cli/cli_action_runner.py,sha256=zfZqCc1ZSgEUODG17Q1GB5wIAbm9wNvibdivs45_KwY,15750
 fovus/cli/documenter.py,sha256=uzpu25Wd8YXirM7oQPLG3hqgAZa2_H_YPz0i522qxyo,161
-fovus/cli/fovus_cli.py,sha256=JGO28oDHjwO7E8-5f-di09eEmOVQbrfk8FrmLZkC-dk,997
+fovus/cli/fovus_cli.py,sha256=LcSQpRx6sBQzUGre9-Bypr_9dpRI4zrQf9a-ycfMxF4,1656
 fovus/cli/fovus_cli_argument_parser.py,sha256=vqckMSOhyepatQ6kSOzYG3eZR2bfZ62UFN_EGF22TgQ,31421
 fovus/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/config/config.py,sha256=7pE82qidwfnY9lczL-rFoPq6jFP5Gp1LL5dGRZ2qeNY,840
 fovus/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/constants/benchmark_constants.py,sha256=9V-T9Sa1lGAPRYU_Jic7FpOvxBQ1haukwJ-dTLBz9og,1658
 fovus/constants/cli_action_runner_constants.py,sha256=PQkh9gznZCcc-cNtddO748WkLgPh6Rms9ug6ib0E7CE,485
-fovus/constants/cli_constants.py,sha256=0OaqM31p59RzzkuRzBujTAbu-BXcbsgiDOwAxXp9fBA,9584
+fovus/constants/cli_constants.py,sha256=YwPAOBJ9WowJnpqK3SCqdfcrKw0dKE0O9h_ySK-tB8M,9641
 fovus/constants/fovus_api_constants.py,sha256=qP-nzSI5u7gsmXgJx_Jhr4v4uj14XaUYqEzKhwgm2PY,2001
 fovus/constants/util_constants.py,sha256=tcIzvskdO_N9aYrNLLoqoASG76AVeiuexcfzG-IouPQ,194
 fovus/exception/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/exception/status_code_exception.py,sha256=HXfQ6E3gGSEg2dUxS6ccPN5kAgCC33nVzCuAy_zxN7o,291
 fovus/exception/system_exception.py,sha256=lzoDivDErUE47Cz3v9U1AhbzI4MQHTeYbvmn02myOHA,183
 fovus/exception/user_exception.py,sha256=Un3pq8s1a7gXdZ8MoHNhxE5xZz_fO4cBy4lE2n7uEzg,174
 fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json,sha256=xe3e-qZuKR_7gHL5vg3cb-NMx9liwNJxXp-QyDjkLwY,1191
@@ -34,13 +34,13 @@
 fovus/util/file_util.py,sha256=Qok_f2i7FTtTDA5vAPlQ0wUXvJezN_8uVM7VG_Xgs_k,9310
 fovus/util/fovus_api_util.py,sha256=7drvoKaRvrP7kTGZVgAeyoP1zjxHshlDeim71DtXaio,15335
 fovus/util/fovus_cli_argument_parser_util.py,sha256=XRLoaMCulYzh_Ew85imIwcZwb-8bEYT_gIpiodjwOuo,1956
 fovus/util/fovus_s3_adapter_util.py,sha256=T_gtVF1QDaWBhozsSyPa886zsCTcz5sdxyZJSJKDm4g,1198
 fovus/util/util.py,sha256=mjpVD723Uasdpq03TYGkn41NMmMG-0nO-HRXIzqmjFE,1240
 fovus/validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/validator/fovus_api_validator.py,sha256=hF6weIoyMh0FlpFWAaF8kUnMa3MiWz-F0m5dHitovK8,4793
-fovus-1.1.8.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
-fovus-1.1.8.dist-info/METADATA,sha256=NR2EAhCZA3xZ8D7FnmPmj5do5xdS72zIk2UYXHok06w,12427
-fovus-1.1.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-fovus-1.1.8.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
-fovus-1.1.8.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
-fovus-1.1.8.dist-info/RECORD,,
+fovus-1.1.9.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
+fovus-1.1.9.dist-info/METADATA,sha256=Vg4vXgaNhbfrAsKc02mtjwf-tuDhSuHKE9J7tIyDfnM,12427
+fovus-1.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+fovus-1.1.9.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
+fovus-1.1.9.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
+fovus-1.1.9.dist-info/RECORD,,
```

