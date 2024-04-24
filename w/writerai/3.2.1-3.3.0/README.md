# Comparing `tmp/writerai-3.2.1.tar.gz` & `tmp/writerai-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "writerai-3.2.1.tar", last modified: Tue Mar 26 14:30:33 2024, max compression
+gzip compressed data, was "writerai-3.3.0.tar", last modified: Wed Apr 24 15:16:25 2024, max compression
```

## Comparing `writerai-3.2.1.tar` & `writerai-3.3.0.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.652947 writerai-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    13742 2024-03-26 14:30:33.652947 writerai-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10943 2024-03-26 14:30:25.000000 writerai-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 14:30:33.652947 writerai-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-26 14:30:25.000000 writerai-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.632947 writerai-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.636947 writerai-3.2.1/src/writer/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.636947 writerai-3.2.1/src/writer/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/ai_content_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/cowrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/document_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/download_the_customized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/modelcustomization_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.648947 writerai-3.2.1/src/writer/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/addtermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/approvedtermextension.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/approvedtermextensioncreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/briefdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/briefdocuments.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/completiongenerationchoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/completiongenerationchoicelogprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/completionrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/completionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentcheckop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentcorrectop.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentdetectorrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentdetectorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentissue.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/contentsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/correctionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/createcompletionop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/createcustomizationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/createmodelcustomizationcompletionop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/createmodelcustomizationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/createtermsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/createtermsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/customizationsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/deletefileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/deletemodelcustomizationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/deleteresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/deletesnippetsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/deletetermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/detectcontentop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/draft.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/failmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/failresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/fetchcustomizedmodelfileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/findsnippetsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/findtermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/fulllinkedterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/fulltermwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/generate_contentop.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/generatetemplaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/generationmodelinforesponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/generationmodelsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/getdocumentdetailsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/getfileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/getmodelcustomizationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/getsubscriptiondetailsop.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/linkedtermcreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listfilesop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listmodelcustomizationsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listmodelsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listpagesop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listteamdocumentsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listtemplatesop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/listusersop.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/magicrequestinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/modelcustomization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/modelfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/modelfilesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/pagedetailsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/pagepublicapiresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/pagewithsectionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/paginatedresult_fulltermwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/paginatedresult_pagepublicapiresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/paginatedresult_snippetwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/paginatedresult_userpublicresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/processedcontent.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/sectioninfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/simpleuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/snippettagv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/snippetupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/snippetwithuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/subscriptionpublicresponseapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/templatedetailsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termcreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termexample.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termexamplecreate.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/terminologyuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termmistake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termmistakecreate.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termtagcreate.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termtagresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/termupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/updatesnippetsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/updatetermsop.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/updatetermsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/uploadfileop.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/uploadmodelfilerequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/usageitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models/userpublicresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/models_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/snippet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/styleguide.py
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/terminology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.648947 writerai-3.2.1/src/writer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29893 2024-03-26 14:30:25.000000 writerai-3.2.1/src/writer/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:30:33.652947 writerai-3.2.1/src/writerai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13742 2024-03-26 14:30:33.000000 writerai-3.2.1/src/writerai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-26 14:30:33.000000 writerai-3.2.1/src/writerai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:30:33.000000 writerai-3.2.1/src/writerai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-26 14:30:33.000000 writerai-3.2.1/src/writerai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 14:30:33.000000 writerai-3.2.1/src/writerai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-24 15:16:25.905017 writerai-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-04-24 15:16:16.000000 writerai-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:16:25.905017 writerai-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 15:16:16.000000 writerai-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.885016 writerai-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.889016 writerai-3.3.0/src/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.889016 writerai-3.3.0/src/writer/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/ai_content_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/cowrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/document_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/download_the_customized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17790 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/modelcustomization_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/addtermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/approvedtermextension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/approvedtermextensioncreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/briefdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/briefdocuments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completiongenerationchoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completiongenerationchoicelogprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completionrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/completionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentcheckop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentcorrectop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentdetectorrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentdetectorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentissue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/contentsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/correctionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createcompletionop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createcustomizationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createmodelcustomizationcompletionop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createmodelcustomizationop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createtermsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/createtermsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/customizationsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletefileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletemodelcustomizationop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deleteresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletesnippetsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/deletetermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/detectcontentop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/draft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/failmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/failresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/fetchcustomizedmodelfileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/findsnippetsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/findtermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/fulllinkedterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/fulltermwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generate_contentop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generatetemplaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generationmodelinforesponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/generationmodelsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getdocumentdetailsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getfileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getmodelcustomizationop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/getsubscriptiondetailsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writer/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/internal/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/linkedtermcreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listfilesop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listmodelcustomizationsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listmodelsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listpagesop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listteamdocumentsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listtemplatesop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/listusersop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/magicrequestinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/modelcustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/modelfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/modelfilesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagedetailsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagepublicapiresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagewithsectionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_fulltermwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_pagepublicapiresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_snippetwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/paginatedresult_userpublicresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/processedcontent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/sectioninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/simpleuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/snippettagv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/snippetupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/snippetwithuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/subscriptionpublicresponseapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/templatedetailsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termcreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termexample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termexamplecreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/terminologyuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termmistake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termmistakecreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termtagcreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termtagresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/termupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/updatesnippetsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/updatetermsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/updatetermsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/uploadfileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/uploadmodelfilerequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/usageitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models/userpublicresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/models_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/styleguide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/terminology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32082 2024-04-24 15:16:16.000000 writerai-3.3.0/src/writer/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:16:25.905017 writerai-3.3.0/src/writerai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 15:16:25.000000 writerai-3.3.0/src/writerai.egg-info/top_level.txt
```

### Comparing `writerai-3.2.1/PKG-INFO` & `writerai-3.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,330 +1,318 @@
-Metadata-Version: 2.1
-Name: writerai
-Version: 3.2.1
-Summary: Python SDK for Writer API
-Home-page: UNKNOWN
-Author: writerai
-License: UNKNOWN
-Description: <div align="center">
-                <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
-                <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
-            <h1>Python SDK</h1>
-           <p>AI for everyone.</p>
-           <a href="https://dev.writer.com/docs"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
-          <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
-          <a href="https://github.com/writerai/writer-client-sdk-python/releases"><img src="https://img.shields.io/github/v/release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge" /></a>
-          <a href="https://codespaces.new/writerai/writer-client-sdk-python.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
-        </div>
-        
-        <!-- Start SDK Installation [installation] -->
-        ## SDK Installation
-        
-        ```bash
-        pip install writerai
-        ```
-        <!-- End SDK Installation [installation] -->
-        
-        ## Authentication
-        
-        Writer authenticates your API requests using your account’s API keys. If you do not include your key when making an API request, or use one that is incorrect or outdated, Writer returns an error.
-        
-        Your API keys are available in the account dashboard. We include randomly generated API keys in our code examples if you are not logged in. Replace these with your own or log in to see code examples populated with your own API keys.
-        
-        <img width="1070" alt="writer-auth" src="https://user-images.githubusercontent.com/6267663/223578295-89087c24-c55a-48bf-b74a-5f057e21e14f.png">
-        
-        If you cannot see your secret API keys in the Dashboard, this means you do not have access to them. Contact your Writer account owner and ask to be added to their team as a developer.
-        
-        <!-- Start SDK Example Usage [usage] -->
-        ## SDK Example Usage
-        
-        ### Example
-        
-        ```python
-        import writer
-        
-        s = writer.Writer(
-            api_key="<YOUR_API_KEY_HERE>",
-            organization_id=850421,
-        )
-        
-        
-        res = s.billing.get_subscription_details()
-        
-        if res.subscription_public_response_api is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End SDK Example Usage [usage] -->
-        
-        <!-- Start Available Resources and Operations [operations] -->
-        ## Available Resources and Operations
-        
-        ### [billing](docs/sdks/billing/README.md)
-        
-        * [get_subscription_details](docs/sdks/billing/README.md#get_subscription_details) - Get your organization subscription details
-        
-        ### [ai_content_detector](docs/sdks/aicontentdetector/README.md)
-        
-        * [detect](docs/sdks/aicontentdetector/README.md#detect) - Content detector api
-        
-        ### [content](docs/sdks/content/README.md)
-        
-        * [check](docs/sdks/content/README.md#check) - Check your content against your preset styleguide.
-        * [correct](docs/sdks/content/README.md#correct) - Apply the style guide suggestions directly to your content.
-        
-        ### [co_write](docs/sdks/cowrite/README.md)
-        
-        * [generate_content](docs/sdks/cowrite/README.md#generate_content) - Generate content using predefined templates
-        * [list_templates](docs/sdks/cowrite/README.md#list_templates) - Get a list of your existing CoWrite templates
-        
-        ### [files](docs/sdks/files/README.md)
-        
-        * [delete](docs/sdks/files/README.md#delete) - Delete file
-        * [get](docs/sdks/files/README.md#get) - Get file
-        * [list](docs/sdks/files/README.md#list) - List files
-        * [upload](docs/sdks/files/README.md#upload) - Upload file
-        
-        ### [models](docs/sdks/models/README.md)
-        
-        * [list](docs/sdks/models/README.md#list) - List available LLM models
-        
-        ### [completions](docs/sdks/completions/README.md)
-        
-        * [create](docs/sdks/completions/README.md#create) - Create completion for LLM model
-        * [create_model_customization_completion](docs/sdks/completions/README.md#create_model_customization_completion) - Create completion for LLM customization model
-        
-        ### [model_customization](docs/sdks/modelcustomizationsdk/README.md)
-        
-        * [create](docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
-        * [delete](docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
-        * [get](docs/sdks/modelcustomizationsdk/README.md#get) - Get model customization
-        * [list](docs/sdks/modelcustomizationsdk/README.md#list) - List model customizations
-        
-        ### [download_the_customized_model](docs/sdks/downloadthecustomizedmodel/README.md)
-        
-        * [fetch_file](docs/sdks/downloadthecustomizedmodel/README.md#fetch_file) - Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)
-        
-        ### [document](docs/sdks/documentsdk/README.md)
-        
-        * [get](docs/sdks/documentsdk/README.md#get) - Get document details
-        * [list](docs/sdks/documentsdk/README.md#list) - List team documents
-        
-        ### [snippet](docs/sdks/snippet/README.md)
-        
-        * [delete](docs/sdks/snippet/README.md#delete) - Delete snippets
-        * [find](docs/sdks/snippet/README.md#find) - Find snippets
-        * [update](docs/sdks/snippet/README.md#update) - Update snippets
-        
-        ### [styleguide](docs/sdks/styleguide/README.md)
-        
-        * [get](docs/sdks/styleguide/README.md#get) - Page details
-        * [list_pages](docs/sdks/styleguide/README.md#list_pages) - List your styleguide pages
-        
-        ### [terminology](docs/sdks/terminology/README.md)
-        
-        * [add](docs/sdks/terminology/README.md#add) - Add terms
-        * [delete](docs/sdks/terminology/README.md#delete) - Delete terms
-        * [find](docs/sdks/terminology/README.md#find) - Find terms
-        * [update](docs/sdks/terminology/README.md#update) - Update terms
-        
-        ### [user](docs/sdks/user/README.md)
-        
-        * [list](docs/sdks/user/README.md#list) - List users
-        <!-- End Available Resources and Operations [operations] -->
-        
-        
-        <!-- Start Global Parameters [global-parameters] -->
-        ## Global Parameters
-        
-        A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
-        
-        For example, you can set `organizationId` to `99895` at SDK initialization and then you do not have to pass the same value on calls to operations like `detect`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
-        
-        
-        ### Available Globals
-        
-        The following global parameter is available. The required parameter must be set when you initialize the SDK client.
-        
-        | Name | Type | Required | Description |
-        | ---- | ---- |:--------:| ----------- |
-        | organization_id | int | ✔️ | The organization_id parameter. |
-        
-        
-        ### Example
-        
-        ```python
-        import writer
-        
-        s = writer.Writer(
-            api_key="<YOUR_API_KEY_HERE>",
-            organization_id=496531,
-        )
-        
-        
-        res = s.ai_content_detector.detect(content_detector_request=writer.ContentDetectorRequest(
-            input='<value>',
-        ), organization_id=592237)
-        
-        if res.classes is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Global Parameters [global-parameters] -->
-        
-        
-        
-        <!-- Start Error Handling [errors] -->
-        ## Error Handling
-        
-        Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
-        
-        | Error Object        | Status Code         | Content Type        |
-        | ------------------- | ------------------- | ------------------- |
-        | models.FailResponse | 400,401,403,404,500 | application/json    |
-        | models.SDKError     | 4x-5xx              | */*                 |
-        
-        ### Example
-        
-        ```python
-        import writer
-        from writer import models
-        
-        s = writer.Writer(
-            api_key="<YOUR_API_KEY_HERE>",
-            organization_id=850421,
-        )
-        
-        
-        res = None
-        try:
-            res = s.billing.get_subscription_details()
-        except models.FailResponse as e:
-            # handle exception
-            raise(e)
-        except models.SDKError as e:
-            # handle exception
-            raise(e)
-        
-        if res.subscription_public_response_api is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Error Handling [errors] -->
-        
-        
-        
-        <!-- Start Server Selection [server] -->
-        ## Server Selection
-        
-        ### Select Server by Index
-        
-        You can override the default server globally by passing a server index to the `server_idx: int` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:
-        
-        | # | Server | Variables |
-        | - | ------ | --------- |
-        | 0 | `https://enterprise-api.writer.com` | None |
-        
-        #### Example
-        
-        ```python
-        import writer
-        
-        s = writer.Writer(
-            server_idx=0,
-            api_key="<YOUR_API_KEY_HERE>",
-            organization_id=850421,
-        )
-        
-        
-        res = s.billing.get_subscription_details()
-        
-        if res.subscription_public_response_api is not None:
-            # handle response
-            pass
-        
-        ```
-        
-        
-        ### Override Server URL Per-Client
-        
-        The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
-        ```python
-        import writer
-        
-        s = writer.Writer(
-            server_url="https://enterprise-api.writer.com",
-            api_key="<YOUR_API_KEY_HERE>",
-            organization_id=850421,
-        )
-        
-        
-        res = s.billing.get_subscription_details()
-        
-        if res.subscription_public_response_api is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Server Selection [server] -->
-        
-        
-        
-        <!-- Start Custom HTTP Client [http-client] -->
-        ## Custom HTTP Client
-        
-        The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
-        
-        For example, you could specify a header for every request that this sdk makes as follows:
-        ```python
-        import writer
-        import requests
-        
-        http_client = requests.Session()
-        http_client.headers.update({'x-custom-header': 'someValue'})
-        s = writer.Writer(client: http_client)
-        ```
-        <!-- End Custom HTTP Client [http-client] -->
-        
-        
-        
-        <!-- Start Authentication [security] -->
-        ## Authentication
-        
-        ### Per-Client Security Schemes
-        
-        This SDK supports the following security scheme globally:
-        
-        | Name      | Type      | Scheme    |
-        | --------- | --------- | --------- |
-        | `api_key` | apiKey    | API key   |
-        
-        To authenticate with the API the `api_key` parameter must be set when initializing the SDK client instance. For example:
-        ```python
-        import writer
-        
-        s = writer.Writer(
-            api_key="<YOUR_API_KEY_HERE>",
-            organization_id=850421,
-        )
-        
-        
-        res = s.billing.get_subscription_details()
-        
-        if res.subscription_public_response_api is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Authentication [security] -->
-        
-        <!-- Placeholder for Future Speakeasy SDK Sections -->
-        
-        ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-        
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+<div align="center">
+        <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
+        <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
+    <h1>Python SDK</h1>
+   <p>AI for everyone.</p>
+   <a href="https://dev.writer.com/docs"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
+  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
+  <a href="https://github.com/writerai/writer-client-sdk-python/releases"><img src="https://img.shields.io/github/v/release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge" /></a>
+  <a href="https://codespaces.new/writerai/writer-client-sdk-python.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
+</div>
+
+<!-- Start SDK Installation [installation] -->
+## SDK Installation
+
+```bash
+pip install writerai
+```
+<!-- End SDK Installation [installation] -->
+
+## Authentication
+
+Writer authenticates your API requests using your account’s API keys. If you do not include your key when making an API request, or use one that is incorrect or outdated, Writer returns an error.
+
+Your API keys are available in the account dashboard. We include randomly generated API keys in our code examples if you are not logged in. Replace these with your own or log in to see code examples populated with your own API keys.
+
+<img width="1070" alt="writer-auth" src="https://user-images.githubusercontent.com/6267663/223578295-89087c24-c55a-48bf-b74a-5f057e21e14f.png">
+
+If you cannot see your secret API keys in the Dashboard, this means you do not have access to them. Contact your Writer account owner and ask to be added to their team as a developer.
+
+<!-- Start SDK Example Usage [usage] -->
+## SDK Example Usage
+
+### Example
+
+```python
+import writer
+
+s = writer.Writer(
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=850421,
+)
+
+
+res = s.billing.get_subscription_details()
+
+if res.subscription_public_response_api is not None:
+    # handle response
+    pass
+
+```
+<!-- End SDK Example Usage [usage] -->
+
+<!-- Start Available Resources and Operations [operations] -->
+## Available Resources and Operations
+
+### [billing](docs/sdks/billing/README.md)
+
+* [get_subscription_details](docs/sdks/billing/README.md#get_subscription_details) - Get your organization subscription details
+
+### [ai_content_detector](docs/sdks/aicontentdetector/README.md)
+
+* [detect](docs/sdks/aicontentdetector/README.md#detect) - Content detector api
+
+### [content](docs/sdks/content/README.md)
+
+* [check](docs/sdks/content/README.md#check) - Check your content against your preset styleguide.
+* [correct](docs/sdks/content/README.md#correct) - Apply the style guide suggestions directly to your content.
+
+### [co_write](docs/sdks/cowrite/README.md)
+
+* [generate_content](docs/sdks/cowrite/README.md#generate_content) - Generate content using predefined templates
+* [list_templates](docs/sdks/cowrite/README.md#list_templates) - Get a list of your existing CoWrite templates
+
+### [files](docs/sdks/files/README.md)
+
+* [delete](docs/sdks/files/README.md#delete) - Delete file
+* [get](docs/sdks/files/README.md#get) - Get file
+* [list](docs/sdks/files/README.md#list) - List files
+* [upload](docs/sdks/files/README.md#upload) - Upload file
+
+### [models](docs/sdks/models/README.md)
+
+* [list](docs/sdks/models/README.md#list) - List available LLM models
+
+### [completions](docs/sdks/completions/README.md)
+
+* [create](docs/sdks/completions/README.md#create) - Create completion for LLM model
+* [create_model_customization_completion](docs/sdks/completions/README.md#create_model_customization_completion) - Create completion for LLM customization model
+
+### [model_customization](docs/sdks/modelcustomizationsdk/README.md)
+
+* [create](docs/sdks/modelcustomizationsdk/README.md#create) - Create model customization
+* [delete](docs/sdks/modelcustomizationsdk/README.md#delete) - Delete Model customization
+* [get](docs/sdks/modelcustomizationsdk/README.md#get) - Get model customization
+* [list](docs/sdks/modelcustomizationsdk/README.md#list) - List model customizations
+
+### [download_the_customized_model](docs/sdks/downloadthecustomizedmodel/README.md)
+
+* [fetch_file](docs/sdks/downloadthecustomizedmodel/README.md#fetch_file) - Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)
+
+### [document](docs/sdks/documentsdk/README.md)
+
+* [get](docs/sdks/documentsdk/README.md#get) - Get document details
+* [list](docs/sdks/documentsdk/README.md#list) - List team documents
+
+### [snippet](docs/sdks/snippet/README.md)
+
+* [delete](docs/sdks/snippet/README.md#delete) - Delete snippets
+* [find](docs/sdks/snippet/README.md#find) - Find snippets
+* [update](docs/sdks/snippet/README.md#update) - Update snippets
+
+### [styleguide](docs/sdks/styleguide/README.md)
+
+* [get](docs/sdks/styleguide/README.md#get) - Page details
+* [list_pages](docs/sdks/styleguide/README.md#list_pages) - List your styleguide pages
+
+### [terminology](docs/sdks/terminology/README.md)
+
+* [add](docs/sdks/terminology/README.md#add) - Add terms
+* [delete](docs/sdks/terminology/README.md#delete) - Delete terms
+* [find](docs/sdks/terminology/README.md#find) - Find terms
+* [update](docs/sdks/terminology/README.md#update) - Update terms
+
+### [user](docs/sdks/user/README.md)
+
+* [list](docs/sdks/user/README.md#list) - List users
+<!-- End Available Resources and Operations [operations] -->
+
+
+<!-- Start Global Parameters [global-parameters] -->
+## Global Parameters
+
+A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
+
+For example, you can set `organizationId` to `99895` at SDK initialization and then you do not have to pass the same value on calls to operations like `detect`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+
+
+### Available Globals
+
+The following global parameter is available. The required parameter must be set when you initialize the SDK client.
+
+| Name | Type | Required | Description |
+| ---- | ---- |:--------:| ----------- |
+| organization_id | int | ✔️ | The organization_id parameter. |
+
+
+### Example
+
+```python
+import writer
+
+s = writer.Writer(
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=496531,
+)
+
+
+res = s.ai_content_detector.detect(content_detector_request=writer.ContentDetectorRequest(
+    input='<value>',
+), organization_id=592237)
+
+if res.classes is not None:
+    # handle response
+    pass
+
+```
+<!-- End Global Parameters [global-parameters] -->
+
+
+
+<!-- Start Error Handling [errors] -->
+## Error Handling
+
+Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
+
+| Error Object        | Status Code         | Content Type        |
+| ------------------- | ------------------- | ------------------- |
+| models.FailResponse | 400,401,403,404,500 | application/json    |
+| models.SDKError     | 4xx-5xx             | */*                 |
+
+### Example
+
+```python
+import writer
+from writer import models
+
+s = writer.Writer(
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=850421,
+)
+
+
+res = None
+try:
+    res = s.billing.get_subscription_details()
+except models.FailResponse as e:
+    # handle exception
+    raise(e)
+except models.SDKError as e:
+    # handle exception
+    raise(e)
+
+if res.subscription_public_response_api is not None:
+    # handle response
+    pass
+
+```
+<!-- End Error Handling [errors] -->
+
+
+
+<!-- Start Server Selection [server] -->
+## Server Selection
+
+### Select Server by Index
+
+You can override the default server globally by passing a server index to the `server_idx: int` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:
+
+| # | Server | Variables |
+| - | ------ | --------- |
+| 0 | `https://enterprise-api.writer.com` | None |
+
+#### Example
+
+```python
+import writer
+
+s = writer.Writer(
+    server_idx=0,
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=850421,
+)
+
+
+res = s.billing.get_subscription_details()
+
+if res.subscription_public_response_api is not None:
+    # handle response
+    pass
+
+```
+
+
+### Override Server URL Per-Client
+
+The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
+```python
+import writer
+
+s = writer.Writer(
+    server_url="https://enterprise-api.writer.com",
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=850421,
+)
+
+
+res = s.billing.get_subscription_details()
+
+if res.subscription_public_response_api is not None:
+    # handle response
+    pass
+
+```
+<!-- End Server Selection [server] -->
+
+
+
+<!-- Start Custom HTTP Client [http-client] -->
+## Custom HTTP Client
+
+The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
+
+For example, you could specify a header for every request that this sdk makes as follows:
+```python
+import writer
+import requests
+
+http_client = requests.Session()
+http_client.headers.update({'x-custom-header': 'someValue'})
+s = writer.Writer(client=http_client)
+```
+<!-- End Custom HTTP Client [http-client] -->
+
+
+
+<!-- Start Authentication [security] -->
+## Authentication
+
+### Per-Client Security Schemes
+
+This SDK supports the following security scheme globally:
+
+| Name      | Type      | Scheme    |
+| --------- | --------- | --------- |
+| `api_key` | apiKey    | API key   |
+
+To authenticate with the API the `api_key` parameter must be set when initializing the SDK client instance. For example:
+```python
+import writer
+
+s = writer.Writer(
+    api_key="<YOUR_API_KEY_HERE>",
+    organization_id=850421,
+)
+
+
+res = s.billing.get_subscription_details()
+
+if res.subscription_public_response_api is not None:
+    # handle response
+    pass
+
+```
+<!-- End Authentication [security] -->
+
+<!-- Placeholder for Future Speakeasy SDK Sections -->
+
+### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

