# Comparing `tmp/allocmd-1.0.0.tar.gz` & `tmp/allocmd-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/allocmd-1.0.0.tar", last modified: Thu Apr 25 15:41:54 2024, max compression
+gzip compressed data, was "dist/allocmd-2.0.0.tar", last modified: Thu Apr 25 15:48:24 2024, max compression
```

## Comparing `allocmd-1.0.0.tar` & `allocmd-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:41:54.000000 allocmd-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-25 15:41:54.000000 allocmd-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-25 15:41:41.000000 allocmd-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:41:41.000000 allocmd-1.0.0/allocmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-25 15:41:41.000000 allocmd-1.0.0/allocmd/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:41:41.000000 allocmd-1.0.0/allocmd/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 15:41:41.000000 allocmd-1.0.0/allocmd/utilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 15:41:41.000000 allocmd-1.0.0/allocmd/utilities/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20019 2024-04-25 15:41:41.000000 allocmd-1.0.0/allocmd/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:41:54.000000 allocmd-1.0.0/allocmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:41:54.000000 allocmd-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-25 15:41:41.000000 allocmd-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:48:24.000000 allocmd-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-25 15:48:24.000000 allocmd-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-25 15:48:13.000000 allocmd-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:48:13.000000 allocmd-2.0.0/allocmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-25 15:48:13.000000 allocmd-2.0.0/allocmd/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:48:13.000000 allocmd-2.0.0/allocmd/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 15:48:13.000000 allocmd-2.0.0/allocmd/utilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:48:13.000000 allocmd-2.0.0/allocmd/utilities/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24416 2024-04-25 15:48:13.000000 allocmd-2.0.0/allocmd/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:48:24.000000 allocmd-2.0.0/allocmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:48:24.000000 allocmd-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-25 15:48:13.000000 allocmd-2.0.0/setup.py
```

### Comparing `allocmd-1.0.0/PKG-INFO` & `allocmd-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 Metadata-Version: 2.1
 Name: allocmd
