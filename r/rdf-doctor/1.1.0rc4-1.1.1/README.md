# Comparing `tmp/rdf_doctor-1.1.0rc4-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59856 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 24-Apr-22 07:45 doctor/__init__.py
--rw-r--r--  2.0 unx     1754 b- defN 24-Mar-29 08:43 doctor/consts.py
--rw-r--r--  2.0 unx    81750 b- defN 24-Apr-22 08:00 doctor/doctor.py
--rw-r--r--  2.0 unx   134314 b- defN 24-Apr-22 02:03 doctor/reference/prefixes.tsv
+Zip file size: 59877 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-25 04:53 doctor/__init__.py
+-rw-r--r--  2.0 unx     1754 b- defN 24-Apr-24 04:07 doctor/consts.py
+-rw-r--r--  2.0 unx    81134 b- defN 24-Apr-25 04:53 doctor/doctor.py
+-rw-r--r--  2.0 unx   134314 b- defN 24-Apr-24 04:07 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-Mar-06 07:08 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-Mar-06 07:13 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/LICENSE
--rw-r--r--  2.0 unx    10653 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-22 08:02 rdf_doctor-1.1.0rc4.dist-info/RECORD
-12 files, 231388 bytes uncompressed, 58140 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10665 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      995 b- defN 24-Apr-25 04:56 rdf_doctor-1.1.1.dist-info/RECORD
+12 files, 230763 bytes uncompressed, 58197 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc4.dist-info/LICENSE
+Filename: rdf_doctor-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc4.dist-info/METADATA
+Filename: rdf_doctor-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc4.dist-info/WHEEL
+Filename: rdf_doctor-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc4.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc4.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc4.dist-info/RECORD
+Filename: rdf_doctor-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0rc4"
+__version__ = "1.1.1"
```

## doctor/doctor.py

```diff
@@ -22,15 +22,15 @@
 from doctor.consts import VERSION_FILE, TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, \
                             EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL, EXTENSION_GZ, EXTENSION_ZIP, EXTENSION_TAR_GZ, \
                             PREFIXES_FILE_PATH, REFINE_CLASS_URIS_FILE_PATH, REFINE_PREFIX_URIS_FILE_PATH, HELP_LINK_URL, \
                             FILE_TYPE_TTL, FILE_TYPE_NT, FILE_TYPE_RDF_XML, FILE_TYPE_TTL_GZ, FILE_TYPE_NT_GZ, FILE_TYPE_RDF_XML_GZ, \
                             FILE_TYPE_TTL_ZIP, FILE_TYPE_NT_ZIP, FILE_TYPE_RDF_XML_ZIP, FILE_TYPE_ALL, FILE_TYPE_DICT, TMP_DISK_USAGE_LIMIT_DEFAULT
 
 from shexer.shaper import Shaper
-from shexer.consts import NT, TURTLE, RDF_XML, GZ, ZIP, MIXED_INSTANCES
+from shexer.consts import NT, TURTLE, TURTLE_ITER, RDF_XML, GZ, ZIP, MIXED_INSTANCES
 
 is_displaying_spinner = False
 in_progress_rdflib_query = False
 
 # Main processing of rdf-doctor
 def doctor():
     args = get_command_line_args(sys.argv[1:])
@@ -81,15 +81,23 @@
 
         global is_displaying_spinner
         if args.verbose:
             is_displaying_spinner = True
             executor_spinner.submit(display_spinner)
 
         try:
+            # Obtaining the contents of various reference files
             widely_used_prefixes_dict = get_widely_used_prefixes_dict(args.prefix_list)
+            if args.report:
+                refine_prefix_uris = get_refine_prefix_uris(args.prefix_uri_dict)
+                refine_class_uris = get_refine_class_uris(args.class_uri_dict)
+            else:
+                # Not used if -r option is not specified
+                refine_prefix_uris = None
+                refine_class_uris = None
 
             for input_file_list in input_file_2d_list:
                 if is_target_file(input_file_list, target_file_types) == False:
                     continue
 
                 compression_mode = input_file_list[1]
                 if args.force_format is not None:
@@ -97,15 +105,15 @@
                 else:
                     input_format = input_file_list[2]
 
                 if args.verbose:
                     print_overwrite(get_dt_now() + " -- Start processing [" + ", ".join(str(input_file) for input_file in input_file_list[0]) + "]")
 
                 # Get and output result. If an error occurs, store it in a queue
-                executor_calc.submit(get_and_output_result, args, input_file_list[0], input_format, compression_mode, widely_used_prefixes_dict, error_queue)
+                executor_calc.submit(get_and_output_result, args, input_file_list[0], input_format, compression_mode, widely_used_prefixes_dict, refine_prefix_uris, refine_class_uris, error_queue)
 
             executor_calc.shutdown()
             if args.verbose:
                 is_displaying_spinner = False
                 executor_spinner.shutdown()
 
             # Output if there is an error