#### html2text {}

```diff
@@ -1,9 +1,7 @@
-Metadata-Version: 2.1 Name: writerai Version: 3.2.1 Summary: Python SDK for
-Writer API Home-page: UNKNOWN Author: writerai License: UNKNOWN Description:
   [https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-
                           44e8-ac48-f9494101e1dc.svg]
                            ************ PPyytthhoonn SSDDKK ************
                                AI for everyone.
            _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_D_o_c_s_&_m_e_s_s_a_g_e_=_A_P_I
 _R_e_f_&_c_o_l_o_r_=_0_0_0_0_0_0_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-
 _b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_w_r_i_t_e_r_a_i_/
@@ -83,15 +81,15 @@
 organization_id=592237) if res.classes is not None: # handle response pass ```
 ## Error Handling Handling errors in this SDK should largely match your
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 ------------ | ------------------- | ------------------- | |
 models.FailResponse | 400,401,403,404,500 | application/json | |
-models.SDKError | 4x-5xx | */* | ### Example ```python import writer from
+models.SDKError | 4xx-5xx | */* | ### Example ```python import writer from
 writer import models s = writer.Writer( api_key="", organization_id=850421, )
 res = None try: res = s.billing.get_subscription_details() except
 models.FailResponse as e: # handle exception raise(e) except models.SDKError as
 e: # handle exception raise(e) if res.subscription_public_response_api is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
