# Comparing `tmp/nitrain-0.2.2.tar.gz` & `tmp/nitrain-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrain-0.2.2.tar", max compression
+gzip compressed data, was "nitrain-0.3.0.tar", max compression
```

## Comparing `nitrain-0.2.2.tar` & `nitrain-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0    34522 2024-04-09 10:29:00.544266 nitrain-0.2.2/LICENSE
--rw-r--r--   0        0        0    10716 2024-04-09 10:29:00.544266 nitrain-0.2.2/README.md
--rw-r--r--   0        0        0      121 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/__init__.py
--rw-r--r--   0        0        0      423 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/base_dataset.py
--rw-r--r--   0        0        0     4070 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/bids_dataset.py
--rw-r--r--   0        0        0     6925 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/configs.py
--rw-r--r--   0        0        0     3027 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/csv_dataset.py
--rw-r--r--   0        0        0     3847 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/folder_dataset.py
--rw-r--r--   0        0        0     7700 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/google_cloud_dataset.py
--rw-r--r--   0        0        0     1574 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/memory_dataset.py
--rw-r--r--   0        0        0     5853 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/platform_dataset.py
--rw-r--r--   0        0        0     2250 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/utils.py
--rw-r--r--   0        0        0      125 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/explainers/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/explainers/occlusion_explainer.py
--rw-r--r--   0        0        0       86 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/loaders/__init__.py
--rw-r--r--   0        0        0     4930 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/loaders/dataset_loader.py
--rw-r--r--   0        0        0      868 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/loaders/keras_loader.py
--rw-r--r--   0        0        0      401 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/loaders/torch_loader.py
--rw-r--r--   0        0        0      145 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/__init__.py
--rw-r--r--   0        0        0     2293 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/fetch_architecture.py
--rw-r--r--   0        0        0      728 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/fetch_pretrained.py
--rw-r--r--   0        0        0      107 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/load.py
--rw-r--r--   0        0        0     7021 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/platform.py
--rw-r--r--   0        0        0      375 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/__init__.py
--rw-r--r--   0        0        0     1136 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/base_sampler.py
--rw-r--r--   0        0        0     2828 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/block_sampler.py
--rw-r--r--   0        0        0     2615 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/patch_sampler.py
--rw-r--r--   0        0        0     1993 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/slice_patch_sampler.py
--rw-r--r--   0        0        0     2421 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/slice_sampler.py
--rw-r--r--   0        0        0      153 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/__init__.py
--rw-r--r--   0        0        0      419 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/cloud_trainer.py
--rw-r--r--   0        0        0     3379 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/model_trainer.py
--rw-r--r--   0        0        0     5825 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/platform_trainer.py
--rw-r--r--   0        0        0      376 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/__init__.py
--rw-r--r--   0        0        0     5189 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/ants_transforms.py
--rw-r--r--   0        0        0      475 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/base_transform.py
--rw-r--r--   0        0        0     5620 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/intensity_transforms.py
--rw-r--r--   0        0        0     4672 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/spatial_transforms.py
--rw-r--r--   0        0        0     5865 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/structural_transforms.py
--rw-r--r--   0        0        0     1553 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/utility_transforms.py
--rw-r--r--   0        0        0      674 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/utils.py
--rw-r--r--   0        0        0      724 2024-04-09 10:29:00.556266 nitrain-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    11944 1970-01-01 00:00:00.000000 nitrain-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-04-24 12:16:09.356540 nitrain-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10779 2024-04-24 12:16:09.356540 nitrain-0.3.0/README.md
+-rw-r--r--   0        0        0      187 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/dataset.py
+-rw-r--r--   0        0        0     3604 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/google_cloud_dataset.py
+-rw-r--r--   0        0        0     3416 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/platform_dataset.py
+-rw-r--r--   0        0        0     1264 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/utils.py
+-rw-r--r--   0        0        0      125 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/explainers/__init__.py
+-rw-r--r--   0        0        0     2307 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/explainers/occlusion_explainer.py
+-rw-r--r--   0        0        0       27 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/loaders/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/loaders/keras_loader.py
+-rw-r--r--   0        0        0     4588 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/loaders/loader.py
+-rw-r--r--   0        0        0      389 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/loaders/torch_loader.py
+-rw-r--r--   0        0        0      145 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/__init__.py
+-rw-r--r--   0        0        0     2293 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/fetch_architecture.py
+-rw-r--r--   0        0        0      728 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/fetch_pretrained.py
+-rw-r--r--   0        0        0      107 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/load.py
+-rw-r--r--   0        0        0     6706 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/platform.py
+-rw-r--r--   0        0        0      200 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/array_reader.py
+-rw-r--r--   0        0        0     1986 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/column_reader.py
+-rw-r--r--   0        0        0      915 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/compose_reader.py
+-rw-r--r--   0        0        0      942 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/image_reader.py
+-rw-r--r--   0        0        0     2143 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/pattern_reader.py
+-rw-r--r--   0        0        0     4749 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/utils.py
+-rw-r--r--   0        0        0      375 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/__init__.py
+-rw-r--r--   0        0        0     1134 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/base_sampler.py
+-rw-r--r--   0        0        0     2828 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/block_sampler.py
+-rw-r--r--   0        0        0     2615 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/patch_sampler.py
+-rw-r--r--   0        0        0     1993 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/slice_patch_sampler.py
+-rw-r--r--   0        0        0     2390 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/slice_sampler.py
+-rw-r--r--   0        0        0      195 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/google_cloud_trainer.py
+-rw-r--r--   0        0        0     5825 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/platform_trainer.py
+-rw-r--r--   0        0        0     3779 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/trainer.py
+-rw-r--r--   0        0        0      276 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/base_transform.py
+-rw-r--r--   0        0        0     5591 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/intensity_transforms.py
+-rw-r--r--   0        0        0     4642 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/spatial_transforms.py
+-rw-r--r--   0        0        0     6597 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/structural_transforms.py
+-rw-r--r--   0        0        0     1556 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/utility_transforms.py
+-rw-r--r--   0        0        0      675 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/utils.py
+-rw-r--r--   0        0        0      416 2024-04-24 12:16:09.360540 nitrain-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11478 1970-01-01 00:00:00.000000 nitrain-0.3.0/PKG-INFO
```

### Comparing `nitrain-0.2.2/LICENSE` & `nitrain-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/README.md` & `nitrain-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,106 @@
-# Nitrain - a framework for medical imaging-native AI
+Metadata-Version: 2.1
+Name: nitrain
+Version: 0.3.0
+Summary: Cloud-based framework for training and sharing medical imaging AI models
+License: MIT
+Author: ncullen93
+Author-email: nicholas.cullen@med.lu.se
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: nitrain-image (>=0.1.1,<0.2.0)
+Requires-Dist: parse (>=1.20.1,<2.0.0)
+Requires-Dist: pydot (>=2.0.0,<3.0.0)
+Description-Content-Type: text/markdown
 
