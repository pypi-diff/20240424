# Comparing `tmp/ixbrl-viewer-1.4.8.tar.gz` & `tmp/ixbrl-viewer-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl-viewer-1.4.8.tar", last modified: Tue Nov 21 20:47:51 2023, max compression
+gzip compressed data, was "ixbrl-viewer-1.4.9.tar", last modified: Tue Nov 28 00:09:11 2023, max compression
```

## Comparing `ixbrl-viewer-1.4.8.tar` & `ixbrl-viewer-1.4.9.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.090076 ixbrl-viewer-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.babelrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.042075 ixbrl-viewer-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.042075 ixbrl-viewer-1.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/ISSUE_TEMPLATE/questions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/ISSUE_TEMPLATE/request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.042075 ixbrl-viewer-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/node-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/npm-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/puppeteer.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2023-11-21 20:47:51.090076 ixbrl-viewer-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.042075 ixbrl-viewer-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.054075 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (127)    92632 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149033 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
--rw-r--r--   0 runner    (1001) docker     (127)  2413470 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
--rw-r--r--   0 runner    (1001) docker     (127)   535018 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1219995 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
--rw-r--r--   0 runner    (1001) docker     (127)   858776 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
--rw-r--r--   0 runner    (1001) docker     (127)    60067 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
--rw-r--r--   0 runner    (1001) docker     (127)    68052 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
--rw-r--r--   0 runner    (1001) docker     (127)  4343804 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.058075 ixbrl-viewer-1.4.8/examples/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   194458 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/example-plugin.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/extended-viewer.js
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    95465 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/example_plugin/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)   917698 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/ixbrl-viewer-demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)    17954 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/review-mode.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.062075 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (127)   222306 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (127)   223016 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (127)    56173 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    24833 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.062075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-21 20:47:50.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/featureConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    28138 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/stubviewer.html
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.062075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.066075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   860807 2023-11-21 20:47:36.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-11-21 20:47:36.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/i18next-parser.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.034075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.066075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/html/fact-details.html
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
--rw-r--r--   0 runner    (1001) docker     (127)    18109 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/html/inspector.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.034075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.066075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/en/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.066075 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/es/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.070076 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/chevron-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/chevron-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/cog.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/dimension-member.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/dimension.svg
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/filter.svg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/graph.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/member.svg
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/outline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/print.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/question.svg
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/search.svg
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/select.svg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/summary.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/tag.svg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/text-block.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/tick.svg
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/warning.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.070076 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/arelle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.078076 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/accordian.js
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/aspect.js
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/calculations.js
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/chart.js
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/chart.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/concept.js
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/concept.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/dialog.js
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
--rw-r--r--   0 runner    (1001) docker     (127)    10103 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/fact.js
--rw-r--r--   0 runner    (1001) docker     (127)    22957 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/fact.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/factset.js
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/factset.test.js
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/footnote.js
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/identifiers.js
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    45281 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/inspector.js
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
--rw-r--r--   0 runner    (1001) docker     (127)    85048 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/interact.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/ixnode.js
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/menu.js
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/messagebox.js
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/outline.js
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/outline.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/period.js
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/period.test.js
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/qname.js
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/report.js
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/report.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/reportset.js
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/reportset.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/search.js
--rw-r--r--   0 runner    (1001) docker     (127)    20925 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/search.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/summary.js
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/summary.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/tableExport.js
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/test-utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/unit.js
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/unit.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/util.test.js
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/validationreport.js
--rw-r--r--   0 runner    (1001) docker     (127)    34884 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/viewer.js
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.082076 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/accordian.less
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/block-list.less
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/chart.less
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/clearfix.less
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/colours.less
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/common.less
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/components.less
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/core.less
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/dialog.less
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/fonts.less
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/form-controls.less
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/icons.less.njk
--rw-r--r--   0 runner    (1001) docker     (127)    20516 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/inspector.less
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/loader.less
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/menu.less
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/summary.less
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/tabs.less
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/validation-report.less
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/viewer.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.082076 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/tools/build-font.js
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/version.js
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/webpack.common.js
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/webpack.dev.js
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/webpack.prod.js
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/iXBRLViewerPlugin/xhtmlserialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.082076 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2023-11-21 20:47:50.000000 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2023-11-21 20:47:51.000000 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 20:47:50.000000 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-21 20:47:50.000000 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-21 20:47:50.000000 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-21 20:47:50.000000 ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   497302 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/Makefile-src
--rwxr-xr-x   0 runner    (1001) docker     (127)     4323 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/build-viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2053 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/fetch-sample-files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/sample-files.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.038075 ixbrl-viewer-1.4.8/samples/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/samples/src/continuation/
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/src/continuation/continuation.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/samples/src/ixds-test/
--rw-r--r--   0 runner    (1001) docker     (127)    26111 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/src/ixds-test/document1.html
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/src/ixds-test/faurecia.html
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/src/ixds-test/valeo.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/samples/src/scrollable-div/
--rw-r--r--   0 runner    (1001) docker     (127)    21858 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/src/scrollable-div/scrollable-div.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/samples/src/xbrl-invalid-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 20:47:51.090076 ixbrl-viewer-1.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/puppeteer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/puppeteer/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/core_elements.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/doc_frame.js
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/fact_details_panel.js
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/search_panel.js
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/toolbar.js
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/framework/viewer_page.js
--rw-r--r--   0 runner    (1001) docker     (127)    61701 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/puppeteer/test_filings/
--rw-r--r--   0 runner    (1001) docker     (127)    21469 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
--rw-r--r--   0 runner    (1001) docker     (127)    18766 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/test_filings/highlights.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/puppeteer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/tests/fact_properties.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/tests/highlight.test.js
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/tests/search.test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.086076 ixbrl-viewer-1.4.8/tests/puppeteer/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      500 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/puppeteer/tools/generate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.090076 ixbrl-viewer-1.4.8/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:51.090076 ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
--rw-r--r--   0 runner    (1001) docker     (127)    31583 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12570 2023-11-21 20:47:13.000000 ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.babelrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.745556 ixbrl-viewer-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.745556 ixbrl-viewer-1.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/ISSUE_TEMPLATE/questions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/ISSUE_TEMPLATE/request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.745556 ixbrl-viewer-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/node-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/npm-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/puppeteer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.749556 ixbrl-viewer-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.757556 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)    92632 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149033 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  2413470 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
+-rw-r--r--   0 runner    (1001) docker     (127)   535018 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1219995 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   858776 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    60067 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
+-rw-r--r--   0 runner    (1001) docker     (127)    68052 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
+-rw-r--r--   0 runner    (1001) docker     (127)  4343804 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.765556 ixbrl-viewer-1.4.9/examples/example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   194458 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/example-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/extended-viewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95465 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/example_plugin/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   917698 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/ixbrl-viewer-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    17954 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/review-mode.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.765556 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)   222306 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (127)   223016 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (127)    56173 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    24833 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.765556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    13974 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/featureConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/stubviewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.765556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.769556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   860807 2023-11-28 00:08:57.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-11-28 00:08:57.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/i18next-parser.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.741556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.769556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/html/fact-details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18109 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/html/inspector.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.737556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.769556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.769556 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.773557 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/chevron-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/chevron-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/cog.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/dimension-member.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/dimension.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/filter.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/graph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/member.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/outline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/print.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/question.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/search.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/select.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/summary.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/text-block.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/tick.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/warning.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.773557 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/arelle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.785557 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/accordian.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/aspect.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/calculations.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/chart.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/concept.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/concept.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/dialog.js
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10103 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/fact.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22957 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/fact.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/factset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/factset.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/identifiers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45281 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/inspector.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)    85048 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/interact.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/ixnode.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/menu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/messagebox.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/outline.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/outline.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/period.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/period.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/qname.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/report.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/report.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/reportset.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/reportset.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20925 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/search.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/summary.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/summary.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/tableExport.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/test-utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/unit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/unit.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/util.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/validationreport.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34884 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/viewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.785557 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/accordian.less
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/block-list.less
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/chart.less
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/clearfix.less
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/colours.less
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/common.less
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/components.less
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/core.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/dialog.less
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/fonts.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/form-controls.less
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/icons.less.njk
+-rw-r--r--   0 runner    (1001) docker     (127)    20516 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/inspector.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/loader.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/menu.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/summary.less
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/tabs.less
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/validation-report.less
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/viewer.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/tools/build-font.js
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/version.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/webpack.common.js
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/webpack.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/webpack.prod.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/iXBRLViewerPlugin/xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-28 00:09:11.000000 ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   497302 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/Makefile-src
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4323 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/build-viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2053 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/fetch-sample-files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/sample-files.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.741556 ixbrl-viewer-1.4.9/samples/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/samples/src/continuation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/src/continuation/continuation.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/samples/src/ixds-test/
+-rw-r--r--   0 runner    (1001) docker     (127)    26111 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/src/ixds-test/document1.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/src/ixds-test/faurecia.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10726 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/src/ixds-test/valeo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/samples/src/scrollable-div/
+-rw-r--r--   0 runner    (1001) docker     (127)    21858 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/src/scrollable-div/scrollable-div.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/samples/src/xbrl-invalid-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/tests/puppeteer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.789557 ixbrl-viewer-1.4.9/tests/puppeteer/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/core_elements.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/doc_frame.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/fact_details_panel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/search_panel.js
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/toolbar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/framework/viewer_page.js
+-rw-r--r--   0 runner    (1001) docker     (127)    61701 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/tests/puppeteer/test_filings/
+-rw-r--r--   0 runner    (1001) docker     (127)    21469 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    18766 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/test_filings/highlights.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/tests/puppeteer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/tests/fact_properties.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/tests/highlight.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/tests/search.test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/tests/puppeteer/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      500 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/puppeteer/tools/generate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 00:09:11.793557 ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31583 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12570 2023-11-28 00:08:29.000000 ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
```

### Comparing `ixbrl-viewer-1.4.8/.github/ISSUE_TEMPLATE/bug.yml` & `ixbrl-viewer-1.4.9/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/.github/dependabot.yml` & `ixbrl-viewer-1.4.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/.github/workflows/node-tests.yml` & `ixbrl-viewer-1.4.9/.github/workflows/node-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/.github/workflows/npm-package.yml` & `ixbrl-viewer-1.4.9/.github/workflows/npm-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/.github/workflows/puppeteer.yml` & `ixbrl-viewer-1.4.9/.github/workflows/puppeteer.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/.github/workflows/python-package.yml` & `ixbrl-viewer-1.4.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/.github/workflows/python-tests.yml` & `ixbrl-viewer-1.4.9/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/ARCHITECTURE.md` & `ixbrl-viewer-1.4.9/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/LICENSE` & `ixbrl-viewer-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/Makefile` & `ixbrl-viewer-1.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/NOTICE` & `ixbrl-viewer-1.4.9/NOTICE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/PKG-INFO` & `ixbrl-viewer-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.4.8
+Version: 1.4.9
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `ixbrl-viewer-1.4.8/PLUGINS.md` & `ixbrl-viewer-1.4.9/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/README.md` & `ixbrl-viewer-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/README.md` & `ixbrl-viewer-1.4.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.4.9/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/example_plugin/README.md` & `ixbrl-viewer-1.4.9/examples/example_plugin/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/example_plugin/example-plugin.gif` & `ixbrl-viewer-1.4.9/examples/example_plugin/example-plugin.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/example_plugin/extended-viewer.js` & `ixbrl-viewer-1.4.9/examples/example_plugin/extended-viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/example_plugin/package-lock.json` & `ixbrl-viewer-1.4.9/examples/example_plugin/package-lock.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/example_plugin/webpack.config.js` & `ixbrl-viewer-1.4.9/examples/example_plugin/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/ixbrl-viewer-demo.gif` & `ixbrl-viewer-1.4.9/examples/ixbrl-viewer-demo.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/review-mode.png` & `ixbrl-viewer-1.4.9/examples/review-mode.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm` & `ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm` & `ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd` & `ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml` & `ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml` & `ixbrl-viewer-1.4.9/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/__init__.py` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,17 @@
 
 def load_plugin_url():
     return __file__
 
 
 __pluginInfo__ = {
     'name': 'ixbrl-viewer',
+    'aliases': [
+        'iXBRLViewerPlugin',
+    ],
     'version': '0.1',
     'description': "iXBRL Viewer creator",
     'license': 'License :: OSI Approved :: Apache License, Version 2.0 (Apache-2.0)',
     'author': 'Paul Warren',
     'copyright': 'Copyright :: Workiva Inc. :: 2019',
     'CntlrCmdLine.Options': commandLineOptionExtender,
     'CntlrCmdLine.Filing.End': commandLineRun,
```

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/constants.py` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/constants.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/iXBRLViewer.py` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/iXBRLViewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/ui.py` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/ui.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -27641,15 +27641,15 @@
                 return "false" === (new URLSearchParams(window.location.search).get("disable-viewer") ?? "false")
             }
             _loadInspectorHTML() {
                 t()(n(845)).prependTo("body");
                 const e = n(610).toString();
                 t()('<style id="ixv-style"></style>').prop("type", "text/css").text(e).appendTo("head"), t()('<link id="ixv-favicon" type="image/x-icon" rel="shortcut icon" />').attr("href", n(688)).appendTo("head");
                 try {
-                    t()(".inspector-foot .version").text("1.4.8")
+                    t()(".inspector-foot .version").text("1.4.9")
                 } catch (e) {}
             }
             _reparentDocument() {
                 const e = t()("#ixv #iframe-container"),
                     n = t()('<iframe title="iXBRL document view"/>').data("report-index", 0).appendTo(e)[0],
                     i = n.contentDocument || n.contentWindow.document;
                 i.open(), i.write("<!DOCTYPE html><html><head><title></title></head><body></body></html>"), i.close();
```

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/html/fact-details.html` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/html/fact-details.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/html/inspector.html` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/html/inspector.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/clipboard.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/clipboard.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/close.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/close.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/cog.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/cog.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/dimension-member.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/dimension-member.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/dimension.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/dimension.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/download.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/download.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/member.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/member.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/outline.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/outline.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/print.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/print.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/question.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/question.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/search.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/search.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/select.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/select.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/summary.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/summary.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/tag.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/tag.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/text-block.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/text-block.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/icons/warning.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/arelle.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/arelle.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/favicon.ico` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/accordian.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/accordian.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/aspect.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/aspect.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/aspect.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/aspect.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/calculations.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/calculations.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/chart.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/chart.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/chart.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/chart.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/concept.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/concept.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/concept.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/concept.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/dialog.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/dialog.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/fact.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/fact.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/fact.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/fact.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/factset.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/factset.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/factset.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/factset.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/footnote.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/footnote.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/identifiers.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/identifiers.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/inspector.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/inspector.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/inspector.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/inspector.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/interact.min.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/interact.min.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/ixnode.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/ixnode.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/menu.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/menu.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/messagebox.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/messagebox.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/moment-jest.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/moment-jest.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/number-matcher.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/number-matcher.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/outline.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/outline.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/outline.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/outline.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/period.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/period.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/period.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/period.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/report.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/report.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/report.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/report.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/reportset.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/reportset.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/reportset.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/reportset.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/search.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/search.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/search.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/summary.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/summary.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/summary.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/summary.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/tableExport.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/tableExport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/test-utils.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/test-utils.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/unit.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/unit.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/unit.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/unit.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/util.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/util.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/util.test.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/util.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/validationreport.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/validationreport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/js/viewer.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/js/viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/accordian.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/accordian.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/chart.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/chart.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/colours.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/colours.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/dialog.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/dialog.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/form-controls.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/form-controls.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/inspector.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/inspector.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/loader.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/loader.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/menu.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/menu.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/summary.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/summary.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/tabs.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/tabs.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/src/less/viewer.less` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/src/less/viewer.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/tools/build-font.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/tools/build-font.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/webpack.common.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/webpack.common.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/viewer/webpack.dev.js` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/viewer/webpack.dev.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/iXBRLViewerPlugin/xhtmlserialize.py` & `ixbrl-viewer-1.4.9/iXBRLViewerPlugin/xhtmlserialize.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/PKG-INFO` & `ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.4.8
+Version: 1.4.9
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `ixbrl-viewer-1.4.8/ixbrl_viewer.egg-info/SOURCES.txt` & `ixbrl-viewer-1.4.9/ixbrl_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/package-lock.json` & `ixbrl-viewer-1.4.9/package-lock.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/package.json` & `ixbrl-viewer-1.4.9/package.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/pyproject.toml` & `ixbrl-viewer-1.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/Makefile` & `ixbrl-viewer-1.4.9/samples/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/Makefile-src` & `ixbrl-viewer-1.4.9/samples/Makefile-src`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/build-viewer.py` & `ixbrl-viewer-1.4.9/samples/build-viewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/fetch-sample-files.py` & `ixbrl-viewer-1.4.9/samples/fetch-sample-files.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/sample-files.list` & `ixbrl-viewer-1.4.9/samples/sample-files.list`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/src/continuation/continuation.html` & `ixbrl-viewer-1.4.9/samples/src/continuation/continuation.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/src/ixds-test/document1.html` & `ixbrl-viewer-1.4.9/samples/src/ixds-test/document1.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/src/ixds-test/faurecia.html` & `ixbrl-viewer-1.4.9/samples/src/ixds-test/faurecia.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/src/ixds-test/valeo.html` & `ixbrl-viewer-1.4.9/samples/src/ixds-test/valeo.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/src/scrollable-div/scrollable-div.html` & `ixbrl-viewer-1.4.9/samples/src/scrollable-div/scrollable-div.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html` & `ixbrl-viewer-1.4.9/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/framework/core_elements.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/framework/core_elements.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/doc_frame.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/doc_frame.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/fact_details_panel.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/fact_details_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/search_panel.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/search_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/framework/page_objects/toolbar.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/framework/page_objects/toolbar.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/framework/viewer_page.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/framework/viewer_page.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/puppeteer_test_run_via_intellij.jpg` & `ixbrl-viewer-1.4.9/tests/puppeteer/puppeteer_test_run_via_intellij.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/test_filings/filing_documents_smoke_test.zip` & `ixbrl-viewer-1.4.9/tests/puppeteer/test_filings/filing_documents_smoke_test.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/test_filings/highlights.zip` & `ixbrl-viewer-1.4.9/tests/puppeteer/test_filings/highlights.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/tests/fact_properties.test.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/tests/fact_properties.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/tests/highlight.test.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/tests/highlight.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/puppeteer/tests/search.test.js` & `ixbrl-viewer-1.4.9/tests/puppeteer/tests/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py` & `ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py` & `ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.4.8/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py` & `ixbrl-viewer-1.4.9/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py`

 * *Files identical despite different names*

