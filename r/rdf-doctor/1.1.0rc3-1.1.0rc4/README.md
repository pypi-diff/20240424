# Comparing `tmp/rdf_doctor-1.1.0rc3-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.0rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59874 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 24-Apr-16 02:41 doctor/__init__.py
+Zip file size: 59856 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-22 07:45 doctor/__init__.py
 -rw-r--r--  2.0 unx     1754 b- defN 24-Mar-29 08:43 doctor/consts.py
--rw-r--r--  2.0 unx    81777 b- defN 24-Apr-16 02:29 doctor/doctor.py
--rw-r--r--  2.0 unx   134314 b- defN 24-Mar-12 04:38 doctor/reference/prefixes.tsv
+-rw-r--r--  2.0 unx    81750 b- defN 24-Apr-22 08:00 doctor/doctor.py
+-rw-r--r--  2.0 unx   134314 b- defN 24-Apr-22 02:03 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-Mar-06 07:08 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-Mar-06 07:13 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/LICENSE
--rw-r--r--  2.0 unx    10653 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-16 04:24 rdf_doctor-1.1.0rc3.dist-info/RECORD
-12 files, 231415 bytes uncompressed, 58158 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10653 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/RECORD
+12 files, 231388 bytes uncompressed, 58140 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc3.dist-info/LICENSE
+Filename: rdf_doctor-1.1.0rc4.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc3.dist-info/METADATA
+Filename: rdf_doctor-1.1.0rc4.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc3.dist-info/WHEEL
+Filename: rdf_doctor-1.1.0rc4.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc3.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.0rc4.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc3.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.0rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc3.dist-info/RECORD
+Filename: rdf_doctor-1.1.0rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0rc3"
+__version__ = "1.1.0rc4"
```

## doctor/doctor.py

```diff
@@ -49,18 +49,14 @@
             # Retrieve input files in dictionary format by type
             input_file_2d_list, exists_file_types, error_msg = get_input_files_by_type(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
             if error_msg is not None:
                 print(error_msg)
                 return
 
         else:
-            # if args.output is None:
-            #     print("The --each option should be used with the --output option.")
-            #     return
-
             # Get an array containing each file to be processed
             # Acquire as a two-dimensional array for compatibility with subsequent processing
             input_file_2d_list, exists_file_types, error_msg = get_input_files_each(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
             if error_msg is not None:
                 print(error_msg)
                 return
 
@@ -70,105 +66,72 @@
             else:
                 target_file_types = args.type.split(",")
         else:
             target_file_types = get_target_file_types(exists_file_types)
 
         for input_file_list in input_file_2d_list:
             if is_target_file(input_file_list, target_file_types):
-                error_msg = validate_command_line_args_input(args, input_file_list[0])
+                error_msg = validate_command_line_args_input(input_file_list[0])
                 if error_msg is not None:
                     print(error_msg)
                     return
 
-        result_queue = queue.Queue()
+        error_queue = queue.Queue()
         executor_calc = ThreadPoolExecutor(max_workers=multiprocessing.cpu_count())
         executor_spinner = ThreadPoolExecutor(max_workers=multiprocessing.cpu_count())
 
         global is_displaying_spinner
         if args.verbose:
             is_displaying_spinner = True
             executor_spinner.submit(display_spinner)
 
         try:
+            widely_used_prefixes_dict = get_widely_used_prefixes_dict(args.prefix_list)
+
             for input_file_list in input_file_2d_list:
                 if is_target_file(input_file_list, target_file_types) == False:
                     continue
 
                 compression_mode = input_file_list[1]
-                input_format = input_file_list[2]
+                if args.force_format is not None:
+                    input_format = args.force_format
+                else:
+                    input_format = input_file_list[2]
 
                 if args.verbose:
                     print_overwrite(get_dt_now() + " -- Start processing [" + ", ".join(str(input_file) for input_file in input_file_list[0]) + "]")
 
-                executor_calc.submit(get_shex_result, args, input_file_list[0], input_format, compression_mode, result_queue)
+                # Get and output result. If an error occurs, store it in a queue
+                executor_calc.submit(get_and_output_result, args, input_file_list[0], input_format, compression_mode, widely_used_prefixes_dict, error_queue)
 
             executor_calc.shutdown()
             if args.verbose:
                 is_displaying_spinner = False
                 executor_spinner.shutdown()
 
-            while not result_queue.empty():
-                result_output = result_queue.get()
-                if type(result_output) is list:
-                    # Normal case
-                    if args.output is None:
-                        # Standard output
-                        print_overwrite("".join(result_output[0]))
-
-                        if args.verbose:
-                            print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in result_output[1]) + "]")
-                    else:
-                        # Output to file
-                        if args.merge:
-                            # Output one result file for each type of file processed(Turtle, N-triples, and RDF/XML)
-                            # turtle.shex, nt.shex, rdf.shex
-                            if result_output[2] == TURTLE:
-                                output_file_name = TURTLE
-                            elif result_output[2] == NT:
-                                output_file_name = "n-triples"
-                            elif result_output[2] == RDF_XML:
-                                output_file_name = "rdf_xml"
-
-                            if result_output[3] is None:
-                                compression_exetention = ""
-                            else:
-                                compression_exetention = "." + result_output[3]
-
-                            with open(args.output + "/" + output_file_name + compression_exetention + ".shex", "w", encoding="utf-8") as f:
-                                f.write("".join(result_output[0]))
-
-                        else:
-                            with open(args.output + "/" + Path(result_output[1][0]).name + ".shex", "w", encoding="utf-8") as f:
-                                f.write("".join(result_output[0]))
-
-                        if args.verbose:
-                            print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in result_output[1]) + "] Output file: [" + str(Path(args.output + "/" + Path(result_output[1][0]).name)) + ".shex]")
-
-                elif type(result_output) in [ValueError, IndexError, MemoryError, Exception]:
-                    # Error case
-                    raise result_output
-
-                else:
-                    # Else case does not occur.
-                    raise Exception("An exception error has occurred. Not the expected processing result.")
+            # Output if there is an error
+            if not error_queue.empty():
+                print("Some files could not be processed successfully. Please check the following errors.")
+                while not error_queue.empty():
+                    print(error_queue.get())
 
         except ValueError as e:
-            print(e)
+            print("[ERROR] A value error occurred. Error message: " + str(e))
 
         except IndexError as e:
-            print(e)
+            print("[ERROR] An index error occurred. Error message: " + str(e))
 
         except MemoryError as e:
-            print(e)
+            print("[ERROR] A memory error occurred. Error message: " + str(e))
 
         except KeyboardInterrupt:
             print ("Keyboard interrupt occurred.")
 
         except Exception as e:
-            print(e)
+            print("[ERROR] An exception occurred. Error message: " + str(e))
 
         finally:
             is_displaying_spinner = False
             executor_calc.shutdown()
             executor_spinner.shutdown()
 
     return
@@ -290,25 +253,25 @@
 
     return parser.parse_args(args)
 
 
 # Returns a two-dimensional array of input file array, compression mode, and input format
 # One element of the two-dimensional array is configured for each compression mode and input format.
 # example
-# {
-#     ttl: [["test1.ttl", "test2.ttl", "test3.ttl"], None, "turtle"]
-#     nt: [["test4.nt", "test5.nt", "test6.nt"], None, "nt"],
-#     rdf_xml: [["test7.rdf", "test8.xml", "test9.owl"], None, "xml"],
-#     ttl_gz: [["test10.ttl.gz", "test11.ttl.gz", "test12.ttl.gz"], "gz", "turtle"]
-#     nt_gz: [["test13.nt.gz", "test14.nt.gz", "test15.nt.gz"], gz, "nt"],
-#     rdf_xml_gz: [["test16.rdf.gz", "test17.xml.gz", "test18.owl.gz"], gz, "xml"],
-#     ttl_zip: [["test19.ttl.zip", "test20.ttl.zip", "test21.ttl.zip"], zip, "turtle"]
-#     nt_zip: [["test22.nt.zip", "test23.nt.zip", "test24.nt.zip"], zip, "nt"],
-#     rdf_xml_zip: [["test25.rdf.zip", "test26.xml.zip", "test27.owl.zip"], zip, "xml"]
-# }
+# [
+#     [["test1.ttl", "test2.ttl", "test3.ttl"], None, "turtle"]
+#     [["test4.nt", "test5.nt", "test6.nt"], None, "nt"],
+#     [["test7.rdf", "test8.xml", "test9.owl"], None, "xml"],
+#     [["test10.ttl.gz", "test11.ttl.gz", "test12.ttl.gz"], "gz", "turtle"]
+#     [["test13.nt.gz", "test14.nt.gz", "test15.nt.gz"], "gz", "nt"],
+#     [["test16.rdf.gz", "test17.xml.gz", "test18.owl.gz"], "gz", "xml"],
+#     [["test19.ttl.zip", "test20.ttl.zip", "test21.ttl.zip"], "zip", "turtle"]
+#     [["test22.nt.zip", "test23.nt.zip", "test24.nt.zip"], "zip", "nt"],
+#     [["test25.rdf.zip", "test26.xml.zip", "test27.owl.zip"], "zip", "xml"]
+# ]
 def get_input_files_by_type(input_files, temp_dir, tmp_dir_disk_usage_limit):
 
     input_file_list_ttl = []            # Turtle(.ttl)
     input_file_list_nt = []             # N-Triples(.nt)
     input_file_list_rdf_xml = []        # RDF/XML(.rdf, .xml, .owl)
     input_file_list_ttl_gz = []         # GZ compressed Turtle(.ttl.gz)
     input_file_list_nt_gz = []          # GZ compressed N-Triples(.nt.gz)
