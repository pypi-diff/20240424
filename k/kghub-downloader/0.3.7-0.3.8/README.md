# Comparing `tmp/kghub_downloader-0.3.7.tar.gz` & `tmp/kghub_downloader-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kghub_downloader-0.3.7.tar", max compression
+gzip compressed data, was "kghub_downloader-0.3.8.tar", max compression
```

## Comparing `kghub_downloader-0.3.7.tar` & `kghub_downloader-0.3.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4464 2024-03-22 00:26:33.173953 kghub_downloader-0.3.7/docs/index.md
--rw-r--r--   0        0        0    13772 2024-03-22 00:26:33.173953 kghub_downloader-0.3.7/kghub_downloader/download_utils.py
--rw-r--r--   0        0        0     1019 2024-03-22 00:26:33.173953 kghub_downloader-0.3.7/kghub_downloader/main.py
--rw-r--r--   0        0        0      926 2024-03-22 00:26:46.878065 kghub_downloader-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     5471 1970-01-01 00:00:00.000000 kghub_downloader-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     4981 2024-04-24 21:37:31.165563 kghub_downloader-0.3.8/docs/index.md
+-rw-r--r--   0        0        0    13772 2024-04-24 21:37:31.165563 kghub_downloader-0.3.8/kghub_downloader/download_utils.py
+-rw-r--r--   0        0        0     1019 2024-04-24 21:37:31.165563 kghub_downloader-0.3.8/kghub_downloader/main.py
+-rw-r--r--   0        0        0      931 2024-04-24 21:37:44.021506 kghub_downloader-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     5972 1970-01-01 00:00:00.000000 kghub_downloader-0.3.8/PKG-INFO
```

### Comparing `kghub_downloader-0.3.7/docs/index.md` & `kghub_downloader-0.3.8/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 # KG-Hub Downloader
 
