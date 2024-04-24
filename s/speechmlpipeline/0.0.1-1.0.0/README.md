# Comparing `tmp/speechmlpipeline-0.0.1-py3-none-any.whl.zip` & `tmp/speechmlpipeline-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 26016 bytes, number of entries: 30
+Zip file size: 28884 bytes, number of entries: 32
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-22 17:49 speechmlpipeline/__init__.py
 -rw-r--r--  2.0 unx    12095 b- defN 24-Feb-23 22:25 speechmlpipeline/main_pipeline_local_function.py
 -rw-r--r--  2.0 unx     4897 b- defN 24-Feb-26 20:08 speechmlpipeline/sample_run.py
 -rw-r--r--  2.0 unx     4680 b- defN 24-Feb-26 17:42 speechmlpipeline/sample_run_existingllama2output.py
 -rw-r--r--  2.0 unx     1542 b- defN 24-Jan-30 23:07 speechmlpipeline/AudioToTextTranscription/Whisper.py
 -rw-r--r--  2.0 unx     4399 b- defN 24-Feb-19 20:12 speechmlpipeline/AudioToTextTranscription/Whispertimestamped.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 19:14 speechmlpipeline/AudioToTextTranscription/__init__.py
@@ -11,22 +11,24 @@
 -rw-r--r--  2.0 unx      376 b- defN 24-Jan-30 22:22 speechmlpipeline/DownloadModels/Download_Whisper_Model.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-22 17:38 speechmlpipeline/DownloadModels/__init__.py
 -rw-r--r--  2.0 unx     1340 b- defN 24-Feb-19 20:25 speechmlpipeline/DownloadModels/download_models_main_function.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-23 22:13 speechmlpipeline/EnsembleSpeakerChangeDetection/__init__.py
 -rw-r--r--  2.0 unx     1496 b- defN 24-Feb-26 17:27 speechmlpipeline/EnsembleSpeakerChangeDetection/ensemble_detection.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 19:14 speechmlpipeline/Evaluation/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 20:35 speechmlpipeline/Evaluation/SpeakerChangeDetection/__init__.py
--rw-r--r--  2.0 unx     5994 b- defN 24-Feb-26 18:21 speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-Apr-03 21:40 speechmlpipeline/Evaluation/SpeakerChangeDetection/examine_pyannote_metrics.py
+-rw-r--r--  2.0 unx     9970 b- defN 24-Apr-03 22:43 speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function.py
+-rw-r--r--  2.0 unx     1942 b- defN 24-Apr-03 19:02 speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function_revised.py
 -rw-r--r--  2.0 unx     1926 b- defN 24-Feb-23 22:19 speechmlpipeline/Helpers/helpers.py
 -rw-r--r--  2.0 unx     3694 b- defN 24-Jan-30 21:42 speechmlpipeline/PreprocessData/Run_VideoAudioPreprocessing.py
 -rw-r--r--  2.0 unx     5338 b- defN 24-Jan-30 21:42 speechmlpipeline/PreprocessData/VideoAudioPreprocessing.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 19:14 speechmlpipeline/PreprocessData/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-23 22:13 speechmlpipeline/SpeakerChangeDetection/__init__.py
 -rw-r--r--  2.0 unx     3353 b- defN 24-Feb-26 17:27 speechmlpipeline/SpeakerChangeDetection/speaker_change_detection_main_function.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-15 23:45 speechmlpipeline/SpeakerIdentification/__init__.py
 -rw-r--r--  2.0 unx     6549 b- defN 24-Feb-23 22:25 speechmlpipeline/SpeakerIdentification/speaker_identification_main_function.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Feb-26 20:30 speechmlpipeline-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7169 b- defN 24-Feb-26 20:30 speechmlpipeline-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-26 20:30 speechmlpipeline-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Feb-26 20:30 speechmlpipeline-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3194 b- defN 24-Feb-26 20:30 speechmlpipeline-0.0.1.dist-info/RECORD
