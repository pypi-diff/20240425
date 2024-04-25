# Comparing `tmp/opentf_tools-0.45.0-py3-none-any.whl.zip` & `tmp/opentf_tools-0.46.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 55594 bytes, number of entries: 17
--rw-r--r--  2.0 unx    23421 b- defN 23-Dec-18 09:30 opentf/tools/ctl.py
--rw-r--r--  2.0 unx    16082 b- defN 23-Dec-18 09:30 opentf/tools/ctlattachments.py
--rw-r--r--  2.0 unx    16227 b- defN 23-Dec-18 09:30 opentf/tools/ctlcommons.py
--rw-r--r--  2.0 unx    32399 b- defN 23-Dec-18 09:30 opentf/tools/ctlconfig.py
--rw-r--r--  2.0 unx    12738 b- defN 23-Dec-18 09:30 opentf/tools/ctlnetworking.py
--rw-r--r--  2.0 unx    11840 b- defN 23-Dec-18 09:30 opentf/tools/ctlplugin_gitlab.py
--rw-r--r--  2.0 unx    13793 b- defN 23-Dec-18 09:30 opentf/tools/ctlqualitygate.py
--rw-r--r--  2.0 unx    10092 b- defN 23-Dec-18 09:30 opentf/tools/ctltokens.py
--rw-r--r--  2.0 unx    38832 b- defN 23-Dec-18 09:30 opentf/tools/ctlworkflows.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Dec-18 09:30 opentf/tools/done.py
--rw-r--r--  2.0 unx     9391 b- defN 23-Dec-18 09:30 opentf/tools/ready.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Dec-18 09:30 opentf_tools-0.45.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1783 b- defN 23-Dec-18 09:30 opentf_tools-0.45.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-18 09:30 opentf_tools-0.45.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-Dec-18 09:30 opentf_tools-0.45.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Dec-18 09:30 opentf_tools-0.45.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1439 b- defN 23-Dec-18 09:30 opentf_tools-0.45.0.dist-info/RECORD
-17 files, 202820 bytes uncompressed, 53240 bytes compressed:  73.8%
+Zip file size: 58253 bytes, number of entries: 18
+-rw-r--r--  2.0 unx    23841 b- defN 24-Apr-25 08:03 opentf/tools/ctl.py
+-rw-r--r--  2.0 unx    15915 b- defN 24-Apr-25 08:03 opentf/tools/ctlattachments.py
+-rw-r--r--  2.0 unx    16292 b- defN 24-Apr-25 08:03 opentf/tools/ctlcommons.py
+-rw-r--r--  2.0 unx    32112 b- defN 24-Apr-25 08:03 opentf/tools/ctlconfig.py
+-rw-r--r--  2.0 unx     7392 b- defN 24-Apr-25 08:03 opentf/tools/ctlgenerate.py
+-rw-r--r--  2.0 unx    12664 b- defN 24-Apr-25 08:03 opentf/tools/ctlnetworking.py
+-rw-r--r--  2.0 unx    11840 b- defN 24-Apr-25 08:03 opentf/tools/ctlplugin_gitlab.py
+-rw-r--r--  2.0 unx    13655 b- defN 24-Apr-25 08:03 opentf/tools/ctlqualitygate.py
+-rw-r--r--  2.0 unx     9704 b- defN 24-Apr-25 08:03 opentf/tools/ctltokens.py
+-rw-r--r--  2.0 unx    38262 b- defN 24-Apr-25 08:03 opentf/tools/ctlworkflows.py
+-rw-r--r--  2.0 unx     3188 b- defN 24-Apr-25 08:03 opentf/tools/done.py
+-rw-r--r--  2.0 unx     9391 b- defN 24-Apr-25 08:03 opentf/tools/ready.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 24-Apr-25 08:03 opentf_tools-0.46.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1763 b- defN 24-Apr-25 08:03 opentf_tools-0.46.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 08:03 opentf_tools-0.46.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-25 08:03 opentf_tools-0.46.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-25 08:03 opentf_tools-0.46.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1522 b- defN 24-Apr-25 08:03 opentf_tools-0.46.0.dist-info/RECORD
+18 files, 209135 bytes uncompressed, 55769 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: opentf/tools/ctlcommons.py
 Comment: 
 
 Filename: opentf/tools/ctlconfig.py
 Comment: 
 
+Filename: opentf/tools/ctlgenerate.py
+Comment: 
+
 Filename: opentf/tools/ctlnetworking.py
 Comment: 
 
 Filename: opentf/tools/ctlplugin_gitlab.py
 Comment: 
 
 Filename: opentf/tools/ctlqualitygate.py
@@ -27,26 +30,26 @@
 
 Filename: opentf/tools/done.py
 Comment: 
 
 Filename: opentf/tools/ready.py
 Comment: 
 
-Filename: opentf_tools-0.45.0.dist-info/LICENSE
+Filename: opentf_tools-0.46.0.dist-info/LICENSE
 Comment: 
 
-Filename: opentf_tools-0.45.0.dist-info/METADATA
+Filename: opentf_tools-0.46.0.dist-info/METADATA
 Comment: 
 
-Filename: opentf_tools-0.45.0.dist-info/WHEEL
+Filename: opentf_tools-0.46.0.dist-info/WHEEL
 Comment: 
 
-Filename: opentf_tools-0.45.0.dist-info/entry_points.txt
+Filename: opentf_tools-0.46.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: opentf_tools-0.45.0.dist-info/top_level.txt
+Filename: opentf_tools-0.46.0.dist-info/top_level.txt
 Comment: 
 
-Filename: opentf_tools-0.45.0.dist-info/RECORD
+Filename: opentf_tools-0.46.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opentf/tools/ctl.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Henix, henix.fr
+# Copyright 2021-2024 Henix, henix.fr
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,14 +22,15 @@
 from opentf.tools.ctlcommons import (
     generate_output,
     _make_params_from_selectors,
     _ensure_either_uuids_or_selectors,
     _ensure_options,
     _is_command,
     _error,
+    _fatal,
     _get_arg,
     _ensure_uuid,
 )
 from opentf.tools.ctlconfig import (
     read_configuration,
     config_cmd,
     print_config_help,
@@ -40,16 +41,17 @@
     _agentchannel,
     _observer,
     _get,
     _delete,
 )
 from opentf.tools.ctlworkflows import print_workflow_help, workflow_cmd
 from opentf.tools.ctlqualitygate import print_qualitygate_help, qualitygate_cmd
+from opentf.tools.ctlattachments import print_attachments_help, attachments_cmd
+from opentf.tools.ctlgenerate import print_generate_report_help, generate_report_cmd
 from opentf.tools.ctltokens import print_tokens_help, tokens_cmd
-from opentf.tools.ctlattachments import attachments_cmd, print_attachments_help
 
 
 ########################################################################
 
 # pylint: disable=broad-except
 
 DEFAULT_NAMESPACE = 'default'
@@ -81,15 +83,22 @@
 
 Channel Commands:
   get channels                     List known channels
 
 Qualitygate Commands:
   get qualitygate {workflow_id}    Get quality gate status for a workflow
   describe qualitygate {workflow_id}
-                                   Get description of a quality gate status for a workflow
+                                   Get quality gate status description for a workflow
+
+Attachments Commands:
+  get attachments {workflow_id}    List workflow attachments
+  cp {workflow_id}:{...} {destination}
+                                   Get a local copy of a workflow attachment
+  generate report {workflow_id} using {file}
+                                   Generate a report based on an insight from definition file
 
 Token Commands:
   generate token using {key}       Interactively generate a signed token
   check token {token} using {key}  Check if token signature matches public key
   view token {token}               Show token payload
 
 Advanced Commands:
