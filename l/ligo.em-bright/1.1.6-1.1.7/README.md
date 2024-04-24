# Comparing `tmp/ligo.em-bright-1.1.6.tar.gz` & `tmp/ligo_em_bright-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo.em-bright-1.1.6.tar", max compression
+gzip compressed data, was "ligo_em_bright-1.1.7.tar", max compression
```

## Comparing `ligo.em-bright-1.1.6.tar` & `ligo_em_bright-1.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-06-02 19:51:52.112296 ligo.em-bright-1.1.6/LICENSE
--rw-r--r--   0        0        0      977 2023-06-02 19:51:52.113296 ligo.em-bright-1.1.6/README.md
--rw-r--r--   0        0        0      828 2023-08-29 18:24:45.393389 ligo.em-bright-1.1.6/ligo/em_bright/__init__.py
--rw-r--r--   0        0        0     9617 2023-06-27 22:48:05.855588 ligo.em-bright-1.1.6/ligo/em_bright/categorize.py
--rw-r--r--   0        0        0     9917 2023-08-04 19:27:32.802778 ligo.em-bright-1.1.6/ligo/em_bright/computeDiskMass.py
--rw-r--r--   0        0        0    14843 2023-06-02 19:51:52.119296 ligo.em-bright-1.1.6/ligo/em_bright/dag_writer.py
--rw-r--r--   0        0        0     2322 2023-06-02 19:51:53.643297 ligo.em-bright-1.1.6/ligo/em_bright/data/__init__.py
--rw-r--r--   0        0        0    10998 2023-08-29 18:08:26.590523 ligo.em-bright-1.1.6/ligo/em_bright/em_bright.py
--rw-r--r--   0        0        0        0 2023-06-02 19:51:53.645297 ligo.em-bright-1.1.6/ligo/em_bright/tests/__init__.py
--rw-r--r--   0        0        0      303 2023-06-02 19:51:53.646297 ligo.em-bright-1.1.6/ligo/em_bright/tests/data/test_categorize_data.tbl
--rw-r--r--   0        0        0    11317 2023-08-29 18:13:46.242428 ligo.em-bright-1.1.6/ligo/em_bright/tests/test_em_bright.py
--rw-r--r--   0        0        0    23258 2023-06-02 19:51:53.648297 ligo.em-bright-1.1.6/ligo/em_bright/utils.py
--rw-r--r--   0        0        0     1328 2023-08-29 18:12:21.355445 ligo.em-bright-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2496 2023-08-29 18:41:11.330942 ligo.em-bright-1.1.6/setup.py
--rw-r--r--   0        0        0     1649 2023-08-29 18:41:11.331230 ligo.em-bright-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-26 15:14:29.858255 ligo_em_bright-1.1.7/LICENSE
+-rw-r--r--   0        0        0      977 2023-02-26 15:14:29.858255 ligo_em_bright-1.1.7/README.md
+-rw-r--r--   0        0        0      876 2024-04-24 21:18:10.670473 ligo_em_bright-1.1.7/ligo/em_bright/__init__.py
+-rw-r--r--   0        0        0    13353 2024-04-24 21:00:07.364036 ligo_em_bright-1.1.7/ligo/em_bright/categorize.py
+-rw-r--r--   0        0        0     9917 2024-04-24 21:00:07.364036 ligo_em_bright-1.1.7/ligo/em_bright/computeDiskMass.py
+-rw-r--r--   0        0        0    18387 2024-04-24 21:00:07.368036 ligo_em_bright-1.1.7/ligo/em_bright/dag_writer.py
+-rw-r--r--   0        0        0     2322 2024-04-24 21:00:07.380036 ligo_em_bright-1.1.7/ligo/em_bright/data/__init__.py
+-rw-r--r--   0        0        0    13361 2024-04-24 21:00:07.384036 ligo_em_bright-1.1.7/ligo/em_bright/em_bright.py
+-rw-r--r--   0        0        0        0 2023-02-26 15:14:29.870255 ligo_em_bright-1.1.7/ligo/em_bright/tests/__init__.py
+-rw-r--r--   0        0        0      303 2023-02-26 15:14:29.870255 ligo_em_bright-1.1.7/ligo/em_bright/tests/data/test_categorize_data.tbl
+-rw-r--r--   0        0        0      598 2024-04-24 21:00:07.384036 ligo_em_bright-1.1.7/ligo/em_bright/tests/data/test_categorize_ssm_data.csv
+-rw-r--r--   0        0        0    13446 2024-04-24 21:32:44.086550 ligo_em_bright-1.1.7/ligo/em_bright/tests/test_em_bright.py
+-rw-r--r--   0        0        0    28412 2024-04-24 21:00:07.384036 ligo_em_bright-1.1.7/ligo/em_bright/utils.py
+-rw-r--r--   0        0        0     1328 2024-04-24 21:58:17.750385 ligo_em_bright-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.7/PKG-INFO
```

### Comparing `ligo.em-bright-1.1.6/LICENSE` & `ligo_em_bright-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo.em-bright-1.1.6/README.md` & `ligo_em_bright-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/__init__.py` & `ligo_em_bright-1.1.7/ligo/em_bright/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.1.6'
+__version__ = '1.1.7'
 
 PACKAGE_DATA_BASE_URL = (
     'https://git.ligo.org/emfollow/em-properties/em-bright/'
     f'-/raw/v{__version__}/ligo/em_bright/data'
 )
 
 PACKAGE_DATA_LINKS = {name: f'{PACKAGE_DATA_BASE_URL}/{name}' for name in (
@@ -29,9 +29,11 @@
     'SLY230A.pickle',
     'SLY2.pickle',
     'SLY9.pickle',
     'SLy.pickle',
     'EOS_BAYES_FACTOR_MAP.json',
     'EOS_MAX_MASS_MAP.json',
     'EOS_POSTERIOR_DRAWS.h5',
-    'MASS_GAP.pickle'
+    'MASS_GAP.pickle',
+    'GSTLAL_SSM.pickle',
+    'MBTA_SSM.pickle'
 )}
```

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/categorize.py` & `ligo_em_bright-1.1.7/ligo/em_bright/categorize.py`

 * *Files 22% similar despite different names*

