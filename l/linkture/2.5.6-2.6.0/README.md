# Comparing `tmp/linkture-2.5.6.tar.gz` & `tmp/linkture-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkture-2.5.6.tar", last modified: Wed Apr 24 13:53:18 2024, max compression
+gzip compressed data, was "linkture-2.6.0.tar", last modified: Wed Apr 24 16:57:39 2024, max compression
```

## Comparing `linkture-2.5.6.tar` & `linkture-2.6.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-04-24 13:53:05.188418 linkture-2.5.6/LICENSE
--rw-r--r--   0        0        0     9870 2024-04-24 13:53:05.188418 linkture-2.5.6/README.md
--rw-r--r--   0        0        0     1429 2024-04-24 13:53:18.036353 linkture-2.5.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/__init__.py
--rwxr-xr-x   0        0        0    29101 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/__main__.py
--rw-r--r--   0        0        0     1904 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/res/custom.json
--rw-r--r--   0        0        0   581632 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/res/resources.db
--rw-r--r--   0        0        0     1297 2024-04-24 13:53:05.192417 linkture-2.5.6/src/linkture/res/rss-36.png
--rw-r--r--   0        0        0    11098 1970-01-01 00:00:00.000000 linkture-2.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 16:57:24.794953 linkture-2.6.0/LICENSE
+-rw-r--r--   0        0        0     9870 2024-04-24 16:57:24.794953 linkture-2.6.0/README.md
+-rw-r--r--   0        0        0     1407 2024-04-24 16:57:39.362927 linkture-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/__init__.py
+-rwxr-xr-x   0        0        0     6427 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/__main__.py
+-rwxr-xr-x   0        0        0    23670 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/linkture.py
+-rw-r--r--   0        0        0     1904 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/res/custom.json
+-rw-r--r--   0        0        0   581632 2024-04-24 16:57:24.798953 linkture-2.6.0/src/linkture/res/resources.db
+-rw-r--r--   0        0        0     1297 2024-04-24 16:57:24.798953 linkture-2.6.0/src/linkture/res/rss-36.png
+-rw-r--r--   0        0        0    11068 1970-01-01 00:00:00.000000 linkture-2.6.0/PKG-INFO
```

### Comparing `linkture-2.5.6/LICENSE` & `linkture-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linkture-2.5.6/README.md` & `linkture-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `linkture-2.5.6/pyproject.toml` & `linkture-2.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     { name = "Eryk J.", email = "infiniti@inventati.org" },
 ]
 dependencies = [
     "setuptools>=59.6.0",
     "argparse>=1.4.0",
     "regex>=2023.8.8",
     "unidecode>=1.3.8",
-    "pathlib>=1.0.1",
     "pandas==2.2.2",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -32,15 +31,15 @@
     "bible",
     "scriptures",
     "scripture-references",
     "scripture-translation",
     "scripture-parser",
     "scripture-linker",
 ]
-version = "v2.5.6"
+version = "v2.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/erykjj/linkture"
 Issues = "https://github.com/erykjj/linkture/issues"
@@ -52,8 +51,8 @@
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.version]
 source = "file"
-path = "src/linkture/__main__.py"
+path = "src/linkture/linkture.py"
```

