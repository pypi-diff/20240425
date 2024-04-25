# Comparing `tmp/easytl-0.2.0b2.tar.gz` & `tmp/easytl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.2.0b2.tar", last modified: Thu Apr 18 14:24:15 2024, max compression
+gzip compressed data, was "easytl-0.2.1.tar", last modified: Thu Apr 25 01:33:50 2024, max compression
```

## Comparing `easytl-0.2.0b2.tar` & `easytl-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.248703 easytl-0.2.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.240702 easytl-0.2.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.244703 easytl-0.2.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-18 14:22:45.000000 easytl-0.2.0b2/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-18 14:22:45.000000 easytl-0.2.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-18 14:22:45.000000 easytl-0.2.0b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-18 14:24:15.248703 easytl-0.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-18 14:22:45.000000 easytl-0.2.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-18 14:22:45.000000 easytl-0.2.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:24:15.248703 easytl-0.2.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.240702 easytl-0.2.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.244703 easytl-0.2.0b2/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    49369 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15958 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.248703 easytl-0.2.0b2/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.248703 easytl-0.2.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 14:22:45.000000 easytl-0.2.0b2/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-18 14:22:45.000000 easytl-0.2.0b2/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.466145 easytl-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.466145 easytl-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-25 01:32:16.000000 easytl-0.2.1/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-25 01:32:16.000000 easytl-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-25 01:32:16.000000 easytl-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-25 01:33:50.470145 easytl-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-25 01:32:16.000000 easytl-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 01:32:16.000000 easytl-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:33:50.470145 easytl-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.466145 easytl-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52195 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 01:32:16.000000 easytl-0.2.1/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 01:33:50.000000 easytl-0.2.1/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:33:50.470145 easytl-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-25 01:32:16.000000 easytl-0.2.1/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-25 01:32:16.000000 easytl-0.2.1/tests/passing.py
```

### Comparing `easytl-0.2.0b2/.github/workflows/workflow.yml` & `easytl-0.2.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/.gitignore` & `easytl-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/LICENSE.md` & `easytl-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/PKG-INFO` & `easytl-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,122 @@
-Metadata-Version: 2.1
-Name: easytl
-Version: 0.2.0b2
-Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
-Author-email: Bikatr7 <Tetralon07@gmail.com>
-Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
-Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.1
-Requires-Dist: deepl==1.16.1
-Requires-Dist: openai==1.13.3
-Requires-Dist: backoff==2.2.1
-Requires-Dist: tiktoken==0.6.0
-
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
+- [Features](#features)
+- [API Usage](#api-usage)
 - [License](#license)
 - [Contact](#contact)
 - [Contribution](#contribution)
 - [Notes](#notes)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
 Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 
-EasyTL has a trello board:
+EasyTL has a Trello board for tracking features and issues:
 https://trello.com/b/Td555CoW/easytl
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
-Then, you can translate Japanese text using DeepL by importing the global client.
+Then, you can translate Japanese text using by importing the global client.
+
+For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
-## set your api key
+## Set your API key
 EasyTL.set_api_key("deepL", "your_api_key_here")
 
-## you can also validate your api keys, translation functions will do this automatically
+## You can also validate your API keys; translation functions will do this automatically
 is_valid, e = EasyTL.validate_api_key("deepL")
 
 translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality.
-
-## easytl also has a generic translate method, which defaults to deepl, requires text, and kwargs for the translate method it uses.
-
-translated_text = EasyTL.translate("私は日本語が話せます", target_lang="EN")
-
-## There is also a calculate cost method.
-## for deepl, model is deepl
-num_characters, cost, model = EasyTL.calculate_cost("私は日本語が話せます", "deepL") ## Text to translate, service to use
-
-## or for llms
-## last 2 arguments are optional, defaults to gpt-4 and "Translate to English"
-num_tokens, cost, model = EasyTL.calculate_cost("私は日本語が話せます", "openai", "gpt-4", "Translate to English") ## Text to translate, service to use, model to use, prompt to use
-
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
 Python 3.10+
 
 EasyTL can be installed using pip:
 
-
 ```bash
 pip install easytl
 ```
 
 This will install EasyTL along with its dependencies and requirements.
 
 These are the dependencies/requirements that will be installed:
 ```
 setuptools>=61.0
-
 wheel
-
 setuptools_scm>=6.0
-
 tomli
-
 google-generativeai==0.5.1
-
 deepl==1.16.1
-
 openai==1.13.3
-
 backoff==2.2.1
-
 tiktoken==0.6.0
+```
+---------------------------------------------------------------------------------------------------------------------------------------------------
+
+**Features**<a name="features"></a>
 
+EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
+
+- Support for multiple translation APIs including OpenAI, DeepL, and Gemini.
+- Simple API key management.
+- Methods to validate API keys before usage.
+- Cost estimation tools to help manage usage based on text length and service.
+- Highly customizable translation options, with the API's original features.
+- Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
+
+---------------------------------------------------------------------------------------------------------------------------------------------------
+
+**API Usage**<a name="api-usage"></a>
+
+### Translating Text
+
+Use `deepl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+
+### Cost Calculation
+
+The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
+
+characters or tokens depending on the service.
+
+```python
+num_characters, cost, model = EasyTL.calculate_cost("Example text.", "deepL")
 ```
+
+### API Key Management
+
+API keys can be set and validated using `set_api_key` and `validate_api_key` methods to ensure they are active and correct before submitting translation requests.
+
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
-Under the LGPLv2.1, any modifications made to EasyTL's libraries must be shared under the same license, ensuring the open source nature of the library itself is maintained. However, it allows the wider work that includes the library to remain under different licensing terms, provided the terms of the LGPLv2.1 are met for the library.
-
-I encourage the use of EasyTL within all projects. This approach ensures a balance between open collaboration and the flexibility required for proprietary development.
-
-For a thorough explanation of the conditions and how they may apply to your use of the project, please review the full license text. This comprehensive documentation will offer guidance on your rights and obligations when utilizing LGPLv2.1 licensed software.
-
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
 If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
@@ -144,8 +133,8 @@
 
 **Notes**<a name="notes"></a>
 
 EasyTL was originally developed as a part of [Kudasai](https://github.com/Bikatr7/Kudasai), a Japanese preprocessor later turned Machine Translator. It was later split off into its own package to be used independently of Kudasai for multiple reasons.
 
 This package is also my second serious attempt at creating a Python package, so I'm sure there are some things that could be improved. Feedback is welcomed.
 
----------------------------------------------------------------------------------------------------------------------------------------------------
+---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.2.0b2/pyproject.toml` & `easytl-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     "deepl==1.16.1",
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0"
 ]
 
 name = "easytl"
-version = "v0.2.0-beta-2"
+version = "v0.2.1"
 authors = [
   { name="Bikatr7", email="Tetralon07@gmail.com" },
 ]
-description = "Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text."
+description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, and Gemini."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
```

### Comparing `easytl-0.2.0b2/src/easytl/__init__.py` & `easytl-0.2.1/src/easytl/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 from .classes import Message, SystemTranslationMessage, ModelTranslationMessage
 from .classes import ChatCompletion
 from .classes import GenerateContentResponse, AsyncGenerateContentResponse, GenerationConfig
 
 from .util import MODEL_COSTS, ALLOWED_GEMINI_MODELS, ALLOWED_OPENAI_MODELS, VALID_JSON_OPENAI_MODELS
 
-from .exceptions import DeepLException, GoogleAPIError, OpenAIError, EasyTLException, InvalidAPIKeyException, InvalidEasyTLSettings
+from .exceptions import DeepLException, GoogleAPIError, OpenAIError, EasyTLException, InvalidAPIKeyException, InvalidEasyTLSettingsException, InvalidTextInputException, InvalidAPITypeException, InvalidResponseFormatException
 from .exceptions import AuthenticationError, InternalServerError, RateLimitError, APITimeoutError, APIConnectionError, APIStatusError
 from .exceptions import AuthorizationException, QuotaExceededException
 from .exceptions import GoogleAuthError
```

### Comparing `easytl-0.2.0b2/src/easytl/classes.py` & `easytl-0.2.1/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/src/easytl/decorators.py` & `easytl-0.2.1/src/easytl/decorators.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/src/easytl/deepl_service.py` & `easytl-0.2.1/src/easytl/deepl_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ## Copyright Bikatr7 (https://github.com/Bikatr7)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
+import time
 
 ## third-party libraries
 from deepl.translator import Translator
 
 from .util import _convert_iterable_to_str
 from .decorators import _async_logging_decorator, _sync_logging_decorator
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
@@ -31,34 +32,20 @@
     _non_splitting_tags:str | typing.List[str] | None = None
     _splitting_tags:str | typing.List[str] | None = None
     _ignore_tags:str | typing.List[str] | None = None
 
     _semaphore_value:int = 30
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
+    _rate_limit_delay:float | None = None 
+
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
 
-##-------------------start-of-_set_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _set_decorator(decorator:typing.Callable | None) -> None:
-
-        """
-
-        Sets the decorator to use for the DeepL service. Should be a callable that returns a decorator or None.
-
-        Parameters:
-        decorator (callable or None) : The decorator to use for the DeepL service.
-
-        """
-
-        DeepLService._decorator_to_use = decorator
-
 ##-------------------start-of-set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     def _set_attributes(target_lang:str | Language = "EN",
                         source_lang:str | Language | None = None,
                         context:str | None = None,
                         split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
@@ -66,42 +53,52 @@
                         formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                         glossary:str | GlossaryInfo | None = None,
                         tag_handling:typing.Literal["xml", "html"] | None = None,
                         outline_detection:bool | None = None,
                         non_splitting_tags:str | typing.List[str] | None = None,
                         splitting_tags:str | typing.List[str] | None = None,
                         ignore_tags:str | typing.List[str] | None = None,
-                        semaphore:int | None = None,
+                        decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
+                        semaphore:int | None = None,
+                        rate_limit_delay:float | None = None
                         ) -> None:
 
         """
 
         Sets the attributes of the DeepL client.
 
         """
 
+        ## API Attributes
+
         DeepLService._target_lang = target_lang
         DeepLService._source_lang = source_lang
         DeepLService._context = context
         DeepLService._split_sentences = split_sentences
         DeepLService._preserve_formatting = preserve_formatting
         DeepLService._formality = formality
         DeepLService._glossary = glossary
         DeepLService._tag_handling = tag_handling
         DeepLService._outline_detection = outline_detection
         DeepLService._non_splitting_tags = non_splitting_tags
         DeepLService._splitting_tags = splitting_tags
         DeepLService._ignore_tags = ignore_tags
 
+        ## Service Attributes
+
+        DeepLService._decorator_to_use = decorator
+
+        DeepLService._log_directory = logging_directory
+
         if(semaphore is not None):
             DeepLService._semaphore_value = semaphore
             DeepLService._semaphore = asyncio.Semaphore(semaphore)
 
-        DeepLService._log_directory = logging_directory
+        DeepLService._rate_limit_delay = rate_limit_delay
 
 ##-------------------start-of-_prepare_translation_parameters()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _prepare_translation_parameters(text:str):
 
         """
@@ -153,14 +150,17 @@
         text (string) : The text to translate.
 
         Returns:
         translation (TextResult or list of TextResult) : The translation result.
 
         """
 
+        if(DeepLService._rate_limit_delay is not None):
+            time.sleep(DeepLService._rate_limit_delay)
+
         params = DeepLService._prepare_translation_parameters(text)
 
         try:
 
             if(DeepLService._decorator_to_use is None):
                 return DeepLService._translator.translate_text(**params)
             
@@ -187,14 +187,17 @@
         Returns:
         translation (TextResult or list of TextResult) : The translation result.
 
         """
 
         async with DeepLService._semaphore:
 
+            if(DeepLService._rate_limit_delay is not None):
+                await asyncio.sleep(DeepLService._rate_limit_delay)
+
             params = DeepLService._prepare_translation_parameters(text)
 
             try:
                 if(DeepLService._decorator_to_use is None):
                     loop = asyncio.get_running_loop()
                     return await loop.run_in_executor(None, lambda: DeepLService._translator.translate_text(**params))
                 
@@ -248,30 +251,14 @@
 
             return _validity, None
 
         except Exception as _e:
 
             return _validity, _e
         
-##-------------------start-of-_get_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _get_decorator() -> typing.Union[typing.Callable, None]:
-
-        """
-
-        Returns the decorator to use for the DeepL service.
-
-        Returns:
-        decorator (callable) : The decorator to use.
-
-        """
-
-        return DeepLService._decorator_to_use
-    
 ##-------------------start-of-_calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     def _calculate_cost(text:str | typing.Iterable) -> typing.Tuple[int, float, str]:
 
         """
```

### Comparing `easytl-0.2.0b2/src/easytl/easytl.py` & `easytl-0.2.1/src/easytl/easytl.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 ## custom modules
 from .deepl_service import DeepLService
 from .gemini_service import GeminiService
 from .openai_service import OpenAIService
 
 from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion
-from .exceptions import DeepLException, GoogleAPIError,OpenAIError, EasyTLException
+from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException
 
-from .util import _convert_to_correct_type, _validate_easytl_translation_settings, _is_iterable_of_strings
+from .util import _convert_to_correct_type, _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences
 
 class EasyTL:
 
     """
     
     EasyTL global client, used to interact with Translation APIs.
 
@@ -29,14 +29,16 @@
 
     Use test_api_key_validity() to test the validity of the API key for the specified API type. (Optional) Will be done automatically when calling translation functions.
 
     Use translate() to translate text using the specified service with it's appropriate kwargs. Or specify the service by calling the specific translation function. (e.g. openai_translate())
 
     Use calculate_cost() to calculate the cost of translating text using the specified service. (Optional)
 
+    See the documentation for each function for more information.
+
     """
 
 ##-------------------start-of-set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def set_api_key(api_type:typing.Literal["deepl", "gemini", "openai"], api_key:str) -> None:
         
@@ -46,24 +48,23 @@
 
         Parameters:
         api_type (literal["deepl", "gemini", "openai"]) : The API type to set the key for.
         api_key (string) : The API key to set.
 
         """
 
-        assert api_type in ["deepl", "gemini", "openai"], ValueError("Invalid API type specified.")
+        service_map = {
+            "deepl": DeepLService,
+            "gemini": GeminiService,
+            "openai": OpenAIService
+        }
 
-        if(api_type == "deepl"):
-            DeepLService._set_api_key(api_key)
+        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini' and 'openai'.")
 
-        elif(api_type == "gemini"):
-            GeminiService._set_api_key(api_key)
-            
-        elif(api_type == "openai"):
-            OpenAIService._set_api_key(api_key)
+        service_map[api_type]._set_api_key(api_key)
 
 ##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
             
     @staticmethod
     def test_api_key_validity(api_type:typing.Literal["deepl", "gemini", "openai"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
         
         """
@@ -74,60 +75,42 @@
         api_type (literal["deepl", "gemini", "openai"]) : The API type to test the key for.
 
         Returns:
         (bool) : Whether the API key is valid.
         (Exception) : The exception that was raised, if any. None otherwise.
 
         """
-
-        if(api_type == "deepl"):
-            _is_valid, _e = DeepLService._test_api_key_validity()
-
-            if(_is_valid == False):
-
-                ## make sure issue is due to DeepL and not the fault of easytl, cause it needs to be raised if it is
-                assert isinstance(_e, DeepLException), _e
-
-                return False, _e
-            
-        if(api_type == "gemini"):
-            
-            _is_valid, _e = GeminiService._test_api_key_validity()
-
-            if(_is_valid == False):
-
-                ## make sure issue is due to Gemini and not the fault of easytl, cause it needs to be raised if it is
-                assert isinstance(_e, GoogleAPIError), _e
-
-                return False, _e
         
-        if(api_type == "openai"):
-            
-            _is_valid, _e = OpenAIService._test_api_key_validity()
+        api_services = {
+            "deepl": {"service": DeepLService, "exception": DeepLException},
+            "gemini": {"service": GeminiService, "exception": GoogleAPIError},
+            "openai": {"service": OpenAIService, "exception": OpenAIError}
+        }
 
-            if(_is_valid == False):
+        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini' and 'openai'.")
 
-                ## make sure issue is due to OpenAI and not the fault of easytl, cause it needs to be raised if it is
-                assert isinstance(_e, OpenAIError), _e
+        _is_valid, _e = api_services[api_type]["service"]._test_api_key_validity()
 
-                return False, _e
-            
-        assert api_type in ["deepl", "gemini", "openai"], ValueError("Invalid API type specified.")
+        if(not _is_valid):
+            ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
+            assert isinstance(_e, api_services[api_type]["exception"]), _e
+            return False, _e
 
         return True, None
         
 ##-------------------start-of-deepl_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def deepl_translate(text:typing.Union[str, typing.Iterable[str]],
                         target_lang:str | Language = "EN-US",
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
                         response_type:typing.Literal["text", "raw"] | None = "text",
+                        translation_delay:float | None = None,
                         source_lang:str | Language | None = None,
                         context:str | None = None,
                         split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
                         preserve_formatting:bool | None = None,
                         formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                         glossary:str | GlossaryInfo | None = None,
                         tag_handling:typing.Literal["xml", "html"] | None = None,
@@ -140,96 +123,94 @@
 
         Translates the given text to the target language using DeepL.
 
         This function assumes that the API key has already been set.
 
         DeepL has backoff retrying implemented by default.
 
+        Due to how DeepL's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
+
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         source_lang (string or Language or None) : The source language to translate from.
-        context (string or None) : Additional information for the translator to be considered when translating. Not translated itself.
+        context (string or None) : Additional information for the translator to be considered when translating. Not translated itself. This is a DeepL alpha feature and may be removed at any time.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
         preserve_formatting (bool or None) : Whether to preserve formatting.
         formality (literal or Formality or None) : The formality level to use.
         glossary (string or GlossaryInfo or None) : The glossary to use.
         tag_handling (literal or None) : How to handle tags.
         outline_detection (bool or None) : Whether to detect outlines.
         non_splitting_tags (string or list or None) : Tags that should not be split.
         splitting_tags (string or list or None) : Tags that should be split.
         ignore_tags (string or list or None) : Tags that should be ignored.
 
         Returns:
-        translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+        result (string or list - string or TextResult or list - TextResult) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise.
 
         """
 
-        assert response_type in ["text", "raw"], ValueError("Invalid response type specified. Must be 'text' or 'raw'.")
+        assert response_type in ["text", "raw"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'raw'.")
 
         EasyTL.test_api_key_validity("deepl")
 
-        DeepLService._set_decorator(decorator)
-
         if(override_previous_settings == True):
             DeepLService._set_attributes(target_lang = target_lang, 
                                         source_lang = source_lang, 
                                         context = context, 
                                         split_sentences = split_sentences,
                                         preserve_formatting = preserve_formatting, 
                                         formality = formality, 
                                         glossary = glossary, 
                                         tag_handling = tag_handling, 
                                         outline_detection = outline_detection, 
                                         non_splitting_tags = non_splitting_tags, 
                                         splitting_tags = splitting_tags, 
                                         ignore_tags = ignore_tags,
+                                        decorator=decorator,
+                                        logging_directory=logging_directory,
                                         semaphore=None,
-                                        logging_directory=logging_directory)
+                                        rate_limit_delay=translation_delay)
             
         if(isinstance(text, str)):
             result = DeepLService._translate_text(text)
         
-            assert not isinstance(result, list), "Unexpected error occurred. Please try again."
+            assert not isinstance(result, list), EasyTLException("Malformed response received. Please try again.")
 
-            if(response_type == "text"):
-                return result.text
-            
-            else:
-                return result
+            result = result if response_type == "raw" else result.text
         
         elif(_is_iterable_of_strings(text)):
 
             results = [DeepLService._translate_text(t) for t in text]
 
-            assert isinstance(results, list), "Unexpected error occurred. Please try again."
+            assert isinstance(results, list), EasyTLException("Malformed response received. Please try again.")
 
-            if(all(isinstance(_r, TextResult) for _r in results)):
-                if(response_type == "text"):
-                    return [_r.text for _r in results] # type: ignore
-                
-                else:
-                    return results # type: ignore
+            result = [_r.text for _r in results] if response_type == "text" else results # type: ignore    
+            
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
         
-        raise ValueError("text must be a string or an iterable of strings.")
+        return result
         
 ##-------------------start-of-deepl_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def deepl_translate_async(text:typing.Union[str, typing.Iterable[str]],
                             target_lang:str | Language = "EN-US",
                             override_previous_settings:bool = True,
                             decorator:typing.Callable | None = None,
                             logging_directory:str | None = None,
-                            semaphore:int | None = None,
                             response_type:typing.Literal["text", "raw"] | None = "text",
+                            semaphore:int | None = None,
+                            translation_delay:float | None = None,
                             source_lang:str | Language | None = None,
                             context:str | None = None,
                             split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
                             preserve_formatting:bool | None = None,
                             formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                             glossary:str | GlossaryInfo | None = None,
                             tag_handling:typing.Literal["xml", "html"] | None = None,
@@ -244,96 +225,93 @@
         
         Translates the given text to the target language using DeepL.
         Will generally be faster for iterables. Order is preserved.
 
         This function assumes that the API key has already been set.
 
         DeepL has backoff retrying implemented by default.
+
+        Due to how DeepL's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
         
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        semaphore (int) : The number of concurrent requests to make. Default is 30.
         response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
+        semaphore (int) : The number of concurrent requests to make. Default is 30.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         source_lang (string or Language or None) : The source language to translate from.
-        context (string or None) : Additional information for the translator to be considered when translating. Not translated itself.
+        context (string or None) : Additional information for the translator to be considered when translating. Not translated itself. This is a DeepL alpha feature and may be removed at any time.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
         preserve_formatting (bool or None) : Whether to preserve formatting.
         formality (literal or Formality or None) : The formality level to use.
         glossary (string or GlossaryInfo or None) : The glossary to use.
         tag_handling (literal or None) : How to handle tags.
         outline_detection (bool or None) : Whether to detect outlines.
         non_splitting_tags (string or list or None) : Tags that should not be split.
         splitting_tags (string or list or None) : Tags that should be split.
         ignore_tags (string or list or None) : Tags that should be ignored.
 
         Returns:
-        translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+        result (string or list - string or TextResult or list - TextResult) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise.
 
         """
 
-        assert response_type in ["text", "raw"], ValueError("Invalid response type specified. Must be 'text' or 'raw'.")
+        assert response_type in ["text", "raw"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'raw'.")
 
         EasyTL.test_api_key_validity("deepl")
 
-        DeepLService._set_decorator(decorator)
-
         if(override_previous_settings == True):
             DeepLService._set_attributes(target_lang=target_lang, 
                                         source_lang=source_lang, 
                                         context=context, 
                                         split_sentences=split_sentences,
                                         preserve_formatting=preserve_formatting, 
                                         formality=formality, 
                                         glossary=glossary, 
                                         tag_handling=tag_handling, 
                                         outline_detection=outline_detection, 
                                         non_splitting_tags=non_splitting_tags, 
                                         splitting_tags=splitting_tags, 
                                         ignore_tags=ignore_tags,
+                                        decorator=decorator,
+                                        logging_directory=logging_directory,
                                         semaphore=semaphore,
-                                        logging_directory=logging_directory)
-            
+                                        rate_limit_delay=translation_delay)
         if(isinstance(text, str)):
             _result = await DeepLService._async_translate_text(text)
 
-            assert not isinstance(_result, list), "Unexpected error occurred. Please try again."
+            assert not isinstance(_result, list), EasyTLException("Malformed response received. Please try again.")
 
-            if(response_type == "text"):
-                return _result.text
-            
-            else:
-                return _result
+            result = _result if response_type == "raw" else _result.text
             
         elif(_is_iterable_of_strings(text)):
             _tasks = [DeepLService._async_translate_text(t) for t in text]
             _results = await asyncio.gather(*_tasks)
             
-            assert isinstance(_results, list), "Unexpected error occurred. Please try again."
+            assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
 
-            if(all(isinstance(_r, TextResult) for _r in _results)):
-                if(response_type == "text"):
-                    return [_r.text for _r in _results] # type: ignore
+            result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
                 
-                else:
-                    return _results # type: ignore
-            
-        raise ValueError("text must be a string or an iterable of strings.")
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
+        
+        return result
             
 ##-------------------start-of-gemini_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def gemini_translate(text:typing.Union[str, typing.Iterable[str]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
                         response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                        translation_delay:float | None = None,
                         translation_instructions:str | None = None,
                         model:str="gemini-pro",
                         temperature:float=0.5,
                         top_p:float=0.9,
                         top_k:int=40,
                         stop_sequences:typing.List[str] | None=None,
                         max_output_tokens:int | None=None) -> typing.Union[typing.List[str], str, GenerateContentResponse, typing.List[GenerateContentResponse]]:
@@ -344,109 +322,98 @@
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
-        It is not known whether Gemini has backoff retrying implemented. (Their API is a mess.)
+        It is not known whether Gemini has backoff retrying implemented. Assume it does not exist. 
         
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a GenerateContentResponse object, 'json' returns a json-parseable string.
-        translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use. 
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
         stop_sequences (list or None) : The sequences to stop at.
         max_output_tokens (int or None) : The maximum number of tokens to output.
 
         Returns:
-        translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+        result (string or list - string or GenerateContentResponse or list - GenerateContentResponse) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of GenerateContentResponse objects if the response type is 'raw' and input was an iterable, a GenerateContentResponse object otherwise.
 
         """
 
-        assert response_type in ["text", "raw", "json"], ValueError("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
-
-        _settings = {
-        "gemini_model": "",
-        "gemini_temperature": "",
-        "gemini_top_p": "",
-        "gemini_top_k": "",
-        "gemini_stop_sequences": "",
-        "gemini_max_output_tokens": ""
-        }
-
-        _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type"]
-        _custom_validation_params = ["gemini_stop_sequences"]
-
-        assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), "text must be a string or an iterable of strings."
+        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
 
-        for _key in _settings.keys():
-            param_name = _key.replace("gemini_", "")
-            if(param_name in locals() and _key not in _non_gemini_params and _key not in _custom_validation_params):
-                _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
+        _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
-        EasyTL.test_api_key_validity("gemini")
-
-        GeminiService._set_decorator(decorator)
+        _validate_stop_sequences(stop_sequences)
 
-        GeminiService._set_json_mode(True if response_type == "json" else False)
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_api_key_validity("gemini")
 
-        translation_instructions = translation_instructions or GeminiService._system_message
+        json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
                                           top_p=top_p,
                                           top_k=top_k,
                                           candidate_count=1,
                                           stream=False,
                                           stop_sequences=stop_sequences,
                                           max_output_tokens=max_output_tokens,
+                                          decorator=decorator,
+                                          logging_directory=logging_directory,
                                           semaphore=None,
-                                          logging_directory=logging_directory)
-
+                                          rate_limit_delay=translation_delay,
+                                          json_mode=json_mode)
+            
+            ## Done afterwards, cause default translation instructions can change based on set_attributes()       
+            GeminiService._system_message = translation_instructions or GeminiService._default_translation_instructions
+        
         if(isinstance(text, str)):
             _result = GeminiService._translate_text(text)
             
-            if(response_type == "text" or response_type == "json"):
-                return _result.text
+            assert not isinstance(_result, list) and hasattr(_result, "text"), EasyTLException("Malformed response received. Please try again.")
             
-            else:
-                return _result
+            result = _result if response_type == "raw" else _result.text
 
         elif(_is_iterable_of_strings(text)):
             
             _results = [GeminiService._translate_text(t) for t in text]
 
-            if(response_type == "text" or response_type == "json"):
-                return [_r.text for _r in _results]
-            
-            else:
-                return _results
+            assert isinstance(_results, list) and all([hasattr(_r, "text") for _r in _results]), EasyTLException("Malformed response received. Please try again.")
+
+            result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
             
-        raise ValueError("text must be a string or an iterable of strings.")
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
         
+        return result
+
 ##-------------------start-of-gemini_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def gemini_translate_async(text:typing.Union[str, typing.Iterable[str]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
-                                    semaphore:int | None = None,
                                     response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                    semaphore:int | None = None,
+                                    translation_delay:float | None = None,
                                     translation_instructions:str | None = None,
                                     model:str="gemini-pro",
                                     temperature:float=0.5,
                                     top_p:float=0.9,
                                     top_k:int=40,
                                     stop_sequences:typing.List[str] | None=None,
                                     max_output_tokens:int | None=None) -> typing.Union[typing.List[str], str, AsyncGenerateContentResponse, typing.List[AsyncGenerateContentResponse]]:
@@ -460,219 +427,202 @@
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
-        It is not known whether Gemini has backoff retrying implemented. (Their API is a mess.)
+        It is not known whether Gemini has backoff retrying implemented. Assume it does not exist.
         
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        semaphore (int) : The number of concurrent requests to make. Default is 15 for 1.0 and 2 for 1.5 gemini models.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a AsyncGenerateContentResponse object, 'json' returns a json-parseable string.
-        translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
+        semaphore (int) : The number of concurrent requests to make. Default is 15 for 1.0 and 2 for 1.5 gemini models. For Gemini, it is recommend to use translation_delay along with the semaphore to prevent rate limiting.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
         stop_sequences (list or None) : The sequences to stop at.
         max_output_tokens (int or None) : The maximum number of tokens to output.
 
         Returns:
-        translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+        result (string or list - string or AsyncGenerateContentResponse or list - AsyncGenerateContentResponse) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of AsyncGenerateContentResponse objects if the response type is 'raw' and input was an iterable, a AsyncGenerateContentResponse object otherwise.
 
         """
 
-        _settings = {
-        "gemini_model": "",
-        "gemini_temperature": "",
-        "gemini_top_p": "",
-        "gemini_top_k": "",
-        "gemini_stop_sequences": "",
-        "gemini_max_output_tokens": ""
-        }
-
-        _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "semaphore", "response_type"]
-        _custom_validation_params = ["gemini_stop_sequences"]
-
-        assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), "stop_sequences must be a string or an iterable of strings."
+        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
 
-        for _key in _settings.keys():
-            param_name = _key.replace("gemini_", "")
-            if(param_name in locals() and _key not in _non_gemini_params and _key not in _custom_validation_params):
-                _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
+        _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
-        EasyTL.test_api_key_validity("gemini")
-
-        GeminiService._set_decorator(decorator)
+        _validate_stop_sequences(stop_sequences)
 
-        GeminiService._set_json_mode(True if response_type == "json" else False)
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_api_key_validity("gemini")
 
-        translation_instructions = translation_instructions or GeminiService._system_message
+        json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
                                           top_p=top_p,
                                           top_k=top_k,
                                           candidate_count=1,
                                           stream=False,
                                           stop_sequences=stop_sequences,
                                           max_output_tokens=max_output_tokens,
+                                          decorator=decorator,
+                                          logging_directory=logging_directory,
                                           semaphore=semaphore,
-                                          logging_directory=logging_directory)
+                                          rate_limit_delay=translation_delay,
+                                          json_mode=json_mode)
+            
+            ## Done afterwards, cause default translation instructions can change based on set_attributes()
+            GeminiService._system_message = translation_instructions or GeminiService._default_translation_instructions
             
         if(isinstance(text, str)):
             _result = await GeminiService._translate_text_async(text)
 
-            if(response_type == "text" or response_type == "json"):
-                return _result.text
-            
-            else:
-                return _result
+            result = _result if response_type == "raw" else _result.text
             
         elif(_is_iterable_of_strings(text)):
             _tasks = [GeminiService._translate_text_async(_t) for _t in text]
-
             _results = await asyncio.gather(*_tasks)
 
-            if(response_type == "text" or response_type == "json"):
-                return [_r.text for _r in _results]
-            
-            else:
-                return _results 
+            result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
 
-        raise ValueError("text must be a string or an iterable of strings.")
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
+        
+        return result
             
 ##-------------------start-of-openai_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def openai_translate(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
                         response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                        translation_delay:float | None = None,
                         translation_instructions:str | SystemTranslationMessage | None = None,
                         model:str="gpt-4",
                         temperature:float=0.3,
                         top_p:float=1.0,
                         stop:typing.List[str] | None=None,
                         max_tokens:int | None=None,
                         presence_penalty:float=0.0,
                         frequency_penalty:float=0.0
                         ) -> typing.Union[typing.List[str], str, typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
-        Translates the given text to the target language using OpenAI.
+        Translates the given text using OpenAI.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
-        OpenAI has it's backoff retrying disabled by EasyTL.
+        OpenAI has it's backoff retrying disabled by EasyTL, in favor of the user implementing their own retrying mechanism via the decorator.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
-        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
-        model (string) : The model to use.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         stop (list or None) : The sequences to stop at.
         max_tokens (int or None) : The maximum number of tokens to output.
         presence_penalty (float) : The presence penalty to use.
         frequency_penalty (float) : The frequency penalty to use.
 
         Returns:
-        translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+        result (string or list - string or ChatCompletion or list - ChatCompletion) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise.
 
         """
 
-        _settings = {
-        "openai_model": "",
-        "openai_temperature": "",
-        "openai_top_p": "",
-        "openai_stop": "",
-        "openai_max_tokens": "",
-        "openai_presence_penalty": "",
-        "openai_frequency_penalty": ""
-        }
-
-        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type"]
-        _custom_validation_params = ["openai_stop"]
-    
-        assert stop is None or isinstance(stop, str) or (hasattr(stop, '__iter__') and all(isinstance(i, str) for i in stop)), "stop must be a string or an iterable of strings."
-
-        for _key in _settings.keys():
-            param_name = _key.replace("openai_", "")
-            if(param_name in locals() and _key not in _non_openai_params and _key not in _custom_validation_params):
-                _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
+        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
 
-        EasyTL.test_api_key_validity("openai")
+        _settings = _return_curated_openai_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "openai")
 
-        OpenAIService._set_decorator(decorator)
+        _validate_stop_sequences(stop)
 
-        OpenAIService._set_json_mode(True if response_type == "json" else False)
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_api_key_validity("openai")
 
+        json_mode = True if response_type == "json" else False
+        
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
                                         top_p=top_p,
                                         n=1,
                                         stop=stop,
                                         max_tokens=max_tokens,
                                         presence_penalty=presence_penalty,
                                         frequency_penalty=frequency_penalty,
+                                        decorator=decorator,
+                                        logging_directory=logging_directory,
                                         semaphore=None,
-                                        logging_directory=logging_directory)
-            
+                                        rate_limit_delay=translation_delay,
+                                        json_mode=json_mode)
+
+            ## Done afterwards, cause default translation instructions can change based on set_attributes()
+            translation_instructions = translation_instructions or OpenAIService._default_translation_instructions
+        
+        else:
+            translation_instructions = OpenAIService._system_message
+
+        assert isinstance(text, str) or _is_iterable_of_strings(text) or isinstance(text, ModelTranslationMessage) or _is_iterable_of_strings(text), InvalidTextInputException("text must be a string, an iterable of strings, a ModelTranslationMessage or an iterable of ModelTranslationMessages.")
+
         translation_batches = OpenAIService._build_translation_batches(text, translation_instructions)
         
         translations = []
