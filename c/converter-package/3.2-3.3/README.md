# Comparing `tmp/converter_package-3.2.tar.gz` & `tmp/converter_package-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/converter_package-3.2.tar", last modified: Thu Apr 27 10:14:43 2023, max compression
+gzip compressed data, was "converter_package-3.3.tar", last modified: Thu Apr 25 15:25:50 2024, max compression
```

## Comparing `converter_package-3.2.tar` & `converter_package-3.3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:14:43.000000 converter_package-3.2/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 10:14:43.000000 converter_package-3.2/PKG-INFO
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      696 2023-04-27 10:14:39.000000 converter_package-3.2/setup.py
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     7027 2023-01-23 08:59:17.000000 converter_package-3.2/converter_package/MatchingModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     1305 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/CloudFramework.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     3428 2022-11-17 10:24:26.000000 converter_package-3.2/converter_package/ComputeNode.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      666 2022-11-24 13:31:15.000000 converter_package-3.2/converter_package/ActionModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      438 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/Workflows.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      242 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/Action.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      565 2022-11-24 13:33:47.000000 converter_package-3.2/converter_package/ID.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)    91997 2023-04-27 10:14:19.000000 converter_package-3.2/converter_package/Converter.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)    11636 2023-02-01 11:10:18.000000 converter_package-3.2/converter_package/Parser.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        0 2022-07-28 09:30:38.000000 converter_package-3.2/converter_package/__init__.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     3816 2023-01-19 14:51:16.000000 converter_package-3.2/converter_package/Container.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      514 2022-01-26 10:33:29.000000 converter_package-3.2/converter_package/Image.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     1385 2022-11-24 13:33:47.000000 converter_package-3.2/converter_package/WorkflowModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      733 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/Repository.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      622 2022-10-13 11:01:53.000000 converter_package-3.2/converter_package/Kafka_Producer.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2369 2023-03-30 13:41:33.000000 converter_package-3.2/README.md
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2022-09-13 13:10:54.000000 converter_package-3.2/converter_package.egg-info/not-zip-safe
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/PKG-INFO
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/dependency_links.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       18 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/top_level.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      732 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/SOURCES.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       58 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/requires.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       38 2023-04-27 10:14:43.000000 converter_package-3.2/setup.cfg
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2024-04-25 15:25:50.456651 converter_package-3.3/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1080 2024-04-25 08:08:16.000000 converter_package-3.3/LICENSE
+-rw-r--r--   0 giannis   (1000) giannis   (1000)    17638 2024-04-25 15:25:50.456651 converter_package-3.3/PKG-INFO
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    17030 2024-04-25 15:04:36.000000 converter_package-3.3/README.md
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2024-04-25 15:25:50.456651 converter_package-3.3/converter_package/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      242 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/Action.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      666 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/ActionModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1305 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/CloudFramework.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     3428 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/ComputeNode.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     3848 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/Container.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    91888 2024-04-25 14:52:54.000000 converter_package-3.3/converter_package/Converter.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      565 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/ID.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     7027 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/MatchingModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    10707 2024-04-25 14:52:54.000000 converter_package-3.3/converter_package/Parser.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      733 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/Repository.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1385 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/WorkflowModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      438 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/Workflows.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        0 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package/__init__.py
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2024-04-25 15:25:50.456651 converter_package-3.3/converter_package.egg-info/
+-rw-r--r--   0 giannis   (1000) giannis   (1000)    17638 2024-04-25 15:25:50.000000 converter_package-3.3/converter_package.egg-info/PKG-INFO
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      677 2024-04-25 15:25:50.000000 converter_package-3.3/converter_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2024-04-25 15:25:50.000000 converter_package-3.3/converter_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2024-04-25 08:08:16.000000 converter_package-3.3/converter_package.egg-info/not-zip-safe
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       45 2024-04-25 15:25:50.000000 converter_package-3.3/converter_package.egg-info/requires.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       18 2024-04-25 15:25:50.000000 converter_package-3.3/converter_package.egg-info/top_level.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       38 2024-04-25 15:25:50.456651 converter_package-3.3/setup.cfg
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      891 2024-04-25 15:25:37.000000 converter_package-3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `converter_package-3.2/setup.py` & `converter_package-3.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(name='converter_package',
-      version='3.2',
-      description='This converter library is able to transform the ACCORDION application model to K3s configuration files',
+      version='3.3',
+      description='Converter is a reasoning tool designed for the cloud language known as CEAML. CEAML is an extension of TOSCA capable to describe deployment and runtime adaptation for platforms that utilize both Cloud and Edge resources. It can parse CEAML entities and translate them into configuration files for K3s or Kubevirt.',
       author='Giannis Korontanis',
       author_email='gkorod2@gmail.com',
       license='MIT',
       packages=['converter_package'],
       long_description=long_description,
       long_description_content_type='text/markdown',
       install_requires=[
-          'pyyaml==5.3.1', 'kafka==1.3.5', 'hurry.filesize==0.9', 'oyaml==1.0'
+          'pyyaml==5.3.1', 'hurry.filesize==0.9', 'oyaml==1.0'
       ],
       zip_safe=False)
```