### Comparing `linkture-2.5.6/src/linkture/__main__.py` & `linkture-2.6.0/src/linkture/linkture.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,22 +22,20 @@
   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
   SOFTWARE.
 """
 
-__version__ = 'v2.5.6'
+__app__ = 'linkture'
+__version__ = 'v2.6.0'
 
 
-import argparse, json, regex, sqlite3
+import json, regex, sqlite3
 import pandas as pd
-
-from ast import literal_eval
-from pathlib import Path
 from unidecode import unidecode
 
 
 available_languages = ('Cebuano', 'Chinese', 'Danish', 'Dutch', 'English', 'French', 'German', 'Greek', 'Hungarian', 'Italian', 'Japanese', 'Korean', 'Norwegian', 'Polish', 'Portuguese', 'Russian', 'Spanish', 'Tagalog', 'Ukrainian')
 non_latin = ('Chinese', 'Greek', 'Japanese', 'Korean', 'Russian', 'Ukrainian')
 
 
@@ -64,33 +62,32 @@
         elif form == "standard":
             form = 4
         elif form == "official":
             form = 5
         else:
             form = 3
         self._src_book_names = {}
-        path = Path(__file__).resolve().parent
 
         self._tr_book_names = ['Bible']
-        con = sqlite3.connect(path / 'res/resources.db')
+        con = sqlite3.connect('res/resources.db')
         cur = con.cursor()
         for rec in cur.execute(f"SELECT * FROM Books WHERE Language = '{translate}';").fetchall():
             if self._upper:
                 tr = rec[form].upper()
             else:
                 tr = rec[form]
             self._tr_book_names.insert(rec[2], tr)
         for rec in cur.execute(f"SELECT * FROM Books WHERE Language = '{language}';").fetchall():
             for i in range(3,6):
                 item = rec[i]
                 if not self._nl:
                     item = unidecode(item)
                 normalized = regex.sub(r'\p{P}|\p{Z}', '', item.upper())
                 self._src_book_names[normalized] = rec[2]
-        with open(path / 'res/custom.json', 'r', encoding='UTF-8') as json_file:
+        with open('res/custom.json', 'r', encoding='UTF-8') as json_file:
             b = json.load(json_file)
         if language in b.keys():
             for row in b[language]:
                 names = row[1].split(', ')
                 for item in names:
                     if not self._nl:
                         item = unidecode(item)
@@ -604,110 +601,7 @@
         try:
             for i in self._verses[self._verses['VerseId'] == int(verse)].values[0][1:]:
                 bcv += str(i).zfill(3)
             return f"('{bcv[1:]}', '{bcv[1:]}')"
         except:
             self._error_report(verse, 'OUT OF RANGE')
             return None
-
-
-def _main(args):
-
-    def switchboard(text):
-        if args['cc']:
-            return s.code_chapter(args['cc'])
-        elif args['cv']:
-            return s.code_verse(args['cv'])
-        elif args['sc']:
-            return s.serial_chapter_number(args['sc'])
-        elif args['sv']:
-            return s.serial_verse_number(args['sv'])
-        if args['l'] is not None:
-            prefix = '<a href='
-            suffix = '>'
-            if len(args['l']) > 1:
-                suffix = args['l'][1]
-            if len(args['l']) > 0:
-                prefix = args['l'][0]
-            return s.link_scriptures(text, prefix, suffix)
-        elif args['c']:
-            return s.code_scriptures(text)
-        elif args['d']:
-            return s.decode_scriptures(literal_eval(text))
-        elif args['x']:
-            return s.list_scriptures(text)
-        elif args['t']:
-            return s.tag_scriptures(text)
-        else:
-            return s.rewrite_scriptures(text)
-
-    form = None
-    if args['standard']:
-        form = 'standard'
-    elif args['official']:
-        form = 'official'
-    elif args['full']:
-        form = 'full'
-
-    s = Scriptures(language=args['language'], translate=args['translate'], form=form, separator=args['s'], upper=args['u'], verbose=(not args['q']))
-
-    if args['f']:
-        if args['o'] and (args['o'] == args['f']):
-            print('Make sure in-file and out-file are different!\n')
-            exit()
-        with open(args['f'], 'r', encoding='UTF-8') as f:
-            txt = f.read()
-    else:
-        txt = args['r']
-
-    if txt:
-        txt = switchboard(txt)
-    else:
-        print(parser.format_help())
-        exit()
-
-    if args['o']:
-        with open(args['o'], 'w', encoding='UTF-8') as f:
-            f.write(str(txt))
-    else:
-        print(txt)
-
-if __name__ == "__main__":
-    PROJECT_PATH = Path(__file__).resolve().parent
-    APP = 'linkture' # Path(__file__).stem
-    parser = argparse.ArgumentParser(description="PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode. See README for more information")
-
-    parser.add_argument('-v', action='version', version=f"{APP} {__version__}", help='show version and exit')
-    parser.add_argument('-q', action='store_true', help="don't show errors")
-
-    function_group = parser.add_argument_group('data source (one required - except for auxiliary functions, which only take command-line arguments)', 'choose between terminal or file input:')
-    mode = function_group.add_mutually_exclusive_group()
-    mode.add_argument('-f', metavar='in-file', help='get input from file (UTF-8)')
-    mode.add_argument('-r', metavar='reference', help='process "reference; reference; etc."')
-    parser.add_argument('-o', metavar='out-file', help='output file (terminal output if not provided)')
-
-    parser.add_argument('--language', default='English', choices=available_languages, help='indicate source language for book names (English if unspecified)')
-    parser.add_argument('--translate', choices=available_languages, help='indicate output language for book names (same as source if unspecified)')
-    parser.add_argument('-s', metavar='separator', default=' ', help='segment separator (space by default)')
-    parser.add_argument('-u', action='store_true', help='capitalize (upper-case) book names')
-    format_group = parser.add_argument_group('output format (optional)', 'if provided, book names will be rewritten accordingly:')
-    formats = format_group.add_mutually_exclusive_group()
-    formats.add_argument('--full', action='store_true', help='output as full name - default (eg., "Genesis")')
-    formats.add_argument('--official', action='store_true', help='output as official abbreviation (eg., "Ge")')
-    formats.add_argument('--standard', action='store_true', help='output as standard abbreviation (eg., "Gen.")')
-
-    type_group = parser.add_argument_group('type of conversion', 'if not specified, references are simply rewritten according to chosen (or default) output format:')
-    tpe = type_group.add_mutually_exclusive_group(required=False)
-    tpe.add_argument('-c', action='store_true', help='encode as BCV-notation ranges')
-    tpe.add_argument('-d', action='store_true', help='decode list of BCV-notation ranges')
-    tpe.add_argument('-l', nargs='*', metavar=('prefix', 'suffix'), help='create <a></a> links; provide a "prefix" and a "suffix" (or neither for testing)')
-    tpe.add_argument('-t', action='store_true', help='tag scriptures with {{ }}')
-    tpe.add_argument('-x', action='store_true', help='extract list of scripture references')
-
-    aux_group = parser.add_argument_group('auxiliary functions')
-    aux = aux_group.add_mutually_exclusive_group(required=False)
-    aux.add_argument('-sc', metavar=('BCV'), help='return the serial number (1-1189) of the chapter with code "BCV" ("bbcccvvv")')
-    aux.add_argument('-sv', metavar=('BCV'), help='return the serial number (1-31091) of the verse with code "BCV" ("bbcccvvv")')
-    aux.add_argument('-cc', metavar=('chapter'), help='return the BCV range for serial chapter number "chapter" (integer value)')
-    aux.add_argument('-cv', metavar=('verse'), help='return the BCV code for serial verse number "verse" (integer value)')
-    args = parser.parse_args()
-    _main(vars(args))
```

### Comparing `linkture-2.5.6/src/linkture/res/custom.json` & `linkture-2.6.0/src/linkture/res/custom.json`

 * *Files identical despite different names*

### Comparing `linkture-2.5.6/src/linkture/res/resources.db` & `linkture-2.6.0/src/linkture/res/resources.db`

 * *Files identical despite different names*

### Comparing `linkture-2.5.6/src/linkture/res/rss-36.png` & `linkture-2.6.0/src/linkture/res/rss-36.png`

 * *Files identical despite different names*

### Comparing `linkture-2.5.6/PKG-INFO` & `linkture-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkture
-Version: 2.5.6
+Version: 2.6.0
 Summary: PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode
 Keywords: bible,scriptures,scripture-references,scripture-translation,scripture-parser,scripture-linker
 Author-Email: "Eryk J." <infiniti@inventati.org>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,14 @@
 Project-URL: Homepage, https://github.com/erykjj/linkture
 Project-URL: Issues, https://github.com/erykjj/linkture/issues
 Requires-Python: >=3.9
 Requires-Dist: setuptools>=59.6.0
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: regex>=2023.8.8
 Requires-Dist: unidecode>=1.3.8
-Requires-Dist: pathlib>=1.0.1
 Requires-Dist: pandas==2.2.2
 Description-Content-Type: text/markdown
 
 # linkture
 
 
 ## Purpose
```

