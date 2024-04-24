# Comparing `tmp/aespm-1.0.4.tar.gz` & `tmp/aespm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aespm-1.0.4.tar", last modified: Mon Apr 22 19:48:56 2024, max compression
+gzip compressed data, was "aespm-1.0.5.tar", last modified: Wed Apr 24 22:11:06 2024, max compression
```

## Comparing `aespm-1.0.4.tar` & `aespm-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-04-22 19:48:56.069600 aespm-1.0.4/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1016 2024-04-22 19:48:56.069000 aespm-1.0.4/PKG-INFO
--rw-r--r--   0 richardyuliu   (501) staff       (20)    10023 2024-04-22 18:35:58.000000 aespm-1.0.4/README.md
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-04-22 19:48:56.065187 aespm-1.0.4/aespm/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1394 2024-04-22 17:50:53.000000 aespm-1.0.4/aespm/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    31981 2024-04-22 19:00:14.000000 aespm-1.0.4/aespm/aespm.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    24769 2024-04-22 18:52:49.000000 aespm-1.0.4/aespm/tools.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     3686 2024-04-22 17:44:38.000000 aespm-1.0.4/aespm/utils.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-04-22 19:48:56.068346 aespm-1.0.4/aespm.egg-info/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1016 2024-04-22 19:48:56.000000 aespm-1.0.4/aespm.egg-info/PKG-INFO
--rw-r--r--   0 richardyuliu   (501) staff       (20)      225 2024-04-22 19:48:56.000000 aespm-1.0.4/aespm.egg-info/SOURCES.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2024-04-22 19:48:56.000000 aespm-1.0.4/aespm.egg-info/dependency_links.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       44 2024-04-22 19:48:56.000000 aespm-1.0.4/aespm.egg-info/requires.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)        6 2024-04-22 19:48:56.000000 aespm-1.0.4/aespm.egg-info/top_level.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       38 2024-04-22 19:48:56.069739 aespm-1.0.4/setup.cfg
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1181 2024-04-22 19:48:43.000000 aespm-1.0.4/setup.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-04-24 22:11:06.491165 aespm-1.0.5/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1016 2024-04-24 22:11:06.490463 aespm-1.0.5/PKG-INFO
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     6080 2024-04-23 18:09:20.000000 aespm-1.0.5/README.md
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-04-24 22:11:06.486577 aespm-1.0.5/aespm/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1826 2024-04-24 22:08:21.000000 aespm-1.0.5/aespm/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    33003 2024-04-24 22:10:29.000000 aespm-1.0.5/aespm/experiment.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    24769 2024-04-22 18:52:49.000000 aespm-1.0.5/aespm/tools.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     5757 2024-04-24 22:09:40.000000 aespm-1.0.5/aespm/utils.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-04-24 22:11:06.489727 aespm-1.0.5/aespm.egg-info/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1016 2024-04-24 22:11:06.000000 aespm-1.0.5/aespm.egg-info/PKG-INFO
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      230 2024-04-24 22:11:06.000000 aespm-1.0.5/aespm.egg-info/SOURCES.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2024-04-24 22:11:06.000000 aespm-1.0.5/aespm.egg-info/dependency_links.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       44 2024-04-24 22:11:06.000000 aespm-1.0.5/aespm.egg-info/requires.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        6 2024-04-24 22:11:06.000000 aespm-1.0.5/aespm.egg-info/top_level.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       38 2024-04-24 22:11:06.491314 aespm-1.0.5/setup.cfg
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1181 2024-04-23 18:05:06.000000 aespm-1.0.5/setup.py
```

### Comparing `aespm-1.0.4/PKG-INFO` & `aespm-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespm
-Version: 1.0.4
+Version: 1.0.5
 Summary: SPM Automation with Python and Machine Learning.
 Home-page: https://github.com/RichardLiuCoding/aespm
 Download-URL: https://github.com/RichardLiuCoding/aespm.git
 Author: Richard (Yu) Liu
 Author-email: yliu206@utk.edu
 License: MIT
 Keywords: SPM,Python,Instrument control,Autonomoous,Machine learning,Data Analysis
```

### Comparing `aespm-1.0.4/aespm/__init__.py` & `aespm-1.0.5/aespm/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 import warnings
 warnings.filterwarnings("ignore", category=SyntaxWarning)
 #For Python 3.8+, to avoid SyntaxWarning: "is" with a literal. Did you mean "=="?
 