```diff
@@ -156,15 +156,113 @@
     drop_mask = (m1_inj_source > max_mass) & (m1_inj_source < 3.0)  # noqa: E501; Restricts m2 by construction
     df_complete = df_complete.loc[~drop_mask]
     with open(outFile, 'wb') as f:
         pickle.dump(df_complete, f)
     return df_complete
 
 
-@_TupleHandler()
+def ssm_categorization(inFile, outFile):
+    '''Multilabel classification for ssm alerts.
+    The categories has_SSM, has_NS, has_MassGap are
+    further divided into multiple mutually disjoint
+    categories
+
+    Parameters
+    ----------
+    inFile : str
+        input filename
+    outFile : str
+        output filename
+    '''
+    df = pd.read_csv(inFile)
+    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
+    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
+    redshift_inj = df.inj_redshift.values
+    m1_inj_source = m1_inj / (1 + redshift_inj)
+    m2_inj_source = m2_inj / (1 + redshift_inj)
+
+    mc_rec = ((m1_rec * m2_rec)**(3/5))/((m1_rec + m2_rec)**(1/5))
+    chi1_inj, chi1_rec = np.zeros_like(m1_inj), df.rec_spin1z.values
+    chi2_inj, chi2_rec = np.zeros_like(m2_inj), df.rec_spin2z.values
+    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
+        m1_inj, m2_inj, chi1_inj, chi2_inj
+    )
+    m1_rec, m2_rec, _, _ = regularize(
+        m1_rec, m2_rec, chi1_rec, chi2_rec
+    )
+    m1_inj_source, m2_inj_source, _, _ = regularize(
+        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
+    )  # spins regularized from previous step.
+
+    classification_array = np.vstack((m1_inj_source, m2_inj_source)).T
+    classification_df = pd.DataFrame(classification_array,
+                                     columns=['m1_inj_source',
+                                              'm2_inj_source'])
+    classification_df["class_label"] = classification_df.apply(
+        has_SSM_conditions, axis=1)
+    class_label = classification_df['class_label']
+    output = np.vstack(
+        (m1_inj_source, m2_inj_source, m1_inj, m2_inj, redshift_inj,
+         m1_rec, m2_rec, chi1_rec, chi2_rec, mc_rec, df.cfar.values,
+         df.snr.values, df.gpstime.values, class_label)
+    ).T
+
+    df_complete = pd.DataFrame(output, columns=[
+        'm1_inj_source', 'm2_inj_source', 'm1_inj', 'm2_inj',
+        'inj_redshift', 'm1_rec', 'm2_rec', 'chi1_rec', 'chi2_rec',
+        'mc_rec', 'cfar', 'snr', 'gpstime', 'class_label']
+    )
+    with open(outFile, 'wb') as f:
+        pickle.dump(df_complete, f)
+    return df_complete
+
+
+def has_SSM_conditions(df):
+    ''' Categorization conditions for ssm
+
+    SSM sub-categories:
+    Only SSM : m1 < 1.0 & m2 < 1.0 : 1
+    SSM & NS: m1 > 1.0 & m1 < 3.0 & m2 < 1.0 : 2
+    SSM & MG: m1 > 3.0 & m1 < 5.0 & m2 < 1.0 : 3
+    SSM & BBH: m1 > 5.0 & m2 < 1.0 : 4
+
+    NS sub-categories:
+    Only NS: m1 > 1.0 & m1 < 3.0 & m2 > 1.0 & m1 < 3.0 : 5
+    NS & MG: m1 > 3.0 & m1 < 5.0 & m2 > 1.0 & m1 < 3.0 : 6
+    NS & BBH: m1 > 5.0 & m2 > 1.0 & m2 < 3.0 : 7
+
+    MG sub-categories:
+    Only MG: m1 > 3.0 & m1 < 5.0 & m2 > 3.0 & m2 < 5.0 N/A
+    MG & BBH : m1 > 5.0 & m2 > 3.0 & m1 < 5.0 N/A
+
+    N/A not available for training
+    '''
+    if ((df['m1_inj_source'] < 1.0) & (df['m2_inj_source'] < 1.0)):
+        return 1
+    elif (((df['m1_inj_source'] > 1.0) & (df['m1_inj_source'] < 3.0)) &
+          (df['m2_inj_source'] < 1.0)):
+        return 2
+    elif (((df['m1_inj_source'] > 3.0) & (df['m1_inj_source'] < 5.0)) &
+          (df['m2_inj_source'] < 1.0)):
+        return 3
+    elif ((df['m1_inj_source'] > 5.0) & (df['m2_inj_source'] < 1.0)):
+        return 4
+    elif (((df['m1_inj_source'] < 3.0) & (df['m1_inj_source'] > 1.0)) &
+          ((df['m2_inj_source'] < 3.0) & (df['m2_inj_source'] > 1.0))):
+        return 5
+    elif (((df['m1_inj_source'] < 5.0) & (df['m1_inj_source'] > 3.0)) &
+          ((df['m2_inj_source'] < 3.0) & (df['m2_inj_source'] > 1.0))):
+        return 6
+    elif ((df['m1_inj_source'] > 5.0) &
+          ((df['m2_inj_source'] < 3.0) & (df['m2_inj_source'] > 1.0))):
+        return 7
+    else:
+        return 0
+
+
 def mass_gap_categorization(inFile, outFile):
     '''Categorize whether the binary is in the lower mass gap
     i.e., any component is between 3 and 5 solar mass
 
     Parameters
     ----------
     inFile : str
@@ -211,30 +309,28 @@
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-i", "--input", action="store", type=str,
                         help="Name of the input file")
     parser.add_argument("-o", "--output", action="store", type=str,
                         help="Name of the output file")
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
-        "-e", "--eosname", default='2H',
-        help="Equation of state used compute remnant matter."
-    )
-    group.add_argument(
-        "--mass-gap", required=False, action="store_true",
-        default=False, help="Supply for mass gap categorization")
-
+    parser.add_argument("-m", "--mode",
+                        help="training mode em_bright/massgap/ssm")
+    parser.add_argument("-e", "--eosname", default='2H',
+                        required=False,
+                        help="Equation of state used compute remnant matter.")
     args = parser.parse_args()
 
-    if args.mass_gap:
+    if args.mode == "massgap":
         mass_gap_categorization(args.input, args.output)
-    else:
+    elif args.mode == "em_bright":
         embright_categorization(args.input, args.output,
                                 eosname=args.eosname)
+    elif args.mode == "ssm":
+        ssm_categorization(args.input, args.output)
 
 
 def main_all():
     parser = argparse.ArgumentParser(
         "Run categorization on all available EoSs: "
         f"{EOS_BAYES_FACTORS.keys()}\n"
         "Output will be tagged by EoS names."
```

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/computeDiskMass.py` & `ligo_em_bright-1.1.7/ligo/em_bright/computeDiskMass.py`

 * *Files identical despite different names*

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/dag_writer.py` & `ligo_em_bright-1.1.7/ligo/em_bright/dag_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -161,21 +161,22 @@
                                             'em_bright_train')
     em_bright_paramater_sweep_plot_executable = config.get(
             'executables', 'em_bright_create_param_sweep_plot'
     )
     exec_arg_assoc = {
         em_bright_train_executable:
             " --input $(macroinput) --config $(macroconfig) "
-            "--output $(macrooutput) --param-sweep-plot-prefix $(macroeos)",
+            "--output $(macrooutput) --param-sweep-plot-prefix $(macroeos) "
+            "--mode em_bright",
         em_bright_paramater_sweep_plot_executable:
             " --input $(macroinput) --config $(macroconfig)"
             " --verbose",
         em_bright_categorize_executable:
             " --input $(macroinput) --output $(macrooutput)"
-            " --eosname $(macroeos) "
+            " --eosname $(macroeos) --mode em_bright"
     }
     condor_sub_dict = dict.fromkeys(exec_arg_assoc)
 
     for exect, arg_sub in exec_arg_assoc.items():
         common_submit_dict["executable"] = exect
         common_submit_dict["arguments"] = arg_sub
         condor_sub_dict[exect] = htcondor.Submit(
@@ -257,18 +258,18 @@
     em_bright_categorize_executable = config.get('executables',
                                                  'em_bright_categorize')
     em_bright_train_executable = config.get('executables',
                                             'em_bright_train')
     exec_arg_assoc = {
         em_bright_categorize_executable:
             " --input $(macroinput) --output $(macrooutput)"
-            " --mass-gap",
+            " --mode massgap",
         em_bright_train_executable:
             " --input $(macroinput) --config $(macroconfig)"
-            " --output $(macrooutput) --mass-gap"
+            " --output $(macrooutput) --mode massgap"
     }
     condor_sub_dict = dict.fromkeys(exec_arg_assoc)
     for exect, arg_sub in exec_arg_assoc.items():
         common_submit_dict["executable"] = exect
         common_submit_dict["arguments"] = arg_sub
         condor_sub_dict[exect] = htcondor.Submit(
             common_submit_dict)
@@ -306,30 +307,107 @@
     em_bright_categorize_layer.child_layer(
             name=em_bright_train_executable,
             submit_description=condor_sub_dict[em_bright_train_executable],
             vars=em_bright_train_vars
         )
 
 
+def _add_ssm_workflow(condor_dag, args, common_submit_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+    # Get injection directory
+
+    em_bright_categorize_prefix = config.get('output_filenames',
+                                             'em_bright_categorize_prefix')
+    em_bright_categorize_suffix = config.get('output_filenames',
+                                             'em_bright_categorize_suffix')
+    em_bright_categorize_executable = config.get('executables',
+                                                 'em_bright_categorize')
+    em_bright_train_executable = config.get('executables',
+                                            'em_bright_train')
+    em_bright_train_suffix = config.get('output_filenames',
+                                        'em_bright_train_suffix')
+    exec_arg_assoc = {
+        em_bright_categorize_executable:
+            " --input $(macroinput) --output $(macrooutput)"
+            " --mode ssm",
+        em_bright_train_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --output $(macrooutput) --mode ssm"
+    }
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+
+    em_bright_categorize_vars = list()
+    em_bright_train_vars = list()
+
+    pipelines = ['gstlal', 'mbta']
+    for i, pipeline in enumerate(pipelines):
+        injection_file_paths = config.get('ssm',
+                                          f'{pipeline}_injection_filename')
+        categorize_input = os.path.join(args.file_dir,
+                                        injection_file_paths)
+        categorize_output = \
+            em_bright_categorize_prefix + f"_{pipeline}_ssm" + \
+            em_bright_categorize_suffix
+        categorize_output = os.path.join(abs_work_dir, categorize_output)
+        em_bright_categorize_vars.append(
+                dict(
+                    macroinput=categorize_input,
+                    macrooutput=categorize_output,
+                )
+        )
+
+        train_output = f"{pipeline}_ssm" + \
+            em_bright_train_suffix
+        train_output = os.path.join(abs_work_dir, train_output)
+        em_bright_train_vars.append(
+         dict(
+                macroinput=categorize_output,
+                macrooutput=train_output,
+                macroconfig=config_path,
+            )
+        )
+
+    em_bright_categorize_layer = condor_dag.layer(
+        name=em_bright_categorize_executable,
+        submit_description=condor_sub_dict[em_bright_categorize_executable],
+        vars=em_bright_categorize_vars
+    )
+
+    em_bright_categorize_layer.child_layer(
+            name=em_bright_train_executable,
+            submit_description=condor_sub_dict[em_bright_train_executable],
+            vars=em_bright_train_vars
+        )
+
+
 def main():
     parser = ArgumentParser("Condor DAG writer for workflow")
     parser.add_argument("-d", "--dagname", required=True,
                         help="Name of the dag file. Placed under --work-dir")
     parser.add_argument("-w", "--work-dir", required=True,
                         help="Working directory to store data outputs")
     parser.add_argument(
         "-i", "--file-dir", required=True,
         help="File containing input injection sqlite databases"
     )
     parser.add_argument("-c", "--config", required=True,
                         help="Name of the config file")
     parser.add_argument("-e", "--executables-dir", required=True,
                         help="Directory containing executables")
-    parser.add_argument("--mass-gap", action='store_true',
-                        help="use --random_forest for Random Forest Mode")
+    parser.add_argument("-m", "--mode", required=True,
+                        choices=["em_bright", "massgap", "ssm"],
+                        help="training mode")
     args = parser.parse_args()
 
     assert _HTCONDOR_INSTALLED, "HTCondor python bindings missing."
 
     config = ConfigParser()
     config.read(args.config)
     # Get path for the work directory
@@ -345,26 +423,33 @@
             'output': '$(executable).stdout',
             'error': '$(executable).stderr',
             'log': '$(executable).log',
             'accounting_group': accounting_group
     }
 
     condor_dag = dags.DAG()
-    join_layer, join_output_dict = _add_common_workflow(
-                                                condor_dag,
-                                                args,
-                                                common_submit_dict)
-    if not args.mass_gap:
+
+    if args.mode == "em_bright":
+        join_layer, join_output_dict = _add_common_workflow(
+                                                    condor_dag,
+                                                    args,
+                                                    common_submit_dict)
         _add_knn_workflow(join_layer, args,
                           common_submit_dict,
                           join_output_dict)
-    else:
+    elif args.mode == "massgap":
+        join_layer, join_output_dict = _add_common_workflow(
+                                            condor_dag,
+                                            args,
+                                            common_submit_dict)
         _add_massgap_workflow(join_layer, args,
                               common_submit_dict,
                               join_output_dict)
+    elif args.mode == "ssm":
+        _add_ssm_workflow(condor_dag, args, common_submit_dict)
 
     print("DAG desription:\n", condor_dag.describe())
     dags.write_dag(condor_dag, abs_work_dir,
                    dag_file_name=args.dagname)
 
     # FIXME Condor refuses to carry over env vars
     # remove when solution is found
```

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/data/__init__.py` & `ligo_em_bright-1.1.7/ligo/em_bright/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/em_bright.py` & `ligo_em_bright-1.1.7/ligo/em_bright/em_bright.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 assert set(_classifiers) == set(EOS_BAYES_FACTORS), "Inconsistency in"
 " number of trained classifiers."
 
 _massgap_classifier = utils._open_and_return_clfs(
         PACKAGE_FILENAMES['MASS_GAP.pickle']
     )
 
