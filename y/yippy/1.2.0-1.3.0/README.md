# Comparing `tmp/yippy-1.2.0.tar.gz` & `tmp/yippy-1.3.0.tar.gz`

## Comparing `yippy-1.2.0.tar` & `yippy-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,36 @@
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 yippy-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 yippy-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 yippy-1.2.0/README.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 yippy-1.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 yippy-1.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yippy-1.2.0/.github/workflows/release-please.yml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/_version.py
--rwxr-xr-x   0        0        0    10612 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/coronagraph.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/logger.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_base.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/stellar_intens.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/util.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/__init__.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/one_d.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/quarter_symmetric.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 yippy-1.2.0/src/yippy/offax_psf/two_d.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 yippy-1.2.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yippy-1.2.0/LICENSE
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 yippy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 yippy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 yippy-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 yippy-1.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 yippy-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 yippy-1.3.0/README.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 yippy-1.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 yippy-1.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yippy-1.3.0/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/Makefile
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/conf.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/examples.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/make.bat
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/_static/favicon.ico
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/_static/logo.png
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/develop/_changelog.md
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/modules/off_axis_psf.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/modules/sky_transmission_maps.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yippy-1.3.0/docs/modules/stellar_intensity_maps.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/_version.py
+-rwxr-xr-x   0        0        0     8291 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/coronagraph.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/header.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/logger.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/offax_base.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/sky_trans.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/stellar_intens.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/util.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/offax_psf/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/offax_psf/one_d.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/offax_psf/quarter_symmetric.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 yippy-1.3.0/src/yippy/offax_psf/two_d.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 yippy-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yippy-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 yippy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 yippy-1.3.0/PKG-INFO
```

### Comparing `yippy-1.2.0/.pre-commit-config.yaml` & `yippy-1.3.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.6.0"
     hooks:
       - id: trailing-whitespace
       - id: name-tests-test
       - id: end-of-file-fixer
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.7
+    rev: v0.4.1
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/compilerla/conventional-pre-commit
```

### Comparing `yippy-1.2.0/CHANGELOG.md` & `yippy-1.3.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [1.3.0](https://github.com/CoreySpohn/yippy/compare/v1.2.0...v1.3.0) (2024-04-23)
+
+
+### Features
+
+* **main:** Add a temporary sky_trans file ([ad89135](https://github.com/CoreySpohn/yippy/commit/ad89135fc2687b60af018e7a9fde503513ee1854))
+* **main:** Added dataclass that handles the header ([3120eda](https://github.com/CoreySpohn/yippy/commit/3120eda53bb75dc96ead74ae3e37c5cd206785ac))
+
 ## [1.2.0](https://github.com/CoreySpohn/yippy/compare/v1.1.1...v1.2.0) (2024-04-17)
 
 
 ### Features
 
 * **main:** Added stellar intensity map ([481d333](https://github.com/CoreySpohn/yippy/commit/481d333b89280a906bf8be3642f0eb7bf1fa946e))
 * **main:** Adding more support for 2d and quarter symmetric coronagraphs ([3e98780](https://github.com/CoreySpohn/yippy/commit/3e9878034b37535780ee0004f69ad4409b961445))
```

### Comparing `yippy-1.2.0/.github/workflows/publish-to-pypi.yml` & `yippy-1.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/.github/workflows/release-please.yml` & `yippy-1.3.0/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/src/yippy/coronagraph.py` & `yippy-1.3.0/src/yippy/coronagraph.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from pathlib import Path
 
 import astropy.io.fits as pyfits
 import astropy.units as u
 import numpy as np
 import xarray as xr
-from lod_unit import lod
 from scipy.ndimage import rotate
 from tqdm import tqdm
 
-from .logger import setup_logger
+from .header import HeaderData
+from .logger import logger
 from .offax_base import OffAx
+from .sky_trans import SkyTrans
 from .stellar_intens import StellarIntens
 
 
 class Coronagraph:
     """Primary object for simulating a coronagraph.
 
     The Coronagraph object manages the coronagraph response for both on-axis
@@ -28,15 +29,15 @@
     def __init__(
         self,
         yip_path: Path,
         stellar_intens_file: str = "stellar_intens.fits",
         stellar_diam_file: str = "stellar_intens_diam_list.fits",
         offax_data_file: str = "offax_psf.fits",
         offax_offsets_file: str = "offax_psf_offset_list.fits",
-        logging_level: str = "INFO",
+        sky_trans_file: str = "sky_trans.fits",
     ):
         """Initialize the Coronagraph object.
 
         Loads the coronagraph data from the given yield input package and creates
         the interpolation functions for the stellar intensity and off-axis PSF.
 
         Args:
@@ -51,106 +52,49 @@
                 Name of the stellar intensity diameter list file. Default is
                 stellar_intens_diam_list.fits
             offax_data_file (str):
                 Name of the off-axis PSF file. Default is offax_psf.fits
             offax_offsets_file (str):
                 Name of the off-axis PSF offset list file. Default is
                 offax_psf_offset_list.fits
-            logging_level (str):
-                Logging level for the logger (e.g. INFO, DEBUG, WARNING, ERROR,
-                CRITICAL), use to suppress logging if used as part of a larger
-                workflow. Default is INFO.
+            sky_trans_file (str):
+                Name of the sky transmission data file. Default is sky_trans.fits.
         """
-        self.logger = setup_logger(logging_level)
         ###################
         # Read input data #
         ###################
-        self.logger.info("Creating coronagraph")
+        logger.info("Creating coronagraph")
 
         yip_path = Path(yip_path)
         self.name = yip_path.stem
         # Get header and calculate the lambda/D value
-        stellar_intens_header = pyfits.getheader(
-            Path(yip_path, "stellar_intens.fits"), 0
-        )
+        stellar_intens_header = pyfits.getheader(Path(yip_path, stellar_intens_file), 0)
 
         # Get pixel scale with units
-        self.pixel_scale = stellar_intens_header["PIXSCALE"] * lod / u.pixel
+        self.header = HeaderData.from_fits_header(stellar_intens_header)
+        self.pixel_scale = self.header.pixscale
 
         # Stellar intensity of the star being observed as function of stellar
         # angular diameter (unitless)
         self.stellar_intens = StellarIntens(
-            yip_path, self.logger, stellar_intens_file, stellar_diam_file
+            yip_path, stellar_intens_file, stellar_diam_file
         )
 
         # Offaxis PSF of the planet as function of separation from the star
         self.offax = OffAx(
-            yip_path, self.logger, offax_data_file, offax_offsets_file, self.pixel_scale
+            yip_path, offax_data_file, offax_offsets_file, self.pixel_scale
         )
 
-        # ############
-        # # Clean up #
-        # ############
-        # # Center coronagraph model so that image size is odd
-        # # and central pixel is center
-        # # TODO: Automate this process
-        # verified_coronagraph_models = [
-        #     "LUVOIR-A_APLC_10bw_smallFPM_2021-05-05_Dyn10pm-nostaticabb",
-        #     "LUVOIR-A_APLC_18bw_medFPM_2021-05-07_Dyn10pm-nostaticabb",
-        #     "LUVOIR-B-VC6_timeseries",
-        #     "LUVOIR-B_VC6_timeseries",
-        # ]
-        # if yip_path.parts[-1] in verified_coronagraph_models:
-        #     self.stellar_intens = self.stellar_intens[:, 1:, 1:]
-        #     self.offax_psf = self.offax_psf[:, :-1, 1:]
-        # else:
-        #     raise UserWarning(
-        #         "Please validate centering for this unknown coronagraph model"
-        #     )
-        #
-        # # Simulation parameters
-        # self.yip_path = yip_path
-        #
-        # #########################################################################
-        # # Interpolate coronagraph model (in log space to avoid negative values) #
-        # #########################################################################
-        # # Fill value for interpolation
-        # fill = np.log(1e-100)
-        #
-        # # interpolate stellar data
-        # self.ln_stellar_intens_interp = interp1d(
-        #     self.stellar_intens_diam_list,
-        #     np.log(self.stellar_intens),
-        #     kind="cubic",
-        #     axis=0,
-        #     bounds_error=False,
-        #     fill_value=fill,
-        # )
-        # self.stellar_intens_interp = lambda stellar_diam: np.exp(
-        #     self.ln_stellar_intens_interp(stellar_diam)
-        # )
-        # ##################################################
-        # # Get remaining parameters and throughput values #
-        # ##################################################
-        #
-        # # Gets the number of pixels in the image
-        # self.img_pixels = self.stellar_intens.shape[1] * u.pixel
-        # self.npixels = self.img_pixels.value.astype(int)
-        #
-        # # Photometric parameters.
-        # head = pyfits.getheader(Path(yip_path, "stellar_intens.fits"), 0)
-        #
-        # # fractional obscuration
-        # self.frac_obscured = head["OBSCURED"]
-        #
-        # # fractional bandpass
-        # self.frac_bandwidth = (head["MAXLAM"] - head["MINLAM"]) / head["LAMBDA"]
-        #
-        # # PSF datacube info
-        # self.has_psf_datacube = False
+        # Get the sky_trans mask
+        self.sky_trans = SkyTrans(yip_path, sky_trans_file)
+
+        # PSF datacube here is a 4D array of PSFs at each pixel (x psf offset,
+        # y psf offset, x, y). Given the computational cost of generating this
+        # datacube, it is only generated when needed.
+        self.has_psf_datacube = False
 
     def get_disk_psfs(self):
         """Load the disk image from a file or generate it if it doesn't exist."""
         # Load data cube of spatially dependent PSFs.
         disk_dir = Path(".cache/disks/")
         if not disk_dir.exists():
             disk_dir.mkdir(parents=True, exist_ok=True)
@@ -163,20 +107,18 @@
             "x psf offset (pix)": np.arange(self.npixels),
             "y psf offset (pix)": np.arange(self.npixels),
             "x (pix)": np.arange(self.npixels),
             "y (pix)": np.arange(self.npixels),
         }
         dims = ["x psf offset (pix)", "y psf offset (pix)", "x (pix)", "y (pix)"]
         if path.exists():
-            self.logger.info(
-                "Loading data cube of spatially dependent PSFs, please hold..."
-            )
+            logger.info("Loading data cube of spatially dependent PSFs, please hold...")
             psfs_xr = xr.open_dataarray(path)
         else:
-            self.logger.info(
+            logger.info(
                 "Calculating data cube of spatially dependent PSFs, please hold..."
             )
             # Compute pixel grid.
             # lambda/D
             pixel_lod = (
                 (np.arange(self.npixels) - ((self.npixels - 1) // 2))
                 * u.pixel
```

### Comparing `yippy-1.2.0/src/yippy/offax_base.py` & `yippy-1.3.0/src/yippy/offax_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Base class for all offax_psfs.fits files."""
 
 from pathlib import Path
-from typing import TYPE_CHECKING
 
 import astropy.io.fits as pyfits
 import astropy.units as u
 import numpy as np
 from astropy.units import Quantity
 from lod_unit import lod
 from numpy.typing import NDArray
 
 from yippy.offax_psf import OneD, QuarterSymmetric, TwoD
 from yippy.util import convert_to_lod
 
-if TYPE_CHECKING:
-    from logging import Logger
+from .logger import logger
 
 
 class OffAx:
     """Base class for handling off-axis PSFs.
 
     This class loads and processes PSF data from the yield input package (YIP).
     It currently supports oneD and quater symmetric PSF YIPs. The primary use
@@ -48,15 +46,14 @@
         pixel_scale (Quantity):
             Pixel scale of the PSF data in lambda/D.
     """
 
     def __init__(
         self,
         yip_dir: Path,
-        logger: "Logger",
         offax_data_file: str,
         offax_offsets_file: str,
         pixel_scale: Quantity,
     ) -> None:
         """Initializes the OffAx class by loading PSF and offset data from YIP.
 
         Determines the type of coronagraph based on the symmetry and structure of the
```

### Comparing `yippy-1.2.0/src/yippy/stellar_intens.py` & `yippy-1.3.0/src/yippy/stellar_intens.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """Module for handling stellar intensity data from stellar_intens files."""
 
 from pathlib import Path
-from typing import TYPE_CHECKING
 
 import astropy.io.fits as pyfits
 import numpy as np
 from astropy.units import Quantity
 from lod_unit import lod
 from scipy.interpolate import CubicSpline
 
 from .util import convert_to_lod
 
-if TYPE_CHECKING:
-    from logging import Logger
-
 
 class StellarIntens:
     """Class to handle and interpolate stellar intensity data.
 
     This class loads stellar intensity data and corresponding stellar diameters,
     providing an interpolation interface to get the stellar intensity map for a given
     stellar diameter.
@@ -26,41 +22,36 @@
         ln_interp (CubicSpline):
             A spline interpolator that operates on the natural logarithm of the
             stellar intensities to ensure that interpolated values are non-negative.
 
     Args:
         yip_dir (Path):
             Path to the directory containing the yield input package (YIP).
-        logger (Logger):
-            Logger for logging information and debugging.
         stellar_intens_file (str):
             Filename of the FITS file containing the stellar intensity data.
         stellar_diam_file (str):
             Filename of the FITS file containing the stellar diameters.
     """
 
     def __init__(
         self,
         yip_dir: Path,
-        logger: "Logger",
         stellar_intens_file: str,
         stellar_diam_file: str,
     ) -> None:
         """Initializes StellarIntens class by loading data and creating the interpolant.
 
         Stellar intensity data and stellar diameters are loaded from FITS files,
         and a natural logarithm-based cubic spline interpolator is set up to
         facilitate interpolation.
 
         Args:
             yip_dir (Path):
                 The directory where the stellar intensity and diameter FITS
                 files are located.
-            logger (Logger):
-                Logger for logging setup and processing steps.
             stellar_intens_file (str):
                 The filename of the FITS file containing unitless arrays of stellar
                 intensities.
             stellar_diam_file (str):
                 The filename of the FITS file containing arrays of stellar diameters in
                 lambda/D units.
         """
```

### Comparing `yippy-1.2.0/src/yippy/util.py` & `yippy-1.3.0/src/yippy/util.py`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/src/yippy/offax_psf/one_d.py` & `yippy-1.3.0/src/yippy/offax_psf/one_d.py`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/src/yippy/offax_psf/quarter_symmetric.py` & `yippy-1.3.0/src/yippy/offax_psf/quarter_symmetric.py`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/src/yippy/offax_psf/two_d.py` & `yippy-1.3.0/src/yippy/offax_psf/two_d.py`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/.gitignore` & `yippy-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/LICENSE` & `yippy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yippy-1.2.0/pyproject.toml` & `yippy-1.3.0/pyproject.toml`

 * *Files identical despite different names*

