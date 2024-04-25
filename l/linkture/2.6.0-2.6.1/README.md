# Comparing `tmp/linkture-2.6.0.tar.gz` & `tmp/linkture-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkture-2.6.0.tar", last modified: Wed Apr 24 16:57:39 2024, max compression
+gzip compressed data, was "linkture-2.6.1.tar", last modified: Wed Apr 24 23:50:46 2024, max compression
```

## Comparing `linkture-2.6.0.tar` & `linkture-2.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-04-24 16:57:24.794953 linkture-2.6.0/LICENSE
--rw-r--r--   0        0        0     9870 2024-04-24 16:57:24.794953 linkture-2.6.0/README.md
--rw-r--r--   0        0        0     1407 2024-04-24 16:57:39.362927 linkture-2.6.0/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/__init__.py
--rwxr-xr-x   0        0        0     6427 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/__main__.py
--rwxr-xr-x   0        0        0    23670 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/linkture.py
--rw-r--r--   0        0        0     1904 2024-04-24 16:57:24.794953 linkture-2.6.0/src/linkture/res/custom.json
--rw-r--r--   0        0        0   581632 2024-04-24 16:57:24.798953 linkture-2.6.0/src/linkture/res/resources.db
--rw-r--r--   0        0        0     1297 2024-04-24 16:57:24.798953 linkture-2.6.0/src/linkture/res/rss-36.png
--rw-r--r--   0        0        0    11068 1970-01-01 00:00:00.000000 linkture-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 23:50:32.106253 linkture-2.6.1/LICENSE
+-rw-r--r--   0        0        0     9787 2024-04-24 23:50:32.106253 linkture-2.6.1/README.md
+-rw-r--r--   0        0        0     1407 2024-04-24 23:50:46.318279 linkture-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-24 23:50:32.106253 linkture-2.6.1/src/linkture/__init__.py
+-rwxr-xr-x   0        0        0     6478 2024-04-24 23:50:32.106253 linkture-2.6.1/src/linkture/__main__.py
+-rwxr-xr-x   0        0        0    23701 2024-04-24 23:50:32.106253 linkture-2.6.1/src/linkture/linkture.py
+-rw-r--r--   0        0        0     1904 2024-04-24 23:50:32.106253 linkture-2.6.1/src/linkture/res/custom.json
+-rw-r--r--   0        0        0   581632 2024-04-24 23:50:32.110253 linkture-2.6.1/src/linkture/res/resources.db
+-rw-r--r--   0        0        0     1297 2024-04-24 23:50:32.110253 linkture-2.6.1/src/linkture/res/rss-36.png
+-rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 linkture-2.6.1/PKG-INFO
```

### Comparing `linkture-2.6.0/LICENSE` & `linkture-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linkture-2.6.0/README.md` & `linkture-2.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# linkture
-
-
 ## Purpose
 
 This module contains functions to parse and process Bible scripture references.
 
 The parser can work in **Cebuano, Chinese, Danish, Dutch, English, French, German, Greek, Hungarian, Italian, Japanese, Korean, Norwegian, Polish, Portuguese, Russian, Spanish, Tagalog and Ukrainian**. It will **recognize** such references and **validate** them to ensure the chapter(s) and/or verse(s) are within range.
 
 It *does not* work with whole books (like "James") unless they are preceded by a number (like "1 John"); otherwise it would have to look up ever single word. Also, it will *not* find the multi-word book name "Song of Solomon" (and its variations), though this (and any other scripture) can be force-detected by tagging the desired reference "manually" within the source text (eg., "{{Song of Solomon 1:1}}") - *one book* per brace pair. These two limitations aside, it works with most book name variants in all the available languages (including common abbreviations): "2 Sam.", "2nd Samuel", "II Samuel", "2Sa", etc. Any special/unusual variants can be added to the *res/custom.json* list.
@@ -84,91 +81,99 @@
 
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --standard
 John 17:17; 2 Tim. 3:16, 17
 
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --official
 Joh 17:17; 2Ti 3:16, 17
 
