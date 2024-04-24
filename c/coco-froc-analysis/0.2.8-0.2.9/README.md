# Comparing `tmp/coco_froc_analysis-0.2.8.tar.gz` & `tmp/coco_froc_analysis-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coco_froc_analysis-0.2.8.tar", max compression
+gzip compressed data, was "coco_froc_analysis-0.2.9.tar", max compression
```

## Comparing `coco_froc_analysis-0.2.8.tar` & `coco_froc_analysis-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2021-03-08 12:57:59.751706 coco_froc_analysis-0.2.8/LICENSE
--rw-r--r--   0        0        0     5438 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.8/README.md
--rw-r--r--   0        0        0       97 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/__init__.py
--rw-r--r--   0        0        0      109 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/__main__.py
--rw-r--r--   0        0        0     4095 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/cli_froc_analysis.py
--rw-r--r--   0        0        0      234 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/count/__init__.py
--rw-r--r--   0        0        0     8944 2023-10-02 07:41:54.914492 coco_froc_analysis-0.2.8/coco_froc_analysis/count/bootstrap_count_curve.py
--rw-r--r--   0        0        0     5978 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.8/coco_froc_analysis/count/count_curve.py
--rw-r--r--   0        0        0     3380 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/count/count_stats.py
--rw-r--r--   0        0        0      228 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/froc/__init__.py
--rw-r--r--   0        0        0     8705 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.8/coco_froc_analysis/froc/bootstrap_froc_curve.py
--rw-r--r--   0        0        0     6548 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.8/coco_froc_analysis/froc/froc_curve.py
--rw-r--r--   0        0        0     4320 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/froc/froc_stats.py
--rw-r--r--   0        0        0     4730 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.8/coco_froc_analysis/utils.py
--rw-r--r--   0        0        0      822 2023-10-02 07:45:44.744855 coco_froc_analysis-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 coco_froc_analysis-0.2.8/setup.py
--rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 coco_froc_analysis-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-03-08 12:57:59.751706 coco_froc_analysis-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5438 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.9/README.md
+-rw-r--r--   0        0        0       97 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/__init__.py
+-rw-r--r--   0        0        0      109 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/__main__.py
+-rw-r--r--   0        0        0     4095 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/cli_froc_analysis.py
+-rw-r--r--   0        0        0      234 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/count/__init__.py
+-rw-r--r--   0        0        0     9147 2023-10-02 17:02:02.951269 coco_froc_analysis-0.2.9/coco_froc_analysis/count/bootstrap_count_curve.py
+-rw-r--r--   0        0        0     5978 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.9/coco_froc_analysis/count/count_curve.py
+-rw-r--r--   0        0        0     3380 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/count/count_stats.py
+-rw-r--r--   0        0        0      228 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/froc/__init__.py
+-rw-r--r--   0        0        0     8909 2023-10-02 17:02:23.824923 coco_froc_analysis-0.2.9/coco_froc_analysis/froc/bootstrap_froc_curve.py
+-rw-r--r--   0        0        0     6548 2023-10-02 07:37:18.444353 coco_froc_analysis-0.2.9/coco_froc_analysis/froc/froc_curve.py
+-rw-r--r--   0        0        0     4320 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/froc/froc_stats.py
+-rw-r--r--   0        0        0     4730 2023-10-02 07:34:33.395097 coco_froc_analysis-0.2.9/coco_froc_analysis/utils.py
+-rw-r--r--   0        0        0      822 2023-10-02 17:02:48.426872 coco_froc_analysis-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 coco_froc_analysis-0.2.9/setup.py
+-rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 coco_froc_analysis-0.2.9/PKG-INFO
```

### Comparing `coco_froc_analysis-0.2.8/LICENSE` & `coco_froc_analysis-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/README.md` & `coco_froc_analysis-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/cli_froc_analysis.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/cli_froc_analysis.py`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/count/bootstrap_count_curve.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/count/bootstrap_count_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -283,12 +283,17 @@
 
     if bounds is not None:
         x_min, x_max, _, _ = bounds
         ax.set_xlim([x_min, x_max])
     else:
         ax.set_xlim([.7, 1.0])
         ax.set_ylim(bottom=0.05, top=1.02)
+        
+    ax.spines['top'].set_visible(False)
+    ax.spines['right'].set_visible(False)
+    ax.spines['left'].set_visible(False)
+    ax.grid(True, which='both', axis='both', alpha=.3, linestyle='--')
     fig.tight_layout()
     fig.savefig(plot_output_path, dpi=150)
 
     os.remove('/tmp/tmp_bootstrap_gt.json')
     os.remove('/tmp/tmp_bootstrap_pred.json')
```

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/count/count_curve.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/count/count_curve.py`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/count/count_stats.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/count/count_stats.py`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/froc/bootstrap_froc_curve.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/froc/bootstrap_froc_curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,12 +273,18 @@
 
     if bounds is not None:
         x_min, x_max, y_min, y_max = bounds
         ax.set_ylim([y_min, y_max])
         ax.set_xlim([x_min, x_max])
     else:
         ax.set_ylim(bottom=0.05, top=1.02)