-
+        
         for _text, _translation_instructions in translation_batches:
 
             _result = OpenAIService._translate_text(_translation_instructions, _text)
 
-            if(response_type == "text" or response_type == "json"):
-                translation = _result.choices[0].message.content
+            assert not isinstance(_result, list) and hasattr(_result, "choices"), EasyTLException("Malformed response received. Please try again.")
 
-            else:
-                translation = _result
+            translation = _result if response_type == "raw" else _result.choices[0].message.content
             
             translations.append(translation)
         
         ## If originally a single text was provided, return a single translation instead of a list
-        return translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else translations[0]
+        result = translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else translations[0]
         
+        return result
+    
 ##-------------------start-of-openai_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def openai_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
-                                    semaphore:int | None = None,
                                     logging_directory:str | None = None,
                                     response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                    semaphore:int | None = None,
+                                    translation_delay:float | None = None,
                                     translation_instructions:str | SystemTranslationMessage | None = None,
                                     model:str="gpt-4",
                                     temperature:float=0.3,
                                     top_p:float=1.0,
                                     stop:typing.List[str] | None=None,
                                     max_tokens:int | None=None,
                                     presence_penalty:float=0.0,
@@ -692,92 +642,88 @@
 
         OpenAI has it's backoff retrying disabled by EasyTL.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
