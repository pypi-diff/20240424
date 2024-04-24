# Comparing `tmp/kso_utils-0.2.5.tar.gz` & `tmp/kso_utils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kso_utils-0.2.5.tar", max compression
+gzip compressed data, was "kso_utils-0.2.6.tar", max compression
```

## Comparing `kso_utils-0.2.5.tar` & `kso_utils-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35126 2023-09-21 14:24:50.986126 kso_utils-0.2.5/LICENSE
--rw-r--r--   0        0        0    14312 2024-04-02 13:24:27.140946 kso_utils-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996729 kso_utils-0.2.5/kso_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996795 kso_utils-0.2.5/kso_utils/db_starter/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-02 13:24:18.424978 kso_utils-0.2.5/kso_utils/db_starter/cdn_projects_list.csv
--rw-r--r--   0        0        0     1461 2024-02-28 09:49:51.234739 kso_utils-0.2.5/kso_utils/db_starter/projects_list.csv
--rw-r--r--   0        0        0     1994 2024-04-02 13:24:18.425126 kso_utils-0.2.5/kso_utils/db_starter/schema.py
--rw-r--r--   0        0        0    18574 2024-04-24 09:19:37.426261 kso_utils-0.2.5/kso_utils/db_utils.py
--rw-r--r--   0        0        0     6741 2024-04-02 13:24:18.426034 kso_utils-0.2.5/kso_utils/frame_utils.py
--rw-r--r--   0        0        0     4091 2023-09-22 19:06:03.217864 kso_utils-0.2.5/kso_utils/general.py
--rw-r--r--   0        0        0    13317 2024-04-02 13:24:18.426336 kso_utils-0.2.5/kso_utils/koster_utils.py
--rw-r--r--   0        0        0    31563 2024-04-02 13:24:18.426758 kso_utils-0.2.5/kso_utils/movie_utils.py
--rw-r--r--   0        0        0    97323 2024-04-24 09:19:15.263961 kso_utils-0.2.5/kso_utils/project.py
--rw-r--r--   0        0        0     3606 2024-04-02 13:24:18.428216 kso_utils-0.2.5/kso_utils/project_utils.py
--rw-r--r--   0        0        0    14924 2024-04-02 13:24:18.428542 kso_utils-0.2.5/kso_utils/server_utils.py
--rw-r--r--   0        0        0     6295 2024-04-02 13:24:18.429109 kso_utils-0.2.5/kso_utils/sgu_utils.py
--rw-r--r--   0        0        0    10031 2024-04-02 13:24:18.429517 kso_utils-0.2.5/kso_utils/spyfish_utils.py
--rw-r--r--   0        0        0    13795 2024-04-11 09:53:06.799605 kso_utils-0.2.5/kso_utils/video_reader.py
--rw-r--r--   0        0        0    76147 2024-04-02 13:24:18.430796 kso_utils-0.2.5/kso_utils/widgets.py
--rw-r--r--   0        0        0    81215 2024-04-03 13:05:07.486948 kso_utils-0.2.5/kso_utils/yolo_utils.py
--rw-r--r--   0        0        0     3347 2023-09-21 14:24:50.998838 kso_utils-0.2.5/kso_utils/zenodo_utils.py
--rw-r--r--   0        0        0    85468 2024-04-02 13:24:18.432485 kso_utils-0.2.5/kso_utils/zooniverse_utils.py
--rw-r--r--   0        0        0     2535 2024-04-24 09:20:18.561032 kso_utils-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    15784 1970-01-01 00:00:00.000000 kso_utils-0.2.5/setup.py
--rw-r--r--   0        0        0    15879 1970-01-01 00:00:00.000000 kso_utils-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35126 2023-09-21 14:24:50.986126 kso_utils-0.2.6/LICENSE
+-rw-r--r--   0        0        0    14312 2024-04-02 13:24:27.140946 kso_utils-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996729 kso_utils-0.2.6/kso_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996795 kso_utils-0.2.6/kso_utils/db_starter/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-02 13:24:18.424978 kso_utils-0.2.6/kso_utils/db_starter/cdn_projects_list.csv
+-rw-r--r--   0        0        0     1461 2024-02-28 09:49:51.234739 kso_utils-0.2.6/kso_utils/db_starter/projects_list.csv
+-rw-r--r--   0        0        0     1995 2024-04-24 12:05:24.834909 kso_utils-0.2.6/kso_utils/db_starter/schema.py
+-rw-r--r--   0        0        0    18574 2024-04-24 09:19:37.426261 kso_utils-0.2.6/kso_utils/db_utils.py
+-rw-r--r--   0        0        0     6741 2024-04-02 13:24:18.426034 kso_utils-0.2.6/kso_utils/frame_utils.py
+-rw-r--r--   0        0        0     4091 2023-09-22 19:06:03.217864 kso_utils-0.2.6/kso_utils/general.py
+-rw-r--r--   0        0        0    13317 2024-04-02 13:24:18.426336 kso_utils-0.2.6/kso_utils/koster_utils.py
+-rw-r--r--   0        0        0    31563 2024-04-02 13:24:18.426758 kso_utils-0.2.6/kso_utils/movie_utils.py
+-rw-r--r--   0        0        0    97323 2024-04-24 09:19:15.263961 kso_utils-0.2.6/kso_utils/project.py
+-rw-r--r--   0        0        0     3606 2024-04-02 13:24:18.428216 kso_utils-0.2.6/kso_utils/project_utils.py
+-rw-r--r--   0        0        0    14924 2024-04-02 13:24:18.428542 kso_utils-0.2.6/kso_utils/server_utils.py
+-rw-r--r--   0        0        0     6295 2024-04-02 13:24:18.429109 kso_utils-0.2.6/kso_utils/sgu_utils.py
+-rw-r--r--   0        0        0    10031 2024-04-02 13:24:18.429517 kso_utils-0.2.6/kso_utils/spyfish_utils.py
+-rw-r--r--   0        0        0    13795 2024-04-11 09:53:06.799605 kso_utils-0.2.6/kso_utils/video_reader.py
+-rw-r--r--   0        0        0    76147 2024-04-02 13:24:18.430796 kso_utils-0.2.6/kso_utils/widgets.py
+-rw-r--r--   0        0        0    81215 2024-04-03 13:05:07.486948 kso_utils-0.2.6/kso_utils/yolo_utils.py
+-rw-r--r--   0        0        0     3347 2023-09-21 14:24:50.998838 kso_utils-0.2.6/kso_utils/zenodo_utils.py
+-rw-r--r--   0        0        0    85468 2024-04-02 13:24:18.432485 kso_utils-0.2.6/kso_utils/zooniverse_utils.py
+-rw-r--r--   0        0        0     2535 2024-04-24 12:05:47.242910 kso_utils-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    15784 1970-01-01 00:00:00.000000 kso_utils-0.2.6/setup.py
+-rw-r--r--   0        0        0    15879 1970-01-01 00:00:00.000000 kso_utils-0.2.6/PKG-INFO
```

### Comparing `kso_utils-0.2.5/LICENSE` & `kso_utils-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/README.md` & `kso_utils-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/db_starter/cdn_projects_list.csv` & `kso_utils-0.2.6/kso_utils/db_starter/cdn_projects_list.csv`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/db_starter/projects_list.csv` & `kso_utils-0.2.6/kso_utils/db_starter/projects_list.csv`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/db_starter/schema.py` & `kso_utils-0.2.6/kso_utils/db_starter/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 filename text NOT NULL,
 created_on datetime NULL,
 fps real NULL,
 duration datetime NULL,
 sampling_start real NULL,
 sampling_end real NULL,
 author text NULL,