@@ -244,15 +252,15 @@
     parser.add_argument("--prefix-list", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(PREFIXES_FILE_PATH)),
                         help="list of prefixes (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv)",
                         metavar="FILE")
 
     # input format (--force-format [INPUT_FORMAT]、default: Standard output)
     parser.add_argument("--force-format", type=str,
-                        help='This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle", "nt" and "xml"(=RDF/XML) can be specified.',
+                        help='This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle", "turtle_iter", "nt" and "xml"(=RDF/XML) can be specified.',
                         metavar="INPUT-FORMAT")
 
     return parser.parse_args(args)
 
 
 # Returns a two-dimensional array of input file array, compression mode, and input format
 # One element of the two-dimensional array is configured for each compression mode and input format.
@@ -545,36 +553,28 @@
             for root, _, files in os.walk(top=input_file):
                 for file in files:
                     file_path = Path(root) / file
                     compression_mode = get_compression_mode(file_path)
                     input_format = get_input_format(file_path, compression_mode)
 
                     # Determine file type and add to array
-                    if input_format == TURTLE:
-                        input_file_2d_list.append([[file_path], compression_mode, TURTLE])
-                    elif input_format == NT:
-                        input_file_2d_list.append([[file_path], compression_mode, NT])
-                    elif input_format == RDF_XML:
-                        input_file_2d_list.append([[file_path], compression_mode, RDF_XML])
+                    if input_format in (TURTLE, NT, RDF_XML):
+                        input_file_2d_list.append([[file_path], compression_mode, input_format])
                     else:
                         # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
                         pass
 
         else:
             # Files with the following extensions are supported: .ttl, .nt, .rdf, .xml, and .owl.
             # However, other files are also added to the list for input checking.
             compression_mode = get_compression_mode(input_file)
             input_format = get_input_format(input_file, compression_mode)
 