+    
+    ax.spines['top'].set_visible(False)
+    ax.spines['right'].set_visible(False)
+    ax.spines['left'].set_visible(False)
+    ax.grid(True, which='both', axis='both', alpha=.3, linestyle='--')
+    
     fig.tight_layout()
     fig.savefig(fname=plot_output_path, dpi=150)
 
     os.remove('/tmp/tmp_bootstrap_gt.json')
     os.remove('/tmp/tmp_bootstrap_pred.json')
```

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/froc/froc_curve.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/froc/froc_curve.py`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/froc/froc_stats.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/froc/froc_stats.py`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/coco_froc_analysis/utils.py` & `coco_froc_analysis-0.2.9/coco_froc_analysis/utils.py`

 * *Files identical despite different names*

### Comparing `coco_froc_analysis-0.2.8/pyproject.toml` & `coco_froc_analysis-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coco-froc-analysis"
-version = "0.2.8"
+version = "0.2.9"
 description = "FROC analysis for COCO detections for Detectron(2) and OpenMMLab"
 authors = ["Alex Olar <olaralex666@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "coco_froc_analysis"}]
 
 [tool.poetry.dependencies]
```

### Comparing `coco_froc_analysis-0.2.8/setup.py` & `coco_froc_analysis-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.23.5,<2.0.0',
  'scipy>=1.9.3,<2.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'coco-froc-analysis',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'FROC analysis for COCO detections for Detectron(2) and OpenMMLab',
     'long_description': '# COCO FROC analysis\n\nFROC analysis for COCO annotations and Detectron(2) detection results. The COCO annotation style is defined [here](https://cocodataset.org/).\n\n### Installation\n\n```bash\npip install coco-froc-analysis\n```\n\n### About\n\nA single annotation record in the ground-truth file might look like this:\n\n```json\n{\n  "area": 2120,\n  "iscrowd": 0,\n  "bbox": [111, 24, 53, 40],\n  "category_id": 3,\n  "ignore": 0,\n  "segmentation": [],\n  "image_id": 407,\n  "id": 945\n}\n```\n\nWhile the prediction (here for bounding box) given by the region detection framework is such:\n\n```json\n{\n  "image_id": 407,\n  "category_id": 3,\n  "score": 0.9990422129631042,\n  "bbox": [\n    110.72555541992188,\n    13.9161834716797,\n    49.4566650390625,\n    36.65155029296875\n  ]\n}\n```\n\nThe FROC analysis counts the number of images, number of lesions in the ground truth file for all categories and then counts the lesion localization predictions and the non-lesion localization predictions. A lesion is localized by default if its center is inside any ground truth box and the categories match or if you wish to use IoU you should provide threshold upon which you can define the \'close enough\' relation.\n\n## Usage\n\n```python\nfrom coco_froc_analysis.count import generate_bootstrap_count_curves\nfrom coco_froc_analysis.count import generate_count_curve\nfrom coco_froc_analysis.froc import generate_bootstrap_froc_curves\nfrom coco_froc_analysis.froc import generate_froc_curve\n\n# For single FROC curve\ngenerate_froc_curve(\n            gt_ann=args.gt_ann,\n            pr_ann=args.pr_ann,\n            use_iou=args.use_iou,\n            iou_thres=args.iou_thres,\n            n_sample_points=args.n_sample_points,\n            plot_title=\'FROC\' if args.plot_title is None else args.plot_title,\n            plot_output_path=\'froc.png\' if args.plot_output_path is None else args.plot_output_path,\n            test_ann=args.test_ann,\n        )\n\n# For bootstrapped curves\ngenerate_bootstrap_froc_curves(\n            gt_ann=args.gt_ann,\n            pr_ann=args.pr_ann,\n            n_bootstrap_samples=args.bootstrap,\n            use_iou=args.use_iou,\n            iou_thres=args.iou_thres,\n            n_sample_points=args.n_sample_points,\n            plot_title=\'FROC (bootstrap)\' if args.plot_title is None else args.plot_title,\n            plot_output_path=\'froc_bootstrap.png\' if args.plot_output_path is None else args.plot_output_path,\n            test_ann=args.test_ann,\n        )\n```\n\nPlease check `run.py` for more details. The `IoU` part of this code is not reliable and currently the codebase only works for binary evaluation, but any multiclass problem could be chunked up to work with it.\n\nDescription of `run.py` arguments:\n\n```bash\nusage: run.py [-h] [--bootstrap BOOTSTRAP] --gt_ann GT_ANN --pr_ann PR_ANN [--use_iou] [--iou_thres IOU_THRES] [--n_sample_points N_SAMPLE_POINTS]\n              [--plot_title PLOT_TITLE] [--plot_output_path PLOT_OUTPUT_PATH] [--test_ann TEST_ANN] [--counts] [--weighted]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --bootstrap BOOTSTRAP\n                        Whether to do a single or bootstrap runs.\n  --gt_ann GT_ANN\n  --pr_ann PR_ANN\n  --use_iou             Use IoU score to decide based on `proximity`\n  --iou_thres IOU_THRES\n                        If IoU score is used the default threshold is set to .5\n  --n_sample_points N_SAMPLE_POINTS\n                        Number of points to evaluate the FROC curve at.\n  --plot_title PLOT_TITLE\n  --plot_output_path PLOT_OUTPUT_PATH\n  --test_ann TEST_ANN   Extra ground-truth like annotations\n  --counts\n  --weighted\n```\n\n## CLI Usage\n\n```bash\npython -m coco_froc_analysis [-h] [--bootstrap N_BOOTSTRAP_ROUNDS] --gt_ann GT_ANN --pred_ann PRED_ANN [--use_iou] [--iou_thres IOU_THRES] [--n_sample_points N_SAMPLE_POINTS]\n                        [--plot_title PLOT_TITLE] [--plot_output_path PLOT_OUTPUT_PATH]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --bootstrap  N_ROUNDS Whether to do a single or bootstrap runs.\n  --gt_ann GT_ANN\n  --pred_ann PRED_ANN\n  --use_iou             Use IoU score to decide on `proximity` rather then using center pixel inside GT box.\n  --iou_thres IOU_THRES\n                        If IoU score is used the default threshold is arbitrarily set to .5\n  --n_sample_points N_SAMPLE_POINTS\n                        Number of points to evaluate the FROC curve at.\n  --plot_title PLOT_TITLE\n  --plot_output_path PLOT_OUTPUT_PATH\n```\n\nBy default centroid closeness is used, if the `--use_iou` flag is set, `--iou_thres` defaults to `.75` while the `--score_thres` score defaults to `.5`. The code outputs the FROC curve on the given detection results and GT dataset.\n\n## For developers\n\n### Running tests\n\n```bash\npython -m coverage run -m unittest discover --pattern "*_test.py" -v\npython -m coverage report -m\n```\n\n### Building and publishing (reminder)\n\n```bash\nact # for local CI pipeline\npdoc -d google coco_froc_analysis -o docs # build docs\npoetry version prerelease/patch # test or actual release\npoetry publish --build -r test-pypi # or without -r test-pypi for publishing to pypi\n```\n\n@Regards, Alex\n\n```\n@misc{qbeer,\n  author       = {Alex Olar},\n  title        = {FROC analysis for COCO-like file format},\n  howpublished = {GitHub repository},\n  month        = {September},\n  year         = {2022},\n  url          = {https://github.com/qbeer/coco-froc-analysis}\n}\n```\n',
     'author': 'Alex Olar',
     'author_email': 'olaralex666@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `coco_froc_analysis-0.2.8/PKG-INFO` & `coco_froc_analysis-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coco-froc-analysis
-Version: 0.2.8
+Version: 0.2.9
 Summary: FROC analysis for COCO detections for Detectron(2) and OpenMMLab
 License: MIT
 Author: Alex Olar
 Author-email: olaralex666@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