-Version: 1.0.0
+Version: 2.0.0
 Summary: A CLI tool for creating Allora Chain Worker Nodes
 Home-page: UNKNOWN
 Author: Upshot Technologies
 Author-email: tobi@upshot.xyz
 License: UNKNOWN
 Description: # Building a Worker Node with the allocmd CLI
         ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
         ![Python!](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
         ![Apache License](https://img.shields.io/badge/Apache%20License-D22128?style=for-the-badge&logo=Apache&logoColor=white)
         
-        The `allocmd` is a CLI tool that handles worker nodes' seamless creation and deployment. With this tool, you do not need to write the worker node from scratch, the CLI tool will help you bootstrap all the needed components to get worker nodes working. All you have to do is to update the `config.yaml` file with your custom parameters, update the provided`main.py`to communicate with your inference server, run the deploy command, and your worker should be up and running.
+        The `allocmd` is a CLI tool that handles seamless creation of Allora external resources built to integrate with Allora chain. With this tool, you do not need to write the worker or reputer node or even a validator from scratch, the CLI tool will help you bootstrap all the needed components to get resource working.
         
-        To build a worker node with `allocmd`, you will need to follow the following steps:
+        The following are the list of stuff that can don with this tool at the moment
+        1. Generating worker node files
+        2. Genrating reputer node files
+        3. Generating validator node files
+        4. Funding of testnet account addresses
         
-        ### 1. Install `allocmd` CLI
+        for all the files generation commands, the tool will help in generation of the needed files and their respective docker files and you can spin them up as usual docker containers with docker-compose
+        
+        ## Install `allocmd` CLI
         
         You will begin with installing the tool on your machine. 
         
         ```shell
         pip install allocmd
         ```
         
-        > you can run `allocmd --help` to get general help or `allocmd [command] --help` to get help relating to a particular command.
+        > you should use version 1.0.0 for Allora Chain v1 and version 2.0.0 for Allora Chain v2. Run `allocmd --help` to get general help or `allocmd [command] --help` to get help relating to a particular command.
         
-        ### 2. Initialize the worker for development
+        ## Initializing resources
+        ### Initialize the worker/reputer for development
+        > Note that all commands here will pass for both worker or reputer node
         
-        The next step is initializing the CLI to bootstrap all the needed components to get your worker running. The following command will handle the initialization process. It will create all the files in the appropriate directories and generate identities for your node to be used for local development.
+        The next step is initializing the CLI to bootstrap all the needed components to get your worker or reputer running. The following command will handle the initialization process. It will create all the files in the appropriate directories and generate identities for your node to be used for local development.
         
         ```shell
-        allocmd init --name <preffered name> --topic <topic id> --env dev
+        allocmd generate worker --name <preffered name> --topic <topic id> --env dev
         ```
         
-        Before running this command you will have to [pick the topic Id ](https://docs.allora.network/docs/existing-allora-appchain-topics)you wish to generate inference for after which you can run this command with the topic Id. The command will auto-create some files, the most important of which is the `dev-docker-compose.yaml`file which is an already complete docker-compose that you can run immediately to see your worker and head nodes running perfectly on your local machine. You can edit the files as you wish. for instance the `main.py` is meant for you to call your inference server, hence you will have to edit the sample code with actual URLs and logic as you prefer.
+        Before running this command you will have to [pick the topic Id ](https://docs.allora.network/docs/existing-allora-appchain-topics)you wish to generate inference for after which you can run this command with the topic Id. The command will auto-create some files, the most important of which is the `dev-docker-compose.yaml`file which is an already complete docker-compose that you can run immediately to see your worker/reputer and head nodes running perfectly on your local machine. You can edit the files as you wish. for instance the `main.py` is meant for you to call your inference server, hence you will have to edit the sample code with actual URLs and logic as you prefer.
         
-        When you run the docker-compose (`docker-compose -f dev-docker-compose.yaml up --build`), maybe after you have written and tested your logic in `main.py`, you then should be seeing the logs from the nodes, and you should be able to make a request to your head node and see it get a response from the worker node. Note that in production, you won't be the one to make the inference request, as the Allora chain will do this at the cadence provided by the topic creator.
+        When you run the docker-compose (`docker-compose -f dev-docker-compose.yaml up --build`), maybe after you have written and tested your logic in `main.py`, you then should be seeing the logs from the nodes, and you should be able to make a request to your head node and see it get a response from the worker/reputer node. Note that in production, you won't be the one to make the inference request, as the Allora chain will do this at the cadence provided by the topic creator.
         
         You can test your node by running the following curl command:
         
         ```
         curl --location 'http://localhost:6000/api/v1/functions/execute' --header 'Accept: application/json, text/plain, */*' --header 'Content-Type: application/json;charset=UTF-8' --data '{
             "function_id": "bafybeigpiwl3o73zvvl6dxdqu7zqcub5mhg65jiky2xqb4rdhfmikswzqm",
             "method": "allora-inference-function.wasm",
@@ -60,23 +68,35 @@
                 "timeout" : 2
             }
         }' | jq
         ```
         
         The `<TOPIC_ID>` needs to be [an existing topic on the chain](https://docs.allora.network/docs/existing-allora-appchain-topics). The `<argument>` is what the topic is expecting to receive to perform the inference (as an indication to test, you can use the `DefaultArg`  value from the topic on-chain, e.g. for ETH prediction topic, it should be `"ETH"`).
         
-        ### 3. Initialize the worker for production
+        ### Initialize the worker/reputer for production
         
-        Your worker node is now ready to be deployed, the `main.py` has been modified, all env variables passed, and the worker node is running locally and you are now ready to deploy your worker to run in the production environment. The following command will handle the generation of the `prod-docker-compose.yaml` file which contains all the keys and parameters needed for your worker to function perfectly in production.
+        Your worker/reputer node is now ready to be deployed, the `main.py` has been modified, all env variables passed, and the worker/reputer node is running locally and you are now ready to deploy your worker/reputer to run in the production environment. The following command will handle the generation of the `prod-docker-compose.yaml` file which contains all the keys and parameters needed for your worker/reputer to function perfectly in production.
         
         ```shell
-        allocmd init --env prod
+        allocmd generate worker --env prod
         ```
         
         By running this command, `prod-docker-compose.yaml` will be generated with appropriate keys and parameters. You can now run the docker-compose file or deploy the whole codebase in your preferred cloud instance. At this stage, your worker should be responding to inference request from the Allora Chain.
         
+        ### Initialize validator production
+        ```shell
+        allocmd generate validator --name <validator-name> --network <testnet or mainnet>
+        ```
+        The above command can generate validator files and you can then use docker-compose to deploy
+        
+        ### Fund account address
+        ```shell
+        allocmd fund <address> 
+        ```
+        The above command takes address and fund the account with Allora Faucet
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `allocmd-1.0.0/README.md` & `allocmd-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 # Building a Worker Node with the allocmd CLI
 ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
 ![Python!](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
 ![Apache License](https://img.shields.io/badge/Apache%20License-D22128?style=for-the-badge&logo=Apache&logoColor=white)
 
-The `allocmd` is a CLI tool that handles worker nodes' seamless creation and deployment. With this tool, you do not need to write the worker node from scratch, the CLI tool will help you bootstrap all the needed components to get worker nodes working. All you have to do is to update the `config.yaml` file with your custom parameters, update the provided`main.py`to communicate with your inference server, run the deploy command, and your worker should be up and running.
+The `allocmd` is a CLI tool that handles seamless creation of Allora external resources built to integrate with Allora chain. With this tool, you do not need to write the worker or reputer node or even a validator from scratch, the CLI tool will help you bootstrap all the needed components to get resource working.
 
-To build a worker node with `allocmd`, you will need to follow the following steps:
+The following are the list of stuff that can don with this tool at the moment
+1. Generating worker node files
+2. Genrating reputer node files
+3. Generating validator node files
+4. Funding of testnet account addresses
 
-### 1. Install `allocmd` CLI
+for all the files generation commands, the tool will help in generation of the needed files and their respective docker files and you can spin them up as usual docker containers with docker-compose
+
+## Install `allocmd` CLI
 
 You will begin with installing the tool on your machine. 
 
 ```shell
 pip install allocmd
 ```
 
-> you can run `allocmd --help` to get general help or `allocmd [command] --help` to get help relating to a particular command.
+> you should use version 1.0.0 for Allora Chain v1 and version 2.0.0 for Allora Chain v2. Run `allocmd --help` to get general help or `allocmd [command] --help` to get help relating to a particular command.
 
-### 2. Initialize the worker for development
+## Initializing resources
+### Initialize the worker/reputer for development
+> Note that all commands here will pass for both worker or reputer node
 
-The next step is initializing the CLI to bootstrap all the needed components to get your worker running. The following command will handle the initialization process. It will create all the files in the appropriate directories and generate identities for your node to be used for local development.
+The next step is initializing the CLI to bootstrap all the needed components to get your worker or reputer running. The following command will handle the initialization process. It will create all the files in the appropriate directories and generate identities for your node to be used for local development.
 
 ```shell
-allocmd init --name <preffered name> --topic <topic id> --env dev
+allocmd generate worker --name <preffered name> --topic <topic id> --env dev
 ```
 
-Before running this command you will have to [pick the topic Id ](https://docs.allora.network/docs/existing-allora-appchain-topics)you wish to generate inference for after which you can run this command with the topic Id. The command will auto-create some files, the most important of which is the `dev-docker-compose.yaml`file which is an already complete docker-compose that you can run immediately to see your worker and head nodes running perfectly on your local machine. You can edit the files as you wish. for instance the `main.py` is meant for you to call your inference server, hence you will have to edit the sample code with actual URLs and logic as you prefer.
+Before running this command you will have to [pick the topic Id ](https://docs.allora.network/docs/existing-allora-appchain-topics)you wish to generate inference for after which you can run this command with the topic Id. The command will auto-create some files, the most important of which is the `dev-docker-compose.yaml`file which is an already complete docker-compose that you can run immediately to see your worker/reputer and head nodes running perfectly on your local machine. You can edit the files as you wish. for instance the `main.py` is meant for you to call your inference server, hence you will have to edit the sample code with actual URLs and logic as you prefer.
 
-When you run the docker-compose (`docker-compose -f dev-docker-compose.yaml up --build`), maybe after you have written and tested your logic in `main.py`, you then should be seeing the logs from the nodes, and you should be able to make a request to your head node and see it get a response from the worker node. Note that in production, you won't be the one to make the inference request, as the Allora chain will do this at the cadence provided by the topic creator.
+When you run the docker-compose (`docker-compose -f dev-docker-compose.yaml up --build`), maybe after you have written and tested your logic in `main.py`, you then should be seeing the logs from the nodes, and you should be able to make a request to your head node and see it get a response from the worker/reputer node. Note that in production, you won't be the one to make the inference request, as the Allora chain will do this at the cadence provided by the topic creator.
 
 You can test your node by running the following curl command:
 
 ```
 curl --location 'http://localhost:6000/api/v1/functions/execute' --header 'Accept: application/json, text/plain, */*' --header 'Content-Type: application/json;charset=UTF-8' --data '{
     "function_id": "bafybeigpiwl3o73zvvl6dxdqu7zqcub5mhg65jiky2xqb4rdhfmikswzqm",
     "method": "allora-inference-function.wasm",
@@ -52,16 +60,28 @@
         "timeout" : 2
     }
 }' | jq
 ```
 
 The `<TOPIC_ID>` needs to be [an existing topic on the chain](https://docs.allora.network/docs/existing-allora-appchain-topics). The `<argument>` is what the topic is expecting to receive to perform the inference (as an indication to test, you can use the `DefaultArg`  value from the topic on-chain, e.g. for ETH prediction topic, it should be `"ETH"`).
 
-### 3. Initialize the worker for production
+### Initialize the worker/reputer for production
 
-Your worker node is now ready to be deployed, the `main.py` has been modified, all env variables passed, and the worker node is running locally and you are now ready to deploy your worker to run in the production environment. The following command will handle the generation of the `prod-docker-compose.yaml` file which contains all the keys and parameters needed for your worker to function perfectly in production.
+Your worker/reputer node is now ready to be deployed, the `main.py` has been modified, all env variables passed, and the worker/reputer node is running locally and you are now ready to deploy your worker/reputer to run in the production environment. The following command will handle the generation of the `prod-docker-compose.yaml` file which contains all the keys and parameters needed for your worker/reputer to function perfectly in production.
 
 ```shell
-allocmd init --env prod
+allocmd generate worker --env prod
 ```
 
 By running this command, `prod-docker-compose.yaml` will be generated with appropriate keys and parameters. You can now run the docker-compose file or deploy the whole codebase in your preferred cloud instance. At this stage, your worker should be responding to inference request from the Allora Chain.
+
+### Initialize validator production
+```shell
+allocmd generate validator --name <validator-name> --network <testnet or mainnet>
+```
+The above command can generate validator files and you can then use docker-compose to deploy
+
+### Fund account address
+```shell
+allocmd fund <address> 
+```
+The above command takes address and fund the account with Allora Faucet
```

### Comparing `allocmd-1.0.0/allocmd/cli.py` & `allocmd-2.0.0/allocmd/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 import os
 import click
 import subprocess
 from jinja2 import Environment, FileSystemLoader
 from importlib.resources import files
 from termcolor import colored, cprint
-from .utilities.utils import generate_all_files, print_allora_banner, run_key_generate_command, deployWorker, deployValidator, generateWorkerAccount, generateProdCompose
-from .utilities.typings import Command
+from .utilities.utils import generate_all_files, print_allora_banner, run_key_generate_command, deployWorker, deployValidator, generateWorkerAccount, generateProdCompose, check_docker_running, blocklessNode, fundAddress
+from .utilities.typings import Command, BlocklessNodeType
 from .utilities.constants import cliVersion
 
 template_path = files('allocmd').joinpath('templates')
 env = Environment(loader=FileSystemLoader(template_path), autoescape=True)
 
 @click.group()
 @click.version_option(version=cliVersion, prog_name='allocmd', message='%(prog)s version %(version)s')
 def cli():
     """A CLI Tool that handles creation of an Allora Worker Node"""
     pass
 
-@click.command()
+@cli.group()
+def generate():
+    """generate scaffolded files and directories depending on the command type passed."""
+    pass
+
+@generate.command()
 @click.option('--env', 'environment', required=True, type=click.Choice(['dev', 'prod']), help='Environment to generate for')
 @click.option('--name', required=False, help='Name of the worker.')
 @click.option('--topic', required=False, type=int, help='The topic ID the worker is registered with.')
-def init(environment, name=None, topic=None):
+def worker(environment, name=None, topic=None):
     """Initialize your Allora Worker Node with necessary boilerplates"""
 
-    if environment == 'dev':
-        if topic is None:
-            cprint("You must provide topic id when running development init.", 'red')
-            return
-        elif name is None:
-            cprint("You must provide name when running development init.", 'red')
-            return
+    blocklessNode(environment, env, BlocklessNodeType.worker.name, name, topic)
 
+@generate.command()
+@click.option('--env', 'environment', required=True, type=click.Choice(['dev', 'prod']), help='Environment to generate for')
+@click.option('--name', required=False, help='Name of the reputer.')
+@click.option('--topic', required=False, type=int, help='The topic ID the reputer is registered with.')
+def reputer(environment, name=None, topic=None):
+    """Initialize your Allora Reputer Node with necessary boilerplates"""
+
+    blocklessNode(environment, env, BlocklessNodeType.reputer.name, name, topic)
 
-        print_allora_banner()
-        cprint("Welcome to the Allora CLI!", 'green', attrs=['bold'])
-        print(colored("Allora CLI assists in the seamless creation and deployment of Allora worker nodes", 'yellow'))
-        print(colored("to provide model inference to the Allora Chain.", 'yellow'))
-        cprint(f"\nThis command will generate some files in the directory named '{name}'.", 'cyan')
-        
-        if click.confirm(colored("\nWould you like to proceed?", 'white', attrs=['bold']), default=True):
-            cprint("\nProceeding with the creation of worker node directory...", 'green')
 
-            head_peer_id = run_key_generate_command(name)
+@generate.command()
+@click.option('--name',required=True, help='Name of the validator.')
+@click.option('--network', required=True, type=click.Choice(['testnet', 'edgenet']), help='Your preffered chain network to run the validator on.')
+def validator(name=None, network=None):
+    """Initialize your Allora Worker Node with necessary boilerplates"""
+
+    if not check_docker_running():
+        cprint("Docker is not running, please start docker before running this command", 'red')
+        return
+
+    print_allora_banner()
+    cprint("Welcome to the Allora CLI!", 'green', attrs=['bold'])
+    print(colored("Allora CLI assists in the seamless creation and deployment of Allora validator nodes", 'yellow'))
+    cprint(f"\nThis command will generate some files in the directory named '{name}'.", 'cyan')
+    
+    if click.confirm(colored("\nWould you like to proceed?", 'white', attrs=['bold']), default=True):
+        cprint("\nProceeding with the creation of validator node directory...", 'green')
+
+        os.makedirs(f"{name}/validator/scripts", exist_ok=True)
+
+        file_configs = [
+            {
+                "template_name": "validator-docker-compose.yaml.j2",
+                "file_name": "validator-docker-compose.yaml",
+                "context": {"val_name": name, "network": network}
+            },
+            {
+                "template_name": "start-validator.sh.j2",
+                "file_name": "scripts/start-validator.sh",
+                "context": {"val_name": name, "network": network}
+            },
+        ]
+
+        generate_all_files(env, file_configs, Command.INIT, "validator", name)
+
+        subprocess.run(['chmod', '+x', f'{name}/validator/scripts/start-validator.sh'], check=True)
+    else:
+        cprint("\nOperation cancelled.", 'red')
+
+@click.command()
+@click.option('--address',required=True, help='the account address to be funded.')
+@click.option('--network', required=True, type=click.Choice(['testnet', 'edgenet']), help='Your preffered chain network to fund address from.')
+def fund(address=None, network=None):
+    """fund allora account address"""
+
+    cprint(f"\nfunding allora address: {address}", 'green')
+    cprint(f"Funding account with {network} tokens", 'green')
+    faucet_url = f'https://faucet.{network}.allora.network/'
+    fundAddress(faucet_url, address, network)
+
+cli.add_command(fund)
+
 
-            file_configs = [
-                {
-                    "template_name": "Dockerfile.j2",
-                    "file_name": "Dockerfile",
-                    "context": {}
-                },
-                {
-                    "template_name": "main.py.j2",
-                    "file_name": "main.py",
-                    "context": {}
-                },
-                {
-                    "template_name": "dev-docker-compose.yaml.j2",
-                    "file_name": "dev-docker-compose.yaml",
-                    "context": {"head_peer_id": head_peer_id, "topic_id": topic}
-                },
-                {
-                    "template_name": "requirements.txt.j2",
-                    "file_name": "requirements.txt",
-                    "context": {}
-                },
-                {
-                    "template_name": "gitignore.j2",
-                    "file_name": ".gitignore",
-                    "context": {}
-                },
-                {
-                    "template_name": "env.j2",
-                    "file_name": ".env",
-                    "context": {}
-                },
-                {
-                    "template_name": "config.yaml.j2",
-                    "file_name": "config.yaml",
-                    "context": {"name": name, "topic_id": topic}
-                }
-            ]
 
-            generate_all_files(env, file_configs, Command.INIT, name)
 
-            generateWorkerAccount(name)
-        else:
-            cprint("\nOperation cancelled.", 'red')
-    elif environment == 'prod':
-        devComposePath = os.path.join(os.getcwd(), 'dev-docker-compose.yaml')
-        if not os.path.exists(devComposePath):
-            cprint("You must initialize the worker on dev please run allocmd init --env dev --name <worker name> --topic <topic id> and then run the prod init in the directory created", 'red')
-        else:
-            generateProdCompose(env)
 
 # @click.command()
 # @click.option('--logs', is_flag=True, help="Follow logs immediately after starting services.")
 def run(logs):
     """Starts worker and head nodes locally for development and testing"""
 
     compose_dir = os.getcwd()
@@ -161,14 +164,14 @@
     elif type_ == 'validator':
         deployValidator(env)
     else:
         click.echo("Invalid resource type specified.")
 
 
     
-cli.add_command(init)
+# cli.add_command(init)
 # cli.add_command(run)
 # cli.add_command(terminate)
 # cli.add_command(deploy)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `allocmd-1.0.0/allocmd/utilities/utils.py` & `allocmd-2.0.0/allocmd/utilities/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import click
 import subprocess
 from jinja2 import Environment
 from importlib.resources import files
 from termcolor import colored, cprint
 import time
 import shutil 
-from .typings import Command
+from .typings import Command, BlocklessNodeType
 import re
 import yaml
 
-def create_worker_account(worker_name, faucet_url, type='worker'):
+def create_worker_account(worker_name, faucet_url, type, network="testnet"):
     current_file_dir = os.path.dirname(os.path.abspath(__file__))
     cli_tool_dir = os.path.dirname(current_file_dir)
     allora_chain_dir = os.path.join(cli_tool_dir, 'allora-chain')
 
     if not os.path.exists(allora_chain_dir):
         print(colored("Could not find allora-chain. Initializing allora-chain...", "yellow"))
         subprocess.run(
@@ -70,24 +70,37 @@
         
         hex_coded_pk = hex_pk_result.strip()
         with open(key_path, "a") as file:
             file.write(f"\nHEX-CODED PRIVATE KEY: \n{hex_coded_pk}")
 
         subprocess.run([
                         'curl',
-                        '-Lvvv',
-                        f'{faucet_url}/send/testnet/{address}'
+                        '-L',
+                        f'{faucet_url}send/{network}/{address}'
                     ], stdout=subprocess.DEVNULL)
         
-        print(colored(f"keys created and testnet-funded for this worker. please check config.yaml for your address and mnemonic", "green"))
+        print(colored(f"keys created and {network}-funded for this {type}. please check config.yaml for your address and mnemonic", "green"))
         return mnemonic, hex_coded_pk, address
     else:
         print(colored("'make' is not available in the system's PATH. Please install it or check your PATH settings.", "red"))
         return ''
 
+def fundAddress(faucet_url, address, network="testnet"):
+    try:
+        subprocess.run([
+                        'curl',
+                        '-L',
+                        f'{faucet_url}send/{network}/{address}'
+                    ], stdout=subprocess.DEVNULL)
+        
+        print(colored(f"address funded with {network}-faucet", "green"))
+        return address
+    except subprocess.CalledProcessError as e:
+        click.echo(f"error funding address: {e}", err=True)
+
 def print_allora_banner():
     """Prints an ASCII art styled banner for ALLORA."""
     banner_text = r"""
     
       __      ___      ___        ______     _______        __      
      /""\    |"  |    |"  |      /    " \   /"      \      /""\     
     /    \   ||  |    ||  |     // ____  \ |:        |    /    \    
@@ -96,128 +109,217 @@
  /   /  \\  \( \_|:  \( \_|:  \\        /  |:  __   \  /   /  \\  \ 
 (___/    \___)\_______)\_______)\"_____/   |__|  \___)(___/    \___)
                                                                     
 
     """
     cprint(banner_text, 'blue', attrs=['bold'])
 
-def generate_all_files(env: Environment, file_configs, command: Command, worker_name = ''):
+def generate_all_files(env: Environment, file_configs, command: Command, type, name = ''):
     if command == Command.INIT:
-        cprint(f"Bootstraping '{worker_name}' directory...", 'cyan')
+        cprint(f"Bootstraping '{name}' directory...", 'cyan')
         time.sleep(1) 
 
     for config in file_configs:
         template = env.get_template(config["template_name"])
 
         if command == Command.INIT:
-            file_path = os.path.join(os.getcwd(), f'{worker_name}/{config["file_name"]}')
+            file_path = os.path.join(os.getcwd(), f'{name}/{type}/{config["file_name"]}')
         elif command == Command.DEPLOY: 
             file_path = os.path.join(os.getcwd(), f'{config["file_name"]}')
 
         content = template.render(**config["context"])
         with open(file_path, 'w') as f:
             f.write(content)
 
     if command == Command.INIT:
         cprint("\nAll files bootstrapped successfully. ALLORA!!!", 'green', attrs=['bold'])
 
-def run_key_generate_command(worker_name):
+def run_key_generate_command(worker_name, type):
     command = (
-        f'docker run -it --entrypoint=bash -v "$(pwd)/{worker_name}/data":/data '
+        f'docker run -it --entrypoint=bash -v "$(pwd)/{worker_name}/{type}/data":/data '
         'alloranetwork/allora-inference-base:latest '
-        '-c "mkdir -p /data/head/key /data/worker/key && (cd /data/head/key && allora-keys) && (cd /data/worker/key && allora-keys)"'
+        f'-c "mkdir -p /data/head/key /data/{type}/key && (cd /data/head/key && allora-keys) && (cd /data/{type}/key && allora-keys)"'
     )
     try:
         subprocess.run(command, shell=True, check=True)
-        peer_id_path = os.path.join(os.getcwd(), f'{worker_name}/data/head/key', 'identity')
+        peer_id_path = os.path.join(os.getcwd(), f'{worker_name}/{type}/data/head/key', 'identity')
         with open(peer_id_path, 'r') as file:
-            cprint(f"local workers identity generated successfully.", 'cyan')
+            cprint(f"local {type} identity generated successfully.", 'cyan')
             head_peer_id = file.read().strip()
             return head_peer_id
     except subprocess.CalledProcessError as e:
-        click.echo(f"error generating local workers identity: {e}", err=True)
+        click.echo(f"error generating local {type} identity: {e}", err=True)
 
-def generateWorkerAccount(worker_name):
-    config_path = os.path.join(os.getcwd(), worker_name, 'config.yaml')
+def generateWorkerAccount(worker_name, type):
+    config_path = os.path.join(os.getcwd(), worker_name, type, 'config.yaml')
     try:
         with open(config_path, 'r') as file:
             config = yaml.safe_load(file)
     except yaml.YAMLError as e:
         print(colored(f"Error reading config file: {e}", 'red', attrs=['bold']))
         return
 
     worker_name = config['name']
     faucet_url = config['faucet_url']
     account_details = None
-    if not config['worker']['mnemonic'] or not config['worker']['hex_coded_pk'] or not config['worker']['address']:
-        account_details = create_worker_account(worker_name, faucet_url, 'worker')
+    if not config[type]['mnemonic'] or not config[type]['hex_coded_pk'] or not config[type]['address']:
+        account_details = create_worker_account(worker_name, faucet_url, type)
 
-    mnemonic = account_details[0] if account_details else config['worker']['mnemonic']
-    hex_coded_pk = account_details[1] if account_details else config['worker']['hex_coded_pk']
-    address = account_details[2] if account_details else config['worker']['address']
-
-    if not config['worker']['mnemonic'] or not config['worker']['hex_coded_pk'] or not config['worker']['address']:
-        config['worker']['mnemonic'] = mnemonic
-        config['worker']['hex_coded_pk'] = hex_coded_pk
-        config['worker']['address'] = address
+    mnemonic = account_details[0] if account_details else config[type]['mnemonic']
+    hex_coded_pk = account_details[1] if account_details else config[type]['hex_coded_pk']
+    address = account_details[2] if account_details else config[type]['address']
+
+    if not config[type]['mnemonic'] or not config[type]['hex_coded_pk'] or not config[type]['address']:
+        config[type]['mnemonic'] = mnemonic
+        config[type]['hex_coded_pk'] = hex_coded_pk
+        config[type]['address'] = address
         with open(config_path, 'w') as file:
             yaml.safe_dump(config, file)
 
-def generateProdCompose(env: Environment):
+def generateProdCompose(env: Environment, type):
     """Deploy resource production kubernetes cluster"""
 
-    subprocess.run("mkdir -p ./data/scripts", shell=True, check=True)
-    # subprocess.run("chmod -R +rx ./data/scripts", shell=True, check=True)
+    cprint(f"\nMake sure you are running this command in the appropriate directory [validator, reputer, worker]", 'cyan')
+    cprint(f"\nif not, please cd to the right directory", 'cyan')
+    if click.confirm(colored("\nif you are in the right folder, please proceed", 'white', attrs=['bold']), default=True):
 
-    try:
-        result = subprocess.run("chmod -R +rx ./data/scripts", shell=True, check=True, capture_output=True, text=True)
-        print(result)
-    except subprocess.CalledProcessError as e:
-        print(f"Command '{e.cmd}' returned non-zero exit status {e.returncode}.")
-        if e.stderr:
-            print(f"Stderr: {e.stderr}")
+        subprocess.run("mkdir -p ./data/scripts", shell=True, check=True)
 
-    config_path = os.path.join(os.getcwd(), 'config.yaml')
-    try:
-        with open(config_path, 'r') as file:
-            config = yaml.safe_load(file)
-    except yaml.YAMLError as e:
-        print(colored(f"Error reading config file: {e}", 'red', attrs=['bold']))
-        return
+        try:
+            result = subprocess.run("chmod -R +rx ./data/scripts", shell=True, check=True, capture_output=True, text=True)
+        except subprocess.CalledProcessError as e:
+            print(f"Command '{e.cmd}' returned non-zero exit status {e.returncode}.")
+            if e.stderr:
+                print(f"Stderr: {e.stderr}")
 
-    worker_name = config['name']
-    hex_coded_pk = config['worker']['hex_coded_pk']
-    boot_nodes = config['worker']['boot_nodes']
-    chain_rpc_address = config['worker']['chain_rpc_address']
-    chain_topic_id = config['worker']['chain_topic_id']
-
-    file_configs = [
-        {
-            "template_name": "prod-docker-compose.yaml.j2",
-            "file_name": "prod-docker-compose.yaml",
-            "context": {
-                "worker_name": worker_name, 
-                "boot_nodes": boot_nodes, 
-                "chain_rpc_address": chain_rpc_address, 
-                "topic_id": chain_topic_id, 
-            }
-        },
-        {
-            "template_name": "init.sh.j2",
-            "file_name": "data/scripts/init.sh",
-            "context": {
-                "worker_name": worker_name, 
-                "hex_coded_pk": hex_coded_pk
+        config_path = os.path.join(os.getcwd(), 'config.yaml')
+        try:
+            with open(config_path, 'r') as file:
+                config = yaml.safe_load(file)
+        except yaml.YAMLError as e:
+            print(colored(f"Error reading config file: {e}", 'red', attrs=['bold']))
+            return
+
+        worker_name = config['name']
+        hex_coded_pk = config[type]['hex_coded_pk']
+        boot_nodes = config[type]['boot_nodes']
+        chain_rpc_address = config[type]['chain_rpc_address']
+        chain_topic_id = config[type]['chain_topic_id']
+
+        file_configs = [
+            {
+                "template_name": "prod-docker-compose.yaml.j2",
+                "file_name": "prod-docker-compose.yaml",
+                "context": {
+                    "worker_name": worker_name, 
+                    "boot_nodes": boot_nodes, 
+                    "chain_rpc_address": chain_rpc_address, 
+                    "topic_id": chain_topic_id, 
+                }
+            },
+            {
+                "template_name": "init.sh.j2",
+                "file_name": "data/scripts/init.sh",
+                "context": {
+                    "worker_name": worker_name, 
+                    "hex_coded_pk": hex_coded_pk
+                }
             }
-        }
-    ]
+        ]
+
+        generate_all_files(env, file_configs, Command.DEPLOY, type)
+        cprint(f"production docker compose file generated to be deployed", 'green')
+        cprint(f"please run chmod -R +rx ./data/scripts to grant script access to the image", 'yellow')
+    else:
+        cprint("\nOperation cancelled.", 'red')
+
+
+def blocklessNode(environment, env, type, name=None, topic=None):
+    """Initialize your Allora Worker Node with necessary boilerplates"""
+
+    if not check_docker_running():
+        cprint("Docker is not running on your machine, please start docker before running this command", 'red')
+        return
+    
+    if environment == 'dev':
+        if topic is None:
+            cprint(f"You must provide topic id when generating {type} in development", 'red')
+            return
+        elif name is None:
+            cprint(f"You must provide name when generating {type} in development", 'red')
+            return
+
+        print_allora_banner()
+        cprint("Welcome to the Allora CLI!", 'green', attrs=['bold'])
+        print(colored(f"Allora CLI assists in the seamless creation and deployment of Allora {type} nodes", 'yellow'))
+        cprint(f"\nThis command will generate some files in the directory named '{name}'.", 'cyan')
+        
+        if click.confirm(colored("\nWould you like to proceed?", 'white', attrs=['bold']), default=True):
+            cprint(f"\nProceeding with the creation of {type} node directory...", 'green')
+
+            head_peer_id = run_key_generate_command(name, type)
+
+            file_configs = [
+                {
+                    "template_name": "Dockerfile.j2",
+                    "file_name": "Dockerfile",
+                    "context": {}
+                },
+                {
+                    "template_name": "main.py.j2",
+                    "file_name": "main.py",
+                    "context": {}
+                },
+                {
+                    "template_name": "dev-docker-compose.yaml.j2",
+                    "file_name": "dev-docker-compose.yaml",
+                    "context": {"head_peer_id": head_peer_id, "topic_id": topic, "b7s_type": type}
+                },
+                {
+                    "template_name": "requirements.txt.j2",
+                    "file_name": "requirements.txt",
+                    "context": {}
+                },
+                {
+                    "template_name": "gitignore.j2",
+                    "file_name": ".gitignore",
+                    "context": {}
+                },
+                {
+                    "template_name": "env.j2",
+                    "file_name": ".env",
+                    "context": {}
+                },
+                {
+                    "template_name": "config.yaml.j2",
+                    "file_name": "config.yaml",
+                    "context": {"name": name, "topic_id": topic, "b7s_type": type}
+                }
+            ]
+
+            generate_all_files(env, file_configs, Command.INIT, type, name)
+
+            generateWorkerAccount(name, type)
+        else:
+            cprint("\nOperation cancelled.", 'red')
+    elif environment == 'prod':
+        devComposePath = os.path.join(os.getcwd(), 'dev-docker-compose.yaml')
+        if not os.path.exists(devComposePath):
+            cprint(f"You must initialize the {type} on dev please run allocmd generate {type} --env dev --name <{type} name> --topic <topic id> and then run the prod generate in the directory created", 'red')
+        else:
+            generateProdCompose(env, type)
+
+
+
+
+
+
+
+
 
-    generate_all_files(env, file_configs, Command.DEPLOY)
-    cprint(f"production docker compose file generated to be deployed", 'green')
-    cprint(f"please run chmod -R +rx ./data/scripts to grant script access to the image", 'yellow')
 
 def deployWorker(env: Environment):
     """Deploy resource production kubernetes cluster"""
 
     print(colored('\nREQUIREMENTS', 'yellow', attrs=['bold']))
     print(colored('1. Ensure to have the Dockerfile built and docker image pushed to your preferred registry.\n'
                   '   You should have your image URI and tag available\n', 'yellow'))
@@ -412,7 +514,15 @@
             print(colored("Helm chart 'universal-helm' installed successfully.", 'green'))
             
         except subprocess.CalledProcessError as e:
             print(colored(f"An error occurred: {e}", 'red'))
             return
     else:
         print(colored('Operation cancelled.', 'magenta'))
+
+def check_docker_running():
+    """Check if Docker daemon is running."""
+    try:
+        subprocess.run(['docker', 'info'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, check=True)
+        return True
+    except subprocess.CalledProcessError:
+        return False
```

### Comparing `allocmd-1.0.0/allocmd.egg-info/PKG-INFO` & `allocmd-2.0.0/allocmd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 Metadata-Version: 2.1
 Name: allocmd
-Version: 1.0.0
+Version: 2.0.0
 Summary: A CLI tool for creating Allora Chain Worker Nodes
 Home-page: UNKNOWN
 Author: Upshot Technologies
 Author-email: tobi@upshot.xyz
 License: UNKNOWN
 Description: # Building a Worker Node with the allocmd CLI
         ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
         ![Python!](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
         ![Apache License](https://img.shields.io/badge/Apache%20License-D22128?style=for-the-badge&logo=Apache&logoColor=white)
         
-        The `allocmd` is a CLI tool that handles worker nodes' seamless creation and deployment. With this tool, you do not need to write the worker node from scratch, the CLI tool will help you bootstrap all the needed components to get worker nodes working. All you have to do is to update the `config.yaml` file with your custom parameters, update the provided`main.py`to communicate with your inference server, run the deploy command, and your worker should be up and running.
+        The `allocmd` is a CLI tool that handles seamless creation of Allora external resources built to integrate with Allora chain. With this tool, you do not need to write the worker or reputer node or even a validator from scratch, the CLI tool will help you bootstrap all the needed components to get resource working.
         
-        To build a worker node with `allocmd`, you will need to follow the following steps:
+        The following are the list of stuff that can don with this tool at the moment
+        1. Generating worker node files
+        2. Genrating reputer node files
+        3. Generating validator node files
+        4. Funding of testnet account addresses
         
-        ### 1. Install `allocmd` CLI
+        for all the files generation commands, the tool will help in generation of the needed files and their respective docker files and you can spin them up as usual docker containers with docker-compose
+        
+        ## Install `allocmd` CLI
         
         You will begin with installing the tool on your machine. 
         
         ```shell
         pip install allocmd
         ```
         
-        > you can run `allocmd --help` to get general help or `allocmd [command] --help` to get help relating to a particular command.
+        > you should use version 1.0.0 for Allora Chain v1 and version 2.0.0 for Allora Chain v2. Run `allocmd --help` to get general help or `allocmd [command] --help` to get help relating to a particular command.
         
-        ### 2. Initialize the worker for development
+        ## Initializing resources
+        ### Initialize the worker/reputer for development
+        > Note that all commands here will pass for both worker or reputer node
         
-        The next step is initializing the CLI to bootstrap all the needed components to get your worker running. The following command will handle the initialization process. It will create all the files in the appropriate directories and generate identities for your node to be used for local development.
+        The next step is initializing the CLI to bootstrap all the needed components to get your worker or reputer running. The following command will handle the initialization process. It will create all the files in the appropriate directories and generate identities for your node to be used for local development.
         
         ```shell
-        allocmd init --name <preffered name> --topic <topic id> --env dev
+        allocmd generate worker --name <preffered name> --topic <topic id> --env dev
         ```
         
-        Before running this command you will have to [pick the topic Id ](https://docs.allora.network/docs/existing-allora-appchain-topics)you wish to generate inference for after which you can run this command with the topic Id. The command will auto-create some files, the most important of which is the `dev-docker-compose.yaml`file which is an already complete docker-compose that you can run immediately to see your worker and head nodes running perfectly on your local machine. You can edit the files as you wish. for instance the `main.py` is meant for you to call your inference server, hence you will have to edit the sample code with actual URLs and logic as you prefer.
+        Before running this command you will have to [pick the topic Id ](https://docs.allora.network/docs/existing-allora-appchain-topics)you wish to generate inference for after which you can run this command with the topic Id. The command will auto-create some files, the most important of which is the `dev-docker-compose.yaml`file which is an already complete docker-compose that you can run immediately to see your worker/reputer and head nodes running perfectly on your local machine. You can edit the files as you wish. for instance the `main.py` is meant for you to call your inference server, hence you will have to edit the sample code with actual URLs and logic as you prefer.
         
-        When you run the docker-compose (`docker-compose -f dev-docker-compose.yaml up --build`), maybe after you have written and tested your logic in `main.py`, you then should be seeing the logs from the nodes, and you should be able to make a request to your head node and see it get a response from the worker node. Note that in production, you won't be the one to make the inference request, as the Allora chain will do this at the cadence provided by the topic creator.
+        When you run the docker-compose (`docker-compose -f dev-docker-compose.yaml up --build`), maybe after you have written and tested your logic in `main.py`, you then should be seeing the logs from the nodes, and you should be able to make a request to your head node and see it get a response from the worker/reputer node. Note that in production, you won't be the one to make the inference request, as the Allora chain will do this at the cadence provided by the topic creator.
         
         You can test your node by running the following curl command:
         
         ```
         curl --location 'http://localhost:6000/api/v1/functions/execute' --header 'Accept: application/json, text/plain, */*' --header 'Content-Type: application/json;charset=UTF-8' --data '{
             "function_id": "bafybeigpiwl3o73zvvl6dxdqu7zqcub5mhg65jiky2xqb4rdhfmikswzqm",
             "method": "allora-inference-function.wasm",
@@ -60,23 +68,35 @@
                 "timeout" : 2
             }
         }' | jq
         ```
         
         The `<TOPIC_ID>` needs to be [an existing topic on the chain](https://docs.allora.network/docs/existing-allora-appchain-topics). The `<argument>` is what the topic is expecting to receive to perform the inference (as an indication to test, you can use the `DefaultArg`  value from the topic on-chain, e.g. for ETH prediction topic, it should be `"ETH"`).
         
-        ### 3. Initialize the worker for production
+        ### Initialize the worker/reputer for production
         
-        Your worker node is now ready to be deployed, the `main.py` has been modified, all env variables passed, and the worker node is running locally and you are now ready to deploy your worker to run in the production environment. The following command will handle the generation of the `prod-docker-compose.yaml` file which contains all the keys and parameters needed for your worker to function perfectly in production.
+        Your worker/reputer node is now ready to be deployed, the `main.py` has been modified, all env variables passed, and the worker/reputer node is running locally and you are now ready to deploy your worker/reputer to run in the production environment. The following command will handle the generation of the `prod-docker-compose.yaml` file which contains all the keys and parameters needed for your worker/reputer to function perfectly in production.
         
         ```shell
-        allocmd init --env prod
+        allocmd generate worker --env prod
         ```
         
         By running this command, `prod-docker-compose.yaml` will be generated with appropriate keys and parameters. You can now run the docker-compose file or deploy the whole codebase in your preferred cloud instance. At this stage, your worker should be responding to inference request from the Allora Chain.
         
+        ### Initialize validator production
+        ```shell
+        allocmd generate validator --name <validator-name> --network <testnet or mainnet>
+        ```
+        The above command can generate validator files and you can then use docker-compose to deploy
+        
+        ### Fund account address
+        ```shell
+        allocmd fund <address> 
+        ```
+        The above command takes address and fund the account with Allora Faucet
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `allocmd-1.0.0/setup.py` & `allocmd-2.0.0/setup.py`

 * *Files identical despite different names*