-__all__ = ['tools']
+__all__ = ['experiment']
 
-from aespm.aespm import *
+from aespm.experiment import *
 
 from aespm import tools
 from aespm import utils
 
 # If there is no buffer files, create them in Documents/buffers
 import os 
 import shutil
+import platform
 
 doc_path = os.path.expanduser('~')
 buffer_path = os.path.join(doc_path, 'Documents', 'buffer')
 
-try:
-	# Create the buffer folder
-	if not os.path.exists(buffer_path):
-		os.makedirs(buffer_path)
-
-	# Create the commands buffer file
-	if not os.path.exists(os.path.join(buffer_path, 'ToIgor.arcmd')):
-		with open(os.path.join(buffer_path, 'ToIgor.arcmd'), 'w') as fopen:
-			fopen.write(' ')
-	# Create bash file to execute commands in hte buffer file
-	if not os.path.exists(os.path.join(buffer_path, 'SendToIgor.bat')):
-		with open(os.path.join(buffer_path, 'SendToIgor.bat'), 'w') as fopen:
-			fopen.write('"C:\\AsylumResearch\\v19\\RealTime\\Igor Pro Folder\\Igor.exe" "{}"'.format(os.path.join(buffer_path, 'ToIgor.arcmd')))
+# Initialize the buffer files only on Windows operating system
 
-	# Copy the user functions into the default include folder of AR
-	# shutil.copy(os.path.join(aespm.__path__, 'user functions', 'UserFunctions.ipf'), os.path.join(doc_path, 'AsylumResearch', 'UserIncludes'))
+if platform.system() == 'Windows':
+	try:
+		# Create the buffer folder
+		if not os.path.exists(buffer_path):
+			os.makedirs(buffer_path)
+
+		# Create the commands buffer file
+		if not os.path.exists(os.path.join(buffer_path, 'ToIgor.arcmd')):
+			with open(os.path.join(buffer_path, 'ToIgor.arcmd'), 'w') as fopen:
+				fopen.write(' ')
+		# Create bash file to execute commands in hte buffer file
+		if not os.path.exists(os.path.join(buffer_path, 'SendToIgor.bat')):
+			with open(os.path.join(buffer_path, 'SendToIgor.bat'), 'w') as fopen:
+				if os.path.exists("C:\\AsylumResearch\\v19"):
+					fopen.write('"C:\\AsylumResearch\\v19\\RealTime\\Igor Pro Folder\\Igor.exe" "{}"'.format(os.path.join(buffer_path, 'ToIgor.arcmd')))
+				elif os.path.exists("C:\\AsylumResearch\\v18"):
+					fopen.write('"C:\\AsylumResearch\\v18\\RealTime\\Igor Pro Folder\\Igor.exe" "{}"'.format(os.path.join(buffer_path, 'ToIgor.arcmd')))
+				else:
+					print("No supported AR versions!")
 
-except PermissionError:
-	print('No writing permission to ~/Documents. Please create buffer folder and files manually.')
+		# Copy the user functions into the default include folder of AR
+		# shutil.copy(os.path.join(aespm.__path__, 'user functions', 'UserFunctions.ipf'), os.path.join(doc_path, 'AsylumResearch', 'UserIncludes'))
+
+	except PermissionError:
+		print('No writing permission to ~/Documents. Please create buffer folder and files manually.')
```

### Comparing `aespm-1.0.4/aespm/aespm.py` & `aespm-1.0.5/aespm/experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,30 @@
 import shutil
 import subprocess
 
 import types
 import pickle
 
 import aespm
+from aespm.utils import shared
 