+_gstlal_ssm_classifier = utils._open_and_return_clfs(
+        PACKAGE_FILENAMES['GSTLAL_SSM.pickle']
+    )
+
+_mbta_ssm_classifier = utils._open_and_return_clfs(
+        PACKAGE_FILENAMES['MBTA_SSM.pickle']
+    )
+
 
 def mchirp(mass_1, mass_2):
     return (mass_1 * mass_2)**(3./5.)/(mass_1 + mass_2)**(1./5.)
 
 
 def q(mass_1, mass_2):
     return mass_2/mass_1 if mass_2 < mass_1 else mass_1/mass_2
@@ -109,14 +117,77 @@
             features).T[1][0] * bayes_factor
         reweighted_emb_score += emb_classifier.predict_proba(
             features).T[1][0] * bayes_factor
     massgap_score = _massgap_classifier.predict_proba(features).T[1][0]
     return reweighted_ns_score, reweighted_emb_score, massgap_score
 
 
+def source_classification_ssm(mass_1, mass_2, chi1, chi2, mc, snr,
+                              pipeline, ssm_classifier=None):
+    """
+    Computes ``HasSSM``, ``HasNS``, ``HasMassGap`` probabilities
+    from point mass, spin, chirp mass and signal to
+    noise ratio estimates for SSM search.
+
+    Parameters
+    ----------
+    mass_1 : float
+        primary mass
+    mass_2 : float
+        secondary mass
+    chi1 : float
+        dimensionless primary spin
+    chi2 : float
+        dimensionless secondary spin
+    mc : float
+        chirp mass
+    snr : float
+        signal to noise ratio of the signal
+    pipeline : string
+        search pipeline
+    ssm_classifier : object, optional
+        pickled object for gstlal ssm classification
+
+    Returns
+    -------
+    tuple
+        (HasSSM, HasNS, HasMassGap) predicted values.
+    --------
+    >>> from ligo.em_bright import em_bright
+    >>> em_bright.source_classification_ssm(2.0 ,1.0 ,0. ,0. ,10.0, "gstlal")
+    (1.0, 1.0, 0.0)
+    """
+    if mass_1 >= mass_2:
+        features = [[mass_1, mass_2, chi1, chi2, mc, snr]]
+    elif mass_1 < mass_2:
+        features = [[mass_2, mass_1, chi2, chi1, mc, snr]]
+    try:
+        # custom classifiers supplied
+        predict = ssm_classifier.predict_proba(features).T
+        has_SSM = predict[0][0] + predict[1][0] + predict[2][0] + predict[3][0]
+        has_NS = predict[1][0] + predict[4][0] + predict[5][0] + predict[6][0]
+        has_MassGap = predict[2][0] + predict[5][0]
+        return has_SSM, has_NS, has_MassGap
+    except AttributeError as e:
+        msg, *_ = e.args
+        if msg != """'NoneType' object has no attribute 'predict_proba'""":
+            raise
+    if pipeline == 'gstlal':
+        clf = _gstlal_ssm_classifier
+    elif pipeline == "mbta":
+        clf = _mbta_ssm_classifier
+    predict = clf.predict_proba(features).T
+    has_SSM_score = predict[0][0] + predict[1][0] + \
+        predict[2][0] + predict[3][0]
+    has_NS_score = predict[1][0] + predict[4][0] + \
+        predict[5][0] + predict[6][0]
+    has_MassGap_score = predict[2][0] + predict[5][0]
+    return has_SSM_score, has_NS_score, has_MassGap_score
+
+
 def get_redshifts(distances, N=10000):
     """
     Compute redshift using the Planck15 cosmology.
 
     Parameters
     ----------
     distances: float or numpy.ndarray
```

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/tests/test_em_bright.py` & `ligo_em_bright-1.1.7/ligo/em_bright/tests/test_em_bright.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .. import em_bright, categorize, utils
 from ..data import EOS_MAX_MASS
 
 
 def test_version():
     from .. import __version__
-    assert __version__ == '1.1.6'
+    assert __version__ == '1.1.7'
 
 
 @pytest.mark.parametrize(
     'posteriors, dtype, result_2H, result_SLy, result_eos',
     [[[(1.2, 1.0, 0.0, 0.0, 0.0, 0.0, 100.0),
        (2.0, 0.5, 0.99, 0.99, 0.0, 0.0, 150.0)],
       [('chirp_mass', '<f8'), ('mass_ratio', '<f8'), ('a_1', '<f8'),
@@ -174,16 +174,37 @@
     '''Test results for limiting cases'''
     ns, em, mg = em_bright.source_classification(m1, m2, chi1, chi2, snr)
     assert ns == pytest.approx(result_ns, abs=1e-2)
     assert em == pytest.approx(result_em, abs=1e-2)
     assert mg == pytest.approx(result_mg, abs=1e-2)
 
 
+@pytest.mark.parametrize(
+    'm1,m2,chi1,chi2,mc,snr,pipeline,result_ssm,result_ns,result_mg',
+    [[0.5, 0.5, 0.0, 0.0, 0.435, 10.0, 'gstlal', 1.0, 0.52, 0.0],
+     [2.5, 1.0, 0.0, 0.0, 1.348, 10.0, 'gstlal', 0.52, 0.8, 0.16],
+     [10.0, 1.0, 0.0, 0.0, 2.464, 10.0, 'gstlal', 0.04, 0.96, 0.2],
+     [0.5, 0.5, 0.0, 0.0, 0.435, 10.0, 'mbta', 1.0, 0.28, 0.0],
+     [2.5, 1.0, 0.0, 0.0, 1.348, 10.0, 'mbta', 0.68, 0.84, 0.16],
+     [10.0, 1.0, 0.0, 0.0, 2.464, 10.0, 'mbta', 0.12, 0.879, 0.36],
+     [1.0, 10.0, 0.0, 0.0, 2.464, 10.0, 'mbta', 0.12, 0.879, 0.36]]
+)
+def test_source_classification_ssm_sanity(m1, m2, chi1, chi2, mc,
+                                          snr, pipeline, result_ssm,
+                                          result_ns, result_mg):
+    '''Test results for limiting cases'''
+    ssm, ns, mg = em_bright.source_classification_ssm(
+        m1, m2, chi1, chi2, mc, snr, pipeline)
+    assert ssm == pytest.approx(result_ssm, abs=1e-2)
+    assert ns == pytest.approx(result_ns, abs=1e-2)
+    assert mg == pytest.approx(result_mg, abs=1e-2)
+
+
 def test_mock_classifier():
-    '''Test to check usage of custom classifier'''
+    '''Test to check usage of custom classifier for em_bright'''
     m1 = 1.1
     m2 = 1.0
     chi1 = 0.04
     chi2 = 0.0
     snr = 20.
     # Define mock objects
     mock_clf_ns = Mock()
@@ -197,14 +218,37 @@
     mock_clf_ns.predict_proba.assert_called_once()
     mock_clf_emb.predict_proba.assert_called_once()
     assert ns == 1.0
     assert em == 1.0
     assert mg == 0.0
 
 
+def test_mock_classifier_ssm():
+    '''Test to check usage of custom classifier for ssm'''
+    m1 = 0.9
+    m2 = 0.5
+    mc = 0.579
+    chi1 = 0.0
+    chi2 = 0.0
+    snr = 20.
+    pipeline = "gstlal"
+    # Define mock objects
+    mock_clf_ssm = Mock()
+    mock_clf_ssm.predict_proba = Mock(return_value=np.array([[
+        0.28, 0.6, 0.08, 0.0, 0.04, 0.0, 0.0]]))
+    ssm, ns, mg = em_bright.source_classification_ssm(
+        m1, m2, chi1,
+        chi2, mc, snr, pipeline,
+        ssm_classifier=mock_clf_ssm)
+    mock_clf_ssm.predict_proba.assert_called_once()
+    assert ssm == 0.96
+    assert ns == 0.64
+    assert mg == 0.08
+
+
 @pytest.mark.parametrize(
     'm1,m2,chi1,chi2,eosname,non_zero_remnant',
     [[1.1, 1.0, 0.0, 0.0, "2H", 1.0],
      [1.1, 1.0, 0.0, 0.0, "SLy", 1.0],
      [1.1, 1.0, 0.0, 0.0, "AP4", 1.0],
      [1.1, 1.0, 0.0, 0.0, "WFF1", 1.0],
      [26.0, 2.6, 0.0, 0.0, "2H", 0.0],
@@ -288,7 +332,20 @@
     )
     assert ~np.all(
         np.logical_xor(
             res.mass_gap.values.astype(bool),
             expected_mask
         )
     )
+
+
+def test_ssm_categorization():
+    with NamedTemporaryFile() as tf:
+        outFile = tf.name
+    categorize.ssm_categorization(
+        Path(__file__).parents[0] / 'data/test_categorize_ssm_data.csv',
+        outFile
+    )
+    df = pd.read_csv(Path(__file__).parents[0] /
+                     'data/test_categorize_ssm_data.csv')
+    res = pd.read_pickle(outFile)
+    assert (df.truth == res.class_label).all()
```

### Comparing `ligo.em-bright-1.1.6/ligo/em_bright/utils.py` & `ligo_em_bright-1.1.7/ligo/em_bright/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -183,46 +183,22 @@
     WHERE
     sngl_inspiral.ifo=='H1';
     """
     np.savetxt(args.output, np.array(cur.execute(query).fetchall()),
                fmt='%f|%f|%f|%f|%f|%f|%f|%f|%f|%d|%e|%f|%f')
 
 
