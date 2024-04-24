# Comparing `tmp/waretomo-0.1.3.tar.gz` & `tmp/waretomo-0.1.4.tar.gz`

## Comparing `waretomo-0.1.3.tar` & `waretomo-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 waretomo-0.1.3/.cruft.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 waretomo-0.1.3/.github_changelog_generator
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 waretomo-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 waretomo-0.1.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 waretomo-0.1.3/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 waretomo-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 waretomo-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_aretomo.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_fix.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_fix_mdoc.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_parse.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_stack.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_threaded.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/_topaz.py
--rw-r--r--   0        0        0    12509 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 waretomo-0.1.3/src/waretomo/py.typed
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 waretomo-0.1.3/tests/test_waretomo.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 waretomo-0.1.3/.gitignore
--rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 waretomo-0.1.3/LICENSE
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 waretomo-0.1.3/README.md
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 waretomo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 waretomo-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 waretomo-0.1.4/.cruft.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github_changelog_generator
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 waretomo-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 waretomo-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/__init__.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_aretomo.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_fix_mdoc.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_parse.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_stack.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_threaded.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/_topaz.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 waretomo-0.1.4/src/waretomo/py.typed
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 waretomo-0.1.4/tests/test_waretomo.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 waretomo-0.1.4/.gitignore
+-rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 waretomo-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 waretomo-0.1.4/README.md
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 waretomo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 waretomo-0.1.4/PKG-INFO
```

### Comparing `waretomo-0.1.3/.cruft.json` & `waretomo-0.1.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.3/.pre-commit-config.yaml` & `waretomo-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.3/.github/workflows/ci.yml` & `waretomo-0.1.4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         python-version: ['3.9', '3.10', '3.11']
         platform: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache-dependency-path: "pyproject.toml"
           cache: "pip"
 
       # if running a cron job, we add the --pre flag to test against pre-releases
       - name: Install dependencies
@@ -60,15 +60,15 @@
           RUN_ID: ${{ github.run_id }}
           TITLE: '[test-bot] pip install --pre is failing'
         with:
           filename: .github/TEST_FAIL_TEMPLATE.md
           update_existing: true
 
       - name: Coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
 
   deploy:
     name: Deploy
     needs: test
     if: success() && startsWith(github.ref, 'refs/tags/') && github.event_name != 'schedule'
     runs-on: ubuntu-latest
     permissions:
@@ -76,15 +76,15 @@
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: install
         run: |
           pip install -U pip build twine
           python -m build
