# Comparing `tmp/tidal-wave-2024.4.2.tar.gz` & `tmp/tidal_wave-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal-wave-2024.4.2.tar", last modified: Tue Apr  9 01:03:19 2024, max compression
+gzip compressed data, was "tidal_wave-2024.4.3.tar", last modified: Wed Apr 24 04:32:19 2024, max compression
```

## Comparing `tidal-wave-2024.4.2.tar` & `tidal_wave-2024.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25953 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:03:19.914816 tidal-wave-2024.4.2/tidal_wave/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/album.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/mix.py
--rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/requesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/tidal_wave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40189 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26032 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:32:19.071366 tidal_wave-2024.4.3/tidal_wave/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26637 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18615 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/requesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37425 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/tidal_wave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40189 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/top_level.txt
```

### Comparing `tidal-wave-2024.4.2/LICENSE` & `tidal_wave-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/PKG-INFO` & `tidal_wave-2024.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -225,15 +225,15 @@
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: m3u8==4.1.0
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: requests[socks]==2.31.0
-Requires-Dist: typer==0.12.1
+Requires-Dist: typer==0.12.3
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
 [![GNU/Linux amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml)
@@ -250,36 +250,42 @@
 
 This software uses libraries from the [FFmpeg](http://ffmpeg.org) project under the [LGPLv2.1](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). FFmpeg is a trademark of [Fabrice Bellard](http://www.bellard.org/), originator of the FFmpeg project. 
 
 ## Features
 * Retrieve [FLAC](https://xiph.org/flac/), [Dolby Atmos](https://www.dolby.com/technologies/dolby-atmos/), [Sony 360 Reality Audio](https://electronics.sony.com/360-reality-audio), or [AAC](https://en.wikipedia.org/wiki/Advanced_Audio_Coding) tracks; [AVC/H.264](https://en.wikipedia.org/wiki/Advanced_Video_Coding) (up to 1920x1080) + [AAC](https://en.wikipedia.org/wiki/Advanced_Audio_Coding) videos
 * Either a single track or an entire album can be retrieved
 * Album covers are retrieved by default, and embedded into all tracks
+  - Highest-resolution, "original" album covers, which can be up to 6000x6000 pixels resolution, are retrieved if available
 * Support for albums with multiple discs
 * If available, lyrics are added as metadata to tracks
 * If available, album reviews are retrieved as JSON
 * If available, album credits are retrieved as JSON
 * If available, artist bios are retrieved as JSON
 * If available, artist images are retrieved as JPEG
 * Playlist retrieval support (video or audio or both)
 * Playlist .m3u8 file automatically created
 * Mix retrieval support (video or audio)
 * Artist's entire works retrieval support (video and audio; albums or albums and EPs and singles)
 * Because of the use of the `requests` package, system proxies are respected (HTTP, HTTPs, Socks); or can be specified by typical environment variable
 * Also because of the use of `requests`, very simple [`Cache-Control`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) request caching occurs via `CacheControl`
+* If desired, all JSON responses from the TIDAL API can be saved for inspection or posterity or debugging
 
 ## Getting Started
-A [HiFi Plus](https://tidal.com/pricing) account is **required** in order to retrieve HiRes FLAC, Dolby Atmos, and Sony 360 Reality Audio tracks. Simply a [HiFi](https://tidal.com/pricing) plan is sufficient to retrieve in 16-bit, 44.1 kHz (i.e., lossless) or lower quality as well as videos. More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
+A current, valid TIDAL subscription is required in order to run `tidal-wave`. Previously, TIDAL segmented the available audio qualities into HiFi and HiFi Plus plans: now, 
+> All current TIDAL plans feature Max sound quality formats such as full lossless, HiRes FLAC, and Dolby Atmos (up to 24-bit, 192 kHz).
+
+More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
 
 ### Requirements
  - As resources will be fetched from the World Wide Web, an Internet connection is required
- - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binary for Ubuntu GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_aarch64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_amd64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe) build FFmpeg from source, so separate installation is unnecessary.
+ - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binaries](https://github.com/ebb-earl-co/tidal-wave/releases/latest) build FFmpeg from source, so separate installation is unnecessary.
    - Static builds of FFmpeg are available from [John Van Sickle](https://www.johnvansickle.com/ffmpeg/) for GNU/Linux, or most package managers feature `ffmpeg`.
    - For macOS, the [FFmpeg download page](http://ffmpeg.org/download.html#build-mac) links to [this download source](https://evermeet.cx/ffmpeg/); or there is always [Homebrew](https://formulae.brew.sh/formula/ffmpeg)
    - For Windows, the [FFmpeg download page](http://ffmpeg.org/download.html#build-windows) lists 2 resources; or [`chocolatey`](https://community.chocolatey.org/packages/ffmpeg) is an option
+   - If a minimal FFmpeg, compiled from source, is desired, take a look at this project's [BUILDME.md](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/BUILDME.md) file for decent instructions
  - This is a Python package, so **to use it in the default manner** you will need [Python 3](https://www.python.org/downloads/), version 3.8 or newer, on your system.
    - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); and [PyInstaller](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, x86\_64 macOS, and x86\_64 Windows are provided for download and use that *do not require Python to be installed*
  - Only a handful of Python libraries are dependencies:
    - [`backoff`](https://pypi.org/project/backoff/)
    - [`cachecontrol`](https://pypi.org/project/CacheControl/)
    - [`dataclass-wizard`](https://pypi.org/project/dataclass-wizard/)
    - [`ffmpeg-python`](https://pypi.org/project/ffmpeg-python/)
@@ -298,36 +304,29 @@
 $ python3 -m pip install tidal-wave
 ```
 ```powershell
 # Windows
 PS > python.exe -m pip install tidal-wave
 ```
 
-Optionally, to get the full `typer` experience when using this utility, add `[all]` to the end of the `pip install command`:
-```bash
-$ python3 -m pip install tidal-wave[all]
-```
-```powershell
-PS > python.exe -m pip install tidal-wave[all]
-```
 ### `pip` Install from the Repository
 Alternatively, you can clone this repository; `cd` into it; and install from there:
 ```bash
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
 These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64
-$ chmod +x ./tidal-wave_ubuntu_amd64
-$ ./tidal-wave_ubuntu_amd64 --help
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
+$ chmod +x ./tidal-wave_ubuntu_22.04_amd64
+$ ./tidal-wave_ubuntu_22.04_amd64 --help
 ```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
@@ -354,15 +353,15 @@
 │ --help                                                                Show this message and exit.                                                                                                                                 │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Usage
 Invocation of this tool will store credentials in a particular directory in the user's "home" directory: for Unix-like systems, this will be `/home/${USER}/.config/tidal-wave`: for Windows, it varies: in either OS situation, the exact directory is determined by the `user_config_path()` function of the `platformdirs` package.
 
-Similarly, by default, all media retrieved is placed in subdirectories of the user's default music directory: for Unix-like systems, this probably is `/home/${USER}/Music`; for Windows it is probably `C:\Users\<USER>\Music`. This directory is determined by `platformdirs.user_music_path()`. 
+Similarly, by default, all media retrieved is placed in subdirectories of the user's default music directory: for Unix-like systems, this probably is `/home/${USER}/Music`; for Windows it is probably `C:\Users\<USER>\Music`. This directory is determined by [`platformdirs.user_music_path()`](https://github.com/platformdirs/platformdirs?tab=readme-ov-file#platformdirs-to-the-rescue). 
  - If a different path is passed to the second CLI argument, `output_directory`, then all media is written to subdirectories of that directory.
 
 ### Which Audio Formats Are Available to Which Clients
 Source: [TIDAL](https://tidal.com/supported-devices)
 |                | Low                | High               | Lossless           |      MQA           | HiRes FLAC         | Dolby Atmos        | Sony 360 Reality Audio | Video (H.264 + AAC) |
 | :---           | :---:              | :---:              |   :---:            |     :---:          |   :---:            |    :---:           |        :---:           |     :---:           |
 | Android        | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |     :x:            |   :heavy_check_mark:   | :heavy_check_mark: |
@@ -478,19 +477,20 @@
 $ docker run \
     --name tidal-wave \
     -dit \  # is short for: --detach --interactive --tty
     --volume ./Music:/home/debian/Music \
     --volume ./config/tidal-wave:/home/debian/.config/tidal-wave \
     --entrypoint "/bin/bash" \
     ghcr.io/ebb-earl-co/tidal-wave:latest
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/album/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/mix/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/playlist/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/track/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/album/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/mix/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/playlist/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/track/...
 ```
+Note: the first `tidal-wave` is whatever `--name` you give the container, so that can be whatever your heart desires, but the second `tidal-wave` is invoking the Python program *inside* the container and needs to exactly `tidal-wave`.
 ## Development
 The easiest way to start working on development is to fork this project on GitHub, or clone the repository to your local machine and do the pull requesting on GitHub later. In any case, there will need to be some getting from GitHub first, so, roughly, the process is:
   1. Get Python 3.8+ on your system
   2. Use a virtualenv or some other Python environment system (poetry, pipenv, etc.)
   3. Clone the repository: `$ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave/git`
 
     * Obviously replace the URL with your forked version if you've followed that strategy
```

### Comparing `tidal-wave-2024.4.2/README.md` & `tidal_wave-2024.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,36 +17,42 @@
 
 This software uses libraries from the [FFmpeg](http://ffmpeg.org) project under the [LGPLv2.1](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). FFmpeg is a trademark of [Fabrice Bellard](http://www.bellard.org/), originator of the FFmpeg project. 
 
 ## Features
 * Retrieve [FLAC](https://xiph.org/flac/), [Dolby Atmos](https://www.dolby.com/technologies/dolby-atmos/), [Sony 360 Reality Audio](https://electronics.sony.com/360-reality-audio), or [AAC](https://en.wikipedia.org/wiki/Advanced_Audio_Coding) tracks; [AVC/H.264](https://en.wikipedia.org/wiki/Advanced_Video_Coding) (up to 1920x1080) + [AAC](https://en.wikipedia.org/wiki/Advanced_Audio_Coding) videos
 * Either a single track or an entire album can be retrieved
 * Album covers are retrieved by default, and embedded into all tracks
+  - Highest-resolution, "original" album covers, which can be up to 6000x6000 pixels resolution, are retrieved if available
 * Support for albums with multiple discs
 * If available, lyrics are added as metadata to tracks
 * If available, album reviews are retrieved as JSON
 * If available, album credits are retrieved as JSON
 * If available, artist bios are retrieved as JSON
 * If available, artist images are retrieved as JPEG
 * Playlist retrieval support (video or audio or both)
 * Playlist .m3u8 file automatically created
 * Mix retrieval support (video or audio)
 * Artist's entire works retrieval support (video and audio; albums or albums and EPs and singles)
 * Because of the use of the `requests` package, system proxies are respected (HTTP, HTTPs, Socks); or can be specified by typical environment variable
 * Also because of the use of `requests`, very simple [`Cache-Control`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) request caching occurs via `CacheControl`
+* If desired, all JSON responses from the TIDAL API can be saved for inspection or posterity or debugging
 
 ## Getting Started
-A [HiFi Plus](https://tidal.com/pricing) account is **required** in order to retrieve HiRes FLAC, Dolby Atmos, and Sony 360 Reality Audio tracks. Simply a [HiFi](https://tidal.com/pricing) plan is sufficient to retrieve in 16-bit, 44.1 kHz (i.e., lossless) or lower quality as well as videos. More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
+A current, valid TIDAL subscription is required in order to run `tidal-wave`. Previously, TIDAL segmented the available audio qualities into HiFi and HiFi Plus plans: now, 
+> All current TIDAL plans feature Max sound quality formats such as full lossless, HiRes FLAC, and Dolby Atmos (up to 24-bit, 192 kHz).
+
+More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
 
 ### Requirements
  - As resources will be fetched from the World Wide Web, an Internet connection is required
- - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binary for Ubuntu GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_aarch64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_amd64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe) build FFmpeg from source, so separate installation is unnecessary.
+ - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binaries](https://github.com/ebb-earl-co/tidal-wave/releases/latest) build FFmpeg from source, so separate installation is unnecessary.
    - Static builds of FFmpeg are available from [John Van Sickle](https://www.johnvansickle.com/ffmpeg/) for GNU/Linux, or most package managers feature `ffmpeg`.
    - For macOS, the [FFmpeg download page](http://ffmpeg.org/download.html#build-mac) links to [this download source](https://evermeet.cx/ffmpeg/); or there is always [Homebrew](https://formulae.brew.sh/formula/ffmpeg)
    - For Windows, the [FFmpeg download page](http://ffmpeg.org/download.html#build-windows) lists 2 resources; or [`chocolatey`](https://community.chocolatey.org/packages/ffmpeg) is an option
+   - If a minimal FFmpeg, compiled from source, is desired, take a look at this project's [BUILDME.md](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/BUILDME.md) file for decent instructions
  - This is a Python package, so **to use it in the default manner** you will need [Python 3](https://www.python.org/downloads/), version 3.8 or newer, on your system.
    - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); and [PyInstaller](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, x86\_64 macOS, and x86\_64 Windows are provided for download and use that *do not require Python to be installed*
  - Only a handful of Python libraries are dependencies:
    - [`backoff`](https://pypi.org/project/backoff/)
    - [`cachecontrol`](https://pypi.org/project/CacheControl/)
    - [`dataclass-wizard`](https://pypi.org/project/dataclass-wizard/)
    - [`ffmpeg-python`](https://pypi.org/project/ffmpeg-python/)
@@ -65,36 +71,29 @@
 $ python3 -m pip install tidal-wave
 ```
 ```powershell
 # Windows
 PS > python.exe -m pip install tidal-wave
 ```
 
-Optionally, to get the full `typer` experience when using this utility, add `[all]` to the end of the `pip install command`:
-```bash
-$ python3 -m pip install tidal-wave[all]
-```
-```powershell
-PS > python.exe -m pip install tidal-wave[all]
-```
 ### `pip` Install from the Repository
 Alternatively, you can clone this repository; `cd` into it; and install from there:
 ```bash
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
 These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64
-$ chmod +x ./tidal-wave_ubuntu_amd64
-$ ./tidal-wave_ubuntu_amd64 --help
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
+$ chmod +x ./tidal-wave_ubuntu_22.04_amd64
+$ ./tidal-wave_ubuntu_22.04_amd64 --help
 ```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
@@ -121,15 +120,15 @@
 │ --help                                                                Show this message and exit.                                                                                                                                 │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Usage
 Invocation of this tool will store credentials in a particular directory in the user's "home" directory: for Unix-like systems, this will be `/home/${USER}/.config/tidal-wave`: for Windows, it varies: in either OS situation, the exact directory is determined by the `user_config_path()` function of the `platformdirs` package.
 
-Similarly, by default, all media retrieved is placed in subdirectories of the user's default music directory: for Unix-like systems, this probably is `/home/${USER}/Music`; for Windows it is probably `C:\Users\<USER>\Music`. This directory is determined by `platformdirs.user_music_path()`. 
+Similarly, by default, all media retrieved is placed in subdirectories of the user's default music directory: for Unix-like systems, this probably is `/home/${USER}/Music`; for Windows it is probably `C:\Users\<USER>\Music`. This directory is determined by [`platformdirs.user_music_path()`](https://github.com/platformdirs/platformdirs?tab=readme-ov-file#platformdirs-to-the-rescue). 
  - If a different path is passed to the second CLI argument, `output_directory`, then all media is written to subdirectories of that directory.
 
 ### Which Audio Formats Are Available to Which Clients
 Source: [TIDAL](https://tidal.com/supported-devices)
 |                | Low                | High               | Lossless           |      MQA           | HiRes FLAC         | Dolby Atmos        | Sony 360 Reality Audio | Video (H.264 + AAC) |
 | :---           | :---:              | :---:              |   :---:            |     :---:          |   :---:            |    :---:           |        :---:           |     :---:           |
 | Android        | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |     :x:            |   :heavy_check_mark:   | :heavy_check_mark: |
@@ -245,19 +244,20 @@
 $ docker run \
     --name tidal-wave \
     -dit \  # is short for: --detach --interactive --tty
     --volume ./Music:/home/debian/Music \
     --volume ./config/tidal-wave:/home/debian/.config/tidal-wave \
     --entrypoint "/bin/bash" \
     ghcr.io/ebb-earl-co/tidal-wave:latest
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/album/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/mix/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/playlist/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/track/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/album/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/mix/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/playlist/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/track/...
 ```
+Note: the first `tidal-wave` is whatever `--name` you give the container, so that can be whatever your heart desires, but the second `tidal-wave` is invoking the Python program *inside* the container and needs to exactly `tidal-wave`.
 ## Development
 The easiest way to start working on development is to fork this project on GitHub, or clone the repository to your local machine and do the pull requesting on GitHub later. In any case, there will need to be some getting from GitHub first, so, roughly, the process is:
   1. Get Python 3.8+ on your system
   2. Use a virtualenv or some other Python environment system (poetry, pipenv, etc.)
   3. Clone the repository: `$ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave/git`
 
     * Obviously replace the URL with your forked version if you've followed that strategy
```

### Comparing `tidal-wave-2024.4.2/pyproject.toml` & `tidal_wave-2024.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 [bdist_wheel]
 universal = 0  # Make the generated wheels have "py3" tag
 [project]
 name = "tidal-wave"
-version = "2024.4.2"
+version = "2024.4.3"
 description = "A tool to wave at the TIDAL music service."
 authors = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
 maintainers = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
@@ -33,13 +33,13 @@
     "dataclass-wizard==0.22.3",
     "ffmpeg-python==0.2.0",
     "mutagen==1.47.0",
     "m3u8==4.1.0",
     "platformdirs==4.2.0",
     "pycryptodome==3.20.0",
     "requests[socks]==2.31.0",
-    "typer==0.12.1"
+    "typer==0.12.3"
 ]
 [project.scripts]
 tidal-wave = "tidal_wave.main:app"
 [project.urls]
 Homepage = "https://github.com/ebb-earl-co/tidal-wave"
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/album.py` & `tidal_wave-2024.4.3/tidal_wave/album.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from dataclasses import dataclass
 import json
 import logging
 from pathlib import Path
 import sys
 from typing import List, Optional, Tuple
 
-from requests import Session
+from requests import RequestException, Session
 
 from .media import AudioFormat
 from .models import (
     AlbumsCreditsResponseJSON,
     AlbumsEndpointResponseJSON,
     AlbumsItemsResponseJSON,
     AlbumsReviewResponseJSON,
     TracksEndpointResponseJSON,
 )
 from .requesting import (
     request_albums,
     request_albums_credits,
-    request_album_items,
+    request_albums_items,
     request_album_review,
 )
 from .track import Track
-from .utils import download_cover_image
+from .utils import download_cover_image, IMAGE_URL
 
 logger = logging.getLogger("__name__")
 
 
 @dataclass
 class Album:
     album_id: int
@@ -35,18 +35,40 @@
     def __post_init__(self):
         self.album_dir: Optional[Path] = None
         self.album_cover_saved: bool = False
 
     def set_tracks(self, session: Session):
         """This method populates self.tracks by requesting from
         TIDAL albums/items endpoint."""
-        album_items: AlbumsItemsResponseJSON = request_album_items(
+        album_items: Optional[AlbumsItemsResponseJSON] = request_albums_items(
             session=session, album_id=self.album_id, transparent=self.transparent
         )
-        _items = album_items.items if album_items is not None else ()
+        _items = album_items.items if album_items is not None else []
+        if self.metadata.number_of_tracks > len(_items):
+            items_to_retrieve: int = self.metadata.number_of_tracks - len(_items)
+            offset: int = 100
+            while items_to_retrieve > 0:
+                airj: Optional[AlbumsItemsResponseJSON] = request_albums_items(
+                    session=session,
+                    album_id=self.album_id,
+                    transparent=self.transparent,
+                    offset=offset,
+                )
+                if (airj is not None) and (airj.items is not None):
+                    _items += airj.items
+                    offset += 100
+                    items_to_retrieve -= 100
+                else:
+                    logger.warning(
+                        f"Could not retrieve more than {len(_items)} "
+                        f"tracks of album '{self.album_id}'. Continuing "
+                        "without the remaining "
+                        f"{self.metadata.number_of_tracks - len(_items)}"
+                    )
+
         self.tracks: Tuple[TracksEndpointResponseJSON] = tuple(
             _item.item for _item in _items
         )
 
     def set_metadata(self, session: Session):
         """This method sets self.metadata by requesting from
         TIDAL /albums endpoint"""
@@ -119,14 +141,37 @@
                 session=session,
                 cover_uuid=self.metadata.cover,
                 output_dir=self.album_dir,
             )
         else:
             self.album_cover_saved = True
 
+    def original_album_cover(self, session: Session):
+        """For most albums, TIDAL features the "original" album cover, in the highest
+        resolution possible. This JPEG can be too large to be embedded into FLAC tracks,
+        however it is ideal to have for music archiving etc. purposes. This method requests
+        the original cover and overwrites the smaller, 1280x1280 image used to embed into the
+        track file. The filename on the API side is origin.jpg. It is *probably* okay to
+        get this URL as a track.Track method, as HTTP requests are cached, so e.g. executing
+        this method for each track in an album won't result in many redundant GET requests
+        """
+        origin_jpg_url: str = (
+            IMAGE_URL % f"{self.metadata.cover.replace('-', '/')}/origin"
+        )
+        with session.get(url=origin_jpg_url, headers={"Accept": "image/jpeg"}) as resp:
+            try:
+                resp.raise_for_status()
+            except RequestException as re:
+                logger.warning(
+                    "Could not retrieve origin.jpg from TIDAL "
+                    f"due to error '{re.args[0]}'"
+                )
+            else:
+                (self.album_dir / "cover.jpg").write_bytes(resp.content)
+
     def get_tracks(
         self,
         session: Session,
         audio_format: AudioFormat,
         out_dir: Path,
         no_extra_files: bool,
     ) -> List[Optional[str]]:
@@ -140,14 +185,15 @@
             track_files_value: Optional[str] = track.get(
                 session=session,
                 audio_format=audio_format,
                 out_dir=out_dir,
                 metadata=t,
                 album=self.metadata,
                 no_extra_files=no_extra_files,
+                origin_jpg=False,
             )
             track_files[i] = {track.metadata.track_number: track_files_value}
         else:
             self.track_files = track_files
 
     def dumps(self):
         """This method returns a JSON-like string of self.track_files"""
@@ -190,17 +236,18 @@
         if self.metadata.cover != "":  # None was sent from the API
             self.save_cover_image(session, out_dir)
         else:
             logger.warning(
                 f"No cover image was returned from TIDAL API for album {self.album_id}"
             )
 
+        self.get_tracks(session, audio_format, out_dir, no_extra_files)
+
         if not no_extra_files:
             self.set_album_review(session)
             self.set_album_credits(session)
+            self.original_album_cover(session)
         else:
             try:
                 self.cover_path.unlink()
             except FileNotFoundError:
                 pass
-
-        self.get_tracks(session, audio_format, out_dir, no_extra_files)
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/artist.py` & `tidal_wave-2024.4.3/tidal_wave/artist.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/tidal_wave/dash.py` & `tidal_wave-2024.4.3/tidal_wave/dash.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/tidal_wave/hls.py` & `tidal_wave-2024.4.3/tidal_wave/hls.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/tidal_wave/login.py` & `tidal_wave-2024.4.3/tidal_wave/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         elif (TOKEN_DIR_PATH / "mac_os-tidal.token").exists():
             return (login_macos(), audio_format)
 
         options: set = {"android", "a", "macos", "m", "windows", "w"}
         _input: str = ""
         while _input not in options:
             _input = typer.prompt(
-                "For which of Android [a] or Windows [w] would you like to provide an API token?"
+                "For which of Android [a], macOS [m], or Windows [w] would you like to provide an API token?"
             ).lower()
         else:
             if _input in {"android", "a"}:
                 return (login_android(), audio_format)
             elif _input in {"macos", "m"}:
                 return (login_macos(), audio_format)
             elif _input in {"windows", "w"}:
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/main.py` & `tidal_wave-2024.4.3/tidal_wave/main.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/tidal_wave/media.py` & `tidal_wave-2024.4.3/tidal_wave/media.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/tidal_wave/mix.py` & `tidal_wave-2024.4.3/tidal_wave/mix.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 from pathlib import Path
 import shutil
 import sys
 from types import SimpleNamespace
 from typing import Dict, List, Optional, Set, Tuple, Union
+from uuid import uuid4
 
 from .media import AudioFormat
 from .models import (
     TracksEndpointResponseJSON,
     VideosEndpointResponseJSON,
 )
 from .track import Track
@@ -31,108 +32,118 @@
 
     def __post_init__(self):
         self.mix_dir: Optional[Path] = None
         self.mix_cover_saved: bool = False
 
     def set_metadata(self, session: Session):
         """Request from TIDAL API /mixes endpoint"""
-        self.metadata: Optional[SimpleNamespace] = request_mixes(
-            session=session, mix_id=self.mix_id
+        self.metadata: Optional[SimpleNamespace] = request_mix(
+            session=session, mix_id=self.mix_id, transparent=self.transparent
         )
 
         if self.metadata is None:
             return
 
         self.name = replace_illegal_characters(self.metadata.title)
 
     def set_items(self, session: Session):
         """Uses data from TIDAL API /mixes/items endpoint to
         populate self.items"""
-        mix_items: Optional[MixesItemsResponseJSON] = get_mix(
-            session=session, mix_id=self.mix_id
-        )
-        if mix_items is None:
+        try:
+            mix_items: Optional[MixesItemsResponseJSON] = retrieve_mix_items(
+                session=session, mix_id=self.mix_id, transparent=self.transparent
+            )
+        except TidalMixException as tme:
+            logger.exception(tme.args[0])
             self.items = tuple()
         else:
-            self.items: Tuple[Optional[MixItem]] = tuple(filter(None, mix_items.items))
+            if mix_items is None:
+                self.items = tuple()
+            else:
+                self.items: Tuple[Optional[MixItem]] = tuple(
+                    filter(None, mix_items.items)
+                )
 
     def set_mix_dir(self, out_dir: Path):
         """Populates self.mix_dir based on self.name, self.mix_id"""
         mix_substring: str = f"{self.name} [{self.mix_id}]"
         self.mix_dir: Path = out_dir / "Mixes" / mix_substring
         self.mix_dir.mkdir(parents=True, exist_ok=True)
 
     def save_cover_image(self, session: Session, out_dir: Path):
         """Requests self.metadata.image and attempts to write it to disk"""
         if self.mix_dir is None:
             self.set_mix_dir(out_dir=out_dir)
         self.cover_path: Path = self.mix_dir / "cover.jpg"
+
         if not self.cover_path.exists():
             with session.get(
                 url=self.metadata.image, params={k: None for k in session.params}
             ) as r:
                 (self.mix_dir / "cover.jpg").write_bytes(r.content)
 
             self.mix_cover_saved = True
         else:
-            self.mix_cover_saved = True
+            if self.cover_path.stat().st_size > 0:
+                self.mix_cover_saved = True
 
     def get_items(
         self, session: Session, audio_format: AudioFormat, no_extra_files: bool
-    ):
+    ) -> Tuple[Optional[Union[Track, Video]]]:
         """Using either Track.get() or Video.get(), attempt to request
         the data for each track or video in self.items."""
         if len(self.items) == 0:
             self.files = {}
             return
 
-        tracks_videos: list = [None] * len(self.items)
+        tracks_videos: List[Optional[Union[Track, Video]]] = [None] * len(self.items)
         for i, item in enumerate(self.items):
             if item is None:
                 tracks_videos[i] = None
                 continue
             elif isinstance(item, TracksEndpointResponseJSON):
                 track: Track = Track(track_id=item.id, transparent=self.transparent)
                 track.get(
                     session=session,
                     audio_format=audio_format,
                     out_dir=self.mix_dir,
                     metadata=item,
                     no_extra_files=no_extra_files,
+                    origin_jpg=False,
                 )
                 tracks_videos[i] = track
             elif isinstance(item, VideosEndpointResponseJSON):
                 video: Video = Video(video_id=item.id, transparent=self.transparent)
                 video.get(
                     session=session,
                     out_dir=self.mix_dir,
                     metadata=item,
                 )
                 tracks_videos[i] = video
             else:
                 tracks_videos[i] = None
                 continue
         else:
-            self.tracks_videos: Tuple[Tuple[int, Optional[Union[Track, Video]]]] = (
-                tuple(tracks_videos)
+            self.tracks_videos: Tuple[Optional[Union[Track, Video]]] = tuple(
+                tracks_videos
             )
         return tracks_videos
 
     def flatten_mix_dir(self):
         """When self.get_items() is called, the tracks and/or videos in
         self.items are downloaded using their self-contained .get() logic;
         this means that they will be downloaded to albums. This function
         "flattens" self.mix_dir, meaning that it moves all downloaded
         audio and video files to self.mix_dir, and removes the various
         subdirectories created"""
         files: List[Dict[int, Optional[str]]] = [None] * len(self.tracks_videos)
         if len(self.tracks_videos) == 0:
             return
-        subdirs: Set[Path] = set()
 
+        subdirs: Set[Path] = set()
         for i, tv in enumerate(self.tracks_videos, 1):
             if getattr(tv, "outfile") is None:
                 try:
                     getattr(tv, "album_dir")
                 except AttributeError:
                     pass
                 else:
@@ -293,14 +304,15 @@
                 track: Track = Track(track_id=item.id, transparent=self.transparent)
                 track_file: Optional[str] = track.get(
                     session=session,
                     audio_format=audio_format,
                     out_dir=out_dir,
                     metadata=item,
                     no_extra_files=no_extra_files,
+                    origin_jpg=False,
                 )
                 files[i] = track_file
             elif isinstance(item, VideosEndpointResponseJSON):
                 video: Video = Video(video_id=item.id, transparent=self.transparent)
                 video_file: Optional[str] = video.get(
                     session=session,
                     out_dir=self.mix_dir,
@@ -314,77 +326,104 @@
             self.files: List[Optional[str]] = files
 
 
 class TidalMixException(Exception):
     pass
 
 
-def request_mixes(session: Session, mix_id: str) -> Optional[SimpleNamespace]:
+def request_mix(
+    session: Session, mix_id: str, transparent: bool = False
+) -> Optional[SimpleNamespace]:
     """Request from TIDAL API /pages/mix endpoint. If an error occurs from
     session.get(), None is returned. Otherwise, a typing.SimpleNamespace
     object is returned with some metadata to do with the mix: title,
     description, URL to cover image."""
     url: str = f"{TIDAL_API_URL}/pages/mix?mixId={mix_id}"
     kwargs: dict = {"url": url}
     kwargs["headers"] = {"Accept": "application/json"}
 
-    logger.info(f"Requesting from TIDAL API: mixes/{mix_id}/items")
+    json_name: str = f"pages-mix-{mix_id}_{uuid4().hex}.json"
+
+    logger.info(f"Requesting from TIDAL API: mixes/{mix_id}")
     with session.get(**kwargs) as resp:
         try:
             resp.raise_for_status()
         except HTTPError as he:
             if resp.status_code == 404:
                 logger.warning(
                     "404 Client Error: not found for TIDAL API endpoint pages/mix"
                 )
             else:
                 logger.exception(he)
             return
+        else:
+            if transparent:
+                Path(json_name).write_text(
+                    json.dumps(resp.json(), ensure_ascii=True, indent=4, sort_keys=True)
+                )
 
-        d = dict()
-        d["title"] = resp.json().get("title")
-        d["description"] = resp.json().get("rows")[0]["modules"][0]["mix"]["subTitle"]
+        d: Dict[str, str] = {
+            "title": resp.json().get("title"),
+            "description": resp.json().get("rows")[0]["modules"][0]["mix"]["subTitle"],
+        }
         d["image"] = (
             resp.json()
             .get("rows", [{}])[0]
             .get("modules")[0]["mix"]["images"]["LARGE"]["url"]
         )
 
         logger.debug(
             f"{resp.status_code} response from TIDAL API to request: pages/mix"
         )
         return SimpleNamespace(**d)
 
 
-def request_mix_items(session: Session, mix_id: str) -> Optional[Dict]:
+def request_mixes_items(
+    session: Session,
+    mix_id: str,
+    offset: Optional[int] = None,
+    transparent: bool = False,
+) -> Optional[Dict]:
     """Request from TIDAL API /mixes/items endpoint. If error arises when
     requesting with 'session'.get(), None is returned. Otherwise, the
     dict object returned by requests.Response.json() is returned."""
     url: str = f"{TIDAL_API_URL}/mixes/{mix_id}/items"
     kwargs: dict = {"url": url}
-    kwargs["params"] = {"limit": 100}
+    kwargs["params"] = (
+        {"limit": 100} if offset is None else {"limit": 100, "offset": offset}
+    )
     kwargs["headers"] = {"Accept": "application/json"}
+    json_name: str = f"mixes-{mix_id}-items_{uuid4().hex}.json"
 
     data: Optional[dict] = None
     logger.info(f"Requesting from TIDAL API: mixes/{mix_id}/items")
     with session.get(**kwargs) as resp:
         try:
             resp.raise_for_status()
         except HTTPError as he:
             if resp.status_code == 404:
                 logger.warning(
                     f"404 Client Error: not found for TIDAL API endpoint mixes/{mix_id}/items"
                 )
             else:
                 logger.exception(he)
         else:
-            data = resp.json()
-            logger.debug(
-                f"{resp.status_code} response from TIDAL API to request: mixes/{mix_id}/items"
-            )
+            if transparent:
+                Path(json_name).write_text(
+                    json.dumps(resp.json(), ensure_ascii=True, indent=4, sort_keys=True)
+                )
+                data = resp.json()
+                logger.debug(
+                    f"{resp.status_code} response from TIDAL API to request: mixes/{mix_id}/items"
+                )
+            else:
+                data = resp.json()
+                logger.debug(
+                    f"{resp.status_code} response from TIDAL API to request: mixes/{mix_id}/items"
+                )
         finally:
             return data
 
 
 @dataclass(frozen=True)
 class MixesItemsResponseJSON:
     """The response from the TIDAL API endpoint /mixes/<ID>/items
@@ -394,15 +433,15 @@
     offset: int
     total_number_of_items: int
     items: Tuple[
         Optional[Union["TracksEndpointResponseJSON", "VideosEndpointResponseJSON"]]
     ]
 
 
-def mix_maker(
+def mix_items_response_json_maker(
     mixes_response: Dict[str, Union[int, List[dict]]],
 ) -> "MixesItemsResponseJSON":
     """This function massages the response from the TIDAL API endpoint
     mixes/items into a format that MixesItemsResponseJSON.from_dict()
     can ingest. Returns a MixesItemsResponseJSON instance"""
     init_args: dict = {}
     init_args["limit"] = mixes_response.get("limit")
@@ -448,21 +487,73 @@
             continue  # value stays None
     else:
         init_args["items"] = tuple(mixes_items)
 
     return MixesItemsResponseJSON(**init_args)
 
 
-def get_mix(session: Session, mix_id: str) -> Optional["MixesItemsResponseJSON"]:
+def retrieve_mix_items(
+    session: Session, mix_id: str, transparent: bool = False
+) -> Optional["MixesItemsResponseJSON"]:
     """The pattern for mix items retrieval does not follow the
-    requesting.request_* functions, hence its implementation here.
+    requesting.request_* functions, hence its implementation here. N.b.
+    if the first response from /mixes/<ID>/items endpoint indicates that
+    the playlist contains more than 100 items, multiple requests will be
+    sent until all N > 100 items are retrieved.
     """
     mixes_items_response_json: Optional["MixesItemsResponseJSON"] = None
+    mixes_response: Optional[dict] = request_mixes_items(
+        session=session, mix_id=mix_id, transparent=transparent
+    )
+    if mixes_response is None:
+        raise TidalMixException(f"Could not retrieve the items in mix '{mix_id}'")
+
+    total_number_of_items: Optional[int] = mixes_response.get("totalNumberOfItems")
+    if total_number_of_items is None:
+        raise TidalMixException(
+            f"TIDAL API did not respond with number of items in mix '{mix_id}'"
+        )
+    else:
+        logger.info(f"Mix '{mix_id}' is comprised of {total_number_of_items} items")
+
+    num_items: int = len(mixes_response.get("items", []))
+    if num_items == 0:
+        raise TidalMixException(
+            f"TIDAL API did not return any mix items for mix '{mix_id}'"
+        )
+
+    if num_items < total_number_of_items:
+        items_to_retrieve: int = total_number_of_items
+        all_items_mixes_response: dict = mixes_response
+        if total_number_of_items > 100:
+            items_list: List[dict] = mixes_response.pop("items")
+            offset: int = 100
+            while items_to_retrieve > 0:
+                mr: Optional[dict] = request_mixes_items(
+                    session=session, mix_id=mix_id, offset=offset
+                )
+                if (mr is not None) and ((mr_items := mr.get("items")) is not None):
+                    items_list += mr_items
+                    offset += 100
+                    items_to_retrieve -= 100
+                else:
+                    logger.exception(
+                        TidalMixException(
+                            f"Could not retrieve more than {len(items_list)} "
+                            f"elements of mix '{mix_id}'. Continuing "
+                            "without the remaining "
+                            f"{total_number_of_items - len(items_list)}"
+                        )
+                    )
+        else:
+            all_items_mixes_response = mixes_response
+    else:
+        all_items_mixes_response = mixes_response
+
     try:
-        mixes_response: dict = request_mix_items(session=session, mix_id=mix_id)
-        mixes_items_response_json: Optional["MixesItemsResponseJSON"] = mix_maker(
-            mixes_response=mixes_response
+        mixes_items_response_json: Optional["MixesItemsResponseJSON"] = (
+            mix_items_response_json_maker(mixes_response=all_items_mixes_response)
         )
     except Exception as e:
         logger.exception(TidalMixException(e.args[0]))
     finally:
         return mixes_items_response_json
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/models.py` & `tidal_wave-2024.4.3/tidal_wave/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     payment_overdue: bool
 
 
 @dataclass(frozen=True)
 class AlbumsItemsResponseJSONItem:
     """A sub-object of the response from the TIDAL API endpoint
     /albums/<ID>/items. It simply denotes the type of item, which is surely
-    going to be 'track', and the same object that is returned from the TIDAL
+    going to be 'track', and is the same object that is returned from the TIDAL
     API /tracks endpoint."""
 
     item: "TracksEndpointResponseJSON"
     type: str  # "track"
 
 
 @dataclass(frozen=True)
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/oauth.py` & `tidal_wave-2024.4.3/tidal_wave/oauth.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.2/tidal_wave/playlist.py` & `tidal_wave-2024.4.3/tidal_wave/playlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import math
 from pathlib import Path
 import shutil
 import sys
 from types import SimpleNamespace
 from typing import Dict, List, Optional, Set, Tuple, Union
+from uuid import uuid4
 
 from .media import AudioFormat
 from .models import (
     PlaylistsEndpointResponseJSON,
     TracksEndpointResponseJSON,
     VideosEndpointResponseJSON,
 )
@@ -49,26 +50,23 @@
         if self.metadata is None:
             return
 
         self.name = replace_illegal_characters(self.metadata.title)
 
     def set_items(self, session: Session):
         """Uses data from TIDAL API /playlists/items endpoint to
-        populate self.items"""
-        playlist_items: Optional[PlaylistsItemsResponseJSON] = get_playlist(
+        populate self.items.  If 'totalNumberOfItems' field returned
+        has value greater than 100, multiple requests of size <= 100 will be
+        sent to the endpoint until all items for the playlist are retrieved."""
+        playlist_items: Optional[PlaylistsItemsResponseJSON] = retrieve_playlist_items(
             session=session, playlist_id=self.playlist_id
         )
         if playlist_items is None:
             self.items = tuple()
         else:
-            # For now, if playlist size, N, exceeds 100 items,
-            # N items are returned, and all those between 101 and N
-            # are simply None. It's a temporary fix before properly
-            # handling paginated API requests, but it should stop
-            # NoneType errors!
             self.items: Tuple[Optional[PlaylistItem]] = tuple(
                 filter(None, playlist_items.items)
             )
 
     def set_playlist_dir(self, out_dir: Path):
         """Populates self.playlist_dir based on self.name, self.playlist_id"""
         playlist_substring: str = f"{self.name} [{self.playlist_id}]"
@@ -115,30 +113,31 @@
                 track: Track = Track(track_id=item.id, transparent=self.transparent)
                 track.get(
                     session=session,
                     audio_format=audio_format,
                     out_dir=self.playlist_dir,
                     metadata=item,
                     no_extra_files=no_extra_files,
+                    origin_jpg=False,
                 )
                 tracks_videos[i] = track
             elif isinstance(item, VideosEndpointResponseJSON):
                 video: Video = Video(video_id=item.id, transparent=self.transparent)
                 video.get(
                     session=session,
                     out_dir=self.playlist_dir,
                     metadata=item,
                 )
                 tracks_videos[i] = video
             else:
                 tracks_videos[i] = None
                 continue
         else:
-            self.tracks_videos: Tuple[Tuple[int, Optional[Union[Track, Video]]]] = (
-                tuple(tracks_videos)
+            self.tracks_videos: Tuple[Optional[Union[Track, Video]]] = tuple(
+                tracks_videos
             )
         return tracks_videos
 
     def flatten_playlist_dir(self):
         """When self.get_items() is called, the tracks and/or videos in
         self.items are downloaded using their self-contained .get() logic;
         this means that they will be downloaded to albums. This function
@@ -188,15 +187,14 @@
                 new_path.write_bytes(_path.read_bytes())
                 _path.unlink()
                 files[i - 1] = {i: str(new_path.absolute())}
         else:
             self.files: List[Dict[int, Optional[str]]] = files
 
         # Find all subdirectories written to
-        subdirs: Set[Path] = set()
         for tv in self.tracks_videos:
             if isinstance(tv, Track):
                 try:
                     getattr(tv, "album_dir")
                 except AttributeError:
                     pass
                 else:
@@ -420,14 +418,15 @@
                 track: Track = Track(track_id=item.id, transparent=self.transparent)
                 track_file: Optional[str] = track.get(
                     session=session,
                     audio_format=audio_format,
                     out_dir=out_dir,
                     metadata=item,
                     no_extra_files=no_extra_files,
+                    origin_jpg=False,
                 )
                 files[i] = {i: track_file}
             elif isinstance(item, VideosEndpointResponseJSON):
                 video: Video = Video(video_id=item.id, transparent=self.transparent)
                 video_file: Optional[str] = video.get(
                     session=session,
                     out_dir=out_dir,
@@ -441,41 +440,59 @@
             self.files: List[Dict[int, Optional[str]]] = files
 
 
 class TidalPlaylistException(Exception):
     pass
 
 
-def request_playlist_items(session: Session, playlist_id: str) -> Optional[dict]:
+def request_playlists_items(
+    session: Session,
+    playlist_id: str,
+    offset: Optional[int] = None,
+    transparent: bool = False,
+) -> Optional[dict]:
     """Request from TIDAL API /playlists/items endpoint. If requests.HTTPError
     arises, warning is logged; upon this or any other exception, None is returned.
     If no exception arises from 'session'.get(), the requests.Response.json()
-    object is returned."""
+    object is returned. If transparent is True, all JSON responses from the API
+    are written to disk"""
     url: str = f"{TIDAL_API_URL}/playlists/{playlist_id}/items"
     kwargs: dict = {"url": url}
-    kwargs["params"] = {"limit": 100}
+    kwargs["params"] = (
+        {"limit": 100} if offset is None else {"limit": 100, "offset": offset}
+    )
     kwargs["headers"] = {"Accept": "application/json"}
+    json_name: str = f"playlists-{playlist_id}-items_{uuid4().hex}.json"
 
     data: Optional[dict] = None
     logger.info(f"Requesting from TIDAL API: playlists/{playlist_id}/items")
     with session.get(**kwargs) as resp:
         try:
             resp.raise_for_status()
         except HTTPError as he:
             if resp.status_code == 404:
                 logger.warning(
                     f"404 Client Error: not found for TIDAL API endpoint playlists/{playlist_id}/items"
                 )
             else:
                 logger.exception(he)
         else:
-            data = resp.json()
-            logger.debug(
-                f"{resp.status_code} response from TIDAL API to request: playlists/{playlist_id}/items"
-            )
+            if transparent:
+                Path(json_name).write_text(
+                    json.dumps(resp.json(), ensure_ascii=True, indent=4, sort_keys=True)
+                )
+                data = resp.json()
+                logger.debug(
+                    f"{resp.status_code} response from TIDAL API to request: playlists/{playlist_id}/items"
+                )
+            else:
+                data = resp.json()
+                logger.debug(
+                    f"{resp.status_code} response from TIDAL API to request: playlists/{playlist_id}/items"
+                )
         finally:
             return data
 
 
 @dataclass(frozen=True)
 class PlaylistsItemsResponseJSON:
     """The response from the TIDAL API endpoint /playlists/<ID>/items
@@ -485,24 +502,25 @@
     offset: int
     total_number_of_items: int
     items: Tuple[
         Optional[Union["TracksEndpointResponseJSON", "VideosEndpointResponseJSON"]]
     ]
 
 
-def playlist_maker(
+def playlists_items_response_json_maker(
     playlists_response: Dict[str, Union[int, List[dict]]],
 ) -> "PlaylistsItemsResponseJSON":
     """This function massages the response from the TIDAL API endpoint
-    playlists/items into a format that PlaylistsItemsResponseJSON.from_dict()
-    can ingest. Returns a PlaylistsItemsResponseJSON instance"""
-    init_args: dict = {}
-    init_args["limit"] = playlists_response.get("limit")
-    init_args["offset"] = playlists_response.get("offset")
-    init_args["total_number_of_items"] = playlists_response.get("totalNumberOfItems")
+    /playlists/items into a format that PlaylistsItemsResponseJSON.__init__()
+    can ingest, and then returns a PlaylistsItemsResponseJSON instance"""
+    init_args: Dict[str, Optional[int]] = {
+        "limit": playlists_response.get("limit"),
+        "offset": playlists_response.get("offset"),
+        "total_number_of_items": playlists_response.get("totalNumberOfItems"),
+    }
 
     items: Tuple[SimpleNamespace] = tuple(
         SimpleNamespace(**d) for d in playlists_response["items"]
     )
     if len(items) == 0:
         return
 
@@ -539,27 +557,75 @@
             continue  # value stays None
     else:
         init_args["items"] = tuple(playlist_items)
 
     return PlaylistsItemsResponseJSON(**init_args)
 
 
-def get_playlist(
-    session: Session, playlist_id: str
+def retrieve_playlist_items(
+    session: Session,
+    playlist_id: str,
+    transparent: bool = False,
 ) -> Optional["PlaylistsItemsResponseJSON"]:
     """The pattern for playlist items retrieval does not follow the
-    requesting.request_* functions, hence its implementation here.
-    """
+    requesting.request_* functions, hence its implementation here. N.b.
+    if the first response from /playlists/items endpoint indicates that
+    the playlist contains more than 100 items, multiple requests will be
+    sent until all N > 100 items are retrieved."""
     playlists_items_response_json: Optional["PlaylistsItemsResponseJSON"] = None
-    try:
-        playlists_response: dict = request_playlist_items(
-            session=session, playlist_id=playlist_id
+    playlists_response: Optional[dict] = request_playlists_items(
+        session=session, playlist_id=playlist_id, transparent=transparent
+    )
+    if playlists_response is None:
+        raise TidalPlaylistException(
+            f"Could not retrieve the items in playlist '{playlist_id}'"
+        )
+
+    total_number_of_items: Optional[int] = playlists_response.get("totalNumberOfItems")
+    logger.info(
+        f"Playlist '{playlist_id}' is comprised of {total_number_of_items} items"
+    )
+    if total_number_of_items is None:
+        raise TidalPlaylistException(
+            f"TIDAL API did not respond with number of items in playlist '{playlist_id}'"
         )
+    else:
+        items_to_retrieve: int = total_number_of_items
+
+    all_items_playlist_response: dict = playlists_response
+
+    if total_number_of_items > 100:
+        items_list: List[dict] = playlists_response.pop("items")
+        offset: int = 100
+        while items_to_retrieve > 0:
+            pr: Optional[dict] = request_playlists_items(
+                session=session, playlist_id=playlist_id, offset=offset
+            )
+
+            if (pr is not None) and ((pr_items := pr.get("items")) is not None):
+                items_list += pr_items
+                offset += 100
+                items_to_retrieve -= 100
+            else:
+                logger.exception(
+                    TidalPlaylistException(
+                        f"Could not retrieve more than {len(items_list)} "
+                        f"elements of playlist '{playlist_id}'. Continuing "
+                        "without the remaining "
+                        f"{total_number_of_items - len(items_list)}"
+                    )
+                )
+        else:
+            all_items_playlist_response["items"] = items_list
+
+    try:
         playlists_items_response_json: Optional["PlaylistsItemsResponseJSON"] = (
-            playlist_maker(playlists_response=playlists_response)
+            playlists_items_response_json_maker(
+                playlists_response=all_items_playlist_response
+            )
         )
     except Exception as e:
         logger.exception(TidalPlaylistException(e.args[0]))
     finally:
         return playlists_items_response_json
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/requesting.py` & `tidal_wave-2024.4.3/tidal_wave/requesting.py`

 * *Files 19% similar despite different names*

```diff
@@ -60,37 +60,42 @@
     identifier: int,
     url_end: str = "",
     headers: Optional[dict] = None,
     parameters: Optional[dict] = None,
     subclass: Optional["ResponseJSON"] = None,
     credits_flag: bool = False,
     transparent: bool = False,
+    offset: Optional[int] = None,
 ) -> Callable:
     """This function is a function factory: it crafts nearly identical
     versions of the same logic: send a GET request to a certain endpoint;
     if a requests.HTTPError arises, return None; else, transform the
     JSON response into an instance of a subclass of JSONWizard."""
 
-    def function(s, e, i, u, h, p, sc, cf, t):
+    def function(s, e, i, u, h, p, sc, cf, t, o):
         url: str = f"{TIDAL_API_URL}/{e}/{i}{u}"
         kwargs: dict = {"url": url}
         if p is not None:
-            kwargs["params"] = p
+            kwargs["params"] = p if offset is None else p | {"offset": offset}
+        else:
+            if offset is not None:
+                kwargs["params"] = {"offset": offset}
+
         if h is not None:
             kwargs["headers"] = h
 
         @backoff.on_predicate(
             backoff.expo,
             predicate=lambda r: r.status_code == 429,
             jitter=backoff.random_jitter,
             max_time=15,
             logger=logger,
         )
         def _get(s: Session, request_kwargs: dict) -> Response:
-            """Return a requests.Response object, from having passed request_kwargs
+            """Return a requests.Response object from having passed request_kwargs
             to s.get(), optionally retrying if 429 error occurs."""
             with s.get(**request_kwargs) as r:
                 return r
 
         data: Optional[sc] = None
         logger.info(f"Requesting from TIDAL API: {e}/{i}{u}")
         resp: Response = _get(s=s, request_kwargs=kwargs)
@@ -131,109 +136,134 @@
         i=identifier,
         u=url_end,
         h=headers,
         p=parameters,
         sc=subclass,
         cf=credits_flag,
         t=transparent,
+        o=offset,
     )
 
 
 # Functions will curry all arguments except session and identifier, as those
 # don't change during runtime, and session is only available once the __main__
 # process (on the happy path) creates a requests.Session object. Identifier
 # varies with the media type, etc.
-
-
 def request_albums(
     session: Session, album_id: int, transparent: bool = False
 ) -> Optional[AlbumsEndpointResponseJSON]:
+    """Send a GET request to the /albums endpoint of the TIDAL API. If an
+    Exception occurs, return None. Else, return an instance of
+    AlbumsEndpointResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="albums",
         identifier=album_id,
         headers={"Accept": "application/json"},
         subclass=AlbumsEndpointResponseJSON,
         transparent=transparent,
     )
 
 
-def request_album_items(
-    session: Session, album_id: int, transparent: bool = False
+def request_albums_items(
+    session: Session,
+    album_id: int,
+    transparent: bool = False,
+    offset: Optional[int] = None,
 ) -> Optional[AlbumsItemsResponseJSON]:
+    """Send a GET request to the /albums/<album ID>/items
+    endpoint of the TIDAL API. If an Exception occurs,
+    return None. Else, return an instance of
+    AlbumsItemsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="albums",
         identifier=album_id,
         headers={"Accept": "application/json"},
         parameters={"limit": 100},
         url_end="/items",
         subclass=AlbumsItemsResponseJSON,
         transparent=transparent,
+        offset=offset,
     )
 
 
 def request_album_review(
     session: Session, album_id: int, transparent: bool = False
 ) -> Optional[AlbumsReviewResponseJSON]:
+    """Send a GET request to the /albums/<album ID>/review
+    endpoint of the TIDAL API. If an Exception occurs, return None.
+    Else, return an instance of AlbumsReviewResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="albums",
         identifier=album_id,
         headers={"Accept": "application/json"},
         url_end="/review",
         subclass=AlbumsReviewResponseJSON,
         transparent=transparent,
     )
 
 
 def request_artist_bio(
     session: Session, artist_id: int, transparent: bool = False
 ) -> Optional[ArtistsBioResponseJSON]:
+    """Send a GET request to the /artists/<artist ID>/bio
+    endpoint of the TIDAL API. If an Exception occurs, return None.
+    Else, return an instance of ArtistsBioResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="artists",
         identifier=artist_id,
         headers={"Accept": "application/json"},
         url_end="/bio",
         subclass=ArtistsBioResponseJSON,
         transparent=transparent,
     )
 
 
 def request_artists(
     session: Session, artist_id: int, transparent: bool = False
 ) -> Optional[ArtistsEndpointResponseJSON]:
+    """Send a GET request to the /artists endpoint of the TIDAL API.
+    If an Exception occurs, return None. Else, return an instance of
+    ArtistsEndpointResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="artists",
         identifier=artist_id,
         headers={"Accept": "application/json"},
         subclass=ArtistsEndpointResponseJSON,
         transparent=transparent,
     )
 
 
 def request_artists_albums(
     session: Session, artist_id: int, transparent: bool = False
 ) -> Optional[ArtistsAlbumsResponseJSON]:
+    """Send a GET request to the /artists/<artist ID>/albums
+    endpoint of the TIDAL API. If an Exception occurs, return None.
+    Else, return an instance of ArtistsAlbumsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="artists",
         identifier=artist_id,
         headers={"Accept": "application/json"},
         url_end="/albums",
         subclass=ArtistsAlbumsResponseJSON,
         transparent=transparent,
     )
 
 
 def request_artists_audio_works(
     session: Session, artist_id: int, transparent: bool = False
 ) -> Optional[ArtistsAlbumsResponseJSON]:
+    """Send a GET request to the /artists/<artist ID>/albums
+    endpoint of the TIDAL API. If an Exception occurs, return None.
+    Else, return an instance of ArtistsAlbumsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="artists",
         identifier=artist_id,
         headers={"Accept": "application/json"},
         parameters={"filter": "EPSANDSINGLES"},
         url_end="/albums",
@@ -241,28 +271,34 @@
         transparent=transparent,
     )
 
 
 def request_artists_videos(
     session: Session, artist_id: int, transparent: bool = False
 ) -> Optional[ArtistsVideosResponseJSON]:
+    """Send a GET request to the /artists/<artist ID>/videos
+    endpoint of the TIDAL API. If an Exception occurs, return None.
+    Else, return an instance of ArtistsVideosResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="artists",
         identifier=artist_id,
         headers={"Accept": "application/json"},
         url_end="/videos",
         subclass=ArtistsVideosResponseJSON,
         transparent=transparent,
     )
 
 
 def request_tracks(
     session: Session, track_id: int, transparent: bool = False
 ) -> Optional[TracksEndpointResponseJSON]:
+    """Send a GET request to the /tracks endpoint of the TIDAL API.
+    If an Exception occurs, return None. Else, return an instance of
+    TracksEndpointResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="tracks",
         identifier=track_id,
         headers={"Accept": "application/json"},
         subclass=TracksEndpointResponseJSON,
         transparent=transparent,
@@ -271,14 +307,17 @@
 
 # This one's special, because its JSON response isn't proper JSON:
 # it's just an array of JSON objects, so we have to pass a flag to mark
 # that the logic common to the rest of the functions is slightly different here.
 def request_credits(
     session: Session, track_id: int, transparent: bool = False
 ) -> Optional[TracksCreditsResponseJSON]:
+    """Send a GET request to the /tracks/<track ID>/credits endpoint of the
+    TIDAL API. If an Exception occurs, return None. Else, return an instance
+    of TracksCreditsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="tracks",
         identifier=track_id,
         headers={"Accept": "application/json"},
         parameters={"includeContributors": True},
         url_end="/credits",
@@ -290,14 +329,17 @@
 
 # This one's special, because its JSON response isn't proper JSON:
 # it's just an array of JSON objects, so we have to pass a flag to mark
 # that the logic common to the rest of the functions is slightly different here.
 def request_albums_credits(
     session: Session, album_id: int, transparent: bool = False
 ) -> Optional[AlbumsCreditsResponseJSON]:
+    """Send a GET request to the /albums/<album ID>/credits endpoint of the
+    TIDAL API. If an Exception occurs, return None. Else, return an instance
+    of AlbumsCreditsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="albums",
         identifier=album_id,
         headers={"Accept": "application/json"},
         parameters={"includeContributors": True, "limit": 50},
         url_end="/credits",
@@ -306,14 +348,17 @@
         transparent=transparent,
     )
 
 
 def request_lyrics(
     session: Session, track_id: int, transparent: bool = False
 ) -> Optional[TracksLyricsResponseJSON]:
+    """Send a GET request to the /tracks/<track ID>/lyrics endpoint of the
+    TIDAL API. If an Exception occurs, return None. Else, return an instance
+    of TracksLyricsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="tracks",
         identifier=track_id,
         headers={"Accept": "application/json"},
         url_end="/lyrics",
         subclass=TracksLyricsResponseJSON,
@@ -322,14 +367,17 @@
 
 
 # One more layer of currying here, as the parameters argument
 # is dependent on a runtime variable.
 def request_stream(
     session: Session, track_id: int, audio_quality: str, transparent: bool = False
 ) -> Optional[TracksEndpointStreamResponseJSON]:
+    """Send a GET request to the /tracks/<track ID>/playbackinfopostpaywall
+    endpoint of the TIDAL API. If an Exception occurs, return None. Else,
+    return an instance of TracksEndpointStreamResponseJSON"""
     func = partial(
         requester_maker,
         session=session,
         endpoint="tracks",
         identifier=track_id,
         headers={"Accept": "application/json"},
         parameters={
@@ -343,27 +391,33 @@
     )
     return func()
 
 
 def request_videos(
     session: Session, video_id: int, transparent: bool = False
 ) -> Optional[VideosEndpointResponseJSON]:
+    """Send a GET request to the /videos endpoint of the TIDAL API.
+    If an Exception occurs, return None. Else, return an instance of
+    VideosEndpointResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="videos",
         identifier=video_id,
         headers={"Accept": "application/json"},
         subclass=VideosEndpointResponseJSON,
         transparent=transparent,
     )
 
 
 def request_video_contributors(
     session: Session, video_id: int, transparent: bool = False
 ) -> Optional[VideosContributorsResponseJSON]:
+    """Send a GET request to the /videos/<video ID>/contributors endpoint of the
+    TIDAL API. If an Exception occurs, return None. Else, return an instance
+    of VideosContributorsResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="videos",
         identifier=video_id,
         headers={"Accept": "application/json"},
         parameters={"limit": 100},
         url_end="/contributors",
@@ -371,14 +425,17 @@
         transparent=transparent,
     )
 
 
 def request_video_stream(
     session: Session, video_id: int, video_quality: str, transparent: bool = False
 ) -> Optional[VideosEndpointStreamResponseJSON]:
+    """Send a GET request to the /videos/<video ID>/playbackinfopostpaywall
+    endpoint of the TIDAL API. If an Exception occurs, return None. Else,
+    return an instance of VideosEndpointStreamResponseJSON"""
     func = partial(
         requester_maker,
         session=session,
         identifier=video_id,
         endpoint="videos",
         headers={"Accept": "application/json"},
         parameters={
@@ -392,14 +449,17 @@
     )
     return func()
 
 
 def request_playlists(
     session: Session, playlist_id: int, transparent: bool = False
 ) -> Optional[PlaylistsEndpointResponseJSON]:
+    """Send a GET request to the /playlists endpoint of the TIDAL API.
+    If an Exception occurs, return None. Else, return an instance of
+    PlaylistsEndpointResponseJSON"""
     return requester_maker(
         session=session,
         endpoint="playlists",
         identifier=playlist_id,
         headers={"Accept": "application/json"},
         subclass=PlaylistsEndpointResponseJSON,
         transparent=transparent,
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/track.py` & `tidal_wave-2024.4.3/tidal_wave/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     request_albums,
     request_artist_bio,
     request_credits,
     request_lyrics,
     request_stream,
     request_tracks,
 )
-from .utils import download_cover_image, temporary_file
+from .utils import download_cover_image, temporary_file, IMAGE_URL
 
 import ffmpeg
 import mutagen
 from mutagen.mp4 import MP4Cover
-from requests import Session
+from requests import RequestException, Session
 from Crypto.Cipher import AES
 from Crypto.Util import Counter
 
 logger = logging.getLogger("__name__")
 
 
 @dataclass
@@ -289,14 +289,35 @@
         """This method saves cover.jpg to self.album_dir; the bytes for cover.jpg
         come from self.album.cover"""
         if not self.cover_path.exists():
             download_cover_image(
                 session=session, cover_uuid=self.album.cover, output_dir=self.album_dir
             )
 
+    def original_album_cover(self, session: Session):
+        """For most albums, TIDAL features the "original" album cover, in the highest
+        resolution possible. This JPEG can be too large to be embedded into FLAC tracks,
+        however it is ideal to have for music archiving etc. purposes. This method requests
+        the original cover and overwrites the smaller, 1280x1280 image used to embed into the
+        track file. The filename on the API side is origin.jpg. It is *probably* okay to
+        get this URL as a track.Track method, as HTTP requests are cached, so e.g. executing
+        this method for each track in an album won't result in many redundant GET requests
+        """
+        origin_jpg_url: str = IMAGE_URL % f"{self.album.cover.replace('-', '/')}/origin"
+        with session.get(url=origin_jpg_url, headers={"Accept": "image/jpeg"}) as resp:
+            try:
+                resp.raise_for_status()
+            except RequestException as re:
+                logger.warning(
+                    "Could not retrieve origin.jpg from TIDAL "
+                    f"due to error '{re.args[0]}'"
+                )
+            else:
+                (self.album_dir / "cover.jpg").write_bytes(resp.content)
+
     def set_urls(self, session: Session):
         """This method sets self.urls based on self.manifest"""
         if isinstance(self.manifest, JSONDASHManifest):
             self.urls: List[str] = self.manifest.urls
         elif isinstance(self.manifest, XMLDASHManifest):
             self.urls: List[str] = self.manifest.build_urls(session=session)
         self.download_headers: Dict[str, str] = {"Accept": self.manifest.mime_type}
@@ -673,15 +694,15 @@
         self,
         session: Session,
         audio_format: AudioFormat,
         out_dir: Path,
         metadata: Optional[TracksEndpointResponseJSON] = None,
         album: Optional[AlbumsEndpointResponseJSON] = None,
         no_extra_files: bool = True,
-        transparent: bool = False,
+        origin_jpg: bool = True,
     ) -> Optional[str]:
         """This is the main driver method of Track. It executes the other
         methods in order, catching Exceptions and attempting to handle
         edge cases."""
 
         if metadata is None:
             self.set_metadata(session)
@@ -802,14 +823,20 @@
             except Exception:
                 pass
 
             try:
                 self.save_artist_bio(session)
             except Exception:
                 pass
+
+            if origin_jpg:
+                try:
+                    self.original_album_cover(session)
+                except Exception:
+                    pass
         else:
             try:
                 self.cover_path.unlink()
             except FileNotFoundError:
                 pass
 
         return self.absolute_outfile
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/utils.py` & `tidal_wave-2024.4.3/tidal_wave/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     session: Session,
     cover_uuid: str,
     output_dir: Path,
     file_name: str = "cover.jpg",
     dimension: Union[int, Tuple[int]] = 1280,
 ) -> Optional[Path]:
     """Given a UUID that corresponds to a (JPEG) image on Tidal's servers,
-    download the image file and write it as 'cover.jpeg' or 'cover.png'
-    in the directory `path_to_output_dir`. Returns path to downloaded file"""
+    download the image file and write it as 'cover.jpeg' in the directory
+    'output_dir'. Returns path to downloaded file"""
     cover_url_part: str = cover_uuid.replace("-", "/")
     if isinstance(dimension, int):
         _url: str = IMAGE_URL % f"{cover_url_part}/{dimension}x{dimension}"
     elif isinstance(dimension, tuple):
         _url: str = IMAGE_URL % f"{cover_url_part}/{dimension[0]}x{dimension[1]}"
 
     with session.get(url=_url, headers={"Accept": "image/jpeg"}) as r:
         if not r.ok:
             logger.warning(
-                "Could not retrieve data from Tidal resources/images URL "
+                "Could not retrieve data from TIDAL resources/images URL "
                 f"due to error code: {r.status_code}"
             )
             logger.debug(r.reason)
             return
         else:
             bytes_to_write = BytesIO(r.content)
```

### Comparing `tidal-wave-2024.4.2/tidal_wave/video.py` & `tidal_wave-2024.4.3/tidal_wave/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
             try:
                 ffmpeg.input(tf.name, hide_banner=None, y=None).output(
                     self.absolute_outfile,
                     vcodec="copy",
                     acodec="copy",
                     loglevel="quiet",
-                    **{"movflags": "+faststart"}
+                    **{"movflags": "+faststart"},
                 ).run()
             except ffmpeg.Error:
                 logger.warning(
                     f"Could not convert video {self.video_id} with FFmpeg: "
                     "metadata will not be added and format will stay as MPEG-TS"
                 )
```

### Comparing `tidal-wave-2024.4.2/tidal_wave.egg-info/PKG-INFO` & `tidal_wave-2024.4.3/tidal_wave.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -225,15 +225,15 @@
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: m3u8==4.1.0
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: requests[socks]==2.31.0
-Requires-Dist: typer==0.12.1
+Requires-Dist: typer==0.12.3
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
 [![GNU/Linux amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml)
@@ -250,36 +250,42 @@
 
 This software uses libraries from the [FFmpeg](http://ffmpeg.org) project under the [LGPLv2.1](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). FFmpeg is a trademark of [Fabrice Bellard](http://www.bellard.org/), originator of the FFmpeg project. 
 
 ## Features
 * Retrieve [FLAC](https://xiph.org/flac/), [Dolby Atmos](https://www.dolby.com/technologies/dolby-atmos/), [Sony 360 Reality Audio](https://electronics.sony.com/360-reality-audio), or [AAC](https://en.wikipedia.org/wiki/Advanced_Audio_Coding) tracks; [AVC/H.264](https://en.wikipedia.org/wiki/Advanced_Video_Coding) (up to 1920x1080) + [AAC](https://en.wikipedia.org/wiki/Advanced_Audio_Coding) videos
 * Either a single track or an entire album can be retrieved
 * Album covers are retrieved by default, and embedded into all tracks
+  - Highest-resolution, "original" album covers, which can be up to 6000x6000 pixels resolution, are retrieved if available
 * Support for albums with multiple discs
 * If available, lyrics are added as metadata to tracks
 * If available, album reviews are retrieved as JSON
 * If available, album credits are retrieved as JSON
 * If available, artist bios are retrieved as JSON
 * If available, artist images are retrieved as JPEG
 * Playlist retrieval support (video or audio or both)
 * Playlist .m3u8 file automatically created
 * Mix retrieval support (video or audio)
 * Artist's entire works retrieval support (video and audio; albums or albums and EPs and singles)
 * Because of the use of the `requests` package, system proxies are respected (HTTP, HTTPs, Socks); or can be specified by typical environment variable
 * Also because of the use of `requests`, very simple [`Cache-Control`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) request caching occurs via `CacheControl`
+* If desired, all JSON responses from the TIDAL API can be saved for inspection or posterity or debugging
 
 ## Getting Started
-A [HiFi Plus](https://tidal.com/pricing) account is **required** in order to retrieve HiRes FLAC, Dolby Atmos, and Sony 360 Reality Audio tracks. Simply a [HiFi](https://tidal.com/pricing) plan is sufficient to retrieve in 16-bit, 44.1 kHz (i.e., lossless) or lower quality as well as videos. More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
+A current, valid TIDAL subscription is required in order to run `tidal-wave`. Previously, TIDAL segmented the available audio qualities into HiFi and HiFi Plus plans: now, 
+> All current TIDAL plans feature Max sound quality formats such as full lossless, HiRes FLAC, and Dolby Atmos (up to 24-bit, 192 kHz).
+
+More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
 
 ### Requirements
  - As resources will be fetched from the World Wide Web, an Internet connection is required
- - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binary for Ubuntu GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_aarch64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_amd64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe) build FFmpeg from source, so separate installation is unnecessary.
+ - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binaries](https://github.com/ebb-earl-co/tidal-wave/releases/latest) build FFmpeg from source, so separate installation is unnecessary.
    - Static builds of FFmpeg are available from [John Van Sickle](https://www.johnvansickle.com/ffmpeg/) for GNU/Linux, or most package managers feature `ffmpeg`.
    - For macOS, the [FFmpeg download page](http://ffmpeg.org/download.html#build-mac) links to [this download source](https://evermeet.cx/ffmpeg/); or there is always [Homebrew](https://formulae.brew.sh/formula/ffmpeg)
    - For Windows, the [FFmpeg download page](http://ffmpeg.org/download.html#build-windows) lists 2 resources; or [`chocolatey`](https://community.chocolatey.org/packages/ffmpeg) is an option
+   - If a minimal FFmpeg, compiled from source, is desired, take a look at this project's [BUILDME.md](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/BUILDME.md) file for decent instructions
  - This is a Python package, so **to use it in the default manner** you will need [Python 3](https://www.python.org/downloads/), version 3.8 or newer, on your system.
    - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); and [PyInstaller](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, x86\_64 macOS, and x86\_64 Windows are provided for download and use that *do not require Python to be installed*
  - Only a handful of Python libraries are dependencies:
    - [`backoff`](https://pypi.org/project/backoff/)
    - [`cachecontrol`](https://pypi.org/project/CacheControl/)
    - [`dataclass-wizard`](https://pypi.org/project/dataclass-wizard/)
    - [`ffmpeg-python`](https://pypi.org/project/ffmpeg-python/)
@@ -298,36 +304,29 @@
 $ python3 -m pip install tidal-wave
 ```
 ```powershell
 # Windows
 PS > python.exe -m pip install tidal-wave
 ```
 
-Optionally, to get the full `typer` experience when using this utility, add `[all]` to the end of the `pip install command`:
-```bash
-$ python3 -m pip install tidal-wave[all]
-```
-```powershell
-PS > python.exe -m pip install tidal-wave[all]
-```
 ### `pip` Install from the Repository
 Alternatively, you can clone this repository; `cd` into it; and install from there:
 ```bash
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
 These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64
-$ chmod +x ./tidal-wave_ubuntu_amd64
-$ ./tidal-wave_ubuntu_amd64 --help
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
+$ chmod +x ./tidal-wave_ubuntu_22.04_amd64
+$ ./tidal-wave_ubuntu_22.04_amd64 --help
 ```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
@@ -354,15 +353,15 @@
 │ --help                                                                Show this message and exit.                                                                                                                                 │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Usage
 Invocation of this tool will store credentials in a particular directory in the user's "home" directory: for Unix-like systems, this will be `/home/${USER}/.config/tidal-wave`: for Windows, it varies: in either OS situation, the exact directory is determined by the `user_config_path()` function of the `platformdirs` package.
 
-Similarly, by default, all media retrieved is placed in subdirectories of the user's default music directory: for Unix-like systems, this probably is `/home/${USER}/Music`; for Windows it is probably `C:\Users\<USER>\Music`. This directory is determined by `platformdirs.user_music_path()`. 
+Similarly, by default, all media retrieved is placed in subdirectories of the user's default music directory: for Unix-like systems, this probably is `/home/${USER}/Music`; for Windows it is probably `C:\Users\<USER>\Music`. This directory is determined by [`platformdirs.user_music_path()`](https://github.com/platformdirs/platformdirs?tab=readme-ov-file#platformdirs-to-the-rescue). 
  - If a different path is passed to the second CLI argument, `output_directory`, then all media is written to subdirectories of that directory.
 
 ### Which Audio Formats Are Available to Which Clients
 Source: [TIDAL](https://tidal.com/supported-devices)
 |                | Low                | High               | Lossless           |      MQA           | HiRes FLAC         | Dolby Atmos        | Sony 360 Reality Audio | Video (H.264 + AAC) |
 | :---           | :---:              | :---:              |   :---:            |     :---:          |   :---:            |    :---:           |        :---:           |     :---:           |
 | Android        | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |     :x:            |   :heavy_check_mark:   | :heavy_check_mark: |
@@ -478,19 +477,20 @@
 $ docker run \
     --name tidal-wave \
     -dit \  # is short for: --detach --interactive --tty
     --volume ./Music:/home/debian/Music \
     --volume ./config/tidal-wave:/home/debian/.config/tidal-wave \
     --entrypoint "/bin/bash" \
     ghcr.io/ebb-earl-co/tidal-wave:latest
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/album/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/mix/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/playlist/...
-$ docker exec -it tidal-wave python3 -m tidal_wave https://tidal.com/browse/track/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/album/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/mix/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/playlist/...
+$ docker exec -it tidal-wave tidal-wave https://tidal.com/browse/track/...
 ```
+Note: the first `tidal-wave` is whatever `--name` you give the container, so that can be whatever your heart desires, but the second `tidal-wave` is invoking the Python program *inside* the container and needs to exactly `tidal-wave`.
 ## Development
 The easiest way to start working on development is to fork this project on GitHub, or clone the repository to your local machine and do the pull requesting on GitHub later. In any case, there will need to be some getting from GitHub first, so, roughly, the process is:
   1. Get Python 3.8+ on your system
   2. Use a virtualenv or some other Python environment system (poetry, pipenv, etc.)
   3. Clone the repository: `$ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave/git`
 
     * Obviously replace the URL with your forked version if you've followed that strategy
```

### Comparing `tidal-wave-2024.4.2/tidal_wave.egg-info/SOURCES.txt` & `tidal_wave-2024.4.3/tidal_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