@@ -111,18 +109,16 @@
 API calls using the [requests](https://pypi.org/project/requests/) HTTP
 library. In order to provide a convenient way to configure timeouts, cookies,
 proxies, custom headers, and other low-level configuration, you can initialize
 the SDK client with a custom `requests.Session` object. For example, you could
 specify a header for every request that this sdk makes as follows: ```python
 import writer import requests http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'}) s = writer.Writer
-(client: http_client) ``` ## Authentication ### Per-Client Security Schemes
-This SDK supports the following security scheme globally: | Name | Type |
-Scheme | | --------- | --------- | --------- | | `api_key` | apiKey | API key |
-To authenticate with the API the `api_key` parameter must be set when
-initializing the SDK client instance. For example: ```python import writer s =
-writer.Writer( api_key="", organization_id=850421, ) res =
+(client=http_client) ``` ## Authentication ### Per-Client Security Schemes This
+SDK supports the following security scheme globally: | Name | Type | Scheme | |
+--------- | --------- | --------- | | `api_key` | apiKey | API key | To
+authenticate with the API the `api_key` parameter must be set when initializing
+the SDK client instance. For example: ```python import writer s = writer.Writer
+( api_key="", organization_id=850421, ) res =
 s.billing.get_subscription_details() if res.subscription_public_response_api is
 not None: # handle response pass ``` ### SDK Generated by [Speakeasy](https://
-docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks) Platform: UNKNOWN
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev
+docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `writerai-3.2.1/src/writer/_hooks/sdkhooks.py` & `writerai-3.3.0/src/writer/_hooks/sdkhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -25,27 +25,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `writerai-3.2.1/src/writer/_hooks/types.py` & `writerai-3.3.0/src/writer/_hooks/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
 
@@ -38,21 +42,21 @@
     @abstractmethod
     def before_request(self, hook_ctx: BeforeRequestContext, request: requests_http.PreparedRequest) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterSuccessHook(ABC):
     @abstractmethod
-    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.PreparedRequest, Exception]:
+    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.Response, Exception]:
         pass
 
 
 class AfterErrorHook(ABC):
     @abstractmethod
-    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.PreparedRequest], Optional[Exception]], Exception]:
+    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.Response], Optional[Exception]], Exception]:
         pass
 
 
 class Hooks(ABC):
     @abstractmethod
     def register_sdk_init_hook(self, hook: SDKInitHook):
         pass