-        semaphore (int) : The number of concurrent requests to make. Default is 5.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
-        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
+        semaphore (int) : The number of concurrent requests to make. Default is 5.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         stop (list or None) : The sequences to stop at.
         max_tokens (int or None) : The maximum number of tokens to output.
         presence_penalty (float) : The presence penalty to use.
         frequency_penalty (float) : The frequency penalty to use.
 
         Returns:
-        translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
-
+        result (string or list - string or ChatCompletion or list - ChatCompletion) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise.
+        
         """
 
-        _settings = {
-        "openai_model": "",
-        "openai_temperature": "",
-        "openai_top_p": "",
-        "openai_stop": "",
-        "openai_max_tokens": "",
-        "openai_presence_penalty": "",
-        "openai_frequency_penalty": ""
-        }
-
-        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "semaphore", "response_type"]
-        _custom_validation_params = ["openai_stop"]
-
-        assert stop is None or isinstance(stop, str) or (hasattr(stop, '__iter__') and all(isinstance(i, str) for i in stop)), "stop must be a string or an iterable of strings."
+        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
 
-        for _key in _settings.keys():
-            param_name = _key.replace("openai_", "")
-            if(param_name in locals() and _key not in _non_openai_params and _key not in _custom_validation_params):
-                _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
+        _settings = _return_curated_openai_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "openai")
 
-        EasyTL.test_api_key_validity("openai")
+        _validate_stop_sequences(stop)
 
-        OpenAIService._set_decorator(decorator)
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_api_key_validity("openai")
 
-        OpenAIService._set_json_mode(True if response_type == "json" else False)
+        json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
                                         top_p=top_p,
                                         n=1,
                                         stop=stop,
                                         max_tokens=max_tokens,
                                         presence_penalty=presence_penalty,
                                         frequency_penalty=frequency_penalty,
+                                        decorator=decorator,
+                                        logging_directory=logging_directory,
                                         semaphore=semaphore,
-                                        logging_directory=logging_directory)
+                                        rate_limit_delay=translation_delay,
+                                        json_mode=json_mode)
+            
+            ## Done afterwards, cause default translation instructions can change based on set_attributes()
+            translation_instructions = translation_instructions or OpenAIService._default_translation_instructions
+
+        else:
+            translation_instructions = OpenAIService._system_message        
+            
+        assert isinstance(text, str) or _is_iterable_of_strings(text) or isinstance(text, ModelTranslationMessage) or _is_iterable_of_strings(text), InvalidTextInputException("text must be a string, an iterable of strings, a ModelTranslationMessage or an iterable of ModelTranslationMessages.")
 
         _translation_batches = OpenAIService._build_translation_batches(text, translation_instructions)
 
         _translation_tasks = []
 
         for _text, _translation_instructions in _translation_batches:
             _task = OpenAIService._translate_text_async(_translation_instructions, _text)
             _translation_tasks.append(_task)
 
         _results = await asyncio.gather(*_translation_tasks)
 
         _results:typing.List[ChatCompletion] = _results
-        
-        if(response_type == "text" or response_type == "json"):
-            _translations = [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
 
-        elif(response_type == "raw"):
-            _translations = _results
+        assert all([hasattr(_r, "choices") for _r in _results]), EasyTLException("Malformed response received. Please try again.")
+
+        translation = _results if response_type == "raw" else [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
+
+        result = translation if isinstance(text, typing.Iterable) and not isinstance(text, str) else translation[0]
 
-        # If the original input was a single text (not an iterable of texts), return a single translation instead of a list
-        return _translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else _translations[0]
+        return result
     
 ##-------------------start-of-translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def translate(text:str | typing.Iterable[str],
                   service:typing.Optional[typing.Literal["deepl", "openai", "gemini"]] = "deepl", 
                   **kwargs) -> typing.Union[typing.List[str], str,
```

### Comparing `easytl-0.2.0b2/src/easytl/gemini_service.py` & `easytl-0.2.1/src/easytl/gemini_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import google.generativeai as genai
 
 ## custom modules
 from .util import _estimate_cost, _convert_iterable_to_str, _is_iterable_of_strings
 from .decorators import _async_logging_decorator, _sync_logging_decorator
 
 from .classes import GenerationConfig, GenerateContentResponse, AsyncGenerateContentResponse
+from .exceptions import EasyTLException, InvalidTextInputException
 
 class GeminiService:
 
     _default_translation_instructions:str = "Please translate the following text into English."
     _default_model:str = "gemini-pro"
 
     _system_message = _default_translation_instructions
@@ -32,19 +33,21 @@
 
     _client:genai.GenerativeModel
     _generation_config:GenerationConfig
 
     _semaphore_value:int = 15
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
+    _rate_limit_delay:float | None = None
+
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
 
-    ## I don't plan to easily allowing users to change these settings, as I believe that translations should be as accurate as possible, avoiding any censorship or filtering of content.
+    ## Set to prevent any blockage of content
     _safety_settings = [
         {
             "category": "HARM_CATEGORY_DANGEROUS",
             "threshold": "BLOCK_NONE",
         },
         {
             "category": "HARM_CATEGORY_HARASSMENT",
@@ -78,60 +81,31 @@
         Parameters:
         api_key (string) : The API key.
 
         """
 
         genai.configure(api_key=api_key)
 