@@ -309,23 +318,21 @@
         'Could not get subscriptions list',
         params=params,
         raw=True,
     )
     if params:
         header = response.headers.get('X-Processed-Query')
         if not header or not ('fieldSelector' in header or 'labelSelector' in header):
-            _error(
+            _fatal(
                 'The orchestrator does not support selectors, please specify explicit subscription IDs or upgrade your orchestrator.'
             )
-            sys.exit(2)
     try:
         result = response.json()
     except Exception as err:
-        _error('Could not get subscriptions list: %s.', err)
-        sys.exit(2)
+        _fatal('Could not get subscriptions list: %s.', err)
     return result['items']
 
 
 def list_subscriptions() -> None:
     """List all active subscriptions.
 
     Outputs information in requested format.
@@ -416,41 +423,37 @@
 
     Abort with an error code 2 if another error occurred.
     """
     resource = verb = None
     selector = _get_arg('--selector=') or _get_arg('-l=')
     if selector:
         if len(selector.split(',')) != 2:
-            _error(
+            _fatal(
                 'Invalid selector, must be of form: "resource==resource,verb==verb", got: %s.',
                 selector,
             )
-            sys.exit(2)
         for item in selector.split(','):
             what, _, value = item.partition('=')
             if what == 'resource':
                 resource = value.lstrip('=').strip()
             elif what == 'verb':
                 verb = value.lstrip('=').strip()
             else:
-                _error(
+                _fatal(
                     'Invalid selector, expecting "resource" or "verb", got: %s.', what
                 )
-                sys.exit(2)
     if (resource and not verb) or (verb and not resource):
-        _error('Incomplete selector, expecting both "resource" and "verb".')
-        sys.exit(2)
+        _fatal('Incomplete selector, expecting both "resource" and "verb".')
 
     url = '/namespaces'
     if resource and verb:
         url += f'?resource={resource}&verb={verb}'
     what = _get(_observer(), url, 'Could not get namespaces list')
     if 'details' not in what or 'items' not in what['details']:
-        _error('Unexpected response: %s', what)
-        sys.exit(2)
+        _fatal('Unexpected response: %s', what)
     namespaces = what['details']['items']
     print('NAMESPACE')
     if '*' in namespaces:
         print('*')
     else:
         for ns in namespaces:
             print(ns)
@@ -476,23 +479,21 @@
         'Could not get agents list',
         params=params,
         raw=True,
     )
     if params and ('fieldSelector' in params or 'labelSelector' in params):
         header = response.headers.get('X-Processed-Query')
         if not header or not ('fieldSelector' in header or 'labelSelector' in header):
-            _error(
+            _fatal(
                 'The orchestrator does not support selectors, please specify explicit agent IDs or upgrade your orchestrator.'
             )
-            sys.exit(2)
     try:
         result = response.json()
     except Exception as err:
-        _error('Could not get agents list: %s.', err)
-        sys.exit(2)
+        _fatal('Could not get agents list: %s.', err)
 
     data = result['items']
 
     # pre-2022-05 orchestrators where returning a dictionary, not a list
     # of manifests.
     if isinstance(data, dict):
         data = []
@@ -609,14 +610,16 @@
         'describe qualitygate', args
     ):
         print_qualitygate_help(args)
     elif _is_command('cp', args):
         print_attachments_help(args)
     elif _is_command('get attachments', args):
         print_attachments_help(args)
+    elif _is_command('generate report', args):
+        print_generate_report_help(args)
     elif _is_command(GETNAMESPACES_COMMAND, args):
         print(GET_NAMESPACES_HELP)
     elif len(args) == 2:
         print(GENERAL_HELP)
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
@@ -702,14 +705,16 @@
         'describe qualitygate', sys.argv
     ):
         qualitygate_cmd()
     elif _is_command('cp', sys.argv):
         attachments_cmd()
     elif _is_command('get attachments', sys.argv):
         attachments_cmd()
+    elif _is_command('generate report', sys.argv):
+        generate_report_cmd()
     elif _is_command('config', sys.argv):
         config_cmd()
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
```

## opentf/tools/ctlattachments.py

```diff
@@ -10,52 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """opentf-ctl workflow attachments handling part"""
 
-from typing import Any, Dict, List, NoReturn, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import fnmatch
 import os
 import sys
 
 from opentf.tools.ctlcommons import (
     _error,
+    _fatal,
     _is_command,
     _ensure_options,
     _ensure_uuid,
     generate_output,
     _get_arg,
 )
 from opentf.tools.ctlconfig import read_configuration
 from opentf.tools.ctlnetworking import _localstore, _get_file, _head
 from opentf.tools.ctlworkflows import _get_workflows, _get_workflow_attachments_events
 
 
 ########################################################################
 # Constants
 
-ALLURE_ENDING = '_a'
-GLOBAL_ENDING = '_e'
-ENDINGS = (ALLURE_ENDING, GLOBAL_ENDING)
 WILDCARDS = ('*', '?', '[', ']', '!')
 
 UUID_LENGTH = 36
 ATTACHMENT_PREFIX_LENGTH = len('/tmp/')
 ALLURE_PREFIX_LENGTH = len('allureReporting/')
 
 
 ########################################################################
 # Help messages
 
 CP_HELP = '''Get a local copy of a workflow attachment or workflow attachments
 
-Example:
+Examples:
   # Get a local copy of a workflow attachment
   opentf-ctl cp 9ea3be45-ee90-4135-b47f-e66e4f793383:39e68299-8995-4915-9367-1df1ff642159 /target/dir/output_file.ext
 
   # Get a local copy of all workflow attachments in .tar format
   opentf-ctl cp 9ea3be45-ee90-4135-b47f-e66e4f793383:*.tar /target/dir/
 
   # Get a local copy of all surefire-xml typed workflow attachments
@@ -80,58 +78,53 @@
   opentf-ctl get attachments 9ea3be45-ee90-4135-b47f-e66e4f793383 --verbose
 
 Options:
   --output={yaml,json} or -o {yaml,json}: show information as YAML or JSON.
   --output=wide or -o wide: show additional information (channel OS, attachment type and creation time).
   --output=custom-columns= or -o custom-columns=: show specified information.
     (more at: https://opentestfactory.org/tools/running-commands#output-formats)
-  --verbose or -v: show attachments source files (i.e. workflow Allure report source files)
+  --verbose or -v: show attachments source files (i.e., workflow Allure report source files)
 
 Usage:
   opent-ctl get attachments WORKFLOW_ID [--output=wide] [options]
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
 '''
 
 ########################################################################
 # Helpers
 
 
-def _fatal(*msg) -> NoReturn:
-    _error(*msg)
-    sys.exit(2)
-
-
 def _get_attachment_uuids(workflow_id: str) -> List[str]:
     attachments = _get_attachments_dict(workflow_id, True)
     return [attachment['uuid'] for attachment in attachments.values()]
 
 
 def _get_options(options: List[str]) -> Tuple[str, str, str]:
+    """Parse command line.
+
+    Returns workflow_id, attachment_id or spec, destination filepath.
+    """
     workflow_id, _, attachment_id = options[0].partition(':')
     if not workflow_id or not attachment_id or len(options) != 2:
-        _error(
+        _fatal(
             'Invalid parameters. Was expecting WORKFLOW_ID:ATTACHMENT_ID DESTINATION_FILEPATH, got: %s.',
             ' '.join(options),
         )
-        sys.exit(2)
     workflow_id = _ensure_uuid(workflow_id, _get_workflows)
     if any(wildcard in attachment_id for wildcard in WILDCARDS):
         return (workflow_id, attachment_id, options[1])
-    if attachment_id.endswith(ENDINGS):
-        ending = attachment_id[-2:]
-        attachment_id = _ensure_uuid(attachment_id[:-2], _get_workflows) + ending
-    else:
-        attachment_id = _ensure_uuid(
-            attachment_id, lambda: _get_attachment_uuids(workflow_id)
-        )
+    attachment_id = _ensure_uuid(
+        attachment_id, lambda: _get_attachment_uuids(workflow_id)
+    )
     return (workflow_id, attachment_id, options[1])
 
 
 def _get_download_name(headers, attachment_id: str) -> str:
+    """Try to get name based on Content-Disposition header."""
     _, _, name_with_uuid = headers.get('Content-Disposition', '').partition('name=')
     if name_with_uuid.startswith(attachment_id):
         return name_with_uuid[UUID_LENGTH + 1 :]
     return 'untitled'
 
 
 ########################################################################
@@ -154,15 +147,23 @@
             response.status_code,
             response.json().get('message'),
         )
 
     return response
 
 
-def _save_attachment_stream(response, attachment_id, filepath):
+def _save_attachment_stream(response, attachment_id: str, filepath: str) -> None:
+    """Save attachment to file or directory.
+
+    #  Required parameters
+
+    - response: a Response object
+    - attachment_id: a string
+    - filepath: a string, the file or directory path
+    """
     filename = _get_download_name(response.headers, attachment_id)
     if os.path.isdir(filepath):
         filepath += f'/{filename}'
     with open(os.path.normpath(filepath), 'wb') as file:
         for chunk in response.iter_content(chunk_size=128):
             file.write(chunk)
     print(f'Attachment {filename} ({attachment_id}) is downloaded as {filepath}.')
@@ -183,14 +184,19 @@
 
 
 ########################################################################
 # Handle multiple attachments
 
 
 def _matches_type(filetype: Optional[str], pattern: Optional[str]) -> bool:
+    """Check if filetype matches pattern.
+
+    If no pattern specified, returns True.  Otherwise, return False if
+    no filetype specified.  Compare filetype with pattern.
+    """
     if not pattern:
         return True
     if not filetype:
         return False
     return fnmatch.fnmatch(filetype, pattern)
 
 
@@ -208,24 +214,24 @@
         'filename': data['filename'],
     }
 
 
 def _get_attachments_paths(
     attachments: Dict[str, Any], name_pattern: str, type_pattern: Optional[str]
 ) -> Dict[str, Any]:
-    attachments = {
-        uuid: data
+    result = {
+        uuid: _make_target_path(data)
         for uuid, data in attachments.items()
         if fnmatch.fnmatch(data['filename'], name_pattern)
         and _matches_type(data.get('type'), type_pattern)
     }
-    if not attachments:
+    if not result:
         _error('No attachment matching pattern found.')
         sys.exit(1)
-    return {uuid: _make_target_path(data) for uuid, data in attachments.items()}
+    return result
 
 
 def download_attachments(workflow_id: str, pattern: str, filepath: str) -> None:
     """Download multiple attachments to filepath."""
     if os.path.isfile(filepath):
         _error(
             'File path `%s` is a file, not directory. Can not download multiple attachments to a file, aborting.',
@@ -274,21 +280,19 @@
     'step_sequence_id',
 )
 JOB_KEYS = ('namespace', 'channel_os', 'channel_id', 'job_id', 'job_origin')
 
 EventsList = List[Dict[str, Any]]
 
 
-def _get_file_name(kind: str, attachment: str) -> str:
+def _get_file_name(attachment: str) -> str:
     file = attachment[ATTACHMENT_PREFIX_LENGTH:]
-    if kind == 'ExecutionResult':
-        return file.split('_', maxsplit=2)[2]
     if 'allure' in attachment:
         return file[ALLURE_PREFIX_LENGTH + UUID_LENGTH + 1 :]
-    return file[UUID_LENGTH + 1 :]
+    return file.split('_', maxsplit=2)[2]
 
 
 def _complete_job_and_parent_step(
     attachment: Dict[str, Any],
     parents: EventsList,
     commands: EventsList,
 ) -> Dict[str, Optional[str]]:
@@ -323,33 +327,23 @@
             .get('opentestfactory.org/hooks', {})
             .get('channel')
         }
     attachment['parent_step'] = parent_step
     return attachment
 
 
-def _get_uuid_and_filetype(kind, attachment, metadata):
-    if kind == 'ExecutionResult':
+def _get_uuid_and_filetype(attachment, metadata):
+    if not 'allure' in attachment:
         properties = metadata.get('attachments', {}).get(attachment, {})
         return properties['uuid'], properties.get('type')
-
-    # WorkflowResult
-    uuid = metadata['workflow_id']
-    if 'allure' in attachment:
-        uuid += ALLURE_ENDING
-        filetype = None
-    else:
-        uuid += GLOBAL_ENDING
-        filetype = metadata['attachments'][attachment].get('type')
-    return uuid, filetype
+    return metadata['workflow_id'], None
 
 
 def _get_attachment_data_steps(
-    workflow_id: str,
-    verbose: bool,
+    workflow_id: str, verbose: bool
 ) -> Tuple[EventsList, EventsList, EventsList]:
     events = _get_workflow_attachments_events(workflow_id, verbose)
     results = [
         event
         for event in events
         if event['kind'] in ('ExecutionResult', 'WorkflowResult')
     ]
@@ -373,48 +367,49 @@
         msg=msg,
         statuses=(200, 404),
     )
 
     return response.status_code == 200
 
 
-def _add_attachment_metadata(event, data):
+def _add_attachment_metadata(
+    event: Dict[str, Any], data: Dict[str, Any]
+) -> Dict[str, Any]:
     metadata = event['metadata']
     for key, value in metadata.items():
         if key in METADATA_KEYS:
-            data['metadata'].update({key: value})
+            data['metadata'][key] = value
         elif key in JOB_KEYS:
-            data['job'].update({key: value})
-        data['status'] = event.get('status', 0)
-        if data['status'] != 0:
-            data['message'] = '\n'.join(event.get('logs', []))
+            data['job'][key] = value
+    data['status'] = event.get('status', 0)
+    if data['status'] != 0:
+        data['message'] = '\n'.join(event.get('logs', []))
     return data
 
 
 def _get_attachments_dict(workflow_id: str, verbose: bool) -> Dict[str, Any]:
     results, parents, commands = _get_attachment_data_steps(workflow_id, verbose)
     attachments = {}
     for event in results:
         for attachment in event['attachments']:
             metadata = event['metadata']
-            kind = event['kind']
-            uuid, filetype = _get_uuid_and_filetype(kind, attachment, metadata)
+            uuid, filetype = _get_uuid_and_filetype(attachment, metadata)
 
             data = {
                 'uuid': uuid,
-                'filename': _get_file_name(kind, attachment),
+                'filename': _get_file_name(attachment),
                 'type': filetype,
                 'metadata': {},
                 'job': {},
                 'parent_step': {},
             }
 
             _add_attachment_metadata(event, data)
 