-30 files, 70160 bytes uncompressed, 20572 bytes compressed:  70.7%
+-rw-r--r--  2.0 unx     1092 b- defN 24-Apr-24 16:23 speechmlpipeline-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7861 b- defN 24-Apr-24 16:23 speechmlpipeline-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 16:23 speechmlpipeline-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-24 16:23 speechmlpipeline-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3469 b- defN 24-Apr-24 16:23 speechmlpipeline-1.0.0.dist-info/RECORD
+32 files, 78914 bytes uncompressed, 22966 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -42,17 +42,23 @@
 
 Filename: speechmlpipeline/Evaluation/__init__.py
 Comment: 
 
 Filename: speechmlpipeline/Evaluation/SpeakerChangeDetection/__init__.py
 Comment: 
 
+Filename: speechmlpipeline/Evaluation/SpeakerChangeDetection/examine_pyannote_metrics.py
+Comment: 
+
 Filename: speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function.py
 Comment: 
 
+Filename: speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function_revised.py
+Comment: 
+
 Filename: speechmlpipeline/Helpers/helpers.py
 Comment: 
 
 Filename: speechmlpipeline/PreprocessData/Run_VideoAudioPreprocessing.py
 Comment: 
 
 Filename: speechmlpipeline/PreprocessData/VideoAudioPreprocessing.py
@@ -69,23 +75,23 @@
 
 Filename: speechmlpipeline/SpeakerIdentification/__init__.py
 Comment: 
 
 Filename: speechmlpipeline/SpeakerIdentification/speaker_identification_main_function.py
 Comment: 
 
-Filename: speechmlpipeline-0.0.1.dist-info/LICENSE
+Filename: speechmlpipeline-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: speechmlpipeline-0.0.1.dist-info/METADATA
+Filename: speechmlpipeline-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: speechmlpipeline-0.0.1.dist-info/WHEEL
+Filename: speechmlpipeline-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: speechmlpipeline-0.0.1.dist-info/top_level.txt
+Filename: speechmlpipeline-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: speechmlpipeline-0.0.1.dist-info/RECORD
+Filename: speechmlpipeline-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function.py