-##-------------------start-of-_set_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _set_decorator(decorator:typing.Callable | None) -> None:
-
-        """
-
-        Sets the decorator to use for the Gemini service. Should be a callable that returns a decorator or None.
-
-        Parameters:
-        decorator (callable | None) : The decorator to use.
-
-        """
-
-        GeminiService._decorator_to_use = decorator
-
-##-------------------start-of-_set_json_mode()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _set_json_mode(json_mode:bool) -> None:
-
-        """
-
-        Sets the JSON mode for the Gemini service.
-
-        Parameters:
-        json_mode (bool) : True if the service should return JSON responses, False if it should return text responses.
-
-        """
-
-        GeminiService._json_mode = json_mode
-
 ##-------------------start-of-_set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def _set_attributes(model:str="gemini-pro",
-                        system_message:str = _default_translation_instructions,
+                        system_message:str | None = _default_translation_instructions,
                         temperature:float=0.5,
                         top_p:float=0.9,
                         top_k:int=40,
                         candidate_count:int=1,
                         stream:bool=False,
                         stop_sequences:typing.List[str] | None=None,
                         max_output_tokens:int | None=None,
+                        decorator:typing.Union[typing.Callable, None]=None,
+                        logging_directory:str | None=None,
                         semaphore:int | None=None,