@@ -92,10 +92,10 @@
 
       - name: Build and publish
         run: twine upload dist/*
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
 
-      - uses: softprops/action-gh-release@v1
+      - uses: softprops/action-gh-release@v2
         with:
           generate_release_notes: true
```

### Comparing `waretomo-0.1.3/src/waretomo/_aretomo.py` & `waretomo-0.1.4/src/waretomo/_aretomo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import logging
 import os
 import shutil
 import subprocess
 from contextlib import contextmanager
 from pathlib import Path
 from queue import Queue
 from time import sleep
 
 import GPUtil
-from rich import print
 
 from ._threaded import run_threaded
 
 
 @contextmanager
 def _cd(dir):
     prev = os.getcwd()
@@ -40,30 +40,30 @@
     kv=0,
     dose=0,
     cs=0,
     defocus=0,
     reconstruct=False,
     gpu_queue=None,
     dry_run=False,
-    verbose=False,
     overwrite=False,
 ):
+    log = logging.getLogger("waretomo")
     # cwd dance is necessary cause aretomo messes up paths otherwise
     # need to use os.path.relpath cause pathlib cannot handle non-subpath relative paths
     # https://stackoverflow.com/questions/38083555/using-pathlibs-relative-to-for-directories-on-the-same-level
     cwd = output.parent.absolute()
     input_ = Path(os.path.relpath(input_, cwd))
     rawtlt = Path(os.path.relpath(rawtlt, cwd))
     aln = Path(os.path.relpath(aln, cwd))
     xf = Path(os.path.relpath(xf, cwd))
     output = Path(os.path.relpath(output, cwd))
     if not reconstruct:
         output = output.with_stem(output.stem + "_aligned").with_suffix(".st")
     # LogFile is broken, so we do it ourselves
-    log = output.with_suffix(".aretomolog")
+    aretomolog = output.with_suffix(".aretomolog")
     with _cd(cwd):
         if not overwrite and output.exists():
             raise FileExistsError(output)
 
     # only one job per gpu
     gpu = 0 if gpu_queue is None else gpu_queue.get()
 
@@ -79,21 +79,23 @@
     if reconstruct:
         options.update(
             {
                 "AlnFile": aln,
                 "VolZ": thickness_recon,
                 "PixSize": px_size,
                 "Kv": kv,
-                "ImgDose": dose,
                 "Cs": cs,
                 "Defoc": defocus,
                 "FlipVol": 1,
                 "WBP": 1,
             }
         )
+        if dose:
+            options["ImgDose"] = dose
+
     else:
         options.update(
             {
                 "AngFile": rawtlt,
                 "AlignZ": thickness_align,
                 "TiltCor": int(tilt_corr),
                 "VolZ": 0,
@@ -105,27 +107,26 @@
             options["RoiFile"] = roi_file
         if patches is not None:
             options["Patch"] = f"{patches} {patches}"
 
     # run aretomo with basic settings
     aretomo_cmd = f"{cmd} {' '.join(f'-{k} {v}' for k, v in options.items())}"
 
-    if verbose:
-        print(aretomo_cmd)
-        if not reconstruct:
-            print(f'mv {xf} {warp_mdoc_basename + ".xf"}')
+    log.info(aretomo_cmd)
+    if not reconstruct:
+        log.info(f'mv {xf} {warp_mdoc_basename + ".xf"}')
 
     if not dry_run:
         with _cd(cwd):
             try:
                 proc = subprocess.run(
                     aretomo_cmd.split(), capture_output=True, check=False, cwd=cwd
                 )
             finally:
-                log.write_bytes(proc.stdout + proc.stderr)
+                aretomolog.write_bytes(proc.stdout + proc.stderr)
                 if gpu_queue is not None:
                     gpu_queue.put(gpu)
             proc.check_returncode()
         if not reconstruct:
             # move xf file so warp can see it (needs full ts name + .xf)
             shutil.move(cwd / xf, cwd / (warp_mdoc_basename + ".xf"))
     else:
@@ -133,33 +134,33 @@
         if gpu_queue is not None:
             gpu_queue.put(gpu)
 
 
 def aretomo_batch(
     progress, tilt_series, suffix="", label="", cmd="AreTomo", gpus=None, **kwargs
 ):
+    log = logging.getLogger("waretomo")
     if not shutil.which(cmd):
         raise FileNotFoundError(f"{cmd} is not available on the system")
     if gpus is None:
         gpus = [gpu.id for gpu in GPUtil.getGPUs()]
     if not gpus:
         raise RuntimeError("you need at least one GPU to run AreTomo")
-    if kwargs.get("verbose"):
-        print(f"[yellow]Running AreTomo in parallel on {len(gpus)} GPUs.")
+    log.info(f"Running AreTomo in parallel on {len(gpus)} GPUs.")
 
     # use a queue to hold gpu ids to ensure we only run one job per gpu
     gpu_queue = Queue()
     for gpu in gpus:
         gpu_queue.put(gpu)
 
     partials = []
     for ts in tilt_series:
         partials.append(
             lambda ts=ts: _aretomo(
-                input_=ts["stack" + suffix] if suffix else ts["fix"],
+                input_=ts["stack" + suffix],
                 rawtlt=ts["rawtlt"],
                 aln=ts["aln"],
                 xf=ts["xf"],
                 roi_file=ts["roi"],
                 output=ts["recon" + suffix],
                 gpu_queue=gpu_queue,
                 cmd=cmd,
```

### Comparing `waretomo-0.1.3/src/waretomo/_fix_mdoc.py` & `waretomo-0.1.4/src/waretomo/_fix_mdoc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+import logging
+
 import pandas as pd
 from mdocfile.data_models import Mdoc
 
 from ._threaded import run_threaded
 
 
-def _tilt_mdoc(
-    mdoc_file, tlt_file, skipped_tilts, verbose=False, dry_run=False, overwrite=False
-):
+def _tilt_mdoc(mdoc_file, tlt_file, skipped_tilts, dry_run=False, overwrite=False):
     output = mdoc_file.parent / "mdoc_tilted" / mdoc_file.name
 
     if not overwrite and output.exists():
         raise FileExistsError(output)
 
-    if verbose:
-        print(f"Tilting mdoc: {mdoc_file}")
-        print(f"using: {tlt_file}")
-        print(f"saving to {output}")
+    log = logging.getLogger("waretomo")
+    log.info(f"Tilting mdoc: {mdoc_file}")
+    log.info(f"using: {tlt_file}")
+    log.info(f"saving to {output}")
 
     if not dry_run:
         mdoc = Mdoc.from_file(mdoc_file)
         new_angles = iter(pd.read_csv(tlt_file, header=None)[0])
         # mdoc is still out of order, but aretomo puts the new_angles in order
         # this gives us tuples like (original_index, section), but ordered by angle
         # like aretomo so we can compare it with the new angles
```

### Comparing `waretomo-0.1.3/src/waretomo/_parse.py` & `waretomo-0.1.4/src/waretomo/_parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import logging
 from pathlib import Path, PureWindowsPath
 from xml.etree import ElementTree
 
 from mdocfile.data_models import Mdoc
-from rich import print
 
 
 def parse_data(
     progress, warp_dir, mdoc_dir, output_dir, roi_dir, just=(), exclude=(), train=False
 ):
+    log = logging.getLogger("waretomo")
+
     imod_dir = warp_dir / "imod"
     if not imod_dir.exists():
         raise FileNotFoundError("warp directory does not have an `imod` subdirectory")
 
     if just:
         mdocs = [
             p
@@ -54,20 +56,18 @@
         ]
         skipped_tilts = []
         odd = []
         even = []
         valid_xml = None
         for i, tilt in enumerate(tilts):
             if not tilt.exists():
-                print(
-                    f"[red]WARN: {tilt.name} is listed in an mdoc file, "
-                    "but the file does not exists."
-                )
-                print(
-                    "[red]      The tilt will be skipped, "
+                log.warning(
+                    f"{tilt.name} is listed in an mdoc file, "
+                    "but the file does not exists. "
+                    "The tilt will be skipped, "
                     "but you may want to check your data."
                 )
                 skipped_tilts.append(i)
                 continue
 
             xml = ElementTree.parse(tilt.with_suffix(".xml")).getroot()
             if xml.attrib["UnselectManual"] == "True":
@@ -106,40 +106,47 @@
             if len(roi_files) == 1:
                 roi_file = roi_files[0]
             else:
                 roi_file = None
         else:
             roi_file = None
 
-        ts_fixed = ts_name + "_fix"
+        dose = mdoc.section_data[0].ExposureDose
+        if not dose:
+            log.error("Exposure dose not present in mdoc! Setting to 0.")
+        px_size_raw = mdoc.section_data[0].PixelSpacing
+        if not px_size_raw:
+            log.error("Pixel spacing not present in mdoc! Setting to 1.")
+
+        # aretomo being weird about paths and names splitting needs extra care...
         ts_stripped = ts_name.split(".")[0]
-        alignment_result_dir = output_dir / (ts_stripped + "_Imod")
+        ts_aligned = ts_stripped + "_aligned"
+        alignment_result_dir = output_dir / (ts_aligned + ".st_Imod")
 
         tilt_series.append(
             {
                 "name": ts_name,
                 "stack": stack,
                 "rawtlt": stack.with_suffix(".rawtlt"),
-                "fix": output_dir / (ts_fixed + ".st"),
                 "aln": output_dir / (ts_stripped + ".aln"),
-                "xf": alignment_result_dir / (ts_stripped + ".xf"),
-                "tlt": alignment_result_dir / (ts_stripped + ".tlt"),
+                "xf": alignment_result_dir / (ts_aligned + ".xf"),
+                "tlt": alignment_result_dir / (ts_aligned + ".tlt"),
                 "skipped_tilts": skipped_tilts,
                 "mdoc": mdoc_file,
                 "roi": roi_file,
                 "odd": odd,
                 "even": even,
                 "stack_odd": output_dir / (ts_name + "_odd.st"),
                 "stack_even": output_dir / (ts_name + "_even.st"),
                 "recon_odd": output_dir / "odd" / (ts_name + ".mrc"),
                 "recon_even": output_dir / "even" / (ts_name + ".mrc"),
                 "recon": output_dir / (ts_name + ".mrc"),
                 "aretomo_kwargs": {
-                    "dose": mdoc.section_data[0].ExposureDose,
-                    "px_size": mdoc.section_data[0].PixelSpacing * 2**binning,
+                    "dose": dose,
+                    "px_size": px_size_raw * 2**binning,
                     "cs": cs,
                     "kv": kv,
                     "defocus": defocus,
                 },
             }
         )
```

### Comparing `waretomo-0.1.3/src/waretomo/_stack.py` & `waretomo-0.1.4/src/waretomo/_stack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
+import logging
 import shutil
 import subprocess
 from time import sleep
 
-from rich import print
-
 from ._threaded import run_threaded
 
 
-def _stack(
-    images, output, cmd="newstack", dry_run=False, verbose=False, overwrite=False
-):
+def _stack(images, output, cmd="newstack", dry_run=False, overwrite=False):
     if not overwrite and output.exists():
         raise FileExistsError(output)
     stack_cmd = f'{cmd} {" ".join(str(img) for img in images)} {output}'
 
-    if verbose:
-        short_cmd = f"{cmd} {images[0]} [...] {images[-1]} {output}"
-        print(short_cmd)
+    log = logging.getLogger("waretomo")
+    short_cmd = f"{cmd} {images[0]} [...] {images[-1]} {output}"
+    log.info(short_cmd)
 
     if not dry_run:
         subprocess.run(stack_cmd.split(), capture_output=True, check=True)
     else:
         sleep(0.1)
```

### Comparing `waretomo-0.1.3/src/waretomo/_threaded.py` & `waretomo-0.1.4/src/waretomo/_threaded.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+import logging
 import os
 import subprocess
 from concurrent import futures
 
-from rich import print
-
 
 def run_threaded(
     progress,
     partials,
     label="",
     max_workers=None,
     dry_run=False,
-    verbose=False,
     **kwargs,
 ):
     max_workers = max_workers or min(32, os.cpu_count() + 4)  # see concurrent docs
 
+    log = logging.getLogger("waretomo")
+
     with futures.ThreadPoolExecutor(max_workers) as executor:
         main_task = progress.add_task(f"{label}...", total=len(partials))
 
         jobs = []
         for fn in partials:
             job = executor.submit(fn)
             jobs.append(job)
@@ -33,24 +33,22 @@
         for job in futures.as_completed(jobs):
             try:
                 job.result()
             except FileExistsError:
                 exist += 1
             except subprocess.CalledProcessError as e:
                 errors.append(e)
-                if verbose:
-                    print(e)
+                log.warning("Subprocess failed with:")
             progress.update(main_task, advance=1)
 
         for t in tasks:
             progress.update(t, total=1, completed=1, visible=False)
 
         if exist:
-            print(f"[red]{label}: {exist} files already exist and were not overwritten")
+            log.warn(f"{label}: {exist} files already exist and were not overwritten")
 
         if errors:
-            print(f"[red]{label}: {len(errors)} commands have failed:")
+            log.error(f"{label}: {len(errors)} commands have failed:")
             for err in errors:
-                print(
-                    f'[yellow]{" ".join(err.cmd)}[/yellow] '
-                    f"failed with:\n[red]{err.stderr.decode()}"
+                log.error(
+                    f'{" ".join(err.cmd)} ' f"failed with:\n{err.stderr.decode()}"
                 )
```

### Comparing `waretomo-0.1.3/src/waretomo/_topaz.py` & `waretomo-0.1.4/src/waretomo/_topaz.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import io
+import logging
 import multiprocessing
 import re
 import time
 from concurrent import futures
 
-from rich import print
 from topaz.commands.denoise3d import denoise, load_model, set_device, train_model
 from topaz.torch import set_num_threads
 
 
 def _run_and_update_progress(progress, task, func, *args, **kwargs):
     std = io.StringIO()
 
@@ -48,27 +48,26 @@
     odd,
     model_name="unet-3d-10a",
     train=False,
     tile_size=32,
     patch_size=32,
     gpus=None,
     dry_run=False,
-    verbose=False,
     overwrite=False,
 ):
     inputs = [ts["recon"] for ts in tilt_series]
 
-    if verbose:
-        if train:
-            print(f"training model: '{model_name}' with inputs '{even}' and '{odd}'")
-        if len(inputs) > 2:
-            print(f"denoising: [{inputs[0]} [...] {inputs[-1]}]")
-        else:
-            print(f"denoising: {inputs}")
-        print(f"output: {outdir}")
+    log = logging.getLogger("waretomo")
+    if train:
+        log.info(f"training model: '{model_name}' with inputs '{even}' and '{odd}'")
+    if len(inputs) > 2:
+        log.info(f"denoising: [{inputs[0]} [...] {inputs[-1]}]")
+    else:
+        log.info(f"denoising: {inputs}")
+    log.info(f"output: {outdir}")
 
     if not dry_run:
         set_num_threads(0)
         std = io.StringIO()
         if train:
             task = progress.add_task(description="Training...")
             model, _ = _run_and_update_progress(
```

### Comparing `waretomo-0.1.3/src/waretomo/main.py` & `waretomo-0.1.4/src/waretomo/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import waretomo
 
 
 class ProcessingStep(str, Enum):
     """Enum for step selection."""
 
-    fix = auto()
     align = auto()
     tilt_mdocs = auto()
     reconstruct = auto()
     stack_halves = auto()
     reconstruct_halves = auto()
     denoise = auto()
 
@@ -43,15 +42,15 @@
 )
 @click.option(
     "-d",
     "--dry-run",
     is_flag=True,
     help="only print some info, without running the commands.",
 )
-@click.option("-v", "--verbose", is_flag=True, help="echo all individual commands")
+@click.option("-v", "--verbose", count=True, help="echo all individual commands")
 @click.option(
     "-j",
     "--just",
     type=str,
     multiple=True,
     help="reconstruct just this tomogram (can be passed multiple times)",
 )
@@ -126,24 +125,23 @@
     "previously generated model. If instead --train was given, a new model will"
     "be generated with the given name. New models are saved inside "
     "'OUTPUT_DIR/trained_models/.",
 )
 @click.option(
     "--start-from",
     type=click.Choice(ProcessingStep.__members__),
-    default="fix",
+    default="align",
     help="use outputs from a previous run, starting processing at this step",
 )
 @click.option(
     "--stop-at",
     type=click.Choice(ProcessingStep.__members__),
     default="denoise",
     help="terminate processing after this step",
 )
-@click.option("--ccderaser", type=str, default="ccderaser", help="ccderaser executable")
 @click.option("--aretomo", type=str, default="AreTomo", help="aretomo executable")
 @click.option(
     "--gpus",
     type=str,
     help="Comma separated list of gpus to use for aretomo. Default to all.",
 )
 @click.option(
@@ -167,38 +165,47 @@
     overwrite,
     train,
     topaz_tile_size,
     topaz_patch_size,
     topaz_model,
     start_from,
     stop_at,
-    ccderaser,
     aretomo,
     gpus,
     tiltcorr,
 ):
     """
     Run aretomo in batch on data preprocessed in warp.
 
     Needs to be ran after imod stacks were generated.
-    Requires ccderaser and AreTomo>=1.3.0.
+    Requires AreTomo>=1.3.0.
 
     Assumes the default Warp directory structure with generated imod stacks.
     """
+    import logging
     import sys
     from datetime import datetime
     from inspect import cleandoc
     from pathlib import Path
 
     from rich import print
+    from rich.logging import RichHandler
     from rich.panel import Panel
     from rich.progress import Progress
 
     from ._parse import parse_data
 
+    logging.basicConfig(
+        level=40 - max(verbose * 10, 0),
+        format="%(message)s",
+        datefmt="[%X]",
+        handlers=[RichHandler()],
+    )
+    log = logging.getLogger("waretomo")
+
     if gpus is not None:
         gpus = [int(gpu) for gpu in gpus.split(",")]
 
     warp_dir = Path(warp_dir)
     if mdoc_dir is None:
         mdoc_dir = warp_dir
     mdoc_dir = Path(mdoc_dir)
@@ -251,15 +258,14 @@
             "gpus": gpus,
             "tilt_corr": tiltcorr,
         }
 
         meta_kwargs = {
             "overwrite": overwrite,
             "dry_run": dry_run,
-            "verbose": verbose,
         }
 
         topaz_kwargs = {
             "train": train,
             "model_name": topaz_model,
             "gpus": gpus,
             "tile_size": topaz_tile_size,
@@ -308,84 +314,77 @@
             [bold]Run options[/bold]: {opts_log}
             [bold]AreTomo options[/bold]: {aretomo_opts_log}
             [bold]Topaz options[/bold]: {topaz_log}
             """
         )
         print(Panel(summary))
 
+        ts = tilt_series[0]
+        ts_name = ts["name"]
+        ts_info = {k: v for k, v in ts.items() if k not in ("even", "odd")}
+        log.info(f'Metadata from tiltseries "{ts_name}": {ts_info}')
+
         if not dry_run:
             with open(output_dir / "waretomo.log", "a") as f:
                 print("=" * 80, file=f)
                 print(datetime.now().strftime("%d/%m/%Y %H:%M:%S"), file=f)
                 print(f'Command: {" ".join(sys.argv)}', file=f)
                 print(summary, "\n", file=f)
 
-        if steps["fix"]:
-            from ._fix import fix_batch
-
-            if verbose:
-                print("\n[green]Fixing with ccderaser...")
-            fix_batch(progress, tilt_series, cmd=ccderaser, **meta_kwargs)
-
         if steps["align"]:
             from ._aretomo import aretomo_batch
 
-            if verbose:
-                print("\n[green]Aligning with AreTomo...")
+            log.info("Aligning with AreTomo...")
             aretomo_batch(
                 progress,
                 tilt_series,
                 label="Aligning",
                 **aretomo_kwargs,
                 **meta_kwargs,
             )
 
         if steps["tilt_mdocs"]:
             if not tiltcorr:
-                print("No need to tilt mdocs!")
+                log.info("No need to tilt mdocs!")
             else:
                 from ._fix_mdoc import tilt_mdocs_batch
 
-                if verbose:
-                    print("\n[green]Tilting mdocs...")
+                log.info("Tilting mdocs...")
                 (mdoc_dir / "mdoc_tilted").mkdir(parents=True, exist_ok=True)
                 tilt_mdocs_batch(
                     progress,
                     tilt_series,
                     **meta_kwargs,
                 )
 
         if steps["reconstruct"]:
             from ._aretomo import aretomo_batch
 
-            if verbose:
-                print("\n[green]Reconstructing with AreTomo...")
+            log.info("Reconstructing with AreTomo...")
             aretomo_batch(
                 progress,
                 tilt_series,
                 reconstruct=True,
                 label="Reconstructing",
                 **aretomo_kwargs,
                 **meta_kwargs,
             )
 
         if steps["stack_halves"]:
             from ._stack import prepare_half_stacks
 
             for half in ("even", "odd"):
-                if verbose:
-                    print(f"\n[green]Preparing {half} stacks for denoising...")
+                log.info(f"Preparing {half} stacks for denoising...")
                 prepare_half_stacks(progress, tilt_series, half=half, **meta_kwargs)
 
         if steps["reconstruct_halves"]:
             from ._aretomo import aretomo_batch
 
             for half in ("even", "odd"):
-                if verbose:
-                    print(f"\n[green]Reconstructing {half} tomograms for deonoising...")
+                log.info(f"Reconstructing {half} tomograms for deonoising...")
                 half_dir = output_dir / half
                 half_dir.mkdir(parents=True, exist_ok=True)
                 aretomo_batch(
                     progress,
                     tilt_series,
                     suffix=f"_{half}",
                     reconstruct=True,
@@ -398,16 +397,15 @@
                     f.unlink(missing_ok=True)
                 for f in half_dir.glob("*.aretomolog"):
                     f.unlink(missing_ok=True)
 
         if steps["denoise"]:
             from ._topaz import topaz_batch
 
-            if verbose:
-                print("\n[green]Denoising tomograms...")
+            log.info("Denoising tomograms...")
             outdir_denoised = output_dir / "denoised"
             outdir_denoised.mkdir(parents=True, exist_ok=True)
             topaz_batch(
                 progress,
                 tilt_series,
                 outdir=outdir_denoised,
                 even=str(output_dir / "even"),
```

### Comparing `waretomo-0.1.3/.gitignore` & `waretomo-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.3/LICENSE` & `waretomo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.3/README.md` & `waretomo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.3/pyproject.toml` & `waretomo-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waretomo-0.1.3/PKG-INFO` & `waretomo-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: waretomo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Overengineered batch processing script for tomography data with Warp and aretomo.
 Project-URL: homepage, https://github.com/brisvag/waretomo
 Project-URL: repository, https://github.com/brisvag/waretomo
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GPLv3
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