```

### Comparing `writerai-3.2.1/src/writer/billing.py` & `writerai-3.3.0/src/writer/billing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
 class Billing:
     r"""Methods related to Billing"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -28,55 +28,55 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.GetSubscriptionDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.GetSubscriptionDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.SubscriptionPublicResponseAPI])
                 res.subscription_public_response_api = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/completions.py` & `writerai-3.3.0/src/writer/completions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
 class Completions:
     r"""Methods related to Completions"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -20,68 +20,73 @@
         hook_ctx = HookContext(operation_id='createCompletion', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = models.CreateCompletionRequest(
             completion_request=completion_request,
             model_id=model_id,
             organization_id=organization_id,
         )
         
+        _globals = models.CreateCompletionGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.CreateCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/completions', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/completions', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, models.CreateCompletionRequest, "completion_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.CreateCompletionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.CreateCompletionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.CompletionResponse])
                 res.completion_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -98,74 +103,80 @@
         request = models.CreateModelCustomizationCompletionRequest(
             completion_request=completion_request,
             customization_id=customization_id,
             model_id=model_id,
             organization_id=organization_id,
         )
         
+        _globals = models.CreateModelCustomizationCompletionGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.CreateModelCustomizationCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/completions', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/completions', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, models.CreateModelCustomizationCompletionRequest, "completion_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.CreateModelCustomizationCompletionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.CreateModelCustomizationCompletionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.CompletionResponse])
                 res.completion_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/content.py` & `writerai-3.3.0/src/writer/document_sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,172 +1,165 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Content:
-    r"""Methods related to Content"""
+class DocumentSDK:
+    r"""Methods related to document"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def check(self, content_request: models.ContentRequest, team_id: int, organization_id: Optional[int] = None) -> models.ContentCheckResponse:
-        r"""Check your content against your preset styleguide."""
-        hook_ctx = HookContext(operation_id='contentCheck', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ContentCheckRequest(
-            content_request=content_request,
+    def get(self, document_id: int, team_id: int, organization_id: Optional[int] = None) -> models.GetDocumentDetailsResponse:
+        r"""Get document details"""
+        hook_ctx = HookContext(operation_id='getDocumentDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.GetDocumentDetailsRequest(
+            document_id=document_id,
             team_id=team_id,
             organization_id=organization_id,
         )
         
+        _globals = models.GetDocumentDetailsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ContentCheckRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/organization/{organizationId}/team/{teamId}/document/{documentId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCheckRequest, "content_request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ContentCheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.GetDocumentDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ProcessedContent])
-                res.processed_content = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.Document])
+                res.document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def correct(self, content_request: models.ContentRequest, team_id: int, x_request_id: Optional[str] = None, organization_id: Optional[int] = None) -> models.ContentCorrectResponse:
-        r"""Apply the style guide suggestions directly to your content."""
-        hook_ctx = HookContext(operation_id='contentCorrect', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ContentCorrectRequest(
-            content_request=content_request,
-            team_id=team_id,
-            x_request_id=x_request_id,
-            organization_id=organization_id,
+    def list(self, request: models.ListTeamDocumentsRequest) -> models.ListTeamDocumentsResponse:
+        r"""List team documents"""
+        hook_ctx = HookContext(operation_id='listTeamDocuments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = models.ListTeamDocumentsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ContentCorrectRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/organization/{organizationId}/team/{teamId}/document', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCorrectRequest, "content_request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ContentCorrectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ListTeamDocumentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.CorrectionResponse])
-                res.correction_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.BriefDocuments])
+                res.brief_documents = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/cowrite.py` & `writerai-3.3.0/src/writer/styleguide.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,158 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class CoWrite:
-    r"""Methods related to CoWrite"""
+class Styleguide:
+    r"""Methods related to Styleguide"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def generate_content(self, generate_template_request: models.GenerateTemplateRequest, team_id: int, organization_id: Optional[int] = None) -> models.GenerateContentResponse:
-        r"""Generate content using predefined templates"""
-        hook_ctx = HookContext(operation_id='Generate Content', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.GenerateContentRequest(
-            generate_template_request=generate_template_request,
-            team_id=team_id,
-            organization_id=organization_id,
+    def get(self, page_id: int) -> models.PageDetailsResponse:
+        r"""Page details"""
+        hook_ctx = HookContext(operation_id='pageDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.PageDetailsRequest(
+            page_id=page_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.GenerateContentRequest, base_url, '/cowrite/organization/{organizationId}/team/{teamId}/generate', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/styleguide/page/{pageId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, models.GenerateContentRequest, "generate_template_request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.GenerateContentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.PageDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.Draft])
-                res.draft = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.PageWithSectionResponse])
+                res.page_with_section_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list_templates(self, team_id: int, template_id: str, organization_id: Optional[int] = None) -> models.ListTemplatesResponse:
-        r"""Get a list of your existing CoWrite templates"""
-        hook_ctx = HookContext(operation_id='listTemplates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ListTemplatesRequest(
-            team_id=team_id,
-            template_id=template_id,
-            organization_id=organization_id,
+    def list_pages(self, limit: Optional[int] = None, offset: Optional[int] = None, status: Optional[models.QueryParamStatus] = None) -> models.ListPagesResponse:
+        r"""List your styleguide pages"""
+        hook_ctx = HookContext(operation_id='listPages', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ListPagesRequest(
+            limit=limit,
+            offset=offset,
+            status=status,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ListTemplatesRequest, base_url, '/cowrite/organization/{organizationId}/team/{teamId}/template/{templateId}', request, self.sdk_configuration.globals)
+        url = base_url + '/styleguide/page'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ListTemplatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ListPagesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.TemplateDetailsResponse])
-                res.template_details_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultPagePublicAPIResponse])
+                res.paginated_result_page_public_api_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/document_sdk.py` & `writerai-3.3.0/src/writer/content.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,182 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class DocumentSDK:
-    r"""Methods related to document"""
+class Content:
+    r"""Methods related to Content"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get(self, document_id: int, team_id: int, organization_id: Optional[int] = None) -> models.GetDocumentDetailsResponse:
-        r"""Get document details"""
-        hook_ctx = HookContext(operation_id='getDocumentDetails', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.GetDocumentDetailsRequest(
-            document_id=document_id,
+    def check(self, content_request: models.ContentRequest, team_id: int, organization_id: Optional[int] = None) -> models.ContentCheckResponse:
+        r"""Check your content against your preset styleguide."""
+        hook_ctx = HookContext(operation_id='contentCheck', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ContentCheckRequest(
+            content_request=content_request,
             team_id=team_id,
             organization_id=organization_id,
         )
         
+        _globals = models.ContentCheckGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.GetDocumentDetailsRequest, base_url, '/organization/{organizationId}/team/{teamId}/document/{documentId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCheckRequest, "content_request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.GetDocumentDetailsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ContentCheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.Document])
-                res.document = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.ProcessedContent])
+                res.processed_content = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: models.ListTeamDocumentsRequest) -> models.ListTeamDocumentsResponse:
-        r"""List team documents"""
-        hook_ctx = HookContext(operation_id='listTeamDocuments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def correct(self, content_request: models.ContentRequest, team_id: int, x_request_id: Optional[str] = None, organization_id: Optional[int] = None) -> models.ContentCorrectResponse:
+        r"""Apply the style guide suggestions directly to your content."""
+        hook_ctx = HookContext(operation_id='contentCorrect', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ContentCorrectRequest(
+            content_request=content_request,
+            team_id=team_id,
+            x_request_id=x_request_id,
+            organization_id=organization_id,
+        )
+        
+        _globals = models.ContentCorrectGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ListTeamDocumentsRequest, base_url, '/organization/{organizationId}/team/{teamId}/document', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(models.ListTeamDocumentsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, models.ContentCorrectRequest, "content_request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ListTeamDocumentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ContentCorrectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.BriefDocuments])
-                res.brief_documents = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.CorrectionResponse])
+                res.correction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/download_the_customized_model.py` & `writerai-3.3.0/src/writer/ai_content_detector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
-from enum import Enum
-from typing import Optional
+from typing import List, Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class FetchFileAcceptEnum(str, Enum):
-    APPLICATION_JSON = "application/json"
-    APPLICATION_OCTET_STREAM = "application/octet-stream"
-
-class DownloadTheCustomizedModel:
-    r"""Methods related to Download the customized model"""
+class AIContentDetector:
+    r"""Methods related to AI Content Detector"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def fetch_file(self, customization_id: str, model_id: str, organization_id: Optional[int] = None, accept_header_override: Optional[FetchFileAcceptEnum] = None) -> models.FetchCustomizedModelFileResponse:
-        r"""Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)"""
-        hook_ctx = HookContext(operation_id='fetchCustomizedModelFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.FetchCustomizedModelFileRequest(
-            customization_id=customization_id,
-            model_id=model_id,
+    def detect(self, content_detector_request: models.ContentDetectorRequest, organization_id: Optional[int] = None) -> models.DetectContentResponse:
+        r"""Content detector api"""
+        hook_ctx = HookContext(operation_id='detectContent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.DetectContentRequest(
+            content_detector_request=content_detector_request,
             organization_id=organization_id,
         )
         
+        _globals = models.DetectContentGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.FetchCustomizedModelFileRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/fetch', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/content/organization/{organizationId}/detect', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        if accept_header_override is not None:
-            headers['Accept'] = accept_header_override.value
-        else:
-            headers['Accept'] = 'application/json;q=1, application/octet-stream;q=0'
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, models.DetectContentRequest, "content_detector_request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.FetchCustomizedModelFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.DetectContentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/octet-stream'):                
-                res.stream = http_res
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[List[models.ContentDetectorResponse]])
+                res.classes = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/files.py` & `writerai-3.3.0/src/writer/modelcustomization_sdk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,304 +1,329 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Files:
-    r"""Methods related to Files"""
+class ModelCustomizationSDK:
+    r"""Methods related to Model Customization"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def delete(self, file_id: str, organization_id: Optional[int] = None) -> models.DeleteFileResponse:
-        r"""Delete file"""
-        hook_ctx = HookContext(operation_id='deleteFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.DeleteFileRequest(
-            file_id=file_id,
+    def create(self, create_customization_request: models.CreateCustomizationRequest, model_id: str, organization_id: Optional[int] = None) -> models.CreateModelCustomizationResponse:
+        r"""Create model customization"""
+        hook_ctx = HookContext(operation_id='createModelCustomization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.CreateModelCustomizationRequest(
+            create_customization_request=create_customization_request,
+            model_id=model_id,
             organization_id=organization_id,
         )
         
+        _globals = models.CreateModelCustomizationGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.DeleteFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, models.CreateModelCustomizationRequest, "create_customization_request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.DeleteFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.CreateModelCustomizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.DeleteFileResponseBody])
-                res.object = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.ModelCustomization])
+                res.model_customization = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, file_id: str, organization_id: Optional[int] = None) -> models.GetFileResponse:
-        r"""Get file"""
-        hook_ctx = HookContext(operation_id='getFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.GetFileRequest(
-            file_id=file_id,
+    def delete(self, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> models.DeleteModelCustomizationResponse:
+        r"""Delete Model customization"""
+        hook_ctx = HookContext(operation_id='deleteModelCustomization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.DeleteModelCustomizationRequest(
+            customization_id=customization_id,
+            model_id=model_id,
             organization_id=organization_id,
         )
         
+        _globals = models.DeleteModelCustomizationGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.GetFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.GetFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.DeleteModelCustomizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ModelFile])
-                res.model_file = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.DeleteModelCustomizationResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, organization_id: Optional[int] = None) -> models.ListFilesResponse:
-        r"""List files"""
-        hook_ctx = HookContext(operation_id='listFiles', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ListFilesRequest(
+    def get(self, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> models.GetModelCustomizationResponse:
+        r"""Get model customization"""
+        hook_ctx = HookContext(operation_id='getModelCustomization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.GetModelCustomizationRequest(
+            customization_id=customization_id,
+            model_id=model_id,
             organization_id=organization_id,
         )
         
+        _globals = models.GetModelCustomizationGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ListFilesRequest, base_url, '/llm/organization/{organizationId}/file', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ListFilesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.GetModelCustomizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ModelFilesResponse])
-                res.model_files_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.ModelCustomization])
+                res.model_customization = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def upload(self, upload_model_file_request: models.UploadModelFileRequest, organization_id: Optional[int] = None) -> models.UploadFileResponse:
-        r"""Upload file"""
-        hook_ctx = HookContext(operation_id='uploadFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.UploadFileRequest(
-            upload_model_file_request=upload_model_file_request,
+    def list(self, model_id: str, organization_id: Optional[int] = None) -> models.ListModelCustomizationsResponse:
+        r"""List model customizations"""
+        hook_ctx = HookContext(operation_id='listModelCustomizations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ListModelCustomizationsRequest(
+            model_id=model_id,
             organization_id=organization_id,
         )
         
+        _globals = models.ListModelCustomizationsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.UploadFileRequest, base_url, '/llm/organization/{organizationId}/file', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, models.UploadFileRequest, "upload_model_file_request", False, False, 'multipart')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.UploadFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ListModelCustomizationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ModelFile])
-                res.model_file = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.CustomizationsResponse])
+                res.customizations_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/modelcustomization_sdk.py` & `writerai-3.3.0/src/writer/files.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,308 +1,325 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class ModelCustomizationSDK:
-    r"""Methods related to Model Customization"""
+class Files:
+    r"""Methods related to Files"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, create_customization_request: models.CreateCustomizationRequest, model_id: str, organization_id: Optional[int] = None) -> models.CreateModelCustomizationResponse:
-        r"""Create model customization"""
-        hook_ctx = HookContext(operation_id='createModelCustomization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.CreateModelCustomizationRequest(
-            create_customization_request=create_customization_request,
-            model_id=model_id,
+    def delete(self, file_id: str, organization_id: Optional[int] = None) -> models.DeleteFileResponse:
+        r"""Delete file"""
+        hook_ctx = HookContext(operation_id='deleteFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.DeleteFileRequest(
+            file_id=file_id,
             organization_id=organization_id,
         )
         
+        _globals = models.DeleteFileGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.CreateModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/file/{fileId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, models.CreateModelCustomizationRequest, "create_customization_request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.CreateModelCustomizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.DeleteFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ModelCustomization])
-                res.model_customization = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.DeleteFileResponseBody])
+                res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def delete(self, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> models.DeleteModelCustomizationResponse:
-        r"""Delete Model customization"""
-        hook_ctx = HookContext(operation_id='deleteModelCustomization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.DeleteModelCustomizationRequest(
-            customization_id=customization_id,
-            model_id=model_id,
+    def get(self, file_id: str, organization_id: Optional[int] = None) -> models.GetFileResponse:
+        r"""Get file"""
+        hook_ctx = HookContext(operation_id='getFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.GetFileRequest(
+            file_id=file_id,
             organization_id=organization_id,
         )
         
+        _globals = models.GetFileGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.DeleteModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/file/{fileId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.DeleteModelCustomizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.GetFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.DeleteModelCustomizationResponseBody])
-                res.object = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.ModelFile])
+                res.model_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> models.GetModelCustomizationResponse:
-        r"""Get model customization"""
-        hook_ctx = HookContext(operation_id='getModelCustomization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.GetModelCustomizationRequest(
-            customization_id=customization_id,
-            model_id=model_id,
+    def list(self, organization_id: Optional[int] = None) -> models.ListFilesResponse:
+        r"""List files"""
+        hook_ctx = HookContext(operation_id='listFiles', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.ListFilesRequest(
             organization_id=organization_id,
         )
         
+        _globals = models.ListFilesGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.GetModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/file', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.GetModelCustomizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ListFilesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.ModelCustomization])
-                res.model_customization = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.ModelFilesResponse])
+                res.model_files_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, model_id: str, organization_id: Optional[int] = None) -> models.ListModelCustomizationsResponse:
-        r"""List model customizations"""
-        hook_ctx = HookContext(operation_id='listModelCustomizations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ListModelCustomizationsRequest(
-            model_id=model_id,
+    def upload(self, upload_model_file_request: models.UploadModelFileRequest, organization_id: Optional[int] = None) -> models.UploadFileResponse:
+        r"""Upload file"""
+        hook_ctx = HookContext(operation_id='uploadFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = models.UploadFileRequest(
+            upload_model_file_request=upload_model_file_request,
             organization_id=organization_id,
         )
         
+        _globals = models.UploadFileGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ListModelCustomizationsRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/llm/organization/{organizationId}/file', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, models.UploadFileRequest, "upload_model_file_request", False, False, 'multipart')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ListModelCustomizationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.UploadFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.CustomizationsResponse])
-                res.customizations_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.ModelFile])
+                res.model_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/models/__init__.py` & `writerai-3.3.0/src/writer/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,8 +94,8 @@
 from .updatetermsrequest import *
 from .uploadfileop import *
 from .uploadmodelfilerequest import *
 from .usage import *
 from .usageitem import *
 from .userpublicresponse import *
 