-                        logging_directory:str | None=None
+                        rate_limit_delay:float | None=None,
+                        json_mode:bool=False
                         ) -> None:
         
         """
 
         Sets the attributes for the Gemini service.
 
         """
@@ -142,68 +116,68 @@
         GeminiService._top_p = top_p
         GeminiService._top_k = top_k
         GeminiService._candidate_count = candidate_count
         GeminiService._stream = stream
         GeminiService._stop_sequences = stop_sequences
         GeminiService._max_output_tokens = max_output_tokens
 
-        ## if a semaphore is not provided, set it to the default value based on the model
-        if(semaphore is not None):
-            GeminiService._semaphore_value = semaphore
-
-        else:
-            GeminiService._semaphore_value = 15 if GeminiService._model != "gemini-1.5-pro-latest" else 2
+        GeminiService._decorator_to_use = decorator
 
         GeminiService._log_directory = logging_directory
 
-        if(GeminiService._json_mode and GeminiService._model != "gemini-1.5-pro-latest"):
-            GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format."
+        GeminiService._rate_limit_delay = rate_limit_delay
+
+        GeminiService._json_mode = json_mode
+
+        # if a semaphore is not provided, set it to the default value based on the model
+        semaphore_values = {"gemini-1.5-pro-latest": 2}
+        GeminiService._semaphore_value = semaphore or semaphore_values.get(GeminiService._model, 15)
 