+
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -c
 [('43017017', '43017017'), ('55003016', '55003017')]
 
 $ python3 -m linkture -r "[('43017017', '43017017'), ('55003016', '55003017')]" -d --translate German
 ['Johannes 17:17', '2. Timotheus 3:16, 17']
 
+
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -l '<a href="https://my.website.com/' '/index.html" class="test">'
 <a href="https://my.website.com/43:17:17/index.html" class="test">John 17:17</a>; <a href="https://my.website.com/55:3:16-55:3:17/index.html" class="test">2 Timothy 3:16, 17</a>
 
+
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --translate Chinese
 约翰福音 17:17; 提摩太后书 3:16, 17
 
 $ python3 -m linkture -r "约翰福音 17:17; 提摩太后书 3:16, 17" --language Chinese --translate Dutch
 Johannes 17:17; 2 Timotheüs 3:16, 17
 
 $ python3 -m linkture -r "{{Jean 17:17}}; 2 Timothée 3:16, 17" --language French --translate Spanish --standard
 Juan 17:17; 2 Tim. 3:16, 17
 
 $ python3 -m linkture -r "Mat 17:17; Paul 3:16, 17" --full -x
 ['Matthew 17:17']
 
+
 $ python3 -m linkture -cc 2
 ('01002001', '01002025')
 
 $ python3 -m linkture -cv 31091
 ('66022021', '66022021')
 
 $ python3 -m linkture -sv '01001001'
 1
 
 python3 -m linkture -sc '66022001'
 1189
 
+
 python3 -m linkture -r '2Ti 3:16, 17' --full -s '_'
 2_Timothy_3:16,_17
 ```
 
 **Note**: The serial verse options (`-sv` and `-cv`) *do not* count Psalm headings as separate verses.
 
 Of course, you can pass a whole text file to parse and process using the `-f in_file` flag, instead of `-r "references"`. And you can output to another text file (instead of the terminal) using `-o out_file`.
 
 Unless you use `-q`, you will see in the terminal any out-of-range errors encountered while parsing. Of course, these entries will not be processed, but they will not affect the rest of the operation.
 
 ____
 ## Script/import usage
 
-Assume the text (short string or long document) you want to process is in the variable `txt`. It's in English, but you would like the scriptures to be in Spanish, with the full book name:
+Assume the text (short string or long document) you want to process is in the variable `txt`.
+
 ```
 from linkture import Scriptures
 
 s = Scriptures(language="English", translate="Spanish", form="full")
 
+
 lst = s.list_scriptures(txt)
 # returns a list of (valid) extracted scriptures in the desired language and format
 
 lst = s.code_scriptures(txt)
 # returns a list of BCV-range tuples (start, end)
 
 html = s.link_scriptures(txt, prefix='<a href="http://mywebsite.com/', suffix='" class="b"')
 # this will turn all references into HTML links
 
 tagged = s.tag_scriptures(txt)
 # tagged will contain your document with the translated references enclosed within double braces
 
-txt = s.rewrite_scriptures(txt)
+new_txt = s.rewrite_scriptures(txt)
 # the references will simply be rewritten in the desired language and format
 
-i = s.serial_chapter_number(txt)
+
+i = s.serial_chapter_number(ch_bcv)
 # returns the serial number (1-1189) of the chapter identified by the provided BCV-format string; verse digits irrelevant
 
-i = s.serial_verse_number(txt)
+i = s.serial_verse_number(vs_bcv)
 # returns the serial number (1-31091) of the verse identified by the provided BCV-format string
 
-txt = s.code_chapter(i)
+ch_bcv = s.code_chapter(i)
 # returns a BCV-format range string for the whole chapter indicated by the provided integer (1-1189)
 
-txt = s.code_verse(i)
+vs_bcv = s.code_verse(i)
 # returns a BCV-format range string for the verse indicated by the provided integer (1-31091)
 ```
 
 Parameters:
 * *language* - source language for Scripture parsing
 * *translate* - language for Bible book name translation
 * *form* - output format of Bible book names
```

### Comparing `linkture-2.6.0/pyproject.toml` & `linkture-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "bible",
     "scriptures",
     "scripture-references",
     "scripture-translation",
     "scripture-parser",
     "scripture-linker",
 ]