-def train():
-    parser = ArgumentParser(
-        description='Executable to train source classifier from injections')
-
-    parser.add_argument(
-        '-i', '--input',
-        help='Pickled dataframe containing source categorized data')
-    parser.add_argument(
-        '-o', '--output',
-        help='Pickled object storing the trained classifiers')
-    parser.add_argument(
-        '-d', '--param-sweep-plot-prefix', default=None,
-        help='Supply filename prefix to output a parameter sweep plot')
-    parser.add_argument(
-        '-c', '--config', required=True,
-        help='Config file with additional parameters')
-    parser.add_argument("--mass-gap", required=False, action="store_true",
-                        help="mode of categorization")
-
-    args = parser.parse_args()
-    if args.mass_gap:
-        settings = 'massgap'
-    else:
-        settings = 'em_bright'
-    config = ConfigParser()
-    config.read(args.config)
+def pre_train(config, input, mode):
     # compulsory sections in config
     required_sections = ['core',
                          'em_bright']
     assert all(config.has_section(s) for s in required_sections), \
         'Config file must have sections %s' % (required_sections,)
 
+    settings = mode
     # get column names and values from config
     feature_cols = config.get(settings,
                               'feature_cols').split(',')
     category_cols = config.get(settings,
                                'category_cols').split(',')
     threshold_cols = config.get(settings,
                                 'threshold_cols').split(',')