-            if input_format == TURTLE:
-                input_file_2d_list.append([[input_file], compression_mode, TURTLE])
-            elif input_format == NT:
-                input_file_2d_list.append([[input_file], compression_mode, NT])
-            elif input_format == RDF_XML:
-                input_file_2d_list.append([[input_file], compression_mode, RDF_XML])
+            if input_format in (TURTLE, NT, RDF_XML):
+                input_file_2d_list.append([[input_file], compression_mode, input_format])
             else:
                 # Case None
                 if compression_mode is None:
                     extension = get_extension(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
 
@@ -592,20 +592,16 @@
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
                         for file in files:
                             file_path = Path(root) / file
                             # Determine file type and add to array
                             compression_mode = get_compression_mode(file_path)
                             input_format = get_input_format(file_path, compression_mode)
-                            if input_format == TURTLE:
-                                input_file_2d_list.append([[file_path], compression_mode, TURTLE])
-                            elif input_format == NT:
-                                input_file_2d_list.append([[file_path], compression_mode, NT])
-                            elif input_format == RDF_XML:
-                                input_file_2d_list.append([[file_path], compression_mode, RDF_XML])
+                            if input_format in (TURTLE, NT, RDF_XML):
+                                input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
                                 # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
                                 pass
 
                 elif extension == EXTENSION_ZIP:
                     # Check disk usage percentage
                     if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
@@ -619,20 +615,16 @@
 
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
                         for file in files:
                             file_path = Path(root) / file
                             compression_mode = get_compression_mode(file_path)
                             input_format = get_input_format(file_path, compression_mode)
-                            if input_format == TURTLE:
-                                input_file_2d_list.append([[file_path], compression_mode, TURTLE])
-                            elif input_format == NT:
-                                input_file_2d_list.append([[file_path], compression_mode, NT])
-                            elif input_format == RDF_XML:
-                                input_file_2d_list.append([[file_path], compression_mode, RDF_XML])
+                            if input_format in (TURTLE, NT, RDF_XML):
+                                input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
                                 # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
                                 pass
                 else:
                     error_msg = '"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                     return None, None, error_msg
 
@@ -767,16 +759,16 @@
     if TARGET_CLASS_ALL in args.classes:
         if len(args.classes) != 1:
             error_msg = 'Target class error: If "all" is specified, other classes cannot be specified.'
             return error_msg
 
     # Input Format only allows "turtle" or "nt" or "xml"
     if args.force_format is not None:
-        if args.force_format not in [TURTLE, NT, RDF_XML]:
-            error_msg = 'Input format error: "' + args.force_format + '" is an unsupported input format. "' + TURTLE + '", "' + NT + '" and "' + RDF_XML + '"(=RDF/XML) are supported.'
+        if args.force_format not in [TURTLE, TURTLE_ITER, NT, RDF_XML]:
+            error_msg = 'Input format error: "' + args.force_format + '" is an unsupported input format. "' + TURTLE + '", "' + TURTLE_ITER + '", "' + NT + '" and "' + RDF_XML + '"(=RDF/XML) are supported.'
             return error_msg
 
     if Path(args.prefix_uri_dict).is_file() == False:
         error_msg = "Prefix URIs dictionary file error: Prefix dictionary does not exist or you don't have read permission."
         return error_msg
 
     # Check if the file has read permission
@@ -838,43 +830,40 @@
         error_msg = "Temporary directory disk usage limit error: Please specify the upper limit of Disk containing temporary directory usage percentage as a number between 1 and 100."
         return error_msg
 
     return None
 
 
 # Retrieve processing results and store them in a queue
-def get_and_output_result(args, input_file_list, input_format, compression_mode, widely_used_prefixes_dict, error_queue):
+def get_and_output_result(args, input_file_list, input_format, compression_mode, widely_used_prefixes_dict, refine_prefix_uris, refine_class_uris, error_queue):
 
     try:
         # Get Prefix when input file is turtle format
         if input_format == NT:
             input_prefixes = []
             duplicated_prefixes = []
             namespaces_dict = get_default_namespaces_dict()
         else:
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Getting prefixes from input file... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
-            if input_format == TURTLE:
+            if input_format in (TURTLE, TURTLE_ITER):
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_turtle(input_file_list, compression_mode)
             elif input_format == RDF_XML:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_rdf_xml(input_file_list, compression_mode)
             else:
                 raise ValueError("Invalid input format: " + str(input_format))
 
             namespaces_dict = get_namespaces_dict(input_prefixes, duplicated_prefixes_dict, widely_used_prefixes_dict)
 
         shaper_result = get_shaper_result(args, input_file_list, input_format, compression_mode, namespaces_dict)
 
         report_result = []
         # Output only if report output option is specified
         if args.report:
-            refine_prefix_uris = get_refine_prefix_uris(args.prefix_uri_dict)
-            refine_class_uris = get_refine_class_uris(args.class_uri_dict)
-
             # Prefixes with the same Namespace but different URIs at the same time
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_duplicated_prefixes = []
             if len(duplicated_prefixes) != 0:
                 result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
@@ -946,15 +935,15 @@
                 result_refine_class_uris.append("# Input-class-URI\tSuggested-class-URI\n")
                 result_refine_class_uris.extend(["# " + s for s in class_comparison_result])
                 result_refine_class_uris.append("# ```\n")
                 result_refine_class_uris.append("# \n# \n")
 
             # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
             if args.verbose:
-                print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...[" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
+                print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             result_class_fingerprint = []
             fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
             # When there is data to output
             if len(fingerprint_comparison_result) != 0:
                 result_class_fingerprint.append("# Found multiple strings that appear to represent the same class.\n")
                 result_class_fingerprint.append("# ```\n# ")
@@ -1008,15 +997,15 @@
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Done! [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
         else:
             # Output to file
             if args.merge:
                 # Output one result file for each type of file processed(Turtle, N-triples, and RDF/XML)
                 # turtle.shex, nt.shex, rdf.shex
-                if input_format == TURTLE:
+                if input_format in (TURTLE, TURTLE_ITER):
                     output_file_name = TURTLE
                 elif input_format == NT:
                     output_file_name = "n-triples"
                 elif input_format == RDF_XML:
                     output_file_name = "rdf_xml"
 
                 if compression_mode is None:
```

## Comparing `rdf_doctor-1.1.0rc4.dist-info/LICENSE` & `rdf_doctor-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.0rc4.dist-info/METADATA` & `rdf_doctor-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.0rc4
+Version: 1.1.1
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask (>=2.2.5)
 Requires-Dist: Flask-Cors (>=3.0.9)
 Requires-Dist: rdflib (>=6.3.1)
 Requires-Dist: SPARQLWrapper (>=2.0.0)
 Requires-Dist: wlighter (>=1.0.1)
-Requires-Dist: shexer (>=2.3.0)
+Requires-Dist: shexer (==2.3.0)
 Requires-Dist: unidecode (>=1.3.6)
 
 # rdf-doctor
 [![Pyversions](https://img.shields.io/pypi/pyversions/rdf-doctor.svg)](https://pypi.python.org/pypi/rdf-doctor)
 
 ## Motivation
 DBCLS has conducted to convert various life science databases to RDF and support it. This development will enable us to provide a high-quality dataset that better links existing RDF datasets stored in the RDF portal site and newly developed RDF.
@@ -71,15 +71,15 @@
                         Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz or zip. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)
   --prefix-uri-dict FILE
                         path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)
   --class-uri-dict FILE
                         path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-class-uris.tsv)
   --prefix-list FILE    list of prefixes (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv)
   --force-format INPUT-FORMAT
-                        This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle", "nt" and "xml"(=RDF/XML) can be specified.
+                        This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle", "turtle_iter", "nt" and "xml"(=RDF/XML) can be specified.
 ```
 
 ## See Also
 - [1] https://github.com/DaniFdezAlvarez/shexer
 - [2] http://shex.io/shex-primer/#combined-constraints
 - [3] https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
```

