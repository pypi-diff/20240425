# Comparing `tmp/timelength-2.0.1.tar.gz` & `tmp/timelength-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelength-2.0.1.tar", max compression
+gzip compressed data, was "timelength-2.0.2.tar", max compression
```

## Comparing `timelength-2.0.1.tar` & `timelength-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1082 2024-01-19 07:44:29.030225 timelength-2.0.1/LICENSE
--rw-r--r--   0        0        0      983 2024-04-05 00:58:04.282919 timelength-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5485 2024-04-04 23:50:53.149033 timelength-2.0.1/README.md
--rw-r--r--   0        0        0      176 2024-04-04 23:50:53.152033 timelength-2.0.1/timelength/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-04 23:50:53.153032 timelength-2.0.1/timelength/dataclasses.py
--rw-r--r--   0        0        0      919 2024-04-04 23:50:53.154032 timelength-2.0.1/timelength/enums.py
--rw-r--r--   0        0        0      406 2024-04-04 23:50:53.155032 timelength-2.0.1/timelength/errors.py
--rw-r--r--   0        0        0     9721 2024-04-04 23:50:53.156033 timelength-2.0.1/timelength/locales/english.json
--rw-r--r--   0        0        0    12417 2024-04-05 02:05:38.194008 timelength-2.0.1/timelength/locales/spanish.json
--rw-r--r--   0        0        0     8406 2024-04-04 23:50:53.155032 timelength-2.0.1/timelength/locales.py
--rw-r--r--   0        0        0    17248 2024-04-05 02:05:48.024835 timelength-2.0.1/timelength/parsers/parser_one.py
--rw-r--r--   0        0        0     8749 2024-04-05 00:57:48.478450 timelength-2.0.1/timelength/timelength.py
--rw-r--r--   0        0        0     1296 2024-04-04 23:50:53.159032 timelength-2.0.1/timelength/utils.py
--rw-r--r--   0        0        0     6137 1970-01-01 00:00:00.000000 timelength-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-25 11:57:51.204519 timelength-2.0.2/LICENSE
+-rw-r--r--   0        0        0     5563 2024-04-25 11:57:51.204519 timelength-2.0.2/README.md
+-rw-r--r--   0        0        0     1023 2024-04-25 11:57:51.204519 timelength-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      172 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/__init__.py
+-rw-r--r--   0        0        0     2235 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/dataclasses.py
+-rw-r--r--   0        0        0      884 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/enums.py
+-rw-r--r--   0        0        0      392 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/errors.py
+-rw-r--r--   0        0        0     9457 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/locales/english.json
+-rw-r--r--   0        0        0    12113 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/locales/spanish.json
+-rw-r--r--   0        0        0     8170 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/locales.py
+-rw-r--r--   0        0        0    16803 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/parsers/parser_one.py
+-rw-r--r--   0        0        0     8755 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/timelength.py
+-rw-r--r--   0        0        0     1254 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/utils.py
+-rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 timelength-2.0.2/PKG-INFO
```

### Comparing `timelength-2.0.1/LICENSE` & `timelength-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timelength-2.0.1/pyproject.toml` & `timelength-2.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-[tool.poetry]
-name = "timelength"
-version = "2.0.1"
-description = "A Python package to parse human readable lengths of time."
-authors = ["Etorix <admin@etorix.dev>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://pypi.org/project/timelength/"
-repository = "https://github.com/EtorixDev/timelength/"
-keywords = ["timelength", "duration", "python", "parsing", "time"]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-]
-include = ["timelength/locales/*.json"]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.3.5"
-pytest = "^8.1.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "timelength"
+version = "2.0.2"
+description = "A Python package to parse human readable lengths of time."
+authors = ["Etorix <admin@etorix.dev>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://pypi.org/project/timelength/"
+repository = "https://github.com/EtorixDev/timelength/"
+keywords = ["timelength", "duration", "python", "parsing", "time"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+include = ["timelength/locales/*.json"]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.3.5"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+tox = "^4.14.2"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+exclude = ["tests"]
```

### Comparing `timelength-2.0.1/README.md` & `timelength-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 ## Usage (English)
 ### Default
 While `TimeLength.strict` is `False` (default), `TimeLength.result.success` will be `True` if at least one valid result is found, regardless of invalid results.
 ```python
 from timelength import TimeLength
 
-output = TimeLength("1d5h25m and 23miles")
+output = TimeLength("1d5h25m15.5s and 23miles")
 print(output.result.success)
 # True
 print(output.result.seconds)
-# 105900.0
+# 105915.5
 print(output.to_minutes(max_precision = 3))
-# 1765.0
+# 1765.258
 print(output.result.invalid)
 # [('miles', 'UNKNOWN_TERM'), (23.0, 'LONELY_VALUE')]
 print(output.result.valid)
-# [(1.0, Scale(86400.0, "day", "days")), (5.0, Scale(3600.0, "hour", "hours")), (25.0, Scale(60.0, "minute", "minutes"))]
+# [(1.0, Scale(86400.0, "day", "days")), (5.0, Scale(3600.0, "hour", "hours")), (25.0, Scale(60.0, "minute", "minutes")), (15.5, Scale(1.0, "second", "seconds"))]
 ```
 Additionally, if a single lone value is parsed without a paired scale, seconds will be assumed. However, if more than one value is parsed, nothing will be assumed.
 ```python
 output = TimeLength("45")
 print(output.result.invalid)
 # []
 print(output.result.valid)
@@ -50,42 +50,42 @@
 
 output = TimeLength("3.5d, 35m, 19", strict = True)
 print(output.result.success)
 # False
 print(output.result.invalid)
 # [(19.0, "LONELY_VALUE")]
 print(output.result.valid)
-# [(3.5, Scale(scale=86400.0, "day", "days")), (35.0, Scale(scale=60.0, "minute", "minutes"))]
+# [(3.5, Scale(86400.0, "day", "days")), (35.0, Scale(60.0, "minute", "minutes"))]
 ```
 Additionally, unlike with the default behavior, scales must be present. No assumptions will be made.
 
 ## Supported Locales
 1. English
 2. Spanish
-3. Custom (Copy & modify an existing config with new terms as long as your new `Locale` follows the existing config parser's grammar structure)
-4. Custom (Write your own parsing logic if your `Locale`'s grammar structure differs too drastically) (PRs welcome)
+3. Basic Custom (Copy & modify an existing config with new terms as long as your new `Locale` follows the existing config parser's grammar structure)
+4. Advanced Custom (Write your own parsing logic if your `Locale`'s grammar structure differs too drastically) (PRs welcome)
 
 ## Customization
 `timelength` allows for customizing the parsing behavior through JSON configuration. To get started, copy an existing locale JSON in `timelength/locales/`. The custom JSON may be placed anywhere.
 
 **Ensure the JSON being used is from a trusted source, as the parser is loaded dynamically based on the file specified in the JSON. This could allow for unintended code execution if an unsafe config is loaded.**
 
 Valid JSONs must include the following keys, even if their contents are empty: 
 - `connectors`
   - Characters/phrases that join two parts of the same segment.
 - `segmentors`
   - Characters/phrases that join two segments together.
-- `allowed_symbols`
-  - Characters that won't be categorized as an invalid input. If sent multiple times in a row (ex: !!), they will still be marked as invalid.
+- `allowed_terms`
+  - Characters or terms that won't be categorized as an invalid input. If sent multiple times in a row (ex: !!), they will still be marked as invalid.
 - `decimal_separators`
   - Characters used to separate decimals from digits. Can't have overlap with `thousand_separators`.
 - `thousand_separators`
   - Characters used to break up large numbers. Can't have overlap with `decimal_separators`.
 - `parser_file`
-  - The name of this locale's parser file located in `timelength/parsers/`, or the path to the parser file if stored elsewhere. 
+  - The name of this locale's parser file (extension included) located in `timelength/parsers/`, or the path to the parser file if stored elsewhere. 
   - **Ensure only a trusted file is used as this could allow unintended code execution.**
   - The internal parser method must share a name with the file.
 - `numerals`
   - Word forms of numbers. May be populated or left empty. Each element must itself have the following keys, even if their contents are not used:
     - `type`
       - The numeral type.
     - `value`
@@ -99,15 +99,15 @@
     - singular
       - The lowercase singular form of this scale.
     - plural
       - The lowercase plural form of this scale.
     - terms
       - All terms that could be parsed as this scale. Accents and other NFKD markings should not be present as they are filtered from the user input.
 - `extra_data`
-  - Any data a parser needs that is not already covered. May be populated or left empty. The locale loads this into a `Locale._extra_data` attribute, leaving the parser to utilizes it.
+  - Any data a parser needs that is not already covered. May be populated or left empty. The locale loads this into a `Locale._extra_data` attribute, leaving the parser to utilize it.
 
 Once your custom JSON is filled out, you can use it as follows:
 ```python
 from timelength import TimeLength, CustomLocale
 
 output = TimeLength("30 minutes", locale = CustomLocale("path/to/config.json"))
 ```
```

### Comparing `timelength-2.0.1/timelength/dataclasses.py` & `timelength-2.0.2/timelength/dataclasses.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from dataclasses import dataclass, field
-
-
-@dataclass
-class ParsedTimeLength:
-    """
-    Represents the outcome of parsing a length of time from a string.
-
-    ### Attributes
-
-    - `success` (`bool`): Indicates if the parsing was successful.
-    - `seconds` (`float`): The total length of time parsed, in seconds.
-    - `invalid` (`list`): A list of parts of the input string that could not be parsed as valid time.
-    - `valid` (`list`): A list of parts of the input string that were successfully parsed as valid time.
-
-    ### Methods
-
-    - `__str__`: Return a string indicating the success or failure of the parsing.
-    - `__repr__`: Return a string representation of the `ParsedTimeLength` with attributes included.
-    """
-
-    success: bool = False
-    seconds: float = 0.0
-    invalid: list = field(default_factory=list)
-    valid: list = field(default_factory=list)
-
-    def __str__(self):
-        """Return a string indicating the success or failure of the parsing."""
-        return "Success" if self.success else "Failure"
-
-    def __repr__(self):
-        """Return a string representation of the `ParsedTimeLength` with attributes included."""
-        return f"ParsedTimeLength({self.success}, {self.seconds}, {self.invalid}, {self.valid})"
-
-
-@dataclass
-class Scale:
-    """
-    Represents a scale for converting units of time.
-
-    ### Attributes
-
-    - `scale` (`float`): Approximately how many seconds this `Scale` is equivalent to.
-    - `singular` (`str`): The singular form of the `Scale`'s name.
-    - `plural` (`str`): The plural form of the `Scale`'s name.
-    - `terms` (`list`): A list of abbreviations associated with the `Scale`.
-
-    ### Methods
-
-    - `__str__`: Returns the singular form of the Scale.
-    - `__repr__`: Returns a string representation of the Scale with attributes included.
-    """
-
-    scale: float = 0.0
-    singular: str = ""
-    plural: str = ""
-    terms: list = field(default_factory=list)
-
-    def __str__(self):
-        """Return the singular form of the Scale."""
-        return self.singular
-
-    def __repr__(self):
-        """Return a string representation of the Scale with attributes included."""
-        return f'Scale({self.scale}, "{self.singular}", "{self.plural}")'
+from dataclasses import dataclass, field
+
+
+@dataclass
+class ParsedTimeLength:
+    """
+    Represents the outcome of parsing a length of time from a string.
+
+    ### Attributes
+
+    - `success` (`bool`): Indicates if the parsing was successful.
+    - `seconds` (`float`): The total length of time parsed, in seconds.
+    - `invalid` (`list`): A list of parts of the input string that could not be parsed as valid time.
+    - `valid` (`list`): A list of parts of the input string that were successfully parsed as valid time.
+
+    ### Methods
+
+    - `__str__`: Return a string indicating the success or failure of the parsing.
+    - `__repr__`: Return a string representation of the `ParsedTimeLength` with attributes included.
+    """
+
+    success: bool = False
+    seconds: float = 0.0
+    invalid: list = field(default_factory=list)
+    valid: list = field(default_factory=list)
+
+    def __str__(self):
+        """Return a string indicating the success or failure of the parsing."""
+        return "Success" if self.success else "Failure"
+
+    def __repr__(self):
+        """Return a string representation of the `ParsedTimeLength` with attributes included."""
+        return f"ParsedTimeLength({self.success}, {self.seconds}, {self.invalid}, {self.valid})"
+
+
+@dataclass
+class Scale:
+    """
+    Represents a scale for converting units of time.
+
+    ### Attributes
+
+    - `scale` (`float`): Approximately how many seconds this `Scale` is equivalent to.
+    - `singular` (`str`): The singular form of the `Scale`'s name.
+    - `plural` (`str`): The plural form of the `Scale`'s name.
+    - `terms` (`list`): A list of abbreviations associated with the `Scale`.
+
+    ### Methods
+
+    - `__str__`: Returns the singular form of the Scale.
+    - `__repr__`: Returns a string representation of the Scale with attributes included.
+    """
+
+    scale: float = 0.0
+    singular: str = ""
+    plural: str = ""
+    terms: list = field(default_factory=list)
+
+    def __str__(self):
+        """Return the singular form of the Scale."""
+        return self.singular
+
+    def __repr__(self):
+        """Return a string representation of the Scale with attributes included."""
+        return f'Scale({self.scale}, "{self.singular}", "{self.plural}")'
```

### Comparing `timelength-2.0.1/timelength/enums.py` & `timelength-2.0.2/timelength/enums.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from enum import Enum
-
-
-class CharacterType(Enum):
-    """
-    Enumerates the types of characters recognized during parsing.
-
-    ### Members
-    - `NUMBER`: Represents number characters.
-    - `ALPHABET`: Represents alphabetic characters.
-    - `SPECIAL`: Represents special characters (ex: !).
-    """
-
-    NUMBER = "NUMBER"
-    ALPHABET = "ALPHABET"
-    SPECIAL = "SPECIAL"
-
-
-class BufferType(Enum):
-    """
-    Enumerates the types of buffers recognized during parsing.
-
-    ### Members
-    - `NUMBER`: Represents number strings.
-    - `SCALE`: Represents scale strings (ex: minutes).
-    - `NUMERAL`: Represents numeral strings (ex: twenty).
-    - `SPECIAL`: Represents special strings (ex: !$^).
-    - `UNKNOWN`: Represents other uncategorizable strings.
-    """
-
-    NUMBER = "NUMBER"
-    SCALE = "SCALE"
-    NUMERAL = "NUMERAL"
-    SPECIAL = "SPECIAL"
-    UNKNOWN = "UNKNOWN"
+from enum import Enum
+
+
+class CharacterType(Enum):
+    """
+    Enumerates the types of characters recognized during parsing.
+
+    ### Members
+    - `NUMBER`: Represents number characters.
+    - `ALPHABET`: Represents alphabetic characters.
+    - `SPECIAL`: Represents special characters (ex: !).
+    """
+
+    NUMBER = "NUMBER"
+    ALPHABET = "ALPHABET"
+    SPECIAL = "SPECIAL"
+
+
+class BufferType(Enum):
+    """
+    Enumerates the types of buffers recognized during parsing.
+
+    ### Members
+    - `NUMBER`: Represents number strings.
+    - `SCALE`: Represents scale strings (ex: minutes).
+    - `NUMERAL`: Represents numeral strings (ex: twenty).
+    - `SPECIAL`: Represents special strings (ex: !$^).
+    - `UNKNOWN`: Represents other uncategorizable strings.
+    """
+
+    NUMBER = "NUMBER"
+    SCALE = "SCALE"
+    NUMERAL = "NUMERAL"
+    SPECIAL = "SPECIAL"
+    UNKNOWN = "UNKNOWN"
```

### Comparing `timelength-2.0.1/timelength/locales/english.json` & `timelength-2.0.2/timelength/locales/english.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 23% similar despite different names*

```diff
@@ -1,608 +1,592 @@
-00000000: 7b0d 0a20 2020 2022 636f 6e6e 6563 746f  {..    "connecto
-00000010: 7273 223a 205b 2220 222c 2022 5c74 222c  rs": [" ", "\t",
-00000020: 2022 2d22 5d2c 0d0a 2020 2020 2273 6567   "-"],..    "seg
-00000030: 6d65 6e74 6f72 7322 3a20 5b22 2c22 2c20  mentors": [",", 
-00000040: 2261 6e64 222c 2022 2622 5d2c 0d0a 2020  "and", "&"],..  
-00000050: 2020 2261 6c6c 6f77 6564 5f74 6572 6d73    "allowed_terms
-00000060: 223a 205b 2221 222c 2022 3f22 2c20 2227  ": ["!", "?", "'
-00000070: 222c 2022 2e22 2c20 222c 222c 2022 7468  ", ".", ",", "th
-00000080: 6522 5d2c 0d0a 2020 2020 2264 6563 696d  e"],..    "decim
-00000090: 616c 5f73 6570 6172 6174 6f72 7322 3a20  al_separators": 
-000000a0: 5b22 2e22 5d2c 0d0a 2020 2020 2274 686f  ["."],..    "tho
-000000b0: 7573 616e 645f 7365 7061 7261 746f 7273  usand_separators
-000000c0: 223a 205b 222c 222c 2022 2022 5d2c 0d0a  ": [",", " "],..
-000000d0: 2020 2020 2270 6172 7365 725f 6669 6c65      "parser_file
-000000e0: 223a 2022 7061 7273 6572 5f6f 6e65 2e70  ": "parser_one.p
-000000f0: 7922 2c0d 0a20 2020 2022 6e75 6d65 7261  y",..    "numera
-00000100: 6c73 223a 207b 0d0a 2020 2020 2020 2020  ls": {..        
-00000110: 227a 6572 6f22 3a20 7b0d 0a20 2020 2020  "zero": {..     
-00000120: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000130: 6469 6769 7473 222c 0d0a 2020 2020 2020  digits",..      
-00000140: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
-00000150: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000160: 2022 7465 726d 7322 3a20 5b22 7a65 726f   "terms": ["zero
-00000170: 222c 2022 5a65 726f 222c 2022 5a45 524f  ", "Zero", "ZERO
-00000180: 222c 2022 7a65 726f 6573 222c 2022 5a65  ", "zeroes", "Ze
-00000190: 726f 6573 222c 2022 5a45 524f 4553 222c  roes", "ZEROES",
-000001a0: 2022 7a65 726f 7322 2c20 225a 6572 6f73   "zeros", "Zeros
-000001b0: 222c 2022 5a45 524f 5322 5d0d 0a20 2020  ", "ZEROS"]..   
-000001c0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-000001d0: 2022 6f6e 6522 3a20 7b0d 0a20 2020 2020   "one": {..     
-000001e0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000001f0: 6469 6769 7473 222c 0d0a 2020 2020 2020  digits",..      
-00000200: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
-00000210: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000220: 2022 7465 726d 7322 3a20 5b22 6f6e 6522   "terms": ["one"
-00000230: 2c20 224f 6e65 222c 2022 4f4e 4522 2c20  , "One", "ONE", 
-00000240: 226f 6e65 7322 2c20 224f 6e65 7322 2c20  "ones", "Ones", 
-00000250: 224f 4e45 5322 2c20 2261 222c 2022 4122  "ONES", "a", "A"
-00000260: 2c20 2261 6e22 2c20 2241 6e22 2c20 2241  , "an", "An", "A
-00000270: 4e22 5d0d 0a20 2020 2020 2020 207d 2c0d  N"]..        },.
-00000280: 0a20 2020 2020 2020 2022 7477 6f22 3a20  .        "two": 
-00000290: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-000002a0: 7479 7065 223a 2022 6469 6769 7473 222c  type": "digits",
-000002b0: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-000002c0: 616c 7565 223a 2032 2e30 2c0d 0a20 2020  alue": 2.0,..   
-000002d0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-000002e0: 3a20 5b22 7477 6f22 2c20 2254 776f 222c  : ["two", "Two",
-000002f0: 2022 5457 4f22 2c20 2274 776f 7322 2c20   "TWO", "twos", 
-00000300: 2254 776f 7322 2c20 2254 574f 5322 5d0d  "Twos", "TWOS"].
-00000310: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00000320: 2020 2020 2022 7468 7265 6522 3a20 7b0d       "three": {.
-00000330: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00000340: 7065 223a 2022 6469 6769 7473 222c 0d0a  pe": "digits",..
-00000350: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00000360: 7565 223a 2033 2e30 2c0d 0a20 2020 2020  ue": 3.0,..     
-00000370: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
-00000380: 5b22 7468 7265 6522 2c20 2254 6872 6565  ["three", "Three
-00000390: 222c 2022 5448 5245 4522 2c20 2274 6872  ", "THREE", "thr
-000003a0: 6565 7322 2c20 2254 6872 6565 7322 2c20  ees", "Threes", 
-000003b0: 2254 4852 4545 5322 5d0d 0a20 2020 2020  "THREES"]..     
-000003c0: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-000003d0: 666f 7572 223a 207b 0d0a 2020 2020 2020  four": {..      
-000003e0: 2020 2020 2020 2274 7970 6522 3a20 2264        "type": "d
-000003f0: 6967 6974 7322 2c0d 0a20 2020 2020 2020  igits",..       
-00000400: 2020 2020 2022 7661 6c75 6522 3a20 342e       "value": 4.
-00000410: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00000420: 2274 6572 6d73 223a 205b 2266 6f75 7222  "terms": ["four"
-00000430: 2c20 2246 6f75 7222 2c20 2246 4f55 5222  , "Four", "FOUR"
-00000440: 2c20 2266 6f75 7273 222c 2022 466f 7572  , "fours", "Four
-00000450: 7322 2c20 2246 4f55 5253 225d 0d0a 2020  s", "FOURS"]..  
-00000460: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000470: 2020 2266 6976 6522 3a20 7b0d 0a20 2020    "five": {..   
-00000480: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000490: 2022 6469 6769 7473 222c 0d0a 2020 2020   "digits",..    
-000004a0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-000004b0: 2035 2e30 2c0d 0a20 2020 2020 2020 2020   5.0,..         
-000004c0: 2020 2022 7465 726d 7322 3a20 5b22 6669     "terms": ["fi
-000004d0: 7665 222c 2022 4669 7665 222c 2022 4649  ve", "Five", "FI
-000004e0: 5645 222c 2022 6669 7665 7322 2c20 2246  VE", "fives", "F
-000004f0: 6976 6573 222c 2022 4649 5645 5322 5d0d  ives", "FIVES"].
-00000500: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00000510: 2020 2020 2022 7369 7822 3a20 7b0d 0a20       "six": {.. 
-00000520: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000530: 223a 2022 6469 6769 7473 222c 0d0a 2020  ": "digits",..  
-00000540: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00000550: 223a 2036 2e30 2c0d 0a20 2020 2020 2020  ": 6.0,..       
-00000560: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-00000570: 7369 7822 2c20 2253 6978 222c 2022 5349  six", "Six", "SI
-00000580: 5822 2c20 2273 6978 6573 222c 2022 5369  X", "sixes", "Si
-00000590: 7865 7322 2c20 2253 4958 4553 225d 0d0a  xes", "SIXES"]..
-000005a0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000005b0: 2020 2020 2273 6576 656e 223a 207b 0d0a      "seven": {..
-000005c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000005d0: 6522 3a20 2264 6967 6974 7322 2c0d 0a20  e": "digits",.. 
-000005e0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-000005f0: 6522 3a20 372e 302c 0d0a 2020 2020 2020  e": 7.0,..      
-00000600: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00000610: 2273 6576 656e 222c 2022 5365 7665 6e22  "seven", "Seven"
-00000620: 2c20 2253 4556 454e 222c 2022 7365 7665  , "SEVEN", "seve
-00000630: 6e73 222c 2022 5365 7665 6e73 222c 2022  ns", "Sevens", "
-00000640: 5345 5645 4e53 225d 0d0a 2020 2020 2020  SEVENS"]..      
-00000650: 2020 7d2c 0d0a 2020 2020 2020 2020 2265    },..        "e
-00000660: 6967 6874 223a 207b 0d0a 2020 2020 2020  ight": {..      
-00000670: 2020 2020 2020 2274 7970 6522 3a20 2264        "type": "d
-00000680: 6967 6974 7322 2c0d 0a20 2020 2020 2020  igits",..       
-00000690: 2020 2020 2022 7661 6c75 6522 3a20 382e       "value": 8.
-000006a0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-000006b0: 2274 6572 6d73 223a 205b 2265 6967 6874  "terms": ["eight
-000006c0: 222c 2022 4569 6768 7422 2c20 2245 4947  ", "Eight", "EIG
-000006d0: 4854 222c 2022 6569 6768 7473 222c 2022  HT", "eights", "
-000006e0: 4569 6768 7473 222c 2022 4549 4748 5453  Eights", "EIGHTS
-000006f0: 225d 0d0a 2020 2020 2020 2020 7d2c 0d0a  "]..        },..
-00000700: 2020 2020 2020 2020 226e 696e 6522 3a20          "nine": 
-00000710: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00000720: 7479 7065 223a 2022 6469 6769 7473 222c  type": "digits",
-00000730: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00000740: 616c 7565 223a 2039 2e30 2c0d 0a20 2020  alue": 9.0,..   
-00000750: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-00000760: 3a20 5b22 6e69 6e65 222c 2022 4e69 6e65  : ["nine", "Nine
-00000770: 222c 2022 4e49 4e45 222c 2022 6e69 6e65  ", "NINE", "nine
-00000780: 7322 2c20 224e 696e 6573 222c 2022 4e49  s", "Nines", "NI
-00000790: 4e45 5322 5d0d 0a20 2020 2020 2020 207d  NES"]..        }
-000007a0: 2c0d 0a20 2020 2020 2020 2022 7465 6e22  ,..        "ten"
-000007b0: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-000007c0: 2022 7479 7065 223a 2022 7465 656e 7322   "type": "teens"
-000007d0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000007e0: 7661 6c75 6522 3a20 3130 2e30 2c0d 0a20  value": 10.0,.. 
-000007f0: 2020 2020 2020 2020 2020 2022 7465 726d             "term
-00000800: 7322 3a20 5b22 7465 6e22 2c20 2254 656e  s": ["ten", "Ten
-00000810: 222c 2022 5445 4e22 2c20 2274 656e 7322  ", "TEN", "tens"
-00000820: 2c20 2254 656e 7322 2c20 2254 454e 5322  , "Tens", "TENS"
-00000830: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00000840: 2020 2020 2020 2022 656c 6576 656e 223a         "eleven":
-00000850: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000860: 2274 7970 6522 3a20 2274 6565 6e73 222c  "type": "teens",
-00000870: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00000880: 616c 7565 223a 2031 312e 302c 0d0a 2020  alue": 11.0,..  
-00000890: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-000008a0: 223a 205b 2265 6c65 7665 6e22 2c20 2245  ": ["eleven", "E
-000008b0: 6c65 7665 6e22 2c20 2245 4c45 5645 4e22  leven", "ELEVEN"
-000008c0: 2c20 2265 6c65 7665 6e73 222c 2022 456c  , "elevens", "El
-000008d0: 6576 656e 7322 2c20 2245 4c45 5645 4e53  evens", "ELEVENS
-000008e0: 225d 0d0a 2020 2020 2020 2020 7d2c 0d0a  "]..        },..
-000008f0: 2020 2020 2020 2020 2274 7765 6c76 6522          "twelve"
-00000900: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00000910: 2022 7479 7065 223a 2022 7465 656e 7322   "type": "teens"
-00000920: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000930: 7661 6c75 6522 3a20 3132 2e30 2c0d 0a20  value": 12.0,.. 
-00000940: 2020 2020 2020 2020 2020 2022 7465 726d             "term
-00000950: 7322 3a20 5b22 7477 656c 7665 222c 2022  s": ["twelve", "
-00000960: 5477 656c 7665 222c 2022 5457 454c 5645  Twelve", "TWELVE
-00000970: 222c 2022 7477 656c 7665 7322 2c20 2254  ", "twelves", "T
-00000980: 7765 6c76 6573 222c 2022 5457 454c 5645  welves", "TWELVE
-00000990: 5322 5d0d 0a20 2020 2020 2020 207d 2c0d  S"]..        },.
-000009a0: 0a20 2020 2020 2020 2022 7468 6972 7465  .        "thirte
-000009b0: 656e 223a 207b 0d0a 2020 2020 2020 2020  en": {..        
-000009c0: 2020 2020 2274 7970 6522 3a20 2274 6565      "type": "tee
-000009d0: 6e73 222c 0d0a 2020 2020 2020 2020 2020  ns",..          
-000009e0: 2020 2276 616c 7565 223a 2031 332e 302c    "value": 13.0,
-000009f0: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00000a00: 6572 6d73 223a 205b 2274 6869 7274 6565  erms": ["thirtee
-00000a10: 6e22 2c20 2254 6869 7274 6565 6e22 2c20  n", "Thirteen", 
-00000a20: 2254 4849 5254 4545 4e22 2c20 2274 6869  "THIRTEEN", "thi
-00000a30: 7274 6565 6e73 222c 2022 5468 6972 7465  rteens", "Thirte
-00000a40: 656e 7322 2c20 2254 4849 5254 4545 4e53  ens", "THIRTEENS
-00000a50: 225d 0d0a 2020 2020 2020 2020 7d2c 0d0a  "]..        },..
-00000a60: 2020 2020 2020 2020 2266 6f75 7274 6565          "fourtee
-00000a70: 6e22 3a20 7b0d 0a20 2020 2020 2020 2020  n": {..         
-00000a80: 2020 2022 7479 7065 223a 2022 7465 656e     "type": "teen
-00000a90: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00000aa0: 2022 7661 6c75 6522 3a20 3134 2e30 2c0d   "value": 14.0,.
-00000ab0: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00000ac0: 726d 7322 3a20 5b22 666f 7572 7465 656e  rms": ["fourteen
-00000ad0: 222c 2022 466f 7572 7465 656e 222c 2022  ", "Fourteen", "
-00000ae0: 464f 5552 5445 454e 222c 2022 666f 7572  FOURTEEN", "four
-00000af0: 7465 656e 7322 2c20 2246 6f75 7274 6565  teens", "Fourtee
-00000b00: 6e73 222c 2022 464f 5552 5445 454e 5322  ns", "FOURTEENS"
-00000b10: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00000b20: 2020 2020 2020 2022 6669 6674 6565 6e22         "fifteen"
-00000b30: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00000b40: 2022 7479 7065 223a 2022 7465 656e 7322   "type": "teens"
-00000b50: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000b60: 7661 6c75 6522 3a20 3135 2e30 2c0d 0a20  value": 15.0,.. 
-00000b70: 2020 2020 2020 2020 2020 2022 7465 726d             "term
-00000b80: 7322 3a20 5b22 6669 6674 6565 6e22 2c20  s": ["fifteen", 
-00000b90: 2246 6966 7465 656e 222c 2022 4649 4654  "Fifteen", "FIFT
-00000ba0: 4545 4e22 2c20 2266 6966 7465 656e 7322  EEN", "fifteens"
-00000bb0: 2c20 2246 6966 7465 656e 7322 2c20 2246  , "Fifteens", "F
-00000bc0: 4946 5445 454e 5322 5d0d 0a20 2020 2020  IFTEENS"]..     
-00000bd0: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-00000be0: 7369 7874 6565 6e22 3a20 7b0d 0a20 2020  sixteen": {..   
-00000bf0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000c00: 2022 7465 656e 7322 2c0d 0a20 2020 2020   "teens",..     
-00000c10: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00000c20: 3136 2e30 2c0d 0a20 2020 2020 2020 2020  16.0,..         
-00000c30: 2020 2022 7465 726d 7322 3a20 5b22 7369     "terms": ["si
-00000c40: 7874 6565 6e22 2c20 2253 6978 7465 656e  xteen", "Sixteen
-00000c50: 222c 2022 5349 5854 4545 4e22 2c20 2273  ", "SIXTEEN", "s
-00000c60: 6978 7465 656e 7322 2c20 2253 6978 7465  ixteens", "Sixte
-00000c70: 656e 7322 2c20 2253 4958 5445 454e 5322  ens", "SIXTEENS"
-00000c80: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00000c90: 2020 2020 2020 2022 7365 7665 6e74 6565         "seventee
-00000ca0: 6e22 3a20 7b0d 0a20 2020 2020 2020 2020  n": {..         
-00000cb0: 2020 2022 7479 7065 223a 2022 7465 656e     "type": "teen
-00000cc0: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00000cd0: 2022 7661 6c75 6522 3a20 3137 2e30 2c0d   "value": 17.0,.
-00000ce0: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00000cf0: 726d 7322 3a20 5b22 7365 7665 6e74 6565  rms": ["seventee
-00000d00: 6e22 2c20 2253 6576 656e 7465 656e 222c  n", "Seventeen",
-00000d10: 2022 5345 5645 4e54 4545 4e22 2c20 2273   "SEVENTEEN", "s
-00000d20: 6576 656e 7465 656e 7322 2c20 2253 6576  eventeens", "Sev
-00000d30: 656e 7465 656e 7322 2c20 2253 4556 454e  enteens", "SEVEN
-00000d40: 5445 454e 5322 5d0d 0a20 2020 2020 2020  TEENS"]..       
-00000d50: 207d 2c0d 0a20 2020 2020 2020 2022 6569   },..        "ei
-00000d60: 6768 7465 656e 223a 207b 0d0a 2020 2020  ghteen": {..    
-00000d70: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00000d80: 2274 6565 6e73 222c 0d0a 2020 2020 2020  "teens",..      
-00000d90: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
-00000da0: 382e 302c 0d0a 2020 2020 2020 2020 2020  8.0,..          
-00000db0: 2020 2274 6572 6d73 223a 205b 2265 6967    "terms": ["eig
-00000dc0: 6874 6565 6e22 2c20 2245 6967 6874 6565  hteen", "Eightee
-00000dd0: 6e22 2c20 2245 4947 4854 4545 4e22 2c20  n", "EIGHTEEN", 
-00000de0: 2265 6967 6874 6565 6e73 222c 2022 4569  "eighteens", "Ei
-00000df0: 6768 7465 656e 7322 2c20 2245 4947 4854  ghteens", "EIGHT
-00000e00: 4545 4e53 225d 0d0a 2020 2020 2020 2020  EENS"]..        
-00000e10: 7d2c 0d0a 2020 2020 2020 2020 226e 696e  },..        "nin
-00000e20: 6574 6565 6e22 3a20 7b0d 0a20 2020 2020  eteen": {..     
-00000e30: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000e40: 7465 656e 7322 2c0d 0a20 2020 2020 2020  teens",..       
-00000e50: 2020 2020 2022 7661 6c75 6522 3a20 3139       "value": 19
-00000e60: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000e70: 2022 7465 726d 7322 3a20 5b22 6e69 6e65   "terms": ["nine
-00000e80: 7465 656e 222c 2022 4e69 6e65 7465 656e  teen", "Nineteen
-00000e90: 222c 2022 4e49 4e45 5445 454e 222c 2022  ", "NINETEEN", "
-00000ea0: 6e69 6e65 7465 656e 7322 2c20 224e 696e  nineteens", "Nin
-00000eb0: 6574 6565 6e73 222c 2022 4e49 4e45 5445  eteens", "NINETE
-00000ec0: 454e 5322 5d0d 0a20 2020 2020 2020 207d  ENS"]..        }
-00000ed0: 2c0d 0a20 2020 2020 2020 2022 7477 656e  ,..        "twen
-00000ee0: 7479 223a 207b 0d0a 2020 2020 2020 2020  ty": {..        
-00000ef0: 2020 2020 2274 7970 6522 3a20 2274 656e      "type": "ten
-00000f00: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00000f10: 2022 7661 6c75 6522 3a20 3230 2e30 2c0d   "value": 20.0,.
-00000f20: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00000f30: 726d 7322 3a20 5b22 7477 656e 7479 222c  rms": ["twenty",
-00000f40: 2022 5477 656e 7479 222c 2022 5457 454e   "Twenty", "TWEN
-00000f50: 5459 222c 2022 7477 656e 7469 6573 222c  TY", "twenties",
-00000f60: 2022 5477 656e 7469 6573 222c 2022 5457   "Twenties", "TW
-00000f70: 454e 5449 4553 225d 0d0a 2020 2020 2020  ENTIES"]..      
-00000f80: 2020 7d2c 0d0a 2020 2020 2020 2020 2274    },..        "t
-00000f90: 6869 7274 7922 3a20 7b0d 0a20 2020 2020  hirty": {..     
-00000fa0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000fb0: 7465 6e73 222c 0d0a 2020 2020 2020 2020  tens",..        
-00000fc0: 2020 2020 2276 616c 7565 223a 2033 302e      "value": 30.
-00000fd0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00000fe0: 2274 6572 6d73 223a 205b 2274 6869 7274  "terms": ["thirt
-00000ff0: 7922 2c20 2254 6869 7274 7922 2c20 2254  y", "Thirty", "T
-00001000: 4849 5254 5922 2c20 2274 6869 7274 6965  HIRTY", "thirtie
-00001010: 7322 2c20 2254 6869 7274 6965 7322 2c20  s", "Thirties", 
-00001020: 2254 4849 5254 4945 5322 5d0d 0a20 2020  "THIRTIES"]..   
-00001030: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00001040: 2022 666f 7274 7922 3a20 7b0d 0a20 2020   "forty": {..   
-00001050: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00001060: 2022 7465 6e73 222c 0d0a 2020 2020 2020   "tens",..      
-00001070: 2020 2020 2020 2276 616c 7565 223a 2034        "value": 4
-00001080: 302e 302c 0d0a 2020 2020 2020 2020 2020  0.0,..          
-00001090: 2020 2274 6572 6d73 223a 205b 2266 6f72    "terms": ["for
-000010a0: 7479 222c 2022 466f 7274 7922 2c20 2246  ty", "Forty", "F
-000010b0: 4f52 5459 222c 2022 666f 7274 6965 7322  ORTY", "forties"
-000010c0: 2c20 2246 6f72 7469 6573 222c 2022 464f  , "Forties", "FO
-000010d0: 5254 4945 5322 2c20 2266 6f75 7274 7922  RTIES", "fourty"
-000010e0: 2c20 2246 6f75 7274 7922 2c20 2246 4f55  , "Fourty", "FOU
-000010f0: 5254 5922 2c20 2266 6f75 7274 6965 7322  RTY", "fourties"
-00001100: 2c20 2246 6f75 7274 6965 7322 2c20 2246  , "Fourties", "F
-00001110: 4f55 5254 4945 5322 5d0d 0a20 2020 2020  OURTIES"]..     
-00001120: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-00001130: 6669 6674 7922 3a20 7b0d 0a20 2020 2020  fifty": {..     
-00001140: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00001150: 7465 6e73 222c 0d0a 2020 2020 2020 2020  tens",..        
-00001160: 2020 2020 2276 616c 7565 223a 2035 302e      "value": 50.
-00001170: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00001180: 2274 6572 6d73 223a 205b 2266 6966 7479  "terms": ["fifty
-00001190: 222c 2022 4669 6674 7922 2c20 2246 4946  ", "Fifty", "FIF
-000011a0: 5459 222c 2022 6669 6674 6965 7322 2c20  TY", "fifties", 
-000011b0: 2246 6966 7469 6573 222c 2022 4649 4654  "Fifties", "FIFT
-000011c0: 4945 5322 5d0d 0a20 2020 2020 2020 207d  IES"]..        }
-000011d0: 2c0d 0a20 2020 2020 2020 2022 7369 7874  ,..        "sixt
-000011e0: 7922 3a20 7b0d 0a20 2020 2020 2020 2020  y": {..         
-000011f0: 2020 2022 7479 7065 223a 2022 7465 6e73     "type": "tens
-00001200: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001210: 2276 616c 7565 223a 2036 302e 302c 0d0a  "value": 60.0,..
-00001220: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
-00001230: 6d73 223a 205b 2273 6978 7479 222c 2022  ms": ["sixty", "
-00001240: 5369 7874 7922 2c20 2253 4958 5459 222c  Sixty", "SIXTY",
-00001250: 2022 7369 7874 6965 7322 2c20 2253 6978   "sixties", "Six
-00001260: 7469 6573 222c 2022 5349 5854 4945 5322  ties", "SIXTIES"
-00001270: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00001280: 2020 2020 2020 2022 7365 7665 6e74 7922         "seventy"
-00001290: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-000012a0: 2022 7479 7065 223a 2022 7465 6e73 222c   "type": "tens",
-000012b0: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-000012c0: 616c 7565 223a 2037 302e 302c 0d0a 2020  alue": 70.0,..  
-000012d0: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-000012e0: 223a 205b 2273 6576 656e 7479 222c 2022  ": ["seventy", "
-000012f0: 5365 7665 6e74 7922 2c20 2253 4556 454e  Seventy", "SEVEN
-00001300: 5459 222c 2022 7365 7665 6e74 6965 7322  TY", "seventies"
-00001310: 2c20 2253 6576 656e 7469 6573 222c 2022  , "Seventies", "
-00001320: 5345 5645 4e54 4945 5322 5d0d 0a20 2020  SEVENTIES"]..   
-00001330: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00001340: 2022 6569 6768 7479 223a 207b 0d0a 2020   "eighty": {..  
-00001350: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001360: 3a20 2274 656e 7322 2c0d 0a20 2020 2020  : "tens",..     
-00001370: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00001380: 3830 2e30 2c0d 0a20 2020 2020 2020 2020  80.0,..         
-00001390: 2020 2022 7465 726d 7322 3a20 5b22 6569     "terms": ["ei
-000013a0: 6768 7479 222c 2022 4569 6768 7479 222c  ghty", "Eighty",
-000013b0: 2022 4549 4748 5459 222c 2022 6569 6768   "EIGHTY", "eigh
-000013c0: 7469 6573 222c 2022 4569 6768 7469 6573  ties", "Eighties
-000013d0: 222c 2022 4549 4748 5449 4553 225d 0d0a  ", "EIGHTIES"]..
-000013e0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000013f0: 2020 2020 226e 696e 6574 7922 3a20 7b0d      "ninety": {.
-00001400: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00001410: 7065 223a 2022 7465 6e73 222c 0d0a 2020  pe": "tens",..  
-00001420: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00001430: 223a 2039 302e 302c 0d0a 2020 2020 2020  ": 90.0,..      
-00001440: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00001450: 226e 696e 6574 7922 2c20 224e 696e 6574  "ninety", "Ninet
-00001460: 7922 2c20 224e 494e 4554 5922 2c20 226e  y", "NINETY", "n
-00001470: 696e 6574 6965 7322 2c20 224e 696e 6574  ineties", "Ninet
-00001480: 6965 7322 2c20 224e 494e 4554 4945 5322  ies", "NINETIES"
-00001490: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-000014a0: 2020 2020 2020 2022 6875 6e64 7265 6422         "hundred"
-000014b0: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-000014c0: 2022 7479 7065 223a 2022 7468 6f75 7361   "type": "thousa
-000014d0: 6e64 7322 2c0d 0a20 2020 2020 2020 2020  nds",..         
-000014e0: 2020 2022 7661 6c75 6522 3a20 3130 302e     "value": 100.
-000014f0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00001500: 2274 6572 6d73 223a 205b 2268 756e 6472  "terms": ["hundr
-00001510: 6564 222c 2022 4875 6e64 7265 6422 2c20  ed", "Hundred", 
-00001520: 2248 554e 4452 4544 222c 2022 6875 6e64  "HUNDRED", "hund
-00001530: 7265 6473 222c 2022 4875 6e64 7265 6473  reds", "Hundreds
-00001540: 222c 2022 4855 4e44 5245 4453 225d 0d0a  ", "HUNDREDS"]..
-00001550: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00001560: 2020 2020 2274 686f 7573 616e 6422 3a20      "thousand": 
-00001570: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00001580: 7479 7065 223a 2022 7468 6f75 7361 6e64  type": "thousand
-00001590: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-000015a0: 2022 7661 6c75 6522 3a20 3130 3030 2e30   "value": 1000.0
-000015b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000015c0: 7465 726d 7322 3a20 5b22 7468 6f75 7361  terms": ["thousa
-000015d0: 6e64 222c 2022 5468 6f75 7361 6e64 222c  nd", "Thousand",
-000015e0: 2022 5448 4f55 5341 4e44 222c 2022 7468   "THOUSAND", "th
-000015f0: 6f75 7361 6e64 7322 2c20 2254 686f 7573  ousands", "Thous
-00001600: 616e 6473 222c 2022 5448 4f55 5341 4e44  ands", "THOUSAND
-00001610: 5322 5d0d 0a20 2020 2020 2020 207d 2c0d  S"]..        },.
-00001620: 0a20 2020 2020 2020 2022 6d69 6c6c 696f  .        "millio
-00001630: 6e22 3a20 7b0d 0a20 2020 2020 2020 2020  n": {..         
-00001640: 2020 2022 7479 7065 223a 2022 7468 6f75     "type": "thou
-00001650: 7361 6e64 7322 2c0d 0a20 2020 2020 2020  sands",..       
-00001660: 2020 2020 2022 7661 6c75 6522 3a20 3130       "value": 10
-00001670: 3030 3030 302e 302c 0d0a 2020 2020 2020  00000.0,..      
-00001680: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00001690: 226d 696c 6c69 6f6e 222c 2022 4d69 6c6c  "million", "Mill
-000016a0: 696f 6e22 2c20 224d 494c 4c49 4f4e 222c  ion", "MILLION",
-000016b0: 2022 6d69 6c6c 696f 6e73 222c 2022 4d69   "millions", "Mi
-000016c0: 6c6c 696f 6e73 222c 2022 4d49 4c4c 494f  llions", "MILLIO
-000016d0: 4e53 225d 0d0a 2020 2020 2020 2020 7d2c  NS"]..        },
-000016e0: 0d0a 2020 2020 2020 2020 2262 696c 6c69  ..        "billi
-000016f0: 6f6e 223a 207b 0d0a 2020 2020 2020 2020  on": {..        
-00001700: 2020 2020 2274 7970 6522 3a20 2274 686f      "type": "tho
-00001710: 7573 616e 6473 222c 0d0a 2020 2020 2020  usands",..      
-00001720: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
-00001730: 3030 3030 3030 3030 302e 302c 0d0a 2020  000000000.0,..  
-00001740: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-00001750: 223a 205b 2262 696c 6c69 6f6e 222c 2022  ": ["billion", "
-00001760: 4269 6c6c 696f 6e22 2c20 2242 494c 4c49  Billion", "BILLI
-00001770: 4f4e 222c 2022 6269 6c6c 696f 6e73 222c  ON", "billions",
-00001780: 2022 4269 6c6c 696f 6e73 222c 2022 4249   "Billions", "BI
-00001790: 4c4c 494f 4e53 225d 0d0a 2020 2020 2020  LLIONS"]..      
-000017a0: 2020 7d2c 0d0a 2020 2020 2020 2020 2274    },..        "t
-000017b0: 7269 6c6c 696f 6e22 3a20 7b0d 0a20 2020  rillion": {..   
-000017c0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000017d0: 2022 7468 6f75 7361 6e64 7322 2c0d 0a20   "thousands",.. 
-000017e0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-000017f0: 6522 3a20 3130 3030 3030 3030 3030 3030  e": 100000000000
-00001800: 302e 302c 0d0a 2020 2020 2020 2020 2020  0.0,..          
-00001810: 2020 2274 6572 6d73 223a 205b 2274 7269    "terms": ["tri
-00001820: 6c6c 696f 6e22 2c20 2254 7269 6c6c 696f  llion", "Trillio
-00001830: 6e22 2c20 2254 5249 4c4c 494f 4e22 2c20  n", "TRILLION", 
-00001840: 2274 7269 6c6c 696f 6e73 222c 2022 5472  "trillions", "Tr
-00001850: 696c 6c69 6f6e 7322 2c20 2254 5249 4c4c  illions", "TRILL
-00001860: 494f 4e53 225d 0d0a 2020 2020 2020 2020  IONS"]..        
-00001870: 7d2c 0d0a 2020 2020 2020 2020 2266 756c  },..        "ful
-00001880: 6c22 3a20 7b0d 0a20 2020 2020 2020 2020  l": {..         
-00001890: 2020 2022 7479 7065 223a 2022 6d6f 6469     "type": "modi
-000018a0: 6669 6572 7322 2c0d 0a20 2020 2020 2020  fiers",..       
-000018b0: 2020 2020 2022 7661 6c75 6522 3a20 312e       "value": 1.
-000018c0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-000018d0: 2274 6572 6d73 223a 205b 2266 756c 6c22  "terms": ["full"
-000018e0: 2c20 2246 756c 6c22 2c20 2246 554c 4c22  , "Full", "FULL"
-000018f0: 2c20 2277 686f 6c65 222c 2022 5768 6f6c  , "whole", "Whol
-00001900: 6522 2c20 2257 484f 4c45 225d 0d0a 2020  e", "WHOLE"]..  
-00001910: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00001920: 2020 2268 616c 6622 3a20 7b0d 0a20 2020    "half": {..   
-00001930: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00001940: 2022 6d6f 6469 6669 6572 7322 2c0d 0a20   "modifiers",.. 
-00001950: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00001960: 6522 3a20 302e 352c 0d0a 2020 2020 2020  e": 0.5,..      
-00001970: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00001980: 2268 616c 6622 2c20 2248 616c 6622 2c20  "half", "Half", 
-00001990: 2248 414c 4622 2c20 2268 616c 7665 7322  "HALF", "halves"
-000019a0: 2c20 2248 616c 7665 7322 2c20 2248 414c  , "Halves", "HAL
-000019b0: 5645 5322 5d0d 0a20 2020 2020 2020 207d  VES"]..        }
-000019c0: 2c0d 0a20 2020 2020 2020 2022 7468 6972  ,..        "thir
-000019d0: 6422 3a20 7b0d 0a20 2020 2020 2020 2020  d": {..         
-000019e0: 2020 2022 7479 7065 223a 2022 6d6f 6469     "type": "modi
-000019f0: 6669 6572 7322 2c0d 0a20 2020 2020 2020  fiers",..       
-00001a00: 2020 2020 2022 7661 6c75 6522 3a20 2231       "value": "1
-00001a10: 2f33 222c 0d0a 2020 2020 2020 2020 2020  /3",..          
-00001a20: 2020 2274 6572 6d73 223a 205b 2274 6869    "terms": ["thi
-00001a30: 7264 222c 2022 5468 6972 6422 2c20 2254  rd", "Third", "T
-00001a40: 4849 5244 222c 2022 7468 6972 6473 222c  HIRD", "thirds",
-00001a50: 2022 5468 6972 6473 222c 2022 5448 4952   "Thirds", "THIR
-00001a60: 4453 225d 0d0a 2020 2020 2020 2020 7d2c  DS"]..        },
-00001a70: 0d0a 2020 2020 2020 2020 2271 7561 7274  ..        "quart
-00001a80: 6572 223a 207b 0d0a 2020 2020 2020 2020  er": {..        
-00001a90: 2020 2020 2274 7970 6522 3a20 226d 6f64      "type": "mod
-00001aa0: 6966 6965 7273 222c 0d0a 2020 2020 2020  ifiers",..      
-00001ab0: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
-00001ac0: 2e32 352c 0d0a 2020 2020 2020 2020 2020  .25,..          
-00001ad0: 2020 2274 6572 6d73 223a 205b 2271 7561    "terms": ["qua
-00001ae0: 7274 6572 222c 2022 5175 6172 7465 7222  rter", "Quarter"
-00001af0: 2c20 2251 5541 5254 4552 222c 2022 7175  , "QUARTER", "qu
-00001b00: 6172 7465 7273 222c 2022 5175 6172 7465  arters", "Quarte
-00001b10: 7273 222c 2022 5155 4152 5445 5253 225d  rs", "QUARTERS"]
-00001b20: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00001b30: 2020 2020 2020 226d 756c 7469 706c 6965        "multiplie
-00001b40: 7222 3a20 7b0d 0a20 2020 2020 2020 2020  r": {..         
-00001b50: 2020 2022 7479 7065 223a 2022 6d75 6c74     "type": "mult
-00001b60: 6970 6c69 6572 222c 0d0a 2020 2020 2020  iplier",..      
-00001b70: 2020 2020 2020 2276 616c 7565 223a 202d        "value": -
-00001b80: 312e 302c 0d0a 2020 2020 2020 2020 2020  1.0,..          
-00001b90: 2020 2274 6572 6d73 223a 205b 226f 6622    "terms": ["of"
-00001ba0: 2c20 224f 6622 2c20 224f 4622 5d0d 0a20  , "Of", "OF"].. 
-00001bb0: 2020 2020 2020 207d 0d0a 2020 2020 7d2c         }..    },
-00001bc0: 0d0a 2020 2020 2273 6361 6c65 7322 3a20  ..    "scales": 
-00001bd0: 7b0d 0a20 2020 2020 2020 2022 6d69 6c6c  {..        "mill
-00001be0: 6973 6563 6f6e 6422 3a20 7b0d 0a20 2020  isecond": {..   
-00001bf0: 2020 2020 2020 2020 2022 7363 616c 6522           "scale"
-00001c00: 3a20 302e 3030 312c 0d0a 2020 2020 2020  : 0.001,..      
-00001c10: 2020 2020 2020 2273 696e 6775 6c61 7222        "singular"
-00001c20: 3a20 226d 696c 6c69 7365 636f 6e64 222c  : "millisecond",
-00001c30: 0d0a 2020 2020 2020 2020 2020 2020 2270  ..            "p
-00001c40: 6c75 7261 6c22 3a20 226d 696c 6c69 7365  lural": "millise
-00001c50: 636f 6e64 7322 2c0d 0a20 2020 2020 2020  conds",..       
-00001c60: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-00001c70: 6d73 222c 2022 4d73 222c 2022 4d53 222c  ms", "Ms", "MS",
-00001c80: 2022 6d69 6c6c 6973 6563 6f6e 6422 2c20   "millisecond", 
-00001c90: 224d 696c 6c69 7365 636f 6e64 222c 2022  "Millisecond", "
-00001ca0: 4d49 4c4c 4953 4543 4f4e 4422 2c20 226d  MILLISECOND", "m
-00001cb0: 696c 6c69 7365 636f 6e64 7322 2c20 224d  illiseconds", "M
-00001cc0: 696c 6c69 7365 636f 6e64 7322 2c20 224d  illiseconds", "M
-00001cd0: 494c 4c49 5345 434f 4e44 5322 5d0d 0a20  ILLISECONDS"].. 
-00001ce0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00001cf0: 2020 2022 7365 636f 6e64 223a 207b 0d0a     "second": {..
-00001d00: 2020 2020 2020 2020 2020 2020 2273 6361              "sca
-00001d10: 6c65 223a 2031 2e30 2c0d 0a20 2020 2020  le": 1.0,..     
-00001d20: 2020 2020 2020 2022 7369 6e67 756c 6172         "singular
-00001d30: 223a 2022 7365 636f 6e64 222c 0d0a 2020  ": "second",..  
-00001d40: 2020 2020 2020 2020 2020 2270 6c75 7261            "plura
-00001d50: 6c22 3a20 2273 6563 6f6e 6473 222c 0d0a  l": "seconds",..
-00001d60: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
-00001d70: 6d73 223a 205b 2273 222c 2022 5322 2c20  ms": ["s", "S", 
-00001d80: 2273 6563 222c 2022 5365 6322 2c20 2253  "sec", "Sec", "S
-00001d90: 4543 222c 2022 7365 6373 222c 2022 5365  EC", "secs", "Se
-00001da0: 6373 222c 2022 5345 4353 222c 2022 7365  cs", "SECS", "se
-00001db0: 636f 6e64 222c 2022 5365 636f 6e64 222c  cond", "Second",
-00001dc0: 2022 5345 434f 4e44 222c 2022 7365 636f   "SECOND", "seco
-00001dd0: 6e64 7322 2c20 2253 6563 6f6e 6473 222c  nds", "Seconds",
-00001de0: 2022 5345 434f 4e44 5322 5d0d 0a20 2020   "SECONDS"]..   
-00001df0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00001e00: 2022 6d69 6e75 7465 223a 207b 0d0a 2020   "minute": {..  
-00001e10: 2020 2020 2020 2020 2020 2273 6361 6c65            "scale
-00001e20: 223a 2036 302e 302c 0d0a 2020 2020 2020  ": 60.0,..      
-00001e30: 2020 2020 2020 2273 696e 6775 6c61 7222        "singular"
-00001e40: 3a20 226d 696e 7574 6522 2c0d 0a20 2020  : "minute",..   
-00001e50: 2020 2020 2020 2020 2022 706c 7572 616c           "plural
-00001e60: 223a 2022 6d69 6e75 7465 7322 2c0d 0a20  ": "minutes",.. 
-00001e70: 2020 2020 2020 2020 2020 2022 7465 726d             "term
-00001e80: 7322 3a20 5b22 6d22 2c20 226d 696e 222c  s": ["m", "min",
-00001e90: 2022 4d69 6e22 2c20 224d 494e 222c 2022   "Min", "MIN", "
-00001ea0: 6d69 6e73 222c 2022 4d69 6e73 222c 2022  mins", "Mins", "
-00001eb0: 4d49 4e53 222c 2022 6d69 6e75 7465 222c  MINS", "minute",
-00001ec0: 2022 4d69 6e75 7465 222c 2022 4d49 4e55   "Minute", "MINU
-00001ed0: 5445 222c 2022 6d69 6e75 7465 7322 2c20  TE", "minutes", 
-00001ee0: 224d 696e 7574 6573 222c 2022 4d49 4e55  "Minutes", "MINU
-00001ef0: 5445 5322 5d0d 0a20 2020 2020 2020 207d  TES"]..        }
-00001f00: 2c0d 0a20 2020 2020 2020 2022 686f 7572  ,..        "hour
-00001f10: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00001f20: 2020 2273 6361 6c65 223a 2033 3630 302e    "scale": 3600.
-00001f30: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00001f40: 2273 696e 6775 6c61 7222 3a20 2268 6f75  "singular": "hou
-00001f50: 7222 2c0d 0a20 2020 2020 2020 2020 2020  r",..           
-00001f60: 2022 706c 7572 616c 223a 2022 686f 7572   "plural": "hour
-00001f70: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00001f80: 2022 7465 726d 7322 3a20 5b22 6822 2c20   "terms": ["h", 
-00001f90: 2248 222c 2022 6872 222c 2022 4872 222c  "H", "hr", "Hr",
-00001fa0: 2022 4852 222c 2022 6872 7322 2c20 2248   "HR", "hrs", "H
-00001fb0: 7273 222c 2022 4852 5322 2c20 2268 6f75  rs", "HRS", "hou
-00001fc0: 7222 2c20 2248 6f75 7222 2c20 2248 4f55  r", "Hour", "HOU
-00001fd0: 5222 2c20 2268 6f75 7273 222c 2022 486f  R", "hours", "Ho
-00001fe0: 7572 7322 2c20 2248 4f55 5253 225d 0d0a  urs", "HOURS"]..
-00001ff0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00002000: 2020 2020 2264 6179 223a 207b 0d0a 2020      "day": {..  
-00002010: 2020 2020 2020 2020 2020 2273 6361 6c65            "scale
-00002020: 223a 2038 3634 3030 2e30 2c0d 0a20 2020  ": 86400.0,..   
-00002030: 2020 2020 2020 2020 2022 7369 6e67 756c           "singul
-00002040: 6172 223a 2022 6461 7922 2c0d 0a20 2020  ar": "day",..   
-00002050: 2020 2020 2020 2020 2022 706c 7572 616c           "plural
-00002060: 223a 2022 6461 7973 222c 0d0a 2020 2020  ": "days",..    
-00002070: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
-00002080: 205b 2264 222c 2022 6461 7922 2c20 2244   ["d", "day", "D
-00002090: 6179 222c 2022 4441 5922 2c20 2264 6179  ay", "DAY", "day
-000020a0: 7322 2c20 2244 6179 7322 2c20 2244 4159  s", "Days", "DAY
-000020b0: 5322 2c20 2264 7922 2c20 2244 7922 2c20  S", "dy", "Dy", 
-000020c0: 2244 5922 2c20 2264 7973 222c 2022 4479  "DY", "dys", "Dy
-000020d0: 7322 2c20 2244 5953 225d 0d0a 2020 2020  s", "DYS"]..    
-000020e0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-000020f0: 2277 6565 6b22 3a20 7b0d 0a20 2020 2020  "week": {..     
-00002100: 2020 2020 2020 2022 7363 616c 6522 3a20         "scale": 
-00002110: 3630 3438 3030 2e30 2c0d 0a20 2020 2020  604800.0,..     
-00002120: 2020 2020 2020 2022 7369 6e67 756c 6172         "singular
-00002130: 223a 2022 7765 656b 222c 0d0a 2020 2020  ": "week",..    
-00002140: 2020 2020 2020 2020 2270 6c75 7261 6c22          "plural"
-00002150: 3a20 2277 6565 6b73 222c 0d0a 2020 2020  : "weeks",..    
-00002160: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
-00002170: 205b 2277 222c 2022 5722 2c20 2277 6b22   ["w", "W", "wk"
-00002180: 2c20 2257 6b22 2c20 2257 4b22 2c20 2277  , "Wk", "WK", "w
-00002190: 6b73 222c 2022 576b 7322 2c20 2257 4b53  ks", "Wks", "WKS
-000021a0: 222c 2022 7765 656b 222c 2022 5765 656b  ", "week", "Week
-000021b0: 222c 2022 5745 454b 222c 2022 7765 656b  ", "WEEK", "week
-000021c0: 7322 2c20 2257 6565 6b73 222c 2022 5745  s", "Weeks", "WE
-000021d0: 454b 5322 5d0d 0a20 2020 2020 2020 207d  EKS"]..        }
-000021e0: 2c0d 0a20 2020 2020 2020 2022 6d6f 6e74  ,..        "mont
-000021f0: 6822 3a20 7b0d 0a20 2020 2020 2020 2020  h": {..         
-00002200: 2020 2022 7363 616c 6522 3a20 3236 3335     "scale": 2635
-00002210: 3230 302e 302c 0d0a 2020 2020 2020 2020  200.0,..        
-00002220: 2020 2020 2273 696e 6775 6c61 7222 3a20      "singular": 
-00002230: 226d 6f6e 7468 222c 0d0a 2020 2020 2020  "month",..      
-00002240: 2020 2020 2020 2270 6c75 7261 6c22 3a20        "plural": 
-00002250: 226d 6f6e 7468 7322 2c0d 0a20 2020 2020  "months",..     
-00002260: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
-00002270: 5b22 4d22 2c20 226d 6f6e 7468 222c 2022  ["M", "month", "
-00002280: 4d6f 6e74 6822 2c20 224d 4f4e 5448 222c  Month", "MONTH",
-00002290: 2022 6d6f 6e74 6873 222c 2022 4d6f 6e74   "months", "Mont
-000022a0: 6873 222c 2022 4d4f 4e54 4853 222c 2022  hs", "MONTHS", "
-000022b0: 6d6f 222c 2022 4d6f 222c 2022 4d4f 225d  mo", "Mo", "MO"]
-000022c0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000022d0: 2020 2020 2020 2279 6561 7222 3a20 7b0d        "year": {.
-000022e0: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
-000022f0: 616c 6522 3a20 3331 3533 3630 3030 2e30  ale": 31536000.0
-00002300: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002310: 7369 6e67 756c 6172 223a 2022 7965 6172  singular": "year
-00002320: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002330: 2270 6c75 7261 6c22 3a20 2279 6561 7273  "plural": "years
-00002340: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002350: 2274 6572 6d73 223a 205b 2279 222c 2022  "terms": ["y", "
-00002360: 5922 2c20 2279 7222 2c20 2259 7222 2c20  Y", "yr", "Yr", 
-00002370: 2259 5222 2c20 2279 7273 222c 2022 5972  "YR", "yrs", "Yr
-00002380: 7322 2c20 2259 5253 222c 2022 7965 6172  s", "YRS", "year
-00002390: 222c 2022 5965 6172 222c 2022 5945 4152  ", "Year", "YEAR
-000023a0: 222c 2022 7965 6172 7322 2c20 2259 6561  ", "years", "Yea
-000023b0: 7273 222c 2022 5945 4152 5322 5d0d 0a20  rs", "YEARS"].. 
-000023c0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000023d0: 2020 2022 6465 6361 6465 223a 207b 0d0a     "decade": {..
-000023e0: 2020 2020 2020 2020 2020 2020 2273 6361              "sca
-000023f0: 6c65 223a 2033 3135 3336 3030 3030 2e30  le": 315360000.0
-00002400: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002410: 7369 6e67 756c 6172 223a 2022 6465 6361  singular": "deca
-00002420: 6465 222c 0d0a 2020 2020 2020 2020 2020  de",..          
-00002430: 2020 2270 6c75 7261 6c22 3a20 2264 6563    "plural": "dec
-00002440: 6164 6573 222c 0d0a 2020 2020 2020 2020  ades",..        
-00002450: 2020 2020 2274 6572 6d73 223a 205b 2244      "terms": ["D
-00002460: 222c 2022 6465 6322 2c20 2244 6563 222c  ", "dec", "Dec",
-00002470: 2022 4445 4322 2c20 2264 6563 7322 2c20   "DEC", "decs", 
-00002480: 2244 6563 7322 2c20 2244 4543 5322 2c20  "Decs", "DECS", 
-00002490: 2264 6563 6164 6522 2c20 2244 6563 6164  "decade", "Decad
-000024a0: 6522 2c20 2244 4543 4144 4522 2c20 2264  e", "DECADE", "d
-000024b0: 6563 6164 6573 222c 2022 4465 6361 6465  ecades", "Decade
-000024c0: 7322 2c20 2244 4543 4144 4553 225d 0d0a  s", "DECADES"]..
-000024d0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000024e0: 2020 2020 2263 656e 7475 7279 223a 207b      "century": {
-000024f0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-00002500: 6361 6c65 223a 2033 3135 3336 3030 3030  cale": 315360000
-00002510: 302e 302c 0d0a 2020 2020 2020 2020 2020  0.0,..          
-00002520: 2020 2273 696e 6775 6c61 7222 3a20 2263    "singular": "c
-00002530: 656e 7475 7279 222c 0d0a 2020 2020 2020  entury",..      
-00002540: 2020 2020 2020 2270 6c75 7261 6c22 3a20        "plural": 
-00002550: 2263 656e 7475 7269 6573 222c 0d0a 2020  "centuries",..  
-00002560: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-00002570: 223a 205b 2263 222c 2022 4322 2c20 2263  ": ["c", "C", "c
-00002580: 656e 7475 7279 222c 2022 4365 6e74 7572  entury", "Centur
-00002590: 7922 2c20 2243 454e 5455 5259 222c 2022  y", "CENTURY", "
-000025a0: 6365 6e74 7572 6965 7322 2c20 2243 656e  centuries", "Cen
-000025b0: 7475 7269 6573 222c 2022 4345 4e54 5552  turies", "CENTUR
-000025c0: 4945 5322 5d0d 0a20 2020 2020 2020 207d  IES"]..        }
-000025d0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2265  ..    },..    "e
-000025e0: 7874 7261 5f64 6174 6122 3a20 7b0d 0a20  xtra_data": {.. 
-000025f0: 2020 207d 0d0a 7d0d 0a                      }..}..
+00000000: 7b0a 2020 2020 2263 6f6e 6e65 6374 6f72  {.    "connector
+00000010: 7322 3a20 5b22 2022 2c20 225c 7422 2c20  s": [" ", "\t", 
+00000020: 222d 225d 2c0a 2020 2020 2273 6567 6d65  "-"],.    "segme
+00000030: 6e74 6f72 7322 3a20 5b22 2c22 2c20 2261  ntors": [",", "a
+00000040: 6e64 222c 2022 2622 5d2c 0a20 2020 2022  nd", "&"],.    "
+00000050: 616c 6c6f 7765 645f 7465 726d 7322 3a20  allowed_terms": 
+00000060: 5b22 2122 2c20 223f 222c 2022 2722 2c20  ["!", "?", "'", 
+00000070: 222e 222c 2022 2c22 2c20 2274 6865 225d  ".", ",", "the"]
+00000080: 2c0a 2020 2020 2264 6563 696d 616c 5f73  ,.    "decimal_s
+00000090: 6570 6172 6174 6f72 7322 3a20 5b22 2e22  eparators": ["."
+000000a0: 5d2c 0a20 2020 2022 7468 6f75 7361 6e64  ],.    "thousand
+000000b0: 5f73 6570 6172 6174 6f72 7322 3a20 5b22  _separators": ["
+000000c0: 2c22 2c20 2220 225d 2c0a 2020 2020 2270  ,", " "],.    "p
+000000d0: 6172 7365 725f 6669 6c65 223a 2022 7061  arser_file": "pa
+000000e0: 7273 6572 5f6f 6e65 2e70 7922 2c0a 2020  rser_one.py",.  
+000000f0: 2020 226e 756d 6572 616c 7322 3a20 7b0a    "numerals": {.
+00000100: 2020 2020 2020 2020 227a 6572 6f22 3a20          "zero": 
+00000110: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
+00000120: 7970 6522 3a20 2264 6967 6974 7322 2c0a  ype": "digits",.
+00000130: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00000140: 7565 223a 2030 2e30 2c0a 2020 2020 2020  ue": 0.0,.      
+00000150: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
+00000160: 227a 6572 6f22 2c20 225a 6572 6f22 2c20  "zero", "Zero", 
+00000170: 225a 4552 4f22 2c20 227a 6572 6f65 7322  "ZERO", "zeroes"
+00000180: 2c20 225a 6572 6f65 7322 2c20 225a 4552  , "Zeroes", "ZER
+00000190: 4f45 5322 2c20 227a 6572 6f73 222c 2022  OES", "zeros", "
+000001a0: 5a65 726f 7322 2c20 225a 4552 4f53 225d  Zeros", "ZEROS"]
+000001b0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000001c0: 2020 2020 226f 6e65 223a 207b 0a20 2020      "one": {.   
+000001d0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000001e0: 2022 6469 6769 7473 222c 0a20 2020 2020   "digits",.     
+000001f0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00000200: 312e 302c 0a20 2020 2020 2020 2020 2020  1.0,.           
+00000210: 2022 7465 726d 7322 3a20 5b22 6f6e 6522   "terms": ["one"
+00000220: 2c20 224f 6e65 222c 2022 4f4e 4522 2c20  , "One", "ONE", 
+00000230: 226f 6e65 7322 2c20 224f 6e65 7322 2c20  "ones", "Ones", 
+00000240: 224f 4e45 5322 2c20 2261 222c 2022 4122  "ONES", "a", "A"
+00000250: 2c20 2261 6e22 2c20 2241 6e22 2c20 2241  , "an", "An", "A
+00000260: 4e22 5d0a 2020 2020 2020 2020 7d2c 0a20  N"].        },. 
+00000270: 2020 2020 2020 2022 7477 6f22 3a20 7b0a         "two": {.
+00000280: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00000290: 6522 3a20 2264 6967 6974 7322 2c0a 2020  e": "digits",.  
+000002a0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+000002b0: 223a 2032 2e30 2c0a 2020 2020 2020 2020  ": 2.0,.        
+000002c0: 2020 2020 2274 6572 6d73 223a 205b 2274      "terms": ["t
+000002d0: 776f 222c 2022 5477 6f22 2c20 2254 574f  wo", "Two", "TWO
+000002e0: 222c 2022 7477 6f73 222c 2022 5477 6f73  ", "twos", "Twos
+000002f0: 222c 2022 5457 4f53 225d 0a20 2020 2020  ", "TWOS"].     
+00000300: 2020 207d 2c0a 2020 2020 2020 2020 2274     },.        "t
+00000310: 6872 6565 223a 207b 0a20 2020 2020 2020  hree": {.       
+00000320: 2020 2020 2022 7479 7065 223a 2022 6469       "type": "di
+00000330: 6769 7473 222c 0a20 2020 2020 2020 2020  gits",.         
+00000340: 2020 2022 7661 6c75 6522 3a20 332e 302c     "value": 3.0,
+00000350: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00000360: 726d 7322 3a20 5b22 7468 7265 6522 2c20  rms": ["three", 
+00000370: 2254 6872 6565 222c 2022 5448 5245 4522  "Three", "THREE"
+00000380: 2c20 2274 6872 6565 7322 2c20 2254 6872  , "threes", "Thr
+00000390: 6565 7322 2c20 2254 4852 4545 5322 5d0a  ees", "THREES"].
+000003a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000003b0: 2020 2022 666f 7572 223a 207b 0a20 2020     "four": {.   
+000003c0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000003d0: 2022 6469 6769 7473 222c 0a20 2020 2020   "digits",.     
+000003e0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000003f0: 342e 302c 0a20 2020 2020 2020 2020 2020  4.0,.           
+00000400: 2022 7465 726d 7322 3a20 5b22 666f 7572   "terms": ["four
+00000410: 222c 2022 466f 7572 222c 2022 464f 5552  ", "Four", "FOUR
+00000420: 222c 2022 666f 7572 7322 2c20 2246 6f75  ", "fours", "Fou
+00000430: 7273 222c 2022 464f 5552 5322 5d0a 2020  rs", "FOURS"].  
+00000440: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000450: 2022 6669 7665 223a 207b 0a20 2020 2020   "five": {.     
+00000460: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000470: 6469 6769 7473 222c 0a20 2020 2020 2020  digits",.       
+00000480: 2020 2020 2022 7661 6c75 6522 3a20 352e       "value": 5.
+00000490: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+000004a0: 7465 726d 7322 3a20 5b22 6669 7665 222c  terms": ["five",
+000004b0: 2022 4669 7665 222c 2022 4649 5645 222c   "Five", "FIVE",
+000004c0: 2022 6669 7665 7322 2c20 2246 6976 6573   "fives", "Fives
+000004d0: 222c 2022 4649 5645 5322 5d0a 2020 2020  ", "FIVES"].    
+000004e0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+000004f0: 7369 7822 3a20 7b0a 2020 2020 2020 2020  six": {.        
+00000500: 2020 2020 2274 7970 6522 3a20 2264 6967      "type": "dig
+00000510: 6974 7322 2c0a 2020 2020 2020 2020 2020  its",.          
+00000520: 2020 2276 616c 7565 223a 2036 2e30 2c0a    "value": 6.0,.
+00000530: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
+00000540: 6d73 223a 205b 2273 6978 222c 2022 5369  ms": ["six", "Si
+00000550: 7822 2c20 2253 4958 222c 2022 7369 7865  x", "SIX", "sixe
+00000560: 7322 2c20 2253 6978 6573 222c 2022 5349  s", "Sixes", "SI
+00000570: 5845 5322 5d0a 2020 2020 2020 2020 7d2c  XES"].        },
+00000580: 0a20 2020 2020 2020 2022 7365 7665 6e22  .        "seven"
+00000590: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000005a0: 2274 7970 6522 3a20 2264 6967 6974 7322  "type": "digits"
+000005b0: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+000005c0: 616c 7565 223a 2037 2e30 2c0a 2020 2020  alue": 7.0,.    
+000005d0: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+000005e0: 205b 2273 6576 656e 222c 2022 5365 7665   ["seven", "Seve
+000005f0: 6e22 2c20 2253 4556 454e 222c 2022 7365  n", "SEVEN", "se
+00000600: 7665 6e73 222c 2022 5365 7665 6e73 222c  vens", "Sevens",
+00000610: 2022 5345 5645 4e53 225d 0a20 2020 2020   "SEVENS"].     
+00000620: 2020 207d 2c0a 2020 2020 2020 2020 2265     },.        "e
+00000630: 6967 6874 223a 207b 0a20 2020 2020 2020  ight": {.       
+00000640: 2020 2020 2022 7479 7065 223a 2022 6469       "type": "di
+00000650: 6769 7473 222c 0a20 2020 2020 2020 2020  gits",.         
+00000660: 2020 2022 7661 6c75 6522 3a20 382e 302c     "value": 8.0,
+00000670: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00000680: 726d 7322 3a20 5b22 6569 6768 7422 2c20  rms": ["eight", 
+00000690: 2245 6967 6874 222c 2022 4549 4748 5422  "Eight", "EIGHT"
+000006a0: 2c20 2265 6967 6874 7322 2c20 2245 6967  , "eights", "Eig
+000006b0: 6874 7322 2c20 2245 4947 4854 5322 5d0a  hts", "EIGHTS"].
+000006c0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000006d0: 2020 2022 6e69 6e65 223a 207b 0a20 2020     "nine": {.   
+000006e0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000006f0: 2022 6469 6769 7473 222c 0a20 2020 2020   "digits",.     
+00000700: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00000710: 392e 302c 0a20 2020 2020 2020 2020 2020  9.0,.           
+00000720: 2022 7465 726d 7322 3a20 5b22 6e69 6e65   "terms": ["nine
+00000730: 222c 2022 4e69 6e65 222c 2022 4e49 4e45  ", "Nine", "NINE
+00000740: 222c 2022 6e69 6e65 7322 2c20 224e 696e  ", "nines", "Nin
+00000750: 6573 222c 2022 4e49 4e45 5322 5d0a 2020  es", "NINES"].  
+00000760: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000770: 2022 7465 6e22 3a20 7b0a 2020 2020 2020   "ten": {.      
+00000780: 2020 2020 2020 2274 7970 6522 3a20 2274        "type": "t
+00000790: 6565 6e73 222c 0a20 2020 2020 2020 2020  eens",.         
+000007a0: 2020 2022 7661 6c75 6522 3a20 3130 2e30     "value": 10.0
+000007b0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+000007c0: 6572 6d73 223a 205b 2274 656e 222c 2022  erms": ["ten", "
+000007d0: 5465 6e22 2c20 2254 454e 222c 2022 7465  Ten", "TEN", "te
+000007e0: 6e73 222c 2022 5465 6e73 222c 2022 5445  ns", "Tens", "TE
+000007f0: 4e53 225d 0a20 2020 2020 2020 207d 2c0a  NS"].        },.
+00000800: 2020 2020 2020 2020 2265 6c65 7665 6e22          "eleven"
+00000810: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00000820: 2274 7970 6522 3a20 2274 6565 6e73 222c  "type": "teens",
+00000830: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00000840: 6c75 6522 3a20 3131 2e30 2c0a 2020 2020  lue": 11.0,.    
+00000850: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00000860: 205b 2265 6c65 7665 6e22 2c20 2245 6c65   ["eleven", "Ele
+00000870: 7665 6e22 2c20 2245 4c45 5645 4e22 2c20  ven", "ELEVEN", 
+00000880: 2265 6c65 7665 6e73 222c 2022 456c 6576  "elevens", "Elev
+00000890: 656e 7322 2c20 2245 4c45 5645 4e53 225d  ens", "ELEVENS"]
+000008a0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000008b0: 2020 2020 2274 7765 6c76 6522 3a20 7b0a      "twelve": {.
+000008c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000008d0: 6522 3a20 2274 6565 6e73 222c 0a20 2020  e": "teens",.   
+000008e0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+000008f0: 3a20 3132 2e30 2c0a 2020 2020 2020 2020  : 12.0,.        
+00000900: 2020 2020 2274 6572 6d73 223a 205b 2274      "terms": ["t
+00000910: 7765 6c76 6522 2c20 2254 7765 6c76 6522  welve", "Twelve"
+00000920: 2c20 2254 5745 4c56 4522 2c20 2274 7765  , "TWELVE", "twe
+00000930: 6c76 6573 222c 2022 5477 656c 7665 7322  lves", "Twelves"
+00000940: 2c20 2254 5745 4c56 4553 225d 0a20 2020  , "TWELVES"].   
+00000950: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000960: 2274 6869 7274 6565 6e22 3a20 7b0a 2020  "thirteen": {.  
+00000970: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00000980: 3a20 2274 6565 6e73 222c 0a20 2020 2020  : "teens",.     
+00000990: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000009a0: 3133 2e30 2c0a 2020 2020 2020 2020 2020  13.0,.          
+000009b0: 2020 2274 6572 6d73 223a 205b 2274 6869    "terms": ["thi
+000009c0: 7274 6565 6e22 2c20 2254 6869 7274 6565  rteen", "Thirtee
+000009d0: 6e22 2c20 2254 4849 5254 4545 4e22 2c20  n", "THIRTEEN", 
+000009e0: 2274 6869 7274 6565 6e73 222c 2022 5468  "thirteens", "Th
+000009f0: 6972 7465 656e 7322 2c20 2254 4849 5254  irteens", "THIRT
+00000a00: 4545 4e53 225d 0a20 2020 2020 2020 207d  EENS"].        }
+00000a10: 2c0a 2020 2020 2020 2020 2266 6f75 7274  ,.        "fourt
+00000a20: 6565 6e22 3a20 7b0a 2020 2020 2020 2020  een": {.        
+00000a30: 2020 2020 2274 7970 6522 3a20 2274 6565      "type": "tee
+00000a40: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
+00000a50: 2022 7661 6c75 6522 3a20 3134 2e30 2c0a   "value": 14.0,.
+00000a60: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
+00000a70: 6d73 223a 205b 2266 6f75 7274 6565 6e22  ms": ["fourteen"
+00000a80: 2c20 2246 6f75 7274 6565 6e22 2c20 2246  , "Fourteen", "F
+00000a90: 4f55 5254 4545 4e22 2c20 2266 6f75 7274  OURTEEN", "fourt
+00000aa0: 6565 6e73 222c 2022 466f 7572 7465 656e  eens", "Fourteen
+00000ab0: 7322 2c20 2246 4f55 5254 4545 4e53 225d  s", "FOURTEENS"]
+00000ac0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00000ad0: 2020 2020 2266 6966 7465 656e 223a 207b      "fifteen": {
+00000ae0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+00000af0: 7065 223a 2022 7465 656e 7322 2c0a 2020  pe": "teens",.  
+00000b00: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00000b10: 223a 2031 352e 302c 0a20 2020 2020 2020  ": 15.0,.       
+00000b20: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
+00000b30: 6669 6674 6565 6e22 2c20 2246 6966 7465  fifteen", "Fifte
+00000b40: 656e 222c 2022 4649 4654 4545 4e22 2c20  en", "FIFTEEN", 
+00000b50: 2266 6966 7465 656e 7322 2c20 2246 6966  "fifteens", "Fif
+00000b60: 7465 656e 7322 2c20 2246 4946 5445 454e  teens", "FIFTEEN
+00000b70: 5322 5d0a 2020 2020 2020 2020 7d2c 0a20  S"].        },. 
+00000b80: 2020 2020 2020 2022 7369 7874 6565 6e22         "sixteen"
+00000b90: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00000ba0: 2274 7970 6522 3a20 2274 6565 6e73 222c  "type": "teens",
+00000bb0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00000bc0: 6c75 6522 3a20 3136 2e30 2c0a 2020 2020  lue": 16.0,.    
+00000bd0: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00000be0: 205b 2273 6978 7465 656e 222c 2022 5369   ["sixteen", "Si
+00000bf0: 7874 6565 6e22 2c20 2253 4958 5445 454e  xteen", "SIXTEEN
+00000c00: 222c 2022 7369 7874 6565 6e73 222c 2022  ", "sixteens", "
+00000c10: 5369 7874 6565 6e73 222c 2022 5349 5854  Sixteens", "SIXT
+00000c20: 4545 4e53 225d 0a20 2020 2020 2020 207d  EENS"].        }
+00000c30: 2c0a 2020 2020 2020 2020 2273 6576 656e  ,.        "seven
+00000c40: 7465 656e 223a 207b 0a20 2020 2020 2020  teen": {.       
+00000c50: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
+00000c60: 656e 7322 2c0a 2020 2020 2020 2020 2020  ens",.          
+00000c70: 2020 2276 616c 7565 223a 2031 372e 302c    "value": 17.0,
+00000c80: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00000c90: 726d 7322 3a20 5b22 7365 7665 6e74 6565  rms": ["seventee
+00000ca0: 6e22 2c20 2253 6576 656e 7465 656e 222c  n", "Seventeen",
+00000cb0: 2022 5345 5645 4e54 4545 4e22 2c20 2273   "SEVENTEEN", "s
+00000cc0: 6576 656e 7465 656e 7322 2c20 2253 6576  eventeens", "Sev
+00000cd0: 656e 7465 656e 7322 2c20 2253 4556 454e  enteens", "SEVEN
+00000ce0: 5445 454e 5322 5d0a 2020 2020 2020 2020  TEENS"].        
+00000cf0: 7d2c 0a20 2020 2020 2020 2022 6569 6768  },.        "eigh
+00000d00: 7465 656e 223a 207b 0a20 2020 2020 2020  teen": {.       
+00000d10: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
+00000d20: 656e 7322 2c0a 2020 2020 2020 2020 2020  ens",.          
+00000d30: 2020 2276 616c 7565 223a 2031 382e 302c    "value": 18.0,
+00000d40: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00000d50: 726d 7322 3a20 5b22 6569 6768 7465 656e  rms": ["eighteen
+00000d60: 222c 2022 4569 6768 7465 656e 222c 2022  ", "Eighteen", "
+00000d70: 4549 4748 5445 454e 222c 2022 6569 6768  EIGHTEEN", "eigh
+00000d80: 7465 656e 7322 2c20 2245 6967 6874 6565  teens", "Eightee
+00000d90: 6e73 222c 2022 4549 4748 5445 454e 5322  ns", "EIGHTEENS"
+00000da0: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00000db0: 2020 2020 2022 6e69 6e65 7465 656e 223a       "nineteen":
+00000dc0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000dd0: 7479 7065 223a 2022 7465 656e 7322 2c0a  type": "teens",.
+00000de0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00000df0: 7565 223a 2031 392e 302c 0a20 2020 2020  ue": 19.0,.     
+00000e00: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00000e10: 5b22 6e69 6e65 7465 656e 222c 2022 4e69  ["nineteen", "Ni
+00000e20: 6e65 7465 656e 222c 2022 4e49 4e45 5445  neteen", "NINETE
+00000e30: 454e 222c 2022 6e69 6e65 7465 656e 7322  EN", "nineteens"
+00000e40: 2c20 224e 696e 6574 6565 6e73 222c 2022  , "Nineteens", "
+00000e50: 4e49 4e45 5445 454e 5322 5d0a 2020 2020  NINETEENS"].    
+00000e60: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000e70: 7477 656e 7479 223a 207b 0a20 2020 2020  twenty": {.     
+00000e80: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000e90: 7465 6e73 222c 0a20 2020 2020 2020 2020  tens",.         
+00000ea0: 2020 2022 7661 6c75 6522 3a20 3230 2e30     "value": 20.0
+00000eb0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00000ec0: 6572 6d73 223a 205b 2274 7765 6e74 7922  erms": ["twenty"
+00000ed0: 2c20 2254 7765 6e74 7922 2c20 2254 5745  , "Twenty", "TWE
+00000ee0: 4e54 5922 2c20 2274 7765 6e74 6965 7322  NTY", "twenties"
+00000ef0: 2c20 2254 7765 6e74 6965 7322 2c20 2254  , "Twenties", "T
+00000f00: 5745 4e54 4945 5322 5d0a 2020 2020 2020  WENTIES"].      
+00000f10: 2020 7d2c 0a20 2020 2020 2020 2022 7468    },.        "th
+00000f20: 6972 7479 223a 207b 0a20 2020 2020 2020  irty": {.       
+00000f30: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
+00000f40: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
+00000f50: 2022 7661 6c75 6522 3a20 3330 2e30 2c0a   "value": 30.0,.
+00000f60: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
+00000f70: 6d73 223a 205b 2274 6869 7274 7922 2c20  ms": ["thirty", 
+00000f80: 2254 6869 7274 7922 2c20 2254 4849 5254  "Thirty", "THIRT
+00000f90: 5922 2c20 2274 6869 7274 6965 7322 2c20  Y", "thirties", 
+00000fa0: 2254 6869 7274 6965 7322 2c20 2254 4849  "Thirties", "THI
+00000fb0: 5254 4945 5322 5d0a 2020 2020 2020 2020  RTIES"].        
+00000fc0: 7d2c 0a20 2020 2020 2020 2022 666f 7274  },.        "fort
+00000fd0: 7922 3a20 7b0a 2020 2020 2020 2020 2020  y": {.          
+00000fe0: 2020 2274 7970 6522 3a20 2274 656e 7322    "type": "tens"
+00000ff0: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00001000: 616c 7565 223a 2034 302e 302c 0a20 2020  alue": 40.0,.   
+00001010: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+00001020: 3a20 5b22 666f 7274 7922 2c20 2246 6f72  : ["forty", "For
+00001030: 7479 222c 2022 464f 5254 5922 2c20 2266  ty", "FORTY", "f
+00001040: 6f72 7469 6573 222c 2022 466f 7274 6965  orties", "Fortie
+00001050: 7322 2c20 2246 4f52 5449 4553 222c 2022  s", "FORTIES", "
+00001060: 666f 7572 7479 222c 2022 466f 7572 7479  fourty", "Fourty
+00001070: 222c 2022 464f 5552 5459 222c 2022 666f  ", "FOURTY", "fo
+00001080: 7572 7469 6573 222c 2022 466f 7572 7469  urties", "Fourti
+00001090: 6573 222c 2022 464f 5552 5449 4553 225d  es", "FOURTIES"]
+000010a0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000010b0: 2020 2020 2266 6966 7479 223a 207b 0a20      "fifty": {. 
+000010c0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000010d0: 223a 2022 7465 6e73 222c 0a20 2020 2020  ": "tens",.     
+000010e0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000010f0: 3530 2e30 2c0a 2020 2020 2020 2020 2020  50.0,.          
+00001100: 2020 2274 6572 6d73 223a 205b 2266 6966    "terms": ["fif
+00001110: 7479 222c 2022 4669 6674 7922 2c20 2246  ty", "Fifty", "F
+00001120: 4946 5459 222c 2022 6669 6674 6965 7322  IFTY", "fifties"
+00001130: 2c20 2246 6966 7469 6573 222c 2022 4649  , "Fifties", "FI
+00001140: 4654 4945 5322 5d0a 2020 2020 2020 2020  FTIES"].        
+00001150: 7d2c 0a20 2020 2020 2020 2022 7369 7874  },.        "sixt
+00001160: 7922 3a20 7b0a 2020 2020 2020 2020 2020  y": {.          
+00001170: 2020 2274 7970 6522 3a20 2274 656e 7322    "type": "tens"
+00001180: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00001190: 616c 7565 223a 2036 302e 302c 0a20 2020  alue": 60.0,.   
+000011a0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+000011b0: 3a20 5b22 7369 7874 7922 2c20 2253 6978  : ["sixty", "Six
+000011c0: 7479 222c 2022 5349 5854 5922 2c20 2273  ty", "SIXTY", "s
+000011d0: 6978 7469 6573 222c 2022 5369 7874 6965  ixties", "Sixtie
+000011e0: 7322 2c20 2253 4958 5449 4553 225d 0a20  s", "SIXTIES"]. 
+000011f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001200: 2020 2273 6576 656e 7479 223a 207b 0a20    "seventy": {. 
+00001210: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00001220: 223a 2022 7465 6e73 222c 0a20 2020 2020  ": "tens",.     
+00001230: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00001240: 3730 2e30 2c0a 2020 2020 2020 2020 2020  70.0,.          
+00001250: 2020 2274 6572 6d73 223a 205b 2273 6576    "terms": ["sev
+00001260: 656e 7479 222c 2022 5365 7665 6e74 7922  enty", "Seventy"
+00001270: 2c20 2253 4556 454e 5459 222c 2022 7365  , "SEVENTY", "se
+00001280: 7665 6e74 6965 7322 2c20 2253 6576 656e  venties", "Seven
+00001290: 7469 6573 222c 2022 5345 5645 4e54 4945  ties", "SEVENTIE
+000012a0: 5322 5d0a 2020 2020 2020 2020 7d2c 0a20  S"].        },. 
+000012b0: 2020 2020 2020 2022 6569 6768 7479 223a         "eighty":
+000012c0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000012d0: 7479 7065 223a 2022 7465 6e73 222c 0a20  type": "tens",. 
+000012e0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+000012f0: 6522 3a20 3830 2e30 2c0a 2020 2020 2020  e": 80.0,.      
+00001300: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
+00001310: 2265 6967 6874 7922 2c20 2245 6967 6874  "eighty", "Eight
+00001320: 7922 2c20 2245 4947 4854 5922 2c20 2265  y", "EIGHTY", "e
+00001330: 6967 6874 6965 7322 2c20 2245 6967 6874  ighties", "Eight
+00001340: 6965 7322 2c20 2245 4947 4854 4945 5322  ies", "EIGHTIES"
+00001350: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00001360: 2020 2020 2022 6e69 6e65 7479 223a 207b       "ninety": {
+00001370: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+00001380: 7065 223a 2022 7465 6e73 222c 0a20 2020  pe": "tens",.   
+00001390: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+000013a0: 3a20 3930 2e30 2c0a 2020 2020 2020 2020  : 90.0,.        
+000013b0: 2020 2020 2274 6572 6d73 223a 205b 226e      "terms": ["n
+000013c0: 696e 6574 7922 2c20 224e 696e 6574 7922  inety", "Ninety"
+000013d0: 2c20 224e 494e 4554 5922 2c20 226e 696e  , "NINETY", "nin
+000013e0: 6574 6965 7322 2c20 224e 696e 6574 6965  eties", "Ninetie
+000013f0: 7322 2c20 224e 494e 4554 4945 5322 5d0a  s", "NINETIES"].
+00001400: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001410: 2020 2022 6875 6e64 7265 6422 3a20 7b0a     "hundred": {.
+00001420: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00001430: 6522 3a20 2274 686f 7573 616e 6473 222c  e": "thousands",
+00001440: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00001450: 6c75 6522 3a20 3130 302e 302c 0a20 2020  lue": 100.0,.   
+00001460: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+00001470: 3a20 5b22 6875 6e64 7265 6422 2c20 2248  : ["hundred", "H
+00001480: 756e 6472 6564 222c 2022 4855 4e44 5245  undred", "HUNDRE
+00001490: 4422 2c20 2268 756e 6472 6564 7322 2c20  D", "hundreds", 
+000014a0: 2248 756e 6472 6564 7322 2c20 2248 554e  "Hundreds", "HUN
+000014b0: 4452 4544 5322 5d0a 2020 2020 2020 2020  DREDS"].        
+000014c0: 7d2c 0a20 2020 2020 2020 2022 7468 6f75  },.        "thou
+000014d0: 7361 6e64 223a 207b 0a20 2020 2020 2020  sand": {.       
+000014e0: 2020 2020 2022 7479 7065 223a 2022 7468       "type": "th
+000014f0: 6f75 7361 6e64 7322 2c0a 2020 2020 2020  ousands",.      
+00001500: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
+00001510: 3030 302e 302c 0a20 2020 2020 2020 2020  000.0,.         
+00001520: 2020 2022 7465 726d 7322 3a20 5b22 7468     "terms": ["th
+00001530: 6f75 7361 6e64 222c 2022 5468 6f75 7361  ousand", "Thousa
+00001540: 6e64 222c 2022 5448 4f55 5341 4e44 222c  nd", "THOUSAND",
+00001550: 2022 7468 6f75 7361 6e64 7322 2c20 2254   "thousands", "T
+00001560: 686f 7573 616e 6473 222c 2022 5448 4f55  housands", "THOU
+00001570: 5341 4e44 5322 5d0a 2020 2020 2020 2020  SANDS"].        
+00001580: 7d2c 0a20 2020 2020 2020 2022 6d69 6c6c  },.        "mill
+00001590: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
+000015a0: 2020 2020 2274 7970 6522 3a20 2274 686f      "type": "tho
+000015b0: 7573 616e 6473 222c 0a20 2020 2020 2020  usands",.       
+000015c0: 2020 2020 2022 7661 6c75 6522 3a20 3130       "value": 10
+000015d0: 3030 3030 302e 302c 0a20 2020 2020 2020  00000.0,.       
+000015e0: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
+000015f0: 6d69 6c6c 696f 6e22 2c20 224d 696c 6c69  million", "Milli
+00001600: 6f6e 222c 2022 4d49 4c4c 494f 4e22 2c20  on", "MILLION", 
+00001610: 226d 696c 6c69 6f6e 7322 2c20 224d 696c  "millions", "Mil
+00001620: 6c69 6f6e 7322 2c20 224d 494c 4c49 4f4e  lions", "MILLION
+00001630: 5322 5d0a 2020 2020 2020 2020 7d2c 0a20  S"].        },. 
+00001640: 2020 2020 2020 2022 6269 6c6c 696f 6e22         "billion"
+00001650: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001660: 2274 7970 6522 3a20 2274 686f 7573 616e  "type": "thousan
+00001670: 6473 222c 0a20 2020 2020 2020 2020 2020  ds",.           
+00001680: 2022 7661 6c75 6522 3a20 3130 3030 3030   "value": 100000
+00001690: 3030 3030 2e30 2c0a 2020 2020 2020 2020  0000.0,.        
+000016a0: 2020 2020 2274 6572 6d73 223a 205b 2262      "terms": ["b
+000016b0: 696c 6c69 6f6e 222c 2022 4269 6c6c 696f  illion", "Billio
+000016c0: 6e22 2c20 2242 494c 4c49 4f4e 222c 2022  n", "BILLION", "
+000016d0: 6269 6c6c 696f 6e73 222c 2022 4269 6c6c  billions", "Bill
+000016e0: 696f 6e73 222c 2022 4249 4c4c 494f 4e53  ions", "BILLIONS
+000016f0: 225d 0a20 2020 2020 2020 207d 2c0a 2020  "].        },.  
+00001700: 2020 2020 2020 2274 7269 6c6c 696f 6e22        "trillion"
+00001710: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001720: 2274 7970 6522 3a20 2274 686f 7573 616e  "type": "thousan
+00001730: 6473 222c 0a20 2020 2020 2020 2020 2020  ds",.           
+00001740: 2022 7661 6c75 6522 3a20 3130 3030 3030   "value": 100000
+00001750: 3030 3030 3030 302e 302c 0a20 2020 2020  0000000.0,.     
+00001760: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00001770: 5b22 7472 696c 6c69 6f6e 222c 2022 5472  ["trillion", "Tr
+00001780: 696c 6c69 6f6e 222c 2022 5452 494c 4c49  illion", "TRILLI
+00001790: 4f4e 222c 2022 7472 696c 6c69 6f6e 7322  ON", "trillions"
+000017a0: 2c20 2254 7269 6c6c 696f 6e73 222c 2022  , "Trillions", "
+000017b0: 5452 494c 4c49 4f4e 5322 5d0a 2020 2020  TRILLIONS"].    
+000017c0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+000017d0: 6675 6c6c 223a 207b 0a20 2020 2020 2020  full": {.       
+000017e0: 2020 2020 2022 7479 7065 223a 2022 6d6f       "type": "mo
+000017f0: 6469 6669 6572 7322 2c0a 2020 2020 2020  difiers",.      
+00001800: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
+00001810: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00001820: 2274 6572 6d73 223a 205b 2266 756c 6c22  "terms": ["full"
+00001830: 2c20 2246 756c 6c22 2c20 2246 554c 4c22  , "Full", "FULL"
+00001840: 2c20 2277 686f 6c65 222c 2022 5768 6f6c  , "whole", "Whol
+00001850: 6522 2c20 2257 484f 4c45 225d 0a20 2020  e", "WHOLE"].   
+00001860: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001870: 2268 616c 6622 3a20 7b0a 2020 2020 2020  "half": {.      
+00001880: 2020 2020 2020 2274 7970 6522 3a20 226d        "type": "m
+00001890: 6f64 6966 6965 7273 222c 0a20 2020 2020  odifiers",.     
+000018a0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000018b0: 302e 352c 0a20 2020 2020 2020 2020 2020  0.5,.           
+000018c0: 2022 7465 726d 7322 3a20 5b22 6861 6c66   "terms": ["half
+000018d0: 222c 2022 4861 6c66 222c 2022 4841 4c46  ", "Half", "HALF
+000018e0: 222c 2022 6861 6c76 6573 222c 2022 4861  ", "halves", "Ha
+000018f0: 6c76 6573 222c 2022 4841 4c56 4553 225d  lves", "HALVES"]
+00001900: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001910: 2020 2020 2274 6869 7264 223a 207b 0a20      "third": {. 
+00001920: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00001930: 223a 2022 6d6f 6469 6669 6572 7322 2c0a  ": "modifiers",.
+00001940: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00001950: 7565 223a 2022 312f 3322 2c0a 2020 2020  ue": "1/3",.    
+00001960: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00001970: 205b 2274 6869 7264 222c 2022 5468 6972   ["third", "Thir
+00001980: 6422 2c20 2254 4849 5244 222c 2022 7468  d", "THIRD", "th
+00001990: 6972 6473 222c 2022 5468 6972 6473 222c  irds", "Thirds",
+000019a0: 2022 5448 4952 4453 225d 0a20 2020 2020   "THIRDS"].     
+000019b0: 2020 207d 2c0a 2020 2020 2020 2020 2271     },.        "q
+000019c0: 7561 7274 6572 223a 207b 0a20 2020 2020  uarter": {.     
+000019d0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+000019e0: 6d6f 6469 6669 6572 7322 2c0a 2020 2020  modifiers",.    
+000019f0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+00001a00: 2030 2e32 352c 0a20 2020 2020 2020 2020   0.25,.         
+00001a10: 2020 2022 7465 726d 7322 3a20 5b22 7175     "terms": ["qu
+00001a20: 6172 7465 7222 2c20 2251 7561 7274 6572  arter", "Quarter
+00001a30: 222c 2022 5155 4152 5445 5222 2c20 2271  ", "QUARTER", "q
+00001a40: 7561 7274 6572 7322 2c20 2251 7561 7274  uarters", "Quart
+00001a50: 6572 7322 2c20 2251 5541 5254 4552 5322  ers", "QUARTERS"
+00001a60: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00001a70: 2020 2020 2022 6d75 6c74 6970 6c69 6572       "multiplier
+00001a80: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00001a90: 2022 7479 7065 223a 2022 6d75 6c74 6970   "type": "multip
+00001aa0: 6c69 6572 222c 0a20 2020 2020 2020 2020  lier",.         
+00001ab0: 2020 2022 7661 6c75 6522 3a20 2d31 2e30     "value": -1.0
+00001ac0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00001ad0: 6572 6d73 223a 205b 226f 6622 2c20 224f  erms": ["of", "O
+00001ae0: 6622 2c20 224f 4622 5d0a 2020 2020 2020  f", "OF"].      
+00001af0: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
+00001b00: 7363 616c 6573 223a 207b 0a20 2020 2020  scales": {.     
+00001b10: 2020 2022 6d69 6c6c 6973 6563 6f6e 6422     "millisecond"
+00001b20: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001b30: 2273 6361 6c65 223a 2030 2e30 3031 2c0a  "scale": 0.001,.
+00001b40: 2020 2020 2020 2020 2020 2020 2273 696e              "sin
+00001b50: 6775 6c61 7222 3a20 226d 696c 6c69 7365  gular": "millise
+00001b60: 636f 6e64 222c 0a20 2020 2020 2020 2020  cond",.         
+00001b70: 2020 2022 706c 7572 616c 223a 2022 6d69     "plural": "mi
+00001b80: 6c6c 6973 6563 6f6e 6473 222c 0a20 2020  lliseconds",.   
+00001b90: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+00001ba0: 3a20 5b22 6d73 222c 2022 4d73 222c 2022  : ["ms", "Ms", "
+00001bb0: 4d53 222c 2022 6d69 6c6c 6973 6563 6f6e  MS", "millisecon
+00001bc0: 6422 2c20 224d 696c 6c69 7365 636f 6e64  d", "Millisecond
+00001bd0: 222c 2022 4d49 4c4c 4953 4543 4f4e 4422  ", "MILLISECOND"
+00001be0: 2c20 226d 696c 6c69 7365 636f 6e64 7322  , "milliseconds"
+00001bf0: 2c20 224d 696c 6c69 7365 636f 6e64 7322  , "Milliseconds"
+00001c00: 2c20 224d 494c 4c49 5345 434f 4e44 5322  , "MILLISECONDS"
+00001c10: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00001c20: 2020 2020 2022 7365 636f 6e64 223a 207b       "second": {
+00001c30: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
+00001c40: 616c 6522 3a20 312e 302c 0a20 2020 2020  ale": 1.0,.     
+00001c50: 2020 2020 2020 2022 7369 6e67 756c 6172         "singular
+00001c60: 223a 2022 7365 636f 6e64 222c 0a20 2020  ": "second",.   
+00001c70: 2020 2020 2020 2020 2022 706c 7572 616c           "plural
+00001c80: 223a 2022 7365 636f 6e64 7322 2c0a 2020  ": "seconds",.  
+00001c90: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
+00001ca0: 223a 205b 2273 222c 2022 5322 2c20 2273  ": ["s", "S", "s
+00001cb0: 6563 222c 2022 5365 6322 2c20 2253 4543  ec", "Sec", "SEC
+00001cc0: 222c 2022 7365 6373 222c 2022 5365 6373  ", "secs", "Secs
+00001cd0: 222c 2022 5345 4353 222c 2022 7365 636f  ", "SECS", "seco
+00001ce0: 6e64 222c 2022 5365 636f 6e64 222c 2022  nd", "Second", "
+00001cf0: 5345 434f 4e44 222c 2022 7365 636f 6e64  SECOND", "second
+00001d00: 7322 2c20 2253 6563 6f6e 6473 222c 2022  s", "Seconds", "
+00001d10: 5345 434f 4e44 5322 5d0a 2020 2020 2020  SECONDS"].      
+00001d20: 2020 7d2c 0a20 2020 2020 2020 2022 6d69    },.        "mi
+00001d30: 6e75 7465 223a 207b 0a20 2020 2020 2020  nute": {.       
+00001d40: 2020 2020 2022 7363 616c 6522 3a20 3630       "scale": 60
+00001d50: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00001d60: 2273 696e 6775 6c61 7222 3a20 226d 696e  "singular": "min
+00001d70: 7574 6522 2c0a 2020 2020 2020 2020 2020  ute",.          
+00001d80: 2020 2270 6c75 7261 6c22 3a20 226d 696e    "plural": "min
+00001d90: 7574 6573 222c 0a20 2020 2020 2020 2020  utes",.         
+00001da0: 2020 2022 7465 726d 7322 3a20 5b22 6d22     "terms": ["m"
+00001db0: 2c20 226d 696e 222c 2022 4d69 6e22 2c20  , "min", "Min", 
+00001dc0: 224d 494e 222c 2022 6d69 6e73 222c 2022  "MIN", "mins", "
+00001dd0: 4d69 6e73 222c 2022 4d49 4e53 222c 2022  Mins", "MINS", "
+00001de0: 6d69 6e75 7465 222c 2022 4d69 6e75 7465  minute", "Minute
+00001df0: 222c 2022 4d49 4e55 5445 222c 2022 6d69  ", "MINUTE", "mi
+00001e00: 6e75 7465 7322 2c20 224d 696e 7574 6573  nutes", "Minutes
+00001e10: 222c 2022 4d49 4e55 5445 5322 5d0a 2020  ", "MINUTES"].  
+00001e20: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001e30: 2022 686f 7572 223a 207b 0a20 2020 2020   "hour": {.     
+00001e40: 2020 2020 2020 2022 7363 616c 6522 3a20         "scale": 
+00001e50: 3336 3030 2e30 2c0a 2020 2020 2020 2020  3600.0,.        
+00001e60: 2020 2020 2273 696e 6775 6c61 7222 3a20      "singular": 
+00001e70: 2268 6f75 7222 2c0a 2020 2020 2020 2020  "hour",.        
+00001e80: 2020 2020 2270 6c75 7261 6c22 3a20 2268      "plural": "h
+00001e90: 6f75 7273 222c 0a20 2020 2020 2020 2020  ours",.         
+00001ea0: 2020 2022 7465 726d 7322 3a20 5b22 6822     "terms": ["h"
+00001eb0: 2c20 2248 222c 2022 6872 222c 2022 4872  , "H", "hr", "Hr
+00001ec0: 222c 2022 4852 222c 2022 6872 7322 2c20  ", "HR", "hrs", 
+00001ed0: 2248 7273 222c 2022 4852 5322 2c20 2268  "Hrs", "HRS", "h
+00001ee0: 6f75 7222 2c20 2248 6f75 7222 2c20 2248  our", "Hour", "H
+00001ef0: 4f55 5222 2c20 2268 6f75 7273 222c 2022  OUR", "hours", "
+00001f00: 486f 7572 7322 2c20 2248 4f55 5253 225d  Hours", "HOURS"]
+00001f10: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001f20: 2020 2020 2264 6179 223a 207b 0a20 2020      "day": {.   
+00001f30: 2020 2020 2020 2020 2022 7363 616c 6522           "scale"
+00001f40: 3a20 3836 3430 302e 302c 0a20 2020 2020  : 86400.0,.     
+00001f50: 2020 2020 2020 2022 7369 6e67 756c 6172         "singular
+00001f60: 223a 2022 6461 7922 2c0a 2020 2020 2020  ": "day",.      
+00001f70: 2020 2020 2020 2270 6c75 7261 6c22 3a20        "plural": 
+00001f80: 2264 6179 7322 2c0a 2020 2020 2020 2020  "days",.        
+00001f90: 2020 2020 2274 6572 6d73 223a 205b 2264      "terms": ["d
+00001fa0: 222c 2022 6461 7922 2c20 2244 6179 222c  ", "day", "Day",
+00001fb0: 2022 4441 5922 2c20 2264 6179 7322 2c20   "DAY", "days", 
+00001fc0: 2244 6179 7322 2c20 2244 4159 5322 2c20  "Days", "DAYS", 
+00001fd0: 2264 7922 2c20 2244 7922 2c20 2244 5922  "dy", "Dy", "DY"
+00001fe0: 2c20 2264 7973 222c 2022 4479 7322 2c20  , "dys", "Dys", 
+00001ff0: 2244 5953 225d 0a20 2020 2020 2020 207d  "DYS"].        }
+00002000: 2c0a 2020 2020 2020 2020 2277 6565 6b22  ,.        "week"
+00002010: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002020: 2273 6361 6c65 223a 2036 3034 3830 302e  "scale": 604800.
+00002030: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002040: 7369 6e67 756c 6172 223a 2022 7765 656b  singular": "week
+00002050: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002060: 706c 7572 616c 223a 2022 7765 656b 7322  plural": "weeks"
+00002070: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00002080: 6572 6d73 223a 205b 2277 222c 2022 5722  erms": ["w", "W"
+00002090: 2c20 2277 6b22 2c20 2257 6b22 2c20 2257  , "wk", "Wk", "W
+000020a0: 4b22 2c20 2277 6b73 222c 2022 576b 7322  K", "wks", "Wks"
+000020b0: 2c20 2257 4b53 222c 2022 7765 656b 222c  , "WKS", "week",
+000020c0: 2022 5765 656b 222c 2022 5745 454b 222c   "Week", "WEEK",
+000020d0: 2022 7765 656b 7322 2c20 2257 6565 6b73   "weeks", "Weeks
+000020e0: 222c 2022 5745 454b 5322 5d0a 2020 2020  ", "WEEKS"].    
+000020f0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00002100: 6d6f 6e74 6822 3a20 7b0a 2020 2020 2020  month": {.      
+00002110: 2020 2020 2020 2273 6361 6c65 223a 2032        "scale": 2
+00002120: 3633 3532 3030 2e30 2c0a 2020 2020 2020  635200.0,.      
+00002130: 2020 2020 2020 2273 696e 6775 6c61 7222        "singular"
+00002140: 3a20 226d 6f6e 7468 222c 0a20 2020 2020  : "month",.     
+00002150: 2020 2020 2020 2022 706c 7572 616c 223a         "plural":
+00002160: 2022 6d6f 6e74 6873 222c 0a20 2020 2020   "months",.     
+00002170: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00002180: 5b22 4d22 2c20 226d 6f6e 7468 222c 2022  ["M", "month", "
+00002190: 4d6f 6e74 6822 2c20 224d 4f4e 5448 222c  Month", "MONTH",
+000021a0: 2022 6d6f 6e74 6873 222c 2022 4d6f 6e74   "months", "Mont
+000021b0: 6873 222c 2022 4d4f 4e54 4853 222c 2022  hs", "MONTHS", "
+000021c0: 6d6f 222c 2022 4d6f 222c 2022 4d4f 225d  mo", "Mo", "MO"]
+000021d0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000021e0: 2020 2020 2279 6561 7222 3a20 7b0a 2020      "year": {.  
+000021f0: 2020 2020 2020 2020 2020 2273 6361 6c65            "scale
+00002200: 223a 2033 3135 3336 3030 302e 302c 0a20  ": 31536000.0,. 
+00002210: 2020 2020 2020 2020 2020 2022 7369 6e67             "sing
+00002220: 756c 6172 223a 2022 7965 6172 222c 0a20  ular": "year",. 
+00002230: 2020 2020 2020 2020 2020 2022 706c 7572             "plur
+00002240: 616c 223a 2022 7965 6172 7322 2c0a 2020  al": "years",.  
+00002250: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
+00002260: 223a 205b 2279 222c 2022 5922 2c20 2279  ": ["y", "Y", "y
+00002270: 7222 2c20 2259 7222 2c20 2259 5222 2c20  r", "Yr", "YR", 
+00002280: 2279 7273 222c 2022 5972 7322 2c20 2259  "yrs", "Yrs", "Y
+00002290: 5253 222c 2022 7965 6172 222c 2022 5965  RS", "year", "Ye
+000022a0: 6172 222c 2022 5945 4152 222c 2022 7965  ar", "YEAR", "ye
+000022b0: 6172 7322 2c20 2259 6561 7273 222c 2022  ars", "Years", "
+000022c0: 5945 4152 5322 5d0a 2020 2020 2020 2020  YEARS"].        
+000022d0: 7d2c 0a20 2020 2020 2020 2022 6465 6361  },.        "deca
+000022e0: 6465 223a 207b 0a20 2020 2020 2020 2020  de": {.         
+000022f0: 2020 2022 7363 616c 6522 3a20 3331 3533     "scale": 3153
+00002300: 3630 3030 302e 302c 0a20 2020 2020 2020  60000.0,.       
+00002310: 2020 2020 2022 7369 6e67 756c 6172 223a       "singular":
+00002320: 2022 6465 6361 6465 222c 0a20 2020 2020   "decade",.     
+00002330: 2020 2020 2020 2022 706c 7572 616c 223a         "plural":
+00002340: 2022 6465 6361 6465 7322 2c0a 2020 2020   "decades",.    
+00002350: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00002360: 205b 2244 222c 2022 6465 6322 2c20 2244   ["D", "dec", "D
+00002370: 6563 222c 2022 4445 4322 2c20 2264 6563  ec", "DEC", "dec
+00002380: 7322 2c20 2244 6563 7322 2c20 2244 4543  s", "Decs", "DEC
+00002390: 5322 2c20 2264 6563 6164 6522 2c20 2244  S", "decade", "D
+000023a0: 6563 6164 6522 2c20 2244 4543 4144 4522  ecade", "DECADE"
+000023b0: 2c20 2264 6563 6164 6573 222c 2022 4465  , "decades", "De
+000023c0: 6361 6465 7322 2c20 2244 4543 4144 4553  cades", "DECADES
+000023d0: 225d 0a20 2020 2020 2020 207d 2c0a 2020  "].        },.  
+000023e0: 2020 2020 2020 2263 656e 7475 7279 223a        "century":
+000023f0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002400: 7363 616c 6522 3a20 3331 3533 3630 3030  scale": 31536000
+00002410: 3030 2e30 2c0a 2020 2020 2020 2020 2020  00.0,.          
+00002420: 2020 2273 696e 6775 6c61 7222 3a20 2263    "singular": "c
+00002430: 656e 7475 7279 222c 0a20 2020 2020 2020  entury",.       
+00002440: 2020 2020 2022 706c 7572 616c 223a 2022       "plural": "
+00002450: 6365 6e74 7572 6965 7322 2c0a 2020 2020  centuries",.    
+00002460: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00002470: 205b 2263 222c 2022 4322 2c20 2263 656e   ["c", "C", "cen
+00002480: 7475 7279 222c 2022 4365 6e74 7572 7922  tury", "Century"
+00002490: 2c20 2243 454e 5455 5259 222c 2022 6365  , "CENTURY", "ce
+000024a0: 6e74 7572 6965 7322 2c20 2243 656e 7475  nturies", "Centu
+000024b0: 7269 6573 222c 2022 4345 4e54 5552 4945  ries", "CENTURIE
+000024c0: 5322 5d0a 2020 2020 2020 2020 7d0a 2020  S"].        }.  
+000024d0: 2020 7d2c 0a20 2020 2022 6578 7472 615f    },.    "extra_
+000024e0: 6461 7461 223a 207b 0a20 2020 207d 0a7d  data": {.    }.}
+000024f0: 0a                                       .
```

### Comparing `timelength-2.0.1/timelength/locales/spanish.json` & `timelength-2.0.2/timelength/locales/spanish.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -1,777 +1,758 @@
-00000000: 7b0d 0a20 2020 2022 636f 6e6e 6563 746f  {..    "connecto
-00000010: 7273 223a 205b 2220 222c 2022 5c74 222c  rs": [" ", "\t",
-00000020: 2022 2d22 5d2c 0d0a 2020 2020 2273 6567   "-"],..    "seg
-00000030: 6d65 6e74 6f72 7322 3a20 5b22 2c22 2c20  mentors": [",", 
-00000040: 2279 222c 2022 2622 5d2c 0d0a 2020 2020  "y", "&"],..    
-00000050: 2261 6c6c 6f77 6564 5f74 6572 6d73 223a  "allowed_terms":
-00000060: 205b 2221 222c 2022 c2bf 222c 2022 3f22   ["!", "..", "?"
-00000070: 2c20 2227 222c 2022 2e22 2c20 222c 222c  , "'", ".", ",",
-00000080: 2022 6c61 222c 2022 6c65 222c 2022 6c6f   "la", "le", "lo
-00000090: 222c 2022 6c61 7322 2c20 226c 6573 222c  ", "las", "les",
-000000a0: 2022 6c6f 7322 5d2c 0d0a 2020 2020 2264   "los"],..    "d
-000000b0: 6563 696d 616c 5f73 6570 6172 6174 6f72  ecimal_separator
-000000c0: 7322 3a20 5b22 2c22 5d2c 0d0a 2020 2020  s": [","],..    
-000000d0: 2274 686f 7573 616e 645f 7365 7061 7261  "thousand_separa
-000000e0: 746f 7273 223a 205b 222e 222c 2022 2022  tors": [".", " "
-000000f0: 5d2c 0d0a 2020 2020 2270 6172 7365 725f  ],..    "parser_
-00000100: 6669 6c65 223a 2022 7061 7273 6572 5f6f  file": "parser_o
-00000110: 6e65 2e70 7922 2c0d 0a20 2020 2022 6e75  ne.py",..    "nu
-00000120: 6d65 7261 6c73 223a 207b 0d0a 2020 2020  merals": {..    
-00000130: 2020 2020 227a 6572 6f22 3a20 7b0d 0a20      "zero": {.. 
-00000140: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000150: 223a 2022 6469 6769 7473 222c 0d0a 2020  ": "digits",..  
-00000160: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00000170: 223a 2030 2e30 2c0d 0a20 2020 2020 2020  ": 0.0,..       
-00000180: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-00000190: 6365 726f 222c 2022 4365 726f 222c 2022  cero", "Cero", "
-000001a0: 4345 524f 222c 2022 6365 726f 7322 2c20  CERO", "ceros", 
-000001b0: 2243 6572 6f73 222c 2022 4345 524f 5322  "Ceros", "CEROS"
-000001c0: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-000001d0: 2020 2020 2020 2022 6f6e 6522 3a20 7b0d         "one": {.
-000001e0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-000001f0: 7065 223a 2022 6469 6769 7473 222c 0d0a  pe": "digits",..
-00000200: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00000210: 7565 223a 2031 2e30 2c0d 0a20 2020 2020  ue": 1.0,..     
-00000220: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
-00000230: 5b22 756e 6f22 2c20 2255 6e6f 222c 2022  ["uno", "Uno", "
-00000240: 554e 4f22 2c20 2275 6e6f 7322 2c20 2255  UNO", "unos", "U
-00000250: 6e6f 7322 2c20 2255 4e4f 5322 2c20 2275  nos", "UNOS", "u
-00000260: 6e22 2c20 2255 6e22 2c20 2255 4e22 2c20  n", "Un", "UN", 
-00000270: 2275 6e73 222c 2022 556e 7322 2c20 2255  "uns", "Uns", "U
-00000280: 4e53 222c 2022 756e 6122 2c20 2255 6e61  NS", "una", "Una
-00000290: 222c 2022 554e 4122 2c20 2275 6e61 7322  ", "UNA", "unas"
-000002a0: 2c20 2255 6e61 7322 2c20 2255 4e41 5322  , "Unas", "UNAS"
-000002b0: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-000002c0: 2020 2020 2020 2022 7477 6f22 3a20 7b0d         "two": {.
-000002d0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-000002e0: 7065 223a 2022 6469 6769 7473 222c 0d0a  pe": "digits",..
-000002f0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00000300: 7565 223a 2032 2e30 2c0d 0a20 2020 2020  ue": 2.0,..     
-00000310: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
-00000320: 5b22 646f 7322 2c20 2244 6f73 222c 2022  ["dos", "Dos", "
-00000330: 444f 5322 2c20 2264 6f73 6573 222c 2022  DOS", "doses", "
-00000340: 446f 7365 7322 2c20 2244 4f53 4553 225d  Doses", "DOSES"]
-00000350: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00000360: 2020 2020 2020 2274 6872 6565 223a 207b        "three": {
-00000370: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00000380: 7970 6522 3a20 2264 6967 6974 7322 2c0d  ype": "digits",.
-00000390: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
-000003a0: 6c75 6522 3a20 332e 302c 0d0a 2020 2020  lue": 3.0,..    
-000003b0: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
-000003c0: 205b 2274 7265 7322 2c20 2254 7265 7322   ["tres", "Tres"
-000003d0: 2c20 2254 5245 5322 2c20 2274 7265 7365  , "TRES", "trese
-000003e0: 7322 2c20 2254 7265 7365 7322 2c20 2254  s", "Treses", "T
-000003f0: 5245 5345 5322 5d0d 0a20 2020 2020 2020  RESES"]..       
-00000400: 207d 2c0d 0a20 2020 2020 2020 2022 666f   },..        "fo
-00000410: 7572 223a 207b 0d0a 2020 2020 2020 2020  ur": {..        
-00000420: 2020 2020 2274 7970 6522 3a20 2264 6967      "type": "dig
-00000430: 6974 7322 2c0d 0a20 2020 2020 2020 2020  its",..         
-00000440: 2020 2022 7661 6c75 6522 3a20 342e 302c     "value": 4.0,
-00000450: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00000460: 6572 6d73 223a 205b 2263 7561 7472 6f22  erms": ["cuatro"
-00000470: 2c20 2243 7561 7472 6f22 2c20 2243 5541  , "Cuatro", "CUA
-00000480: 5452 4f22 2c20 2263 7561 7472 6f73 222c  TRO", "cuatros",
-00000490: 2022 4375 6174 726f 7322 2c20 2243 5541   "Cuatros", "CUA
-000004a0: 5452 4f53 225d 0d0a 2020 2020 2020 2020  TROS"]..        
-000004b0: 7d2c 0d0a 2020 2020 2020 2020 2266 6976  },..        "fiv
-000004c0: 6522 3a20 7b0d 0a20 2020 2020 2020 2020  e": {..         
-000004d0: 2020 2022 7479 7065 223a 2022 6469 6769     "type": "digi
-000004e0: 7473 222c 0d0a 2020 2020 2020 2020 2020  ts",..          
-000004f0: 2020 2276 616c 7565 223a 2035 2e30 2c0d    "value": 5.0,.
-00000500: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00000510: 726d 7322 3a20 5b22 6369 6e63 6f22 2c20  rms": ["cinco", 
-00000520: 2243 696e 636f 222c 2022 4349 4e43 4f22  "Cinco", "CINCO"
-00000530: 2c20 2263 696e 636f 7322 2c20 2243 696e  , "cincos", "Cin
-00000540: 636f 7322 2c20 2243 494e 434f 5322 5d0d  cos", "CINCOS"].
-00000550: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00000560: 2020 2020 2022 7369 7822 3a20 7b0d 0a20       "six": {.. 
-00000570: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000580: 223a 2022 6469 6769 7473 222c 0d0a 2020  ": "digits",..  
-00000590: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000005a0: 223a 2036 2e30 2c0d 0a20 2020 2020 2020  ": 6.0,..       
-000005b0: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-000005c0: 7365 6973 222c 2022 5365 6973 222c 2022  seis", "Seis", "
-000005d0: 5345 4953 222c 2022 7365 6973 6573 222c  SEIS", "seises",
-000005e0: 2022 5365 6973 6573 222c 2022 5345 4953   "Seises", "SEIS
-000005f0: 4553 225d 0d0a 2020 2020 2020 2020 7d2c  ES"]..        },
-00000600: 0d0a 2020 2020 2020 2020 2273 6576 656e  ..        "seven
-00000610: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00000620: 2020 2274 7970 6522 3a20 2264 6967 6974    "type": "digit
-00000630: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00000640: 2022 7661 6c75 6522 3a20 372e 302c 0d0a   "value": 7.0,..
-00000650: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
-00000660: 6d73 223a 205b 2273 6965 7465 222c 2022  ms": ["siete", "
-00000670: 5369 6574 6522 2c20 2253 4945 5445 222c  Siete", "SIETE",
-00000680: 2022 7369 6574 6573 222c 2022 5369 6574   "sietes", "Siet
-00000690: 6573 222c 2022 5349 4554 4553 225d 0d0a  es", "SIETES"]..
-000006a0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000006b0: 2020 2020 2265 6967 6874 223a 207b 0d0a      "eight": {..
-000006c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000006d0: 6522 3a20 2264 6967 6974 7322 2c0d 0a20  e": "digits",.. 
-000006e0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-000006f0: 6522 3a20 382e 302c 0d0a 2020 2020 2020  e": 8.0,..      
-00000700: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00000710: 226f 6368 6f22 2c20 224f 6368 6f22 2c20  "ocho", "Ocho", 
-00000720: 224f 4348 4f22 2c20 226f 6368 6f73 222c  "OCHO", "ochos",
-00000730: 2022 4f63 686f 7322 2c20 224f 4348 4f53   "Ochos", "OCHOS
-00000740: 225d 0d0a 2020 2020 2020 2020 7d2c 0d0a  "]..        },..
-00000750: 2020 2020 2020 2020 226e 696e 6522 3a20          "nine": 
-00000760: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00000770: 7479 7065 223a 2022 6469 6769 7473 222c  type": "digits",
-00000780: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00000790: 616c 7565 223a 2039 2e30 2c0d 0a20 2020  alue": 9.0,..   
-000007a0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-000007b0: 3a20 5b22 6e75 6576 6522 2c20 224e 7565  : ["nueve", "Nue
-000007c0: 7665 222c 2022 4e55 4556 4522 2c20 226e  ve", "NUEVE", "n
-000007d0: 7565 7665 7322 2c20 224e 7565 7665 7322  ueves", "Nueves"
-000007e0: 2c20 224e 5545 5645 5322 5d0d 0a20 2020  , "NUEVES"]..   
-000007f0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00000800: 2022 7465 6e22 3a20 7b0d 0a20 2020 2020   "ten": {..     
-00000810: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000820: 7465 656e 7322 2c0d 0a20 2020 2020 2020  teens",..       
-00000830: 2020 2020 2022 7661 6c75 6522 3a20 3130       "value": 10
-00000840: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000850: 2022 7465 726d 7322 3a20 5b22 6469 657a   "terms": ["diez
-00000860: 222c 2022 4469 657a 222c 2022 4449 455a  ", "Diez", "DIEZ
-00000870: 222c 2022 6469 6573 222c 2022 4469 6573  ", "dies", "Dies
-00000880: 222c 2022 4449 4553 222c 2022 6469 6563  ", "DIES", "diec
-00000890: 222c 2022 4469 6563 222c 2022 4449 4543  ", "Diec", "DIEC
-000008a0: 222c 2022 6469 657a 6573 222c 2022 4469  ", "diezes", "Di
-000008b0: 657a 6573 222c 2022 4449 455a 4553 222c  ezes", "DIEZES",
-000008c0: 2022 6469 6573 6573 222c 2022 4469 6573   "dieses", "Dies
-000008d0: 6573 222c 2022 4449 4553 4553 222c 2022  es", "DIESES", "
-000008e0: 6469 6563 6573 222c 2022 4469 6563 6573  dieces", "Dieces
-000008f0: 222c 2022 4449 4543 4553 225d 0d0a 2020  ", "DIECES"]..  
-00000900: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000910: 2020 2265 6c65 7665 6e22 3a20 7b0d 0a20    "eleven": {.. 
-00000920: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000930: 223a 2022 7465 656e 7322 2c0d 0a20 2020  ": "teens",..   
-00000940: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00000950: 3a20 3131 2e30 2c0d 0a20 2020 2020 2020  : 11.0,..       
-00000960: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-00000970: 6f6e 6365 222c 2022 4f6e 6365 222c 2022  once", "Once", "
-00000980: 4f4e 4345 222c 2022 6f6e 6365 7322 2c20  ONCE", "onces", 
-00000990: 224f 6e63 6573 222c 2022 4f4e 4345 5322  "Onces", "ONCES"
-000009a0: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-000009b0: 2020 2020 2020 2022 7477 656c 7665 223a         "twelve":
-000009c0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000009d0: 2274 7970 6522 3a20 2274 6565 6e73 222c  "type": "teens",
-000009e0: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-000009f0: 616c 7565 223a 2031 322e 302c 0d0a 2020  alue": 12.0,..  
-00000a00: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-00000a10: 223a 205b 2264 6f63 6522 2c20 2244 6f63  ": ["doce", "Doc
-00000a20: 6522 2c20 2244 4f43 4522 2c20 2264 6f63  e", "DOCE", "doc
-00000a30: 6573 222c 2022 446f 6365 7322 2c20 2244  es", "Doces", "D
-00000a40: 4f43 4553 225d 0d0a 2020 2020 2020 2020  OCES"]..        
-00000a50: 7d2c 0d0a 2020 2020 2020 2020 2274 6869  },..        "thi
-00000a60: 7274 6565 6e22 3a20 7b0d 0a20 2020 2020  rteen": {..     
-00000a70: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000a80: 7465 656e 7322 2c0d 0a20 2020 2020 2020  teens",..       
-00000a90: 2020 2020 2022 7661 6c75 6522 3a20 3133       "value": 13
-00000aa0: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000ab0: 2022 7465 726d 7322 3a20 5b22 7472 6563   "terms": ["trec
-00000ac0: 6522 2c20 2254 7265 6365 222c 2022 5452  e", "Trece", "TR
-00000ad0: 4543 4522 2c20 2274 7265 6365 7322 2c20  ECE", "treces", 
-00000ae0: 2254 7265 6365 7322 2c20 2254 5245 4345  "Treces", "TRECE
-00000af0: 5322 5d0d 0a20 2020 2020 2020 207d 2c0d  S"]..        },.
-00000b00: 0a20 2020 2020 2020 2022 666f 7572 7465  .        "fourte
-00000b10: 656e 223a 207b 0d0a 2020 2020 2020 2020  en": {..        
-00000b20: 2020 2020 2274 7970 6522 3a20 2274 6565      "type": "tee
-00000b30: 6e73 222c 0d0a 2020 2020 2020 2020 2020  ns",..          
-00000b40: 2020 2276 616c 7565 223a 2031 342e 302c    "value": 14.0,
-00000b50: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00000b60: 6572 6d73 223a 205b 2263 6174 6f72 6365  erms": ["catorce
-00000b70: 222c 2022 4361 746f 7263 6522 2c20 2243  ", "Catorce", "C
-00000b80: 4154 4f52 4345 222c 2022 6361 746f 7263  ATORCE", "catorc
-00000b90: 6573 222c 2022 4361 746f 7263 6573 222c  es", "Catorces",
-00000ba0: 2022 4341 544f 5243 4553 225d 0d0a 2020   "CATORCES"]..  
-00000bb0: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000bc0: 2020 2266 6966 7465 656e 223a 207b 0d0a    "fifteen": {..
-00000bd0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00000be0: 6522 3a20 2274 6565 6e73 222c 0d0a 2020  e": "teens",..  
-00000bf0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00000c00: 223a 2031 352e 302c 0d0a 2020 2020 2020  ": 15.0,..      
-00000c10: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00000c20: 2271 7569 6e63 6522 2c20 2251 7569 6e63  "quince", "Quinc
-00000c30: 6522 2c20 2251 5549 4e43 4522 2c20 2271  e", "QUINCE", "q
-00000c40: 7569 6e63 6573 222c 2022 5175 696e 6365  uinces", "Quince
-00000c50: 7322 2c20 2251 5549 4e43 4553 225d 0d0a  s", "QUINCES"]..
-00000c60: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00000c70: 2020 2020 2273 6978 7465 656e 223a 207b      "sixteen": {
-00000c80: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00000c90: 7970 6522 3a20 2274 6565 6e73 222c 0d0a  ype": "teens",..
-00000ca0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00000cb0: 7565 223a 2031 362e 302c 0d0a 2020 2020  ue": 16.0,..    
-00000cc0: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
-00000cd0: 205b 2264 6965 6369 7365 6973 222c 2022   ["dieciseis", "
-00000ce0: 4469 6563 6973 6569 7322 2c20 2244 4945  Dieciseis", "DIE
-00000cf0: 4349 5345 4953 222c 2022 6469 6563 6973  CISEIS", "diecis
-00000d00: 6569 7365 7322 2c20 2244 6965 6369 7365  eises", "Diecise
-00000d10: 6973 6573 222c 2022 4449 4543 4953 4549  ises", "DIECISEI
-00000d20: 5345 5322 5d0d 0a20 2020 2020 2020 207d  SES"]..        }
-00000d30: 2c0d 0a20 2020 2020 2020 2022 7365 7665  ,..        "seve
-00000d40: 6e74 6565 6e22 3a20 7b0d 0a20 2020 2020  nteen": {..     
-00000d50: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000d60: 7465 656e 7322 2c0d 0a20 2020 2020 2020  teens",..       
-00000d70: 2020 2020 2022 7661 6c75 6522 3a20 3137       "value": 17
-00000d80: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000d90: 2022 7465 726d 7322 3a20 5b22 6469 6563   "terms": ["diec
-00000da0: 6973 6965 7465 222c 2022 4469 6563 6973  isiete", "Diecis
-00000db0: 6965 7465 222c 2022 4449 4543 4953 4945  iete", "DIECISIE
-00000dc0: 5445 222c 2022 6469 6563 6973 6965 7465  TE", "diecisiete
-00000dd0: 7322 2c20 2244 6965 6369 7369 6574 6573  s", "Diecisietes
-00000de0: 222c 2022 4449 4543 4953 4945 5445 5322  ", "DIECISIETES"
-00000df0: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00000e00: 2020 2020 2020 2022 6569 6768 7465 656e         "eighteen
-00000e10: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00000e20: 2020 2274 7970 6522 3a20 2274 6565 6e73    "type": "teens
-00000e30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000e40: 2276 616c 7565 223a 2031 382e 302c 0d0a  "value": 18.0,..
-00000e50: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
-00000e60: 6d73 223a 205b 2264 6965 6369 6f63 686f  ms": ["dieciocho
-00000e70: 222c 2022 4469 6563 696f 6368 6f22 2c20  ", "Dieciocho", 
-00000e80: 2244 4945 4349 4f43 484f 222c 2022 6469  "DIECIOCHO", "di
-00000e90: 6563 696f 6368 6f73 222c 2022 4469 6563  eciochos", "Diec
-00000ea0: 696f 6368 6f73 222c 2022 4449 4543 494f  iochos", "DIECIO
-00000eb0: 4348 4f53 225d 0d0a 2020 2020 2020 2020  CHOS"]..        
-00000ec0: 7d2c 0d0a 2020 2020 2020 2020 226e 696e  },..        "nin
-00000ed0: 6574 6565 6e22 3a20 7b0d 0a20 2020 2020  eteen": {..     
-00000ee0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000ef0: 7465 656e 7322 2c0d 0a20 2020 2020 2020  teens",..       
-00000f00: 2020 2020 2022 7661 6c75 6522 3a20 3139       "value": 19
-00000f10: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00000f20: 2022 7465 726d 7322 3a20 5b22 6469 6563   "terms": ["diec
-00000f30: 696e 7565 7665 222c 2022 4469 6563 696e  inueve", "Diecin
-00000f40: 7565 7665 222c 2022 4449 4543 494e 5545  ueve", "DIECINUE
-00000f50: 5645 222c 2022 6469 6563 696e 7565 7665  VE", "diecinueve
-00000f60: 7322 2c20 2244 6965 6369 6e75 6576 6573  s", "Diecinueves
-00000f70: 222c 2022 4449 4543 494e 5545 5645 5322  ", "DIECINUEVES"
-00000f80: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00000f90: 2020 2020 2020 2022 7477 656e 7479 223a         "twenty":
-00000fa0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000fb0: 2274 7970 6522 3a20 2274 656e 7322 2c0d  "type": "tens",.
-00000fc0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
-00000fd0: 6c75 6522 3a20 3230 2e30 2c0d 0a20 2020  lue": 20.0,..   
-00000fe0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-00000ff0: 3a20 5b22 7665 696e 7465 222c 2022 5665  : ["veinte", "Ve
-00001000: 696e 7465 222c 2022 5645 494e 5445 222c  inte", "VEINTE",
-00001010: 2022 7665 696e 7465 7322 2c20 2256 6569   "veintes", "Vei
-00001020: 6e74 6573 222c 2022 5645 494e 5445 5322  ntes", "VEINTES"
-00001030: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00001040: 2020 2020 2020 2022 7477 656e 7479 2d6f         "twenty-o
-00001050: 6e65 223a 207b 0d0a 2020 2020 2020 2020  ne": {..        
-00001060: 2020 2020 2274 7970 6522 3a20 2264 6967      "type": "dig
-00001070: 6974 7322 2c0d 0a20 2020 2020 2020 2020  its",..         
-00001080: 2020 2022 7661 6c75 6522 3a20 3231 2e30     "value": 21.0
-00001090: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000010a0: 7465 726d 7322 3a20 5b22 7665 696e 7469  terms": ["veinti
-000010b0: 756e 6f22 2c20 2256 6569 6e74 6975 6e6f  uno", "Veintiuno
-000010c0: 222c 2022 5645 494e 5449 554e 4f22 2c20  ", "VEINTIUNO", 
-000010d0: 2276 6569 6e74 6975 6e6f 7322 2c20 2256  "veintiunos", "V
-000010e0: 6569 6e74 6975 6e6f 7322 2c20 2256 4549  eintiunos", "VEI
-000010f0: 4e54 4955 4e4f 5322 2c20 2276 6569 6e74  NTIUNOS", "veint
-00001100: 6975 6e61 222c 2022 5665 696e 7469 756e  iuna", "Veintiun
-00001110: 6122 2c20 2256 4549 4e54 4955 4e41 222c  a", "VEINTIUNA",
-00001120: 2022 7665 696e 7469 756e 6173 222c 2022   "veintiunas", "
-00001130: 5665 696e 7469 756e 6173 222c 2022 5645  Veintiunas", "VE
-00001140: 494e 5449 554e 4153 225d 0d0a 2020 2020  INTIUNAS"]..    
-00001150: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00001160: 2274 7765 6e74 792d 7477 6f22 3a20 7b0d  "twenty-two": {.
-00001170: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00001180: 7065 223a 2022 6469 6769 7473 222c 0d0a  pe": "digits",..
-00001190: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-000011a0: 7565 223a 2032 322e 302c 0d0a 2020 2020  ue": 22.0,..    
-000011b0: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
-000011c0: 205b 2276 6569 6e74 6964 6f73 222c 2022   ["veintidos", "
-000011d0: 5665 696e 7469 646f 7322 2c20 2256 4549  Veintidos", "VEI
-000011e0: 4e54 4944 4f53 222c 2022 7665 696e 7469  NTIDOS", "veinti
-000011f0: 646f 7365 7322 2c20 2256 6569 6e74 6964  doses", "Veintid
-00001200: 6f73 6573 222c 2022 5645 494e 5449 444f  oses", "VEINTIDO
-00001210: 5345 5322 5d0d 0a20 2020 2020 2020 207d  SES"]..        }
-00001220: 2c0d 0a20 2020 2020 2020 2022 7477 656e  ,..        "twen
-00001230: 7479 2d74 6872 6565 223a 207b 0d0a 2020  ty-three": {..  
-00001240: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001250: 3a20 2264 6967 6974 7322 2c0d 0a20 2020  : "digits",..   
-00001260: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00001270: 3a20 3233 2e30 2c0d 0a20 2020 2020 2020  : 23.0,..       
-00001280: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-00001290: 7665 696e 7469 7472 6573 222c 2022 5665  veintitres", "Ve
-000012a0: 696e 7469 7472 6573 222c 2022 5645 494e  intitres", "VEIN
-000012b0: 5449 5452 4553 222c 2022 7665 696e 7469  TITRES", "veinti
-000012c0: 7472 6573 6573 222c 2022 5665 696e 7469  treses", "Veinti
-000012d0: 7472 6573 6573 222c 2022 5645 494e 5449  treses", "VEINTI
-000012e0: 5452 4553 4553 225d 0d0a 2020 2020 2020  TRESES"]..      
-000012f0: 2020 7d2c 0d0a 2020 2020 2020 2020 2274    },..        "t
-00001300: 7765 6e74 792d 666f 7572 223a 207b 0d0a  wenty-four": {..
-00001310: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00001320: 6522 3a20 2264 6967 6974 7322 2c0d 0a20  e": "digits",.. 
-00001330: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00001340: 6522 3a20 3234 2e30 2c0d 0a20 2020 2020  e": 24.0,..     
-00001350: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
-00001360: 5b22 7665 696e 7469 6375 6174 726f 222c  ["veinticuatro",
-00001370: 2022 5665 696e 7469 6375 6174 726f 222c   "Veinticuatro",
-00001380: 2022 5645 494e 5449 4355 4154 524f 222c   "VEINTICUATRO",
-00001390: 2022 7665 696e 7469 6375 6174 726f 7322   "veinticuatros"
-000013a0: 2c20 2256 6569 6e74 6963 7561 7472 6f73  , "Veinticuatros
-000013b0: 222c 2022 5645 494e 5449 4355 4154 524f  ", "VEINTICUATRO
-000013c0: 5322 5d0d 0a20 2020 2020 2020 207d 2c0d  S"]..        },.
-000013d0: 0a20 2020 2020 2020 2022 7477 656e 7479  .        "twenty
-000013e0: 2d66 6976 6522 3a20 7b0d 0a20 2020 2020  -five": {..     
-000013f0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00001400: 6469 6769 7473 222c 0d0a 2020 2020 2020  digits",..      
-00001410: 2020 2020 2020 2276 616c 7565 223a 2032        "value": 2
-00001420: 352e 302c 0d0a 2020 2020 2020 2020 2020  5.0,..          
-00001430: 2020 2274 6572 6d73 223a 205b 2276 6569    "terms": ["vei
-00001440: 6e74 6963 696e 636f 222c 2022 5665 696e  nticinco", "Vein
-00001450: 7469 6369 6e63 6f22 2c20 2256 4549 4e54  ticinco", "VEINT
-00001460: 4943 494e 434f 222c 2022 7665 696e 7469  ICINCO", "veinti
-00001470: 6369 6e63 6f73 222c 2022 5665 696e 7469  cincos", "Veinti
-00001480: 6369 6e63 6f73 222c 2022 5645 494e 5449  cincos", "VEINTI
-00001490: 4349 4e43 4f53 225d 0d0a 2020 2020 2020  CINCOS"]..      
-000014a0: 2020 7d2c 0d0a 2020 2020 2020 2020 2274    },..        "t
-000014b0: 7765 6e74 792d 7369 7822 3a20 7b0d 0a20  wenty-six": {.. 
-000014c0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000014d0: 223a 2022 6469 6769 7473 222c 0d0a 2020  ": "digits",..  
-000014e0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000014f0: 223a 2032 362e 302c 0d0a 2020 2020 2020  ": 26.0,..      
-00001500: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00001510: 2276 6569 6e74 6973 6569 7322 2c20 2256  "veintiseis", "V
-00001520: 6569 6e74 6973 6569 7322 2c20 2256 4549  eintiseis", "VEI
-00001530: 4e54 4953 4549 5322 2c20 2276 6569 6e74  NTISEIS", "veint
-00001540: 6973 6569 7365 7322 2c20 2256 6569 6e74  iseises", "Veint
-00001550: 6973 6569 7365 7322 2c20 2256 4549 4e54  iseises", "VEINT
-00001560: 4953 4549 5345 5322 5d0d 0a20 2020 2020  ISEISES"]..     
-00001570: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-00001580: 7477 656e 7479 2d73 6576 656e 223a 207b  twenty-seven": {
-00001590: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-000015a0: 7970 6522 3a20 2264 6967 6974 7322 2c0d  ype": "digits",.
-000015b0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
-000015c0: 6c75 6522 3a20 3237 2e30 2c0d 0a20 2020  lue": 27.0,..   
-000015d0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-000015e0: 3a20 5b22 7665 696e 7469 7369 6574 6522  : ["veintisiete"
-000015f0: 2c20 2256 6569 6e74 6973 6965 7465 222c  , "Veintisiete",
-00001600: 2022 5645 494e 5449 5349 4554 4522 2c20   "VEINTISIETE", 
-00001610: 2276 6569 6e74 6973 6965 7465 7322 2c20  "veintisietes", 
-00001620: 2256 6569 6e74 6973 6965 7465 7322 2c20  "Veintisietes", 
-00001630: 2256 4549 4e54 4953 4945 5445 5322 5d0d  "VEINTISIETES"].
-00001640: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00001650: 2020 2020 2022 7477 656e 7479 2d65 6967       "twenty-eig
-00001660: 6874 223a 207b 0d0a 2020 2020 2020 2020  ht": {..        
-00001670: 2020 2020 2274 7970 6522 3a20 2264 6967      "type": "dig
-00001680: 6974 7322 2c0d 0a20 2020 2020 2020 2020  its",..         
-00001690: 2020 2022 7661 6c75 6522 3a20 3238 2e30     "value": 28.0
-000016a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000016b0: 7465 726d 7322 3a20 5b22 7665 696e 7469  terms": ["veinti
-000016c0: 6f63 686f 222c 2022 5665 696e 7469 6f63  ocho", "Veintioc
-000016d0: 686f 222c 2022 5645 494e 5449 4f43 484f  ho", "VEINTIOCHO
-000016e0: 222c 2022 7665 696e 7469 6f63 686f 7322  ", "veintiochos"
-000016f0: 2c20 2256 6569 6e74 696f 6368 6f73 222c  , "Veintiochos",
-00001700: 2022 5645 494e 5449 4f43 484f 5322 5d0d   "VEINTIOCHOS"].
-00001710: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00001720: 2020 2020 2022 7477 656e 7479 2d6e 696e       "twenty-nin
-00001730: 6522 3a20 7b0d 0a20 2020 2020 2020 2020  e": {..         
-00001740: 2020 2022 7479 7065 223a 2022 6469 6769     "type": "digi
-00001750: 7473 222c 0d0a 2020 2020 2020 2020 2020  ts",..          
-00001760: 2020 2276 616c 7565 223a 2032 392e 302c    "value": 29.0,
-00001770: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00001780: 6572 6d73 223a 205b 2276 6569 6e74 696e  erms": ["veintin
-00001790: 7565 7665 222c 2022 5665 696e 7469 6e75  ueve", "Veintinu
-000017a0: 6576 6522 2c20 2256 4549 4e54 494e 5545  eve", "VEINTINUE
-000017b0: 5645 222c 2022 7665 696e 7469 6e75 6576  VE", "veintinuev
-000017c0: 6573 222c 2022 5665 696e 7469 6e75 6576  es", "Veintinuev
-000017d0: 6573 222c 2022 5645 494e 5449 4e55 4556  es", "VEINTINUEV
-000017e0: 4553 225d 0d0a 2020 2020 2020 2020 7d2c  ES"]..        },
-000017f0: 0d0a 2020 2020 2020 2020 2274 6869 7274  ..        "thirt
-00001800: 7922 3a20 7b0d 0a20 2020 2020 2020 2020  y": {..         
-00001810: 2020 2022 7479 7065 223a 2022 7465 6e73     "type": "tens
-00001820: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001830: 2276 616c 7565 223a 2033 302e 302c 0d0a  "value": 30.0,..
-00001840: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
-00001850: 6d73 223a 205b 2274 7265 696e 7461 222c  ms": ["treinta",
-00001860: 2022 5472 6569 6e74 6122 2c20 2254 5245   "Treinta", "TRE
-00001870: 494e 5441 222c 2022 7472 6569 6e74 6173  INTA", "treintas
-00001880: 222c 2022 5472 6569 6e74 6173 222c 2022  ", "Treintas", "
-00001890: 5452 4549 4e54 4153 225d 0d0a 2020 2020  TREINTAS"]..    
-000018a0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-000018b0: 2266 6f72 7479 223a 207b 0d0a 2020 2020  "forty": {..    
-000018c0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-000018d0: 2274 656e 7322 2c0d 0a20 2020 2020 2020  "tens",..       
-000018e0: 2020 2020 2022 7661 6c75 6522 3a20 3430       "value": 40
-000018f0: 2e30 2c0d 0a20 2020 2020 2020 2020 2020  .0,..           
-00001900: 2022 7465 726d 7322 3a20 5b22 6375 6172   "terms": ["cuar
-00001910: 656e 7461 222c 2022 4375 6172 656e 7461  enta", "Cuarenta
-00001920: 222c 2022 4355 4152 454e 5441 222c 2022  ", "CUARENTA", "
-00001930: 6375 6172 656e 7461 7322 2c20 2243 7561  cuarentas", "Cua
-00001940: 7265 6e74 6173 222c 2022 4355 4152 454e  rentas", "CUAREN
-00001950: 5441 5322 5d0d 0a20 2020 2020 2020 207d  TAS"]..        }
-00001960: 2c0d 0a20 2020 2020 2020 2022 6669 6674  ,..        "fift
-00001970: 7922 3a20 7b0d 0a20 2020 2020 2020 2020  y": {..         
-00001980: 2020 2022 7479 7065 223a 2022 7465 6e73     "type": "tens
-00001990: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000019a0: 2276 616c 7565 223a 2035 302e 302c 0d0a  "value": 50.0,..
-000019b0: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
-000019c0: 6d73 223a 205b 2263 696e 6375 656e 7461  ms": ["cincuenta
-000019d0: 222c 2022 4369 6e63 7565 6e74 6122 2c20  ", "Cincuenta", 
-000019e0: 2243 494e 4355 454e 5441 222c 2022 6369  "CINCUENTA", "ci
-000019f0: 6e63 7565 6e74 6173 222c 2022 4369 6e63  ncuentas", "Cinc
-00001a00: 7565 6e74 6173 222c 2022 4349 4e43 5545  uentas", "CINCUE
-00001a10: 4e54 4153 225d 0d0a 2020 2020 2020 2020  NTAS"]..        
-00001a20: 7d2c 0d0a 2020 2020 2020 2020 2273 6978  },..        "six
-00001a30: 7479 223a 207b 0d0a 2020 2020 2020 2020  ty": {..        
-00001a40: 2020 2020 2274 7970 6522 3a20 2274 656e      "type": "ten
-00001a50: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00001a60: 2022 7661 6c75 6522 3a20 3630 2e30 2c0d   "value": 60.0,.
-00001a70: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00001a80: 726d 7322 3a20 5b22 7365 7365 6e74 6122  rms": ["sesenta"
-00001a90: 2c20 2253 6573 656e 7461 222c 2022 5345  , "Sesenta", "SE
-00001aa0: 5345 4e54 4122 2c20 2273 6573 656e 7461  SENTA", "sesenta
-00001ab0: 7322 2c20 2253 6573 656e 7461 7322 2c20  s", "Sesentas", 
-00001ac0: 2253 4553 454e 5441 5322 5d0d 0a20 2020  "SESENTAS"]..   
-00001ad0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00001ae0: 2022 7365 7665 6e74 7922 3a20 7b0d 0a20   "seventy": {.. 
-00001af0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00001b00: 223a 2022 7465 6e73 222c 0d0a 2020 2020  ": "tens",..    
-00001b10: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-00001b20: 2037 302e 302c 0d0a 2020 2020 2020 2020   70.0,..        
-00001b30: 2020 2020 2274 6572 6d73 223a 205b 2273      "terms": ["s
-00001b40: 6574 656e 7461 222c 2022 5365 7465 6e74  etenta", "Setent
-00001b50: 6122 2c20 2253 4554 454e 5441 222c 2022  a", "SETENTA", "
-00001b60: 7365 7465 6e74 6173 222c 2022 5365 7465  setentas", "Sete
-00001b70: 6e74 6173 222c 2022 5345 5445 4e54 4153  ntas", "SETENTAS
-00001b80: 225d 0d0a 2020 2020 2020 2020 7d2c 0d0a  "]..        },..
-00001b90: 2020 2020 2020 2020 2265 6967 6874 7922          "eighty"
-00001ba0: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00001bb0: 2022 7479 7065 223a 2022 7465 6e73 222c   "type": "tens",
-00001bc0: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-00001bd0: 616c 7565 223a 2038 302e 302c 0d0a 2020  alue": 80.0,..  
-00001be0: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-00001bf0: 223a 205b 226f 6368 656e 7461 222c 2022  ": ["ochenta", "
-00001c00: 4f63 6865 6e74 6122 2c20 224f 4348 454e  Ochenta", "OCHEN
-00001c10: 5441 222c 2022 6f63 6865 6e74 6173 222c  TA", "ochentas",
-00001c20: 2022 4f63 6865 6e74 6173 222c 2022 4f43   "Ochentas", "OC
-00001c30: 4845 4e54 4153 225d 0d0a 2020 2020 2020  HENTAS"]..      
-00001c40: 2020 7d2c 0d0a 2020 2020 2020 2020 226e    },..        "n
-00001c50: 696e 6574 7922 3a20 7b0d 0a20 2020 2020  inety": {..     
-00001c60: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00001c70: 7465 6e73 222c 0d0a 2020 2020 2020 2020  tens",..        
-00001c80: 2020 2020 2276 616c 7565 223a 2039 302e      "value": 90.
-00001c90: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00001ca0: 2274 6572 6d73 223a 205b 226e 6f76 656e  "terms": ["noven
-00001cb0: 7461 222c 2022 4e6f 7665 6e74 6122 2c20  ta", "Noventa", 
-00001cc0: 224e 4f56 454e 5441 222c 2022 6e6f 7665  "NOVENTA", "nove
-00001cd0: 6e74 6173 222c 2022 4e6f 7665 6e74 6173  ntas", "Noventas
-00001ce0: 222c 2022 4e4f 5645 4e54 4153 225d 0d0a  ", "NOVENTAS"]..
-00001cf0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00001d00: 2020 2020 2268 756e 6472 6564 223a 207b      "hundred": {
-00001d10: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-00001d20: 7970 6522 3a20 2274 686f 7573 616e 6473  ype": "thousands
-00001d30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001d40: 2276 616c 7565 223a 2031 3030 2e30 2c0d  "value": 100.0,.
-00001d50: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00001d60: 726d 7322 3a20 5b22 6369 656e 222c 2022  rms": ["cien", "
-00001d70: 4369 656e 222c 2022 4349 454e 222c 2022  Cien", "CIEN", "
-00001d80: 6369 656e 7322 2c20 2243 6965 6e73 222c  ciens", "Ciens",
-00001d90: 2022 4349 454e 5322 2c20 2263 6965 6e65   "CIENS", "ciene
-00001da0: 7322 2c20 2243 6965 6e65 7322 2c20 2243  s", "Cienes", "C
-00001db0: 4945 4e45 5322 2c20 2263 6965 6e74 6f73  IENES", "cientos
-00001dc0: 222c 2022 4369 656e 746f 7322 2c20 2243  ", "Cientos", "C
-00001dd0: 4945 4e54 4f53 225d 0d0a 2020 2020 2020  IENTOS"]..      
-00001de0: 2020 7d2c 0d0a 2020 2020 2020 2020 2274    },..        "t
-00001df0: 686f 7573 616e 6422 3a20 7b0d 0a20 2020  housand": {..   
-00001e00: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00001e10: 2022 7468 6f75 7361 6e64 7322 2c0d 0a20   "thousands",.. 
-00001e20: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00001e30: 6522 3a20 3130 3030 2e30 2c0d 0a20 2020  e": 1000.0,..   
-00001e40: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-00001e50: 3a20 5b22 6d69 6c22 2c20 224d 696c 222c  : ["mil", "Mil",
-00001e60: 2022 4d49 4c22 2c20 226d 696c 7322 2c20   "MIL", "mils", 
-00001e70: 224d 696c 7322 2c20 224d 494c 5322 2c20  "Mils", "MILS", 
-00001e80: 226d 696c 6573 222c 2022 4d69 6c65 7322  "miles", "Miles"
-00001e90: 2c20 224d 494c 4553 225d 0d0a 2020 2020  , "MILES"]..    
-00001ea0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00001eb0: 226d 696c 6c69 6f6e 223a 207b 0d0a 2020  "million": {..  
-00001ec0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001ed0: 3a20 2274 686f 7573 616e 6473 222c 0d0a  : "thousands",..
-00001ee0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00001ef0: 7565 223a 2031 3030 3030 3030 2e30 2c0d  ue": 1000000.0,.
-00001f00: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00001f10: 726d 7322 3a20 5b22 6d69 6c6c 6f6e 222c  rms": ["millon",
-00001f20: 2022 4d69 6c6c 6f6e 222c 2022 4d49 4c4c   "Millon", "MILL
-00001f30: 4f4e 222c 2022 6d69 6c6c 6f6e 7322 2c20  ON", "millons", 
-00001f40: 224d 696c 6c6f 6e73 222c 2022 4d49 4c4c  "Millons", "MILL
-00001f50: 4f4e 5322 2c20 226d 696c 6c6f 6e65 7322  ONS", "millones"
-00001f60: 2c20 224d 696c 6c6f 6e65 7322 2c20 224d  , "Millones", "M
-00001f70: 494c 4c4f 4e45 5322 5d0d 0a20 2020 2020  ILLONES"]..     
-00001f80: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-00001f90: 7472 696c 6c69 6f6e 223a 207b 0d0a 2020  trillion": {..  
-00001fa0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001fb0: 3a20 2274 686f 7573 616e 6473 222c 0d0a  : "thousands",..
-00001fc0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00001fd0: 7565 223a 2031 3030 3030 3030 3030 3030  ue": 10000000000
-00001fe0: 3030 2e30 2c0d 0a20 2020 2020 2020 2020  00.0,..         
-00001ff0: 2020 2022 7465 726d 7322 3a20 5b22 6269     "terms": ["bi
-00002000: 6c6c 6f6e 222c 2022 4269 6c6c 6f6e 222c  llon", "Billon",
-00002010: 2022 4249 4c4c 4f4e 222c 2022 6269 6c6c   "BILLON", "bill
-00002020: 6f6e 7322 2c20 2242 696c 6c6f 6e73 222c  ons", "Billons",
-00002030: 2022 4249 4c4c 4f4e 5322 2c20 2262 696c   "BILLONS", "bil
-00002040: 6c6f 6e65 7322 2c20 2242 696c 6c6f 6e65  lones", "Billone
-00002050: 7322 2c20 2242 494c 4c4f 4e45 5322 5d0d  s", "BILLONES"].
-00002060: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00002070: 2020 2020 2022 6675 6c6c 223a 207b 0d0a       "full": {..
-00002080: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00002090: 6522 3a20 226d 6f64 6966 6965 7273 222c  e": "modifiers",
-000020a0: 0d0a 2020 2020 2020 2020 2020 2020 2276  ..            "v
-000020b0: 616c 7565 223a 2031 2e30 2c0d 0a20 2020  alue": 1.0,..   
-000020c0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-000020d0: 3a20 5b22 636f 6d70 6c65 746f 222c 2022  : ["completo", "
-000020e0: 436f 6d70 6c65 746f 222c 2022 434f 4d50  Completo", "COMP
-000020f0: 4c45 544f 222c 2022 636f 6d70 6c65 746f  LETO", "completo
-00002100: 7322 2c20 2243 6f6d 706c 6574 6f73 222c  s", "Completos",
-00002110: 2022 434f 4d50 4c45 544f 5322 2c20 2263   "COMPLETOS", "c
-00002120: 6f6d 706c 6574 6122 2c20 2243 6f6d 706c  ompleta", "Compl
-00002130: 6574 6122 2c20 2243 4f4d 504c 4554 4122  eta", "COMPLETA"
-00002140: 2c20 2263 6f6d 706c 6574 6173 222c 2022  , "completas", "
-00002150: 436f 6d70 6c65 7461 7322 2c20 2243 4f4d  Completas", "COM
-00002160: 504c 4554 4153 222c 2022 746f 7461 6c22  PLETAS", "total"
-00002170: 2c20 2254 6f74 616c 222c 2022 544f 5441  , "Total", "TOTA
-00002180: 4c22 2c20 2274 6f74 616c 6573 222c 2022  L", "totales", "
-00002190: 546f 7461 6c65 7322 2c20 2254 4f54 414c  Totales", "TOTAL
-000021a0: 4553 222c 2022 6c6c 656e 6f22 2c20 224c  ES", "lleno", "L
-000021b0: 6c65 6e6f 222c 2022 4c4c 454e 4f22 2c20  leno", "LLENO", 
-000021c0: 226c 6c65 6e6f 7322 2c20 224c 6c65 6e6f  "llenos", "Lleno
-000021d0: 7322 2c20 224c 4c45 4e4f 5322 2c20 226c  s", "LLENOS", "l
-000021e0: 6c65 6e61 222c 2022 4c6c 656e 6122 2c20  lena", "Llena", 
-000021f0: 224c 4c45 4e41 222c 2022 6c6c 656e 6173  "LLENA", "llenas
-00002200: 222c 2022 4c6c 656e 6173 222c 2022 4c4c  ", "Llenas", "LL
-00002210: 454e 4153 222c 2022 656e 7465 726f 222c  ENAS", "entero",
-00002220: 2022 456e 7465 726f 222c 2022 454e 5445   "Entero", "ENTE
-00002230: 524f 222c 2022 656e 7465 726f 7322 2c20  RO", "enteros", 
-00002240: 2245 6e74 6572 6f73 222c 2022 454e 5445  "Enteros", "ENTE
-00002250: 524f 5322 2c20 2265 6e74 6572 6122 2c20  ROS", "entera", 
-00002260: 2245 6e74 6572 6122 2c20 2245 4e54 4552  "Entera", "ENTER
-00002270: 4122 2c20 2265 6e74 6572 6173 222c 2022  A", "enteras", "
-00002280: 456e 7465 7261 7322 2c20 2245 4e54 4552  Enteras", "ENTER
-00002290: 4153 222c 2022 746f 646f 222c 2022 546f  AS", "todo", "To
-000022a0: 646f 222c 2022 544f 444f 222c 2022 746f  do", "TODO", "to
-000022b0: 646f 7322 2c20 2254 6f64 6f73 222c 2022  dos", "Todos", "
-000022c0: 544f 444f 5322 2c20 2274 6f64 6122 2c20  TODOS", "toda", 
-000022d0: 2254 6f64 6122 2c20 2254 4f44 4122 2c20  "Toda", "TODA", 
-000022e0: 2274 6f64 6173 222c 2022 546f 6461 7322  "todas", "Todas"
-000022f0: 2c20 2254 4f44 4153 225d 0d0a 2020 2020  , "TODAS"]..    
-00002300: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00002310: 2268 616c 6622 3a20 7b0d 0a20 2020 2020  "half": {..     
-00002320: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00002330: 6d6f 6469 6669 6572 7322 2c0d 0a20 2020  modifiers",..   
-00002340: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00002350: 3a20 302e 352c 0d0a 2020 2020 2020 2020  : 0.5,..        
-00002360: 2020 2020 2274 6572 6d73 223a 205b 226d      "terms": ["m
-00002370: 6564 696f 222c 2022 4d65 6469 6f22 2c20  edio", "Medio", 
-00002380: 224d 4544 494f 222c 2022 6d65 6469 6f73  "MEDIO", "medios
-00002390: 222c 2022 4d65 6469 6f73 222c 2022 4d45  ", "Medios", "ME
-000023a0: 4449 4f53 222c 2022 6d65 6469 6122 2c20  DIOS", "media", 
-000023b0: 224d 6564 6961 222c 2022 4d45 4449 4122  "Media", "MEDIA"
-000023c0: 2c20 226d 6564 6961 7322 2c20 224d 6564  , "medias", "Med
-000023d0: 6961 7322 2c20 224d 4544 4941 5322 2c20  ias", "MEDIAS", 
-000023e0: 226d 6974 6164 222c 2022 4d69 7461 6422  "mitad", "Mitad"
-000023f0: 2c20 224d 4954 4144 222c 2022 6d69 7461  , "MITAD", "mita
-00002400: 6473 222c 2022 4d69 7461 6473 222c 2022  ds", "Mitads", "
-00002410: 4d49 5441 4453 225d 0d0a 2020 2020 2020  MITADS"]..      
-00002420: 2020 7d2c 0d0a 2020 2020 2020 2020 2274    },..        "t
-00002430: 6869 7264 223a 207b 0d0a 2020 2020 2020  hird": {..      
-00002440: 2020 2020 2020 2274 7970 6522 3a20 226d        "type": "m
-00002450: 6f64 6966 6965 7273 222c 0d0a 2020 2020  odifiers",..    
-00002460: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-00002470: 2022 312f 3322 2c0d 0a20 2020 2020 2020   "1/3",..       
-00002480: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-00002490: 7465 7263 696f 222c 2022 5465 7263 696f  tercio", "Tercio
-000024a0: 222c 2022 5445 5243 494f 222c 2022 7465  ", "TERCIO", "te
-000024b0: 7263 696f 7322 2c20 2254 6572 6369 6f73  rcios", "Tercios
-000024c0: 222c 2022 5445 5243 494f 5322 2c20 2274  ", "TERCIOS", "t
-000024d0: 6572 6365 726f 222c 2022 5465 7263 6572  ercero", "Tercer
-000024e0: 6f22 2c20 2254 4552 4345 524f 222c 2022  o", "TERCERO", "
-000024f0: 7465 7263 6572 6f73 222c 2022 5465 7263  terceros", "Terc
-00002500: 6572 6f73 222c 2022 5445 5243 4552 4f53  eros", "TERCEROS
-00002510: 222c 2022 7465 7263 6572 6122 2c20 2254  ", "tercera", "T
-00002520: 6572 6365 7261 222c 2022 5445 5243 4552  ercera", "TERCER
-00002530: 4122 2c20 2274 6572 6365 7261 7322 2c20  A", "terceras", 
-00002540: 2254 6572 6365 7261 7322 2c20 2254 4552  "Terceras", "TER
-00002550: 4345 5241 5322 5d0d 0a20 2020 2020 2020  CERAS"]..       
-00002560: 207d 2c0d 0a20 2020 2020 2020 2022 7175   },..        "qu
-00002570: 6172 7465 7222 3a20 7b0d 0a20 2020 2020  arter": {..     
-00002580: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00002590: 6d6f 6469 6669 6572 7322 2c0d 0a20 2020  modifiers",..   
-000025a0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-000025b0: 3a20 302e 3235 2c0d 0a20 2020 2020 2020  : 0.25,..       
-000025c0: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
-000025d0: 6375 6172 746f 222c 2022 4375 6172 746f  cuarto", "Cuarto
-000025e0: 222c 2022 4355 4152 544f 222c 2022 6375  ", "CUARTO", "cu
-000025f0: 6172 746f 7322 2c20 2243 7561 7274 6f73  artos", "Cuartos
-00002600: 222c 2022 4355 4152 544f 5322 5d0d 0a20  ", "CUARTOS"].. 
-00002610: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00002620: 2020 2022 6d75 6c74 6970 6c69 6572 223a     "multiplier":
-00002630: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00002640: 2274 7970 6522 3a20 226d 756c 7469 706c  "type": "multipl
-00002650: 6965 7222 2c0d 0a20 2020 2020 2020 2020  ier",..         
-00002660: 2020 2022 7661 6c75 6522 3a20 2d31 2e30     "value": -1.0
-00002670: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002680: 7465 726d 7322 3a20 5b22 6465 222c 2022  terms": ["de", "
-00002690: 4465 222c 2022 4445 225d 0d0a 2020 2020  De", "DE"]..    
-000026a0: 2020 2020 7d0d 0a20 2020 207d 2c0d 0a20      }..    },.. 
-000026b0: 2020 2022 7363 616c 6573 223a 207b 0d0a     "scales": {..
-000026c0: 2020 2020 2020 2020 226d 696c 6c69 7365          "millise
-000026d0: 636f 6e64 223a 207b 0d0a 2020 2020 2020  cond": {..      
-000026e0: 2020 2020 2020 2273 6361 6c65 223a 2030        "scale": 0
-000026f0: 2e30 3031 2c0d 0a20 2020 2020 2020 2020  .001,..         
-00002700: 2020 2022 7369 6e67 756c 6172 223a 2022     "singular": "
-00002710: 6d69 6c69 7365 6775 6e64 6f22 2c0d 0a20  milisegundo",.. 
-00002720: 2020 2020 2020 2020 2020 2022 706c 7572             "plur
-00002730: 616c 223a 2022 6d69 6c69 7365 6775 6e64  al": "milisegund
-00002740: 6f73 222c 0d0a 2020 2020 2020 2020 2020  os",..          
-00002750: 2020 2274 6572 6d73 223a 205b 226d 7322    "terms": ["ms"
-00002760: 2c20 224d 7322 2c20 224d 5322 2c20 226d  , "Ms", "MS", "m
-00002770: 696c 6973 6567 756e 646f 222c 2022 4d69  ilisegundo", "Mi
-00002780: 6c69 7365 6775 6e64 6f22 2c20 224d 494c  lisegundo", "MIL
-00002790: 4953 4547 554e 444f 222c 2022 6d69 6c69  ISEGUNDO", "mili
-000027a0: 7365 6775 6e64 6f73 222c 2022 4d69 6c69  segundos", "Mili
-000027b0: 7365 6775 6e64 6f73 222c 2022 4d49 4c49  segundos", "MILI
-000027c0: 5345 4755 4e44 4f53 225d 0d0a 2020 2020  SEGUNDOS"]..    
-000027d0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-000027e0: 2273 6563 6f6e 6422 3a20 7b0d 0a20 2020  "second": {..   
-000027f0: 2020 2020 2020 2020 2022 7363 616c 6522           "scale"
-00002800: 3a20 312e 302c 0d0a 2020 2020 2020 2020  : 1.0,..        
-00002810: 2020 2020 2273 696e 6775 6c61 7222 3a20      "singular": 
-00002820: 2273 6567 756e 646f 222c 0d0a 2020 2020  "segundo",..    
-00002830: 2020 2020 2020 2020 2270 6c75 7261 6c22          "plural"
-00002840: 3a20 2273 6567 756e 646f 7322 2c0d 0a20  : "segundos",.. 
-00002850: 2020 2020 2020 2020 2020 2022 7465 726d             "term
-00002860: 7322 3a20 5b22 7322 2c20 2253 222c 2022  s": ["s", "S", "
-00002870: 7365 6722 2c20 2253 6567 222c 2022 5345  seg", "Seg", "SE
-00002880: 4722 2c20 2273 6567 7322 2c20 2253 6567  G", "segs", "Seg
-00002890: 7322 2c20 2253 4547 5322 2c20 2273 6567  s", "SEGS", "seg
-000028a0: 756e 646f 222c 2022 5365 6775 6e64 6f22  undo", "Segundo"
-000028b0: 2c20 2253 4547 554e 444f 222c 2022 7365  , "SEGUNDO", "se
-000028c0: 6775 6e64 6f73 222c 2022 5365 6775 6e64  gundos", "Segund
-000028d0: 6f73 222c 2022 5345 4755 4e44 4f53 225d  os", "SEGUNDOS"]
-000028e0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000028f0: 2020 2020 2020 226d 696e 7574 6522 3a20        "minute": 
-00002900: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00002910: 7363 616c 6522 3a20 3630 2e30 2c0d 0a20  scale": 60.0,.. 
-00002920: 2020 2020 2020 2020 2020 2022 7369 6e67             "sing
-00002930: 756c 6172 223a 2022 6d69 6e75 746f 222c  ular": "minuto",
-00002940: 0d0a 2020 2020 2020 2020 2020 2020 2270  ..            "p
-00002950: 6c75 7261 6c22 3a20 226d 696e 7574 6f73  lural": "minutos
-00002960: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002970: 2274 6572 6d73 223a 205b 226d 222c 2022  "terms": ["m", "
-00002980: 6d69 6e22 2c20 224d 696e 222c 2022 4d49  min", "Min", "MI
-00002990: 4e22 2c20 226d 696e 7322 2c20 224d 696e  N", "mins", "Min
-000029a0: 7322 2c20 224d 494e 5322 2c20 226d 696e  s", "MINS", "min
-000029b0: 7574 6f22 2c20 224d 696e 7574 6f22 2c20  uto", "Minuto", 
-000029c0: 224d 494e 5554 4f22 2c20 226d 696e 7574  "MINUTO", "minut
-000029d0: 6f73 222c 2022 4d69 6e75 746f 7322 2c20  os", "Minutos", 
-000029e0: 224d 494e 5554 4f53 225d 0d0a 2020 2020  "MINUTOS"]..    
-000029f0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00002a00: 2268 6f75 7222 3a20 7b0d 0a20 2020 2020  "hour": {..     
-00002a10: 2020 2020 2020 2022 7363 616c 6522 3a20         "scale": 
-00002a20: 3336 3030 2e30 2c0d 0a20 2020 2020 2020  3600.0,..       
-00002a30: 2020 2020 2022 7369 6e67 756c 6172 223a       "singular":
-00002a40: 2022 686f 7261 222c 0d0a 2020 2020 2020   "hora",..      
-00002a50: 2020 2020 2020 2270 6c75 7261 6c22 3a20        "plural": 
-00002a60: 2268 6f72 6173 222c 0d0a 2020 2020 2020  "horas",..      
-00002a70: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00002a80: 2268 222c 2022 4822 2c20 2268 7222 2c20  "h", "H", "hr", 
-00002a90: 2248 7222 2c20 2248 5222 2c20 2268 7273  "Hr", "HR", "hrs
-00002aa0: 222c 2022 4872 7322 2c20 2248 5253 222c  ", "Hrs", "HRS",
-00002ab0: 2022 686f 7261 222c 2022 486f 7261 222c   "hora", "Hora",
-00002ac0: 2022 484f 5241 222c 2022 686f 7261 7322   "HORA", "horas"
-00002ad0: 2c20 2248 6f72 6173 222c 2022 484f 5241  , "Horas", "HORA
-00002ae0: 5322 5d0d 0a20 2020 2020 2020 207d 2c0d  S"]..        },.
-00002af0: 0a20 2020 2020 2020 2022 6461 7922 3a20  .        "day": 
-00002b00: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00002b10: 7363 616c 6522 3a20 3836 3430 302e 302c  scale": 86400.0,
-00002b20: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-00002b30: 696e 6775 6c61 7222 3a20 2264 6961 222c  ingular": "dia",
-00002b40: 0d0a 2020 2020 2020 2020 2020 2020 2270  ..            "p
-00002b50: 6c75 7261 6c22 3a20 2264 6961 7322 2c0d  lural": "dias",.
-00002b60: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00002b70: 726d 7322 3a20 5b22 6422 2c20 2264 6961  rms": ["d", "dia
-00002b80: 222c 2022 4469 6122 2c20 2244 4941 222c  ", "Dia", "DIA",
-00002b90: 2022 6469 6173 222c 2022 4469 6173 222c   "dias", "Dias",
-00002ba0: 2022 4449 4153 225d 0d0a 2020 2020 2020   "DIAS"]..      
-00002bb0: 2020 7d2c 0d0a 2020 2020 2020 2020 2277    },..        "w
-00002bc0: 6565 6b22 3a20 7b0d 0a20 2020 2020 2020  eek": {..       
-00002bd0: 2020 2020 2022 7363 616c 6522 3a20 3630       "scale": 60
-00002be0: 3438 3030 2e30 2c0d 0a20 2020 2020 2020  4800.0,..       
-00002bf0: 2020 2020 2022 7369 6e67 756c 6172 223a       "singular":
-00002c00: 2022 7365 6d61 6e61 222c 0d0a 2020 2020   "semana",..    
-00002c10: 2020 2020 2020 2020 2270 6c75 7261 6c22          "plural"
-00002c20: 3a20 2273 656d 616e 6173 222c 0d0a 2020  : "semanas",..  
-00002c30: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
-00002c40: 223a 205b 2273 656d 222c 2022 5365 6d22  ": ["sem", "Sem"
-00002c50: 2c20 2253 454d 222c 2022 7365 6d61 6e61  , "SEM", "semana
-00002c60: 222c 2022 5365 6d61 6e61 222c 2022 5345  ", "Semana", "SE
-00002c70: 4d41 4e41 222c 2022 7365 6d61 6e61 7322  MANA", "semanas"
-00002c80: 2c20 2253 656d 616e 6173 222c 2022 5345  , "Semanas", "SE
-00002c90: 4d41 4e41 5322 5d0d 0a20 2020 2020 2020  MANAS"]..       
-00002ca0: 207d 2c0d 0a20 2020 2020 2020 2022 6d6f   },..        "mo
-00002cb0: 6e74 6822 3a20 7b0d 0a20 2020 2020 2020  nth": {..       
-00002cc0: 2020 2020 2022 7363 616c 6522 3a20 3236       "scale": 26
-00002cd0: 3335 3230 302e 302c 0d0a 2020 2020 2020  35200.0,..      
-00002ce0: 2020 2020 2020 2273 696e 6775 6c61 7222        "singular"
-00002cf0: 3a20 226d 6573 222c 0d0a 2020 2020 2020  : "mes",..      
-00002d00: 2020 2020 2020 2270 6c75 7261 6c22 3a20        "plural": 
-00002d10: 226d 6573 6573 222c 0d0a 2020 2020 2020  "meses",..      
-00002d20: 2020 2020 2020 2274 6572 6d73 223a 205b        "terms": [
-00002d30: 224d 222c 2022 6d65 7322 2c20 224d 6573  "M", "mes", "Mes
-00002d40: 222c 2022 4d45 5322 2c20 226d 6573 6573  ", "MES", "meses
-00002d50: 222c 2022 4d65 7365 7322 2c20 224d 4553  ", "Meses", "MES
-00002d60: 4553 222c 2022 6d6f 222c 2022 4d6f 222c  ES", "mo", "Mo",
-00002d70: 2022 4d4f 222c 2022 6d6f 7322 2c20 224d   "MO", "mos", "M
-00002d80: 6f73 222c 2022 4d4f 5322 5d0d 0a20 2020  os", "MOS"]..   
-00002d90: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00002da0: 2022 7965 6172 223a 207b 0d0a 2020 2020   "year": {..    
-00002db0: 2020 2020 2020 2020 2273 6361 6c65 223a          "scale":
-00002dc0: 2033 3135 3336 3030 302e 302c 0d0a 2020   31536000.0,..  
-00002dd0: 2020 2020 2020 2020 2020 2273 696e 6775            "singu
-00002de0: 6c61 7222 3a20 2261 6e6f 222c 0d0a 2020  lar": "ano",..  
-00002df0: 2020 2020 2020 2020 2020 2270 6c75 7261            "plura
-00002e00: 6c22 3a20 2261 6e6f 7322 2c0d 0a20 2020  l": "anos",..   
-00002e10: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
-00002e20: 3a20 5b22 6122 2c20 2241 222c 2022 616e  : ["a", "A", "an
-00002e30: 6f22 2c20 2241 6e6f 222c 2022 414e 4f22  o", "Ano", "ANO"
-00002e40: 2c20 2261 6e6f 7322 2c20 2241 6e6f 7322  , "anos", "Anos"
-00002e50: 2c20 2241 4e4f 5322 5d0d 0a20 2020 2020  , "ANOS"]..     
-00002e60: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
-00002e70: 6465 6361 6465 223a 207b 0d0a 2020 2020  decade": {..    
-00002e80: 2020 2020 2020 2020 2273 6361 6c65 223a          "scale":
-00002e90: 2033 3135 3336 3030 3030 2e30 2c0d 0a20   315360000.0,.. 
-00002ea0: 2020 2020 2020 2020 2020 2022 7369 6e67             "sing
-00002eb0: 756c 6172 223a 2022 6465 6361 6461 222c  ular": "decada",
-00002ec0: 0d0a 2020 2020 2020 2020 2020 2020 2270  ..            "p
-00002ed0: 6c75 7261 6c22 3a20 2264 6563 6164 6173  lural": "decadas
-00002ee0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002ef0: 2274 6572 6d73 223a 205b 2244 222c 2022  "terms": ["D", "
-00002f00: 6465 6322 2c20 2244 6563 222c 2022 4445  dec", "Dec", "DE
-00002f10: 4322 2c20 2264 6563 7322 2c20 2244 6563  C", "decs", "Dec
-00002f20: 7322 2c20 2244 4543 5322 2c20 2264 6563  s", "DECS", "dec
-00002f30: 6164 6122 2c20 2244 6563 6164 6122 2c20  ada", "Decada", 
-00002f40: 2244 4543 4144 4122 2c20 2264 6563 6164  "DECADA", "decad
-00002f50: 6173 222c 2022 4465 6361 6461 7322 2c20  as", "Decadas", 
-00002f60: 2244 4543 4144 4153 225d 0d0a 2020 2020  "DECADAS"]..    
-00002f70: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00002f80: 2263 656e 7475 7279 223a 207b 0d0a 2020  "century": {..  
-00002f90: 2020 2020 2020 2020 2020 2273 6361 6c65            "scale
-00002fa0: 223a 2033 3135 3336 3030 3030 302e 302c  ": 3153600000.0,
-00002fb0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-00002fc0: 696e 6775 6c61 7222 3a20 2273 6967 6c6f  ingular": "siglo
-00002fd0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002fe0: 2270 6c75 7261 6c22 3a20 2273 6967 6c6f  "plural": "siglo
-00002ff0: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00003000: 2022 7465 726d 7322 3a20 5b22 6322 2c20   "terms": ["c", 
-00003010: 2243 222c 2022 7369 676c 6f22 2c20 2253  "C", "siglo", "S
-00003020: 6967 6c6f 222c 2022 5349 474c 4f22 2c20  iglo", "SIGLO", 
-00003030: 2273 6967 6c6f 7322 2c20 2253 6967 6c6f  "siglos", "Siglo
-00003040: 7322 2c20 2253 4947 4c4f 5322 5d0d 0a20  s", "SIGLOS"].. 
-00003050: 2020 2020 2020 207d 0d0a 2020 2020 7d2c         }..    },
-00003060: 0d0a 2020 2020 2265 7874 7261 5f64 6174  ..    "extra_dat
-00003070: 6122 3a20 7b0d 0a20 2020 207d 0d0a 7d0d  a": {..    }..}.
-00003080: 0a                                       .
+00000000: 7b0a 2020 2020 2263 6f6e 6e65 6374 6f72  {.    "connector
+00000010: 7322 3a20 5b22 2022 2c20 225c 7422 2c20  s": [" ", "\t", 
+00000020: 222d 225d 2c0a 2020 2020 2273 6567 6d65  "-"],.    "segme
+00000030: 6e74 6f72 7322 3a20 5b22 2c22 2c20 2279  ntors": [",", "y
+00000040: 222c 2022 2622 5d2c 0a20 2020 2022 616c  ", "&"],.    "al
+00000050: 6c6f 7765 645f 7465 726d 7322 3a20 5b22  lowed_terms": ["
+00000060: 2122 2c20 22c2 bf22 2c20 223f 222c 2022  !", "..", "?", "
+00000070: 2722 2c20 222e 222c 2022 2c22 2c20 226c  '", ".", ",", "l
+00000080: 6122 2c20 226c 6522 2c20 226c 6f22 2c20  a", "le", "lo", 
+00000090: 226c 6173 222c 2022 6c65 7322 2c20 226c  "las", "les", "l
+000000a0: 6f73 225d 2c0a 2020 2020 2264 6563 696d  os"],.    "decim
+000000b0: 616c 5f73 6570 6172 6174 6f72 7322 3a20  al_separators": 
+000000c0: 5b22 2c22 5d2c 0a20 2020 2022 7468 6f75  [","],.    "thou
+000000d0: 7361 6e64 5f73 6570 6172 6174 6f72 7322  sand_separators"
+000000e0: 3a20 5b22 2e22 2c20 2220 225d 2c0a 2020  : [".", " "],.  
+000000f0: 2020 2270 6172 7365 725f 6669 6c65 223a    "parser_file":
+00000100: 2022 7061 7273 6572 5f6f 6e65 2e70 7922   "parser_one.py"
+00000110: 2c0a 2020 2020 226e 756d 6572 616c 7322  ,.    "numerals"
+00000120: 3a20 7b0a 2020 2020 2020 2020 227a 6572  : {.        "zer
+00000130: 6f22 3a20 7b0a 2020 2020 2020 2020 2020  o": {.          
+00000140: 2020 2274 7970 6522 3a20 2264 6967 6974    "type": "digit
+00000150: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00000160: 2276 616c 7565 223a 2030 2e30 2c0a 2020  "value": 0.0,.  
+00000170: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
+00000180: 223a 205b 2263 6572 6f22 2c20 2243 6572  ": ["cero", "Cer
+00000190: 6f22 2c20 2243 4552 4f22 2c20 2263 6572  o", "CERO", "cer
+000001a0: 6f73 222c 2022 4365 726f 7322 2c20 2243  os", "Ceros", "C
+000001b0: 4552 4f53 225d 0a20 2020 2020 2020 207d  EROS"].        }
+000001c0: 2c0a 2020 2020 2020 2020 226f 6e65 223a  ,.        "one":
+000001d0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000001e0: 7479 7065 223a 2022 6469 6769 7473 222c  type": "digits",
+000001f0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00000200: 6c75 6522 3a20 312e 302c 0a20 2020 2020  lue": 1.0,.     
+00000210: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00000220: 5b22 756e 6f22 2c20 2255 6e6f 222c 2022  ["uno", "Uno", "
+00000230: 554e 4f22 2c20 2275 6e6f 7322 2c20 2255  UNO", "unos", "U
+00000240: 6e6f 7322 2c20 2255 4e4f 5322 2c20 2275  nos", "UNOS", "u
+00000250: 6e22 2c20 2255 6e22 2c20 2255 4e22 2c20  n", "Un", "UN", 
+00000260: 2275 6e73 222c 2022 556e 7322 2c20 2255  "uns", "Uns", "U
+00000270: 4e53 222c 2022 756e 6122 2c20 2255 6e61  NS", "una", "Una
+00000280: 222c 2022 554e 4122 2c20 2275 6e61 7322  ", "UNA", "unas"
+00000290: 2c20 2255 6e61 7322 2c20 2255 4e41 5322  , "Unas", "UNAS"
+000002a0: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+000002b0: 2020 2020 2022 7477 6f22 3a20 7b0a 2020       "two": {.  
+000002c0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+000002d0: 3a20 2264 6967 6974 7322 2c0a 2020 2020  : "digits",.    
+000002e0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+000002f0: 2032 2e30 2c0a 2020 2020 2020 2020 2020   2.0,.          
+00000300: 2020 2274 6572 6d73 223a 205b 2264 6f73    "terms": ["dos
+00000310: 222c 2022 446f 7322 2c20 2244 4f53 222c  ", "Dos", "DOS",
+00000320: 2022 646f 7365 7322 2c20 2244 6f73 6573   "doses", "Doses
+00000330: 222c 2022 444f 5345 5322 5d0a 2020 2020  ", "DOSES"].    
+00000340: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000350: 7468 7265 6522 3a20 7b0a 2020 2020 2020  three": {.      
+00000360: 2020 2020 2020 2274 7970 6522 3a20 2264        "type": "d
+00000370: 6967 6974 7322 2c0a 2020 2020 2020 2020  igits",.        
+00000380: 2020 2020 2276 616c 7565 223a 2033 2e30      "value": 3.0
+00000390: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+000003a0: 6572 6d73 223a 205b 2274 7265 7322 2c20  erms": ["tres", 
+000003b0: 2254 7265 7322 2c20 2254 5245 5322 2c20  "Tres", "TRES", 
+000003c0: 2274 7265 7365 7322 2c20 2254 7265 7365  "treses", "Trese
+000003d0: 7322 2c20 2254 5245 5345 5322 5d0a 2020  s", "TRESES"].  
+000003e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000003f0: 2022 666f 7572 223a 207b 0a20 2020 2020   "four": {.     
+00000400: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000410: 6469 6769 7473 222c 0a20 2020 2020 2020  digits",.       
+00000420: 2020 2020 2022 7661 6c75 6522 3a20 342e       "value": 4.
+00000430: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00000440: 7465 726d 7322 3a20 5b22 6375 6174 726f  terms": ["cuatro
+00000450: 222c 2022 4375 6174 726f 222c 2022 4355  ", "Cuatro", "CU
+00000460: 4154 524f 222c 2022 6375 6174 726f 7322  ATRO", "cuatros"
+00000470: 2c20 2243 7561 7472 6f73 222c 2022 4355  , "Cuatros", "CU
+00000480: 4154 524f 5322 5d0a 2020 2020 2020 2020  ATROS"].        
+00000490: 7d2c 0a20 2020 2020 2020 2022 6669 7665  },.        "five
+000004a0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000004b0: 2022 7479 7065 223a 2022 6469 6769 7473   "type": "digits
+000004c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000004d0: 7661 6c75 6522 3a20 352e 302c 0a20 2020  value": 5.0,.   
+000004e0: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+000004f0: 3a20 5b22 6369 6e63 6f22 2c20 2243 696e  : ["cinco", "Cin
+00000500: 636f 222c 2022 4349 4e43 4f22 2c20 2263  co", "CINCO", "c
+00000510: 696e 636f 7322 2c20 2243 696e 636f 7322  incos", "Cincos"
+00000520: 2c20 2243 494e 434f 5322 5d0a 2020 2020  , "CINCOS"].    
+00000530: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000540: 7369 7822 3a20 7b0a 2020 2020 2020 2020  six": {.        
+00000550: 2020 2020 2274 7970 6522 3a20 2264 6967      "type": "dig
+00000560: 6974 7322 2c0a 2020 2020 2020 2020 2020  its",.          
+00000570: 2020 2276 616c 7565 223a 2036 2e30 2c0a    "value": 6.0,.
+00000580: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
+00000590: 6d73 223a 205b 2273 6569 7322 2c20 2253  ms": ["seis", "S
+000005a0: 6569 7322 2c20 2253 4549 5322 2c20 2273  eis", "SEIS", "s
+000005b0: 6569 7365 7322 2c20 2253 6569 7365 7322  eises", "Seises"
+000005c0: 2c20 2253 4549 5345 5322 5d0a 2020 2020  , "SEISES"].    
+000005d0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+000005e0: 7365 7665 6e22 3a20 7b0a 2020 2020 2020  seven": {.      
+000005f0: 2020 2020 2020 2274 7970 6522 3a20 2264        "type": "d
+00000600: 6967 6974 7322 2c0a 2020 2020 2020 2020  igits",.        
+00000610: 2020 2020 2276 616c 7565 223a 2037 2e30      "value": 7.0
+00000620: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00000630: 6572 6d73 223a 205b 2273 6965 7465 222c  erms": ["siete",
+00000640: 2022 5369 6574 6522 2c20 2253 4945 5445   "Siete", "SIETE
+00000650: 222c 2022 7369 6574 6573 222c 2022 5369  ", "sietes", "Si
+00000660: 6574 6573 222c 2022 5349 4554 4553 225d  etes", "SIETES"]
+00000670: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00000680: 2020 2020 2265 6967 6874 223a 207b 0a20      "eight": {. 
+00000690: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000006a0: 223a 2022 6469 6769 7473 222c 0a20 2020  ": "digits",.   
+000006b0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+000006c0: 3a20 382e 302c 0a20 2020 2020 2020 2020  : 8.0,.         
+000006d0: 2020 2022 7465 726d 7322 3a20 5b22 6f63     "terms": ["oc
+000006e0: 686f 222c 2022 4f63 686f 222c 2022 4f43  ho", "Ocho", "OC
+000006f0: 484f 222c 2022 6f63 686f 7322 2c20 224f  HO", "ochos", "O
+00000700: 6368 6f73 222c 2022 4f43 484f 5322 5d0a  chos", "OCHOS"].
+00000710: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000720: 2020 2022 6e69 6e65 223a 207b 0a20 2020     "nine": {.   
+00000730: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000740: 2022 6469 6769 7473 222c 0a20 2020 2020   "digits",.     
+00000750: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00000760: 392e 302c 0a20 2020 2020 2020 2020 2020  9.0,.           
+00000770: 2022 7465 726d 7322 3a20 5b22 6e75 6576   "terms": ["nuev
+00000780: 6522 2c20 224e 7565 7665 222c 2022 4e55  e", "Nueve", "NU
+00000790: 4556 4522 2c20 226e 7565 7665 7322 2c20  EVE", "nueves", 
+000007a0: 224e 7565 7665 7322 2c20 224e 5545 5645  "Nueves", "NUEVE
+000007b0: 5322 5d0a 2020 2020 2020 2020 7d2c 0a20  S"].        },. 
+000007c0: 2020 2020 2020 2022 7465 6e22 3a20 7b0a         "ten": {.
+000007d0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000007e0: 6522 3a20 2274 6565 6e73 222c 0a20 2020  e": "teens",.   
+000007f0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00000800: 3a20 3130 2e30 2c0a 2020 2020 2020 2020  : 10.0,.        
+00000810: 2020 2020 2274 6572 6d73 223a 205b 2264      "terms": ["d
+00000820: 6965 7a22 2c20 2244 6965 7a22 2c20 2244  iez", "Diez", "D
+00000830: 4945 5a22 2c20 2264 6965 7322 2c20 2244  IEZ", "dies", "D
+00000840: 6965 7322 2c20 2244 4945 5322 2c20 2264  ies", "DIES", "d
+00000850: 6965 6322 2c20 2244 6965 6322 2c20 2244  iec", "Diec", "D
+00000860: 4945 4322 2c20 2264 6965 7a65 7322 2c20  IEC", "diezes", 
+00000870: 2244 6965 7a65 7322 2c20 2244 4945 5a45  "Diezes", "DIEZE
+00000880: 5322 2c20 2264 6965 7365 7322 2c20 2244  S", "dieses", "D
+00000890: 6965 7365 7322 2c20 2244 4945 5345 5322  ieses", "DIESES"
+000008a0: 2c20 2264 6965 6365 7322 2c20 2244 6965  , "dieces", "Die
+000008b0: 6365 7322 2c20 2244 4945 4345 5322 5d0a  ces", "DIECES"].
+000008c0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000008d0: 2020 2022 656c 6576 656e 223a 207b 0a20     "eleven": {. 
+000008e0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000008f0: 223a 2022 7465 656e 7322 2c0a 2020 2020  ": "teens",.    
+00000900: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+00000910: 2031 312e 302c 0a20 2020 2020 2020 2020   11.0,.         
+00000920: 2020 2022 7465 726d 7322 3a20 5b22 6f6e     "terms": ["on
+00000930: 6365 222c 2022 4f6e 6365 222c 2022 4f4e  ce", "Once", "ON
+00000940: 4345 222c 2022 6f6e 6365 7322 2c20 224f  CE", "onces", "O
+00000950: 6e63 6573 222c 2022 4f4e 4345 5322 5d0a  nces", "ONCES"].
+00000960: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000970: 2020 2022 7477 656c 7665 223a 207b 0a20     "twelve": {. 
+00000980: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00000990: 223a 2022 7465 656e 7322 2c0a 2020 2020  ": "teens",.    
+000009a0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+000009b0: 2031 322e 302c 0a20 2020 2020 2020 2020   12.0,.         
+000009c0: 2020 2022 7465 726d 7322 3a20 5b22 646f     "terms": ["do
+000009d0: 6365 222c 2022 446f 6365 222c 2022 444f  ce", "Doce", "DO
+000009e0: 4345 222c 2022 646f 6365 7322 2c20 2244  CE", "doces", "D
+000009f0: 6f63 6573 222c 2022 444f 4345 5322 5d0a  oces", "DOCES"].
+00000a00: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000a10: 2020 2022 7468 6972 7465 656e 223a 207b     "thirteen": {
+00000a20: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+00000a30: 7065 223a 2022 7465 656e 7322 2c0a 2020  pe": "teens",.  
+00000a40: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00000a50: 223a 2031 332e 302c 0a20 2020 2020 2020  ": 13.0,.       
+00000a60: 2020 2020 2022 7465 726d 7322 3a20 5b22       "terms": ["
+00000a70: 7472 6563 6522 2c20 2254 7265 6365 222c  trece", "Trece",
+00000a80: 2022 5452 4543 4522 2c20 2274 7265 6365   "TRECE", "trece
+00000a90: 7322 2c20 2254 7265 6365 7322 2c20 2254  s", "Treces", "T
+00000aa0: 5245 4345 5322 5d0a 2020 2020 2020 2020  RECES"].        
+00000ab0: 7d2c 0a20 2020 2020 2020 2022 666f 7572  },.        "four
+00000ac0: 7465 656e 223a 207b 0a20 2020 2020 2020  teen": {.       
+00000ad0: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
+00000ae0: 656e 7322 2c0a 2020 2020 2020 2020 2020  ens",.          
+00000af0: 2020 2276 616c 7565 223a 2031 342e 302c    "value": 14.0,
+00000b00: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00000b10: 726d 7322 3a20 5b22 6361 746f 7263 6522  rms": ["catorce"
+00000b20: 2c20 2243 6174 6f72 6365 222c 2022 4341  , "Catorce", "CA
+00000b30: 544f 5243 4522 2c20 2263 6174 6f72 6365  TORCE", "catorce
+00000b40: 7322 2c20 2243 6174 6f72 6365 7322 2c20  s", "Catorces", 
+00000b50: 2243 4154 4f52 4345 5322 5d0a 2020 2020  "CATORCES"].    
+00000b60: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000b70: 6669 6674 6565 6e22 3a20 7b0a 2020 2020  fifteen": {.    
+00000b80: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000b90: 2274 6565 6e73 222c 0a20 2020 2020 2020  "teens",.       
+00000ba0: 2020 2020 2022 7661 6c75 6522 3a20 3135       "value": 15
+00000bb0: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00000bc0: 2274 6572 6d73 223a 205b 2271 7569 6e63  "terms": ["quinc
+00000bd0: 6522 2c20 2251 7569 6e63 6522 2c20 2251  e", "Quince", "Q
+00000be0: 5549 4e43 4522 2c20 2271 7569 6e63 6573  UINCE", "quinces
+00000bf0: 222c 2022 5175 696e 6365 7322 2c20 2251  ", "Quinces", "Q
+00000c00: 5549 4e43 4553 225d 0a20 2020 2020 2020  UINCES"].       
+00000c10: 207d 2c0a 2020 2020 2020 2020 2273 6978   },.        "six
+00000c20: 7465 656e 223a 207b 0a20 2020 2020 2020  teen": {.       
+00000c30: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
+00000c40: 656e 7322 2c0a 2020 2020 2020 2020 2020  ens",.          
+00000c50: 2020 2276 616c 7565 223a 2031 362e 302c    "value": 16.0,
+00000c60: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00000c70: 726d 7322 3a20 5b22 6469 6563 6973 6569  rms": ["diecisei
+00000c80: 7322 2c20 2244 6965 6369 7365 6973 222c  s", "Dieciseis",
+00000c90: 2022 4449 4543 4953 4549 5322 2c20 2264   "DIECISEIS", "d
+00000ca0: 6965 6369 7365 6973 6573 222c 2022 4469  ieciseises", "Di
+00000cb0: 6563 6973 6569 7365 7322 2c20 2244 4945  eciseises", "DIE
+00000cc0: 4349 5345 4953 4553 225d 0a20 2020 2020  CISEISES"].     
+00000cd0: 2020 207d 2c0a 2020 2020 2020 2020 2273     },.        "s
+00000ce0: 6576 656e 7465 656e 223a 207b 0a20 2020  eventeen": {.   
+00000cf0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000d00: 2022 7465 656e 7322 2c0a 2020 2020 2020   "teens",.      
+00000d10: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
+00000d20: 372e 302c 0a20 2020 2020 2020 2020 2020  7.0,.           
+00000d30: 2022 7465 726d 7322 3a20 5b22 6469 6563   "terms": ["diec
+00000d40: 6973 6965 7465 222c 2022 4469 6563 6973  isiete", "Diecis
+00000d50: 6965 7465 222c 2022 4449 4543 4953 4945  iete", "DIECISIE
+00000d60: 5445 222c 2022 6469 6563 6973 6965 7465  TE", "diecisiete
+00000d70: 7322 2c20 2244 6965 6369 7369 6574 6573  s", "Diecisietes
+00000d80: 222c 2022 4449 4543 4953 4945 5445 5322  ", "DIECISIETES"
+00000d90: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00000da0: 2020 2020 2022 6569 6768 7465 656e 223a       "eighteen":
+00000db0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000dc0: 7479 7065 223a 2022 7465 656e 7322 2c0a  type": "teens",.
+00000dd0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00000de0: 7565 223a 2031 382e 302c 0a20 2020 2020  ue": 18.0,.     
+00000df0: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00000e00: 5b22 6469 6563 696f 6368 6f22 2c20 2244  ["dieciocho", "D
+00000e10: 6965 6369 6f63 686f 222c 2022 4449 4543  ieciocho", "DIEC
+00000e20: 494f 4348 4f22 2c20 2264 6965 6369 6f63  IOCHO", "diecioc
+00000e30: 686f 7322 2c20 2244 6965 6369 6f63 686f  hos", "Dieciocho
+00000e40: 7322 2c20 2244 4945 4349 4f43 484f 5322  s", "DIECIOCHOS"
+00000e50: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00000e60: 2020 2020 2022 6e69 6e65 7465 656e 223a       "nineteen":
+00000e70: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000e80: 7479 7065 223a 2022 7465 656e 7322 2c0a  type": "teens",.
+00000e90: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00000ea0: 7565 223a 2031 392e 302c 0a20 2020 2020  ue": 19.0,.     
+00000eb0: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00000ec0: 5b22 6469 6563 696e 7565 7665 222c 2022  ["diecinueve", "
+00000ed0: 4469 6563 696e 7565 7665 222c 2022 4449  Diecinueve", "DI
+00000ee0: 4543 494e 5545 5645 222c 2022 6469 6563  ECINUEVE", "diec
+00000ef0: 696e 7565 7665 7322 2c20 2244 6965 6369  inueves", "Dieci
+00000f00: 6e75 6576 6573 222c 2022 4449 4543 494e  nueves", "DIECIN
+00000f10: 5545 5645 5322 5d0a 2020 2020 2020 2020  UEVES"].        
+00000f20: 7d2c 0a20 2020 2020 2020 2022 7477 656e  },.        "twen
+00000f30: 7479 223a 207b 0a20 2020 2020 2020 2020  ty": {.         
+00000f40: 2020 2022 7479 7065 223a 2022 7465 6e73     "type": "tens
+00000f50: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000f60: 7661 6c75 6522 3a20 3230 2e30 2c0a 2020  value": 20.0,.  
+00000f70: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
+00000f80: 223a 205b 2276 6569 6e74 6522 2c20 2256  ": ["veinte", "V
+00000f90: 6569 6e74 6522 2c20 2256 4549 4e54 4522  einte", "VEINTE"
+00000fa0: 2c20 2276 6569 6e74 6573 222c 2022 5665  , "veintes", "Ve
+00000fb0: 696e 7465 7322 2c20 2256 4549 4e54 4553  intes", "VEINTES
+00000fc0: 225d 0a20 2020 2020 2020 207d 2c0a 2020  "].        },.  
+00000fd0: 2020 2020 2020 2274 7765 6e74 792d 6f6e        "twenty-on
+00000fe0: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
+00000ff0: 2020 2274 7970 6522 3a20 2264 6967 6974    "type": "digit
+00001000: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00001010: 2276 616c 7565 223a 2032 312e 302c 0a20  "value": 21.0,. 
+00001020: 2020 2020 2020 2020 2020 2022 7465 726d             "term
+00001030: 7322 3a20 5b22 7665 696e 7469 756e 6f22  s": ["veintiuno"
+00001040: 2c20 2256 6569 6e74 6975 6e6f 222c 2022  , "Veintiuno", "
+00001050: 5645 494e 5449 554e 4f22 2c20 2276 6569  VEINTIUNO", "vei
+00001060: 6e74 6975 6e6f 7322 2c20 2256 6569 6e74  ntiunos", "Veint
+00001070: 6975 6e6f 7322 2c20 2256 4549 4e54 4955  iunos", "VEINTIU
+00001080: 4e4f 5322 2c20 2276 6569 6e74 6975 6e61  NOS", "veintiuna
+00001090: 222c 2022 5665 696e 7469 756e 6122 2c20  ", "Veintiuna", 
+000010a0: 2256 4549 4e54 4955 4e41 222c 2022 7665  "VEINTIUNA", "ve
+000010b0: 696e 7469 756e 6173 222c 2022 5665 696e  intiunas", "Vein
+000010c0: 7469 756e 6173 222c 2022 5645 494e 5449  tiunas", "VEINTI
+000010d0: 554e 4153 225d 0a20 2020 2020 2020 207d  UNAS"].        }
+000010e0: 2c0a 2020 2020 2020 2020 2274 7765 6e74  ,.        "twent
+000010f0: 792d 7477 6f22 3a20 7b0a 2020 2020 2020  y-two": {.      
+00001100: 2020 2020 2020 2274 7970 6522 3a20 2264        "type": "d
+00001110: 6967 6974 7322 2c0a 2020 2020 2020 2020  igits",.        
+00001120: 2020 2020 2276 616c 7565 223a 2032 322e      "value": 22.
+00001130: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00001140: 7465 726d 7322 3a20 5b22 7665 696e 7469  terms": ["veinti
+00001150: 646f 7322 2c20 2256 6569 6e74 6964 6f73  dos", "Veintidos
+00001160: 222c 2022 5645 494e 5449 444f 5322 2c20  ", "VEINTIDOS", 
+00001170: 2276 6569 6e74 6964 6f73 6573 222c 2022  "veintidoses", "
+00001180: 5665 696e 7469 646f 7365 7322 2c20 2256  Veintidoses", "V
+00001190: 4549 4e54 4944 4f53 4553 225d 0a20 2020  EINTIDOSES"].   
+000011a0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000011b0: 2274 7765 6e74 792d 7468 7265 6522 3a20  "twenty-three": 
+000011c0: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
+000011d0: 7970 6522 3a20 2264 6967 6974 7322 2c0a  ype": "digits",.
+000011e0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+000011f0: 7565 223a 2032 332e 302c 0a20 2020 2020  ue": 23.0,.     
+00001200: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00001210: 5b22 7665 696e 7469 7472 6573 222c 2022  ["veintitres", "
+00001220: 5665 696e 7469 7472 6573 222c 2022 5645  Veintitres", "VE
+00001230: 494e 5449 5452 4553 222c 2022 7665 696e  INTITRES", "vein
+00001240: 7469 7472 6573 6573 222c 2022 5665 696e  titreses", "Vein
+00001250: 7469 7472 6573 6573 222c 2022 5645 494e  titreses", "VEIN
+00001260: 5449 5452 4553 4553 225d 0a20 2020 2020  TITRESES"].     
+00001270: 2020 207d 2c0a 2020 2020 2020 2020 2274     },.        "t
+00001280: 7765 6e74 792d 666f 7572 223a 207b 0a20  wenty-four": {. 
+00001290: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000012a0: 223a 2022 6469 6769 7473 222c 0a20 2020  ": "digits",.   
+000012b0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+000012c0: 3a20 3234 2e30 2c0a 2020 2020 2020 2020  : 24.0,.        
+000012d0: 2020 2020 2274 6572 6d73 223a 205b 2276      "terms": ["v
+000012e0: 6569 6e74 6963 7561 7472 6f22 2c20 2256  einticuatro", "V
+000012f0: 6569 6e74 6963 7561 7472 6f22 2c20 2256  einticuatro", "V
+00001300: 4549 4e54 4943 5541 5452 4f22 2c20 2276  EINTICUATRO", "v
+00001310: 6569 6e74 6963 7561 7472 6f73 222c 2022  einticuatros", "
+00001320: 5665 696e 7469 6375 6174 726f 7322 2c20  Veinticuatros", 
+00001330: 2256 4549 4e54 4943 5541 5452 4f53 225d  "VEINTICUATROS"]
+00001340: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001350: 2020 2020 2274 7765 6e74 792d 6669 7665      "twenty-five
+00001360: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00001370: 2022 7479 7065 223a 2022 6469 6769 7473   "type": "digits
+00001380: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00001390: 7661 6c75 6522 3a20 3235 2e30 2c0a 2020  value": 25.0,.  
+000013a0: 2020 2020 2020 2020 2020 2274 6572 6d73            "terms
+000013b0: 223a 205b 2276 6569 6e74 6963 696e 636f  ": ["veinticinco
+000013c0: 222c 2022 5665 696e 7469 6369 6e63 6f22  ", "Veinticinco"
+000013d0: 2c20 2256 4549 4e54 4943 494e 434f 222c  , "VEINTICINCO",
+000013e0: 2022 7665 696e 7469 6369 6e63 6f73 222c   "veinticincos",
+000013f0: 2022 5665 696e 7469 6369 6e63 6f73 222c   "Veinticincos",
+00001400: 2022 5645 494e 5449 4349 4e43 4f53 225d   "VEINTICINCOS"]
+00001410: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001420: 2020 2020 2274 7765 6e74 792d 7369 7822      "twenty-six"
+00001430: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001440: 2274 7970 6522 3a20 2264 6967 6974 7322  "type": "digits"
+00001450: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+00001460: 616c 7565 223a 2032 362e 302c 0a20 2020  alue": 26.0,.   
+00001470: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+00001480: 3a20 5b22 7665 696e 7469 7365 6973 222c  : ["veintiseis",
+00001490: 2022 5665 696e 7469 7365 6973 222c 2022   "Veintiseis", "
+000014a0: 5645 494e 5449 5345 4953 222c 2022 7665  VEINTISEIS", "ve
+000014b0: 696e 7469 7365 6973 6573 222c 2022 5665  intiseises", "Ve
+000014c0: 696e 7469 7365 6973 6573 222c 2022 5645  intiseises", "VE
+000014d0: 494e 5449 5345 4953 4553 225d 0a20 2020  INTISEISES"].   
+000014e0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000014f0: 2274 7765 6e74 792d 7365 7665 6e22 3a20  "twenty-seven": 
+00001500: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
+00001510: 7970 6522 3a20 2264 6967 6974 7322 2c0a  ype": "digits",.
+00001520: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00001530: 7565 223a 2032 372e 302c 0a20 2020 2020  ue": 27.0,.     
+00001540: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00001550: 5b22 7665 696e 7469 7369 6574 6522 2c20  ["veintisiete", 
+00001560: 2256 6569 6e74 6973 6965 7465 222c 2022  "Veintisiete", "
+00001570: 5645 494e 5449 5349 4554 4522 2c20 2276  VEINTISIETE", "v
+00001580: 6569 6e74 6973 6965 7465 7322 2c20 2256  eintisietes", "V
+00001590: 6569 6e74 6973 6965 7465 7322 2c20 2256  eintisietes", "V
+000015a0: 4549 4e54 4953 4945 5445 5322 5d0a 2020  EINTISIETES"].  
+000015b0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000015c0: 2022 7477 656e 7479 2d65 6967 6874 223a   "twenty-eight":
+000015d0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000015e0: 7479 7065 223a 2022 6469 6769 7473 222c  type": "digits",
+000015f0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00001600: 6c75 6522 3a20 3238 2e30 2c0a 2020 2020  lue": 28.0,.    
+00001610: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00001620: 205b 2276 6569 6e74 696f 6368 6f22 2c20   ["veintiocho", 
+00001630: 2256 6569 6e74 696f 6368 6f22 2c20 2256  "Veintiocho", "V
+00001640: 4549 4e54 494f 4348 4f22 2c20 2276 6569  EINTIOCHO", "vei
+00001650: 6e74 696f 6368 6f73 222c 2022 5665 696e  ntiochos", "Vein
+00001660: 7469 6f63 686f 7322 2c20 2256 4549 4e54  tiochos", "VEINT
+00001670: 494f 4348 4f53 225d 0a20 2020 2020 2020  IOCHOS"].       
+00001680: 207d 2c0a 2020 2020 2020 2020 2274 7765   },.        "twe
+00001690: 6e74 792d 6e69 6e65 223a 207b 0a20 2020  nty-nine": {.   
+000016a0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000016b0: 2022 6469 6769 7473 222c 0a20 2020 2020   "digits",.     
+000016c0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000016d0: 3239 2e30 2c0a 2020 2020 2020 2020 2020  29.0,.          
+000016e0: 2020 2274 6572 6d73 223a 205b 2276 6569    "terms": ["vei
+000016f0: 6e74 696e 7565 7665 222c 2022 5665 696e  ntinueve", "Vein
+00001700: 7469 6e75 6576 6522 2c20 2256 4549 4e54  tinueve", "VEINT
+00001710: 494e 5545 5645 222c 2022 7665 696e 7469  INUEVE", "veinti
+00001720: 6e75 6576 6573 222c 2022 5665 696e 7469  nueves", "Veinti
+00001730: 6e75 6576 6573 222c 2022 5645 494e 5449  nueves", "VEINTI
+00001740: 4e55 4556 4553 225d 0a20 2020 2020 2020  NUEVES"].       
+00001750: 207d 2c0a 2020 2020 2020 2020 2274 6869   },.        "thi
+00001760: 7274 7922 3a20 7b0a 2020 2020 2020 2020  rty": {.        
+00001770: 2020 2020 2274 7970 6522 3a20 2274 656e      "type": "ten
+00001780: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00001790: 2276 616c 7565 223a 2033 302e 302c 0a20  "value": 30.0,. 
+000017a0: 2020 2020 2020 2020 2020 2022 7465 726d             "term
+000017b0: 7322 3a20 5b22 7472 6569 6e74 6122 2c20  s": ["treinta", 
+000017c0: 2254 7265 696e 7461 222c 2022 5452 4549  "Treinta", "TREI
+000017d0: 4e54 4122 2c20 2274 7265 696e 7461 7322  NTA", "treintas"
+000017e0: 2c20 2254 7265 696e 7461 7322 2c20 2254  , "Treintas", "T
+000017f0: 5245 494e 5441 5322 5d0a 2020 2020 2020  REINTAS"].      
+00001800: 2020 7d2c 0a20 2020 2020 2020 2022 666f    },.        "fo
+00001810: 7274 7922 3a20 7b0a 2020 2020 2020 2020  rty": {.        
+00001820: 2020 2020 2274 7970 6522 3a20 2274 656e      "type": "ten
+00001830: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00001840: 2276 616c 7565 223a 2034 302e 302c 0a20  "value": 40.0,. 
+00001850: 2020 2020 2020 2020 2020 2022 7465 726d             "term
+00001860: 7322 3a20 5b22 6375 6172 656e 7461 222c  s": ["cuarenta",
+00001870: 2022 4375 6172 656e 7461 222c 2022 4355   "Cuarenta", "CU
+00001880: 4152 454e 5441 222c 2022 6375 6172 656e  ARENTA", "cuaren
+00001890: 7461 7322 2c20 2243 7561 7265 6e74 6173  tas", "Cuarentas
+000018a0: 222c 2022 4355 4152 454e 5441 5322 5d0a  ", "CUARENTAS"].
+000018b0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000018c0: 2020 2022 6669 6674 7922 3a20 7b0a 2020     "fifty": {.  
+000018d0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+000018e0: 3a20 2274 656e 7322 2c0a 2020 2020 2020  : "tens",.      
+000018f0: 2020 2020 2020 2276 616c 7565 223a 2035        "value": 5
+00001900: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+00001910: 2022 7465 726d 7322 3a20 5b22 6369 6e63   "terms": ["cinc
+00001920: 7565 6e74 6122 2c20 2243 696e 6375 656e  uenta", "Cincuen
+00001930: 7461 222c 2022 4349 4e43 5545 4e54 4122  ta", "CINCUENTA"
+00001940: 2c20 2263 696e 6375 656e 7461 7322 2c20  , "cincuentas", 
+00001950: 2243 696e 6375 656e 7461 7322 2c20 2243  "Cincuentas", "C
+00001960: 494e 4355 454e 5441 5322 5d0a 2020 2020  INCUENTAS"].    
+00001970: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00001980: 7369 7874 7922 3a20 7b0a 2020 2020 2020  sixty": {.      
+00001990: 2020 2020 2020 2274 7970 6522 3a20 2274        "type": "t
+000019a0: 656e 7322 2c0a 2020 2020 2020 2020 2020  ens",.          
+000019b0: 2020 2276 616c 7565 223a 2036 302e 302c    "value": 60.0,
+000019c0: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+000019d0: 726d 7322 3a20 5b22 7365 7365 6e74 6122  rms": ["sesenta"
+000019e0: 2c20 2253 6573 656e 7461 222c 2022 5345  , "Sesenta", "SE
+000019f0: 5345 4e54 4122 2c20 2273 6573 656e 7461  SENTA", "sesenta
+00001a00: 7322 2c20 2253 6573 656e 7461 7322 2c20  s", "Sesentas", 
+00001a10: 2253 4553 454e 5441 5322 5d0a 2020 2020  "SESENTAS"].    
+00001a20: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00001a30: 7365 7665 6e74 7922 3a20 7b0a 2020 2020  seventy": {.    
+00001a40: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00001a50: 2274 656e 7322 2c0a 2020 2020 2020 2020  "tens",.        
+00001a60: 2020 2020 2276 616c 7565 223a 2037 302e      "value": 70.
+00001a70: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00001a80: 7465 726d 7322 3a20 5b22 7365 7465 6e74  terms": ["setent
+00001a90: 6122 2c20 2253 6574 656e 7461 222c 2022  a", "Setenta", "
+00001aa0: 5345 5445 4e54 4122 2c20 2273 6574 656e  SETENTA", "seten
+00001ab0: 7461 7322 2c20 2253 6574 656e 7461 7322  tas", "Setentas"
+00001ac0: 2c20 2253 4554 454e 5441 5322 5d0a 2020  , "SETENTAS"].  
+00001ad0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001ae0: 2022 6569 6768 7479 223a 207b 0a20 2020   "eighty": {.   
+00001af0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00001b00: 2022 7465 6e73 222c 0a20 2020 2020 2020   "tens",.       
+00001b10: 2020 2020 2022 7661 6c75 6522 3a20 3830       "value": 80
+00001b20: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00001b30: 2274 6572 6d73 223a 205b 226f 6368 656e  "terms": ["ochen
+00001b40: 7461 222c 2022 4f63 6865 6e74 6122 2c20  ta", "Ochenta", 
+00001b50: 224f 4348 454e 5441 222c 2022 6f63 6865  "OCHENTA", "oche
+00001b60: 6e74 6173 222c 2022 4f63 6865 6e74 6173  ntas", "Ochentas
+00001b70: 222c 2022 4f43 4845 4e54 4153 225d 0a20  ", "OCHENTAS"]. 
+00001b80: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001b90: 2020 226e 696e 6574 7922 3a20 7b0a 2020    "ninety": {.  
+00001ba0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00001bb0: 3a20 2274 656e 7322 2c0a 2020 2020 2020  : "tens",.      
+00001bc0: 2020 2020 2020 2276 616c 7565 223a 2039        "value": 9
+00001bd0: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+00001be0: 2022 7465 726d 7322 3a20 5b22 6e6f 7665   "terms": ["nove
+00001bf0: 6e74 6122 2c20 224e 6f76 656e 7461 222c  nta", "Noventa",
+00001c00: 2022 4e4f 5645 4e54 4122 2c20 226e 6f76   "NOVENTA", "nov
+00001c10: 656e 7461 7322 2c20 224e 6f76 656e 7461  entas", "Noventa
+00001c20: 7322 2c20 224e 4f56 454e 5441 5322 5d0a  s", "NOVENTAS"].
+00001c30: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001c40: 2020 2022 6875 6e64 7265 6422 3a20 7b0a     "hundred": {.
+00001c50: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00001c60: 6522 3a20 2274 686f 7573 616e 6473 222c  e": "thousands",
+00001c70: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00001c80: 6c75 6522 3a20 3130 302e 302c 0a20 2020  lue": 100.0,.   
+00001c90: 2020 2020 2020 2020 2022 7465 726d 7322           "terms"
+00001ca0: 3a20 5b22 6369 656e 222c 2022 4369 656e  : ["cien", "Cien
+00001cb0: 222c 2022 4349 454e 222c 2022 6369 656e  ", "CIEN", "cien
+00001cc0: 7322 2c20 2243 6965 6e73 222c 2022 4349  s", "Ciens", "CI
+00001cd0: 454e 5322 2c20 2263 6965 6e65 7322 2c20  ENS", "cienes", 
+00001ce0: 2243 6965 6e65 7322 2c20 2243 4945 4e45  "Cienes", "CIENE
+00001cf0: 5322 2c20 2263 6965 6e74 6f73 222c 2022  S", "cientos", "
+00001d00: 4369 656e 746f 7322 2c20 2243 4945 4e54  Cientos", "CIENT
+00001d10: 4f53 225d 0a20 2020 2020 2020 207d 2c0a  OS"].        },.
+00001d20: 2020 2020 2020 2020 2274 686f 7573 616e          "thousan
+00001d30: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
+00001d40: 2020 2274 7970 6522 3a20 2274 686f 7573    "type": "thous
+00001d50: 616e 6473 222c 0a20 2020 2020 2020 2020  ands",.         
+00001d60: 2020 2022 7661 6c75 6522 3a20 3130 3030     "value": 1000
+00001d70: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00001d80: 2274 6572 6d73 223a 205b 226d 696c 222c  "terms": ["mil",
+00001d90: 2022 4d69 6c22 2c20 224d 494c 222c 2022   "Mil", "MIL", "
+00001da0: 6d69 6c73 222c 2022 4d69 6c73 222c 2022  mils", "Mils", "
+00001db0: 4d49 4c53 222c 2022 6d69 6c65 7322 2c20  MILS", "miles", 
+00001dc0: 224d 696c 6573 222c 2022 4d49 4c45 5322  "Miles", "MILES"
+00001dd0: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00001de0: 2020 2020 2022 6d69 6c6c 696f 6e22 3a20       "million": 
+00001df0: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
+00001e00: 7970 6522 3a20 2274 686f 7573 616e 6473  ype": "thousands
+00001e10: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00001e20: 7661 6c75 6522 3a20 3130 3030 3030 302e  value": 1000000.
+00001e30: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00001e40: 7465 726d 7322 3a20 5b22 6d69 6c6c 6f6e  terms": ["millon
+00001e50: 222c 2022 4d69 6c6c 6f6e 222c 2022 4d49  ", "Millon", "MI
+00001e60: 4c4c 4f4e 222c 2022 6d69 6c6c 6f6e 7322  LLON", "millons"
+00001e70: 2c20 224d 696c 6c6f 6e73 222c 2022 4d49  , "Millons", "MI
+00001e80: 4c4c 4f4e 5322 2c20 226d 696c 6c6f 6e65  LLONS", "millone
+00001e90: 7322 2c20 224d 696c 6c6f 6e65 7322 2c20  s", "Millones", 
+00001ea0: 224d 494c 4c4f 4e45 5322 5d0a 2020 2020  "MILLONES"].    
+00001eb0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00001ec0: 7472 696c 6c69 6f6e 223a 207b 0a20 2020  trillion": {.   
+00001ed0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00001ee0: 2022 7468 6f75 7361 6e64 7322 2c0a 2020   "thousands",.  
+00001ef0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00001f00: 223a 2031 3030 3030 3030 3030 3030 3030  ": 1000000000000
+00001f10: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00001f20: 2274 6572 6d73 223a 205b 2262 696c 6c6f  "terms": ["billo
+00001f30: 6e22 2c20 2242 696c 6c6f 6e22 2c20 2242  n", "Billon", "B
+00001f40: 494c 4c4f 4e22 2c20 2262 696c 6c6f 6e73  ILLON", "billons
+00001f50: 222c 2022 4269 6c6c 6f6e 7322 2c20 2242  ", "Billons", "B
+00001f60: 494c 4c4f 4e53 222c 2022 6269 6c6c 6f6e  ILLONS", "billon
+00001f70: 6573 222c 2022 4269 6c6c 6f6e 6573 222c  es", "Billones",
+00001f80: 2022 4249 4c4c 4f4e 4553 225d 0a20 2020   "BILLONES"].   
+00001f90: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001fa0: 2266 756c 6c22 3a20 7b0a 2020 2020 2020  "full": {.      
+00001fb0: 2020 2020 2020 2274 7970 6522 3a20 226d        "type": "m
+00001fc0: 6f64 6966 6965 7273 222c 0a20 2020 2020  odifiers",.     
+00001fd0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00001fe0: 312e 302c 0a20 2020 2020 2020 2020 2020  1.0,.           
+00001ff0: 2022 7465 726d 7322 3a20 5b22 636f 6d70   "terms": ["comp
+00002000: 6c65 746f 222c 2022 436f 6d70 6c65 746f  leto", "Completo
+00002010: 222c 2022 434f 4d50 4c45 544f 222c 2022  ", "COMPLETO", "
+00002020: 636f 6d70 6c65 746f 7322 2c20 2243 6f6d  completos", "Com
+00002030: 706c 6574 6f73 222c 2022 434f 4d50 4c45  pletos", "COMPLE
+00002040: 544f 5322 2c20 2263 6f6d 706c 6574 6122  TOS", "completa"
+00002050: 2c20 2243 6f6d 706c 6574 6122 2c20 2243  , "Completa", "C
+00002060: 4f4d 504c 4554 4122 2c20 2263 6f6d 706c  OMPLETA", "compl
+00002070: 6574 6173 222c 2022 436f 6d70 6c65 7461  etas", "Completa
+00002080: 7322 2c20 2243 4f4d 504c 4554 4153 222c  s", "COMPLETAS",
+00002090: 2022 746f 7461 6c22 2c20 2254 6f74 616c   "total", "Total
+000020a0: 222c 2022 544f 5441 4c22 2c20 2274 6f74  ", "TOTAL", "tot
+000020b0: 616c 6573 222c 2022 546f 7461 6c65 7322  ales", "Totales"
+000020c0: 2c20 2254 4f54 414c 4553 222c 2022 6c6c  , "TOTALES", "ll
+000020d0: 656e 6f22 2c20 224c 6c65 6e6f 222c 2022  eno", "Lleno", "
+000020e0: 4c4c 454e 4f22 2c20 226c 6c65 6e6f 7322  LLENO", "llenos"
+000020f0: 2c20 224c 6c65 6e6f 7322 2c20 224c 4c45  , "Llenos", "LLE
+00002100: 4e4f 5322 2c20 226c 6c65 6e61 222c 2022  NOS", "llena", "
+00002110: 4c6c 656e 6122 2c20 224c 4c45 4e41 222c  Llena", "LLENA",
+00002120: 2022 6c6c 656e 6173 222c 2022 4c6c 656e   "llenas", "Llen
+00002130: 6173 222c 2022 4c4c 454e 4153 222c 2022  as", "LLENAS", "
+00002140: 656e 7465 726f 222c 2022 456e 7465 726f  entero", "Entero
+00002150: 222c 2022 454e 5445 524f 222c 2022 656e  ", "ENTERO", "en
+00002160: 7465 726f 7322 2c20 2245 6e74 6572 6f73  teros", "Enteros
+00002170: 222c 2022 454e 5445 524f 5322 2c20 2265  ", "ENTEROS", "e
+00002180: 6e74 6572 6122 2c20 2245 6e74 6572 6122  ntera", "Entera"
+00002190: 2c20 2245 4e54 4552 4122 2c20 2265 6e74  , "ENTERA", "ent
+000021a0: 6572 6173 222c 2022 456e 7465 7261 7322  eras", "Enteras"
+000021b0: 2c20 2245 4e54 4552 4153 222c 2022 746f  , "ENTERAS", "to
+000021c0: 646f 222c 2022 546f 646f 222c 2022 544f  do", "Todo", "TO
+000021d0: 444f 222c 2022 746f 646f 7322 2c20 2254  DO", "todos", "T
+000021e0: 6f64 6f73 222c 2022 544f 444f 5322 2c20  odos", "TODOS", 
+000021f0: 2274 6f64 6122 2c20 2254 6f64 6122 2c20  "toda", "Toda", 
+00002200: 2254 4f44 4122 2c20 2274 6f64 6173 222c  "TODA", "todas",
+00002210: 2022 546f 6461 7322 2c20 2254 4f44 4153   "Todas", "TODAS
+00002220: 225d 0a20 2020 2020 2020 207d 2c0a 2020  "].        },.  
+00002230: 2020 2020 2020 2268 616c 6622 3a20 7b0a        "half": {.
+00002240: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00002250: 6522 3a20 226d 6f64 6966 6965 7273 222c  e": "modifiers",
+00002260: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+00002270: 6c75 6522 3a20 302e 352c 0a20 2020 2020  lue": 0.5,.     
+00002280: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00002290: 5b22 6d65 6469 6f22 2c20 224d 6564 696f  ["medio", "Medio
+000022a0: 222c 2022 4d45 4449 4f22 2c20 226d 6564  ", "MEDIO", "med
+000022b0: 696f 7322 2c20 224d 6564 696f 7322 2c20  ios", "Medios", 
+000022c0: 224d 4544 494f 5322 2c20 226d 6564 6961  "MEDIOS", "media
+000022d0: 222c 2022 4d65 6469 6122 2c20 224d 4544  ", "Media", "MED
+000022e0: 4941 222c 2022 6d65 6469 6173 222c 2022  IA", "medias", "
+000022f0: 4d65 6469 6173 222c 2022 4d45 4449 4153  Medias", "MEDIAS
+00002300: 222c 2022 6d69 7461 6422 2c20 224d 6974  ", "mitad", "Mit
+00002310: 6164 222c 2022 4d49 5441 4422 2c20 226d  ad", "MITAD", "m
+00002320: 6974 6164 7322 2c20 224d 6974 6164 7322  itads", "Mitads"
+00002330: 2c20 224d 4954 4144 5322 5d0a 2020 2020  , "MITADS"].    
+00002340: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00002350: 7468 6972 6422 3a20 7b0a 2020 2020 2020  third": {.      
+00002360: 2020 2020 2020 2274 7970 6522 3a20 226d        "type": "m
+00002370: 6f64 6966 6965 7273 222c 0a20 2020 2020  odifiers",.     
+00002380: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00002390: 2231 2f33 222c 0a20 2020 2020 2020 2020  "1/3",.         
+000023a0: 2020 2022 7465 726d 7322 3a20 5b22 7465     "terms": ["te
+000023b0: 7263 696f 222c 2022 5465 7263 696f 222c  rcio", "Tercio",
+000023c0: 2022 5445 5243 494f 222c 2022 7465 7263   "TERCIO", "terc
+000023d0: 696f 7322 2c20 2254 6572 6369 6f73 222c  ios", "Tercios",
+000023e0: 2022 5445 5243 494f 5322 2c20 2274 6572   "TERCIOS", "ter
+000023f0: 6365 726f 222c 2022 5465 7263 6572 6f22  cero", "Tercero"
+00002400: 2c20 2254 4552 4345 524f 222c 2022 7465  , "TERCERO", "te
+00002410: 7263 6572 6f73 222c 2022 5465 7263 6572  rceros", "Tercer
+00002420: 6f73 222c 2022 5445 5243 4552 4f53 222c  os", "TERCEROS",
+00002430: 2022 7465 7263 6572 6122 2c20 2254 6572   "tercera", "Ter
+00002440: 6365 7261 222c 2022 5445 5243 4552 4122  cera", "TERCERA"
+00002450: 2c20 2274 6572 6365 7261 7322 2c20 2254  , "terceras", "T
+00002460: 6572 6365 7261 7322 2c20 2254 4552 4345  erceras", "TERCE
+00002470: 5241 5322 5d0a 2020 2020 2020 2020 7d2c  RAS"].        },
+00002480: 0a20 2020 2020 2020 2022 7175 6172 7465  .        "quarte
+00002490: 7222 3a20 7b0a 2020 2020 2020 2020 2020  r": {.          
+000024a0: 2020 2274 7970 6522 3a20 226d 6f64 6966    "type": "modif
+000024b0: 6965 7273 222c 0a20 2020 2020 2020 2020  iers",.         
+000024c0: 2020 2022 7661 6c75 6522 3a20 302e 3235     "value": 0.25
+000024d0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+000024e0: 6572 6d73 223a 205b 2263 7561 7274 6f22  erms": ["cuarto"
+000024f0: 2c20 2243 7561 7274 6f22 2c20 2243 5541  , "Cuarto", "CUA
+00002500: 5254 4f22 2c20 2263 7561 7274 6f73 222c  RTO", "cuartos",
+00002510: 2022 4375 6172 746f 7322 2c20 2243 5541   "Cuartos", "CUA
+00002520: 5254 4f53 225d 0a20 2020 2020 2020 207d  RTOS"].        }
+00002530: 2c0a 2020 2020 2020 2020 226d 756c 7469  ,.        "multi
+00002540: 706c 6965 7222 3a20 7b0a 2020 2020 2020  plier": {.      
+00002550: 2020 2020 2020 2274 7970 6522 3a20 226d        "type": "m
+00002560: 756c 7469 706c 6965 7222 2c0a 2020 2020  ultiplier",.    
+00002570: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+00002580: 202d 312e 302c 0a20 2020 2020 2020 2020   -1.0,.         
+00002590: 2020 2022 7465 726d 7322 3a20 5b22 6465     "terms": ["de
+000025a0: 222c 2022 4465 222c 2022 4445 225d 0a20  ", "De", "DE"]. 
+000025b0: 2020 2020 2020 207d 0a20 2020 207d 2c0a         }.    },.
+000025c0: 2020 2020 2273 6361 6c65 7322 3a20 7b0a      "scales": {.
+000025d0: 2020 2020 2020 2020 226d 696c 6c69 7365          "millise
+000025e0: 636f 6e64 223a 207b 0a20 2020 2020 2020  cond": {.       
+000025f0: 2020 2020 2022 7363 616c 6522 3a20 302e       "scale": 0.
+00002600: 3030 312c 0a20 2020 2020 2020 2020 2020  001,.           
+00002610: 2022 7369 6e67 756c 6172 223a 2022 6d69   "singular": "mi
+00002620: 6c69 7365 6775 6e64 6f22 2c0a 2020 2020  lisegundo",.    
+00002630: 2020 2020 2020 2020 2270 6c75 7261 6c22          "plural"
+00002640: 3a20 226d 696c 6973 6567 756e 646f 7322  : "milisegundos"
+00002650: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00002660: 6572 6d73 223a 205b 226d 7322 2c20 224d  erms": ["ms", "M
+00002670: 7322 2c20 224d 5322 2c20 226d 696c 6973  s", "MS", "milis
+00002680: 6567 756e 646f 222c 2022 4d69 6c69 7365  egundo", "Milise
+00002690: 6775 6e64 6f22 2c20 224d 494c 4953 4547  gundo", "MILISEG
+000026a0: 554e 444f 222c 2022 6d69 6c69 7365 6775  UNDO", "milisegu
+000026b0: 6e64 6f73 222c 2022 4d69 6c69 7365 6775  ndos", "Milisegu
+000026c0: 6e64 6f73 222c 2022 4d49 4c49 5345 4755  ndos", "MILISEGU
+000026d0: 4e44 4f53 225d 0a20 2020 2020 2020 207d  NDOS"].        }
+000026e0: 2c0a 2020 2020 2020 2020 2273 6563 6f6e  ,.        "secon
+000026f0: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
+00002700: 2020 2273 6361 6c65 223a 2031 2e30 2c0a    "scale": 1.0,.
+00002710: 2020 2020 2020 2020 2020 2020 2273 696e              "sin
+00002720: 6775 6c61 7222 3a20 2273 6567 756e 646f  gular": "segundo
+00002730: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002740: 706c 7572 616c 223a 2022 7365 6775 6e64  plural": "segund
+00002750: 6f73 222c 0a20 2020 2020 2020 2020 2020  os",.           
+00002760: 2022 7465 726d 7322 3a20 5b22 7322 2c20   "terms": ["s", 
+00002770: 2253 222c 2022 7365 6722 2c20 2253 6567  "S", "seg", "Seg
+00002780: 222c 2022 5345 4722 2c20 2273 6567 7322  ", "SEG", "segs"
+00002790: 2c20 2253 6567 7322 2c20 2253 4547 5322  , "Segs", "SEGS"
+000027a0: 2c20 2273 6567 756e 646f 222c 2022 5365  , "segundo", "Se
+000027b0: 6775 6e64 6f22 2c20 2253 4547 554e 444f  gundo", "SEGUNDO
+000027c0: 222c 2022 7365 6775 6e64 6f73 222c 2022  ", "segundos", "
+000027d0: 5365 6775 6e64 6f73 222c 2022 5345 4755  Segundos", "SEGU
+000027e0: 4e44 4f53 225d 0a20 2020 2020 2020 207d  NDOS"].        }
+000027f0: 2c0a 2020 2020 2020 2020 226d 696e 7574  ,.        "minut
+00002800: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
+00002810: 2020 2273 6361 6c65 223a 2036 302e 302c    "scale": 60.0,
+00002820: 0a20 2020 2020 2020 2020 2020 2022 7369  .            "si
+00002830: 6e67 756c 6172 223a 2022 6d69 6e75 746f  ngular": "minuto
+00002840: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002850: 706c 7572 616c 223a 2022 6d69 6e75 746f  plural": "minuto
+00002860: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00002870: 2274 6572 6d73 223a 205b 226d 222c 2022  "terms": ["m", "
+00002880: 6d69 6e22 2c20 224d 696e 222c 2022 4d49  min", "Min", "MI
+00002890: 4e22 2c20 226d 696e 7322 2c20 224d 696e  N", "mins", "Min
+000028a0: 7322 2c20 224d 494e 5322 2c20 226d 696e  s", "MINS", "min
+000028b0: 7574 6f22 2c20 224d 696e 7574 6f22 2c20  uto", "Minuto", 
+000028c0: 224d 494e 5554 4f22 2c20 226d 696e 7574  "MINUTO", "minut
+000028d0: 6f73 222c 2022 4d69 6e75 746f 7322 2c20  os", "Minutos", 
+000028e0: 224d 494e 5554 4f53 225d 0a20 2020 2020  "MINUTOS"].     
+000028f0: 2020 207d 2c0a 2020 2020 2020 2020 2268     },.        "h
+00002900: 6f75 7222 3a20 7b0a 2020 2020 2020 2020  our": {.        
+00002910: 2020 2020 2273 6361 6c65 223a 2033 3630      "scale": 360
+00002920: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+00002930: 2022 7369 6e67 756c 6172 223a 2022 686f   "singular": "ho
+00002940: 7261 222c 0a20 2020 2020 2020 2020 2020  ra",.           
+00002950: 2022 706c 7572 616c 223a 2022 686f 7261   "plural": "hora
+00002960: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00002970: 2274 6572 6d73 223a 205b 2268 222c 2022  "terms": ["h", "
+00002980: 4822 2c20 2268 7222 2c20 2248 7222 2c20  H", "hr", "Hr", 
+00002990: 2248 5222 2c20 2268 7273 222c 2022 4872  "HR", "hrs", "Hr
+000029a0: 7322 2c20 2248 5253 222c 2022 686f 7261  s", "HRS", "hora
+000029b0: 222c 2022 486f 7261 222c 2022 484f 5241  ", "Hora", "HORA
+000029c0: 222c 2022 686f 7261 7322 2c20 2248 6f72  ", "horas", "Hor
+000029d0: 6173 222c 2022 484f 5241 5322 5d0a 2020  as", "HORAS"].  
+000029e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000029f0: 2022 6461 7922 3a20 7b0a 2020 2020 2020   "day": {.      
+00002a00: 2020 2020 2020 2273 6361 6c65 223a 2038        "scale": 8
+00002a10: 3634 3030 2e30 2c0a 2020 2020 2020 2020  6400.0,.        
+00002a20: 2020 2020 2273 696e 6775 6c61 7222 3a20      "singular": 
+00002a30: 2264 6961 222c 0a20 2020 2020 2020 2020  "dia",.         
+00002a40: 2020 2022 706c 7572 616c 223a 2022 6469     "plural": "di
+00002a50: 6173 222c 0a20 2020 2020 2020 2020 2020  as",.           
+00002a60: 2022 7465 726d 7322 3a20 5b22 6422 2c20   "terms": ["d", 
+00002a70: 2264 6961 222c 2022 4469 6122 2c20 2244  "dia", "Dia", "D
+00002a80: 4941 222c 2022 6469 6173 222c 2022 4469  IA", "dias", "Di
+00002a90: 6173 222c 2022 4449 4153 225d 0a20 2020  as", "DIAS"].   
+00002aa0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00002ab0: 2277 6565 6b22 3a20 7b0a 2020 2020 2020  "week": {.      
+00002ac0: 2020 2020 2020 2273 6361 6c65 223a 2036        "scale": 6
+00002ad0: 3034 3830 302e 302c 0a20 2020 2020 2020  04800.0,.       
+00002ae0: 2020 2020 2022 7369 6e67 756c 6172 223a       "singular":
+00002af0: 2022 7365 6d61 6e61 222c 0a20 2020 2020   "semana",.     
+00002b00: 2020 2020 2020 2022 706c 7572 616c 223a         "plural":
+00002b10: 2022 7365 6d61 6e61 7322 2c0a 2020 2020   "semanas",.    
+00002b20: 2020 2020 2020 2020 2274 6572 6d73 223a          "terms":
+00002b30: 205b 2273 656d 222c 2022 5365 6d22 2c20   ["sem", "Sem", 
+00002b40: 2253 454d 222c 2022 7365 6d61 6e61 222c  "SEM", "semana",
+00002b50: 2022 5365 6d61 6e61 222c 2022 5345 4d41   "Semana", "SEMA
+00002b60: 4e41 222c 2022 7365 6d61 6e61 7322 2c20  NA", "semanas", 
+00002b70: 2253 656d 616e 6173 222c 2022 5345 4d41  "Semanas", "SEMA
+00002b80: 4e41 5322 5d0a 2020 2020 2020 2020 7d2c  NAS"].        },
+00002b90: 0a20 2020 2020 2020 2022 6d6f 6e74 6822  .        "month"
+00002ba0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002bb0: 2273 6361 6c65 223a 2032 3633 3532 3030  "scale": 2635200
+00002bc0: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00002bd0: 2273 696e 6775 6c61 7222 3a20 226d 6573  "singular": "mes
+00002be0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002bf0: 706c 7572 616c 223a 2022 6d65 7365 7322  plural": "meses"
+00002c00: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00002c10: 6572 6d73 223a 205b 224d 222c 2022 6d65  erms": ["M", "me
+00002c20: 7322 2c20 224d 6573 222c 2022 4d45 5322  s", "Mes", "MES"
+00002c30: 2c20 226d 6573 6573 222c 2022 4d65 7365  , "meses", "Mese
+00002c40: 7322 2c20 224d 4553 4553 222c 2022 6d6f  s", "MESES", "mo
+00002c50: 222c 2022 4d6f 222c 2022 4d4f 222c 2022  ", "Mo", "MO", "
+00002c60: 6d6f 7322 2c20 224d 6f73 222c 2022 4d4f  mos", "Mos", "MO
+00002c70: 5322 5d0a 2020 2020 2020 2020 7d2c 0a20  S"].        },. 
+00002c80: 2020 2020 2020 2022 7965 6172 223a 207b         "year": {
+00002c90: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
+00002ca0: 616c 6522 3a20 3331 3533 3630 3030 2e30  ale": 31536000.0
+00002cb0: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+00002cc0: 696e 6775 6c61 7222 3a20 2261 6e6f 222c  ingular": "ano",
+00002cd0: 0a20 2020 2020 2020 2020 2020 2022 706c  .            "pl
+00002ce0: 7572 616c 223a 2022 616e 6f73 222c 0a20  ural": "anos",. 
+00002cf0: 2020 2020 2020 2020 2020 2022 7465 726d             "term
+00002d00: 7322 3a20 5b22 6122 2c20 2241 222c 2022  s": ["a", "A", "
+00002d10: 616e 6f22 2c20 2241 6e6f 222c 2022 414e  ano", "Ano", "AN
+00002d20: 4f22 2c20 2261 6e6f 7322 2c20 2241 6e6f  O", "anos", "Ano
+00002d30: 7322 2c20 2241 4e4f 5322 5d0a 2020 2020  s", "ANOS"].    
+00002d40: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00002d50: 6465 6361 6465 223a 207b 0a20 2020 2020  decade": {.     
+00002d60: 2020 2020 2020 2022 7363 616c 6522 3a20         "scale": 
+00002d70: 3331 3533 3630 3030 302e 302c 0a20 2020  315360000.0,.   
+00002d80: 2020 2020 2020 2020 2022 7369 6e67 756c           "singul
+00002d90: 6172 223a 2022 6465 6361 6461 222c 0a20  ar": "decada",. 
+00002da0: 2020 2020 2020 2020 2020 2022 706c 7572             "plur
+00002db0: 616c 223a 2022 6465 6361 6461 7322 2c0a  al": "decadas",.
+00002dc0: 2020 2020 2020 2020 2020 2020 2274 6572              "ter
+00002dd0: 6d73 223a 205b 2244 222c 2022 6465 6322  ms": ["D", "dec"
+00002de0: 2c20 2244 6563 222c 2022 4445 4322 2c20  , "Dec", "DEC", 
+00002df0: 2264 6563 7322 2c20 2244 6563 7322 2c20  "decs", "Decs", 
+00002e00: 2244 4543 5322 2c20 2264 6563 6164 6122  "DECS", "decada"
+00002e10: 2c20 2244 6563 6164 6122 2c20 2244 4543  , "Decada", "DEC
+00002e20: 4144 4122 2c20 2264 6563 6164 6173 222c  ADA", "decadas",
+00002e30: 2022 4465 6361 6461 7322 2c20 2244 4543   "Decadas", "DEC
+00002e40: 4144 4153 225d 0a20 2020 2020 2020 207d  ADAS"].        }
+00002e50: 2c0a 2020 2020 2020 2020 2263 656e 7475  ,.        "centu
+00002e60: 7279 223a 207b 0a20 2020 2020 2020 2020  ry": {.         
+00002e70: 2020 2022 7363 616c 6522 3a20 3331 3533     "scale": 3153
+00002e80: 3630 3030 3030 2e30 2c0a 2020 2020 2020  600000.0,.      
+00002e90: 2020 2020 2020 2273 696e 6775 6c61 7222        "singular"
+00002ea0: 3a20 2273 6967 6c6f 222c 0a20 2020 2020  : "siglo",.     
+00002eb0: 2020 2020 2020 2022 706c 7572 616c 223a         "plural":
+00002ec0: 2022 7369 676c 6f73 222c 0a20 2020 2020   "siglos",.     
+00002ed0: 2020 2020 2020 2022 7465 726d 7322 3a20         "terms": 
+00002ee0: 5b22 6322 2c20 2243 222c 2022 7369 676c  ["c", "C", "sigl
+00002ef0: 6f22 2c20 2253 6967 6c6f 222c 2022 5349  o", "Siglo", "SI
+00002f00: 474c 4f22 2c20 2273 6967 6c6f 7322 2c20  GLO", "siglos", 
+00002f10: 2253 6967 6c6f 7322 2c20 2253 4947 4c4f  "Siglos", "SIGLO
+00002f20: 5322 5d0a 2020 2020 2020 2020 7d0a 2020  S"].        }.  
+00002f30: 2020 7d2c 0a20 2020 2022 6578 7472 615f    },.    "extra_
+00002f40: 6461 7461 223a 207b 0a20 2020 207d 0a7d  data": {.    }.}
+00002f50: 0a                                       .
```

### Comparing `timelength-2.0.1/timelength/locales.py` & `timelength-2.0.2/timelength/locales.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-import json
-import os
-from importlib import util
-from typing import Union
-
-from timelength.dataclasses import Scale
-from timelength.errors import LocaleConfigError
-
-
-class Locale:
-    """
-    Represents a default Locale, each of which may handle parsing differently.
-
-    ### Attributes
-
-    - `json_location` (`str`): The string path to the config file for this Locale.
-    """
-
-    def __init__(self, json_location: str = "english.json"):
-        """Initialize the `Locale` based on the passed config file."""
-        self._json_location = json_location
-        self._config = {}
-        base_dir = os.path.dirname(__file__)
-
-        locale_path = os.path.join(base_dir, "locales", json_location)
-        if os.path.exists(locale_path):
-            full_json_path = locale_path
-        else:
-            full_json_path = json_location
-        self._load_config(full_json_path)
-
-        if not self._config:
-            raise LocaleConfigError("Provided config is empty.")
-
-        self._parser_file = self._get_config_or_raise("parser_file")
-        self._parser = None
-        self._load_parser(base_dir)
-
-        self._connectors = self._get_config_or_raise("connectors")
-        self._segmentors = self._get_config_or_raise("segmentors")
-        if set(self._connectors).intersection(self._segmentors):
-            raise LocaleConfigError(
-                "Connectors and Segmentors may not have overlap in config."
-            )
-
-        # _allowed_terms may appear ONCE in a row in the input while strict is enabled.
-        self._allowed_terms = self._get_config_or_raise("allowed_terms")
-        self._decimal_separators = self._get_config_or_raise("decimal_separators")
-        self._thousand_separators = self._get_config_or_raise("thousand_separators")
-        if set(self._decimal_separators).intersection(self._thousand_separators):
-            raise LocaleConfigError(
-                "Decimal separators and Thousand separators may not have overlap in config."
-            )
-
-        # Default Scales can be disabled by removing them from the config. In their place an empty Scale of
-        # scale 0 will be added. This will cause its related TimeLength conversion method, such as `to_minutes`,
-        # to error as dividing by 0 is not allowed. Parsing wise, it will be ignored as the terms list is empty.
-        scales_json = self._get_config_or_raise("scales")
-        self._millisecond = (
-            Scale(**self._config["scales"]["millisecond"])
-            if "millisecond" in scales_json
-            else Scale()
-        )
-        self._second = (
-            Scale(**self._config["scales"]["second"])
-            if "second" in scales_json
-            else Scale()
-        )
-        self._minute = (
-            Scale(**self._config["scales"]["minute"])
-            if "minute" in scales_json
-            else Scale()
-        )
-        self._hour = (
-            Scale(**self._config["scales"]["hour"])
-            if "hour" in scales_json
-            else Scale()
-        )
-        self._day = (
-            Scale(**self._config["scales"]["day"]) if "day" in scales_json else Scale()
-        )
-        self._week = (
-            Scale(**self._config["scales"]["week"])
-            if "week" in scales_json
-            else Scale()
-        )
-        self._month = (
-            Scale(**self._config["scales"]["month"])
-            if "month" in scales_json
-            else Scale()
-        )
-        self._year = (
-            Scale(**self._config["scales"]["year"])
-            if "year" in scales_json
-            else Scale()
-        )
-        self._decade = (
-            Scale(**self._config["scales"]["decade"])
-            if "decade" in scales_json
-            else Scale()
-        )
-        self._century = (
-            Scale(**self._config["scales"]["century"])
-            if "century" in scales_json
-            else Scale()
-        )
-        self._scales: list = [
-            self._millisecond,
-            self._second,
-            self._minute,
-            self._hour,
-            self._day,
-            self._week,
-            self._month,
-            self._year,
-            self._decade,
-            self._century,
-        ]
-
-        # Allow for custom defined Scales.
-        for scale_name in scales_json:
-            if scale_name not in {
-                "millisecond",
-                "second",
-                "minute",
-                "hour",
-                "day",
-                "week",
-                "month",
-                "year",
-                "decade",
-                "century",
-            }:
-                custom_scale = Scale(**self._config["scales"][scale_name])
-                setattr(self, f"_{scale_name}", custom_scale)
-                self._scales.append(custom_scale)
-
-        self._numerals = self._get_config_or_raise("numerals")
-        self._extra_data = self._get_config_or_raise("extra_data")
-
-    def _get_scale(self, text: str) -> Scale:
-        """Get the scale that contains a specific value in its terms list."""
-        for scale in self._scales:
-            scale: Scale
-            if text in scale.terms:
-                return scale
-        return None
-
-    def _get_numeral(self, text: str) -> dict:
-        """Get a numeral that contains a specific value in its terms list."""
-        numeral = {}
-        for numeral in self._numerals:
-            if text in self._numerals[numeral]["terms"]:
-                return self._numerals[numeral]
-        return None
-
-    def _load_parser(self, base_dir):
-        """Load the parser file linked in the config file into a method attached to the `Locale`."""
-        if self._parser and callable(self._parser):
-            return  # Parser already loaded for this locale.
-        parser_path = os.path.join(base_dir, "parsers", self._parser_file)
-        if os.path.exists(parser_path):
-            full_parser_path = parser_path
-        else:
-            full_parser_path = self._parser_file
-        module_name, _ = os.path.splitext(os.path.basename(full_parser_path))
-        try:
-            spec = util.spec_from_file_location(module_name, full_parser_path)
-            if not spec:
-                raise FileNotFoundError
-            module = util.module_from_spec(spec)
-            spec.loader.exec_module(module)
-            self._parser = getattr(module, module_name, None)
-            if not callable(self._parser):
-                raise AttributeError
-        except (ModuleNotFoundError, FileNotFoundError):
-            self._parser = None
-            raise LocaleConfigError(f"File not found: {self._parser_file}") from None
-        except AttributeError:
-            self._parser = None
-            raise LocaleConfigError(
-                f"Parser function not found: {module_name}"
-            ) from None
-
-    def _load_config(self, file: str):
-        """Load the config from the provided path."""
-        with open(file, "r", encoding="utf-8") as f:
-            self._config = json.load(f)
-
-    def _get_config_or_raise(self, key: str) -> Union[str, float, list, dict]:
-        """Retrieve a value from the config or raise if the value is not found."""
-        value = self._config.get(key)
-        if value is None:
-            raise LocaleConfigError(
-                f'Provided config is malformed. No "{key}" key provided.'
-            )
-        return value
-
-    def __str__(self):
-        """Return the name of the `Locale`."""
-        return f"<{self.__class__.__name__}>"
-
-    def __repr__(self):
-        """Return a string representation of the `Locale` with the config path included."""
-        return f'Locale("{self._json_location}")'
-
-
-class CustomLocale(Locale):
-    """
-    Represents a custom `Locale`.
-
-    ### Attributes
-
-    - `json_location` (`str`): The string path to the config file for this `Locale`.
-    """
-
-    def __init__(self, path_to_json: str):
-        super().__init__(path_to_json)
-
-
-class English(Locale):
-    """
-    Represents the `English` `Locale`.
-    """
-
-    def __init__(self):
-        super().__init__("english.json")
-
-
-class Spanish(Locale):
-    """
-    Represents the `Spanish` `Locale`.
-    """
-
-    def __init__(self):
-        super().__init__("spanish.json")
+import json
+import os
+from importlib import util
+from typing import Union
+
+from timelength.dataclasses import Scale
+from timelength.errors import LocaleConfigError
+
+
+class Locale:
+    """
+    Represents a default Locale, each of which may handle parsing differently.
+
+    ### Attributes
+
+    - `json_location` (`str`): The string path to the config file for this Locale.
+    """
+
+    def __init__(self, json_location: str = "english.json"):
+        """Initialize the `Locale` based on the passed config file."""
+        self._json_location = json_location
+        self._config = {}
+        base_dir = os.path.dirname(__file__)
+
+        locale_path = os.path.join(base_dir, "locales", json_location)
+        if os.path.exists(locale_path):
+            full_json_path = locale_path
+        else:
+            full_json_path = json_location
+        self._load_config(full_json_path)
+
+        if not self._config:
+            raise LocaleConfigError("Provided config is empty.")
+
+        self._parser_file = self._get_config_or_raise("parser_file")
+        self._parser = None
+        self._load_parser(base_dir)
+
+        self._connectors = self._get_config_or_raise("connectors")
+        self._segmentors = self._get_config_or_raise("segmentors")
+        if set(self._connectors).intersection(self._segmentors):
+            raise LocaleConfigError(
+                "Connectors and Segmentors may not have overlap in config."
+            )
+
+        # _allowed_terms may appear ONCE in a row in the input while strict is enabled.
+        self._allowed_terms = self._get_config_or_raise("allowed_terms")
+        self._decimal_separators = self._get_config_or_raise("decimal_separators")
+        self._thousand_separators = self._get_config_or_raise("thousand_separators")
+        if set(self._decimal_separators).intersection(self._thousand_separators):
+            raise LocaleConfigError(
+                "Decimal separators and Thousand separators may not have overlap in config."
+            )
+
+        # Default Scales can be disabled by removing them from the config. In their place an empty Scale of
+        # scale 0 will be added. This will cause its related TimeLength conversion method, such as `to_minutes`,
+        # to error as dividing by 0 is not allowed. Parsing wise, it will be ignored as the terms list is empty.
+        scales_json = self._get_config_or_raise("scales")
+        self._millisecond = (
+            Scale(**self._config["scales"]["millisecond"])
+            if "millisecond" in scales_json
+            else Scale()
+        )
+        self._second = (
+            Scale(**self._config["scales"]["second"])
+            if "second" in scales_json
+            else Scale()
+        )
+        self._minute = (
+            Scale(**self._config["scales"]["minute"])
+            if "minute" in scales_json
+            else Scale()
+        )
+        self._hour = (
+            Scale(**self._config["scales"]["hour"])
+            if "hour" in scales_json
+            else Scale()
+        )
+        self._day = (
+            Scale(**self._config["scales"]["day"]) if "day" in scales_json else Scale()
+        )
+        self._week = (
+            Scale(**self._config["scales"]["week"])
+            if "week" in scales_json
+            else Scale()
+        )
+        self._month = (
+            Scale(**self._config["scales"]["month"])
+            if "month" in scales_json
+            else Scale()
+        )
+        self._year = (
+            Scale(**self._config["scales"]["year"])
+            if "year" in scales_json
+            else Scale()
+        )
+        self._decade = (
+            Scale(**self._config["scales"]["decade"])
+            if "decade" in scales_json
+            else Scale()
+        )
+        self._century = (
+            Scale(**self._config["scales"]["century"])
+            if "century" in scales_json
+            else Scale()
+        )
+        self._scales: list = [
+            self._millisecond,
+            self._second,
+            self._minute,
+            self._hour,
+            self._day,
+            self._week,
+            self._month,
+            self._year,
+            self._decade,
+            self._century,
+        ]
+
+        # Allow for custom defined Scales.
+        for scale_name in scales_json:
+            if scale_name not in {
+                "millisecond",
+                "second",
+                "minute",
+                "hour",
+                "day",
+                "week",
+                "month",
+                "year",
+                "decade",
+                "century",
+            }:
+                custom_scale = Scale(**self._config["scales"][scale_name])
+                setattr(self, f"_{scale_name}", custom_scale)
+                self._scales.append(custom_scale)
+
+        self._numerals = self._get_config_or_raise("numerals")
+        self._extra_data = self._get_config_or_raise("extra_data")
+
+    def _get_scale(self, text: str) -> Scale:
+        """Get the scale that contains a specific value in its terms list."""
+        for scale in self._scales:
+            scale: Scale
+            if text in scale.terms:
+                return scale
+        return None
+
+    def _get_numeral(self, text: str) -> dict:
+        """Get a numeral that contains a specific value in its terms list."""
+        numeral = {}
+        for numeral in self._numerals:
+            if text in self._numerals[numeral]["terms"]:
+                return self._numerals[numeral]
+        return None
+
+    def _load_parser(self, base_dir):
+        """Load the parser file linked in the config file into a method attached to the `Locale`."""
+        if self._parser and callable(self._parser):
+            return  # Parser already loaded for this locale.
+        parser_path = os.path.join(base_dir, "parsers", self._parser_file)
+        if os.path.exists(parser_path):
+            full_parser_path = parser_path
+        else:
+            full_parser_path = self._parser_file
+        module_name, _ = os.path.splitext(os.path.basename(full_parser_path))
+        try:
+            spec = util.spec_from_file_location(module_name, full_parser_path)
+            if not spec:
+                raise FileNotFoundError
+            module = util.module_from_spec(spec)
+            spec.loader.exec_module(module)
+            self._parser = getattr(module, module_name, None)
+            if not callable(self._parser):
+                raise AttributeError
+        except (ModuleNotFoundError, FileNotFoundError):
+            self._parser = None
+            raise LocaleConfigError(f"File not found: {self._parser_file}") from None
+        except AttributeError:
+            self._parser = None
+            raise LocaleConfigError(
+                f"Parser function not found: {module_name}"
+            ) from None
+
+    def _load_config(self, file: str):
+        """Load the config from the provided path."""
+        with open(file, "r", encoding="utf-8") as f:
+            self._config = json.load(f)
+
+    def _get_config_or_raise(self, key: str) -> Union[str, float, list, dict]:
+        """Retrieve a value from the config or raise if the value is not found."""
+        value = self._config.get(key)
+        if value is None:
+            raise LocaleConfigError(
+                f'Provided config is malformed. No "{key}" key provided.'
+            )
+        return value
+
+    def __str__(self):
+        """Return the name of the `Locale`."""
+        return f"<{self.__class__.__name__}>"
+
+    def __repr__(self):
+        """Return a string representation of the `Locale` with the config path included."""
+        return f'Locale("{self._json_location}")'
+
+
+class CustomLocale(Locale):
+    """
+    Represents a custom `Locale`.
+
+    ### Attributes
+
+    - `json_location` (`str`): The string path to the config file for this `Locale`.
+    """
+
+    def __init__(self, path_to_json: str):
+        super().__init__(path_to_json)
+
+
+class English(Locale):
+    """
+    Represents the `English` `Locale`.
+    """
+
+    def __init__(self):
+        super().__init__("english.json")
+
+
+class Spanish(Locale):
+    """
+    Represents the `Spanish` `Locale`.
+    """
+
+    def __init__(self):
+        super().__init__("spanish.json")
```

### Comparing `timelength-2.0.1/timelength/parsers/parser_one.py` & `timelength-2.0.2/timelength/parsers/parser_one.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,445 +1,445 @@
-from fractions import Fraction
-
-from timelength.dataclasses import ParsedTimeLength, Scale
-from timelength.enums import BufferType, CharacterType
-from timelength.locales import Locale
-from timelength.utils import buffer_type, character_type, remove_diacritics
-
-
-def parser_one(
-    content: str,
-    strict: bool,
-    locale: Locale,
-    result: ParsedTimeLength,
-):
-    content = remove_diacritics(content)
-    buffer = ""
-    buffer_values = []
-    result.valid = []
-    skip_iteration = 0
-    result.seconds = 0.0
-    last_alphanum = None
-    current_alphanum = None
-
-    def save_buffer():
-        nonlocal buffer
-        if buffer:
-            numerals = locale._numerals
-            scales = locale._scales
-            buffer_alphanum = buffer_type(
-                buffer,
-                [term for scale in scales for term in scale.terms],
-                [
-                    term
-                    for numeral in numerals
-                    if "terms" in numerals[numeral]
-                    for term in numerals[numeral]["terms"]
-                ],
-                locale._connectors + locale._segmentors + locale._allowed_terms,
-            )
-            buffer_values.append(
-                (
-                    float(buffer) if buffer_alphanum == BufferType.NUMBER else buffer,
-                    buffer_alphanum,
-                )
-            )
-            buffer = ""
-
-    def check_next(
-        next_index: int,
-        target_chartype: CharacterType,
-        decimal_only: bool = False,
-    ):
-        nonlocal content, buffer, skip_iteration
-        skip_thousand = 0
-        already_used_decimal = False
-
-        if target_chartype == CharacterType.NUMBER:
-            while next_index < len(content) and (
-                character_type(content[next_index]) == target_chartype
-                or content[next_index]
-                in locale._decimal_separators + locale._thousand_separators
-            ):
-                if skip_thousand:
-                    skip_thousand -= 1
-                    continue
-
-                if character_type(content[next_index]) == CharacterType.NUMBER:
-                    buffer += content[next_index]
-                elif content[next_index] in locale._decimal_separators:
-                    if already_used_decimal:
-                        result.invalid.append(
-                            (
-                                f"{content[next_index - 3]}{content[next_index - 2]}{content[next_index - 1]}{content[next_index]}",
-                                "MALFORMED_DECIMAL",
-                            )
-                        )
-                        next_index += 1
-                        skip_iteration += 1
-                        buffer = ""
-                        break
-                    buffer += "."
-                    decimal_only = True
-                    already_used_decimal = True
-                elif (
-                    not decimal_only
-                    and content[next_index] in locale._thousand_separators
-                ):
-                    if not (
-                        (next_index + 3) < len(content)
-                        and all(
-                            character_type(content[next_index + i])
-                            == CharacterType.NUMBER
-                            for i in range(1, 4)
-                        )
-                    ):
-                        break
-                    else:
-                        for num in range(1, 4):
-                            buffer += content[next_index + num]
-
-                        next_index += 4
-                        skip_iteration += 4
-                        skip_thousand = 4
-                        continue
-                next_index += 1
-                skip_iteration += 1
-        else:
-            while next_index < len(content) and (
-                character_type(content[next_index]) == target_chartype
-            ):
-                buffer += content[next_index]
-                next_index += 1
-                skip_iteration += 1
-
-    for index, char in enumerate(content):
-        if skip_iteration > 0:
-            skip_iteration -= 1
-            continue
-
-        current_alphanum = character_type(char)
-        if buffer and index and last_alphanum != current_alphanum:
-            save_buffer()
-
-        if current_alphanum == CharacterType.NUMBER:
-            if (index + 2) < len(content) and (
-                character_type(content[index + 2]) == CharacterType.NUMBER
-            ):
-                if content[index + 1] in locale._decimal_separators:
-                    buffer += char
-                    check_next(index + 1, CharacterType.NUMBER, True)
-                elif content[index + 1] in locale._thousand_separators:
-                    buffer += char
-                    check_next(index + 1, CharacterType.NUMBER)
-                else:
-                    buffer += char
-            else:
-                buffer += char
-        elif (
-            not buffer
-            and (index + 1) < len(content)
-            and char in locale._decimal_separators
-            and (character_type(content[index + 1]) == CharacterType.NUMBER)
-        ):
-            buffer += "0."
-            check_next(index + 1, CharacterType.NUMBER, True)
-        elif current_alphanum == CharacterType.ALPHABET:
-            buffer += char
-            check_next(index + 1, CharacterType.ALPHABET)
-        elif (
-            current_alphanum == CharacterType.SPECIAL
-            and char
-            not in locale._connectors
-            + locale._segmentors
-            + locale._allowed_terms
-            + locale._decimal_separators
-            + locale._thousand_separators
-        ):
-            buffer += char
-            check_next(index + 1, CharacterType.SPECIAL)
-        else:
-            buffer += char
-            save_buffer()
-
-        last_alphanum = current_alphanum
-
-    if buffer:
-        save_buffer()
-
-    potential_values = []
-    skip_buffer = 0
-    for index, item in enumerate(buffer_values):
-        if skip_buffer:
-            skip_buffer -= 1
-            continue
-        if not item:
-            continue
-        if item[1] == BufferType.UNKNOWN:
-            result.invalid.append((item[0], "UNKNOWN_TERM"))
-            if (
-                index + 1 < len(buffer_values)
-                and buffer_values[index + 1][0] in locale._connectors
-            ):
-                skip_buffer += 1
-        else:
-            potential_values.append(item)
-
-    parsed_value = None
-    segment_value = None
-    parsed_scale = None
-    previous_specials = []
-    previous_segmentors = []
-    current_value_type = None
-    current_value_type_converted = None
-    previous_value_type = None
-    previous_value_type_converted = None
-    current_numeral_type = None
-    previous_numeral_type = None
-    larger_numeral = False
-    starts_with_modifier = False
-
-    def handle_multiplier(text: str, index: int):
-        nonlocal parsed_value, segment_value
-        previous_numeric = False
-        next_numeric = False
-        next_term = False
-        previous_value = 0.0
-        next_value = 0.0
-        if (index - 2) >= 0:
-            previous_type = potential_values[index - 2][1]
-            if previous_type == BufferType.NUMERAL:
-                previous_numeric = True
-                previous_value = locale._get_numeral(potential_values[index - 2][0])[
-                    "value"
-                ]
-                if isinstance(previous_value, str):
-                    previous_value = float(Fraction(previous_value))
-            elif previous_type == BufferType.NUMBER:
-                previous_numeric = True
-                previous_value = potential_values[index - 2][0]
-        if (index + 2) < len(potential_values):
-            next_type = potential_values[index + 2][1]
-            if next_type == BufferType.NUMERAL:
-                next_numeric = True
-                next_value = locale._get_numeral(potential_values[index + 2][0])[
-                    "value"
-                ]
-                if isinstance(next_value, str):
-                    next_value = float(Fraction(next_value))
-            elif next_type == BufferType.NUMBER:
-                next_numeric = True
-                next_value = potential_values[index + 2][0]
-            elif next_type == BufferType.SCALE:
-                next_term = True
-        if previous_numeric and next_numeric:
-            potential_values[index + 2] = (
-                previous_value * next_value,
-                BufferType.NUMBER,
-            )
-        else:
-            if (not previous_numeric and not next_numeric) or not next_term:
-                result.invalid.append((text, "UNUSED_MULTIPLIER"))
-
-    def handle_special(symbol: str):
-        if symbol in previous_specials:
-            result.invalid.append((symbol, "CONSECUTIVE_SPECIALS"))
-        previous_specials.append(symbol)
-
-    def handle_float(number: float):
-        nonlocal parsed_value, segment_value
-
-        if (
-            previous_value_type_converted == BufferType.NUMBER
-            and not starts_with_modifier
-        ):
-            if segment_value:
-                result.invalid.append((segment_value, "LONELY_VALUE"))
-                segment_value = None
-            result.invalid.append((parsed_value, "CONSECUTIVE_VALUES"))
-        parsed_value = number
-
-    def handle_numeral(text: str, index: int):
-        nonlocal \
-            parsed_value, \
-            current_numeral_type, \
-            current_value_type_converted, \
-            starts_with_modifier, \
-            segment_value, \
-            larger_numeral
-
-        numeral = locale._get_numeral(text)
-        numeral_value = (
-            float(Fraction(numeral["value"]))
-            if isinstance(numeral["value"], str)
-            else float(numeral["value"])
-        )
-        current_numeral_type = numeral["type"]
-        current_value_type_converted = BufferType.NUMBER
-
-        if parsed_value is None:
-            parsed_value = 0.0
-            if (
-                current_numeral_type == "modifiers"
-                and index + 2 < len(potential_values)
-                and potential_values[index + 2][1]
-                in [BufferType.NUMBER, BufferType.NUMERAL]
-            ):
-                if potential_values[index + 2][1] == BufferType.NUMERAL:
-                    numeral = locale._get_numeral(potential_values[index + 2][0])
-                    if numeral["type"] == "multiplier":
-                        parsed_value = numeral_value
-                    else:
-                        potential_values[index + 2] = (
-                            numeral["value"] * numeral_value,
-                            BufferType.NUMBER,
-                        )
-                else:
-                    potential_values[index + 2] = (
-                        potential_values[index + 2][0] * numeral_value,
-                        BufferType.NUMBER,
-                    )
-                starts_with_modifier = True
-            else:
-                parsed_value = numeral_value
-        elif current_numeral_type in ["modifiers", "thousands"]:
-            parsed_value *= numeral_value
-        elif current_numeral_type == "digits" and previous_numeral_type == "tens":
-            larger_numeral = True
-            parsed_value = parsed_value + numeral_value
-        elif (
-            current_numeral_type == "digits"
-            and previous_numeral_type == "digits"
-            and not larger_numeral
-        ):
-            parsed_value = float(f"{int(parsed_value)}{int(numeral_value)}")
-        elif current_numeral_type in ["teens", "tens"] and previous_numeral_type in [
-            "digits",
-            "teens",
-            "tens",
-        ]:
-            parsed_value = float(f"{int(parsed_value)}{int(numeral_value)}")
-        elif (
-            current_numeral_type in ["tens", "teens", "digits"]
-            and previous_numeral_type == "thousands"
-        ):
-            parsed_value = parsed_value + numeral_value
-            larger_numeral = True
-        elif (
-            previous_value_type_converted == BufferType.NUMBER
-            or previous_numeral_type == "modifiers"
-        ) and current_numeral_type not in ["thousands", "modifiers"]:
-            if segment_value:
-                result.invalid.append((segment_value, "LONELY_VALUE"))
-                segment_value = None
-            result.invalid.append((parsed_value, "CONSECUTIVE_VALUES"))
-            larger_numeral = False
-            parsed_value = numeral_value
-        else:
-            larger_numeral = False
-            parsed_value = numeral_value
-
-    def handle_scale(text: str):
-        nonlocal parsed_value, segment_value, result, parsed_scale, current_numeral_type
-
-        if index == 0:
-            result.invalid.append((text, "LEADING_SCALE"))
-        elif previous_value_type == BufferType.SCALE:
-            result.invalid.append((text, "CONSECUTIVE_SCALES"))
-        elif parsed_value is None and segment_value is None:
-            result.invalid.append((text, "LONELY_SCALE"))
-
-        if parsed_value is not None or segment_value is not None:
-            scale: Scale
-            scale = locale._get_scale(text)
-            if scale:
-                if not parsed_value:
-                    parsed_value = 0.0
-                if not segment_value:
-                    segment_value = 0.0
-                result.seconds += (parsed_value + segment_value) * scale.scale
-                parsed_scale = scale
-
-    for index, element in enumerate(potential_values):
-        current_value = element[0]
-        current_value_type = element[1]
-        current_value_type_converted = current_value_type
-
-        multiplier = False
-        if current_value_type == BufferType.NUMERAL:
-            multiplier = locale._get_numeral(current_value)
-            multiplier = True if multiplier["type"] == "multiplier" else False
-        if multiplier:
-            if parsed_value is not None:
-                handle_multiplier(current_value, index)
-            else:
-                result.invalid.append((current_value, "UNUSED_MULTIPLIER"))
-                segment_value = None
-                parsed_value = None
-                handle_special(current_value)
-        elif current_value_type == BufferType.SPECIAL:
-            handle_special(current_value)
-        elif current_value_type == BufferType.NUMBER:
-            handle_float(current_value)
-        elif current_value_type == BufferType.NUMERAL:
-            handle_numeral(current_value, index)
-        elif current_value_type == BufferType.SCALE:
-            handle_scale(current_value)
-
-        if (
-            current_value_type != BufferType.SPECIAL
-            or current_value in locale._segmentors
-        ):
-            previous_value_type = current_value_type
-            previous_numeral_type = current_numeral_type
-            previous_value_type_converted = current_value_type_converted
-            current_value_type_converted = None
-            current_numeral_type = None
-            current_value_type = None
-            previous_specials = []
-
-        if (parsed_value is not None or segment_value is not None) and parsed_scale:
-            if not parsed_value:
-                parsed_value = 0.0
-            if not segment_value:
-                segment_value = 0.0
-            result.valid.append((parsed_value + segment_value, parsed_scale))
-            parsed_value = None
-            segment_value = None
-            parsed_scale = None
-            starts_with_modifier = False
-
-        if current_value in locale._segmentors:
-            if current_value in previous_segmentors:
-                result.invalid.append((current_value, "CONSECUTIVE_SPECIALS"))
-            if parsed_value is not None:
-                if not segment_value:
-                    segment_value = 0.0
-                segment_value += parsed_value
-            parsed_value = None
-            starts_with_modifier = False
-            previous_segmentors.append(current_value)
-        else:
-            previous_segmentors = []
-
-    if (parsed_value is not None or segment_value is not None) and not parsed_scale:
-        if not parsed_value:
-            parsed_value = 0.0
-        if not segment_value:
-            segment_value = 0.0
-        selected_value = parsed_value + segment_value
-        if not strict and len(potential_values) == 1:
-            result.valid.append((parsed_value + segment_value, locale._second))
-            result.seconds += parsed_value + segment_value
-        else:
-            result.invalid.append(
-                (
-                    selected_value,
-                    "LONELY_VALUE",
-                )
-            )
-
-    if result.valid:
-        if strict and not result.invalid:
-            result.success = True
-        elif not strict:
-            result.success = True
+from fractions import Fraction
+
+from timelength.dataclasses import ParsedTimeLength, Scale
+from timelength.enums import BufferType, CharacterType
+from timelength.locales import Locale
+from timelength.utils import buffer_type, character_type, remove_diacritics
+
+
+def parser_one(
+    content: str,
+    strict: bool,
+    locale: Locale,
+    result: ParsedTimeLength,
+):
+    content = remove_diacritics(content)
+    buffer = ""
+    buffer_values = []
+    result.valid = []
+    skip_iteration = 0
+    result.seconds = 0.0
+    last_alphanum = None
+    current_alphanum = None
+
+    def save_buffer():
+        nonlocal buffer
+        if buffer:
+            numerals = locale._numerals
+            scales = locale._scales
+            buffer_alphanum = buffer_type(
+                buffer,
+                [term for scale in scales for term in scale.terms],
+                [
+                    term
+                    for numeral in numerals
+                    if "terms" in numerals[numeral]
+                    for term in numerals[numeral]["terms"]
+                ],
+                locale._connectors + locale._segmentors + locale._allowed_terms,
+            )
+            buffer_values.append(
+                (
+                    float(buffer) if buffer_alphanum == BufferType.NUMBER else buffer,
+                    buffer_alphanum,
+                )
+            )
+            buffer = ""
+
+    def check_next(
+        next_index: int,
+        target_chartype: CharacterType,
+        decimal_only: bool = False,
+    ):
+        nonlocal content, buffer, skip_iteration
+        skip_thousand = 0
+        already_used_decimal = False
+
+        if target_chartype == CharacterType.NUMBER:
+            while next_index < len(content) and (
+                character_type(content[next_index]) == target_chartype
+                or content[next_index]
+                in locale._decimal_separators + locale._thousand_separators
+            ):
+                if skip_thousand:
+                    skip_thousand -= 1
+                    continue
+
+                if character_type(content[next_index]) == CharacterType.NUMBER:
+                    buffer += content[next_index]
+                elif content[next_index] in locale._decimal_separators:
+                    if already_used_decimal:
+                        result.invalid.append(
+                            (
+                                f"{content[next_index - 3]}{content[next_index - 2]}{content[next_index - 1]}{content[next_index]}",
+                                "MALFORMED_DECIMAL",
+                            )
+                        )
+                        next_index += 1
+                        skip_iteration += 1
+                        buffer = ""
+                        break
+                    buffer += "."
+                    decimal_only = True
+                    already_used_decimal = True
+                elif (
+                    not decimal_only
+                    and content[next_index] in locale._thousand_separators
+                ):
+                    if not (
+                        (next_index + 3) < len(content)
+                        and all(
+                            character_type(content[next_index + i])
+                            == CharacterType.NUMBER
+                            for i in range(1, 4)
+                        )
+                    ):
+                        break
+                    else:
+                        for num in range(1, 4):
+                            buffer += content[next_index + num]
+
+                        next_index += 4
+                        skip_iteration += 4
+                        skip_thousand = 4
+                        continue
+                next_index += 1
+                skip_iteration += 1
+        else:
+            while next_index < len(content) and (
+                character_type(content[next_index]) == target_chartype
+            ):
+                buffer += content[next_index]
+                next_index += 1
+                skip_iteration += 1
+
+    for index, char in enumerate(content):
+        if skip_iteration > 0:
+            skip_iteration -= 1
+            continue
+
+        current_alphanum = character_type(char)
+        if buffer and index and last_alphanum != current_alphanum:
+            save_buffer()
+
+        if current_alphanum == CharacterType.NUMBER:
+            if (index + 2) < len(content) and (
+                character_type(content[index + 2]) == CharacterType.NUMBER
+            ):
+                if content[index + 1] in locale._decimal_separators:
+                    buffer += char
+                    check_next(index + 1, CharacterType.NUMBER, True)
+                elif content[index + 1] in locale._thousand_separators:
+                    buffer += char
+                    check_next(index + 1, CharacterType.NUMBER)
+                else:
+                    buffer += char
+            else:
+                buffer += char
+        elif (
+            not buffer
+            and (index + 1) < len(content)
+            and char in locale._decimal_separators
+            and (character_type(content[index + 1]) == CharacterType.NUMBER)
+        ):
+            buffer += "0."
+            check_next(index + 1, CharacterType.NUMBER, True)
+        elif current_alphanum == CharacterType.ALPHABET:
+            buffer += char
+            check_next(index + 1, CharacterType.ALPHABET)
+        elif (
+            current_alphanum == CharacterType.SPECIAL
+            and char
+            not in locale._connectors
+            + locale._segmentors
+            + locale._allowed_terms
+            + locale._decimal_separators
+            + locale._thousand_separators
+        ):
+            buffer += char
+            check_next(index + 1, CharacterType.SPECIAL)
+        else:
+            buffer += char
+            save_buffer()
+
+        last_alphanum = current_alphanum
+
+    if buffer:
+        save_buffer()
+
+    potential_values = []
+    skip_buffer = 0
+    for index, item in enumerate(buffer_values):
+        if skip_buffer:
+            skip_buffer -= 1
+            continue
+        if not item:
+            continue
+        if item[1] == BufferType.UNKNOWN:
+            result.invalid.append((item[0], "UNKNOWN_TERM"))
+            if (
+                index + 1 < len(buffer_values)
+                and buffer_values[index + 1][0] in locale._connectors
+            ):
+                skip_buffer += 1
+        else:
+            potential_values.append(item)
+
+    parsed_value = None
+    segment_value = None
+    parsed_scale = None
+    previous_specials = []
+    previous_segmentors = []
+    current_value_type = None
+    current_value_type_converted = None
+    previous_value_type = None
+    previous_value_type_converted = None
+    current_numeral_type = None
+    previous_numeral_type = None
+    larger_numeral = False
+    starts_with_modifier = False
+
+    def handle_multiplier(text: str, index: int):
+        nonlocal parsed_value, segment_value
+        previous_numeric = False
+        next_numeric = False
+        next_term = False
+        previous_value = 0.0
+        next_value = 0.0
+        if (index - 2) >= 0:
+            previous_type = potential_values[index - 2][1]
+            if previous_type == BufferType.NUMERAL:
+                previous_numeric = True
+                previous_value = locale._get_numeral(potential_values[index - 2][0])[
+                    "value"
+                ]
+                if isinstance(previous_value, str):
+                    previous_value = float(Fraction(previous_value))
+            elif previous_type == BufferType.NUMBER:
+                previous_numeric = True
+                previous_value = potential_values[index - 2][0]
+        if (index + 2) < len(potential_values):
+            next_type = potential_values[index + 2][1]
+            if next_type == BufferType.NUMERAL:
+                next_numeric = True
+                next_value = locale._get_numeral(potential_values[index + 2][0])[
+                    "value"
+                ]
+                if isinstance(next_value, str):
+                    next_value = float(Fraction(next_value))
+            elif next_type == BufferType.NUMBER:
+                next_numeric = True
+                next_value = potential_values[index + 2][0]
+            elif next_type == BufferType.SCALE:
+                next_term = True
+        if previous_numeric and next_numeric:
+            potential_values[index + 2] = (
+                previous_value * next_value,
+                BufferType.NUMBER,
+            )
+        else:
+            if (not previous_numeric and not next_numeric) or not next_term:
+                result.invalid.append((text, "UNUSED_MULTIPLIER"))
+
+    def handle_special(symbol: str):
+        if symbol in previous_specials:
+            result.invalid.append((symbol, "CONSECUTIVE_SPECIALS"))
+        previous_specials.append(symbol)
+
+    def handle_float(number: float):
+        nonlocal parsed_value, segment_value
+
+        if (
+            previous_value_type_converted == BufferType.NUMBER
+            and not starts_with_modifier
+        ):
+            if segment_value:
+                result.invalid.append((segment_value, "LONELY_VALUE"))
+                segment_value = None
+            result.invalid.append((parsed_value, "CONSECUTIVE_VALUES"))
+        parsed_value = number
+
+    def handle_numeral(text: str, index: int):
+        nonlocal \
+            parsed_value, \
+            current_numeral_type, \
+            current_value_type_converted, \
+            starts_with_modifier, \
+            segment_value, \
+            larger_numeral
+
+        numeral = locale._get_numeral(text)
+        numeral_value = (
+            float(Fraction(numeral["value"]))
+            if isinstance(numeral["value"], str)
+            else float(numeral["value"])
+        )
+        current_numeral_type = numeral["type"]
+        current_value_type_converted = BufferType.NUMBER
+
+        if parsed_value is None:
+            parsed_value = 0.0
+            if (
+                current_numeral_type == "modifiers"
+                and index + 2 < len(potential_values)
+                and potential_values[index + 2][1]
+                in [BufferType.NUMBER, BufferType.NUMERAL]
+            ):
+                if potential_values[index + 2][1] == BufferType.NUMERAL:
+                    numeral = locale._get_numeral(potential_values[index + 2][0])
+                    if numeral["type"] == "multiplier":
+                        parsed_value = numeral_value
+                    else:
+                        potential_values[index + 2] = (
+                            numeral["value"] * numeral_value,
+                            BufferType.NUMBER,
+                        )
+                else:
+                    potential_values[index + 2] = (
+                        potential_values[index + 2][0] * numeral_value,
+                        BufferType.NUMBER,
+                    )
+                starts_with_modifier = True
+            else:
+                parsed_value = numeral_value
+        elif current_numeral_type in ["modifiers", "thousands"]:
+            parsed_value *= numeral_value
+        elif current_numeral_type == "digits" and previous_numeral_type == "tens":
+            larger_numeral = True
+            parsed_value = parsed_value + numeral_value
+        elif (
+            current_numeral_type == "digits"
+            and previous_numeral_type == "digits"
+            and not larger_numeral
+        ):
+            parsed_value = float(f"{int(parsed_value)}{int(numeral_value)}")
+        elif current_numeral_type in ["teens", "tens"] and previous_numeral_type in [
+            "digits",
+            "teens",
+            "tens",
+        ]:
+            parsed_value = float(f"{int(parsed_value)}{int(numeral_value)}")
+        elif (
+            current_numeral_type in ["tens", "teens", "digits"]
+            and previous_numeral_type == "thousands"
+        ):
+            parsed_value = parsed_value + numeral_value
+            larger_numeral = True
+        elif (
+            previous_value_type_converted == BufferType.NUMBER
+            or previous_numeral_type == "modifiers"
+        ) and current_numeral_type not in ["thousands", "modifiers"]:
+            if segment_value:
+                result.invalid.append((segment_value, "LONELY_VALUE"))
+                segment_value = None
+            result.invalid.append((parsed_value, "CONSECUTIVE_VALUES"))
+            larger_numeral = False
+            parsed_value = numeral_value
+        else:
+            larger_numeral = False
+            parsed_value = numeral_value
+
+    def handle_scale(text: str):
+        nonlocal parsed_value, segment_value, result, parsed_scale, current_numeral_type
+
+        if index == 0:
+            result.invalid.append((text, "LEADING_SCALE"))
+        elif previous_value_type == BufferType.SCALE:
+            result.invalid.append((text, "CONSECUTIVE_SCALES"))
+        elif parsed_value is None and segment_value is None:
+            result.invalid.append((text, "LONELY_SCALE"))
+
+        if parsed_value is not None or segment_value is not None:
+            scale: Scale
+            scale = locale._get_scale(text)
+            if scale:
+                if not parsed_value:
+                    parsed_value = 0.0
+                if not segment_value:
+                    segment_value = 0.0
+                result.seconds += (parsed_value + segment_value) * scale.scale
+                parsed_scale = scale
+
+    for index, element in enumerate(potential_values):
+        current_value = element[0]
+        current_value_type = element[1]
+        current_value_type_converted = current_value_type
+
+        multiplier = False
+        if current_value_type == BufferType.NUMERAL:
+            multiplier = locale._get_numeral(current_value)
+            multiplier = True if multiplier["type"] == "multiplier" else False
+        if multiplier:
+            if parsed_value is not None:
+                handle_multiplier(current_value, index)
+            else:
+                result.invalid.append((current_value, "UNUSED_MULTIPLIER"))
+                segment_value = None
+                parsed_value = None
+                handle_special(current_value)
+        elif current_value_type == BufferType.SPECIAL:
+            handle_special(current_value)
+        elif current_value_type == BufferType.NUMBER:
+            handle_float(current_value)
+        elif current_value_type == BufferType.NUMERAL:
+            handle_numeral(current_value, index)
+        elif current_value_type == BufferType.SCALE:
+            handle_scale(current_value)
+
+        if (
+            current_value_type != BufferType.SPECIAL
+            or current_value in locale._segmentors
+        ):
+            previous_value_type = current_value_type
+            previous_numeral_type = current_numeral_type
+            previous_value_type_converted = current_value_type_converted
+            current_value_type_converted = None
+            current_numeral_type = None
+            current_value_type = None
+            previous_specials = []
+
+        if (parsed_value is not None or segment_value is not None) and parsed_scale:
+            if not parsed_value:
+                parsed_value = 0.0
+            if not segment_value:
+                segment_value = 0.0
+            result.valid.append((parsed_value + segment_value, parsed_scale))
+            parsed_value = None
+            segment_value = None
+            parsed_scale = None
+            starts_with_modifier = False
+
+        if current_value in locale._segmentors:
+            if current_value in previous_segmentors:
+                result.invalid.append((current_value, "CONSECUTIVE_SPECIALS"))
+            if parsed_value is not None:
+                if not segment_value:
+                    segment_value = 0.0
+                segment_value += parsed_value
+            parsed_value = None
+            starts_with_modifier = False
+            previous_segmentors.append(current_value)
+        else:
+            previous_segmentors = []
+
+    if (parsed_value is not None or segment_value is not None) and not parsed_scale:
+        if not parsed_value:
+            parsed_value = 0.0
+        if not segment_value:
+            segment_value = 0.0
+        selected_value = parsed_value + segment_value
+        if not strict and len(potential_values) == 1:
+            result.valid.append((parsed_value + segment_value, locale._second))
+            result.seconds += parsed_value + segment_value
+        else:
+            result.invalid.append(
+                (
+                    selected_value,
+                    "LONELY_VALUE",
+                )
+            )
+
+    if result.valid:
+        if strict and not result.invalid:
+            result.success = True
+        elif not strict:
+            result.success = True
```

### Comparing `timelength-2.0.1/timelength/timelength.py` & `timelength-2.0.2/timelength/timelength.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     - `__str__`: Return the parsed lengths of time.
     - `__repr__`: Return a string representation of the `TimeLength` with attributes included.
 
     ### Example
 
     ```python
     time_length = TimeLength("2 hours 30 minutes")
-    if time_length.success:
-        print(f"Total seconds: {time_length.total_seconds}")
+    if time_length.result.success:
+        print(f"Total Seconds: {time_length.to_seconds()}")
     ```
     """
 
     def __init__(
         self, content: str = "", strict: bool = False, locale: Locale = English()
     ) -> None:
         """Initialize the `TimeLength` based on passed settings and call the `parse` method."""
```

### Comparing `timelength-2.0.1/timelength/utils.py` & `timelength-2.0.2/timelength/utils.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import unicodedata
-
-from timelength.enums import BufferType, CharacterType
-
-
-def is_float(num: str) -> bool:
-    """Check if the passed string is a number."""
-    try:
-        float(num)
-        return True
-    except ValueError:
-        return False
-
-
-def character_type(text: str) -> CharacterType:
-    """Check the type of the passed character based on the `CharacterType` enum."""
-    if is_float(text):
-        return CharacterType.NUMBER
-    elif text.isalpha():
-        return CharacterType.ALPHABET
-    else:
-        return CharacterType.SPECIAL
-
-
-def buffer_type(text: str, scales: list, numerals: list, symbols: list) -> BufferType:
-    """Check the type of the passed string based on the `BufferType` enum."""
-    if is_float(text):
-        return BufferType.NUMBER
-    elif text in scales:
-        return BufferType.SCALE
-    elif text in numerals:
-        return BufferType.NUMERAL
-    elif text in symbols:
-        return BufferType.SPECIAL
-    else:
-        return BufferType.UNKNOWN
-
-
-def remove_diacritics(text: str) -> str:
-    """Replace accented and special characters with their normalized equivalents."""
-    nfkd_form = unicodedata.normalize("NFKD", text)
-    return "".join([c for c in nfkd_form if not unicodedata.combining(c)])
+import unicodedata
+
+from timelength.enums import BufferType, CharacterType
+
+
+def is_float(num: str) -> bool:
+    """Check if the passed string is a number."""
+    try:
+        float(num)
+        return True
+    except ValueError:
+        return False
+
+
+def character_type(text: str) -> CharacterType:
+    """Check the type of the passed character based on the `CharacterType` enum."""
+    if is_float(text):
+        return CharacterType.NUMBER
+    elif text.isalpha():
+        return CharacterType.ALPHABET
+    else:
+        return CharacterType.SPECIAL
+
+
+def buffer_type(text: str, scales: list, numerals: list, symbols: list) -> BufferType:
+    """Check the type of the passed string based on the `BufferType` enum."""
+    if is_float(text):
+        return BufferType.NUMBER
+    elif text in scales:
+        return BufferType.SCALE
+    elif text in numerals:
+        return BufferType.NUMERAL
+    elif text in symbols:
+        return BufferType.SPECIAL
+    else:
+        return BufferType.UNKNOWN
+
+
+def remove_diacritics(text: str) -> str:
+    """Replace accented and special characters with their normalized equivalents."""
+    nfkd_form = unicodedata.normalize("NFKD", text)
+    return "".join([c for c in nfkd_form if not unicodedata.combining(c)])
```

### Comparing `timelength-2.0.1/PKG-INFO` & `timelength-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelength
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python package to parse human readable lengths of time.
 Home-page: https://pypi.org/project/timelength/
 License: MIT
 Keywords: timelength,duration,python,parsing,time
 Author: Etorix
 Author-email: admin@etorix.dev
 Requires-Python: >=3.8,<4.0
@@ -33,25 +33,25 @@
 
 ## Usage (English)
 ### Default
 While `TimeLength.strict` is `False` (default), `TimeLength.result.success` will be `True` if at least one valid result is found, regardless of invalid results.
 ```python
 from timelength import TimeLength
 
-output = TimeLength("1d5h25m and 23miles")
+output = TimeLength("1d5h25m15.5s and 23miles")
 print(output.result.success)
 # True
 print(output.result.seconds)
-# 105900.0
+# 105915.5
 print(output.to_minutes(max_precision = 3))
-# 1765.0
+# 1765.258
 print(output.result.invalid)
 # [('miles', 'UNKNOWN_TERM'), (23.0, 'LONELY_VALUE')]
 print(output.result.valid)
-# [(1.0, Scale(86400.0, "day", "days")), (5.0, Scale(3600.0, "hour", "hours")), (25.0, Scale(60.0, "minute", "minutes"))]
+# [(1.0, Scale(86400.0, "day", "days")), (5.0, Scale(3600.0, "hour", "hours")), (25.0, Scale(60.0, "minute", "minutes")), (15.5, Scale(1.0, "second", "seconds"))]
 ```
 Additionally, if a single lone value is parsed without a paired scale, seconds will be assumed. However, if more than one value is parsed, nothing will be assumed.
 ```python
 output = TimeLength("45")
 print(output.result.invalid)
 # []
 print(output.result.valid)
@@ -70,42 +70,42 @@
 
 output = TimeLength("3.5d, 35m, 19", strict = True)
 print(output.result.success)
 # False
 print(output.result.invalid)
 # [(19.0, "LONELY_VALUE")]
 print(output.result.valid)
-# [(3.5, Scale(scale=86400.0, "day", "days")), (35.0, Scale(scale=60.0, "minute", "minutes"))]
+# [(3.5, Scale(86400.0, "day", "days")), (35.0, Scale(60.0, "minute", "minutes"))]
 ```
 Additionally, unlike with the default behavior, scales must be present. No assumptions will be made.
 
 ## Supported Locales
 1. English
 2. Spanish
-3. Custom (Copy & modify an existing config with new terms as long as your new `Locale` follows the existing config parser's grammar structure)
-4. Custom (Write your own parsing logic if your `Locale`'s grammar structure differs too drastically) (PRs welcome)
+3. Basic Custom (Copy & modify an existing config with new terms as long as your new `Locale` follows the existing config parser's grammar structure)
+4. Advanced Custom (Write your own parsing logic if your `Locale`'s grammar structure differs too drastically) (PRs welcome)
 
 ## Customization
 `timelength` allows for customizing the parsing behavior through JSON configuration. To get started, copy an existing locale JSON in `timelength/locales/`. The custom JSON may be placed anywhere.
 
 **Ensure the JSON being used is from a trusted source, as the parser is loaded dynamically based on the file specified in the JSON. This could allow for unintended code execution if an unsafe config is loaded.**
 
 Valid JSONs must include the following keys, even if their contents are empty: 
 - `connectors`
   - Characters/phrases that join two parts of the same segment.
 - `segmentors`
   - Characters/phrases that join two segments together.
-- `allowed_symbols`
-  - Characters that won't be categorized as an invalid input. If sent multiple times in a row (ex: !!), they will still be marked as invalid.
+- `allowed_terms`
+  - Characters or terms that won't be categorized as an invalid input. If sent multiple times in a row (ex: !!), they will still be marked as invalid.
 - `decimal_separators`
   - Characters used to separate decimals from digits. Can't have overlap with `thousand_separators`.
 - `thousand_separators`
   - Characters used to break up large numbers. Can't have overlap with `decimal_separators`.
 - `parser_file`
-  - The name of this locale's parser file located in `timelength/parsers/`, or the path to the parser file if stored elsewhere. 
+  - The name of this locale's parser file (extension included) located in `timelength/parsers/`, or the path to the parser file if stored elsewhere. 
   - **Ensure only a trusted file is used as this could allow unintended code execution.**
   - The internal parser method must share a name with the file.
 - `numerals`
   - Word forms of numbers. May be populated or left empty. Each element must itself have the following keys, even if their contents are not used:
     - `type`
       - The numeral type.
     - `value`
@@ -119,15 +119,15 @@
     - singular
       - The lowercase singular form of this scale.
     - plural
       - The lowercase plural form of this scale.
     - terms
       - All terms that could be parsed as this scale. Accents and other NFKD markings should not be present as they are filtered from the user input.
 - `extra_data`
-  - Any data a parser needs that is not already covered. May be populated or left empty. The locale loads this into a `Locale._extra_data` attribute, leaving the parser to utilizes it.
+  - Any data a parser needs that is not already covered. May be populated or left empty. The locale loads this into a `Locale._extra_data` attribute, leaving the parser to utilize it.
 
 Once your custom JSON is filled out, you can use it as follows:
 ```python
 from timelength import TimeLength, CustomLocale
 
 output = TimeLength("30 minutes", locale = CustomLocale("path/to/config.json"))
 ```
```