-version = "v2.6.0"
+version = "v2.6.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/erykjj/linkture"
 Issues = "https://github.com/erykjj/linkture/issues"
```

### Comparing `linkture-2.6.0/src/linkture/__main__.py` & `linkture-2.6.1/src/linkture/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
   SOFTWARE.
 """
 
 import argparse
-from .linkture import available_languages, __app__, __version__, Scriptures
+from .linkture import _available_languages, __app__, __version__, Scriptures
 from ast import literal_eval
 
 
 def main(args):
 
     def switchboard(text):
         if args['cc']:
@@ -39,19 +39,19 @@
         elif args['cv']:
             return s.code_verse(args['cv'])
         elif args['sc']:
             return s.serial_chapter_number(args['sc'])
         elif args['sv']:
             return s.serial_verse_number(args['sv'])
         if args['l'] is not None:
-            prefix = '<a href='
-            suffix = '>'
-            if len(args['l']) > 1:
+            prefix = '<a href="'
+            suffix = '">'
+            if len(args['l']) > 1 and args['l'][1] != '':
                 suffix = args['l'][1]
-            if len(args['l']) > 0:
+            if len(args['l']) > 0 and args['l'][0] != '':
                 prefix = args['l'][0]
             return s.link_scriptures(text, prefix, suffix)
         elif args['c']:
             return s.code_scriptures(text)
         elif args['d']:
             return s.decode_scriptures(literal_eval(text))
         elif args['x']:
@@ -100,16 +100,16 @@
 
 function_group = parser.add_argument_group('data source (one required - except for auxiliary functions, which only take command-line arguments)', 'choose between terminal or file input:')
 mode = function_group.add_mutually_exclusive_group()
 mode.add_argument('-f', metavar='in-file', help='get input from file (UTF-8)')
 mode.add_argument('-r', metavar='reference', help='process "reference; reference; etc."')
 parser.add_argument('-o', metavar='out-file', help='output file (terminal output if not provided)')
 
-parser.add_argument('--language', default='English', choices=available_languages, help='indicate source language for book names (English if unspecified)')
-parser.add_argument('--translate', choices=available_languages, help='indicate output language for book names (same as source if unspecified)')
+parser.add_argument('--language', default='English', choices=_available_languages, help='indicate source language for book names (English if unspecified)')
+parser.add_argument('--translate', choices=_available_languages, help='indicate output language for book names (same as source if unspecified)')
 parser.add_argument('-s', metavar='separator', default=' ', help='segment separator (space by default)')
 parser.add_argument('-u', action='store_true', help='capitalize (upper-case) book names')
 format_group = parser.add_argument_group('output format (optional)', 'if provided, book names will be rewritten accordingly:')
 formats = format_group.add_mutually_exclusive_group()
 formats.add_argument('--full', action='store_true', help='output as full name - default (eg., "Genesis")')
 formats.add_argument('--official', action='store_true', help='output as official abbreviation (eg., "Ge")')
 formats.add_argument('--standard', action='store_true', help='output as standard abbreviation (eg., "Gen.")')
```

### Comparing `linkture-2.6.0/src/linkture/linkture.py` & `linkture-2.6.1/src/linkture/linkture.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,39 +23,39 @@
   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
   SOFTWARE.
 """
 
 __app__ = 'linkture'
-__version__ = 'v2.6.0'
+__version__ = 'v2.6.1'
 
 
 import json, regex, sqlite3
 import pandas as pd
 from unidecode import unidecode
 
 