```diff
@@ -8,14 +8,28 @@
 import pandas as pd
 from numpy import NaN
 
 from pyannote.core import Annotation, Timeline, Segment
 from pyannote.metrics.segmentation import SegmentationPrecision, SegmentationRecall, \
     SegmentationCoverage, SegmentationPurity
 
+def map_notsure_to_true(x):
+    if x == 'NotSure':
+        return True
+    else:
+        return x
+
+def map_string_to_bool(x):
+    if type(x) == str: # Check if x is string
+        if x.lower() == 'true':
+            return True
+        elif x.lower() == 'false':
+            return False
+    else:
+        return x
 
 def calculate_detection_metrics(prediction_output_path, labelled_data_path, csv_filename, tolerance=0.5):
     '''
     The function calculates metrics to evaluate the performance of speaker change detection models. The calculated metrics
     are segment precision, segment recall, segment precision recall f1 score,
     segment coverage, segment purity, and segment purity f1 score.
 
@@ -37,81 +51,148 @@
     :return: None
     :rtype: None
     '''
     # Read Prediction and Labelled DF
     prediction_df = pd.read_csv(os.path.join(prediction_output_path, csv_filename))
     labelled_df = pd.read_csv(os.path.join(labelled_data_path, csv_filename))
 
+    # Process Llama2 and NLP Predictions, filling not sure predictions as speaker change as true
+    prediction_df['speaker_change_nlp'] = prediction_df['speaker_change_nlp'].apply(map_notsure_to_true).apply(map_string_to_bool)
+    prediction_df['speaker_change_llama2'] = prediction_df['speaker_change_llama2'].apply(map_notsure_to_true).apply(map_string_to_bool)
+
+    # Fill the empty silence parts into previous speaker ending as the pyannotate metircs module requires the continous segment
     # Parse Inputs to Data Structures in Metrics Module
-    labelled_df['end'] = labelled_df['bgn'] + labelled_df['duration']
-    labels_segments = Timeline()
-    labels_annotation = Annotation()
-    for idx, row in labelled_df[['bgn', 'end', 'speaker']].iterrows():
-        time_segment = Segment(row['bgn'], row['end'])
-        labels_segments.add(time_segment)
-        labels_annotation[time_segment] = row['speaker']
+    labelled_end_times = list(labelled_df['bgn'])[1:]
+    labelled_end_times.append(labelled_df.iloc[-1]['bgn']+labelled_df.iloc[-1]['duration'])
+    labelled_df['end'] = labelled_end_times
+
+
+    prediction_end_times = list(prediction_df['start'])[1:]
+    prediction_end_times.append(prediction_df.iloc[-1]['end'])
+    prediction_df['end'] = prediction_end_times
 
     # Initialize Metrics Class
     coverage_score = SegmentationCoverage(tolerance=tolerance)
     purity_score = SegmentationPurity(tolerance=tolerance)
     precision_score = SegmentationPrecision(tolerance=tolerance)
     recall_score = SegmentationRecall(tolerance=tolerance)
 
     # Initialize Evaluation DataFrame
     evaluation_df = pd.DataFrame()
+
     # List Six Metrics for Calculation
     metrics_names_list = ['precision', 'recall', 'precision_recall_f1', 'coverage', 'purity', 'coverage_purity_f1']
     evaluation_df['metric_name'] = metrics_names_list
-    evaluation_df['audio_file_name'] = [csv_filename.split('.')[0]] * len(metrics_names_list)
 
-    # Check imbalance dataset; Baseline: If predict all speaker change as true or false
+
+    labels_segments = Timeline()
+    labels_annotation = Annotation()
+
+    # Append pseudo last row with speaker col to deal with the last row exception
+    # If the real last row speaker change is FALSE, then merge all false speaker segments including the real last row together
+    # If the real last row speaker change is TRUE, then the real last row itself is also the independent segment
+    labelled_df.loc[len(labelled_df)] = labelled_df.iloc[-1]
+    labelled_df.loc[len(labelled_df)-1, 'speaker'] = 'random'  # pseudo random speaker to ensure the last row get processed
+
     num_speaker_changes = 0
-    prev_speaker = labelled_df.iloc[0]['speaker']
-    for speaker in labelled_df.iloc[1:]['speaker']:
+    first_row = labelled_df.iloc[0]
+    prev_speaker = first_row['speaker']
+    start_segment = first_row['bgn']
+    end_segment = first_row['end']
+
+    for idx, row in labelled_df[['bgn', 'end', 'speaker']].iloc[1:].iterrows():
+        speaker = row['speaker']
         if speaker != prev_speaker:
             num_speaker_changes += 1
+            time_segment = Segment(start_segment, end_segment)
+            labels_segments.add(time_segment)
+            labels_annotation[time_segment] = prev_speaker
+
+            # Update all information after the segment is recorded in annotation
+            start_segment = row['bgn']
+            end_segment = row['end']
             prev_speaker = speaker
-    proportion_no_speaker_changes = 1 - num_speaker_changes/labelled_df.shape[0]
-    evaluation_df['proportion_no_speaker_changes'] = proportion_no_speaker_changes
+        else:
+            end_segment = row['end']
+
+    #Extract files charactersitics
+    npossiblechanges = labelled_df.shape[0]-2 # Exclude pseudo row and first row
+    if npossiblechanges == 0: # Labelled df only has one row and one pseudo row, no speaker change at all
+        proportion_speaker_changes = 0
+    else:
+        proportion_speaker_changes = (num_speaker_changes - 1)/(npossiblechanges)
+    num_of_speakers = len(labelled_df['speaker'].unique())-1 #Drop random speaker in the end
+
+    # Put file characteristics in a df
+    metrics_num = len(metrics_names_list)
+    evaluation_df['audio_file_name'] = [csv_filename.split('.')[0]] * metrics_num
+    evaluation_df['speaking_len_file'] =[labelled_end_times[-1]] * metrics_num
+    evaluation_df['num_of_speakers'] = [num_of_speakers] * metrics_num
+    evaluation_df['num_speaker_changes'] = [num_speaker_changes - 1] * metrics_num
+    evaluation_df['proportion_speaker_changes'] = [proportion_speaker_changes] * metrics_num
+
+    # Append pseudo last row with speaker change col TRUE to deal with the last row exception
+    # If the real last row is FALSE, then merge all false speaker segments including the real last row together
+    # If the real last row is TRUE, then the real last row itself is also the independent segment
+    prediction_df.loc[len(prediction_df)] = prediction_df.iloc[-1]
 
     # Calculate Evaluation Metrics for All Models
     speaker_change_models_cols = [col for col in prediction_df.columns if 'speaker_change' in col and 'true' not in col]
     for speaker_change_col in speaker_change_models_cols:
+        # Update the speaker change column of the model in last row as true
+        prediction_df.loc[len(prediction_df) - 1, speaker_change_col] = True
+
         # Parse Inputs into Data Structures on Metrics Module
         prediction_segments = Timeline()
         start_segment = prediction_df.iloc[0]['start']
         end_segment = prediction_df.iloc[0]['end']
 
-        # Append pseudo last row with speaker change col TRUE to deal with the last row exception
-        # If the real last row is FALSE, then merge all false speaker segments including the real last row together
-        # If the real last row is TRUE, then the real last row itself is also the independent segment
-        prediction_df.loc[len(prediction_df)] = prediction_df.iloc[-1]
-        # New row is appended
-        prediction_df.loc[len(prediction_df)-1, speaker_change_col] = True
-
         for current_row_idx, row in prediction_df.iterrows():
             if current_row_idx == 0:  # No speaker changes information of the first row
                 continue
             # If speaker_change = True, merge previous false speaker change segments together
             if row[speaker_change_col]:
                 prediction_segments.add(Segment(start_segment, end_segment))
                 start_segment = row['start']
                 end_segment = row['end']
             else:
                 end_segment = row['end']
-        precision = precision_score(labels_segments, prediction_segments)
-        recall = recall_score(labels_segments, prediction_segments)
+        # Fix the bug of PyAnnote which calculates the prediction as 1 when there is zero speaker change prediction
+        if sum(prediction_df[speaker_change_col]) == 2: #The first and last rows have two pseudo true speaker changes; zero indeed speaker change prediction
+            precision = NaN
+        else:
+            precision = precision_score(labels_segments, prediction_segments)
+        # Fix the bug of PyAnnote which calculates recall when zero speaker change happens
+        if num_speaker_changes == 1: #only has one pseudo speaker change, zero real speaker change
+            recall = NaN
+        else:
+            recall = recall_score(labels_segments, prediction_segments)
         if (precision+recall != 0):
             precision_recall_f1 = 2 * precision * recall / (precision + recall)
         else:
             precision_recall_f1 = NaN
         coverage = coverage_score(labels_annotation, prediction_segments)
         purity = purity_score(labels_annotation, prediction_segments)
         if (coverage+purity != 0):
             coverage_purity_f1 = 2 * coverage * purity / (coverage + purity)
         else:
             coverage_purity_f1 = NaN
         evaluation_df[speaker_change_col] = [precision, recall, precision_recall_f1, coverage, purity,
                                              coverage_purity_f1]
     return evaluation_df
 
-
+# Test Codes
+# prediction_output_path = '/Users/jf3375/Downloads'
+# labelled_data_path = '/Users/jf3375/Desktop/evaluation_data/VoxConverse/test_csv'
+# csv_filename = 'rmvsh.csv'
+# tolerance = 0
+# evaluation_df, prediction_df, labelled_df, labels_annotation, prediction_segments = calculate_detection_metrics(prediction_output_path, labelled_data_path, csv_filename, tolerance=0.5)
+#
+# coverage_score = SegmentationCoverage(tolerance=tolerance)
+# purity_score = SegmentationPurity(tolerance=tolerance)
+# precision_score = SegmentationPrecision(tolerance=tolerance)
+# recall_score = SegmentationRecall(tolerance=tolerance)
+#
+# print(precision_score(labels_annotation, prediction_segments))
+# print(recall_score(labels_annotation, prediction_segments))
+# print(coverage_score(labels_annotation, prediction_segments))
+# print(purity_score(labels_annotation, prediction_segments))
```