-__all__ = ["Access","AccountStatus","AddTermsRequest","AddTermsResponse","ApprovedTermExtension","ApprovedTermExtensionCreate","BriefDocument","BriefDocuments","CompletionGenerationChoice","CompletionGenerationChoiceLogprobs","CompletionRequest","CompletionResponse","ContentCheckRequest","ContentCheckResponse","ContentCorrectRequest","ContentCorrectResponse","ContentDetectorRequest","ContentDetectorResponse","ContentIssue","ContentRequest","ContentSettings","CorrectionResponse","CreateCompletionRequest","CreateCompletionResponse","CreateCustomizationRequest","CreateModelCustomizationCompletionRequest","CreateModelCustomizationCompletionResponse","CreateModelCustomizationRequest","CreateModelCustomizationResponse","CreateTermsRequest","CreateTermsResponse","CustomizationsResponse","DeleteFileRequest","DeleteFileResponse","DeleteFileResponseBody","DeleteModelCustomizationRequest","DeleteModelCustomizationResponse","DeleteModelCustomizationResponseBody","DeleteResponse","DeleteSnippetsRequest","DeleteSnippetsResponse","DeleteTermsRequest","DeleteTermsResponse","DetectContentRequest","DetectContentResponse","Document","DocumentAccess","Draft","FailHandling","FailMessage","FailResponse","FetchCustomizedModelFileRequest","FetchCustomizedModelFileResponse","File","FindSnippetsRequest","FindSnippetsResponse","FindTermsRequest","FindTermsResponse","FullLinkedTerm","FullTermWithUser","FullTermWithUserPos","GenerateContentRequest","GenerateContentResponse","GenerateTemplateRequest","GenerationModelInfoResponse","GenerationModelInfoResponseType","GenerationModelsResponse","GetDocumentDetailsRequest","GetDocumentDetailsResponse","GetFileRequest","GetFileResponse","GetModelCustomizationRequest","GetModelCustomizationResponse","GetSubscriptionDetailsResponse","HyperParameters","Input","InputType","Label","LinkedTermCreate","ListFilesRequest","ListFilesResponse","ListModelCustomizationsRequest","ListModelCustomizationsResponse","ListModelsRequest","ListModelsResponse","ListPagesRequest","ListPagesResponse","ListTeamDocumentsQueryParamSortField","ListTeamDocumentsQueryParamSortOrder","ListTeamDocumentsRequest","ListTeamDocumentsResponse","ListTemplatesRequest","ListTemplatesResponse","ListUsersQueryParamSortField","ListUsersQueryParamSortOrder","ListUsersRequest","ListUsersResponse","MagicRequestInput","MetaData","ModelCustomization","ModelFile","ModelFilesResponse","PageDetailsRequest","PageDetailsResponse","PagePublicAPIResponse","PageWithSectionResponse","PageWithSectionResponseStatus","PaginatedResultFullTermWithUser","PaginatedResultPagePublicAPIResponse","PaginatedResultSnippetWithUser","PaginatedResultUserPublicResponse","Pagination","PartOfSpeech","Pos","ProcessedContent","ProductName","QueryParamSortField","QueryParamSortOrder","QueryParamStatus","QueryParamType","SDKError","SectionInfo","Security","Service","SimpleUser","SnippetTagV2","SnippetUpdate","SnippetWithUser","SortField","SortOrder","Status","SubscriptionPublicResponseAPI","SubscriptionPublicResponseAPIStatus","TemplateDetailsResponse","TermCreate","TermCreatePos","TermCreateType","TermExample","TermExampleCreate","TermExampleCreateType","TermExampleType","TermMistake","TermMistakeCreate","TermMistakeCreatePos","TermMistakePos","TermTagCreate","TermTagResponse","TermUpdate","TermUpdatePos","TermUpdateType","TerminologyUser","Tier","Type","UpdateSnippetsRequest","UpdateSnippetsResponse","UpdateTermsRequest","UpdateTermsRequest1","UpdateTermsRequestFailHandling","UpdateTermsResponse","UploadFileRequest","UploadFileResponse","UploadModelFileRequest","Usage","UsageItem","UserPublicResponse"]
+__all__ = ["Access","AccountStatus","AddTermsGlobals","AddTermsRequest","AddTermsResponse","ApprovedTermExtension","ApprovedTermExtensionCreate","BriefDocument","BriefDocuments","CompletionGenerationChoice","CompletionGenerationChoiceLogprobs","CompletionRequest","CompletionResponse","ContentCheckGlobals","ContentCheckRequest","ContentCheckResponse","ContentCorrectGlobals","ContentCorrectRequest","ContentCorrectResponse","ContentDetectorRequest","ContentDetectorResponse","ContentIssue","ContentRequest","ContentSettings","CorrectionResponse","CreateCompletionGlobals","CreateCompletionRequest","CreateCompletionResponse","CreateCustomizationRequest","CreateModelCustomizationCompletionGlobals","CreateModelCustomizationCompletionRequest","CreateModelCustomizationCompletionResponse","CreateModelCustomizationGlobals","CreateModelCustomizationRequest","CreateModelCustomizationResponse","CreateTermsRequest","CreateTermsResponse","CustomizationsResponse","DeleteFileGlobals","DeleteFileRequest","DeleteFileResponse","DeleteFileResponseBody","DeleteModelCustomizationGlobals","DeleteModelCustomizationRequest","DeleteModelCustomizationResponse","DeleteModelCustomizationResponseBody","DeleteResponse","DeleteSnippetsGlobals","DeleteSnippetsRequest","DeleteSnippetsResponse","DeleteTermsGlobals","DeleteTermsRequest","DeleteTermsResponse","DetectContentGlobals","DetectContentRequest","DetectContentResponse","Document","DocumentAccess","Draft","FailHandling","FailMessage","FailResponse","FetchCustomizedModelFileGlobals","FetchCustomizedModelFileRequest","FetchCustomizedModelFileResponse","File","FindSnippetsGlobals","FindSnippetsRequest","FindSnippetsResponse","FindTermsGlobals","FindTermsRequest","FindTermsResponse","FullLinkedTerm","FullTermWithUser","FullTermWithUserPos","GenerateContentGlobals","GenerateContentRequest","GenerateContentResponse","GenerateTemplateRequest","GenerationModelInfoResponse","GenerationModelInfoResponseType","GenerationModelsResponse","GetDocumentDetailsGlobals","GetDocumentDetailsRequest","GetDocumentDetailsResponse","GetFileGlobals","GetFileRequest","GetFileResponse","GetModelCustomizationGlobals","GetModelCustomizationRequest","GetModelCustomizationResponse","GetSubscriptionDetailsResponse","HyperParameters","Input","InputType","Label","LinkedTermCreate","ListFilesGlobals","ListFilesRequest","ListFilesResponse","ListModelCustomizationsGlobals","ListModelCustomizationsRequest","ListModelCustomizationsResponse","ListModelsGlobals","ListModelsRequest","ListModelsResponse","ListPagesRequest","ListPagesResponse","ListTeamDocumentsGlobals","ListTeamDocumentsQueryParamSortField","ListTeamDocumentsQueryParamSortOrder","ListTeamDocumentsRequest","ListTeamDocumentsResponse","ListTemplatesGlobals","ListTemplatesRequest","ListTemplatesResponse","ListUsersQueryParamSortField","ListUsersQueryParamSortOrder","ListUsersRequest","ListUsersResponse","MagicRequestInput","MetaData","ModelCustomization","ModelFile","ModelFilesResponse","PageDetailsRequest","PageDetailsResponse","PagePublicAPIResponse","PageWithSectionResponse","PageWithSectionResponseStatus","PaginatedResultFullTermWithUser","PaginatedResultPagePublicAPIResponse","PaginatedResultSnippetWithUser","PaginatedResultUserPublicResponse","Pagination","PartOfSpeech","Pos","ProcessedContent","ProductName","QueryParamSortField","QueryParamSortOrder","QueryParamStatus","QueryParamType","SDKError","SectionInfo","Security","Service","SimpleUser","SnippetTagV2","SnippetUpdate","SnippetWithUser","SortField","SortOrder","Status","SubscriptionPublicResponseAPI","SubscriptionPublicResponseAPIStatus","TemplateDetailsResponse","TermCreate","TermCreatePos","TermCreateType","TermExample","TermExampleCreate","TermExampleCreateType","TermExampleType","TermMistake","TermMistakeCreate","TermMistakeCreatePos","TermMistakePos","TermTagCreate","TermTagResponse","TermUpdate","TermUpdatePos","TermUpdateType","TerminologyUser","Tier","Type","UpdateSnippetsGlobals","UpdateSnippetsRequest","UpdateSnippetsResponse","UpdateTermsGlobals","UpdateTermsRequest","UpdateTermsRequest1","UpdateTermsRequestFailHandling","UpdateTermsResponse","UploadFileGlobals","UploadFileRequest","UploadFileResponse","UploadModelFileRequest","Usage","UsageItem","UserPublicResponse"]
```

### Comparing `writerai-3.2.1/src/writer/models/addtermsop.py` & `writerai-3.3.0/src/writer/models/addtermsop.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .createtermsrequest import CreateTermsRequest
 from .createtermsresponse import CreateTermsResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class AddTermsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class AddTermsRequest:
     create_terms_request: CreateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/approvedtermextension.py` & `writerai-3.3.0/src/writer/models/approvedtermextension.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/approvedtermextensioncreate.py` & `writerai-3.3.0/src/writer/models/approvedtermextensioncreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/briefdocument.py` & `writerai-3.3.0/src/writer/models/briefdocument.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/briefdocuments.py` & `writerai-3.3.0/src/writer/models/briefdocuments.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/completiongenerationchoice.py` & `writerai-3.3.0/src/writer/models/completiongenerationchoice.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/completiongenerationchoicelogprobs.py` & `writerai-3.3.0/src/writer/models/completiongenerationchoicelogprobs.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/completionrequest.py` & `writerai-3.3.0/src/writer/models/completionrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/completionresponse.py` & `writerai-3.3.0/src/writer/models/completionresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/contentcheckop.py` & `writerai-3.3.0/src/writer/models/contentcheckop.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .contentrequest import ContentRequest
 from .processedcontent import ProcessedContent
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class ContentCheckGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class ContentCheckRequest:
     content_request: ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/contentcorrectop.py` & `writerai-3.3.0/src/writer/models/contentcorrectop.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .contentrequest import ContentRequest
 from .correctionresponse import CorrectionResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class ContentCorrectGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class ContentCorrectRequest:
     content_request: ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/contentdetectorresponse.py` & `writerai-3.3.0/src/writer/models/contentdetectorresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/contentissue.py` & `writerai-3.3.0/src/writer/models/contentissue.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/contentrequest.py` & `writerai-3.3.0/src/writer/models/contentrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/contentsettings.py` & `writerai-3.3.0/src/writer/models/contentsettings.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/createcompletionop.py` & `writerai-3.3.0/src/writer/models/createcompletionop.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .completionrequest import CompletionRequest
 from .completionresponse import CompletionResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class CreateCompletionGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class CreateCompletionRequest:
     completion_request: CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/createcustomizationrequest.py` & `writerai-3.3.0/src/writer/models/createcustomizationrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/createmodelcustomizationcompletionop.py` & `writerai-3.3.0/src/writer/models/createmodelcustomizationcompletionop.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .completionrequest import CompletionRequest
 from .completionresponse import CompletionResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class CreateModelCustomizationCompletionGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class CreateModelCustomizationCompletionRequest:
     completion_request: CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
     model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/createmodelcustomizationop.py` & `writerai-3.3.0/src/writer/models/createmodelcustomizationop.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .createcustomizationrequest import CreateCustomizationRequest
 from .modelcustomization import ModelCustomization
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class CreateModelCustomizationGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class CreateModelCustomizationRequest:
     create_customization_request: CreateCustomizationRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/createtermsrequest.py` & `writerai-3.3.0/src/writer/models/createtermsrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/createtermsresponse.py` & `writerai-3.3.0/src/writer/models/createtermsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/customizationsresponse.py` & `writerai-3.3.0/src/writer/models/customizationsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/deletefileop.py` & `writerai-3.3.0/src/writer/models/listfilesop.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from .modelfilesresponse import ModelFilesResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class DeleteFileRequest:
-    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class ListFilesGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class DeleteFileResponseBody:
-    pass
+class ListFilesRequest:
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
 
 
 @dataclasses.dataclass
-class DeleteFileResponse:
+class ListFilesResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[DeleteFileResponseBody] = dataclasses.field(default=None)
+    model_files_response: Optional[ModelFilesResponse] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/deletemodelcustomizationop.py` & `writerai-3.3.0/src/writer/models/getmodelcustomizationop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from .modelcustomization import ModelCustomization
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class DeleteModelCustomizationRequest:
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class GetModelCustomizationGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class DeleteModelCustomizationResponseBody:
-    pass
+class GetModelCustomizationRequest:
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
 
 
 @dataclasses.dataclass
-class DeleteModelCustomizationResponse:
+class GetModelCustomizationResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[DeleteModelCustomizationResponseBody] = dataclasses.field(default=None)
+    model_customization: Optional[ModelCustomization] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/deletesnippetsop.py` & `writerai-3.3.0/src/writer/models/deletesnippetsop.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import dataclasses
 import requests as requests_http
 from .deleteresponse import DeleteResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class DeleteSnippetsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class DeleteSnippetsRequest:
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/deletetermsop.py` & `writerai-3.3.0/src/writer/models/deletetermsop.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import dataclasses
 import requests as requests_http
 from .deleteresponse import DeleteResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class DeleteTermsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class DeleteTermsRequest:
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     ids: Optional[List[int]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/detectcontentop.py` & `writerai-3.3.0/src/writer/models/deletefileop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .contentdetectorrequest import ContentDetectorRequest
-from .contentdetectorresponse import ContentDetectorResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class DetectContentRequest:
-    content_detector_request: ContentDetectorRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+class DeleteFileGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
+class DeleteFileRequest:
+    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class DetectContentResponse:
+class DeleteFileResponseBody:
+    pass
+
+
+@dataclasses.dataclass
+class DeleteFileResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    classes: Optional[List[ContentDetectorResponse]] = dataclasses.field(default=None)
+    object: Optional[DeleteFileResponseBody] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/document.py` & `writerai-3.3.0/src/writer/models/document.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/draft.py` & `writerai-3.3.0/src/writer/models/draft.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/failmessage.py` & `writerai-3.3.0/src/writer/models/failmessage.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/failresponse.py` & `writerai-3.3.0/src/writer/models/failresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/fetchcustomizedmodelfileop.py` & `writerai-3.3.0/src/writer/models/getfileop.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from .modelfile import ModelFile
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class FetchCustomizedModelFileRequest:
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+class GetFileGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
+class GetFileRequest:
+    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class FetchCustomizedModelFileResponse:
+class GetFileResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    stream: Optional[requests_http.Response] = dataclasses.field(default=None)
+    model_file: Optional[ModelFile] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/findsnippetsop.py` & `writerai-3.3.0/src/writer/models/findsnippetsop.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from .paginatedresult_snippetwithuser import PaginatedResultSnippetWithUser
 from enum import Enum
 from typing import Dict, List, Optional
 
+
+@dataclasses.dataclass
+class FindSnippetsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
 class SortField(str, Enum):
     SHORTCUT = 'shortcut'
     CREATION_TIME = 'creationTime'
     MODIFICATION_TIME = 'modificationTime'
 
 class SortOrder(str, Enum):
     ASC = 'asc'
```

### Comparing `writerai-3.2.1/src/writer/models/findtermsop.py` & `writerai-3.3.0/src/writer/models/findtermsop.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from .paginatedresult_fulltermwithuser import PaginatedResultFullTermWithUser
 from enum import Enum
 from typing import Dict, List, Optional
 
+
+@dataclasses.dataclass
+class FindTermsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
 class PartOfSpeech(str, Enum):
     NOUN = 'noun'
     VERB = 'verb'
     ADVERB = 'adverb'
     ADJECTIVE = 'adjective'
 
 class QueryParamSortField(str, Enum):
```

### Comparing `writerai-3.2.1/src/writer/models/fulllinkedterm.py` & `writerai-3.3.0/src/writer/models/fulllinkedterm.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/fulltermwithuser.py` & `writerai-3.3.0/src/writer/models/fulltermwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/generate_contentop.py` & `writerai-3.3.0/src/writer/models/generate_contentop.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from .draft import Draft
 from .generatetemplaterequest import GenerateTemplateRequest
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class GenerateContentGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class GenerateContentRequest:
     generate_template_request: GenerateTemplateRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/generatetemplaterequest.py` & `writerai-3.3.0/src/writer/models/generatetemplaterequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/generationmodelinforesponse.py` & `writerai-3.3.0/src/writer/models/generationmodelinforesponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/generationmodelsresponse.py` & `writerai-3.3.0/src/writer/models/generationmodelsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/getdocumentdetailsop.py` & `writerai-3.3.0/src/writer/models/getdocumentdetailsop.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import dataclasses
 import requests as requests_http
 from .document import Document
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class GetDocumentDetailsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class GetDocumentDetailsRequest:
     document_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'documentId', 'style': 'simple', 'explode': False }})
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/getfileop.py` & `writerai-3.3.0/src/writer/models/listpagesop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .modelfile import ModelFile
+from .paginatedresult_pagepublicapiresponse import PaginatedResultPagePublicAPIResponse
+from enum import Enum
 from typing import Dict, List, Optional
 