-available_languages = ('Cebuano', 'Chinese', 'Danish', 'Dutch', 'English', 'French', 'German', 'Greek', 'Hungarian', 'Italian', 'Japanese', 'Korean', 'Norwegian', 'Polish', 'Portuguese', 'Russian', 'Spanish', 'Tagalog', 'Ukrainian')
-non_latin = ('Chinese', 'Greek', 'Japanese', 'Korean', 'Russian', 'Ukrainian')
+_available_languages = ('Cebuano', 'Chinese', 'Danish', 'Dutch', 'English', 'French', 'German', 'Greek', 'Hungarian', 'Italian', 'Japanese', 'Korean', 'Norwegian', 'Polish', 'Portuguese', 'Russian', 'Spanish', 'Tagalog', 'Ukrainian')
+_non_latin = ('Chinese', 'Greek', 'Japanese', 'Korean', 'Russian', 'Ukrainian')
 
 
 class Scriptures():
 
     def __init__(self, language='English', translate=None, form=None, separator=' ', upper=False, verbose=False):
         self._verbose = verbose
         self._separator = separator
-        if language not in available_languages:
+        if language not in _available_languages:
             raise ValueError("Indicated source language is not an option!")
         if translate:
-            if translate not in available_languages:
+            if translate not in _available_languages:
                 raise ValueError("Indicated translation language is not an option!")
         else:
             translate = language
-        if language in non_latin:
+        if language in _non_latin:
             self._nl = True
         else:
             self._nl = False
         self._rewrite = bool((language != translate) or form)
         self._upper = upper
         if form == "full":
             form = 3
@@ -64,30 +64,30 @@
         elif form == "official":
             form = 5
         else:
             form = 3
         self._src_book_names = {}
 
         self._tr_book_names = ['Bible']
-        con = sqlite3.connect('res/resources.db')
+        con = sqlite3.connect('src/linkture/res/resources.db')
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
-        with open('res/custom.json', 'r', encoding='UTF-8') as json_file:
+        with open('src/linkture/res/custom.json', 'r', encoding='UTF-8') as json_file:
             b = json.load(json_file)
         if language in b.keys():
             for row in b[language]:
                 names = row[1].split(', ')
                 for item in names:
                     if not self._nl:
                         item = unidecode(item)
```

### Comparing `linkture-2.6.0/src/linkture/res/custom.json` & `linkture-2.6.1/src/linkture/res/custom.json`

 * *Files identical despite different names*

### Comparing `linkture-2.6.0/src/linkture/res/resources.db` & `linkture-2.6.1/src/linkture/res/resources.db`

 * *Files identical despite different names*

### Comparing `linkture-2.6.0/src/linkture/res/rss-36.png` & `linkture-2.6.1/src/linkture/res/rss-36.png`

 * *Files identical despite different names*

### Comparing `linkture-2.6.0/PKG-INFO` & `linkture-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkture
-Version: 2.6.0
+Version: 2.6.1
 Summary: PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode
 Keywords: bible,scriptures,scripture-references,scripture-translation,scripture-parser,scripture-linker
 Author-Email: "Eryk J." <infiniti@inventati.org>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -22,17 +22,14 @@
 Requires-Dist: setuptools>=59.6.0
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: regex>=2023.8.8
 Requires-Dist: unidecode>=1.3.8
 Requires-Dist: pandas==2.2.2
 Description-Content-Type: text/markdown
 
-# linkture
-
-
 ## Purpose
 
 This module contains functions to parse and process Bible scripture references.
 
 The parser can work in **Cebuano, Chinese, Danish, Dutch, English, French, German, Greek, Hungarian, Italian, Japanese, Korean, Norwegian, Polish, Portuguese, Russian, Spanish, Tagalog and Ukrainian**. It will **recognize** such references and **validate** them to ensure the chapter(s) and/or verse(s) are within range.
 
 It *does not* work with whole books (like "James") unless they are preceded by a number (like "1 John"); otherwise it would have to look up ever single word. Also, it will *not* find the multi-word book name "Song of Solomon" (and its variations), though this (and any other scripture) can be force-detected by tagging the desired reference "manually" within the source text (eg., "{{Song of Solomon 1:1}}") - *one book* per brace pair. These two limitations aside, it works with most book name variants in all the available languages (including common abbreviations): "2 Sam.", "2nd Samuel", "II Samuel", "2Sa", etc. Any special/unusual variants can be added to the *res/custom.json* list.
@@ -112,91 +109,99 @@
 
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --standard
 John 17:17; 2 Tim. 3:16, 17
 
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --official
 Joh 17:17; 2Ti 3:16, 17
 