## Comparing `speechmlpipeline-0.0.1.dist-info/LICENSE` & `speechmlpipeline-1.0.0.dist-info/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Junying Fang
+Copyright (c) 2024 The Trustees of Princeton University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `speechmlpipeline-0.0.1.dist-info/METADATA` & `speechmlpipeline-1.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: speechmlpipeline
-Version: 0.0.1
+Version: 1.0.0
 Summary: A package of speech machine learning pipeline to automatically get transcriptions with speaker labels from audio inputs
 Author-email: "Junying (Alice) Fang" <jf3375@princeton.edu>
 Project-URL: Homepage, https://github.com/princeton-ddss/SpeechMLPipeline
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Provides-Extra: docs
 Requires-Dist: myst-parser ; extra == 'docs'
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme ; extra == 'docs'
 
-[![DOI](https://zenodo.org/badge/736356201.svg)](https://zenodo.org/doi/10.5281/zenodo.10436874)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10712894.svg)](https://doi.org/10.5281/zenodo.10712894)
 
 ## SpeechMLPipeline #
 [**SpeechMLPipeline**](https://github.com/princeton-ddss/SpeechMLPipeline) is a Python package for users to run the complete speech machine learning pipeline via one simple function
-(Audio-to-Text Transcription, Speaker Change Detection, and Speaker Identification) to get 
-transcriptions with speaker labels from input audio files. SpeechMLPipeline applys and implements the most widely used and the innovative machine learning
+to get transcriptions with speaker labels from input audio files. SpeechMLPipeline applys and implements the most widely used and the innovative machine learning
 models at each step of the pipeline:
- * Audio-to-Text Transcription: [OpenAI Whisper with timestamp adjustment](https://github.com/linto-ai/whisper-timestamped)
- * Speaker Change Detection: [PyAnnotate](https://huggingface.co/pyannote/speaker-diarization-3.1), [Audio-based Spectral Clustering Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection), [Text-based Llama2-70b Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection), [Rule-based NLP Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection), [Ensemble Audio-and-text-based Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection)
- * Speaker Detection: [Speechbrain](https://github.com/speechbrain/speechbrain)
+ * **Audio-to-Text Transcription**: [OpenAI Whisper with timestamp adjustment](https://github.com/linto-ai/whisper-timestamped)
+ * **Speaker Change Detection**: [PyAnnotate](https://huggingface.co/pyannote/speaker-diarization-3.1), [Audio-based Spectral Clustering Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection), [Text-based Llama2-70b Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection), [Rule-based NLP Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection), [Ensemble Audio-and-text-based Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection)
+ * **Speaker Identification**: [Speechbrain](https://github.com/speechbrain/speechbrain)
 
-The [OpenAI Whisper](https://github.com/linto-ai/whisper-timestamped) is selected for the Transcription as it is the most accurate model available for English transcription. The OpenAI Whisper with timestamp adjustment is used to reduce the
+**Audio-to-text Transcription**
+* The [OpenAI Whisper](https://github.com/linto-ai/whisper-timestamped) is selected for the audio-to-text transcription as it is the most accurate model available for English transcription. The OpenAI Whisper with timestamp adjustment is used to reduce the
 misalignment between the timestamps and the transcription texts by identifying the silence parts and predicting timestamps at the word level.
 
-The [PyAnnotate models](https://huggingface.co/pyannote/speaker-diarization-3.1) is by far one of the most popular models for speaker diarization. The speaker change detection results are directly inferred from speaker diarization results.
+**Speaker Change Detection**
+* The [PyAnnotate models](https://huggingface.co/pyannote/speaker-diarization-3.1) is by far one of the most popular models for speaker diarization. It detects speaker change by applying clustering methods based on audio features. The speaker change detection results are directly inferred from speaker diarization results.
 
-The [Audio-based Spectral Clustering Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is developed by extracting audio features from Librosa and applying spectral clustering to audio features. This model is one of the most common speaker change detection models used in academic research.
+* The [Audio-based Spectral Clustering Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is developed by extracting audio features from Librosa and applying spectral clustering to audio features. This model is one of the most common speaker change detection models used in academic research.
 
-The [Text-based Llama2-70b Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is developed by asking Llama2 if the speaker changes across two consecutive text segments by understanding the interrelationships between these two texts via their semantic meaning. 
+* The [Text-based Llama2-70b Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is an innovative speaker change detection model based on LLMs. It is developed by asking Llama2 if the speaker changes across two consecutive text segments by understanding the interrelationships between these two texts via their semantic meaning. 
 
-The [Rule-based NLP Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is applied to detect speaker change by analyzing text using well-defined rules developed by human comprehension. 
+* The [Rule-based NLP Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is applied to detect speaker change by analyzing text using well-defined rules developed by human comprehension. 
 
-The [Ensemble Audio-and-text-based Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is built by ensembling audio-based or text-based speaker change detection models. The voting methods are used to aggregate the predictions of the speaker change detection models above except for Rule-based NLP model.
+* The [Ensemble Audio-and-text-based Speaker Change Detection Model](https://github.com/princeton-ddss/AudioAndTextBasedSpeakerChangeDetection) is built by ensembling audio-based or text-based speaker change detection models. The voting methods are used to aggregate the predictions of the speaker change detection models above except for Rule-based NLP model.
 The aggregated predictions are then corrected by Rule-based NLP model.
 
-The [Speechbrain models](https://github.com/speechbrain/speechbrain) are used to perform the speaker identification by comparing the similarities between the vector embeddings of each input audio segment and labelled speakers audio segments.
+**Speaker Identification**
+* The [Speechbrain models](https://github.com/speechbrain/speechbrain) are used to perform the speaker identification by comparing the similarities between the vector embeddings of each input audio segment and labelled speakers audio segments.
 
 ## Create New Python Environment to Avoid Packages Versions Conflict If Needed
 ```
 python -m venv <envname>
 source <envname>/bin/activate
 ```
 
@@ -91,19 +93,24 @@
 download_models_main_function(<download_model_path>, <models_list>, <hf_access_token>)
 ```
 
 
 
 
 ## Usage