-| [Documentation](https://monarch-initiative.github.io/kghub-downloader) |
+| [Documentation](https://monarch-initiative.github.io/kghub-downloader) | [Repository](https://github.com/monarch-initiative/kghub-downloader) | [PyPI](https://pypi.org/project/kghub-downloader) |
 
 ### Overview
 
 This is a configuration based file caching downloader with initial support for http requests & queries against elasticsearch.
 
 ### Installation
 
 KGHub Downloader is available to install via pip:
+
 ```
 pip install kghub-downloader
 ```
 
-### Configure 
+### Configure
 
 The downloader requires a YAML file which contains a list of target URLs to download, and local names to save those downloads.  
 For an example, see [example/download.yaml](example/download.yaml)
 
 Available options are:
-- \***url**: The URL to download from. Currently supported:  
+
+- \***url**: The URL to download from. Currently supported:
   - `http(s)`
   - `ftp`
     - with `glob:` option to download files with specific extensions (only with ftp as of now and looks recursively).
   - Google Cloud Storage (`gs://`)
   - Google Drive (`gdrive://` or https://drive.google.com/...). The file must be publicly accessible.
   - Amazon AWS S3 bucket (`s3://`)
 - **local_name**: The name to save the file as locally
 - **tag**: A tag to use to filter downloads
 - **api**: The API to use to download the file. Currently supported: `elasticsearch`
-- elastic search options  
+- elastic search options
   - **query_file**: The file containing the query to run against the index
   - **index**: The elastic search index for query
 
 > \* Note:  
->  Google Cloud Storage URLs require that you have set up your credentials as described [here](https://cloud.google.com/artifact-registry/docs/python/authentication#keyring-user). You must:  
-> - [create a service account](https://cloud.google.com/iam/docs/service-accounts-create)  
-> - [add the service account to the relevant bucket](https://cloud.google.com/storage/docs/access-control/using-iam-permissions#bucket-iam) and  
+>  Google Cloud Storage URLs require that you have set up your credentials as described [here](https://cloud.google.com/artifact-registry/docs/python/authentication#keyring-user). You must:
+>
+> - [create a service account](https://cloud.google.com/iam/docs/service-accounts-create)
+> - [add the service account to the relevant bucket](https://cloud.google.com/storage/docs/access-control/using-iam-permissions#bucket-iam) and
 > - [download a JSON key](https://cloud.google.com/iam/docs/keys-create-delete) for that service account.  
->  Then, set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to point to that file.
+>   Then, set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to point to that file.
 >
 > Mirorring local files to Amazon AWS S3 bucket requires the following:
->  - [Create an AWS account](https://portal.aws.amazon.com/)
->  - [Create an IAM user in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html): This enables getting the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` needed for authentication. These two should be stored as environment variables in the user's system.
->  - [Create an S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html): This will be the destination for pushing local files.
+>
+> - [Create an AWS account](https://portal.aws.amazon.com/)
+> - [Create an IAM user in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html): This enables getting the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` needed for authentication. These two should be stored as environment variables in the user's system.
+> - [Create an S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html): This will be the destination for pushing local files.
+
+You can also include any secrets like API keys you have set as environment variables using `{VARIABLE_NAME}`, for example:
 
-You can also include any secrets like API keys you have set as environment variables using `{VARIABLE_NAME}`, for example:  
 ```yaml
 ---
 - url: "https://example.com/myfancyfile.json?key={YOUR_SECRET}"
   localname: myfancyfile.json
 ```
-Note: `YOUR_SECRET` *MUST* as an environment variable, and be sure to include the {curly braces} in the url string.
+
+Note: `YOUR_SECRET` _MUST_ as an environment variable, and be sure to include the {curly braces} in the url string.
 
 ### Usage
 
 Downloader can be used directly in Python or via command line
 
 #### In Python
 
@@ -63,38 +69,39 @@
 from kghub_downloader.download_utils import download_from_yaml
 
 download_from_yaml(yaml_file="download.yaml", output_dir="data")
 ```
 
 #### Command Line
 
+To download files listed in a download.yaml file:
+
 ```bash
 $ downloader [OPTIONS] ARGS
 ```
-╰ Download files listed in a download.yaml file
-
-| OPTIONS | | 
-| --- | --- |
-| yaml_file | A string pointing to the download.yaml file, to be parsed for things to download.<br>Defaults to `./download.yaml` |
-| ignore_cache | Ignore cache and download files even if they exist [false] |
-| snippet_only | Downloads only the first 5 kB of each uncompressed source, for testing and file checks |
-| tags | Limit to only downloads with this tag |
-| mirror | Remote storage URL to mirror download to. Supported buckets: Google Cloud Storage |
 
-
-| ARGUMENTS | | 
-| --- | --- |
-| output_dir | A string pointing to where to write out downloaded files. |
+| OPTIONS      |                                                                                                       |
+| ------------ | ----------------------------------------------------------------------------------------------------- |
+| yaml_file    | Path to the download.yaml file, to be parsed for things to download.<br>Defaults to `./download.yaml` |
+| ignore_cache | Ignore cache and download files even if they exist (Default `False`)                                  |
+| snippet_only | Downloads only the first 5 kB of each uncompressed source, for testing and file checks                |
+| tags         | Limit to only downloads with this tag                                                                 |
+| mirror       | Remote storage URL to upload downloaded files to.<br/>Supported buckets: Google Cloud Storage         |
+
+| ARGUMENTS  |                                 |
+| ---------- | ------------------------------- |
+| output_dir | Where to save downloaded files. |
 
 Examples:
+
 ```bash
 $ downloader --output_dir example_output --tags zfin_gene_to_phenotype example.yaml
 $ downloader --output_dir example_output --mirror gs://your-bucket/desired/directory
 
-# Note that if your YAML file is named `download.yaml`, 
+# Note that if your YAML file is named `download.yaml`,
 # the argument can be omitted from the CLI call.
 $ downloader --output_dir example_output
 ```
 
 ### Development
 
 #### Install
@@ -107,8 +114,8 @@
 
 #### Run tests
 
 ```bash
 poetry run pytest
 ```
 
-NOTE: The tests require gcloud credentials to be set up as described above, using the monarch github actions service account.
+NOTE: The tests require gcloud credentials to be set up as described above, using the Monarch github actions service account.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kghub_downloader-0.3.7/kghub_downloader/download_utils.py` & `kghub_downloader-0.3.8/kghub_downloader/download_utils.py`

 * *Files identical despite different names*

### Comparing `kghub_downloader-0.3.7/kghub_downloader/main.py` & `kghub_downloader-0.3.8/kghub_downloader/main.py`

 * *Files identical despite different names*

### Comparing `kghub_downloader-0.3.7/pyproject.toml` & `kghub_downloader-0.3.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "kghub-downloader"
-version = "v0.3.7"
+version = "v0.3.8"
 description = "Downloads and caches files for knowledge graph ETL"
 authors = ["The Monarch Initiative <info@monarchinitiative.org>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 downloader = "kghub_downloader.main:typer_app"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8, <4.0"
 elasticsearch = ">7.0, <9.0"
 compress-json = ">1.0, <2.0"
 PyYAML = ">5.0,<7.0"
 tqdm = ">=4.62.3"
 google-cloud-storage = "^2.1.0"
-typer = "^0.7.0"
-mkdocs = "^1.4.0"
-mkdocs-material = "^8.5.6"
+typer ="^0.12.3"
+mkdocs = ">=1.4"
+mkdocs-material = ">=9.5"
 mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 gdown = ">=4.7.1"
 boto3 = ">=1.34.35"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
```

### Comparing `kghub_downloader-0.3.7/PKG-INFO` & `kghub_downloader-0.3.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kghub-downloader
-Version: 0.3.7
+Version: 0.3.8
 Summary: Downloads and caches files for knowledge graph ETL
 Author: The Monarch Initiative
 Author-email: info@monarchinitiative.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,75 +13,81 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>5.0,<7.0)
 Requires-Dist: boto3 (>=1.34.35)
 Requires-Dist: compress-json (>1.0,<2.0)
 Requires-Dist: elasticsearch (>7.0,<9.0)
 Requires-Dist: gdown (>=4.7.1)
 Requires-Dist: google-cloud-storage (>=2.1.0,<3.0.0)
-Requires-Dist: mkdocs (>=1.4.0,<2.0.0)
-Requires-Dist: mkdocs-material (>=8.5.6,<9.0.0)
+Requires-Dist: mkdocs (>=1.4)
+Requires-Dist: mkdocs-material (>=9.5)
 Requires-Dist: mkdocstrings[python] (>=0.20.0,<0.21.0)
 Requires-Dist: tqdm (>=4.62.3)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # KG-Hub Downloader
 
-| [Documentation](https://monarch-initiative.github.io/kghub-downloader) |
+| [Documentation](https://monarch-initiative.github.io/kghub-downloader) | [Repository](https://github.com/monarch-initiative/kghub-downloader) | [PyPI](https://pypi.org/project/kghub-downloader) |
 
 ### Overview
 
 This is a configuration based file caching downloader with initial support for http requests & queries against elasticsearch.
 
 ### Installation
 
 KGHub Downloader is available to install via pip:
+
 ```
 pip install kghub-downloader
 ```
 
-### Configure 
+### Configure
 
 The downloader requires a YAML file which contains a list of target URLs to download, and local names to save those downloads.  
 For an example, see [example/download.yaml](example/download.yaml)
 
 Available options are:
-- \***url**: The URL to download from. Currently supported:  
+
+- \***url**: The URL to download from. Currently supported:
   - `http(s)`
   - `ftp`
     - with `glob:` option to download files with specific extensions (only with ftp as of now and looks recursively).
   - Google Cloud Storage (`gs://`)
   - Google Drive (`gdrive://` or https://drive.google.com/...). The file must be publicly accessible.
   - Amazon AWS S3 bucket (`s3://`)
 - **local_name**: The name to save the file as locally
 - **tag**: A tag to use to filter downloads
 - **api**: The API to use to download the file. Currently supported: `elasticsearch`
-- elastic search options  
+- elastic search options
   - **query_file**: The file containing the query to run against the index
   - **index**: The elastic search index for query
 
 > \* Note:  
->  Google Cloud Storage URLs require that you have set up your credentials as described [here](https://cloud.google.com/artifact-registry/docs/python/authentication#keyring-user). You must:  
-> - [create a service account](https://cloud.google.com/iam/docs/service-accounts-create)  
-> - [add the service account to the relevant bucket](https://cloud.google.com/storage/docs/access-control/using-iam-permissions#bucket-iam) and  
+>  Google Cloud Storage URLs require that you have set up your credentials as described [here](https://cloud.google.com/artifact-registry/docs/python/authentication#keyring-user). You must:
+>
+> - [create a service account](https://cloud.google.com/iam/docs/service-accounts-create)
+> - [add the service account to the relevant bucket](https://cloud.google.com/storage/docs/access-control/using-iam-permissions#bucket-iam) and
 > - [download a JSON key](https://cloud.google.com/iam/docs/keys-create-delete) for that service account.  
->  Then, set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to point to that file.
+>   Then, set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to point to that file.
 >
 > Mirorring local files to Amazon AWS S3 bucket requires the following:
->  - [Create an AWS account](https://portal.aws.amazon.com/)
->  - [Create an IAM user in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html): This enables getting the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` needed for authentication. These two should be stored as environment variables in the user's system.
->  - [Create an S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html): This will be the destination for pushing local files.
+>
+> - [Create an AWS account](https://portal.aws.amazon.com/)
+> - [Create an IAM user in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html): This enables getting the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` needed for authentication. These two should be stored as environment variables in the user's system.
+> - [Create an S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html): This will be the destination for pushing local files.
+
+You can also include any secrets like API keys you have set as environment variables using `{VARIABLE_NAME}`, for example:
 
-You can also include any secrets like API keys you have set as environment variables using `{VARIABLE_NAME}`, for example:  
 ```yaml
 ---
 - url: "https://example.com/myfancyfile.json?key={YOUR_SECRET}"
   localname: myfancyfile.json
 ```
-Note: `YOUR_SECRET` *MUST* as an environment variable, and be sure to include the {curly braces} in the url string.
+
+Note: `YOUR_SECRET` _MUST_ as an environment variable, and be sure to include the {curly braces} in the url string.
 
 ### Usage
 
 Downloader can be used directly in Python or via command line
 
 #### In Python
 
@@ -89,38 +95,39 @@
 from kghub_downloader.download_utils import download_from_yaml
 
 download_from_yaml(yaml_file="download.yaml", output_dir="data")
 ```
 
 #### Command Line
 
+To download files listed in a download.yaml file:
+
 ```bash
 $ downloader [OPTIONS] ARGS
 ```
-╰ Download files listed in a download.yaml file
-
-| OPTIONS | | 
-| --- | --- |
-| yaml_file | A string pointing to the download.yaml file, to be parsed for things to download.<br>Defaults to `./download.yaml` |
-| ignore_cache | Ignore cache and download files even if they exist [false] |
-| snippet_only | Downloads only the first 5 kB of each uncompressed source, for testing and file checks |
-| tags | Limit to only downloads with this tag |
-| mirror | Remote storage URL to mirror download to. Supported buckets: Google Cloud Storage |
-
 
-| ARGUMENTS | | 
-| --- | --- |
-| output_dir | A string pointing to where to write out downloaded files. |
+| OPTIONS      |                                                                                                       |
+| ------------ | ----------------------------------------------------------------------------------------------------- |
+| yaml_file    | Path to the download.yaml file, to be parsed for things to download.<br>Defaults to `./download.yaml` |
+| ignore_cache | Ignore cache and download files even if they exist (Default `False`)                                  |
+| snippet_only | Downloads only the first 5 kB of each uncompressed source, for testing and file checks                |
+| tags         | Limit to only downloads with this tag                                                                 |
+| mirror       | Remote storage URL to upload downloaded files to.<br/>Supported buckets: Google Cloud Storage         |
+
+| ARGUMENTS  |                                 |
+| ---------- | ------------------------------- |
+| output_dir | Where to save downloaded files. |
 
 Examples:
+
 ```bash
 $ downloader --output_dir example_output --tags zfin_gene_to_phenotype example.yaml
 $ downloader --output_dir example_output --mirror gs://your-bucket/desired/directory
 
-# Note that if your YAML file is named `download.yaml`, 
+# Note that if your YAML file is named `download.yaml`,
 # the argument can be omitted from the CLI call.
 $ downloader --output_dir example_output
 ```
 
 ### Development
 
 #### Install
@@ -133,8 +140,9 @@
 
 #### Run tests
 
 ```bash
 poetry run pytest
 ```
 
-NOTE: The tests require gcloud credentials to be set up as described above, using the monarch github actions service account.
+NOTE: The tests require gcloud credentials to be set up as described above, using the Monarch github actions service account.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