-buffer_path = os.path.join(os.path.expanduser('~'), 'Documents', 'buffer')
-command_buffer = os.path.join(buffer_path, 'ToIgor.arcmd')
-read_out_buffer = os.path.join(buffer_path, 'readout.txt')
-bash_buffer = os.path.join(buffer_path, 'SendToIgor.bat')
+import platform
+
+if platform.system() == 'Windows':
+    _buffer_path = os.path.join(os.path.expanduser('~'), 'Documents', 'buffer')
+    _command_buffer = os.path.join(_buffer_path, 'ToIgor.arcmd')
+    _read_out_buffer = os.path.join(_buffer_path, 'readout.txt')
+    _bash_buffer = os.path.join(_buffer_path, 'SendToIgor.bat')
+    _exe_path = r"C:\AsylumResearch\v19\RealTime\Igor Pro Folder\Igor.exe"
+else:
+    _buffer_path = r"C:\Users\Asylum User\Documents\buffer"
+    _command_buffer = r"C:\Users\Asylum User\Documents\buffer\ToIgor.arcmd"
+    _read_out_buffer = r"C:\Users\Asylum User\Documents\buffer\readout.txt"
+    _bash_buffer = r"C:\Users\Asylum User\Documents\buffer\SendToIgor.bat"
+    _exe_path = r"C:\AsylumResearch\v19\RealTime\Igor Pro Folder\Igor.exe"
 
 class Experiment(object):
     '''
     Experiment data structure for SPM workflows.
 
     Attributes:
         obj.param      - Dict: A collection of parameters can be updated with obj.update_param
@@ -63,15 +74,23 @@
 
         # This is the folder where your temp data/command files are saved
         self.temp_folder = temp_folder
         
         # Remote control
         if connection is not None:
             host, username, password = connection
+
+            global shared
+            shared.set_host(host)
+
+            local_info = aespm.utils.get_local_directory(host=host).split('$')
+            shared.set_value(local_info)
+
             self.connection, self.client = aespm.utils.return_connection(host, username, password)
+
         else:
             self.connection, self.client = None, None
 
     def execute(self, action, value=None, wait=None, log=True, **kwargs):
         '''
         A wrapper of spm_control() function. 
 
@@ -282,25 +301,25 @@
         write_spm('ARExecuteControl("StartPIDSLoop0","PIDSLoopPanel",0,"")')
 
         # Enable the x PISLoop by remote control
         connection = return_connection()
         write_spm('ARExecuteControl("StartPIDSLoop0","PIDSLoopPanel",0,"")', connection=connection)
     '''
     if connection==None:
-        file = open(command_buffer,"w",encoding = 'utf-8')
+        file = open(_command_buffer,"w",encoding = 'utf-8')
         file.writelines(commands)
         file.close()
 
-        p = Popen(bash_buffer)
+        p = Popen(_bash_buffer)
         p.wait()
         time.sleep(wait)
     else:
         aespm.utils.write_to_remote_file(connection,
-                             file_path = command_buffer, data = commands)
-        aespm.utils.main_exe_on_server()
+                             file_path = _command_buffer, data = commands)
+        aespm.utils.main_exe_on_server(host=shared._host)
         time.sleep(wait)
 
 
 def read_spm(key, commands=None, connection=None):
     '''
     Read Jupiter parameters by exporting them into readout.txt file.
 
@@ -321,61 +340,61 @@
         key = [key]
     if connection == None:
         if commands == None:
             N = len(key)
             start = 'Make/N = ({})/O ReadOut // change N to number of parameters to read out\n'.format(N)
             command = ''
             for i in range(N):
-                if key[i] == 'PIDSLoop.0.Setpoint' or key[i] == 'PIDSLoop.1.Setpoint':
+                if key[i].startswith('PIDSLoop'): # == 'PIDSLoop.0.Setpoint' or key[i] == 'PIDSLoop.1.Setpoint':
                     command += 'ReadOut[{}] = td_ReadValue("{}")\n'.format(i, key[i])
                 else:
                     command += 'ReadOut[{}] = GV("{}")\n'.format(i, key[i])
-            end = 'Save/O/G/J ReadOut as "{}"'.format(read_out_buffer)
-            file = open(command_buffer,"w",encoding = 'utf-8')
+            end = r'Save/O/G/J ReadOut as "{}"'.format(_read_out_buffer.replace('\\', '\\\\'))
+            file = open(_command_buffer,"w",encoding = 'utf-8')
             file.writelines(start+command+end)
             file.close()
-            p = Popen(bash_buffer)
+            p = Popen(_bash_buffer)
             p.wait()
-            return np.loadtxt(read_out_buffer)
+            return np.loadtxt(_read_out_buffer)
 
         else:
-            file = open(command_buffer,"w",encoding = 'utf-8')
+            file = open(_command_buffer,"w",encoding = 'utf-8')
             file.writelines(commands)
             file.close()
 