+        if(GeminiService._json_mode and GeminiService._model == "gemini-1.5-pro-latest"):
+            GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format. The JSON should be in the following format: {\"text\": \"translated text\"}"
+
+        elif(GeminiService._json_mode):
+            raise EasyTLException("JSON mode for Gemini is only supported for the gemini-1.5-pro-latest model.")
+        
         else:
             GeminiService._default_translation_instructions = "Please translate the following text into English."
         
 ##-------------------start-of-_redefine_client()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _redefine_client() -> None:
 
         """
 
         Redefines the Gemini client and generation config. This should be called before making any requests to the Gemini service, or after changing any of the service's settings.
 
         """
 
-        response_mime_type = "text/plain"
-
-        if(GeminiService._json_mode):
-            response_mime_type = "application/json"
-
+        response_mime_type = "application/json" if GeminiService._json_mode else "text/plain"
+        
         gen_model_params = {
             "model_name": GeminiService._model,
-            "safety_settings": GeminiService._safety_settings
+            "safety_settings": GeminiService._safety_settings,
+            "system_instruction": GeminiService._system_message if GeminiService._model == "gemini-1.5-pro-latest" else None
         }
-
-        ## gemini 1.5 is the only model that supports json responses and system instructions
-        if(GeminiService._model == "gemini-1.5-pro-latest"):
-            gen_model_params["system_instruction"] = GeminiService._system_message
-        else:
-            response_mime_type = "text/plain"
-
+        
         GeminiService._client = genai.GenerativeModel(**gen_model_params)
-
-        GeminiService._generation_config = GenerationConfig(
-            candidate_count=GeminiService._candidate_count,
-            stop_sequences=GeminiService._stop_sequences,
-            max_output_tokens=GeminiService._max_output_tokens,
-            temperature=GeminiService._temperature,
-            top_p=GeminiService._top_p,
-            top_k=GeminiService._top_k,
-            response_mime_type=response_mime_type
-        )
-
+        
+        generation_config_params = {
+            "candidate_count": GeminiService._candidate_count,
+            "stop_sequences": GeminiService._stop_sequences,
+            "max_output_tokens": GeminiService._max_output_tokens,
+            "temperature": GeminiService._temperature,
+            "top_p": GeminiService._top_p,
+            "top_k": GeminiService._top_k,
+            "response_mime_type": response_mime_type
+        }
+        
+        GeminiService._generation_config = GenerationConfig(**generation_config_params)
+        
         GeminiService._semaphore = asyncio.Semaphore(GeminiService._semaphore_value)
 
 ##-------------------start-of-_redefine_client_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _redefine_client_decorator(func):
 
@@ -230,15 +204,15 @@
     @staticmethod
     @_redefine_client_decorator
     @_async_logging_decorator
     async def _translate_text_async(text_to_translate:str) -> AsyncGenerateContentResponse:
 
         """
 
-        Asynchronously translates a text.
+        Asynchronously translates text.
         Instructions default to translating whatever text is input into English.
 
         Parameters:
         text_to_translate (string) : The text to translate.
 
         Returns:
         AsyncGenerateContentResponse : The translation.
@@ -256,15 +230,15 @@
     @staticmethod
     @_redefine_client_decorator
     @_sync_logging_decorator
     def _translate_text(text_to_translate:str) -> GenerateContentResponse:
 
         """
 
-        Synchronously translates a text.
+        Synchronously translates text.
         Instructions default to translating whatever text is input into English.
 
         Parameters:
         text_to_translate (string) : The text to translate.
 
         Returns:
         GenerateContentResponse : The translation.
@@ -320,14 +294,17 @@
         Returns:
         _response (AsyncGenerateContentResponse) : The translation.
 
         """
 
         async with GeminiService._semaphore:
 
+            if(GeminiService._rate_limit_delay is not None):
+                await asyncio.sleep(GeminiService._rate_limit_delay)
+
             text_request = f"{text_to_translate}" if GeminiService._model == "gemini--1.5-pro-latest" else f"{GeminiService._system_message}\n{text_to_translate}"
 
             _response = await GeminiService._client.generate_content_async(
                 contents=text_request,
                 generation_config=GeminiService._generation_config,
                 safety_settings=GeminiService._safety_settings,
                 stream=GeminiService._stream
@@ -365,30 +342,14 @@
 
             return _validity, None
 
         except Exception as _e:
 
             return _validity, _e
         
-##-------------------start-of-_get_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _get_decorator() -> typing.Union[typing.Callable, None]:
-
-        """
-
-        Returns the decorator to use for the Gemini service.
-
-        Returns:
-        decorator (callable) : The decorator to use.
-
-        """
-
-        return GeminiService._decorator_to_use
-    
 ##-------------------start-of-_calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     @_redefine_client_decorator
     def _calculate_cost(text:str | typing.Iterable, translation_instructions:str | None, model:str | None) -> typing.Tuple[int, float, str]:
 
         """
@@ -409,15 +370,15 @@
 
         if(translation_instructions is None):
             translation_instructions = GeminiService._default_translation_instructions
 
         if(isinstance(text, typing.Iterable)):
 
             if(not isinstance(text,str) and not _is_iterable_of_strings(text)):
-                raise ValueError("The text must be a string or an iterable of strings.")
+                raise InvalidTextInputException("The text must be a string or an iterable of strings.")
 
             ## since instructions are paired with the text, we need to repeat the instructions for index
             translation_instructions = translation_instructions * len(text) # type: ignore
 
             text = _convert_iterable_to_str(text)
 
         if(isinstance(translation_instructions, typing.Iterable)):
```

### Comparing `easytl-0.2.0b2/src/easytl/openai_service.py` & `easytl-0.2.1/src/easytl/openai_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ## third-party libraries
 from openai import AsyncOpenAI, OpenAI
 
 ## custom modules
 from .classes import SystemTranslationMessage, ModelTranslationMessage, ChatCompletion
 from .util import _convert_iterable_to_str, _estimate_cost, _is_iterable_of_strings, VALID_JSON_OPENAI_MODELS
 from .decorators import _async_logging_decorator, _sync_logging_decorator
+from .exceptions import EasyTLException
 
 class OpenAIService:
 
     _default_model:str = "gpt-4"
     _default_translation_instructions:SystemTranslationMessage = SystemTranslationMessage("Please translate the following text into English.")
 
     _system_message:typing.Optional[typing.Union[SystemTranslationMessage, str]] = _default_translation_instructions
@@ -34,20 +35,22 @@
 
     _semaphore_value:int = 5
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _sync_client = OpenAI(max_retries=0, api_key="DummyKey")
     _async_client = AsyncOpenAI(max_retries=0, api_key="DummyKey")
 
-    _decorator_to_use:typing.Union[typing.Callable, None] = None
+    _rate_limit_delay:float | None = None
 
-    _json_mode:bool = False
+    _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
 
+    _json_mode:bool = False
+
 ##-------------------start-of-set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
 
         """
 
@@ -57,61 +60,32 @@
         api_key (string) : The API key to set.
 
         """
 
         OpenAIService._async_client.api_key = api_key
         OpenAIService._sync_client.api_key = api_key
 
-##-------------------start-of-set_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _set_decorator(decorator:typing.Callable | None) -> None:
-
-        """
-
-        Sets the decorator to use for the OpenAI service. Should be a callable that returns a decorator or None.
-
-        Parameters:
-        decorator (callable | None) : The decorator to use.
-
-        """
-
-        OpenAIService._decorator_to_use = decorator
-
-##-------------------start-of-set_json_mode()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def _set_json_mode(json_mode:bool) -> None:
-            
-        """
-
-        Sets the JSON mode for the OpenAI service.
-
-        Parameters:
-        json_mode (bool) : True if the JSON mode is to be used, False otherwise.
-
-        """
-
-        OpenAIService._json_mode = json_mode
-
 ##-------------------start-of-set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def _set_attributes(model:str = _default_model,
                         temperature:float = 0.3,
                         logit_bias:typing.Dict[str, int] | None = None,
                         top_p:float = 1.0,
                         n:int = 1,
                         stream:bool = False,
                         stop:typing.List[str] | None = None,
                         max_tokens:int | None = None,
                         presence_penalty:float = 0.0,
                         frequency_penalty:float = 0.0,
-                        semaphore:int | None = None,
-                        logging_directory:str | None = None
+                        decorator:typing.Union[typing.Callable, None]=None,
+                        logging_directory:str | None=None,
+                        semaphore:int | None=None,
+                        rate_limit_delay:float | None=None,
+                        json_mode:bool=False
                         ) -> None:
     
             """
     
             Sets the attributes for the OpenAI service.
     
             """