-site_id text NULL,
+siteName text NULL,
 fpath text NULL,
 UNIQUE (filename),
 FOREIGN KEY (site_id) REFERENCES sites (id)
 );
 
 CREATE TABLE IF NOT EXISTS photos
 (
```

### Comparing `kso_utils-0.2.5/kso_utils/db_utils.py` & `kso_utils-0.2.6/kso_utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/frame_utils.py` & `kso_utils-0.2.6/kso_utils/frame_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/general.py` & `kso_utils-0.2.6/kso_utils/general.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/koster_utils.py` & `kso_utils-0.2.6/kso_utils/koster_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/movie_utils.py` & `kso_utils-0.2.6/kso_utils/movie_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/project.py` & `kso_utils-0.2.6/kso_utils/project.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/project_utils.py` & `kso_utils-0.2.6/kso_utils/project_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/server_utils.py` & `kso_utils-0.2.6/kso_utils/server_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/sgu_utils.py` & `kso_utils-0.2.6/kso_utils/sgu_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/spyfish_utils.py` & `kso_utils-0.2.6/kso_utils/spyfish_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/video_reader.py` & `kso_utils-0.2.6/kso_utils/video_reader.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/widgets.py` & `kso_utils-0.2.6/kso_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/yolo_utils.py` & `kso_utils-0.2.6/kso_utils/yolo_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/zenodo_utils.py` & `kso_utils-0.2.6/kso_utils/zenodo_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/kso_utils/zooniverse_utils.py` & `kso_utils-0.2.6/kso_utils/zooniverse_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.5/pyproject.toml` & `kso_utils-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kso_utils"
-version = "0.2.5"
+version = "0.2.6"
 description = "A package containing utility scripts for use with KSO analysis notebooks."
 authors = ["Jurie Germishuys <jurie.germishuys@combine.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "kso_utils"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kso_utils-0.2.5/setup.py` & `kso_utils-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'split-folders==0.5.1',
  'tqdm==4.64.1',
  'ultralytics==8.0.200',
  'wandb==0.13.2']
 
 setup_kwargs = {
     'name': 'kso-utils',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A package containing utility scripts for use with KSO analysis notebooks.',
     'long_description': '# KSO System\n\nThe Koster Seafloor Observatory is an open-source, citizen science and machine learning approach to analyse subsea movies.\n\n<!-- PROJECT SHIELDS -->\n<!--\n*** I\'m using markdown "reference style" links for readability.\n*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).\n*** See the bottom of this document for the declaration of the reference variables\n*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.\n*** https://www.markdownguide.org/basic-syntax/#reference-style-links\n-->\n[![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n[![GPL License][license-shield]][license-url]\n\n### KSO overview\nThe KSO system has been developed to:\n* move and process underwater footage and its associated data (e.g. location, date, sampling device).\n* make this data available to citizen scientists in Zooniverse to annotate the data.\n* train and evaluate machine learning models (customise [Yolov5][YoloV5] or [Yolov8][YoloV8] models).\n  \n![koster_info_diag][high-level-overview]\n\nThe system is built around a series of easy-to-use [Jupyter Notebooks][Jupyter_site]. Each notebook allows users to perform a specific task of the system (e.g. upload footage to the citizen science platform or analyse the classified data).\n\nUsers can run these notebooks via Google Colab (by clicking on the Colab links in the table below), locally or on a High-Performance Computer environment.\n\n### Notebooks\n| Name                                              | Description                                                                                 | Try it!  | \n| ------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------|\n| 1. Check footage and metadata                     | Check format and contents of footage and sites, media and species csv files                 | [![Open In Colab][colablogo]][colab_tut_1] [![binder][binderlogo]][binder_tut] | \n| 2. Upload new media to the system*                | Upload new underwater media to the cloud/server and update the csv files                    | WIP | \n| 3. Upload clips to Zooniverse                     | Prepare original footage and upload short clips to Zooniverse                               | [![Open In Colab][colablogo]][colab_tut_3] [![binder][binderlogo]][binder_tut] |\n| 4. Upload frames to Zooniverse                    | Extract frames of interest from the original footage and upload them to Zooniverse              | [![Open In Colab][colablogo]][colab_tut_4] [![binder][binderlogo]][binder_tut] |\n| 5. Train ML models                                | Prepare the training and test data, set model parameters and train models                   | [![Open In Colab][colablogo]][colab_tut_5] [![binder][binderlogo]][binder_tut] | \n| 6. Evaluate ML models                            | Use ecologically relevant metrics to test the models                                        | [![Open In Colab][colablogo]][colab_tut_6] [![binder][binderlogo]][binder_tut]   |\n| 7. Publish ML models                               | Publish the model to a public repository                                                   | [![Open In Colab][colablogo]][colab_tut_7] [![binder][binderlogo]][binder_tut]  | \n| 8. Analyse Zooniverse classifications             | Pull and analyse up-to-date classifications from Zooniverse and export observations to GBIF             | [![Open In Colab][colablogo]][colab_tut_8] [![binder][binderlogo]][binder_tut] |\n| 9. Run ML models on footage                      | Automatically classify new footage and export observations to GBIF                                                          | [![Open In Colab][colablogo]][colab_tut_9] [![binder][binderlogo]][binder_tut] |\n\n  \n\\* Project-specific notebook\n\n## Local Installation\n\n### Docker Installation\n#### Requirements\n* [Docker](https://www.docker.com/products/docker-desktop/)\n\n#### Pull KSO Docker image\n```\nBash\ndocker pull ghcr.io/ocean-data-factory-sweden/kso:dev\n```\n\n### Conda Installation\n#### Requirements\n* [Python 3.8](https://www.python.org/)\n* [Anaconda](https://docs.anaconda.com/anaconda/install/index.html)\n* [GIT](https://git-scm.com/downloads)\n\n#### Download this repository\nClone this repository using\n```python\ngit clone https://github.com/ocean-data-factory-sweden/kso.git\n``` \n\n#### Prepare your system\nDepending on your system (Windows/Linux/MacOS), you might need to install some extra tools. If this is the case, you will get a message about what you need to install in the next steps. \nFor example, [Microsoft Build Tools C++][Microsoft_C++] with a version higher than 14.0 is required for Windows systems.\n\n#### Set up the environment with Conda\n1. Open the Anaconda Prompt\n2. Navigate to the folder where you have cloned the repository or unzipped the manually downloaded repository. Then go into the kso folder.\n```\ncd kso\n```\n\n3. Create an Anaconda environment with Python 3.8. Remember to change the name env.\n```\nconda create -n <name env> python=3.8\n```\n\n4. Enter the environment: \n```\nconda activate <name env>\n```\n\n5. Specify your GPU details.\n\n  5a. Find out the [pytorch][pytorch] installation you need. Navigate to the system options (example below) and select your device/platform details.\n  <div style="text-align: center;">\n    <img src="https://github.com/ocean-data-factory-sweden/kso/blob/dev/assets/cuda_gpu_example_requirements.png?raw=true" alt="CUDA Requirements" width="450" height="150">\n  </div>\n  \n  5b. Add the recommended command to the KSO\'s gpu_requirements_user.txt file.\n\n6. Install all the requirements:\n```\npip install -r requirements.txt -r gpu_requirements_user.txt\n```\n\n## Cloudina \nCloudina is a hosted version of KSO (powered by JupyterHub) on NAISS Science Cloud. It allows users to scale and automate larger workflows using a powerful processing backend. This is currently an invitation-only service. To access the platform, please contact jurie.germishuys[at]combine.se.\n\nThe current portals are accessible as:\n1. Console (object storage) - [storage][cdn_bucket]\n2. Album (JupyterHub) - [notebooks][cdn_album]\n3. Vendor (MLFlow) - [mlflow][cdn_vendor]\n\n\n## Starting a new project\nTo start a new project you will need to:\n1. Create initial information for the database: Input the information about the underwater footage files, sites and species of interest. You can use a [template of the csv files](https://drive.google.com/file/d/1PZGRoSY_UpyLfMhRphMUMwDXw4yx1_Fn/view?usp=sharing) and move the directory to the "db_starter" folder.\n2. Link your footage to the database: You will need files of underwater footage to run this system. You can [download some samples](https://drive.google.com/drive/folders/1t2ce8euh3SEU2I8uhiZN1Tu-76ZDqB6w?usp=sharing) and move them to `db_starter`. You can also store your own files and specify their directory in the notebooks.\n\nPlease remember the format of the underwater media is standardised (typically .mp4 or .jpg) and the associated metadata captured in three CSV files (“movies”, “sites” and “species”) should follow the [Darwin Core standards (DwC)](https://dwc.tdwg.org/simple/). \n\n## Developer instructions\nIf you would like to expand and improve the KSO capabilities, please follow the instructions above to set the project up on your local computer.\n\nWhen you add any changes, please create your branch on top of the current \'dev\' branch. Before submitting a Merge Request, please:\n* Run Black on the code you have edited \n```shell\nblack filename \n```\n* Clean up your commit history on your branch, so that every commit represents a logical change. (so squash and edit commits so that it is understandable for others)\n* For the commit messages, we ask that you please follow the [conventional commits guidelines](https://www.conventionalcommits.org/en/v1.0.0/) (table below) to facilitate code sharing. Also, please describe the logic behind the commit in the body of the message.\n  #### Commit types\n\n| Commit Type | Title                    | Description                                                                                                 | Emoji | \n|:-----------:|--------------------------|-------------------------------------------------------------------------------------------------------------|:-----:|\n|   `feat`    | Features                 | A new feature                                                                                               |   ✨   |       \n|    `fix`    | Bug Fixes                | A bug Fix                                                                                                   |  🐛   |      \n|   `docs`    | Documentation            | Documentation only changes                                                                                  |  📚   |        \n|   `style`   | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      |  💎   |         \n| `refactor`  | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                                   |  📦   |         \n|   `perf`    | Performance Improvements | A code change that improves performance                                                                     |  🚀   |         \n|   `test`    | Tests                    | Adding missing tests or correcting existing tests                                                           |  🚨   |         \n|   `build`   | Builds                   | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         |  🛠   |       \n|    `ci`     | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |  ⚙️   |       \n|   `chore`   | Chores                   | Other changes that don\'t modify src or test files                                                           |  ♻️   |        \n|  `revert`   | Reverts                  | Reverts a previous commit                                                                                   |  🗑   |        \n\n* Rebase on top of dev. (never merge, only use rebase)\n* Submit a Pull Request and link at least 2 reviewers\n\n\n## Citation\n\nIf you use this code or its models in your research, please cite:\n\nAnton V, Germishuys J, Bergström P, Lindegarth M, Obst M (2021) An open-source, citizen science and machine learning approach to analyse subsea movies. Biodiversity Data Journal 9: e60548. https://doi.org/10.3897/BDJ.9.e60548\n\n## Collaborations/Questions\nYou can find out more about the project at https://subsim.wnmedia.se.\n\nWe are always excited to collaborate and help other marine scientists. Please feel free to contact us (matthias.obst(at)marine.gu.se) with your questions.\n\n## Troubleshooting\n\nIf you experience issues with the Panoptes package and/or uploading movies to Zooniverse, it might be related to the libmagic package. In Windows, the following commands might fix the issue:\n```python\npip install python-libmagic\npip install python-magic-bin\n```\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[contributors-shield]: https://img.shields.io/github/contributors/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[contributors-url]: https://https://github.com/ocean-data-factory-sweden/kso/graphs/contributors\n[forks-shield]: https://img.shields.io/github/forks/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[forks-url]: https://github.com/ocean-data-factory-sweden/kso/network/members\n[stars-shield]: https://img.shields.io/github/stars/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[stars-url]: https://github.com/ocean-data-factory-sweden/kso/stargazers\n[issues-shield]: https://img.shields.io/github/issues/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[issues-url]: https://github.com/ocean-data-factory-sweden/kso/issues\n[license-shield]: https://img.shields.io/github/license/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[license-url]: https://github.com/ocean-data-factory-sweden/kso/blob/main/LICENSE.txt\n[high-level-overview]: https://github.com/ocean-data-factory-sweden/kso/blob/main/assets/high-level-overview.png?raw=true\n[Jupyter_site]: https://jupyter.org/\n[colablogo]: https://colab.research.google.com/assets/colab-badge.svg\n[binderlogo]: https://mybinder.org/badge_logo.svg\n[colab_tut_1]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/01_Check_and_update_csv_files.ipynb\n[binder_tut]: https://mybinder.org/v2/gh/ocean-data-factory-sweden/kso/main\n[colab_tut_2]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/02_Upload_new_footage.ipynb\n[colab_tut_3]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/03_Upload_clips_to_Zooniverse.ipynb\n[colab_tut_4]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/04_Upload_frames_to_Zooniverse.ipynb\n[colab_tut_5]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/05_Train_ML_models.ipynb\n[colab_tut_6]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/06_Evaluate_ML_Models.ipynb\n[colab_tut_7]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/07_Transfer_ML_Models.ipynb\n[colab_tut_8]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/08_Analyse_Aggregate_Zooniverse_Annotations.ipynb\n[colab_tut_9]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/09_Run_ML_Models_on_footage.ipynb\n[Microsoft_C++]: https://visualstudio.microsoft.com/visual-cpp-build-tools/\n[pytorch]: https://pytorch.org/\n[YoloV5]: https://github.com/ultralytics/yolov5\n[YoloV8]: https://github.com/ultralytics/ultralytics\n[cdn_bucket]: https://console.cloudina.org/\n[cdn_album]: https://album.cloudina.org/\n[cdn_vendor]: https://vendor.cloudina.org/\n',
     'author': 'Jurie Germishuys',
     'author_email': 'jurie.germishuys@combine.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kso_utils-0.2.5/PKG-INFO` & `kso_utils-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kso-utils
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package containing utility scripts for use with KSO analysis notebooks.
 License: MIT
 Author: Jurie Germishuys
 Author-email: jurie.germishuys@combine.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