-[![Coverage Status](https://coveralls.io/repos/github/ncullen93/nitrain/badge.svg?branch=main)](https://coveralls.io/github/ncullen93/nitrain?branch=main)
+# Nitrain - a framework for medical imaging AI
+
+[![Coverage Status](https://coveralls.io/repos/github/nitrain/nitrain/badge.svg?branch=main)](https://coveralls.io/github/nitrain/nitrain?branch=main)
 [![Build](https://github.com/ncullen93/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/ncullen93/nitrain/actions/workflows/test.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nitrain)
 
 Nitrain (formerly <i>torchsample</i>) provides tools for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing model results in a medical imaging context. It supports using pytorch, keras, and tensorflow.
 
-You can also train models HIPAA-compliantly in the cloud using nitrain. You are encouraged to make your fitted models available to the community via nitrain, or you can easily use other's pretrained models for fine-tuning or standard image processing.
-
-<br />
-
-## Installation
-
-The latest release of nitrain can be installed from pypi:
-
-```
-pip install nitrain
-```
-
-Or you can install the latest development version directly from github:
-
-```
-python -m pip install git+github.com/ncullen93/nitrain.git
-```
-
-### Dependencies
-
-The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
+To learn how to use nitrain or to view complete examples of training medical imaging AI models using nitrain, visit [github.com/nitrain/tutorials](https://github.com/nitrain/tutorials) or view the rendered version at [nitrain.dev/docs](https://nitrain.dev/docs). If you want to learn more generally about medical imaging AI, check out the book [Becoming a medical imaging AI expert with Python](https://book.nitrain.dev).
 
 <br />
 
 ## Quickstart
 
 Here is a canonical example of using nitrain to fit a brain-age model. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
 
 ```python
-from nitrain import datasets, loaders, models, trainers, transforms as tx
+import nitrain as nt
+from nitrain.readers import PatternReader, ColumnReader
 
 # create dataset from folder of images + participants file
-dataset = datasets.FolderDataset(base_dir='ds004711',
-                                 x={'pattern': 'sub-*/anat/*_T1w.nii.gz'},
-                                 y={'file': 'participants.tsv',
-                                         'column': 'age'},
-                                 x_transforms=[tx.Resize((64,64,64)),
-                                               tx.NormalizeIntensity(0,1)])
+dataset = nt.Dataset(inputs=PatternReader('sub-*/anat/*_T1w.nii.gz'),
+                          outputs=ColumnReader('participants.tsv', 'age'),
+                          transforms={
+                              'inputs': [tx.Resize((64,64,64)), tx.NormalizeIntensity(0,1)],
+                          },
+                          base_dir='~/desktop/ds004711/')
 
 # create loader with random transforms
-loader = loaders.DatasetLoader(dataset,
-                               images_per_batch=4,
-                               shuffle=True,
-                               sampler=samplers.SliceSampler(batch_size=32, axis=2)
-                               x_transforms=[tx.RandomNoise(sd=0.2)])
+loader = nt.Loader(dataset,
+                        images_per_batch=4,
+                        shuffle=True,
+                        sampler=nitrain.SliceSampler(batch_size = 32, axis = 2)
+                        transforms={
+                                'inputs': tx.RandomNoise(sd=0.2)
+                        })
 
 # create model from architecture
-arch_fn = models.fetch_architecture('alexnet', dim=2)
+arch_fn = nt.fetch_architecture('alexnet', dim=2)
 model = arch_fn(input_image_size=(64,64,1),
                 number_of_outcomes=1,
                 mode='regression')
 
 # create trainer and fit model
-trainer = trainers.ModelTrainer(model,
-                                loss='mse',
-                                optimizer='adam',
-                                lr=1e-3,
-                                callbacks=[utils.EarlyStopping(),
-                                           utils.ModelCheckpoints(freq=25)])
+trainer = nt.Trainer(model,
+                          loss='mse',
+                          optimizer='adam',
+                          lr=1e-3,
+                          callbacks=[utils.EarlyStopping(),
+                                     utils.ModelCheckpoints(freq=25)])
 trainer.fit(loader, epochs=100)
 
 # upload trained model to platform
-models.register_model(trainer.model, 'nick/t1-brain-age')
+nt.register_model(trainer.model, 'nick/t1-brain-age')
 ```
 
 A more in-depth introduction can be found in the [tutorials](github.com/ncullen93/nitrain) and if you can also check out the [examples](github.com/ncullen93/nitrain) for self-contained notebooks showing how to perform common deep learning tasks.
 
 <br />
 
+## Installation
+
+The latest release of nitrain can be installed from pypi:
+
+```
+pip install nitrain
+```
+
+Or you can install the latest development version directly from github:
+
+```
+python -m pip install git+github.com/ncullen93/nitrain.git
+```
+
+### Dependencies
+
+The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
+
+<br />
+
 ## Overview of nitrain
 
 The 10-minute overview presented below will take you through the key components of nitrain:
 
 - [Datasets and Loaders](#datasets-and-loaders)
 - [Samplers](#samplers)
 - [Transforms](#transforms)
@@ -86,15 +108,15 @@
 - [Model trainers](#model-trainers)
 - [Explainers](#explainers)
 
 <br />
 
 ### Datasets and Loaders
 
-Datasets help you read in your images from wherever they are stored -- in a local folder with BIDS or datalad, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, BIDS entities, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
+Datasets help you read in your images from wherever they are stored -- in a local folder, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
 
 ```python
 from nitrain import datasets, transforms as tx
 
 dataset = datasets.FolderDataset(base_dir='~/datasets/ds004711',
                                  x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
                                  y={'file': 'participants.tsv', 'column': 'age'},
@@ -162,24 +184,24 @@
 
 my_tx = tx.CustomTransform(lambda x: x * 2)
 ```
 
 If you want to explore what a transform does, you can take a sample of it over any number of trials on the same image and then plot the results:
 
 ```python
-import ants
+import ntimage as nt
 import numpy as np
 from nitrain import transforms as tx
 
-img = ants.image_read(ants.get_data('r16'))
+img = nt.load(nt.example_data('r16'))
 
 my_tx = tx.RandomSmoothing(0, 2)
 imgs = my_tx.sample(img, n=12)
 
-ants.plot_grid(np.array(imgs).reshape(4,3))
+nt.plot_grid(imgs, shape=(4,3))
 ```
 
 <br />
 
 ### Architectures and pretrained models
 
 The nitrain package provides an interface to an extensive amount of deep learning model architectures for all kinds of tasks - regression, classification, image-to-image generation, segmentation, autoencoders, etc.
@@ -205,18 +227,18 @@
 
 <br />
 
 ### Trainers
 
 After you have created a model from a nitrain architecture, fetched a pretrained model, or created a model yourself in your framework of choice, then it's time to actually train the model on the dataset / loader that you've created.
 
-Although you are free to train models on loaders using standard pytorch, keras, or tensorflow workflows, we also provide the `ModelTrainer` class to make training even easier. This class provides sensible defaults for key training parameters based on your task.
+Although you are free to train models on loaders using standard pytorch, keras, or tensorflow workflows, we also provide the `LocalTrainer` class to make training even easier. This class provides sensible defaults for key training parameters based on your task.
 
 ```python
-trainer = trainers.ModelTrainer(model=vgg_model, task='regression')
+trainer = trainers.LocalTrainer(model=vgg_model, task='regression')
 trainer.fit(loader, epochs=10)
 
 # access fitted model
 print(trainer.model)
 ```
 
 If you have signed up for an account at [nitrain.dev](https://www.nitrain.dev) then you can also train your model in the cloud using the `PlatformTrainer` class. All training takes place on HIPAA-compliant GPU servers with competitive pricing.
@@ -239,7 +261,8 @@
 Nitrain provides tools to perform this techique - along with many others - and can help you visualize the results of such explainability experiments directly in brain space. Here is what that might look like:
 
 <br />
 
 ## Contributing
 
 If you would like to contribute to nitrain, we would be extremely thankful. The best way to start is by posting an issue to discuss your proposed feature.
+
```

### Comparing `nitrain-0.2.2/nitrain/explainers/occlusion_explainer.py` & `nitrain-0.3.0/nitrain/explainers/occlusion_explainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,20 @@
         ---------
         model : a fitted model
             The model to use when running the explainer. 
         
         Examples
         --------
         >>> model = models.fetch_pretrained('nick/t1-brain-age')
-        >>> image = ants.image_read(ants.get_data('mni'))
-        >>> trainer = ModelTrainer(model)
+        >>> image = nt.load(nt.example_data('mni'))
+        >>> trainer = LocalTrainer(model)
         >>> trainer.fit(loader)
         >>> explainer = explainers.OcclusionExplainer(trainer.model)
         >>> explainer.fit(image)
-        >>> ants.plot(image, overlay=explainer.result_image)
+        >>> nt.plot(image, overlay=explainer.result_image)
         """
         self.model = model
         
         # generated once fit() method is called
         self.result_image = None
         
     def fit(self, inputs, outputs=None):
```

### Comparing `nitrain-0.2.2/nitrain/loaders/dataset_loader.py` & `nitrain-0.3.0/nitrain/loaders/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import math
 import numpy as np
+import warnings
 
 from .. import samplers
 
-class DatasetLoader:
+class Loader:
     
     def __init__(self, 
                  dataset, 
                  images_per_batch, 
-                 x_transforms=None, 
-                 y_transforms=None, 
-                 co_transforms=None,
+                 transforms=None,
                  expand_dims=-1,
                  shuffle=False,
                  sampler=None):
         """
         Arguments
         ---------
         
         Examples
         --------
         ds = Dataset()
         ld = DatasetLoader(ds)
         xb, yb = next(iter(ld))
 
         """
+        if images_per_batch > len(dataset):
+            warnings.warn(f'Warning: The supplied images_per_batch ({images_per_batch}) is larger than available dataset records ({len(dataset)}). Setting to available dataset records.')
+            images_per_batch = len(dataset)
+            
         self.dataset = dataset
         self.images_per_batch = images_per_batch
         self.expand_dims = expand_dims
-        self.x_transforms = x_transforms
-        self.y_transforms = y_transforms
-        self.co_transforms = co_transforms
+        self.transforms = transforms
         self.shuffle = shuffle
         
         if sampler is None:
             sampler = samplers.BaseSampler(batch_size=images_per_batch)
         self.sampler = sampler
         
     def to_keras(self, output_signature=None):
@@ -76,49 +77,37 @@
             
             data_indices = slice(image_batch_idx*images_per_batch, min((image_batch_idx+1)*images_per_batch, len(dataset)))
             x, y = dataset[data_indices]
             
             image_batch_idx += 1
            
             # perform transforms
-            if self.x_transforms:
-                for tx_fn in self.x_transforms:
-                    x = [tx_fn(xx) for xx in x]
-            
-            if self.y_transforms:
-                for tx_fn in self.y_transforms:
-                    y = [tx_fn(yy) for yy in y]
-            
-            if self.co_transforms:
-                for tx_fn in self.co_transforms:
-                    for i in range(len(x)):
-                        x[i], y[i] = tx_fn(x[i], y[i])
-
+            if self.transforms:
+                pass
             # sample the batch
             sampled_batch = self.sampler(x, y)
             
             # a normal sampler will just return the entire (shuffled, if specified) batch once
             # a slice sampler will return shuffled slices with batch size = sampler.images_per_batch
             for x_batch, y_batch in sampled_batch:
                 
                 if self.expand_dims is not None:
                     if isinstance(x_batch[0], list):
-                        print('got multiple inputs')
                         x_batch_return = []
                         for i in range(len(x_batch[0])):
                             tmp_x_batch = np.array([np.expand_dims(xx[i].numpy(), self.expand_dims) for xx in x_batch])
                             x_batch_return.append(tmp_x_batch)
                         x_batch = x_batch_return
                     else:
                         x_batch = np.array([np.expand_dims(xx.numpy(), self.expand_dims) for xx in x_batch])
-                    if 'ANTsImage' in str(type(y[0])):
+                    if 'NTImage' in str(type(y[0])):
                         y_batch = np.array([np.expand_dims(yy.numpy(), self.expand_dims) for yy in y_batch])
                 else:
                     x_batch = np.array([xx.numpy() for xx in x_batch])
-                    if 'ANTsImage' in str(type(y[0])):
+                    if 'NTImage' in str(type(y[0])):
                         y_batch = np.array([yy.numpy() for yy in y_batch])
                 
                 yield x_batch, y_batch
                 
     def __len__(self):
         return math.ceil((len(self.dataset) / self.images_per_batch) * len(self.sampler))
```

### Comparing `nitrain-0.2.2/nitrain/loaders/keras_loader.py` & `nitrain-0.3.0/nitrain/loaders/keras_loader.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/nitrain/models/fetch_architecture.py` & `nitrain-0.3.0/nitrain/models/fetch_architecture.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/nitrain/models/fetch_pretrained.py` & `nitrain-0.3.0/nitrain/models/fetch_pretrained.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/nitrain/platform.py` & `nitrain-0.3.0/nitrain/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import requests
 import os
 import tempfile
 import json
 from tqdm import tqdm
-import ants
 
-from .datasets import PlatformDataset, GoogleCloudDataset
+from . import datasets
 
 api_url = 'https://api.ants.dev'
 
 def list_platform_datasets():
     return _list_dataset_records()
 
 
@@ -84,15 +83,14 @@
             
 
     # upload participants file (y)
     filename = os.path.join(name, dataset.y_config['file'])
     with open(os.path.join(dataset.base_dir, dataset.y_config['file']), 'rb') as file:
         response = _upload_file_to_platform(file=file, category='datasets', filename=filename)
     
-    # if BIDS dataset -> write json file because BIDS layout doesnt work on platform ?
     return response
 
 def _get_user_from_token(token=None):
     if token is None:
         token = os.environ['NITRAIN_API_TOKEN']
     ## create the dataset record
     response = requests.get(f'{api_url}/username/',
@@ -103,15 +101,15 @@
     
 def _convert_to_platform_dataset(dataset, name, fuse=True):
     """
     Convert any nitrain dataset to a platform dataset that
     can be used in training a model on the platform.
     """
     params = _config_for_platform_dataset(dataset)
-    return GoogleCloudDataset(
+    return datasets.GoogleCloudDataset(
         bucket='ants-dev',
         base_dir=f'datasets/{name}',
         x = params['x_config'],
         y = params['y_config'],
         x_transforms = dataset.x_transforms,
         y_transforms = dataset.y_transforms,
         fuse = fuse,
@@ -189,16 +187,12 @@
                 headers = {'Authorization': f'Bearer {token}'})
     if response.status_code != 201:
         print(f'Error: {response.status_code}')
     return response 
 
 def _config_for_platform_dataset(dataset):
     """Get the x + y config that is appropriate for a PlatformDataset"""
-    if type(dataset).__name__ == 'BIDSDataset':
-        # BIDS entities not
-        parameters = {'x_config': {'filenames': dataset.x},
-                      'y_config': dataset.y_config}
-    elif type(dataset).__name__ == 'FolderDataset':
+    if type(dataset).__name__ == 'FolderDataset':
         parameters = {'x_config': dataset.x_config,
                       'y_config': dataset.y_config}
     return parameters
```

### Comparing `nitrain-0.2.2/nitrain/samplers/base_sampler.py` & `nitrain-0.3.0/nitrain/samplers/base_sampler.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             self.idx += 1
             x = self.x
             y = self.y
                 
             if self.shuffle:
                 indices = random.sample(range(len(y)), len(y))
                 x = [x[i] for i in indices]
-                if 'ANTsImage' in str(type(y[0])):
+                if 'NTImage' in str(type(y[0])):
                     y = [y[i] for i in indices]
                 else:
                     y = y[indices]
             
             return x, y
         else:
             raise StopIteration
```

### Comparing `nitrain-0.2.2/nitrain/samplers/block_sampler.py` & `nitrain-0.3.0/nitrain/samplers/block_sampler.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/nitrain/samplers/patch_sampler.py` & `nitrain-0.3.0/nitrain/samplers/patch_sampler.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/nitrain/samplers/slice_patch_sampler.py` & `nitrain-0.3.0/nitrain/samplers/slice_patch_sampler.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.2/nitrain/samplers/slice_sampler.py` & `nitrain-0.3.0/nitrain/samplers/slice_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         self.idx = 0
         
         # apply shuffling
         if self.shuffle:
             indices = random.sample(range(len(self.y)), len(self.y))
             self.x = [self.x[i] for i in indices]
-            if 'ANTsImage' in str(type(self.y[0])):
+            if 'NTImage' in str(type(self.y[0])):
                 self.y = [self.y[i] for i in indices]
             else:
                 self.y = self.y[indices]
             
         return self
 
     def __next__(self):
@@ -58,25 +58,25 @@
     def __repr__(self):
         return f'''samplers.SliceSampler(axis={self.axis}, batch_size={self.batch_size}, shuffle={self.shuffle})'''
 
 
 
 def create_slices(images, values, axis):
     
-    if 'ANTsImage' in str(type(values[0])):
+    if 'NTImage' in str(type(values[0])):
         slices = []
         co_slices = []
         for image, co_image in zip(images, values):
             for i in range(image.shape[axis]):
-                slices.append(image.slice_image(axis, i, 1))
-                co_slices.append(co_image.slice_image(axis, i, 1))
+                slices.append(image.slice(axis, i))
+                co_slices.append(co_image.slice(axis, i))
                 
         return slices, co_slices
     else:
         slices = []
         new_values = []
         for image, value in zip(images, values):
             for i in range(image.shape[axis]):
-                slices.append(image.slice_image(axis, i, 1))
+                slices.append(image.slice(axis, i))
                 new_values.append(value)
                 
         return slices, np.array(new_values)
```

### Comparing `nitrain-0.2.2/nitrain/trainers/model_trainer.py` & `nitrain-0.3.0/nitrain/trainers/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 
 
-class ModelTrainer:
+class Trainer:
     """
-    The ModelTrainer class provides high-level functionality to train
+    The LocalTrainer class provides high-level functionality to train
     deep learning models on dataset loaders. It wraps the most popular
     frameworks under a common interface.
     
     Examples
     --------
     >>> download = fetch_data('openneuro/ds004711')
     >>> data = FolderDataset(download.path)
     >>> loader = DatasetLoader(data, batch_size=32)
     >>> model_fn = fetch_architecture('autoencoder')
     >>> model = model_fn((120, 60, 30))
-    >>> trainer = ModelTrainer(model, task='regression')
+    >>> trainer = LocalTrainer(model, task='regression')
     >>> trainer.fit(loader, epochs=10)
     """
     
     def __init__(self, 
                  model,
                  task,
                  optimizer=None,
@@ -41,17 +41,17 @@
         ## losses
         """
         self.model = model
         if task == 'regression':
             optimizer = 'adam' if optimizer is None else optimizer
             loss = 'mse' if loss is None else loss
             metrics = ['mse'] if metrics is None else metrics
-        elif task == 'classification':
+        elif task in ('classification', 'segmentation'):
             optimizer = 'adam' if optimizer is None else optimizer
-            if model.output_shape[-1] == 1:
+            if model.output_shape[-1] > 1:
                 loss = 'categorical_crossentropy' if loss is None else loss
             else:
                 loss = 'binary_crossentropy' if loss is None else loss
             metrics = ['accuracy'] if metrics is None else metrics
         else:
             raise ValueError('The only valid tasks are `regression` and `classification`.')
         
@@ -59,46 +59,57 @@
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
                 
         framework = infer_framework(model)
         self.framework = framework
         
-        if framework == 'keras':
-            self.model.compile(optimizer='adam',
-                               loss='mse',
-                               metrics=['mse'])
+        if self.framework == 'keras':
+            self.model.compile(optimizer=self.optimizer,
+                               loss=self.loss,
+                               metrics=self.metrics)
         
     def fit(self, loader, epochs, **kwargs):
         if self.framework == 'keras':
-            if type(loader).__name__ == 'DatasetLoader':
+            if type(loader).__name__ == 'Loader':
                 loader = loader.to_keras()
             return self.model.fit(loader, epochs=epochs, **kwargs)
 
     def evaluate(self, loader):
         if self.framework == 'keras':
-            if type(loader).__name__ == 'DatasetLoader':
+            if type(loader).__name__ == 'Loader':
                 loader = loader.to_keras()
             return self.model.evaluate(loader)
     
     def predict(self, loader):
         if self.framework == 'keras':
-            if type(loader).__name__ == 'DatasetLoader':
+            if type(loader).__name__ == 'Loader':
                 loader = loader.to_keras()
             return self.model.predict(loader)
     
     def summary(self):
         if self.framework == 'keras':
             return self.model.summary()
     
     def save(self, path):
         if self.framework == 'keras':
             self.model.save(path)
+    
+    def __repr__(self):
+        s = 'LocalTrainer ({})\n'.format(self.task)
+        s = s +\
+            '     {:<10} : {}\n'.format('Framework', self.framework)+\
+            '     {:<10} : {}\n'.format('Loss', self.loss)+\
+            '     {:<10} : {}\n'.format('Optimizer', self.optimizer)
+        return s
 
 
 def infer_framework(model):
     model_type = str(type(model))
     if 'keras' in model_type:
         return 'keras'
+    
     if 'torch' in model_type:
         return 'torch'
+    
+    raise ValueError('Could not infer framework from model')
```

### Comparing `nitrain-0.2.2/nitrain/trainers/platform_trainer.py` & `nitrain-0.3.0/nitrain/trainers/platform_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.token = token
         
         
     def fit(self, loader, epochs):
         """
         Launch a training job on the platform.
         
-        This function is used in the same was as for `ModelTrainer`, except that
+        This function is used in the same was as for `LocalTrainer`, except that
         calling `fit()` with a `PlatformTrainer` will launch a training job on the platform.
         
         If the dataset for the loader passed into this function is not a `PlatformDataset` then the
         dataset will be temporarily uploaded to the cloud for training and then deleted after. To save
         time on repeated training jobs, the loader can be cached by setting `cache=True` when 
         initializing the trainer.
         
@@ -84,15 +84,15 @@
         # Generate training script
         
         # imports
         repr_imports = '''
         from nitrain import models, samplers, trainers, transforms as tx
         from nitrain.datasets import GoogleCloudDataset
         from nitrain.loaders import DatasetLoader
-        frmo nitrain.trainers import ModelTrainer
+        frmo nitrain.trainers import LocalTrainer
         '''
         
         # dataset
         platform_dataset = _convert_to_platform_dataset(loader.dataset, job_dir)
         repr_dataset = f'''
         dataset = {repr(platform_dataset)}
         '''
@@ -105,15 +105,15 @@
         # model
         repr_model = f'''
         model = models.load("/gcs/ants-dev/models/{self.user}/untrained__{self.name}")
         '''
         
         # trainer
         repr_trainer = f'''
-        trainer = ModelTrainer(model=model, task="{self.task}")
+        trainer = LocalTrainer(model=model, task="{self.task}")
         trainer.fit(loader, epochs={epochs})
         '''
         
         # save model
         repr_save = f'''
         trainer.save("/gcs/ants-dev/models/{job_dir}")
         '''
```

### Comparing `nitrain-0.2.2/nitrain/transforms/intensity_transforms.py` & `nitrain-0.3.0/nitrain/transforms/structural_transforms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,171 +1,214 @@
-import ants
-
+import ntimage as nt
 import random
-import numpy as np
 
 from .base_transform import BaseTransform
 
 
-class StandardNormalize(BaseTransform):
+class SplitLabels(BaseTransform):
     """
-    import ants
-    img = ants.image_read(ants.get_ants_data('r16'))
-    img2 = (img - img.mean()) / img.std()
+    This transform takes a discrete valued (e.g., segmentation) image
+    with no channels (e.g., shape: [128, 128]) and creates separate
+    channels for each label. 
     
-    from nitrain import transforms as tx
-    my_tx = tx.StandardNormalize()
-    img3 = my_tx(img)
+    For instance, a binary image with 2 classes with shape (128,128) would 
+    be turned into an image of shape (128, 128, 2).
+    
+    Examples
+    --------
+    >>> import ntimage as nt
+    >>> from nitrain import transforms as tx
+    >>> img = nt.load(nt.example_data('r16'))
+    >>> img = img > img.mean()
+    >>> my_tx = tx.SplitLabels()
+    >>> img_split = my_tx(img)
     """
-    def __init__(self, level='individual'):
-        self.level = level
+    def __init__(self):
+        pass
+    
+    def __call__(self, image, co_image=None):
+        # get labels
+        labels = image.unique()
         
-    def __call__(self, *images):
-        new_images = []
-        for img in images:
-            new_image = (img - img.mean()) / img.std()
-            new_images.append(new_image)
+        # split labels into different images
+        image_list = [image == label_value for label_value in labels]
         
-        return new_images if len(new_images) > 1 else new_images[0]
-
+        # merge channels
+        image_merged = nt.merge(image_list)
+        
+        return image_merged
 
-class Threshold(BaseTransform):
+class Resample(BaseTransform):
     """
-    import ants
-    img = ants.image_read(ants.get_ants_data('r16'))
+    img = nt.load(nt.example_data('mni'))
+    # resample voxel directly (fine if image has even dimensions.. not here though)
+    my_tx = ResampleImage((60,60,60))
+    img2 = my_tx(img)
+    # resample with spacing so you dont have to figure out uneven dimensions
+    my_tx2 = ResampleImage((4,4,4), use_spacing=True)
+    img3 = my_tx2(img)
     """
-    def __init__(self, threshold):
-        self.threshold = threshold
+    def __init__(self, params, use_spacing=False, interpolation='linear'):
+        self.params = params
+        self.use_spacing = use_spacing
+        self.interpolation = interpolation
         
     def __call__(self, *images):
         new_images = []
         for image in images:
-            new_image = image * (image > self.threshold)
-            new_images.append(new_image)
+            image = nt.resample(image, self.params, interpolation=self.interpolation, use_spacing=self.use_spacing)
+            new_images.append(image)
+        
         return new_images if len(new_images) > 1 else new_images[0]
 
+    def __repr__(self):
+        return f'tx.Resample({self.params}, {self.use_spacing}, "{self.interpolation}")'
 
-class RangeNormalize(BaseTransform):
-    def __init__(self, min=0, max=1, level='individual'):
-        self.min = min
-        self.max = max
-        
-    def __call__(self, *images):
-        new_images = []
-        for image in images:
-            new_image = (image - image.min()) / (image.max() - image.min())
-            new_images.append(new_image)
-        return new_images if len(new_images) > 1 else new_images[0]
+class ResampleToTarget(BaseTransform):
+    """
+    img = nt.load(nt.example_data('mni'))
+    img2 = img.clone().resample_image((4,4,4))
+    my_tx = ResampleImageToTarget(img2)
+    img3 = my_tx(img)
+    """
+    def __init__(self, target, interpolation='linear'):
+        self.target = target
+        self.interpolation = 0 if interpolation != 'nearest_neighbor' else 1 
+    
+    def __call__(self, image):
+        image = nt.resample(image, self.target, self.interpolation)
+        return image
 
 
-class Smoothing(BaseTransform):
+class Reorient(BaseTransform):
     """
-    import ants
-    img = ants.image_read(ants.get_ants_data('r16'))
-    img2 = ants.smooth_image(img, 2, True)
-    img3 = ants.smooth_image(img, 2, False)
-    """
-    
-    def __init__(self, std, physical_space=True):
-        """
-        Arguments
-        ---------
-        std : float or tuple of floats
-            std of a Gaussian kernal.
-
-        physical_space : boolean
-            If true, std is interpreted as being in millimeters (i.e., physical coordinates).
-            If false, std is interpreted as being in pixels. This makes no difference if 
-            the image has unit spacing.
-        """
-        self.std = std
-        self.physical_space = physical_space
+    Reorient an image.
+    
+    Images are oriented along three axes:
+    - Right (R) to Left (L)
+    - Inferior (I) to Superior (S) 
+    - Anterior (A) to Posterior (P)
+    
+    An image orientation consists of three letters - one from each
+    of the three axes - with the letter for each axes determining
+    where the indexing starts. Orientation is important for slicing.
+    """
+    def __init__(self, orientation='RAS'):
+        self.orientation = orientation
+    
+    def __call__(self, image, co_image=None):
+        image = nt.reorient(image, self.orientation)
         
-    def __call__(self, *images):
-        new_images = []
-        for image in images:
-            new_image = ants.smooth_image(image, 
-                                          self.std,
-                                          self.physical_space)
-            new_images.append(new_image)
-        return new_images if len(new_images) > 1 else new_images[0]
+        if co_image is not None:
+            co_image = nt.reorient(co_image, self.orientation)
+            return image, co_image
 
+        return image
 
-class RandomSmoothing(BaseTransform):
+class Slice(BaseTransform):
+    """
+    Slice a 3D image into 2D. 
+    """
+    def __init__(self, axis, idx):
+        self.axis = axis
+        self.idx = idx
+    
+    def __call__(self, image):
+        if self.idx is None:
+            new_image = [image.slice(self.axis, idx) for idx in range(image.shape[self.axis])]
+        else:
+            new_image = image.slice(self.axis, self.idx)
+        return new_image
 
-    def __init__(self, min_std, max_std, physical_space=True):
-        self.min_std = min_std
-        self.max_std = max_std
-        self.physical_space = physical_space
 
-    def __call__(self, *images):
-        std = random.uniform(self.min_std, self.max_std)
+class RandomSlice(BaseTransform):
+    """
+    Randomly slice a 3D image into 2D. 
+    
+    """
+    def __init__(self, axis, allow_blank=True):
+        self.axis = axis
+        self.allow_blank = allow_blank
+    
+    def __call__(self, image):
+        if not self.allow_blank:
+            image = image.crop_image()
         
-        new_images = []
-        for image in images:
-            new_image = ants.smooth_image(image, 
-                                          std,
-                                          self.physical_space)
-            new_images.append(new_image)
-        return new_images if len(new_images) > 1 else new_images[0]
+        idx = random.sample(range(image.shape[self.axis]), 1)[0]
+        new_image = image.slice(self.axis, idx)
+        
+        return new_image
 
-    def __repr__(self):
-        return f'''tx.RandomSmoothing({self.min_std}, {self.max_std}, {self.physical_space})'''
 
-class RandomNoise(BaseTransform):
+class Crop(BaseTransform):
     """
-    Apply random additive gaussian noise to an image.
-    
-    import ants
-    img = ants.image_read(ants.get_ants_data('r16'))
-    img2 = ants.add_noise_to_image(img, 'additivegaussian', (0, 16))
-    ants.plot((img2 - img))
+    Crop an image to remove all blank space around the brain or
+    crop based on specified indices.
     """
-    def __init__(self, min_std, max_std):
-        self.min_std = min_std
-        self.max_std = max_std
+    def __init__(self, lower=None, upper=None, leader=None):
+        self.lower = lower
+        self.upper = upper
+        self.leader = leader
     
     def __call__(self, *images):
-        std = random.uniform(self.min_std, self.max_std)
         new_images = []
         for image in images:
-            new_image = ants.add_noise_to_image(image,
-                                                'additivegaussian',
-                                                (0, std))
+            new_image = image.crop(self.lower, self.upper)
             new_images.append(new_image)
         return new_images if len(new_images) > 1 else new_images[0]
-    
-    def __repr__(self):
-        return f'''tx.RandomNoise({self.min_std}, {self.max_std})'''
 
 
-class HistogramWarpIntensity(BaseTransform):
+class RandomCrop(BaseTransform):
     """
-    See https://github.com/ANTsX/ANTsPyNet/blob/master/antspynet/utilities/histogram_warp_image_intensities.py
+    Randomly crop an image of the specified size
+    
+    Examples
+    --------
+    >>> import ntimage as nt
+    >>> from nitrain import transforms as tx
+    >>> mni = nt.load(nt.example_data('mni'))
+    >>> my_tx = tx.RandomCrop(size=(30,30,30))
+    >>> mni_crop = my_tx(mni)
+    >>> mni_crop.plot(domain_image_map=mni)
+    >>> mni_orig = mni_crop.decrop_image(mni) # put image back
     """
-    def __init__(self, 
-                 break_points=(0.25, 0.5, 0.75),
-                 displacements=None,
-                 clamp_end_points=(False, False),
-                 sd_displacements=0.05,
-                 transform_domain_size=20):
-        self.break_points = break_points
-        self.displacements = displacements
-        self.clamp_end_points = clamp_end_points
-        self.sd_displacements = sd_displacements
-        self.transform_domain_size = transform_domain_size
+    def __init__(self, size):
+        self.size = size
+    
+    def __call__(self, image):
+        size = self.size
+        if isinstance(size, int):
+            size = tuple([size for _ in range(image.dimension)])
+            
+        lower_indices = [random.sample(range(0, image.shape[i]-size[0]), 1)[0] for i in range(len(size))]
+        upper_indices = [lower_indices[i] + size[i] for i in range(len(size))]
+            
+        new_image = image.crop_indices(lower_indices,
+                                       upper_indices)
+        return new_image
 
-    def __call__(self, *images):
-        import antspynet
-        
-        new_images = []
-        for image in images:
-            new_image = antspynet.histogram_warp_image_intensities(
-                image = image,
-                break_points = self.break_points,
-                displacements = self.displacements,
-                clamp_end_points = self.clamp_end_points,
-                sd_displacements = self.sd_displacements,
-                transform_domain_size = self.transform_domain_size
-            )
-            new_images.append(new_image)
-        return new_images if len(new_images) > 1 else new_images[0]
+
+class Pad(BaseTransform):
+    """
+    Pad an image to a specified shape or by a specified amount.
+    
+    Example
+    -------
+    >>> import ntimage as nt
+    >>> from nitrain import transforms as tx
+    >>> mni = nt.load(nt.example_data('mni'))
+    >>> my_tx = tx.Pad((220,220,220))
+    >>> mni_pad = my_tx(mni)
+    """
+    
+    def __init__(self, shape=None, width=None, value=0.0):
+        if shape is None and width is None:
+            raise Exception('Either shape or width must be supplied to Pad transform.')
+        self.shape = shape
+        self.width = width
+        self.value = value
+    
+    def __call__(self, image):
+        new_image = image.pad_image(shape=self.shape,
+                                    pad_width=self.width,
+                                    value=self.value)
+        return new_image
```

### Comparing `nitrain-0.2.2/nitrain/transforms/spatial_transforms.py` & `nitrain-0.3.0/nitrain/transforms/spatial_transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ants
+import ntimage as nt
 import numpy as np
 import random
 
 from .base_transform import BaseTransform
 
 class RandomAffine(BaseTransform):
     pass
@@ -10,21 +10,21 @@
 class RandomRotate(BaseTransform):
     pass
 
 class RandomTranslate(BaseTransform):
     """
     Examples
     --------
-    >>> import ants
+    >>> import ntimage as nt
     >>> from nitrain import transforms as tx
-    >>> img = ants.image_read(ants.get_data('r16'))
+    >>> img = nt.load(nt.example_data('r16'))
     >>> my_tx = RandomTranslate(-20, 20)
     >>> img_tx = my_tx(img)
     >>> img_tx.plot(img)
-    >>> img = ants.image_read(ants.get_data('mni'))
+    >>> img = nt.load(nt.example_data('mni'))
     >>> my_tx = RandomTranslate(-20, 20)
     >>> img_tx = my_tx(img)
     >>> img_tx.plot(img)
     """
     
     def __init__(self, min_value, max_value, reference=None):
         self.min_value = min_value
@@ -33,19 +33,19 @@
         if self.reference is not None:
             self.reference_com = self.reference.get_center_of_mass()
     
     def __call__(self, x, y=None):
         image_dim = x.dimension
         
         # create transform
-        ants_tx = ants.create_ants_transform(precision="float", 
-                                             dimension=image_dim, 
-                                             transform_type="AffineTransform")
+        my_tx = nt.empty_transform(precision="float", 
+                                      dimension=image_dim, 
+                                      transform_type="AffineTransform")
         if self.reference is not None:
-            ants_tx.set_fixed_parameters(self.reference_com)
+            my_tx.set_fixed_parameters(self.reference_com)
         
         # sample translation value
         min_value = self.min_value
         if isinstance(min_value, (int, float)):
             min_value = [min_value for _ in range(image_dim)]
 
         max_value = self.max_value
@@ -58,36 +58,36 @@
             tx_matrix = np.array([[1, 0, tx_values[0]], 
                                   [0, 1, tx_values[1]]])
         elif image_dim == 3:
             tx_matrix = np.array([[1, 0, 0, tx_values[0]], 
                                   [0, 1, 0, tx_values[1]], 
                                   [0, 0, 1, tx_values[2]]])
             
-        ants_tx.set_parameters(tx_matrix)
+        my_tx.set_parameters(tx_matrix)
         if y is None:
-            return ants_tx.apply_to_image(x, reference=self.reference)
+            return my_tx.apply_to_image(x, reference=self.reference)
         else:
             return (
-                ants_tx.apply_to_image(x, reference=self.reference),
-                ants_tx.apply_to_image(y, reference=self.reference),
+                my_tx.apply_to_image(x, reference=self.reference),
+                my_tx.apply_to_image(y, reference=self.reference),
             )
         
 
 class RandomShear(BaseTransform):
     pass
 
 class RandomZoom(BaseTransform):
     """
     Apply a random zoom transform to an image
     
     Examples
     --------
-    >>> import ants
+    >>> import ntimage as nt
     >>> from nitrain import transforms as tx
-    >>> image = ants.image_read(ants.get_data('r16'))
+    >>> image = nt.load(nt.example_data('r16'))
     >>> my_tx = tx.RandomZoom(0.8,1.2)
     >>> new_image = my_tx(image)
     """
     
     def __init__(self, min_zoom, max_zoom):
         self.min_zoom = min_zoom
         self.max_zoom = max_zoom
@@ -108,17 +108,17 @@
     Randomly flip an image with specified proabilikty.
     
     If no axis is specified, then the axis will be chosen
     randomly with equal probability.
     
     Examples
     --------
-    >>> import ants
+    >>> import ntimage as nt
     >>> from nitrain import transforms as tx
-    >>> img = ants.image_read(ants.get_data('r16'))
+    >>> img = nt.load(nt.example_data('r16'))
     >>> my_tx = tx.RandomFlip(p=1)
     >>> new_img = my_tx(img)
     >>> new_img.plot()
     """
     def __init__(self, p=0.5, axis=None):
         self.p = p
         self.axis = axis
@@ -136,15 +136,15 @@
         return image
     
     def __repr__(self):
         return f'''tx.RandomFlip({self.p}, {self.axis})'''
         
 
 def create_centered_affine_transform(image, matrix):
-    transform = ants.create_ants_transform(
+    transform = nt.empty_transform(
         transform_type="AffineTransform", 
         precision='float', 
         matrix=matrix,
         center=[image.shape[i]/2 for i in range(image.dimension)],
         dimension=image.dimension
     )
     return transform
```

### Comparing `nitrain-0.2.2/nitrain/transforms/utility_transforms.py` & `nitrain-0.3.0/nitrain/transforms/utility_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
-import ants
+import ntimage as nt
 import random
 import string
 import numpy as np
 
 from .base_transform import BaseTransform
 
 class ToFile(BaseTransform):
     """
-    Saves an image to file using `ants.plot`. 
+    Saves an image to file using `nt.plot`. 
     
     Useful as a pass-through ransform when wanting to observe 
     how augmentation affects the data.
     """
     def __init__(self, base_dir, ortho=False):
         self.base_dir = base_dir
         self.ortho = ortho
 
     def __call__(self, image):
         filename = ''.join(random.choice(string.ascii_lowercase) for i in range(10))
         if self.ortho:
-            ants.plot_ortho(image, filename=os.path.join(self.base_dir, filename+'.png'))
+            nt.plot_ortho(image, filename=os.path.join(self.base_dir, filename+'.png'))
         else:
-            ants.plot(image, filename=os.path.join(self.base_dir, filename+'.png'))
+            nt.plot(image, filename=os.path.join(self.base_dir, filename+'.png'))
         return image
 
 
 class CustomFunction(BaseTransform):
     """
     Apply a user-supplied function as a transform
     """
```

### Comparing `nitrain-0.2.2/nitrain/utils.py` & `nitrain-0.3.0/nitrain/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import os
-import ants
+import ntimage as nt
 import numpy as np
 
 def get_nitrain_dir():
     if os.environ.get('NITRAIN_DIR') is not None:
         nitrain_dir = os.environ['NITRAIN_DIR']
     else:
         nitrain_dir = os.path.join(os.path.expanduser('~'), '.nitrain')
@@ -14,13 +14,13 @@
         
     return nitrain_dir    
 
 def files_to_array(files, dtype='float32'):
     # read in the images to a numpy array
     img_arrays = []
     for file in files:
-        img = ants.image_read(file)
+        img = nt.load(file)
         img_array = img.numpy()
         img_arrays.append(img_array)
         
     img_arrays = np.array(img_arrays, dtype=dtype)
     return img_arrays
```

### Comparing `nitrain-0.2.2/PKG-INFO` & `nitrain-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,87 @@
-Metadata-Version: 2.1
-Name: nitrain
-Version: 0.2.2
-Summary: High-level framework for training medical imaging AI models
-License: MIT
-Author: ncullen93
-Author-email: nicholas.cullen@med.lu.se
-Requires-Python: >=3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: antspynet (>=0.2.3,<0.3.0)
-Requires-Dist: antspyx (>=0.4.2,<0.5.0)
-Requires-Dist: boto3 (>=1.34.49,<2.0.0)
-Requires-Dist: datalad (>=0.19.6,<0.20.0)
-Requires-Dist: google-auth (>=2.28.2,<3.0.0)
-Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
-Requires-Dist: google-cloud-storage (>=2.15.0,<3.0.0)
-Requires-Dist: ipython (==8.14)
-Requires-Dist: nibabel (>=5.2.0,<6.0.0)
-Requires-Dist: parse (>=1.20.1,<2.0.0)
-Requires-Dist: pybids (>=0.16.4,<0.17.0)
-Requires-Dist: pydot (>=2.0.0,<3.0.0)
-Requires-Dist: tensorflow (==2.12)
-Requires-Dist: tensorflow-probability (==0.20)
-Requires-Dist: torch (>=2.2.1,<3.0.0)
-Description-Content-Type: text/markdown
+# Nitrain - a framework for medical imaging AI
 
-# Nitrain - a framework for medical imaging-native AI
-
-[![Coverage Status](https://coveralls.io/repos/github/ncullen93/nitrain/badge.svg?branch=main)](https://coveralls.io/github/ncullen93/nitrain?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/nitrain/nitrain/badge.svg?branch=main)](https://coveralls.io/github/nitrain/nitrain?branch=main)
 [![Build](https://github.com/ncullen93/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/ncullen93/nitrain/actions/workflows/test.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nitrain)
 
 Nitrain (formerly <i>torchsample</i>) provides tools for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing model results in a medical imaging context. It supports using pytorch, keras, and tensorflow.
 
-You can also train models HIPAA-compliantly in the cloud using nitrain. You are encouraged to make your fitted models available to the community via nitrain, or you can easily use other's pretrained models for fine-tuning or standard image processing.
-
-<br />
-
-## Installation
-
-The latest release of nitrain can be installed from pypi:
-
-```
-pip install nitrain
-```
-
-Or you can install the latest development version directly from github:
-
-```
-python -m pip install git+github.com/ncullen93/nitrain.git
-```
-
-### Dependencies
-
-The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
+To learn how to use nitrain or to view complete examples of training medical imaging AI models using nitrain, visit [github.com/nitrain/tutorials](https://github.com/nitrain/tutorials) or view the rendered version at [nitrain.dev/docs](https://nitrain.dev/docs). If you want to learn more generally about medical imaging AI, check out the book [Becoming a medical imaging AI expert with Python](https://book.nitrain.dev).
 
 <br />
 
 ## Quickstart
 
 Here is a canonical example of using nitrain to fit a brain-age model. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
 
 ```python
-from nitrain import datasets, loaders, models, trainers, transforms as tx
+import nitrain as nt
+from nitrain.readers import PatternReader, ColumnReader
 
 # create dataset from folder of images + participants file
-dataset = datasets.FolderDataset(base_dir='ds004711',
-                                 x={'pattern': 'sub-*/anat/*_T1w.nii.gz'},
-                                 y={'file': 'participants.tsv',
-                                         'column': 'age'},
-                                 x_transforms=[tx.Resize((64,64,64)),
-                                               tx.NormalizeIntensity(0,1)])
+dataset = nt.Dataset(inputs=PatternReader('sub-*/anat/*_T1w.nii.gz'),
+                          outputs=ColumnReader('participants.tsv', 'age'),
+                          transforms={
+                              'inputs': [tx.Resize((64,64,64)), tx.NormalizeIntensity(0,1)],
+                          },
+                          base_dir='~/desktop/ds004711/')
 
 # create loader with random transforms
-loader = loaders.DatasetLoader(dataset,
-                               images_per_batch=4,
-                               shuffle=True,
-                               sampler=samplers.SliceSampler(batch_size=32, axis=2)
-                               x_transforms=[tx.RandomNoise(sd=0.2)])
+loader = nt.Loader(dataset,
+                        images_per_batch=4,
+                        shuffle=True,
+                        sampler=nitrain.SliceSampler(batch_size = 32, axis = 2)
+                        transforms={
+                                'inputs': tx.RandomNoise(sd=0.2)
+                        })
 
 # create model from architecture
-arch_fn = models.fetch_architecture('alexnet', dim=2)
+arch_fn = nt.fetch_architecture('alexnet', dim=2)
 model = arch_fn(input_image_size=(64,64,1),
                 number_of_outcomes=1,
                 mode='regression')
 
 # create trainer and fit model
-trainer = trainers.ModelTrainer(model,
-                                loss='mse',
-                                optimizer='adam',
-                                lr=1e-3,
-                                callbacks=[utils.EarlyStopping(),
-                                           utils.ModelCheckpoints(freq=25)])
+trainer = nt.Trainer(model,
+                          loss='mse',
+                          optimizer='adam',
+                          lr=1e-3,
+                          callbacks=[utils.EarlyStopping(),
+                                     utils.ModelCheckpoints(freq=25)])
 trainer.fit(loader, epochs=100)
 
 # upload trained model to platform
-models.register_model(trainer.model, 'nick/t1-brain-age')
+nt.register_model(trainer.model, 'nick/t1-brain-age')
 ```
 
 A more in-depth introduction can be found in the [tutorials](github.com/ncullen93/nitrain) and if you can also check out the [examples](github.com/ncullen93/nitrain) for self-contained notebooks showing how to perform common deep learning tasks.
 
 <br />
 
+## Installation
+
+The latest release of nitrain can be installed from pypi:
+
+```
+pip install nitrain
+```
+
+Or you can install the latest development version directly from github:
+
+```
+python -m pip install git+github.com/ncullen93/nitrain.git
+```
+
+### Dependencies
+
+The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
+
+<br />
+
 ## Overview of nitrain
 
 The 10-minute overview presented below will take you through the key components of nitrain:
 
 - [Datasets and Loaders](#datasets-and-loaders)
 - [Samplers](#samplers)
 - [Transforms](#transforms)
@@ -118,15 +89,15 @@
 - [Model trainers](#model-trainers)
 - [Explainers](#explainers)
 
 <br />
 
 ### Datasets and Loaders
 
-Datasets help you read in your images from wherever they are stored -- in a local folder with BIDS or datalad, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, BIDS entities, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
+Datasets help you read in your images from wherever they are stored -- in a local folder, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
 
 ```python
 from nitrain import datasets, transforms as tx
 
 dataset = datasets.FolderDataset(base_dir='~/datasets/ds004711',
                                  x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
                                  y={'file': 'participants.tsv', 'column': 'age'},
@@ -194,24 +165,24 @@
 
 my_tx = tx.CustomTransform(lambda x: x * 2)
 ```
 
 If you want to explore what a transform does, you can take a sample of it over any number of trials on the same image and then plot the results:
 
 ```python
-import ants
+import ntimage as nt
 import numpy as np
 from nitrain import transforms as tx
 
-img = ants.image_read(ants.get_data('r16'))
+img = nt.load(nt.example_data('r16'))
 
 my_tx = tx.RandomSmoothing(0, 2)
 imgs = my_tx.sample(img, n=12)
 
-ants.plot_grid(np.array(imgs).reshape(4,3))
+nt.plot_grid(imgs, shape=(4,3))
 ```
 
 <br />
 
 ### Architectures and pretrained models
 
 The nitrain package provides an interface to an extensive amount of deep learning model architectures for all kinds of tasks - regression, classification, image-to-image generation, segmentation, autoencoders, etc.
@@ -237,18 +208,18 @@
 
 <br />
 
 ### Trainers
 
 After you have created a model from a nitrain architecture, fetched a pretrained model, or created a model yourself in your framework of choice, then it's time to actually train the model on the dataset / loader that you've created.
 
-Although you are free to train models on loaders using standard pytorch, keras, or tensorflow workflows, we also provide the `ModelTrainer` class to make training even easier. This class provides sensible defaults for key training parameters based on your task.
+Although you are free to train models on loaders using standard pytorch, keras, or tensorflow workflows, we also provide the `LocalTrainer` class to make training even easier. This class provides sensible defaults for key training parameters based on your task.
 
 ```python
-trainer = trainers.ModelTrainer(model=vgg_model, task='regression')
+trainer = trainers.LocalTrainer(model=vgg_model, task='regression')
 trainer.fit(loader, epochs=10)
 
 # access fitted model
 print(trainer.model)
 ```
 
 If you have signed up for an account at [nitrain.dev](https://www.nitrain.dev) then you can also train your model in the cloud using the `PlatformTrainer` class. All training takes place on HIPAA-compliant GPU servers with competitive pricing.
@@ -271,8 +242,7 @@
 Nitrain provides tools to perform this techique - along with many others - and can help you visualize the results of such explainability experiments directly in brain space. Here is what that might look like:
 
 <br />
 
 ## Contributing
 
 If you would like to contribute to nitrain, we would be extremely thankful. The best way to start is by posting an issue to discuss your proposed feature.
-
```