-The complete pipeline could be ran by using **run_speech_ml_pipeline** function.
+The complete pipeline could be run by using **run_speech_ml_pipeline** function.
 
-Please view the function and its inputs description inside the Python file **src/speechmlpipeline/main_pipeline_local_function.py**.
+Please view the sample codes to run the function in **sample_run.py** and **sample_run_existingllama2output.py** in the src/speechmlpipeline. 
 
-Please view the sample codes to run the function in **sample_run.py** and **sample_run_existingllama2output.py** in the src/speechmlpipeline.
+Specifically, detection_models in speakerchangedetection input could be set as a list or sublist of 
+['pyannote', 'clustering', 'nlp', 'llama2-70b']. Device in any inputs could be set as None or 'gpu' or 'cpu'. 
+If device is set as None, gpu would be used if it is available. Running llama2-70b requires at least 2 gpus and 250GB memory. 
+If the computing resources is not available for running llama2-70b, please exclude llama2-70b from detection_models input.
+
+Please view the detailed function description and its inputs description inside the Python file **src/speechmlpipeline/main_pipeline_local_function.py**.
 ```python
 from main_pipeline_local_function import TranscriptionInputs, SpeakerChangeDetectionInputs, 
     EnsembleDetectionInputs, SpeakerIdentificationInputs, run_speech_ml_pipeline
 
 # Run Whole Pipeline except for Downloading Models
 run_speech_ml_pipeline(transcription = <transcription_inputs>,
                        speakerchangedetection=<detection_inputs>, ensembledetection=<ensemble_detection_inputs>,
```