@@ -123,23 +97,34 @@
             OpenAIService._n = n
             OpenAIService._stream = stream
             OpenAIService._stop = stop
             OpenAIService._max_tokens = max_tokens
             OpenAIService._presence_penalty = presence_penalty
             OpenAIService._frequency_penalty = frequency_penalty
 
+            OpenAIService._decorator_to_use = decorator
+
+            OpenAIService._log_directory = logging_directory
+
+            OpenAIService._rate_limit_delay = rate_limit_delay
+
+            OpenAIService._json_mode = json_mode
+
+            
             if(semaphore is not None):
                 OpenAIService._semaphore_value = semaphore
                 OpenAIService._semaphore = asyncio.Semaphore(OpenAIService._semaphore_value)
 
-            OpenAIService._log_directory = logging_directory
-
             if(OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS):
                 OpenAIService._default_translation_instructions = SystemTranslationMessage("Please translate the following text into English. Make sure to return the translated text in JSON format.")
 
+            elif(OpenAIService._json_mode):
+                model_string = ", ".join(VALID_JSON_OPENAI_MODELS)
+                raise EasyTLException("JSON mode for OpenAI is only available for the following models: " + model_string)
+            
             else:
                 OpenAIService._default_translation_instructions = SystemTranslationMessage("Please translate the following text into English.")
 
 ##-------------------start-of-_build_translation_batches()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _build_translation_batches(text: typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
@@ -301,14 +286,17 @@
 
         """
 
         response_format = "json_object" if OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS else "text"
 
         async with OpenAIService._semaphore:
 
+            if(OpenAIService._rate_limit_delay is not None):
+                await asyncio.sleep(OpenAIService._rate_limit_delay)
+
             response = await OpenAIService._async_client.chat.completions.create(
                 response_format={ "type": response_format },
                 messages=[
                     instruction.to_dict(),
                     prompt.to_dict()
                 ],  # type: ignore
```

### Comparing `easytl-0.2.0b2/src/easytl/util.py` & `easytl-0.2.1/src/easytl/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,77 @@
 import typing
 
 ## third-party libraries
 import tiktoken
 
 ## custom modules
 import google.generativeai as genai
-from .exceptions import InvalidEasyTLSettings
+from .exceptions import InvalidEasyTLSettingsException
+
+##-------------------start-of-_return_curated_gemini_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _return_curated_gemini_settings(local_settings:dict[str, typing.Any]) -> dict:
+
+    _settings = {
+    "gemini_model": "",
+    "gemini_temperature": "",
+    "gemini_top_p": "",
+    "gemini_top_k": "",
+    "gemini_stop_sequences": "",
+    "gemini_max_output_tokens": ""
+    }
+
+    _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type", "semaphore", "translation_delay"]
+    _custom_validation_params = ["gemini_stop_sequences"]
+
+    for _key in _settings.keys():
+        param_name = _key.replace("gemini_", "")
+        if(param_name in local_settings and _key not in _non_gemini_params and _key not in _custom_validation_params):
+            _settings[_key] = _convert_to_correct_type(_key, local_settings[param_name])
+
+    return _settings
+
+##-------------------start-of-_return_curated_openai_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _return_curated_openai_settings(local_settings:dict[str, typing.Any]) -> dict:
+        
+        """
+        
+        Returns the curated OpenAI settings.
+
+        What this does is it takes local_settings from the calling function, and then returns a dictionary with the settings that are relevant to OpenA that were converted to the correct type.
+
+        """
+
+        _settings = {
+        "openai_model": "",
+        "openai_temperature": "",
+        "openai_top_p": "",
+        "openai_stop": "",
+        "openai_max_tokens": "",
+        "openai_presence_penalty": "",
+        "openai_frequency_penalty": ""
+        }
+
+        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type", "semaphore", "translation_delay"]
+        _custom_validation_params = ["openai_stop"]
+
+        for _key in _settings.keys():
+            param_name = _key.replace("openai_", "")
+            if(param_name in local_settings and _key not in _non_openai_params and _key not in _custom_validation_params):
+                _settings[_key] = _convert_to_correct_type(_key, local_settings[param_name])
+
+        return _settings
+
+##-------------------start-of-_return_curated_gemini_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _validate_stop_sequences(stop_sequences:typing.List[str] | None) -> None:
+
+    assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), InvalidEasyTLSettingsException("Invalid stop sequences. Must be a string or a list of strings.")
+
 
 ##-------------------start-of-_string_to_bool()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _string_to_bool(string:str) -> bool:
 
     return string.lower() in ['true', '1', 'yes', 'y', 't']
 
@@ -146,15 +208,15 @@
                 if (_key in settings and not _validate(settings[_key])):
                     raise ValueError(f"Invalid _value for {_key}")
                 
         ##    settings["gemini_stream"] = False
       ##      settings["gemini_candidate_count"] = 1
         
     except Exception as e:
-        raise InvalidEasyTLSettings(f"Invalid settings, Due to: {str(e)}")
+        raise InvalidEasyTLSettingsException(f"Invalid settings, Due to: {str(e)}")
 
 ##-------------------start-of-_convert_to_correct_type()-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _convert_to_correct_type(setting_name:str, initial_value:str) -> typing.Any:
 
     """
```

### Comparing `easytl-0.2.0b2/src/easytl.egg-info/PKG-INFO` & `easytl-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.2.0b2
-Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
+Version: 0.2.1
+Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, and Gemini.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -20,114 +20,124 @@
 Requires-Dist: tiktoken==0.6.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