-            if kind == 'ExecutionResult':
+            if event['kind'] == 'ExecutionResult':
                 _complete_job_and_parent_step(data, parents, commands)
             if data['status'] != 0 and _file_exists(uuid, workflow_id):
                 data['status'] = 0
                 del data['message']
             attachments[uuid] = data
     return attachments
```

## opentf/tools/ctlcommons.py

```diff
@@ -28,14 +28,19 @@
 # debug
 
 
 def _error(*msg) -> None:
     logging.error(*msg)
 
 
+def _fatal(*msg) -> NoReturn:
+    _error(*msg)
+    sys.exit(2)
+
+
 def _warning(*msg) -> None:
     logging.warning(*msg)
 
 
 def _debug(*msg) -> None:
     logging.debug(*msg)
```

## opentf/tools/ctlconfig.py

```diff
@@ -19,15 +19,21 @@
 import os
 import sys
 
 from importlib.metadata import version
 
 import yaml
 
-from opentf.tools.ctlcommons import _is_command, _get_arg, _error, _ensure_options
+from opentf.tools.ctlcommons import (
+    _is_command,
+    _get_arg,
+    _error,
+    _fatal,
+    _ensure_options,
+)
 
 
 ########################################################################
 
 # pylint: disable=broad-except
 
 CONFIG = {}
@@ -103,15 +109,15 @@
 
 Usage:
   opentf-ctl config use-context CONTEXT_NAME
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
 '''
 
-CONFIG_SET_CONTEXT_HELP = '''Sets a context entry in opentfconfig
+CONFIG_SET_CONTEXT_HELP = '''Set a context entry in opentfconfig
 
  Specifying a name that already exists will merge new fields on top of existing values for those fields.
 
 Examples:
   # Set the user field on the foo context entry without touching other values
   opentf-ctl config set-context foo --user=admin
 
@@ -120,15 +126,15 @@
 
 Usage:
   opentf-ctl config set-context [NAME | --current] [--orchestrator=orchestrator_nickname] [--user=user_nickname] [--namespace=namespace] [options]
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
 '''
 
-CONFIG_SET_ORCHESTRATOR_HELP = '''Sets an orchestrator entry in opentfconfig
+CONFIG_SET_ORCHESTRATOR_HELP = '''Set an orchestrator entry in opentfconfig
 
  Specifying a name that already exists will merge new fields on top of existing values.
 
 Examples:
   # Set only the server field of the e2e orchestrator entry without touching other values.
   opentf-ctl config set-orchestrator e2e --server=https://1.2.3.4
 
@@ -138,23 +144,23 @@
 Options:
   --insecure-skip-tls-verify=false|true: Skip TLS verification
   --server='': Address of the opentf orchestrator
   --SERVICE-force-base-url=false|true: Override link URLs
   --SERVICE-port='': Port of the service (integer)
   --SERVICE-prefix='': Prefix for the service (string)
 
-  where SERVICE is one of 'receptionist', 'observer', 'eventbus', 'killswitch', 'agentchannel', 'localstore' or 'qualitygate'.
+  where SERVICE is one of 'receptionist', 'observer', 'eventbus', 'killswitch', 'agentchannel', 'localstore', or 'qualitygate'.
 
 Usage:
   opentf-ctl config set-orchestrator NAME [--insecure-skip-tls-verify=true] [--server=server] [--SERVICE-port=port] [--SERVICE-prefix=prefix] [--SERVICE-force-base-url=boolean] [options]
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
 '''
 
-CONFIG_SET_CREDENTIALS_HELP = '''Sets a user entry in opentfconfig
+CONFIG_SET_CREDENTIALS_HELP = '''Set a user entry in opentfconfig
 
  Specifying a name that already exists will merge new fields on top of existing values.
 
   Bearer token flags:
     --token=bearer_token
 
 Examples:
@@ -219,16 +225,15 @@
 '''
 
 
 ########################################################################
 
 
 def _fatal_cannot_modify_configuration_file(filename: str, err) -> NoReturn:
-    _error('Could not modify configuration file %s: %s.', filename, err)
-    sys.exit(2)
+    _fatal('Could not modify configuration file %s: %s.', filename, err)
 
 
 def read_configuration() -> None:
     """Read configuration file.
 
     Configuration file is by default ~/.opentf/config, but this can be
     overridden by specifying the OPENTF_CONFIG environment variable or
@@ -280,49 +285,44 @@
                 return item[kind]
         return None
 
     def _safe_get(kind: str, name: str) -> Dict[str, Any]:
         what = _get(kind, name)
         if what is None:
             _error('%s %s is not available in configuration.', kind.title(), repr(name))
-            _error('(Using the %s configuration file.)', repr(_))
-            sys.exit(2)
+            _fatal('(Using the %s configuration file.)', repr(_))
         return what
 
     def _safe_get_arg(option: str) -> Optional[str]:
         what = _get_arg(option)
         if what == '':
-            _error('The %s option specifies an empty value.', option)
-            sys.exit(2)
+            _fatal('The %s option specifies an empty value.', option)
         return what
 
     _, config = _read_opentfconfig()
 
     context_name = _safe_get_arg('--context=') or config.get('current-context')
     if not context_name:
-        _error(
+        _fatal(
             'Empty or undefined current context.  Please specify a current context in your configuration file or use the --context= command line option.'
         )
-        sys.exit(2)
     context = _safe_get('context', context_name)
 
     orchestrator_name = _safe_get_arg('--orchestrator=') or context.get('orchestrator')
     if not orchestrator_name:
-        _error(
+        _fatal(
             'No orchestrator defined in the context.  Please specify an orchestrator in your configuration file or use the --orchestrator= command line option.'
         )
-        sys.exit(2)
     orchestrator = _safe_get('orchestrator', orchestrator_name)
 
     user_name = _safe_get_arg('--user=') or context.get('user')
     if not user_name:
-        _error(
+        _fatal(
             'No user defined in the context.  Please specify a user in your configuration file or use the --user= command line option.'
         )
-        sys.exit(2)
     user = _safe_get('user', user_name)
 
     try:
         CONFIG['token'] = (
             _get_arg('--token=') or os.environ.get('OPENTF_TOKEN') or user['token']
         )
         CONFIG['job-depth'] = user.get('job-depth')
@@ -331,16 +331,15 @@
         CONFIG['orchestrator'] = orchestrator
         CONFIG['orchestrator']['insecure-skip-tls-verify'] = CONFIG['orchestrator'].get(
             'insecure-skip-tls-verify', False
         ) or (_get_arg('--insecure-skip-tls-verify=') == 'true')
         CONFIG['namespace'] = context.get('namespace')
         HEADERS['Authorization'] = 'Bearer ' + CONFIG['token']
     except Exception as err:
-        _error('Could not read configuration: %s.', err)
-        sys.exit(2)
+        _fatal('Could not read configuration: %s.', err)
 
 
 ########################################################################
 # Helpers
 
 
 def _get_port(service: str, default: int) -> int:
@@ -348,16 +347,15 @@
         _get_arg(f'--orchestrator-{service}-port=')
         or input(f'Please specify the {service} port ({default}): ').strip()
         or default
     )
     try:
         return int(port)
     except ValueError as err:
-        _error('Not a valid port value: %s', err)
-        sys.exit(2)
+        _fatal('Not a valid port value: %s', err)
 
 
 ########################################################################
 # Commands
 
 
 ## config commands
@@ -375,32 +373,30 @@
         or os.path.expanduser('~/.opentf/config')
     )
     try:
         with open(conf_filename, 'r', encoding='utf-8') as conffile:
             config = yaml.safe_load(conffile)
     except Exception as err:
         _error('Could not read configuration file %s: %s.', conf_filename, err)
-        _error(
+        _fatal(
             'You may generate a configuration file using the "opentf-ctl config generate" subcommand.  Use "opentf-ctl config generate --help" for usage.'
         )
-        sys.exit(2)
     return conf_filename, config
 
 
 def _ensure_name_exists(name: str, label: str, config, src) -> None:
     names = [item['name'] for item in config[f'{label}s']]
     if name not in names:
         _error(
             '%s %s does not exist in configuration file %s.',
             label.title(),
             repr(name),
             repr(src),
         )
-        _error('Available %ss: %s.', label, ','.join(names))
-        sys.exit(2)
+        _fatal('Available %ss: %s.', label, ','.join(names))
 
 
 # Contexts
 
 
 def use_context(name: str) -> None:
     """Change current context."""
@@ -419,18 +415,17 @@
     try:
         if name == '--current':
             if 'current-context' not in config:
                 _error(
                     'No current context defined in configuration file %s.',
                     conf_filename,
                 )
-                _error(
+                _fatal(
                     'You can use the "opentf-ctl config use-context" subcommand to define a default context.'
                 )
-                sys.exit(2)
             name = config['current-context']
         contexts = {item['name']: item for item in config['contexts']}
         if name not in contexts:
             entry = {'context': {}, 'name': name}
             contexts[name] = entry
             config['contexts'].append(entry)
             msg = f'Context "{name}" created in {conf_filename}.'
@@ -571,27 +566,25 @@
             'qualitygate',
             'localstore',
         ]:
             if port := _get_arg(f'--{svc}-port='):
                 try:
                     port = int(port)
                 except ValueError:
-                    _error('%s port must be an integer: %s.', svc.title(), repr(port))
-                    sys.exit(2)
+                    _fatal('%s port must be an integer: %s.', svc.title(), repr(port))
                 ports[svc] = port
             if prefix := _get_arg(f'--{svc}-prefix='):
                 prefixes[svc] = prefix
             if baseurl := _get_arg(f'--{svc}-force-base-url='):
                 if baseurl.lower() not in ('true', 'false'):
-                    _error(
+                    _fatal(
                         '%s force-base-url must be "true" or "false": %s.',
                         svc.title(),
                         repr(baseurl),
                     )
-                    sys.exit(2)
                 forcebaseurls[svc] = baseurl.lower() == 'true'
         if ports or prefixes or forcebaseurls:
             if 'ports' in orchestrator:
                 # update to new orchestrator definition format
                 services = {
                     svc: {'port': value} for svc, value in orchestrator['ports'].items()
                 }
@@ -679,25 +672,25 @@
     - name: default
       user:
         token: ey...
     ```
 
     Optional command-line options:
 
-    --name="
+    --name=''
     --orchestrator-server=''
     --orchestrator-receptionist-port=''
     --orchestrator-observer-port=''
     --orchestrator-eventbus-port=''
     --orchestrator-killswitch-port=''
     --orchestrator-agentchannel-port=''
     --orchestrator-qualitygate-port=''
     --orchestrator-localstore-port=''
     --insecure-skip-tls-verify=false|true
-    --token="
+    --token=''
     """
 
     generated_conf: Dict[str, Any] = {
         'apiVersion': 'opentestfactory.org/v1alpha1',
         'kind': 'CtlConfig',
     }
 