## Comparing `speechmlpipeline-0.0.1.dist-info/RECORD` & `speechmlpipeline-1.0.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 speechmlpipeline/DownloadModels/Download_Whisper_Model.py,sha256=rwjGOLFSvhWMB4ePd0feJRtNRLGx6rgySdhKoeVxV4s,376
 speechmlpipeline/DownloadModels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 speechmlpipeline/DownloadModels/download_models_main_function.py,sha256=FB0J1lVRUuelCiMBiqfRDZs9Tmnby8XrmOsGXO6sip0,1340
 speechmlpipeline/EnsembleSpeakerChangeDetection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 speechmlpipeline/EnsembleSpeakerChangeDetection/ensemble_detection.py,sha256=y1OnlUHendjc4mbW_VApB4DjibD83NC7yvbz5AiGpY4,1496
 speechmlpipeline/Evaluation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 speechmlpipeline/Evaluation/SpeakerChangeDetection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function.py,sha256=CVDXn6dE2t44_4fTko4BOnY34mKte0gVEPJbszR4z2o,5994
+speechmlpipeline/Evaluation/SpeakerChangeDetection/examine_pyannote_metrics.py,sha256=DYLP43JNUHW49tSLdNkeGIjh2IndHOPMD78ltaTXCBY,1845
+speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function.py,sha256=nkTilySGkMyuO_4Ej7UeOUwI3w40zE69-SuDbUX0okU,9970
+speechmlpipeline/Evaluation/SpeakerChangeDetection/metrics_main_function_revised.py,sha256=k4xDmVcqyrvzdyTjpdYiUdzDId1tSaAwTtPGsGiZRmI,1942
 speechmlpipeline/Helpers/helpers.py,sha256=Ri0zGq-cQAwyq0F_KP8kzGRbLHtIy3BD7aMv-V-syT4,1926
 speechmlpipeline/PreprocessData/Run_VideoAudioPreprocessing.py,sha256=llmQC4oQQm3v5w1DPb2MVJG7yS3wJP7T9gZMuyTh7V4,3694
 speechmlpipeline/PreprocessData/VideoAudioPreprocessing.py,sha256=U7w8Gr7y4FsWtQO-QQi8EmPO6j78CnnmT8B8H0opWQQ,5338
 speechmlpipeline/PreprocessData/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 speechmlpipeline/SpeakerChangeDetection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 speechmlpipeline/SpeakerChangeDetection/speaker_change_detection_main_function.py,sha256=5j_0h3ixauaPtHWaaly_2aSSawnqWFDQ2MzAllA-_Q0,3353
 speechmlpipeline/SpeakerIdentification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 speechmlpipeline/SpeakerIdentification/speaker_identification_main_function.py,sha256=QT9vooigD8mKSHYH3X_I9O6dHsRkhuijSkJb73aN6ic,6549