+
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -c
 [('43017017', '43017017'), ('55003016', '55003017')]
 
 $ python3 -m linkture -r "[('43017017', '43017017'), ('55003016', '55003017')]" -d --translate German
 ['Johannes 17:17', '2. Timotheus 3:16, 17']
 
+
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -l '<a href="https://my.website.com/' '/index.html" class="test">'
 <a href="https://my.website.com/43:17:17/index.html" class="test">John 17:17</a>; <a href="https://my.website.com/55:3:16-55:3:17/index.html" class="test">2 Timothy 3:16, 17</a>
 
+
 $ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --translate Chinese
 约翰福音 17:17; 提摩太后书 3:16, 17
 
 $ python3 -m linkture -r "约翰福音 17:17; 提摩太后书 3:16, 17" --language Chinese --translate Dutch
 Johannes 17:17; 2 Timotheüs 3:16, 17
 
 $ python3 -m linkture -r "{{Jean 17:17}}; 2 Timothée 3:16, 17" --language French --translate Spanish --standard
 Juan 17:17; 2 Tim. 3:16, 17
 
 $ python3 -m linkture -r "Mat 17:17; Paul 3:16, 17" --full -x
 ['Matthew 17:17']
 
+
 $ python3 -m linkture -cc 2
 ('01002001', '01002025')
 
 $ python3 -m linkture -cv 31091
 ('66022021', '66022021')
 
 $ python3 -m linkture -sv '01001001'
 1
 
 python3 -m linkture -sc '66022001'
 1189
 
+
 python3 -m linkture -r '2Ti 3:16, 17' --full -s '_'
 2_Timothy_3:16,_17
 ```
 
 **Note**: The serial verse options (`-sv` and `-cv`) *do not* count Psalm headings as separate verses.
 
 Of course, you can pass a whole text file to parse and process using the `-f in_file` flag, instead of `-r "references"`. And you can output to another text file (instead of the terminal) using `-o out_file`.
 
 Unless you use `-q`, you will see in the terminal any out-of-range errors encountered while parsing. Of course, these entries will not be processed, but they will not affect the rest of the operation.
 
 ____
 ## Script/import usage
 
-Assume the text (short string or long document) you want to process is in the variable `txt`. It's in English, but you would like the scriptures to be in Spanish, with the full book name:
+Assume the text (short string or long document) you want to process is in the variable `txt`.
+
 ```
 from linkture import Scriptures
 
 s = Scriptures(language="English", translate="Spanish", form="full")
 
+
 lst = s.list_scriptures(txt)
 # returns a list of (valid) extracted scriptures in the desired language and format
 
 lst = s.code_scriptures(txt)
 # returns a list of BCV-range tuples (start, end)
 
 html = s.link_scriptures(txt, prefix='<a href="http://mywebsite.com/', suffix='" class="b"')
 # this will turn all references into HTML links
 
 tagged = s.tag_scriptures(txt)
 # tagged will contain your document with the translated references enclosed within double braces
 
-txt = s.rewrite_scriptures(txt)
+new_txt = s.rewrite_scriptures(txt)
 # the references will simply be rewritten in the desired language and format
 
-i = s.serial_chapter_number(txt)
+
+i = s.serial_chapter_number(ch_bcv)
 # returns the serial number (1-1189) of the chapter identified by the provided BCV-format string; verse digits irrelevant
 
-i = s.serial_verse_number(txt)
+i = s.serial_verse_number(vs_bcv)
 # returns the serial number (1-31091) of the verse identified by the provided BCV-format string
 
-txt = s.code_chapter(i)
+ch_bcv = s.code_chapter(i)
 # returns a BCV-format range string for the whole chapter indicated by the provided integer (1-1189)
 
-txt = s.code_verse(i)
+vs_bcv = s.code_verse(i)
 # returns a BCV-format range string for the verse indicated by the provided integer (1-31091)
 ```
 
 Parameters:
 * *language* - source language for Scripture parsing
 * *translate* - language for Bible book name translation
 * *form* - output format of Bible book names
```