+class QueryParamStatus(str, Enum):
+    LIVE = 'live'
+    OFFLINE = 'offline'
+
 
 @dataclasses.dataclass
-class GetFileRequest:
-    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class ListPagesRequest:
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    status: Optional[QueryParamStatus] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'status', 'style': 'form', 'explode': True }})
     
 
 
 
 @dataclasses.dataclass
-class GetFileResponse:
+class ListPagesResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    model_file: Optional[ModelFile] = dataclasses.field(default=None)
+    paginated_result_page_public_api_response: Optional[PaginatedResultPagePublicAPIResponse] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/getmodelcustomizationop.py` & `writerai-3.3.0/src/writer/models/deletemodelcustomizationop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .modelcustomization import ModelCustomization
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class GetModelCustomizationRequest:
+class DeleteModelCustomizationGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
+class DeleteModelCustomizationRequest:
     customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
     model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class GetModelCustomizationResponse:
+class DeleteModelCustomizationResponseBody:
+    pass
+
+
+@dataclasses.dataclass
+class DeleteModelCustomizationResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    model_customization: Optional[ModelCustomization] = dataclasses.field(default=None)
+    object: Optional[DeleteModelCustomizationResponseBody] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/getsubscriptiondetailsop.py` & `writerai-3.3.0/src/writer/models/getsubscriptiondetailsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/input.py` & `writerai-3.3.0/src/writer/models/input.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/linkedtermcreate.py` & `writerai-3.3.0/src/writer/models/linkedtermcreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/listfilesop.py` & `writerai-3.3.0/src/writer/models/uploadfileop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .modelfilesresponse import ModelFilesResponse
+from .modelfile import ModelFile
+from .uploadmodelfilerequest import UploadModelFileRequest
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class ListFilesRequest:
+class UploadFileGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
+class UploadFileRequest:
+    upload_model_file_request: UploadModelFileRequest = dataclasses.field(metadata={'request': { 'media_type': 'multipart/form-data' }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class ListFilesResponse:
+class UploadFileResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    model_files_response: Optional[ModelFilesResponse] = dataclasses.field(default=None)
+    model_file: Optional[ModelFile] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/listmodelcustomizationsop.py` & `writerai-3.3.0/src/writer/models/listmodelcustomizationsop.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import dataclasses
 import requests as requests_http
 from .customizationsresponse import CustomizationsResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class ListModelCustomizationsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class ListModelCustomizationsRequest:
     model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/listmodelsop.py` & `writerai-3.3.0/src/writer/models/listmodelsop.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import dataclasses
 import requests as requests_http
 from .generationmodelsresponse import GenerationModelsResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class ListModelsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class ListModelsRequest:
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
```

### Comparing `writerai-3.2.1/src/writer/models/listpagesop.py` & `writerai-3.3.0/src/writer/models/updatesnippetsop.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .paginatedresult_pagepublicapiresponse import PaginatedResultPagePublicAPIResponse
-from enum import Enum
+from .snippetupdate import SnippetUpdate
+from .snippetwithuser import SnippetWithUser
 from typing import Dict, List, Optional
 
-class QueryParamStatus(str, Enum):
-    LIVE = 'live'
-    OFFLINE = 'offline'
+
+@dataclasses.dataclass
+class UpdateSnippetsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
 
 
 @dataclasses.dataclass
-class ListPagesRequest:
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-    status: Optional[QueryParamStatus] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'status', 'style': 'form', 'explode': True }})
+class UpdateSnippetsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    request_body: Optional[List[SnippetUpdate]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class ListPagesResponse:
+class UpdateSnippetsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    paginated_result_page_public_api_response: Optional[PaginatedResultPagePublicAPIResponse] = dataclasses.field(default=None)
+    classes: Optional[List[SnippetWithUser]] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/listteamdocumentsop.py` & `writerai-3.3.0/src/writer/models/listusersop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .briefdocuments import BriefDocuments
+from .paginatedresult_userpublicresponse import PaginatedResultUserPublicResponse
 from enum import Enum
 from typing import Dict, List, Optional
 
-class ListTeamDocumentsQueryParamSortField(str, Enum):
-    TITLE = 'title'
+class ListUsersQueryParamSortField(str, Enum):
+    ID = 'id'
+    NAME = 'name'
     CREATION_TIME = 'creationTime'
+    DELETED = 'deleted'
     MODIFICATION_TIME = 'modificationTime'
-    MODIFIED_BY_ME_TIME = 'modifiedByMeTime'
-    OPENED_BY_ME_TIME = 'openedByMeTime'
+    EMAIL = 'email'
+    LAST_SEEN = 'lastSeen'
 
-class ListTeamDocumentsQueryParamSortOrder(str, Enum):
+class ListUsersQueryParamSortOrder(str, Enum):
     ASC = 'asc'
     DESC = 'desc'
 
 
 @dataclasses.dataclass
-class ListTeamDocumentsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+class ListUsersRequest:
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
-    sort_field: Optional[ListTeamDocumentsQueryParamSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
-    sort_order: Optional[ListTeamDocumentsQueryParamSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
+    sort_field: Optional[ListUsersQueryParamSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
+    sort_order: Optional[ListUsersQueryParamSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
     
 
 
 
 @dataclasses.dataclass
-class ListTeamDocumentsResponse:
+class ListUsersResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    brief_documents: Optional[BriefDocuments] = dataclasses.field(default=None)
+    paginated_result_user_public_response: Optional[PaginatedResultUserPublicResponse] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/listtemplatesop.py` & `writerai-3.3.0/src/writer/models/listtemplatesop.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import dataclasses
 import requests as requests_http
 from .templatedetailsresponse import TemplateDetailsResponse
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
+class ListTemplatesGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class ListTemplatesRequest:
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     template_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'templateId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
```

### Comparing `writerai-3.2.1/src/writer/models/listusersop.py` & `writerai-3.3.0/src/writer/models/listteamdocumentsop.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .paginatedresult_userpublicresponse import PaginatedResultUserPublicResponse
+from .briefdocuments import BriefDocuments
 from enum import Enum
 from typing import Dict, List, Optional
 
-class ListUsersQueryParamSortField(str, Enum):
-    ID = 'id'
-    NAME = 'name'
+
+@dataclasses.dataclass
+class ListTeamDocumentsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+class ListTeamDocumentsQueryParamSortField(str, Enum):
+    TITLE = 'title'
     CREATION_TIME = 'creationTime'
-    DELETED = 'deleted'
     MODIFICATION_TIME = 'modificationTime'
-    EMAIL = 'email'
-    LAST_SEEN = 'lastSeen'
+    MODIFIED_BY_ME_TIME = 'modifiedByMeTime'
+    OPENED_BY_ME_TIME = 'openedByMeTime'
 
-class ListUsersQueryParamSortOrder(str, Enum):
+class ListTeamDocumentsQueryParamSortOrder(str, Enum):
     ASC = 'asc'
     DESC = 'desc'
 
 
 @dataclasses.dataclass
-class ListUsersRequest:
+class ListTeamDocumentsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
-    sort_field: Optional[ListUsersQueryParamSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
-    sort_order: Optional[ListUsersQueryParamSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
+    sort_field: Optional[ListTeamDocumentsQueryParamSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
+    sort_order: Optional[ListTeamDocumentsQueryParamSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
     
 
 
 
 @dataclasses.dataclass
-class ListUsersResponse:
+class ListTeamDocumentsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    paginated_result_user_public_response: Optional[PaginatedResultUserPublicResponse] = dataclasses.field(default=None)
+    brief_documents: Optional[BriefDocuments] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/magicrequestinput.py` & `writerai-3.3.0/src/writer/models/magicrequestinput.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/metadata.py` & `writerai-3.3.0/src/writer/models/metadata.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/modelcustomization.py` & `writerai-3.3.0/src/writer/models/modelcustomization.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/modelfile.py` & `writerai-3.3.0/src/writer/models/modelfile.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/modelfilesresponse.py` & `writerai-3.3.0/src/writer/models/modelfilesresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/pagedetailsop.py` & `writerai-3.3.0/src/writer/models/pagedetailsop.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/pagepublicapiresponse.py` & `writerai-3.3.0/src/writer/models/pagepublicapiresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/pagewithsectionresponse.py` & `writerai-3.3.0/src/writer/models/pagewithsectionresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/paginatedresult_fulltermwithuser.py` & `writerai-3.3.0/src/writer/models/paginatedresult_fulltermwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/paginatedresult_pagepublicapiresponse.py` & `writerai-3.3.0/src/writer/models/paginatedresult_pagepublicapiresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/paginatedresult_snippetwithuser.py` & `writerai-3.3.0/src/writer/models/paginatedresult_snippetwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/paginatedresult_userpublicresponse.py` & `writerai-3.3.0/src/writer/models/paginatedresult_userpublicresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/pagination.py` & `writerai-3.3.0/src/writer/models/pagination.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/processedcontent.py` & `writerai-3.3.0/src/writer/models/processedcontent.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/sdkerror.py` & `writerai-3.3.0/src/writer/models/sdkerror.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/sectioninfo.py` & `writerai-3.3.0/src/writer/models/sectioninfo.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/simpleuser.py` & `writerai-3.3.0/src/writer/models/simpleuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/snippetupdate.py` & `writerai-3.3.0/src/writer/models/snippetupdate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/snippetwithuser.py` & `writerai-3.3.0/src/writer/models/snippetwithuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/subscriptionpublicresponseapi.py` & `writerai-3.3.0/src/writer/models/subscriptionpublicresponseapi.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/templatedetailsresponse.py` & `writerai-3.3.0/src/writer/models/templatedetailsresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termcreate.py` & `writerai-3.3.0/src/writer/models/termcreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termexample.py` & `writerai-3.3.0/src/writer/models/termexample.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termexamplecreate.py` & `writerai-3.3.0/src/writer/models/termexamplecreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/terminologyuser.py` & `writerai-3.3.0/src/writer/models/terminologyuser.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termmistake.py` & `writerai-3.3.0/src/writer/models/termmistake.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termmistakecreate.py` & `writerai-3.3.0/src/writer/models/termmistakecreate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termtagresponse.py` & `writerai-3.3.0/src/writer/models/termtagresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/termupdate.py` & `writerai-3.3.0/src/writer/models/termupdate.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/updatesnippetsop.py` & `writerai-3.3.0/src/writer/models/updatetermsop.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .snippetupdate import SnippetUpdate
-from .snippetwithuser import SnippetWithUser
+from .createtermsresponse import CreateTermsResponse
+from .updatetermsrequest import UpdateTermsRequest
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class UpdateSnippetsRequest:
+class UpdateTermsGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
+class UpdateTermsRequest1:
+    update_terms_request: UpdateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    request_body: Optional[List[SnippetUpdate]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class UpdateSnippetsResponse:
+class UpdateTermsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    classes: Optional[List[SnippetWithUser]] = dataclasses.field(default=None)
+    create_terms_response: Optional[CreateTermsResponse] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/updatetermsop.py` & `writerai-3.3.0/src/writer/models/fetchcustomizedmodelfileop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from .createtermsresponse import CreateTermsResponse
-from .updatetermsrequest import UpdateTermsRequest
 from typing import Dict, List, Optional
 
 
 @dataclasses.dataclass
-class UpdateTermsRequest1:
-    update_terms_request: UpdateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+class FetchCustomizedModelFileGlobals:
+    organization_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
+class FetchCustomizedModelFileRequest:
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
     organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
-class UpdateTermsResponse:
+class FetchCustomizedModelFileResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     headers: Dict[str, List[str]] = dataclasses.field()
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    create_terms_response: Optional[CreateTermsResponse] = dataclasses.field(default=None)
+    stream: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-3.2.1/src/writer/models/updatetermsrequest.py` & `writerai-3.3.0/src/writer/models/updatetermsrequest.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/usage.py` & `writerai-3.3.0/src/writer/models/usage.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/usageitem.py` & `writerai-3.3.0/src/writer/models/usageitem.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models/userpublicresponse.py` & `writerai-3.3.0/src/writer/models/userpublicresponse.py`

 * *Files identical despite different names*

### Comparing `writerai-3.2.1/src/writer/models_.py` & `writerai-3.3.0/src/writer/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,83 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
-class Models:
-    r"""Methods related to Model"""
+class User:
+    r"""Methods related to User"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, organization_id: Optional[int] = None) -> models.ListModelsResponse:
-        r"""List available LLM models"""
-        hook_ctx = HookContext(operation_id='listModels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = models.ListModelsRequest(
-            organization_id=organization_id,
-        )
-        
+    def list(self, request: models.ListUsersRequest) -> models.ListUsersResponse:
+        r"""List users"""
+        hook_ctx = HookContext(operation_id='listUsers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.ListModelsRequest, base_url, '/llm/organization/{organizationId}/model', request, self.sdk_configuration.globals)
+        url = base_url + '/user'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.ListModelsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.ListUsersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[models.GenerationModelsResponse])
-                res.generation_models_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultUserPublicResponse])
+                res.paginated_result_user_public_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/sdk.py` & `writerai-3.3.0/src/writer/sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 from .modelcustomization_sdk import ModelCustomizationSDK
 from .models_ import Models
 from .sdkconfiguration import SDKConfiguration
 from .snippet import Snippet
 from .styleguide import Styleguide
 from .terminology import Terminology
 from .user import User
+from .utils.retries import RetryConfig
 from typing import Callable, Dict, Optional, Union
 from writer import models, utils
 from writer._hooks import SDKHooks
+from writer.models import internal
 
 class Writer:
     billing: Billing
     r"""Methods related to Billing"""
     ai_content_detector: AIContentDetector
     r"""Methods related to AI Content Detector"""
     content: Content
@@ -55,15 +57,15 @@
     def __init__(self,
                  api_key: Union[str, Callable[[], str]],
                  organization_id: int = None,
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param api_key: The api_key required for authentication
         :type api_key: Union[str, Callable[[], str]]
         :param organization_id: Configures the organization_id parameter for all supported operations
         :type organization_id: int
@@ -72,56 +74,51 @@
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(api_key):
             def security():
                 return models.Security(api_key = api_key())
         else:
             security = models.Security(api_key = api_key)
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
-        global_params = {
-            'parameters': {
-                'queryParam': {
-                },
-                'pathParam': {
-                    'organization_id': organization_id,
-                },
-            },
-        }
+    
+        _globals = internal.Globals(
+            organization_id=organization_id,
+        )
 
         self.sdk_configuration = SDKConfiguration(
             client,
+            _globals,
             security,
             server_url,
             server_idx,
-            global_params,
             retry_config=retry_config
         )
 
         hooks = SDKHooks()
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.billing = Billing(self.sdk_configuration)
         self.ai_content_detector = AIContentDetector(self.sdk_configuration)
```

### Comparing `writerai-3.2.1/src/writer/sdkconfiguration.py` & `writerai-3.3.0/src/writer/sdkconfiguration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
-from dataclasses import dataclass, field
-from typing import Any, Callable, Dict, Tuple, Union
+from dataclasses import dataclass
+from typing import Callable, Dict, Optional, Tuple, Union
 from writer import models
+from writer.models import internal
 
 
 SERVERS = [
     'https://enterprise-api.writer.com',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
+    globals: internal.Globals
     security: Union[models.Security,Callable[[], models.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
-    globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.7'
-    sdk_version: str = '3.2.1'
-    gen_version: str = '2.280.6'
-    user_agent: str = 'speakeasy-sdk/python 3.2.1 2.280.6 1.7 writerai'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '3.3.0'
+    gen_version: str = '2.312.1'
+    user_agent: str = 'speakeasy-sdk/python 3.3.0 2.312.1 1.7 writerai'
+    retry_config: Optional[RetryConfig] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `writerai-3.2.1/src/writer/snippet.py` & `writerai-3.3.0/src/writer/snippet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import List, Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
 class Snippet:
     r"""Methods related to Snippets"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -21,65 +21,68 @@
         request = models.DeleteSnippetsRequest(
             team_id=team_id,
             x_request_id=x_request_id,
             ids=ids,
             organization_id=organization_id,
         )
         
+        _globals = models.DeleteSnippetsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.DeleteSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(models.DeleteSnippetsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.DeleteSnippetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.DeleteSnippetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.DeleteResponse])
                 res.delete_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -89,64 +92,68 @@
         return res
 
     
     
     def find(self, request: models.FindSnippetsRequest) -> models.FindSnippetsResponse:
         r"""Find snippets"""
         hook_ctx = HookContext(operation_id='findSnippets', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = models.FindSnippetsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.FindSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(models.FindSnippetsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.FindSnippetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.FindSnippetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultSnippetWithUser])
                 res.paginated_result_snippet_with_user = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -163,73 +170,78 @@
         request = models.UpdateSnippetsRequest(
             team_id=team_id,
             request_body=request_body,
             x_request_id=x_request_id,
             organization_id=organization_id,
         )
         
+        _globals = models.UpdateSnippetsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.UpdateSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, models.UpdateSnippetsRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.UpdateSnippetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.UpdateSnippetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[models.SnippetWithUser]])
                 res.classes = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/terminology.py` & `writerai-3.3.0/src/writer/terminology.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import List, Optional
 from writer import models, utils
-from writer._hooks import HookContext
+from writer._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 
 class Terminology:
     r"""Methods related to Terminology"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -20,68 +20,73 @@
         hook_ctx = HookContext(operation_id='addTerms', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = models.AddTermsRequest(
             create_terms_request=create_terms_request,
             team_id=team_id,
             organization_id=organization_id,
         )
         
+        _globals = models.AddTermsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.AddTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, models.AddTermsRequest, "create_terms_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.AddTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.AddTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.CreateTermsResponse])
                 res.create_terms_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -98,65 +103,68 @@
         request = models.DeleteTermsRequest(
             team_id=team_id,
             x_request_id=x_request_id,
             ids=ids,
             organization_id=organization_id,
         )
         
+        _globals = models.DeleteTermsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.DeleteTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(models.DeleteTermsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.DeleteTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.DeleteTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.DeleteResponse])
                 res.delete_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -166,64 +174,68 @@
         return res
 
     
     
     def find(self, request: models.FindTermsRequest) -> models.FindTermsResponse:
         r"""Find terms"""
         hook_ctx = HookContext(operation_id='findTerms', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = models.FindTermsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.FindTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(models.FindTermsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.FindTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.FindTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.PaginatedResultFullTermWithUser])
                 res.paginated_result_full_term_with_user = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -240,75 +252,80 @@
         request = models.UpdateTermsRequest1(
             update_terms_request=update_terms_request,
             team_id=team_id,
             x_request_id=x_request_id,
             organization_id=organization_id,
         )
         
+        _globals = models.UpdateTermsGlobals(
+            organization_id=self.sdk_configuration.globals.organization_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(models.UpdateTermsRequest1, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, models.UpdateTermsRequest1, "update_terms_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','401','403','404','4XX','500','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = models.UpdateTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res, headers=None)
+        res = models.UpdateTermsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[models.CreateTermsResponse])
                 res.create_terms_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, models.FailResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise models.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise models.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise models.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `writerai-3.2.1/src/writer/utils/retries.py` & `writerai-3.3.0/src/writer/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `writerai-3.2.1/src/writer/utils/utils.py` & `writerai-3.3.0/src/writer/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, field.name))
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -835,64 +977,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `writerai-3.2.1/src/writerai.egg-info/SOURCES.txt` & `writerai-3.3.0/src/writerai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 src/writer/models/updatetermsop.py
 src/writer/models/updatetermsrequest.py
 src/writer/models/uploadfileop.py
 src/writer/models/uploadmodelfilerequest.py
 src/writer/models/usage.py
 src/writer/models/usageitem.py
 src/writer/models/userpublicresponse.py
+src/writer/models/internal/__init__.py
+src/writer/models/internal/globals.py
 src/writer/utils/__init__.py
 src/writer/utils/retries.py
 src/writer/utils/utils.py
 src/writerai.egg-info/PKG-INFO
 src/writerai.egg-info/SOURCES.txt
 src/writerai.egg-info/dependency_links.txt
 src/writerai.egg-info/requires.txt
```