-speechmlpipeline-0.0.1.dist-info/LICENSE,sha256=qSmCJ6fMgc80WyVgYw1Q1JfhKBWK1peR9Jmmlzogaiw,1068
-speechmlpipeline-0.0.1.dist-info/METADATA,sha256=orrqnWe08ez605mRS3v9uEFZkZ7yOhFGZSEOMOnIbdc,7169
-speechmlpipeline-0.0.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-speechmlpipeline-0.0.1.dist-info/top_level.txt,sha256=4Kk8KkBAxPT_aAf2AwN4oMFOtorAwB1MqdFM-sd3sp0,17
-speechmlpipeline-0.0.1.dist-info/RECORD,,
+speechmlpipeline-1.0.0.dist-info/LICENSE,sha256=y0FxS72Yc01R5i36fN2g0JCldQzKCdCZ_H6h3RtttGw,1092
+speechmlpipeline-1.0.0.dist-info/METADATA,sha256=4YqdrOBAsQgVeTKXsDARxbdb2MW8C6ZFSrT7eJOs7l0,7861
+speechmlpipeline-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+speechmlpipeline-1.0.0.dist-info/top_level.txt,sha256=4Kk8KkBAxPT_aAf2AwN4oMFOtorAwB1MqdFM-sd3sp0,17
+speechmlpipeline-1.0.0.dist-info/RECORD,,
```