### Comparing `converter_package-3.2/converter_package/MatchingModel.py` & `converter_package-3.3/converter_package/MatchingModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.2/converter_package/CloudFramework.py` & `converter_package-3.3/converter_package/CloudFramework.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.2/converter_package/ComputeNode.py` & `converter_package-3.3/converter_package/ComputeNode.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.2/converter_package/ActionModel.py` & `converter_package-3.3/converter_package/ActionModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.2/converter_package/ID.py` & `converter_package-3.3/converter_package/ID.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.2/converter_package/Converter.py` & `converter_package-3.3/converter_package/Converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import oyaml as yaml
 from converter_package import ID
 from converter_package import ComputeNode
 from converter_package import Parser
 import re
 
 
-def undeploy(pod, intermediate_model):
+def undeploy(pod, file_path):
     application_instance, component_name = find_application_instance(pod)
     label = application_instance + "-" + component_name
-    nodelist, imagelist, application_version = Parser.ReadFile(intermediate_model)
+    nodelist = Parser.ReadFile(file_path)
     deployment = {}
     vm_flag = False
     print(application_instance)
     resource_list = []
     for x in nodelist:
         if ('EdgeNode' in x.get_type()) or ('PublicCloud' in x.get_type()):
             resource = ComputeNode.Resource()
@@ -266,17 +266,17 @@
     letters.pop(0)
     component_name = ""
     for letter in letters:
         component_name = component_name + letter
     return namespace, component_name
 
 
-def scale_out_to_k8s(pod, intermediate_model):
+def scale_out_to_k8s(pod, file_path):
     application_instance, component_name, label = find_replica_instance(pod)
-    nodelist, imagelist, application_version = Parser.ReadFile(intermediate_model)
+    nodelist = Parser.ReadFile(file_path)
     deployment = {}
     vm_flag = False
     print(application_instance)
     resource_list = []
     for x in nodelist:
         if ('EdgeNode' in x.get_type()) or ('PublicCloud' in x.get_type()):
             resource = ComputeNode.Resource()
@@ -494,15 +494,15 @@
                                     deployment = extra_labels(deployment, resource.get_gpu_brand(),
                                                               resource.get_gpu_dedicated(),
                                                               resource.get_wifi_antenna())
 
     return deployment
 
 
-def tosca_to_k8s(nodelist, imagelist, application_instance, minicloud, externalIP, gpu_list=[]):
+def tosca_to_k8s(nodelist, application_instance, minicloud, externalIP, gpu_list=[]):
     if not gpu_list:
         gpu_list = None
     deployment = {}
 
     service_files = []
     persistent_files = []
     deployment_files = []