@@ -232,15 +208,15 @@
         eval, config.get(
             settings,
             'threshold_values').split(',')
         )
     threshold_type = config.get(settings,
                                 'threshold_type').split(',')
     # read dataframe, check sanity
-    with open(args.input, 'rb') as f:
+    with open(input, 'rb') as f:
         df = pickle.load(f)
 
     assert all(col in df.keys() for col in all_cols), \
         'Dataframe must contain columns %s' % (all_cols,)
 
     # create masked array based on threshold values,
     # extract features and targets
@@ -249,72 +225,155 @@
                                threshold_type):
         mask &= df[col] < value if typ == 'lesser' else \
             df[col] > value if typ == 'greater' else True
 
     features = df[feature_cols][mask]
     targets = df[category_cols][mask]
 
-    if not args.mass_gap:
-        clf_kwargs = eval(config.get('em_bright',
-                                     'clf_kwargs'))
-        if clf_kwargs.get('metric') == 'mahalanobis':
-            clf_kwargs['metric_params'] = dict(
-                V=features.cov().values
-            )  # covariance matrix needed for mahalanobis metric
-        clfs = []
-        for category, target_value in targets.iteritems():
-            # run KFold cross-validation
-            res_predict, res_predict_proba = run_k_fold_split(
-                features, target_value,
-                training_task=run_KNN_classifier,
-                **clf_kwargs)
-            test_results = pd.DataFrame(
-                np.vstack((features.T, target_value,
-                           res_predict, res_predict_proba)).T,
-                columns=feature_cols + ['targets', 'predict', 'predict_proba']
-            )
-            test_results_filename = 'cross-val-res-' + category + '.csv'
-            test_results.to_csv(test_results_filename, index=False)
-            # train on the full dataset
-            clf = KNeighborsClassifier(**clf_kwargs)
-            clf.fit(features.values, target_value)
-            if args.param_sweep_plot_prefix:
-                _create_param_sweep_plot(
-                    clf, category,
-                    args.param_sweep_plot_prefix
-                )
-            clfs.append(clf)
-        # append the output filename of the classifier
-        clfs.extend([args.output])
-        with open(args.output, 'wb') as f:
-            pickle.dump(clfs, f)
-    else:
-        # train random forest classifier for massgap category
-        clf_kwargs = eval(config.get('massgap',
-                                     'clf_kwargs'))
+    return features, targets
+
+
+def train_embright(input, output, config, parameter_sweep_prefix):
+    mode = 'em_bright'
+    features, targets = pre_train(config, input, mode)
+
+    clf_kwargs = eval(config.get('em_bright',
+                                 'clf_kwargs'))
+    if clf_kwargs.get('metric') == 'mahalanobis':
+        clf_kwargs['metric_params'] = dict(
+            V=features.cov().values
+        )  # covariance matrix needed for mahalanobis metric
+    clfs = []
+    for category, target_value in targets.items():
+        # run KFold cross-validation
         res_predict, res_predict_proba = run_k_fold_split(
-            features, targets,
-            training_task=run_RF_classifier, **clf_kwargs
-        )
+            features, target_value, mode="em_bright",
+            training_task=run_KNN_classifier,
+            **clf_kwargs)
+        feature_cols = config.get('em_bright',
+                                  'feature_cols').split(',')
         test_results = pd.DataFrame(
-            np.vstack((features.T, targets.squeeze().T,
+            np.vstack((features.T, target_value,
                        res_predict, res_predict_proba)).T,
             columns=feature_cols + ['targets', 'predict', 'predict_proba']
         )
-        test_results_filename = 'cross-val-res-' + 'mass-gap' + '.csv'
+        test_results_filename = 'cross-val-res-' + category + '.csv'
         test_results.to_csv(test_results_filename, index=False)
-        clf = RandomForestClassifier(**clf_kwargs)
-        clf.fit(features.values, targets.squeeze())
-        _create_param_sweep_plot(
-            clf, 'mass_gap',
-            prefix='SLy'  # FIXME: ad-hoc prefix needed, not used for plotting
-        )
-        with open(args.output, 'wb') as f:
-            # append the filename of the classfier
-            pickle.dump([clf, args.output], f)
+        # train on the full dataset
+        clf = KNeighborsClassifier(**clf_kwargs)
+        clf.fit(features.values, target_value)
+        if parameter_sweep_prefix:
+            _create_param_sweep_plot(
+                clf, category,
+                parameter_sweep_prefix
+            )
+        clfs.append(clf)
+    # append the output filename of the classifier
+    clfs.extend([output])
+    with open(output, 'wb') as f:
+        pickle.dump(clfs, f)
+
+
+def train_massgap(input, output, config):
+    mode = "massgap"
+    features, targets = pre_train(config, input, mode)
+
+    # train random forest classifier for massgap category
+    clf_kwargs = eval(config.get('massgap',
+                                 'clf_kwargs'))
+    res_predict, res_predict_proba = run_k_fold_split(
+        features, targets, mode="massgap",
+        training_task=run_RF_classifier, **clf_kwargs
+    )
+    feature_cols = config.get('massgap',
+                              'feature_cols').split(',')
+    test_results = pd.DataFrame(
+        np.vstack((features.T, targets.squeeze().T,
+                   res_predict, res_predict_proba)).T,
+        columns=feature_cols + ['targets', 'predict', 'predict_proba']
+    )
+    test_results_filename = 'cross-val-res-' + 'mass-gap' + '.csv'
+    test_results.to_csv(test_results_filename, index=False)
+    clf = RandomForestClassifier(**clf_kwargs)
+    clf.fit(features.values, targets.squeeze())
+    _create_param_sweep_plot(
+        clf, 'mass_gap',
+        prefix='SLy'  # FIXME: ad-hoc prefix needed, not used for plotting
+    )
+    with open(output, 'wb') as f:
+        # append the filename of the classfier
+        pickle.dump([clf, output], f)
+
+
+def train_ssm(input, output, config):
+    mode = 'ssm'
+    features, targets = pre_train(config, input, mode)
+
+    # train random forest classifier for massgap category
+    clf_kwargs = eval(config.get('ssm',
+                                 'clf_kwargs'))
+    res_predict, res_predict_proba = run_k_fold_split(
+        features, targets, mode="ssm",
+        training_task=run_KNN_classifier, **clf_kwargs
+    )
+    pipeline = input.split('/')[-1].split('_')[-2]
+    feature_cols = config.get('ssm',
+                              'feature_cols').split(',')
+    test_results = pd.DataFrame(
+        np.vstack((features.T, targets.squeeze().T,
+                   res_predict)).T,
+        columns=feature_cols + ['targets', 'predict']
+    )
+    pred = pd.DataFrame(res_predict_proba,
+                        columns=['has_SSM', 'has_NS', 'has_MassGap'])
+    test_results = pd.concat([test_results, pred], axis=1)
+    test_results_filename = f'cross-val-res-{pipeline}-' + 'ssm' + '.csv'
+    test_results.to_csv(test_results_filename, index=False)
+    clf = KNeighborsClassifier(**clf_kwargs)
+    clf.fit(features.values, targets.squeeze())
+    _create_param_sweep_plot(
+        clf, 'ssm',
+        prefix=pipeline
+    )
+    with open(output, 'wb') as f:
+        # append the filename of the classfier
+        pickle.dump([clf, output], f)
+
+
+def train():
+    parser = ArgumentParser(
+        description='Executable to train source classifier from injections')
+    parser.add_argument(
+        '-i', '--input',
+        help='Pickled dataframe containing source categorized data')
+    parser.add_argument(
+        '-o', '--output',
+        help='Pickled object storing the trained classifiers')
+    parser.add_argument(
+        '-c', '--config', required=True,
+        help='Config file with additional parameters')
+    parser.add_argument(
+        '-m', '--mode', choices=['em_bright', 'massgap', 'ssm'],
+        required=True,
+        help='Mode of training')
+    parser.add_argument(
+        '-d', '--param-sweep-plot-prefix', default=None, required=False,
+        help='Supply filename prefix to output a parameter sweep plot')
+
+    args = parser.parse_args()
+    config = ConfigParser()
+    config.read(args.config)
+
+    if args.mode == 'em_bright':
+        train_embright(args.input, args.output, config,
+                       args.param_sweep_plot_prefix)
+    elif args.mode == 'massgap':
+        train_massgap(args.input, args.output, config)
+    elif args.mode == 'ssm':
+        train_ssm(args.input, args.output, config)
 
 
 def _open_and_return_clfs(filename):
     """Unpack pickle files storing classifier and return.
     If two classifiers exist, assume first argument is HasNS,
     second HasRemnant. If single classifier exists, then assume
     mass_gap classifier.
@@ -325,33 +384,37 @@
             clf_ns, clf_em, _filename = content
             return clf_ns, clf_em
         except ValueError:
             clf_mass_gap, _filename = content
             return clf_mass_gap
 
 
-def _get_mass_grid():
+def _get_mass_grid(mode="em_bright"):
     """Get a grid over mass1, mass2. Used for parameter sweep."""
-    mass1 = np.linspace(1, 20, 200)
-    mass2 = np.linspace(1, 20, 200)
+    if mode == "em_bright":
+        mass1 = np.linspace(1, 20, 200)
+        mass2 = np.linspace(1, 20, 200)
+    elif mode == "ssm":
+        mass1 = np.linspace(0.2, 10, 200)
+        mass2 = np.linspace(0.2, 1, 200)
     t = Table(
         data=np.vstack(
             (np.repeat(mass1, mass2.size),
              np.tile(mass2, mass1.size))
         ).T, names=('mass1', 'mass2')
     )
     mask = t['mass1'] > t['mass2']
     t = t[mask]
     return t
 
 
 def _get_param_sweep(clf):
     """Create a fake recovered parameter space return
     the predictions for the classifier sweeping across
-    masses.
+    masses (for em_bright/massgap workflow)
     """
     if hasattr(clf, 'metric') and clf.metric == "mahalanobis":
         clf.n_jobs = 1  # issue with BallTree output
     t = _get_mass_grid()
     spins = Table(
         data=np.vstack(
             (np.repeat(np.linspace(0, 1, 2), 2),
@@ -370,34 +433,92 @@
             [t['mass1'], t['mass2'], chi1, chi2, SNR]
         ).T
         predictions = clf.predict_proba(param_sweep_features).T[1]
         res.append((param_sweep_features, predictions))
     return res
 
 
+def _get_param_sweep_ssm(clf, mode="em_bright"):
+    """Create a fake recovered parameter space return
+    the predictions for the classifier sweeping across
+    masses (for SSM workflow)
+    """
+    t = _get_mass_grid(mode)
+    spins = Table(
+        data=np.vstack(
+            (np.repeat(np.linspace(0, 1, 2), 2),
+             np.tile(np.linspace(0, 1, 2), 2))
+        ).T,
+        names=('chi1', 'chi2')
+    )
+    SNR = 10.
+    res = list()
+    t['mc'] = ((t['mass1'] * t['mass2'])**(3/5)) / \
+              ((t['mass1'] + t['mass2'])**(1/5))
+    for spin_vals in spins:
+        SNR *= np.ones(len(t))
+        chi1 = spin_vals['chi1'] * np.ones(len(t))
+        chi2 = spin_vals['chi2'] * np.ones(len(t))
+        # make predictions and make plots
+        param_sweep_features = np.stack(
+            [t['mass1'], t['mass2'], chi1, chi2, t['mc'], SNR]
+        ).T
+        predict_proba = clf.predict_proba(param_sweep_features)
+        has_SSM = predict_proba.T[0] + predict_proba.T[1] + \
+            predict_proba.T[2] + predict_proba.T[3]
+        has_NS = predict_proba.T[1] + predict_proba.T[4] + \
+            predict_proba.T[5] + predict_proba.T[6]
+        has_MassGap = predict_proba.T[2] + predict_proba.T[5]
+        predictions = np.array((has_SSM, has_NS, has_MassGap),
+                               dtype=float)
+        res.append((param_sweep_features, predictions))
+    return res
+
+
 def _create_param_sweep_plot(clf, category, prefix=None):
     """Create a parameter sweep plot using the supplied classifer"""
     import matplotlib.pyplot as plt
-    res = _get_param_sweep(clf)
+    if category == "ssm":
+        res = _get_param_sweep_ssm(clf, mode="ssm")
+    else:
+        res = _get_param_sweep(clf)
     fig = plt.figure(figsize=(14, 20))
-    for idx, r in enumerate(res):
-        features, predictions = r
-        # FIXME: Ugly, but works
-        title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
-            features[0][2], features[0][3],
-            features[0][4]
-        )
-        make_plots(
-            features, predictions, title,
-            (fig, idx+1), prefix=prefix, category=category
-        )
-    try:
-        plt.savefig(prefix+'_param_sweep_'+category+'.png')
-    except TypeError:
-        plt.savefig('param_sweep_'+category+'.png')
+    if category != 'ssm':
+        for idx, r in enumerate(res):
+            features, predictions = r
+            # FIXME: Ugly, but works
+            title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
+                features[0][2], features[0][3],
+                features[0][4]
+            )
+            make_plots(
+                features, predictions, title,
+                (fig, idx+1), prefix=prefix, category=category
+            )
+        try:
+            plt.savefig(prefix+'_param_sweep_'+category+'.png')
+        except TypeError:
+            plt.savefig('param_sweep_'+category+'.png')
+    else:
+        for i, cat in enumerate(["has_SSM", "has_NS", "has_MassGap"]):
+            plt.clf()
+            for idx, r in enumerate(res):
+                features, predictions = r
+                title = "chi1 = {0}; chi2 = {1}; SNR = {2} {3}".format(
+                    features[0][2], features[0][3],
+                    features[0][5], cat
+                )
+                make_plots(
+                    features, predictions[i], title,
+                    (fig, idx+1), prefix=prefix, category=category
+                )
+            try:
+                plt.savefig(prefix+f'_param_sweep_{cat}_'+category+'.png')
+            except TypeError:
+                plt.savefig(f'param_sweep_{cat}_'+category+'.png')
 
 
 def load_eos_posterior():
     '''
     Loads eos posterior draws (https://zenodo.org/record/6502467#.Yoa2EKjMI2z)
 
     Returns
@@ -506,14 +627,16 @@
     fig_.add_subplot(4, 1, idx)
     # indices 0 and 1 correspond to mass1 and mass2 respectively
     plt.scatter(features.T[0], features.T[1],
                 s=10, c=predictions)
     plt.title(title)
     plt.tight_layout()
     plt.colorbar(label='Probability')
+    if category == 'ssm':
+        return
     # plot chirp mass contours
     m1 = np.linspace(1, 20, 1000)
     m2 = np.linspace(1, 20, 1000)
     M1, M2 = np.meshgrid(m1, m2)
     s1z = np.unique(features.T[2])[0]*np.ones(M1.shape)
     s2z = np.unique(features.T[3])[0]*np.ones(M2.shape)
     rem_masses = list()
@@ -561,15 +684,15 @@
                          levels=[0., ], colors='red',
                          linewidths=1.2)
     plt.xlabel(r'$m_1$', fontsize=16)
     plt.ylabel(r'$m_2$', fontsize=16)
 
 
 def run_k_fold_split(features, targets, n_splits=10, random_state=0,
-                     training_task=None, **kwargs):
+                     mode="em_bright", training_task=None, **kwargs):
     """Split the `features` in `n_splits`, train on `n_splits - 1`
     sets, test on the last fraction. This performed across the complete
     dataset.
 
     Parameters
     ----------
     features : numpy.ndarray
@@ -589,15 +712,20 @@
         Keyword arguments passed to `training_task`.
 
     Returns
     -------
     tuple
         (res_predict, res_predict_proba) - predictions and probabilities
     """
-    res_predict_proba = np.empty(len(features))
+    if mode == "ssm":
+        # SSM prediction is divided into hasSSM, hasNS, hasMassGap
+        # This results in array size (X,3)
+        res_predict_proba = np.empty([len(features), 3])
+    else:
+        res_predict_proba = np.empty(len(features))
     res_predict = np.empty(len(features))
     res_predict_proba[:] = np.nan
     res_predict[:] = np.nan
 
     sss = KFold(n_splits=n_splits, shuffle=True, random_state=random_state)
     sss.get_n_splits(features, targets)
     for train_index, test_index in sss.split(features, targets):
@@ -605,17 +733,25 @@
             features.iloc[train_index], \
             features.iloc[test_index], \
             targets.iloc[train_index]
 
         predict_proba, predict = training_task(X_train, y_train, X_test,
                                                **kwargs)
         # second column is the prob of NS/EMB
-        predict_proba = predict_proba.T[1]
-
-        res_predict_proba[test_index] = predict_proba
+        if (mode == "em_bright") | (mode == "massgap"):
+            predict_proba = predict_proba.T[1]
+        elif mode == "ssm":
+            has_SSM = predict_proba.T[0] + predict_proba.T[1] + \
+                predict_proba.T[2] + predict_proba.T[3]
+            has_NS = predict_proba.T[1] + predict_proba.T[4] + \
+                predict_proba.T[5] + predict_proba.T[6]
+            has_MassGap = predict_proba.T[2] + predict_proba.T[5]
+            predict_proba = np.array((has_SSM, has_NS, has_MassGap),
+                                     dtype=float)
+        res_predict_proba[test_index] = predict_proba.T
         res_predict[test_index] = predict
     return res_predict, res_predict_proba
 
 
 def run_KNN_classifier(X_train, y_train,
                        X_test,
                        **kwargs):
```

### Comparing `ligo.em-bright-1.1.6/pyproject.toml` & `ligo_em_bright-1.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ligo.em-bright"
-version = "1.1.6"
+version = "1.1.7"
 description = "Possibility and properties of Electromagnetically-bright sources of gravitational-wave events"
 readme = "README.md"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Shaon Ghosh <shaon.ghosh@ligo.org>"]
 packages = [
     { include = "ligo" },
```

### Comparing `ligo.em-bright-1.1.6/PKG-INFO` & `ligo_em_bright-1.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ligo.em-bright
-Version: 1.1.6
+Version: 1.1.7
 Summary: Possibility and properties of Electromagnetically-bright sources of gravitational-wave events
 License: MIT
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astropy (>=5.2.1)
 Requires-Dist: h5py (>=3.7.0)
 Requires-Dist: lalsuite (>=7.0,<8.0)
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: scikit-learn (==1.2.1)
 Description-Content-Type: text/markdown
```