-            p = Popen(bash_buffer)
+            p = Popen(_bash_buffer)
             p.wait()
-            return np.loadtxt(read_out_buffer)
+            return np.loadtxt(_read_out_buffer)
 
     else:
         if commands == None:
             N = len(key)
             start = 'Make/N = ({})/O ReadOut // change N to number of parameters to read out\n'.format(N)
             command = ''
             for i in range(N):
-                if key[i] == 'PIDSLoop.0.Setpoint' or key[i] == 'PIDSLoop.1.Setpoint':
+                if key[i].startswith('PIDSLoop'): # == 'PIDSLoop.0.Setpoint' or key[i] == 'PIDSLoop.1.Setpoint':
                     command += 'ReadOut[{}] = td_ReadValue("{}")\n'.format(i, key[i])
                 else:
                     command += 'ReadOut[{}] = GV("{}")\n'.format(i, key[i])
-            end = 'Save/O/G/J ReadOut as "{}"'.format(read_out_buffer)
+            end = r'Save/O/G/J ReadOut as "{}"'.format(_read_out_buffer.replace('\\', '\\\\'))
             commands = start+command+end
             aespm.utils.write_to_remote_file(connection,
-                         file_path = command_buffer, data = commands)# doubt as richard
-            aespm.utils.main_exe_on_server()
+                         file_path = _command_buffer, data = commands)# doubt as richard
+            aespm.utils.main_exe_on_server(host=shared._host)
 
-            s = aespm.utils.read_remote_file(connection, read_out_buffer)
+            s = aespm.utils.read_remote_file(connection, _read_out_buffer)
 
             return [float(k) for k in s.decode('utf-8').split('\r')[:-1]]
 
         else:
             aespm.utils.write_to_remote_file(connection,
-                             file_path = command_buffer, data = commands)# doubt as richard
+                             file_path = _command_buffer, data = commands)# doubt as richard
 
-            aespm.utils.main_exe_on_server()
-            s = aespm.utils.read_remote_file(connection, read_out_buffer)
+            aespm.utils.main_exe_on_server(host=shared._host)
+            s = aespm.utils.read_remote_file(connection, _read_out_buffer)
 
             return [float(k) for k in s.decode('utf-8').split('\r')[:-1]]
         
 def spm_control(action, value=None, wait=0.35, connection=None):
     '''
     Control SPM with action. An action-command dict is used to convert the action/input to the actual AR commands.
 
@@ -448,15 +467,16 @@
         ['ScanAngle', 'Scan Angle', 'Angle'],
         ['SetpointAmp', 'AC Setpoint', 'SetpointAC'],
         ['SetpointDefl', 'PFMSetpoint', 'SetpointPFM', 'SetpointContact'],
         ['BlueDriveAmp', 'BlueDriveAmplitude'], # 49
         ['FDTrigger', 'FDTriggerPoint'],
         ['ZeroPD', 'PDZero'],
         ['DARTTrigger', 'SSTrigger'],
-        ['DARTAmp', 'DART v_ac']
+        ['DARTAmp', 'DART v_ac'],
+        ['SampleHeight', 'Sample Height'],
         
     ]
 
     value_list = [
         ['ScanRateSetVar_0', 'MasterPanel', 1], # 0
         ['DownScan_0', 'MasterPanel', 0],
         ['UpScan_0', 'MasterPanel', 0],
@@ -507,14 +527,15 @@
         ['PV("AmplitudeSetpointVolts", {})'.format(value), 4],
         ['PV("DeflectionSetpointVolts", {})'.format(value), 4],
         ['bdDriveAmplitudeSetVar_0', 'MasterPanel', 1], # 49
         ['TriggerPointSetVar_1', 'MasterPanel', 1],
         ["ZeroLDPDButton_1","MasterMotorPanel",0], 
         ["TriggerPointSetVar_2","DARTSpectroscopy", 1],
         ["DriveAmplitudeSetVar_3", "DART", 1], 
+        ['PV("SampleHeight", {})'.format(value), 4],
     ]
     # Construct the action dict
     for i, key in enumerate(key_list):
         for j in range(len(key)):
             action_dict[key[j]] = value_list[i]
 
     cmd = action_dict[action]
@@ -530,15 +551,15 @@
     elif cmd[-1] == 5: # Default numeric input
         commands = 'ARExecuteControl("{}","{}",{},"")'.format(cmd[0], cmd[1], cmd[2])
     elif cmd[-1] == 6: # Default string input
         commands = 'ARExecuteControl("{}","{}",0,"{}")'.format(cmd[0], cmd[1], cmd[2])
     else:
         raise ValueError("Function not implemented yet.")
 
-    write_spm(commands=commands, connection=connection, wait=wait)
+    write_spm(commands=commands, connection=connection, wait=wait, )
 
 
 # Move the tip 
 def move_tip(r, v0=None, s=None, connection=None):
     '''
     Move the tip position based on given displacement.
 