@@ -1147,15 +1147,15 @@
                                                             'name': 'disk0',
                                                             'persistentVolumeClaim': {
                                                                 'claimName': dv}},
                                                         {
                                                             'name': 'virtiocontainerdisk',
                                                             'containerDisk': {
                                                                 'image': 'kubevirt/virtio-container-disk'}},
-                                                    ],'networks': [{'name': 'default', 'pod': {}}]}}}}}
+                                                    ], 'networks': [{'name': 'default', 'pod': {}}]}}}}}
                                 deployment = extra_labels(deployment, resource.get_gpu_brand(),
                                                           resource.get_gpu_dedicated(), resource.get_wifi_antenna())
                             else:
                                 gpu_model = gpu.get('gpu_model')
                                 deployment = {
                                     application_instance + "-" + x.get_name() + "-" + minicloud: {
                                         'apiVersion': 'kubevirt.io/v1',
@@ -1205,15 +1205,15 @@
                                                             'name': 'disk0',
                                                             'persistentVolumeClaim': {
                                                                 'claimName': dv}},
                                                         {
                                                             'name': 'virtiocontainerdisk',
                                                             'containerDisk': {
                                                                 'image': 'kubevirt/virtio-container-disk'}},
-                                                    ],'networks': [{'name': 'default', 'pod': {}}]}}}}}
+                                                    ], 'networks': [{'name': 'default', 'pod': {}}]}}}}}
 
                                 deployment = extra_labels(deployment, resource.get_gpu_brand(),
                                                           resource.get_gpu_dedicated(), resource.get_wifi_antenna())
                         deployment_files.append(deployment)
     if vm_flag:
         exporter_service = {
             application_instance + "-" + x.get_name() + "-" + minicloud + "-exporter-service": {
```

### Comparing `converter_package-3.2/converter_package/Parser.py` & `converter_package-3.3/converter_package/Parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 import os
 from converter_package import Action
-
+import yaml
 from converter_package import Repository
 from converter_package import ComputeNode
 
 from converter_package import CloudFramework
 from converter_package import Container
-from converter_package import Image
 from converter_package import Workflows
 
 home = str(os.getcwd())
 
 
-def ReadFile(json):
+def ReadFile(file_path):
     nodelist = []
 
     imagelist = []
     application = ""
-    requirements = json.get('requirements')
-    definitions = requirements[0].get('toscaDescription')
-    topology = definitions.get('topology_template')
+    with open(file_path, 'r') as yaml_file:
+        file = yaml.safe_load(yaml_file)
+    topology = file.get('topology_template')
     node_template = topology.get('node_templates')
-    registry = json.get('registry')
-    application_details = json.get('details')
-    application_version = application_details.get('version')
-    print(registry)
-    repolist = []
-    for repository in registry:
-        repo = Repository.Repository()
-        repo.set_version(repository.get('version'))
-        repo.set_imageName(repository.get('imageName'))
-        repo.set_path(repository.get('location'))
-        print(repository)
-        repo.set_component(repository.get('component'))
-        repolist.append(repo)
     node_names = node_template.keys()
     print(node_names)
     for x in node_names:
         node = node_template.get(x)
         type = node.get('type')
         properties = node.get('properties')
         if 'Cloud_Framework' in type:
@@ -110,14 +96,20 @@
                                  'send': target_list})
                     workflowlist.append({'scenario': workflow.get_scenario(), 'condition': workflow.get_condition(),
                                          'actions': actionlist})
                 cloud.set_workflows(workflowlist)
         if 'Component' in type:
             container = Container.Container()
             container.set_type(type)
+            registry = properties.get('registry')
+            registry_properties = registry.get('properties')
+            image = registry_properties.get('image')
+            container.set_image(image)
+            type = registry_properties.get('type')
+            container.set_registry_type(type)
             name = properties.get('name')
             container.set_name(name)
             container.set_application(application)
             if properties.get('instance'):
                 instance_num = properties.get('instance')
                 container.set_instance(instance_num)
             else:
@@ -145,23 +137,14 @@
                 dependency = properties.get('dependency')
                 container.set_dependency(dependency)
             else:
                 container.set_dependency(None)
             requirements = node.get('requirements')[0]
             host = requirements.get('host')
             container.set_host(host)
-            # here is done the matching between components of the application model and images of the intermediate model
-            # VM part is not fully developed since we don't have the description of these images at IM
-            for image in imagelist:
-                if name == image.get_path():
-                    if image.get_image_type() == 'vm':
-                        container.set_image(image.get_component().lower())
-                    for repo in repolist:
-                        if repo.get_component() == image.get_path():
-                            container.set_image(repo.get_path())
             nodelist.append(container)
         if 'EdgeNode' in type:
             edgenode = ComputeNode.ComputeNode()
             edgenode.set_name(x)
             edgenode.set_type(type)
             if properties:
                 if properties.get('gpu_model'):
@@ -240,8 +223,8 @@
             os_properties = os.get('properties')
             os_type = os_properties.get('type')
             vm.set_os(os_type)
             architecture = os_properties.get('architecture')
             vm.set_architecture(architecture)
             nodelist.append(vm)
 
-    return (nodelist), (imagelist), application_version.replace(".", "-")
+    return (nodelist)
```

### Comparing `converter_package-3.2/converter_package/Container.py` & `converter_package-3.3/converter_package/Container.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,19 +127,19 @@
 
     def set_image(self, images):
         self.__images = images
 
     def get_image(self):
         return self.__images
 
-    def set_internal(self, boolean):
-        self.__internal = boolean
+    def set_registry_type(self, registry_type):
+        self.__registry_type = registry_type
 
-    def get_internal(self):
-        return self.__internal
+    def get_registry_type(self):
+        return self.__registry_type
 
     def set_unit(self, unit):
         self.__unit = unit
 
     def get_unit(self):
         return self.__unit
```

### Comparing `converter_package-3.2/converter_package/Image.py` & `converter_package-3.3/converter_package/Repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-class Image:
+class Repository:
+    def set_path(self, path):
+        self.__path = path
 
-    def set_component(self, component):
-        self.__component = component
+    def get_path(self):
+        return self.__path
 
-    def get_component(self):
-        return self.__component
+    def set_version(self, version):
+        self.__version = version
 
-    def set_image_name(self, image):
-        self.__image = image
+    def get_version(self):
+        return self.__version
 
-    def get_image_name(self):
-        return self.__image
+    def set_id(self, id):
+        self.__id = id
 
-    def set_image_type(self, type):
-        self.__type = type
+    def get_id(self):
+        return self.__id
 
-    def get_image_type(self):
-        return self.__type
+    def set_size(self, size):
+        self.__size = size
 
-    def set_path(self, path):
-        self.__path = path
+    def get_size(self):
+        return self.__size
 
-    def get_path(self):
-        return self.__path
+    def set_imageName(self,name):
+        self.__imageName = name
 
+    def get_imageName(self):
+        return self.__imageName
 
+    def set_component(self, component):
+        self.__component = component
 
+    def get_component(self):
+        return  self.__component
```

### Comparing `converter_package-3.2/converter_package/WorkflowModel.py` & `converter_package-3.3/converter_package/WorkflowModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.2/converter_package.egg-info/SOURCES.txt` & `converter_package-3.3/converter_package.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+LICENSE
 README.md
 setup.py
 converter_package/Action.py
 converter_package/ActionModel.py
 converter_package/CloudFramework.py
 converter_package/ComputeNode.py
 converter_package/Container.py
 converter_package/Converter.py
 converter_package/ID.py
-converter_package/Image.py
-converter_package/Kafka_Producer.py
 converter_package/MatchingModel.py
 converter_package/Parser.py
 converter_package/Repository.py
 converter_package/WorkflowModel.py
 converter_package/Workflows.py
 converter_package/__init__.py
 converter_package.egg-info/PKG-INFO
```