@@ -727,19 +720,18 @@
     if isinstance(skip_tls_verify, str):
         verify = skip_tls_verify.lower().strip()
         if verify == 'true':
             skip_tls_verify = True
         elif verify == 'false':
             skip_tls_verify = False
         else:
-            _error(
+            _fatal(
                 'Not a valid insecure-skip-tls-verify flag: %s (was expecting true or false).',
                 skip_tls_verify,
             )
-            sys.exit(2)
 
     token = _get_arg('--token=')
     while not token:
         token = input('Please specify the token: ').strip()
 
     contexts = [{'name': name, 'context': {'orchestrator': name, 'user': name}}]
```

## opentf/tools/ctlnetworking.py

```diff
@@ -18,15 +18,15 @@
 
 import sys
 
 from urllib.parse import urlparse
 
 import requests
 
-from opentf.tools.ctlcommons import _error, _debug
+from opentf.tools.ctlcommons import _error, _fatal, _debug
 from opentf.tools.ctlconfig import CONFIG, HEADERS
 
 
 ########################################################################
 
 
 def _make_hostport(service: str) -> str:
@@ -91,22 +91,26 @@
     return _make_hostport('eventbus')
 
 
 def _agentchannel() -> str:
     return _make_hostport('agentchannel')
 
 
-def _qualitygate():
+def _qualitygate() -> str:
     return _make_hostport('qualitygate')
 
 
-def _localstore():
+def _localstore() -> str:
     return _make_hostport('localstore')
 
 
+def _insightcollector() -> str:
+    return _make_hostport('insightcollector')
+
+
 ########################################################################
 
 
 def _get(
     base_url: str,
     path: str = '',
     msg: Optional[str] = None,
@@ -150,16 +154,15 @@
             handler(what)
         else:
             _error(msg + ', got %d: %s.', what.status_code, what.text)
             sys.exit(1)
     except requests.exceptions.ConnectionError as err:
         _could_not_connect(base_url, err)
     except Exception as err:
-        _error(msg + ': %s.', err)
-        sys.exit(2)
+        _fatal(msg + ': %s.', err)
 
     return what
 
 
 def _get_json(
     base_url: str,
     path: str = '',
@@ -192,18 +195,17 @@
         msg,
         statuses=statuses,
         handler=handler,
         params=params,
         raw=False,
     )
     if not isinstance(result, dict):
-        _error(
+        _fatal(
             'Internal error, was expecting a dictionary, got a %s.', result.__class__
         )
-        sys.exit(2)
     return result
 
 
 def _get_file(
     base_url: str,
     path: str = '',
     msg: Optional[str] = None,
@@ -240,16 +242,15 @@
         )
         if what.status_code not in statuses:
             _error(msg + ', got %d: %s.', what.status_code, what.text)
             sys.exit(1)
     except requests.exceptions.ConnectionError as err:
         _could_not_connect(base_url, err)
     except Exception as err:
-        _error(msg + ': %s.', err)
-        sys.exit(2)
+        _fatal(msg + ': %s.', err)
 
     return what
 
 
 def _head(
     base_url: str,
     path: str = '',
@@ -287,16 +288,15 @@
         )
         if what.status_code not in statuses:
             _error(msg + ', got %d: %s.', what.status_code, what.text)
             sys.exit(1)
     except requests.exceptions.ConnectionError as err:
         _could_not_connect(base_url, err)
     except Exception as err:
-        _error(msg + ': %s.', err)
-        sys.exit(2)
+        _fatal(msg + ': %s.', err)
 
     return what
 
 
 def _post(
     base_url: str,
     path: str = '',
@@ -344,16 +344,15 @@
             handler(what)
         else:
             _error(msg + ', got %d: %s.', what.status_code, what.text)
             sys.exit(1)
     except requests.exceptions.ConnectionError as err:
         _could_not_connect(base_url, err)
     except Exception as err:
-        _error(msg + ': %s.', err)
-        sys.exit(2)
+        _fatal(msg + ': %s.', err)
 
     return what  # type: ignore
 
 
 def _delete(
     base_url: str,
     path: str = '',
@@ -380,16 +379,15 @@
             sys.exit(1)
         else:
             _error(msg + ', got %d: %s.', what.status_code, what.text)
             sys.exit(1)
     except requests.exceptions.ConnectionError as err:
         _could_not_connect(base_url, err)
     except Exception as err:
-        _error(base_url + ': %s.', err)
-        sys.exit(2)
+        _fatal(base_url + ': %s.', err)
 
     return what
 
 
 ########################################################################
 
 
@@ -408,16 +406,15 @@
             + ' purpose only.**)'
         )
     else:
         _error(
             'Could not reach the orchestrator (%s).  Is the orchestrator running?',
             str(err),
         )
-    _error('(Attempting to reach %s.)', target)
-    sys.exit(2)
+    _fatal('(Attempting to reach %s.)', target)
 
 
 ########################################################################
 
 
 def _handle_maybe_outdated(response) -> NoReturn:
     if response.status_code in (404, 405):
@@ -437,17 +434,15 @@
         '/workflows',
         'Could not get workflows list',
         handler=_handle_maybe_outdated,
         params=params,
         raw=True,
     )
     if params and not response.headers.get('X-Processed-Query'):
-        _error(
+        _fatal(
             'The orchestrator does not support selectors, please specify explicit workflow IDs or upgrade your orchestrator.'
         )
-        sys.exit(2)
     try:
         result = response.json()
     except Exception as err:
-        _error('Could not get workflows list: %s.', err)
-        sys.exit(2)
+        _fatal('Could not get workflows list: %s.', err)
     return result['details']['items']
```

## opentf/tools/ctlqualitygate.py

```diff
@@ -10,27 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """opentf-ctl quality gate handling part"""
 
-from typing import Any, Dict, List, NoReturn, Optional
+from typing import Any, Dict, List, Optional
 
 import os
 import sys
 
 from opentf.tools.ctlcommons import (
     _ensure_options,
     _file_not_found,
     _is_command,
     _get_arg,
     generate_output,
     _ensure_uuid,
     _error,
+    _fatal,
     _warning,
 )
 
 from opentf.tools.ctlconfig import read_configuration
 from opentf.tools.ctlnetworking import (
     _qualitygate,
     _get_json,
@@ -131,22 +132,14 @@
 }
 
 
 ########################################################################
 # Helpers
 
 
-def _fatal(*msg) -> NoReturn:
-    _error(*msg)
-    sys.exit(2)
-
-
-########################################################################
-
-
 def _describe_qualitygate(workflow_id: str, mode: str, status: Dict[str, Any]) -> None:
     """Get quality gate results for a workflow in a pretty form."""
     for rule, data in status.items():
         if data['result'] not in (SUCCESS, NOTEST, FAILURE, INVALIDSCOPE):
             _error(
                 f'Unexpected quality gate result when applying rule `{rule}`: {data["result"]} (was expecting {", ".join(STATUS_TEMPLATES)}).'
             )
```

## opentf/tools/ctltokens.py

```diff
@@ -21,14 +21,15 @@
 from datetime import datetime
 
 import jwt
 
 from opentf.tools.ctlcommons import (
     _is_command,
     _error,
+    _fatal,
     _warning,
 )
 
 ########################################################################
 
 # pylint: disable=broad-except
 
@@ -96,48 +97,42 @@
 
     try:
         with open(privatekey, 'rb') as keyfile:
             pem = keyfile.read()
         try:
             return serialization.load_pem_private_key(pem, None, default_backend())
         except ValueError as err:
-            _error(
+            _fatal(
                 'This does not seem to be a valid private key in PEM format: %s.', err
             )
-            sys.exit(2)
         except TypeError:
             from getpass import getpass
 
             try:
                 passphrase = getpass(
                     'This private key is encrypted, please enter the passphrase: '
                 )
                 if not passphrase:
-                    _error('Passphrase cannot be empty, the private key is encrypted.')
-                    sys.exit(2)
+                    _fatal('Passphrase cannot be empty, the private key is encrypted.')
                 return serialization.load_pem_private_key(
                     pem, passphrase.encode('utf-8'), backend=default_backend()
                 )
             except ValueError as err:
-                _error(str(err))
-                sys.exit(2)
+                _fatal(str(err))
     except UnsupportedAlgorithm as err:
-        _error(
+        _fatal(
             'The serialized key type is not supported by the OpenSSL version "cryptography" is using: %s.',
             err,
         )
-        sys.exit(2)
     except IsADirectoryError:
-        _error(
+        _fatal(
             'The specified private key must be a file, not a directory: %s.', privatekey
         )
-        sys.exit(2)
     except FileNotFoundError:
-        _error('The specified private key could not be found: %s.', privatekey)
-        sys.exit(2)
+        _fatal('The specified private key could not be found: %s.', privatekey)
 
 
 def _generate_token(privatekey: str) -> None:
     private_key = _load_pem_private_key(privatekey)
     algorithm = (
         input('Please specify an algorithm (RS512 if unspecified): ').strip() or 'RS512'
     )
@@ -160,28 +155,25 @@
         ).strip()
         or None
     )
     if exp:
         try:
             exp = int(datetime.strptime(exp, '%Y/%m/%d').timestamp())
         except ValueError:
-            _error('Invalid expiration date format, must be YYYY/MM/DD.')
-            sys.exit(2)
+            _fatal('Invalid expiration date format, must be YYYY/MM/DD.')
 
     try:
         payload: Dict[str, Union[str, int]] = {'iss': issuer, 'sub': subject}
         if exp:
             payload['exp'] = exp
         token = jwt.encode(payload, private_key, algorithm=algorithm)
     except NotImplementedError:
-        _error('Algorithm not supported: %s.', algorithm)
-        sys.exit(2)
+        _fatal('Algorithm not supported: %s.', algorithm)
     except Exception as err:
-        _error('Could not generate token: %s.', err)
-        sys.exit(2)
+        _fatal('Could not generate token: %s.', err)
 
     print('The signed token is:')
     print(token)
 
 
 def generate_token(privatekey: str) -> None:
     """Generate JWT token.
@@ -236,42 +228,37 @@
 
     Abort with an error code 2 if something went wrong.
     """
     try:
         with open(keyname, 'r', encoding='utf-8') as keyfile:
             key = keyfile.read()
     except IsADirectoryError:
-        _error('The specified public key must be a file, not a directory: %s.', keyname)
-        sys.exit(2)
+        _fatal('The specified public key must be a file, not a directory: %s.', keyname)
     except FileNotFoundError:
-        _error('The specified public key could not be found: %s.', keyname)
-        sys.exit(2)
+        _fatal('The specified public key could not be found: %s.', keyname)
 
     try:
         payload = jwt.decode(token, key, algorithms=ALLOWED_ALGORITHMS)
         print(
             f'The token is signed by the {keyname} public key.  The token payload is:'
         )
         print(payload)
     except jwt.exceptions.InvalidSignatureError:
         _error('The token is not signed by %s.', keyname)
         sys.exit(102)
     except (TypeError, AttributeError) as err:
-        _error(
+        _fatal(
             'The specified key does not looks like a public key.'
             + '  Got "%s" while reading the provided key.',
             err,
         )
-        sys.exit(2)
     except ValueError as err:
-        _error(err.args[0])
-        sys.exit(2)
+        _fatal(err.args[0])
     except Exception as err:
-        _error('Could not validate token signature: %s.', err)
-        sys.exit(2)
+        _fatal('Could not validate token signature: %s.', err)
 
 
 ########################################################################
 # Helpers
 
 
 def print_tokens_help(args: List[str]) -> None:
@@ -291,35 +278,31 @@
 # Main
 
 
 def tokens_cmd():
     """Process tokens command."""
     if _is_command('generate token using _', sys.argv):
         if len(sys.argv) > 5:
-            _error(
+            _fatal(
                 f'"opentf-ctl generate token" does not take options.  Got "{" ".join(sys.argv[5:])}".'
             )
-            sys.exit(2)
         generate_token(sys.argv[4])
         sys.exit(0)
     if _is_command('view token _', sys.argv):
         if len(sys.argv) > 4:
-            _error(
+            _fatal(
                 f'"opentf-ctl view token" does not take options.  Got "{" ".join(sys.argv[4:])}".'
             )
-            sys.exit(2)
         view_token(sys.argv[3])
         sys.exit(0)
     if _is_command('check token _ using _', sys.argv):
         if len(sys.argv) > 6:
-            _error(
+            _fatal(
                 f'"opentf-ctl check token" does not take options.  Got "{" ".join(sys.argv[6:])}".'
             )
-            sys.exit(2)
         check_token(sys.argv[3], sys.argv[5])
         sys.exit(0)
     if _is_command('check token _', sys.argv):
-        _error('Missing required parameter.  Use "check token --help" for details.')
-        sys.exit(2)
+        _fatal('Missing required parameter.  Use "check token --help" for details.')
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
```

## opentf/tools/ctlworkflows.py

```diff
@@ -31,14 +31,15 @@
     _ensure_options,
     _file_not_found,
     _is_command,
     _get_arg,
     generate_output,
     _ensure_uuid,
     _error,
+    _fatal,
     _warning,
     UUID_REGEX,
 )
 from opentf.tools.ctlconfig import read_configuration, CONFIG
 from opentf.tools.ctlnetworking import (
     _observer,
     _receptionist,
@@ -248,19 +249,18 @@
     Abort with an error code 2 if the file does not exist or contains
     invalid content.
     """
     try:
         with open(file, 'r', encoding='utf-8') as varfile:
             for line in varfile:
                 if '=' not in line:
-                    _error(
+                    _fatal(
                         'Invalid format in file %s, was expecting var=value.',
                         file,
                     )
-                    sys.exit(2)
                 var, _, value = line.strip().partition('=')
                 variables[var] = value
     except FileNotFoundError as err:
         _file_not_found(file, err)
 
 
 def _add_files(args: List[str], files: Dict[str, Any]) -> None:
@@ -414,25 +414,23 @@
             _receptionist(),
             '/workflows' + (f'?namespace={ns}' if ns is not None else ''),
             files=files,
             statuses=(201,),
             handler=_handle_maybe_details,
         )
         if not isinstance(result, dict):
-            _error(
+            _fatal(
                 'Internal error: was expecting a dictionary, got a %s while querying /workflows.',
                 result.__class__,
             )
-            sys.exit(2)
         print('Workflow', result['details']['workflow_id'], 'is running.')
     except FileNotFoundError as err:
         _file_not_found(workflow_name, err)
     except Exception as err:
-        _error('Could not start workflow: %s.', err)
-        sys.exit(2)
+        _fatal('Could not start workflow: %s.', err)
 
     workflow_done = False
     watch_args = ['--wait', '--watch', '-w']
     qualitygate_args = ['--mode', '-m']
     if _is_sys_argv(watch_args) or _is_sys_argv(qualitygate_args):
         url = (
             _observer()
@@ -448,16 +446,15 @@
                 sleep(WAIT_DELAY)
             if _is_sys_argv(watch_args):
                 get_workflow(result['details']['workflow_id'], watch=True)
                 workflow_done = True
             if _is_sys_argv(qualitygate_args):
                 _apply_qualitygate(result['details']['workflow_id'], workflow_done)
         except Exception as err:
-            _error('Could not show workflow execution result: %s.', err)
-            sys.exit(2)
+            _fatal('Could not show workflow execution result: %s.', err)
 
 
 def _emit_prefix(event: Dict[str, Any], file=sys.stdout) -> None:
     cts = event['metadata'].get('creationTimestamp')
     job_id = event['metadata'].get('job_id')
     print(
         f'[{cts[:19] if cts else "":19}]',
@@ -506,18 +503,17 @@
     if '--show-notifications' not in sys.argv and '-a' not in sys.argv:
         return
     if 'spec' in event and 'logs' in event['spec']:
         verbosity = ('-v' in sys.argv) or ('--verbose' in sys.argv)
         for log in event['spec']['logs']:
             if TIMESTAMP_PATTERN.match(log):
                 log = log[26:]
-            if (
-                log.startswith('[DEBUG]')
-                or log.startswith('DEBUG')
-                or '] DEBUG in' in log
+            if any(
+                log.startswith((x, f'[{x}]')) or f'] {x} in' in log
+                for x in ('DEBUG', 'TRACE')
             ):
                 if silent or not verbosity:
                     continue
             _emit_prefix(event, file=file)
             if event['metadata']['name'] != 'log notification':
                 print(f'[{event["metadata"]["name"]}] {log}', file=file)
             else:
@@ -545,32 +541,24 @@
 
 
 def _maybe_emit_attachment(
     event: Dict[str, Any], silent: bool, file=sys.stdout
 ) -> None:
     if 'Errno 2' in ''.join(event.get('logs', [])):
         return
-    kind = event.get('kind')
-    if kind == 'WorkflowResult':
-        for attachment in event['attachments']:
+    for attachment in event['attachments']:
+        if 'allure' in attachment:
             uuid = event['metadata']['workflow_id']
-            if 'allure' in attachment:
-                uuid += '_a'
-                name = attachment[
-                    ATTACHMENT_PREFIX_LENGTH + ALLURE_PREFIX_LENGTH + UUID_LENGTH + 1 :
-                ]
-            else:
-                uuid += '_e'
-                name = attachment[ATTACHMENT_PREFIX_LENGTH + UUID_LENGTH + 1 :]
-            _emit_attachment_info(event, silent, name, uuid, file)
-    elif kind == 'ExecutionResult':
-        for path, properties in event['metadata'].get('attachments', {}).items():
-            name = path[ATTACHMENT_PREFIX_LENGTH:].split('_', maxsplit=2)[2]
-            uuid = properties.get('uuid')
-            _emit_attachment_info(event, silent, name, uuid, file)
+            name = attachment[
+                ATTACHMENT_PREFIX_LENGTH + ALLURE_PREFIX_LENGTH + UUID_LENGTH + 1 :
+            ]
+        else:
+            name = attachment[ATTACHMENT_PREFIX_LENGTH:].split('_', maxsplit=2)[2]
+            uuid = event['metadata']['attachments'][attachment].get('uuid')
+        _emit_attachment_info(event, silent, name, uuid, file)
 
 
 def _maybe_emit_testcase_name(event: Dict[str, Any]) -> str:
     if event.get('step', {}).get('with', {}).get('test'):
         return f" for test reference `{event['step']['with']['test']}`:"
     return ''
 
@@ -716,23 +704,21 @@
     )
 
 
 def _get_outputformat(allowed: Iterable[str]) -> Optional[str]:
     """Ensure the specified format, if any, is in the allowed set."""
     output_format = _get_arg('--output=') or _get_arg('-o=')
     if '-o' in sys.argv and not output_format:
-        _error('Missing value for option "-o" (was expecting %s).', ', '.join(allowed))
-        sys.exit(2)
+        _fatal('Missing value for option "-o" (was expecting %s).', ', '.join(allowed))
     if output_format is not None and output_format not in allowed:
-        _error(
+        _fatal(
             'Unexpected output format specified: %s (was expecting %s).',
             output_format,
             ', '.join(allowed),
         )
-        sys.exit(2)
     return output_format
 
 
 def _get_workflow_events(workflow_id: str, watch: bool) -> Iterable[Dict[str, Any]]:
     """Yield events.
 
     If `watch` is True, yields events as they come, til the workflow
@@ -873,38 +859,35 @@
     """
     job_depth = _get_arg('--job-depth=') or _get_arg('-j=') or CONFIG.get('job-depth')
     if job_depth is None:
         job_depth = 1
     try:
         job_depth = int(job_depth)
     except ValueError:
-        _error(f'--job-depth must be an integer.  Got: {job_depth}.')
-        sys.exit(2)
+        _fatal(f'--job-depth must be an integer.  Got: {job_depth}.')
     step_depth = (
         _get_arg('--step-depth=') or _get_arg('-s=') or CONFIG.get('step-depth')
     )
     if step_depth is None:
         step_depth = 1
     try:
         step_depth = int(step_depth)
     except ValueError:
-        _error(f'--step-depth must be an integer.  Got: {step_depth}.')
-        sys.exit(2)
+        _fatal(f'--step-depth must be an integer.  Got: {step_depth}.')
     max_command_length = (
         _get_arg('--max-command-length=')
         or _get_arg('-c=')
         or CONFIG.get('max-command-length')
     )
     if max_command_length is None:
         max_command_length = MAX_COMMAND_LENGTH
     try:
         max_command_length = int(max_command_length) or None
     except ValueError:
-        _error(f'--max-command-length must be an integer.  Got: {max_command_length}.')
-        sys.exit(2)
+        _fatal(f'--max-command-length must be an integer.  Got: {max_command_length}.')
     return job_depth, step_depth, max_command_length
 
 
 def get_workflow(workflow_id: str, watch=False) -> None:
     """Get a workflow.
 
     # Required parameters
```

## Comparing `opentf_tools-0.45.0.dist-info/LICENSE` & `opentf_tools-0.46.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opentf_tools-0.45.0.dist-info/METADATA` & `opentf_tools-0.46.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: opentf-tools
-Version: 0.45.0
+Version: 0.46.0
 Summary: OpenTestFactory Orchestrator Tools
 Home-page: https://opentestfactory.org/tools/
 Author: Martin Lafaix
 Author-email: mlafaix@henix.com
 Maintainer: Henix
 Maintainer-email: opentestfactory@henix.com
 License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >= 3.8.0
 Description-Content-Type: text/markdown
@@ -47,9 +46,7 @@
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
-
```

## Comparing `opentf_tools-0.45.0.dist-info/RECORD` & `opentf_tools-0.46.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-opentf/tools/ctl.py,sha256=5yH0tQWYPsmEFu43Jacd-8md8GlaRkTbF7SipVj-i2Y,23421
-opentf/tools/ctlattachments.py,sha256=qJZNcrfvfojVcSoENX9se4zY_lOs2ZqbF_XgN6dtwzY,16082
-opentf/tools/ctlcommons.py,sha256=6uOFpPTyehWakDPlsE5mcy1LvYNqsSxNt80uuQFOLGU,16227
-opentf/tools/ctlconfig.py,sha256=VWBoFg5Bp74X3yQHy2taYhpqCMGhgacG9qMOG9ySSws,32399
-opentf/tools/ctlnetworking.py,sha256=GtH24md8L1_QC2ABHz_-TX5M7ld6Ua0rAupG0Fz8v08,12738
+opentf/tools/ctl.py,sha256=Yx9gsPLVKjswyOkTQcSwPyyb3WRq-MBk_BA7gD_30sQ,23841
+opentf/tools/ctlattachments.py,sha256=jua6REgWxAbFbp1vTZ1Rw3alxqM9g2-pL18A7Ow1pSQ,15915
+opentf/tools/ctlcommons.py,sha256=C6gNksOEVsAOBpS-dW_BXrpRRKPJkCwrc6JdTj_YQoo,16292
+opentf/tools/ctlconfig.py,sha256=8U2g3E2stF7tQHzpOejv-Gdl5Wj3UgPJQxZv03H_k8A,32112
+opentf/tools/ctlgenerate.py,sha256=hbbxKaM3vM1XTHEFJOQhDNHPaunhd1qdv4s7BQNnCu4,7392
+opentf/tools/ctlnetworking.py,sha256=_KoTMOtuRa3N0iXre9jbPllm0dXWTl1dyYK6HzDWa3Y,12664
 opentf/tools/ctlplugin_gitlab.py,sha256=jC4yuWegC_uFzq4GWp83cbzJgm5EYr8t8z3iLiJsXGQ,11840
-opentf/tools/ctlqualitygate.py,sha256=NQ8IehtlhThI3x-xWMGE6347zspv_hf1fJ4zqT5HaDw,13793
-opentf/tools/ctltokens.py,sha256=fRyaKSzHs13yAnZhEzv2eO4pM0A1i42fWLwtR6Acfhk,10092
-opentf/tools/ctlworkflows.py,sha256=tPIt3r856rAt5bBriMTxpEfhQYhFckkcXy49qi0C728,38832
+opentf/tools/ctlqualitygate.py,sha256=cP17ZUzzL2Ejtye2Vxfsqq4lOv-H1JrBFq8rVL7af3A,13655
+opentf/tools/ctltokens.py,sha256=7KqKvSFQ7iMJkmm6J1xneeHPSlfIq6XnUdceAa8sXbI,9704
+opentf/tools/ctlworkflows.py,sha256=UGMCreOf2e1jDMoL0BhVNOPR4ePOtDWR5YBTx07UKOI,38262
 opentf/tools/done.py,sha256=X3W4liZYhStrc42aAVxbbQD1sEz7w1cxtMTWmCCKY9g,3188
 opentf/tools/ready.py,sha256=WHPdnWCMOKLCxLlF0FTCCpW-8y0BF7rrGCl7H2AJ-DM,9391
-opentf_tools-0.45.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-opentf_tools-0.45.0.dist-info/METADATA,sha256=rcOnAFwsaS_4MBsuF8SaJkZmrSx4QJ13m7GaobvLsHg,1783
-opentf_tools-0.45.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-opentf_tools-0.45.0.dist-info/entry_points.txt,sha256=u5qYtmUbgIMcq8360YobnI9CtDvrjptf4lDkmKojoa0,139
-opentf_tools-0.45.0.dist-info/top_level.txt,sha256=_gPuE6GTT6UNXy1DjtmQSfCcZb_qYA2vWmjg7a30AGk,7
-opentf_tools-0.45.0.dist-info/RECORD,,
+opentf_tools-0.46.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+opentf_tools-0.46.0.dist-info/METADATA,sha256=kX5iC3QVhhqj5gyCqw9gyyjT3b52i-RSeWemxZ7OvJs,1763
+opentf_tools-0.46.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+opentf_tools-0.46.0.dist-info/entry_points.txt,sha256=eNngh7_-coAb7IinsgCmqg-qOIj9ztVToC2gau8KTjU,138
+opentf_tools-0.46.0.dist-info/top_level.txt,sha256=_gPuE6GTT6UNXy1DjtmQSfCcZb_qYA2vWmjg7a30AGk,7
+opentf_tools-0.46.0.dist-info/RECORD,,
```