@@ -570,15 +591,15 @@
         sx, sy = s
     vx = x_delta / sx
     vy = y_delta / sy
 
     command1 = 'td_WriteValue("PIDSLoop.0.Setpoint",{})\n'.format(vx+v0x)
     command2 = 'td_WriteValue("PIDSLoop.1.Setpoint",{})\n'.format(vy+v0y)
 
-    write_spm(commands=command1+command2, connection=connection)
+    write_spm(commands=command1+command2, connection=connection, )
 
 
 def move_stage(distance, connection=None):
     '''
     Move the stage position based on given displacement.
 
     Input:
@@ -603,15 +624,15 @@
     
     if y != 0:
         # Change the motor step size for y direction moving
         write_spm(commands='PV("StageMoveStepSize", {})'.format(abs(y)), connection=connection)
         write_spm(commands='MoveStage("{}")'.format(y_direction), connection=connection)
 
 
-def tune_probe(num=1, path=os.path.join(buffer_path, 'Tune.ibw'), center=None, width=50e3, out=False, connection=None):
+def tune_probe(num=1, path=os.path.join(_buffer_path, 'Tune.ibw'), center=None, width=50e3, out=False, connection=None):
     '''
     Tune the probe in the DART mode and optionally read the tune data.
 
     Input:
         num     - Int: how many times tune will be repeated
         path    - String: path where the tune result is saved
         center  - float: center of the tuning frequency range
@@ -708,16 +729,16 @@
     Each channel contains both the trace and retrace scan lines.
     '''
     retries = 0
     if connection==None:
         if lines==True:
             while retries < retry:
                 try:
-                    shutil.copy(fname, os.path.join(buffer_path, 'copy.ibw'))
-                    data = bw.load(os.path.join(buffer_path, 'copy.ibw'))
+                    shutil.copy(fname, os.path.join(_buffer_path, 'copy.ibw'))
+                    data = bw.load(os.path.join(_buffer_path, 'copy.ibw'))
                     wave = data['wave']['wData']
                     return wave.T
                     # return aespm.tools.load_ibw(fname)
                 except FileNotFoundError:
                     print("File not found. Retrying {} times...".format(retries), end='\r')
                     retries += 1
                     time.sleep(wait)
```

### Comparing `aespm-1.0.4/aespm/tools.py` & `aespm-1.0.5/aespm/tools.py`

 * *Files identical despite different names*

### Comparing `aespm-1.0.4/aespm.egg-info/PKG-INFO` & `aespm-1.0.5/aespm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespm
-Version: 1.0.4
+Version: 1.0.5
 Summary: SPM Automation with Python and Machine Learning.
 Home-page: https://github.com/RichardLiuCoding/aespm
 Download-URL: https://github.com/RichardLiuCoding/aespm.git
 Author: Richard (Yu) Liu
 Author-email: yliu206@utk.edu
 License: MIT
 Keywords: SPM,Python,Instrument control,Autonomoous,Machine learning,Data Analysis
```

### Comparing `aespm-1.0.4/setup.py` & `aespm-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'aespm',
-  version = '1.0.4',
+  version = '1.0.5',
   packages = find_packages(),
   license='MIT',
   description = 'SPM Automation with Python and Machine Learning.',
   long_description = 'Python interface that enables local and remote control of Scanning Probe Microscope (SPM) with codes.\nIt offers a modular way to write autonomous workflows ranging from simple routine operations, to advanced automatic scientific discovery based on machine learning.',
   author = 'Richard (Yu) Liu',
   author_email = 'yliu206@utk.edu',
   url = 'https://github.com/RichardLiuCoding/aespm',
```