@@ -549,26 +512,26 @@
     return input_file_2d_list, exists_file_types, None
 
 
 # Get an array containing each file to be processed
 # Acquire as a two-dimensional array for compatibility with subsequent processing.
 # example
 # [
-#     ["test1.ttl", None, "turtle"],
-#     ["test2.ttl", None, "turtle"],
-#     ["test3.ttl", None, "turtle"],
-#     ["test4.ttl.gz", "gz", "turtle"],
-#     ["test5.nt", None, "nt"],
-#     ["test6.nt", None, "nt"],
-#     ["test7.nt", None, "nt"],
-#     ["test8.nt.gz", "gz", "nt"],
-#     ["test9.rdf", None, "xml"],
-#     ["test10.xml", None, "xml"],
-#     ["test11.owl", None, "xml"],
-#     ["test12.rdf.zip", "zip", "xml"]
+#     [["test1.ttl"], None, "turtle"],
+#     [["test2.ttl"], None, "turtle"],
+#     [["test3.ttl"], None, "turtle"],
+#     [["test4.ttl.gz"], "gz", "turtle"],
+#     [["test5.nt"], None, "nt"],
+#     [["test6.nt"], None, "nt"],
+#     [["test7.nt"], None, "nt"],
+#     [["test8.nt.gz"], "gz", "nt"],
+#     [["test9.rdf"], None, "xml"],
+#     [["test10.xml"], None, "xml"],
+#     [["test11.owl"], None, "xml"],
+#     [["test12.rdf.zip"], "zip", "xml"]
 # ]
 def get_input_files_each(input_files, temp_dir, tmp_dir_disk_usage_limit):
 
     input_file_2d_list = []
     exists_file_types = []
 
     for input_file in input_files:
@@ -726,15 +689,15 @@
         # RDF/XML(.owl、.rdf、.xml)
         return RDF_XML
     else:
         return None
 
 
 # Validate args(input)
-def validate_command_line_args_input(args, input_file_list):
+def validate_command_line_args_input(input_file_list):
     compression_mode = ""
     input_format = ""
     for input_file in input_file_list:
         if input_file is None:
             # This case does not occur because -i / --input is required as an option when parsing command line arguments.
             error_msg = "Input file error: No input file specified. (-i [RDF_FILE], --input [RDF_FILE])"
             return error_msg
@@ -874,43 +837,44 @@
     if args.tmp_dir_disk_usage_limit < 1 or args.tmp_dir_disk_usage_limit > 100:
         error_msg = "Temporary directory disk usage limit error: Please specify the upper limit of Disk containing temporary directory usage percentage as a number between 1 and 100."
         return error_msg
 
     return None
 
 
-# Processing when the report format is "shex"
-def get_shex_result(args, input_file_list, input_format, compression_mode, result_queue):
+# Retrieve processing results and store them in a queue
+def get_and_output_result(args, input_file_list, input_format, compression_mode, widely_used_prefixes_dict, error_queue):
 
     try:
-        widely_used_prefixes_dict = get_widely_used_prefixes_dict(args.prefix_list)
-
         # Get Prefix when input file is turtle format
         if input_format == NT:
             input_prefixes = []
             duplicated_prefixes = []
             namespaces_dict = get_default_namespaces_dict()
         else:
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Getting prefixes from input file... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             if input_format == TURTLE:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_turtle(input_file_list, compression_mode)
             elif input_format == RDF_XML:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_rdf_xml(input_file_list, compression_mode)
             else:
-                raise ValueError('Invalid input format: ' + str(input_format))
+                raise ValueError("Invalid input format: " + str(input_format))
 
             namespaces_dict = get_namespaces_dict(input_prefixes, duplicated_prefixes_dict, widely_used_prefixes_dict)
 
         shaper_result = get_shaper_result(args, input_file_list, input_format, compression_mode, namespaces_dict)
 
         report_result = []
         # Output only if report output option is specified
         if args.report:
+            refine_prefix_uris = get_refine_prefix_uris(args.prefix_uri_dict)
+            refine_class_uris = get_refine_class_uris(args.class_uri_dict)
+
             # Prefixes with the same Namespace but different URIs at the same time
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_duplicated_prefixes = []
             if len(duplicated_prefixes) != 0:
                 result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
@@ -921,15 +885,15 @@
                 result_duplicated_prefixes.append("# \n# \n")
 
             # Suggest Namespace based on URI of validation expression output by sheXer and prefixes.tsv
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Creating suggestions for Namespace... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_widely_used_namespace_and_uri = []
-            widely_used_namespace_and_uri = get_widely_used_namespace_and_uri_result(shaper_result, input_prefixes, widely_used_prefixes_dict, args.prefix_uri_dict)
+            widely_used_namespace_and_uri = get_widely_used_namespace_and_uri_result(shaper_result, input_prefixes, widely_used_prefixes_dict, refine_prefix_uris)
             if len(widely_used_namespace_and_uri) != 0:
                 result_widely_used_namespace_and_uri.append("# There is a more widely used Namespace and URI.\n")
                 result_widely_used_namespace_and_uri.append("# (For each of Namespace and URI, output only if the input value differs from the widely used value.)\n")
                 # When prefix list is explicitly specified
                 if args.prefix_list != str(Path(__file__).resolve().parent.joinpath(PREFIXES_FILE_PATH)):
                     result_widely_used_namespace_and_uri.append("# Using a customized prefix list. (" + args.prefix_list + ")\n")
                 # When prefix URI dictionary is explicitly specified
@@ -966,15 +930,15 @@
 
             # Refers to the class URIs dictionary, acquires the list for result output that candidate pairs of URI rewrite source and rewrite destinations,
             # and generate the class corresponding to each key in fingerprint format stored in dictionary format.
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_refine_class_uris = []
-            class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_uri_dict)
+            class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, refine_class_uris)
             # When there is data to output
             if len(class_comparison_result) != 0:
                 result_refine_class_uris.append("# Found a more widely used one for the class URI inputed.\n")
                 # When class URI dictionary is explicitly specified
                 if args.class_uri_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)):
                     result_refine_class_uris.append("# Using a customized class URI dictionary. (" + args.class_uri_dict + ")\n")
 
@@ -1032,27 +996,59 @@
         # List for storing the final result
         shex_final_result = []
         shex_final_result.extend(shaper_result)
 
         if len(report_result) != 0:
             shex_final_result.extend(report_result)
 
-        result_queue.put([shex_final_result, input_file_list, input_format, compression_mode])
+        # Output results
+        if args.output is None:
+            # Standard output
+            print_overwrite("".join(shex_final_result))
+
+            if args.verbose:
+                print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
+        else:
+            # Output to file
+            if args.merge:
+                # Output one result file for each type of file processed(Turtle, N-triples, and RDF/XML)
+                # turtle.shex, nt.shex, rdf.shex
+                if input_format == TURTLE:
+                    output_file_name = TURTLE
+                elif input_format == NT:
+                    output_file_name = "n-triples"
+                elif input_format == RDF_XML:
+                    output_file_name = "rdf_xml"
+
+                if compression_mode is None:
+                    compression_exetention = ""
+                else:
+                    compression_exetention = "." + compression_mode
+
+                with open(args.output + "/" + output_file_name + compression_exetention + ".shex", "w", encoding="utf-8") as f:
+                    f.write("".join(shex_final_result))
+
+            else:
+                with open(args.output + "/" + Path(input_file_list[0]).name + ".shex", "w", encoding="utf-8") as f:
+                    f.write("".join(shex_final_result))
+
+            if args.verbose:
+                print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in input_file_list) + "] Output file: [" + str(Path(args.output + "/" + Path(input_file_list[0]).name)) + ".shex]")
 
     except ValueError as e:
-        result_queue.put(ValueError('A value error has occurred.\n\nValueError message: ' + str(e)))
+        error_queue.put(ValueError("[ERROR] A value error occurred while processing [" + ", ".join(str(input_file) for input_file in input_file_list) + "] Error message: " + str(e)))
 
     except IndexError as e:
-        result_queue.put(IndexError('An index error has occurred.\n\nIndexError message: ' + str(e)))
+        error_queue.put(IndexError("[ERROR] An index error occurred while processing [" + ", ".join(str(input_file) for input_file in input_file_list) + "] Error message: " + str(e)))
 
     except MemoryError as e:
-        result_queue.put(MemoryError('A memory error has occurred.\n\nMemoryError message: ' + str(e)))
+        error_queue.put(MemoryError("[ERROR] A memory error occurred while processing [" + ", ".join(str(input_file) for input_file in input_file_list) + "] Error message: " + str(e)))
 
     except Exception as e:
-        result_queue.put(Exception('An exception error has occurred.\n\nException message: ' + str(e)))
+        error_queue.put(Exception("[ERROR] An exception occurred while processing [" + ", ".join(str(input_file) for input_file in input_file_list) + "] Error message: " + str(e)))
 
 
 # Call the shex_graph method of shexer's shaper class and output the result
 def get_shaper_result(args, input_file_list, input_format, compression_mode, namespaces_dict):
     # Set parameters when calling the shaper class depending on whether the class is specified as an argument
     if TARGET_CLASS_ALL in args.classes:
         target_classes = None
@@ -1131,15 +1127,15 @@
         if TARGET_CLASS_ALL not in target_classes:
             query += " FILTER (?class_name IN (" + class_filter + "))"
 
         query += """
             }
         """
 
-        # Correspondence for not executing query methods in parallel, since calling them in parallel will result in an error. -----
+        # INFO: Correspondence for not executing query methods in parallel, since calling them in parallel will result in an error. -----
         global in_progress_rdflib_query
         while in_progress_rdflib_query == True:
             time.sleep(0.01)
         in_progress_rdflib_query = True
         qres = g.query(query)
         in_progress_rdflib_query = False
         # -------------------------------------------------------------------------------------------------------------------------
@@ -1169,16 +1165,15 @@
 
     return refine_prefix_uris
 
 
 # Get a list of candidate pairs of URI rewrite source and rewrite destination by referencing the class URLs dictionary.
 # Create a dictionary with a class corresponding to each key in the stored fingerprint format.
 # Return the two.
-def get_class_comparison_result(input_classes, refine_class_uris_file):
-    refine_class_uris = get_refine_class_uris(refine_class_uris_file)
+def get_class_comparison_result(input_classes, refine_class_uris):
     class_comparison_result = []
     fingerprint_class_dict = defaultdict(list)
     # Perform clustering by fingerprint for the acquired class name
     for input_class in input_classes:
         fingerprint_class_dict[fingerprint(input_class)].append(input_class)
         for refine_class_uri in refine_class_uris:
             if input_class == refine_class_uri[0]:
@@ -1331,15 +1326,15 @@
         widely_used_prefixes_dict = {rows[0]: rows[1] for rows in tsv_reader}
 
     return widely_used_prefixes_dict
 
 
 # Compare the URI of the validation expression in the shexer output with the URI of the prepared prefix list
 # and get the matching Namespace from the prefix list
-def get_widely_used_namespace_and_uri_result(shaper_result, input_prefixes, widely_used_prefixes_dict, refine_prefix_uris_file):
+def get_widely_used_namespace_and_uri_result(shaper_result, input_prefixes, widely_used_prefixes_dict, refine_prefix_uris):
     widely_used_namespace_and_uri_result = []
 
     # Comparison of prefix list and minimal URI detected by shaXer
     for line in shaper_result.splitlines():
         if ("[<http" in line and ">~]" in line):
             shaper_result_uri = line[line.find("[<http")+2:line.find(">~]")]
 
@@ -1348,27 +1343,27 @@
             input_namespace = "Undefined"
             for input_prefix in input_prefixes:
                 if shaper_result_uri == input_prefix[1]:
                     input_namespace = input_prefix[0]
                     break
 
             # Obtain namespaces and URIs to suggest, formatting them for output