+- [Features](#features)
+- [API Usage](#api-usage)
 - [License](#license)
 - [Contact](#contact)
 - [Contribution](#contribution)
 - [Notes](#notes)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
 Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 
-EasyTL has a trello board:
+EasyTL has a Trello board for tracking features and issues:
 https://trello.com/b/Td555CoW/easytl
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
-Then, you can translate Japanese text using DeepL by importing the global client.
+Then, you can translate Japanese text using by importing the global client.
+
+For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
-## set your api key
+## Set your API key
 EasyTL.set_api_key("deepL", "your_api_key_here")
 
-## you can also validate your api keys, translation functions will do this automatically
+## You can also validate your API keys; translation functions will do this automatically
 is_valid, e = EasyTL.validate_api_key("deepL")
 
 translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality.
-
-## easytl also has a generic translate method, which defaults to deepl, requires text, and kwargs for the translate method it uses.
-
-translated_text = EasyTL.translate("私は日本語が話せます", target_lang="EN")
-
-## There is also a calculate cost method.
-## for deepl, model is deepl
-num_characters, cost, model = EasyTL.calculate_cost("私は日本語が話せます", "deepL") ## Text to translate, service to use
-
-## or for llms
-## last 2 arguments are optional, defaults to gpt-4 and "Translate to English"
-num_tokens, cost, model = EasyTL.calculate_cost("私は日本語が話せます", "openai", "gpt-4", "Translate to English") ## Text to translate, service to use, model to use, prompt to use
-
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
 Python 3.10+
 
 EasyTL can be installed using pip:
 
-
 ```bash
 pip install easytl
 ```
 
 This will install EasyTL along with its dependencies and requirements.
 
 These are the dependencies/requirements that will be installed:
 ```
 setuptools>=61.0
-
 wheel
-
 setuptools_scm>=6.0
-
 tomli
-
 google-generativeai==0.5.1
-
 deepl==1.16.1
-
 openai==1.13.3
-
 backoff==2.2.1
-
 tiktoken==0.6.0
+```
+---------------------------------------------------------------------------------------------------------------------------------------------------
+
+**Features**<a name="features"></a>
 
+EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
+
+- Support for multiple translation APIs including OpenAI, DeepL, and Gemini.
+- Simple API key management.
+- Methods to validate API keys before usage.
+- Cost estimation tools to help manage usage based on text length and service.
+- Highly customizable translation options, with the API's original features.
+- Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
+
+---------------------------------------------------------------------------------------------------------------------------------------------------
+
+**API Usage**<a name="api-usage"></a>
+
+### Translating Text
+
+Use `deepl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+
+### Cost Calculation
+
+The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
+
+characters or tokens depending on the service.
+
+```python
+num_characters, cost, model = EasyTL.calculate_cost("Example text.", "deepL")
 ```
+
+### API Key Management
+
+API keys can be set and validated using `set_api_key` and `validate_api_key` methods to ensure they are active and correct before submitting translation requests.
+
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
-Under the LGPLv2.1, any modifications made to EasyTL's libraries must be shared under the same license, ensuring the open source nature of the library itself is maintained. However, it allows the wider work that includes the library to remain under different licensing terms, provided the terms of the LGPLv2.1 are met for the library.
-
-I encourage the use of EasyTL within all projects. This approach ensures a balance between open collaboration and the flexibility required for proprietary development.
-
-For a thorough explanation of the conditions and how they may apply to your use of the project, please review the full license text. This comprehensive documentation will offer guidance on your rights and obligations when utilizing LGPLv2.1 licensed software.
-
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
 If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
```

### Comparing `easytl-0.2.0b2/src/easytl.egg-info/SOURCES.txt` & `easytl-0.2.1/src/easytl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/tests/issue_template.py` & `easytl-0.2.1/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b2/tests/passing.py` & `easytl-0.2.1/tests/passing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from easytl import EasyTL
 
 import asyncio
 import os
 import time
 
+##-------------------start-of-read_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
 def read_api_key(filename):
     try:
         with open(filename, 'r') as file:
             return file.read().strip()
         
     except:
         pass
 
-async def main():
+def setup_preconditions():
+
 
     gemini_time_delay = 30
 
     deepl_api_key = os.environ.get('DEEPL_API_KEY')
     gemini_api_key = os.environ.get('GEMINI_API_KEY')
     openai_api_key = os.environ.get('OPENAI_API_KEY')
 
@@ -26,101 +29,129 @@
         deepl_api_key = read_api_key("tests/deepl.txt")
     if(gemini_api_key is None):
         gemini_api_key = read_api_key("tests/gemini.txt")
     if(openai_api_key is None):
         openai_api_key = read_api_key("tests/openai.txt")
         
         logging_directory = "tests/"
+        gemini_time_delay = 5
 
     assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
     assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
     assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
 
     EasyTL.set_api_key("deepl", deepl_api_key)
     EasyTL.set_api_key("gemini", gemini_api_key)
     EasyTL.set_api_key("openai", openai_api_key)
 
-    print("Deepl ------------------------------------------------")
+    return gemini_time_delay, logging_directory
+
+##-------------------start-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+async def main():
+
+    gemini_time_delay, logging_directory = setup_preconditions()
+
+    print("------------------------------------------------Deepl------------------------------------------------")
 
-    print("Text response")
+    print("------------------------------------------------Text response------------------------------------------------")
 
     print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", logging_directory=logging_directory))
     print(await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", logging_directory=logging_directory))
     
     print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory).text) # type: ignore
     result = await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory)
 
     print(result.text) # type: ignore
 
-    print("Raw response")
+    print("------------------------------------------------Raw response------------------------------------------------")
 
     results = EasyTL.deepl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory)
     async_results = await EasyTL.deepl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory)
 
     for result in results: # type: ignore
         print(result.text) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.text)
 
-    print("Gemini ------------------------------------------------")
+    print("------------------------------------------------Cost calculation------------------------------------------------")
+
+    characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="deepl", model=None, translation_instructions=None)
+
+    print(f"Characters: {characters}, Cost: {cost}, Model: {model}")
 
-    print("Text response")
+    print("------------------------------------------------Gemini------------------------------------------------")
+
+    print("-----------------------------------------------Text response-----------------------------------------------")
 
     print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory))
     print(await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory))
 
     print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory).text) # type: ignore
     result = await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
 
     print(result.text) # type: ignore
 
-    print("Raw response")
+    print("-----------------------------------------------Raw response-----------------------------------------------")
 
     results = EasyTL.gemini_translate(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
-    async_results = await EasyTL.gemini_translate_async(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
+    async_results = await EasyTL.gemini_translate_async(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory, translation_delay=5)
 
     for result in results: # type: ignore
         print(result.text) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.text)
 
-    print("JSON response")
+    print("-----------------------------------------------JSON response-----------------------------------------------")
 
     print(EasyTL.gemini_translate("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Translate this to German. Format the response as JSON.", response_type="json", logging_directory=logging_directory))
     
     time.sleep(gemini_time_delay)
     
     print(await EasyTL.gemini_translate_async("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory))
-    
 
-    print("OpenAI ------------------------------------------------")
+    print("------------------------------------------------Cost calculation------------------------------------------------")
+
+    tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="gemini", model="gemini-pro", translation_instructions="Translate this to German.")
+
+    print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
+
+    print("------------------------------------------------OpenAI------------------------------------------------")
 
-    print("Text response")
+    print("-----------------------------------------------Text response-----------------------------------------------")
 
     print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory))
     print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory))
 
     print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory).choices[0].message.content) # type: ignore
     result = await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
 
     print(result.choices[0].message.content) # type: ignore
 
-    print("Raw response")
+    print("-----------------------------------------------Raw response-----------------------------------------------")
 
     results = EasyTL.openai_translate(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
     async_results = await EasyTL.openai_translate_async(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
 
     for result in results: # type: ignore
         print(result.choices[0].message.content) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.choices[0].message.content ) # type: ignore
 
-    print("JSON response")
+    print("-----------------------------------------------JSON response-----------------------------------------------")
 
     print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German. Format the response as JSON parseable string.", response_type="json", logging_directory=logging_directory))
     print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German. Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory))
 
+    print("------------------------------------------------Cost calculation------------------------------------------------")
+
+    tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="openai", model="gpt-3.5-turbo", translation_instructions="Translate this to German.")
+
+    print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
+
+##-------------------end-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
 if(__name__ == "__main__"):
     asyncio.run(main())
```