-            suggest_string = get_suggest_string_for_widely_used_namespace_and_uri(input_namespace, shaper_result_uri, widely_used_prefixes_dict, refine_prefix_uris_file)
+            suggest_string = get_suggest_string_for_widely_used_namespace_and_uri(input_namespace, shaper_result_uri, widely_used_prefixes_dict, refine_prefix_uris)
 
             # If the string for the suggestion you got exists and is not yet included in the results
             if suggest_string not in widely_used_namespace_and_uri_result and len(suggest_string) > 0:
                     widely_used_namespace_and_uri_result.append(suggest_string)
 
     # Comparing of prefix list and prefixes in input file
     for input_prefix in input_prefixes:
         input_namespace = input_prefix[0]
         input_uri = input_prefix[1]
 
         # Obtain namespaces and URIs to suggest, formatting them for output
-        suggest_string = get_suggest_string_for_widely_used_namespace_and_uri(input_namespace, input_uri, widely_used_prefixes_dict, refine_prefix_uris_file)
+        suggest_string = get_suggest_string_for_widely_used_namespace_and_uri(input_namespace, input_uri, widely_used_prefixes_dict, refine_prefix_uris)
 
         # If the string for the suggestion you got exists and is not yet included in the results
         if suggest_string not in widely_used_namespace_and_uri_result and len(suggest_string) > 0:
             widely_used_namespace_and_uri_result.append(suggest_string)
 
     return widely_used_namespace_and_uri_result
 
@@ -1525,20 +1520,18 @@
             # Since the namespace is unique, it ends when it is found.
             return value
 
     return None
 
 
 # Obtain namespaces and URIs to suggest, formatting them for output
-def get_suggest_string_for_widely_used_namespace_and_uri(input_namespace, input_uri, widely_used_prefixes_dict, refine_prefix_uris_file):
+def get_suggest_string_for_widely_used_namespace_and_uri(input_namespace, input_uri, widely_used_prefixes_dict, refine_prefix_uris):
     suggest_string = input_namespace + "\t" + input_uri + "\t"
     exists_suggest = False
 
-    refine_prefix_uris = get_refine_prefix_uris(refine_prefix_uris_file)
-
     # Obtain the corresponding namespace in the list obtained from prefixes.tsv using the URI as a key
     widely_used_namespaces = get_widely_used_namespace_by_uri(input_uri, widely_used_prefixes_dict)
 
     # Output only if input values differ from widely used values
     if len(widely_used_namespaces) > 0:
         match = False
         for widely_used_namespace in widely_used_namespaces:
```

## Comparing `rdf_doctor-1.1.0rc3.dist-info/LICENSE` & `rdf_doctor-1.1.0rc4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.0rc3.dist-info/METADATA` & `rdf_doctor-1.1.0rc4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.0rc3
+Version: 1.1.0rc4
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `rdf_doctor-1.1.0rc3.dist-info/RECORD` & `rdf_doctor-1.1.0rc4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=cL9JVkp_7v5vXYtfMPakVSDg98hX-MyIO3n3MYdTdYI,25
+doctor/__init__.py,sha256=32Meqsm5YR_P22z_CrU4AwgcEOSCbBQilu6L6eQD7w8,25
 doctor/consts.py,sha256=U8KOzdPFgMuf_nMul1Vw9qtAvKtZbu8WLwkiYD49IAs,1754
-doctor/doctor.py,sha256=YQhN_-SN5efT5E9-S0LikSFiREf52Fg_lAsA25h6twY,81777
+doctor/doctor.py,sha256=hBYDHNmk8xQ3E1emVWjZOuaeDkJRYt9GTH_x82bXBaE,81750
 doctor/reference/prefixes.tsv,sha256=_1hW0wBl6K1YvcM8stdiEdD4elzST_ecJqQEvhD9Auk,134314
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.1.0rc3.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.1.0rc3.dist-info/METADATA,sha256=EmzWBa2kTqF4zsvQdoHYiu5UiceT-fQhFDL8qKlO7Kw,10653
-rdf_doctor-1.1.0rc3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-1.1.0rc3.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.1.0rc3.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.1.0rc3.dist-info/RECORD,,
+rdf_doctor-1.1.0rc4.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.1.0rc4.dist-info/METADATA,sha256=p2agE6jqOBMOQhX1yyFb02ZOc2nKI66Y-cCdx-F-iUc,10653
+rdf_doctor-1.1.0rc4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-1.1.0rc4.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.1.0rc4.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.1.0rc4.dist-info/RECORD,,
```

