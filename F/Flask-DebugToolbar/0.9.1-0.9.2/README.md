# Comparing `tmp/Flask-DebugToolbar-0.9.1.tar.gz` & `tmp/Flask-DebugToolbar-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-DebugToolbar-0.9.1.tar", last modified: Mon Nov 24 21:28:56 2014, max compression
+gzip compressed data, was "dist/Flask-DebugToolbar-0.9.2.tar", last modified: Fri Dec  5 23:43:02 2014, max compression
```

## Comparing `Flask-DebugToolbar-0.9.1.tar` & `Flask-DebugToolbar-0.9.2.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/
--rw-r--r--   0 matt       (501) staff       (20)     8118 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      141 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/compat.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/
--rw-r--r--   0 matt       (501) staff       (20)     1520 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      607 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/config_vars.py
--rw-r--r--   0 matt       (501) staff       (20)     1317 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/headers.py
--rw-r--r--   0 matt       (501) staff       (20)     3258 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/logger.py
--rw-r--r--   0 matt       (501) staff       (20)     3609 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/profiler.py
--rw-r--r--   0 matt       (501) staff       (20)     1458 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/request_vars.py
--rw-r--r--   0 matt       (501) staff       (20)     4191 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/sqlalchemy.py
--rw-r--r--   0 matt       (501) staff       (20)     3916 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/template.py
--rw-r--r--   0 matt       (501) staff       (20)     3262 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/timer.py
--rw-r--r--   0 matt       (501) staff       (20)      515 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/versions.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/
--rw-r--r--   0 matt       (501) staff       (20)     2980 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/codemirror.css
--rw-r--r--   0 matt       (501) staff       (20)   121448 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/codemirror.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clike/
--rw-r--r--   0 matt       (501) staff       (20)     8404 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clike/clike.js
--rw-r--r--   0 matt       (501) staff       (20)     3054 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clike/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clojure/
--rw-r--r--   0 matt       (501) staff       (20)    12435 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clojure/clojure.js
--rw-r--r--   0 matt       (501) staff       (20)     1981 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clojure/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/
--rw-r--r--   0 matt       (501) staff       (20)    10731 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/coffeescript.js
--rw-r--r--   0 matt       (501) staff       (20)    21995 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1151 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/LICENSE
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/css/
--rw-r--r--   0 matt       (501) staff       (20)     3646 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/css/css.js
--rw-r--r--   0 matt       (501) staff       (20)     1051 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/css/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/diff/
--rw-r--r--   0 matt       (501) staff       (20)       89 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/diff/diff.css
--rw-r--r--   0 matt       (501) staff       (20)      316 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/diff/diff.js
--rw-r--r--   0 matt       (501) staff       (20)     3860 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/diff/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ecl/
--rw-r--r--   0 matt       (501) staff       (20)     8721 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ecl/ecl.js
--rw-r--r--   0 matt       (501) staff       (20)     1164 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ecl/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/gfm/
--rw-r--r--   0 matt       (501) staff       (20)     3023 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/gfm/gfm.js
--rw-r--r--   0 matt       (501) staff       (20)     1297 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/gfm/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/go/
--rw-r--r--   0 matt       (501) staff       (20)     5471 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/go/go.js
--rw-r--r--   0 matt       (501) staff       (20)     1765 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/go/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/groovy/
--rw-r--r--   0 matt       (501) staff       (20)     7154 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/groovy/groovy.js
--rw-r--r--   0 matt       (501) staff       (20)     1760 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/groovy/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/haskell/
--rw-r--r--   0 matt       (501) staff       (20)     7478 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/haskell/haskell.js
--rw-r--r--   0 matt       (501) staff       (20)     1780 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/haskell/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlembedded/
--rw-r--r--   0 matt       (501) staff       (20)     2280 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlembedded/htmlembedded.js
--rw-r--r--   0 matt       (501) staff       (20)     1703 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlembedded/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlmixed/
--rw-r--r--   0 matt       (501) staff       (20)     2839 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlmixed/htmlmixed.js
--rw-r--r--   0 matt       (501) staff       (20)     1558 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlmixed/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/javascript/
--rw-r--r--   0 matt       (501) staff       (20)     2539 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/javascript/index.html
--rw-r--r--   0 matt       (501) staff       (20)    12693 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/javascript/javascript.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/jinja2/
--rw-r--r--   0 matt       (501) staff       (20)     1040 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/jinja2/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1909 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/jinja2/jinja2.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/less/
--rw-r--r--   0 matt       (501) staff       (20)    14320 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/less/index.html
--rw-r--r--   0 matt       (501) staff       (20)     8250 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/less/less.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/lua/
--rw-r--r--   0 matt       (501) staff       (20)     1693 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/lua/index.html
--rw-r--r--   0 matt       (501) staff       (20)     5347 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/lua/lua.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/markdown/
--rw-r--r--   0 matt       (501) staff       (20)     9858 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/markdown/index.html
--rw-r--r--   0 matt       (501) staff       (20)     6140 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/markdown/markdown.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/mysql/
--rw-r--r--   0 matt       (501) staff       (20)     1132 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/mysql/index.html
--rw-r--r--   0 matt       (501) staff       (20)     7776 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/mysql/mysql.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ntriples/
--rw-r--r--   0 matt       (501) staff       (20)      998 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ntriples/index.html
--rw-r--r--   0 matt       (501) staff       (20)     6348 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ntriples/ntriples.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/
--rw-r--r--   0 matt       (501) staff       (20)     1108 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1078 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     2605 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/pascal.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/
--rw-r--r--   0 matt       (501) staff       (20)     1212 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1094 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)    29358 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/perl.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/php/
--rw-r--r--   0 matt       (501) staff       (20)     1499 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/php/index.html
--rw-r--r--   0 matt       (501) staff       (20)     6076 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/php/php.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/plsql/
--rw-r--r--   0 matt       (501) staff       (20)     1553 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/plsql/index.html
--rw-r--r--   0 matt       (501) staff       (20)     8430 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/plsql/plsql.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/properties/
--rwxr-xr-x   0 matt       (501) staff       (20)     1189 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/properties/index.html
--rwxr-xr-x   0 matt       (501) staff       (20)     1734 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/properties/properties.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/
--rw-r--r--   0 matt       (501) staff       (20)     2835 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1075 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/LICENSE.txt
--rw-r--r--   0 matt       (501) staff       (20)    12178 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/python.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/
--rw-r--r--   0 matt       (501) staff       (20)     2263 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1486 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     4936 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/r.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/changes/
--rw-r--r--   0 matt       (501) staff       (20)      654 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/changes/changes.js
--rw-r--r--   0 matt       (501) staff       (20)     1793 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/changes/index.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/spec/
--rw-r--r--   0 matt       (501) staff       (20)     3037 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/spec/index.html
--rw-r--r--   0 matt       (501) staff       (20)      267 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/spec/spec.css
--rw-r--r--   0 matt       (501) staff       (20)     2698 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/spec/spec.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rst/
--rw-r--r--   0 matt       (501) staff       (20)    17578 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rst/index.html
--rw-r--r--   0 matt       (501) staff       (20)     8429 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rst/rst.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/
--rw-r--r--   0 matt       (501) staff       (20)     5412 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1487 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     7400 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/ruby.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rust/
--rw-r--r--   0 matt       (501) staff       (20)     1071 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rust/index.html
--rw-r--r--   0 matt       (501) staff       (20)    15457 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rust/rust.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/scheme/
--rw-r--r--   0 matt       (501) staff       (20)     2198 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/scheme/index.html
--rw-r--r--   0 matt       (501) staff       (20)    10562 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/scheme/scheme.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smalltalk/
--rw-r--r--   0 matt       (501) staff       (20)     1484 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smalltalk/index.html
--rw-r--r--   0 matt       (501) staff       (20)     3448 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smalltalk/smalltalk.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smarty/
--rw-r--r--   0 matt       (501) staff       (20)     2306 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smarty/index.html
--rw-r--r--   0 matt       (501) staff       (20)     3852 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smarty/smarty.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/sparql/
--rw-r--r--   0 matt       (501) staff       (20)     1196 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/sparql/index.html
--rw-r--r--   0 matt       (501) staff       (20)     4605 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/sparql/sparql.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/
--rw-r--r--   0 matt       (501) staff       (20)     3610 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/index.html
--rw-r--r--   0 matt       (501) staff       (20)     4413 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/stex.js
--rw-r--r--   0 matt       (501) staff       (20)     5785 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/test.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/
--rw-r--r--   0 matt       (501) staff       (20)     4187 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/index.html
--rw-r--r--   0 matt       (501) staff       (20)      840 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.css
--rw-r--r--   0 matt       (501) staff       (20)     9500 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/vbscript/
--rw-r--r--   0 matt       (501) staff       (20)     1161 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/vbscript/index.html
--rw-r--r--   0 matt       (501) staff       (20)      867 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/vbscript/vbscript.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/velocity/
--rw-r--r--   0 matt       (501) staff       (20)     2761 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/velocity/index.html
--rw-r--r--   0 matt       (501) staff       (20)     4959 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/velocity/velocity.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/verilog/
--rw-r--r--   0 matt       (501) staff       (20)     6782 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/verilog/index.html
--rw-r--r--   0 matt       (501) staff       (20)     6996 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/verilog/verilog.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xml/
--rw-r--r--   0 matt       (501) staff       (20)     1617 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xml/index.html
--rw-r--r--   0 matt       (501) staff       (20)     7984 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xml/xml.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xmlpure/
--rw-r--r--   0 matt       (501) staff       (20)     2332 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xmlpure/index.html
--rw-r--r--   0 matt       (501) staff       (20)    17763 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xmlpure/xmlpure.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/
--rw-r--r--   0 matt       (501) staff       (20)     9447 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/index.html
--rw-r--r--   0 matt       (501) staff       (20)     1109 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/LICENSE
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/
--rw-r--r--   0 matt       (501) staff       (20)     1171 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/index.html
--rw-r--r--   0 matt       (501) staff       (20)     6114 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testBase.js
--rw-r--r--   0 matt       (501) staff       (20)      639 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testEmptySequenceKeyword.js
--rw-r--r--   0 matt       (501) staff       (20)      789 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testMultiAttr.js
--rw-r--r--   0 matt       (501) staff       (20)     5494 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testNamespaces.js
--rw-r--r--   0 matt       (501) staff       (20)      719 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testProcessingInstructions.js
--rw-r--r--   0 matt       (501) staff       (20)     1070 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testQuotes.js
--rw-r--r--   0 matt       (501) staff       (20)    15976 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/xquery.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/yaml/
--rw-r--r--   0 matt       (501) staff       (20)     1744 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/yaml/index.html
--rw-r--r--   0 matt       (501) staff       (20)     2677 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/yaml/yaml.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/
--rw-r--r--   0 matt       (501) staff       (20)     1037 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/cobalt.css
--rw-r--r--   0 matt       (501) staff       (20)     1050 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/eclipse.css
--rw-r--r--   0 matt       (501) staff       (20)      593 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/elegant.css
--rw-r--r--   0 matt       (501) staff       (20)     2066 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/lesser-dark.css
--rw-r--r--   0 matt       (501) staff       (20)     1151 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/monokai.css
--rw-r--r--   0 matt       (501) staff       (20)      524 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/neat.css
--rw-r--r--   0 matt       (501) staff       (20)     1118 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/night.css
--rw-r--r--   0 matt       (501) staff       (20)     1300 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/rubyblue.css
--rw-r--r--   0 matt       (501) staff       (20)     2296 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/xq-dark.css
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/
--rw-r--r--   0 matt       (501) staff       (20)     5868 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/closetag.js
--rw-r--r--   0 matt       (501) staff       (20)      401 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/dialog.css
--rw-r--r--   0 matt       (501) staff       (20)     1962 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/dialog.js
--rw-r--r--   0 matt       (501) staff       (20)     5950 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/foldcode.js
--rw-r--r--   0 matt       (501) staff       (20)    10183 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/formatting.js
--rw-r--r--   0 matt       (501) staff       (20)     5385 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/javascript-hint.js
--rw-r--r--   0 matt       (501) staff       (20)     1656 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/match-highlighter.js
--rw-r--r--   0 matt       (501) staff       (20)     1862 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/overlay.js
--rw-r--r--   0 matt       (501) staff       (20)     1611 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/runmode.js
--rw-r--r--   0 matt       (501) staff       (20)     4725 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/search.js
--rw-r--r--   0 matt       (501) staff       (20)     4717 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/searchcursor.js
--rw-r--r--   0 matt       (501) staff       (20)      368 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/simple-hint.css
--rw-r--r--   0 matt       (501) staff       (20)     2943 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/simple-hint.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/css/
--rw-r--r--   0 matt       (501) staff       (20)     7919 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/css/toolbar.css
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/
--rw-r--r--   0 matt       (501) staff       (20)       54 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/asc.gif
--rw-r--r--   0 matt       (501) staff       (20)      575 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/back.png
--rw-r--r--   0 matt       (501) staff       (20)      614 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/back_hover.png
--rw-r--r--   0 matt       (501) staff       (20)       64 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/bg.gif
--rw-r--r--   0 matt       (501) staff       (20)      604 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/close.png
--rw-r--r--   0 matt       (501) staff       (20)      711 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/close_hover.png
--rw-r--r--   0 matt       (501) staff       (20)       54 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/desc.gif
--rw-r--r--   0 matt       (501) staff       (20)      404 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/djdt_vertical.png
--rw-r--r--   0 matt       (501) staff       (20)      444 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/indicator.png
--rw-r--r--   0 matt       (501) staff       (20)       70 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/panel_bg.png
--rwxr-xr-x   0 matt       (501) staff       (20)      538 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/tick-red.png
--rwxr-xr-x   0 matt       (501) staff       (20)      569 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/tick.png
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/
--rw-r--r--   0 matt       (501) staff       (20)    84362 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/jquery.js
--rw-r--r--   0 matt       (501) staff       (20)    40914 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/jquery.tablesorter.js
--rw-r--r--   0 matt       (501) staff       (20)     7074 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/toolbar.js
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/
--rw-r--r--   0 matt       (501) staff       (20)     2045 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/base.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/
--rw-r--r--   0 matt       (501) staff       (20)      398 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/config_vars.html
--rw-r--r--   0 matt       (501) staff       (20)      327 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/headers.html
--rw-r--r--   0 matt       (501) staff       (20)      614 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/logger.html
--rw-r--r--   0 matt       (501) staff       (20)      716 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/profiler.html
--rw-r--r--   0 matt       (501) staff       (20)     1888 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/request_vars.html
--rw-r--r--   0 matt       (501) staff       (20)     2475 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/sqlalchemy.html
--rw-r--r--   0 matt       (501) staff       (20)      797 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/sqlalchemy_explain.html
--rw-r--r--   0 matt       (501) staff       (20)      867 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/sqlalchemy_select.html
--rw-r--r--   0 matt       (501) staff       (20)      696 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/template.html
--rw-r--r--   0 matt       (501) staff       (20)     5757 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/template_editor.html
--rw-r--r--   0 matt       (501) staff       (20)      388 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/timer.html
--rw-r--r--   0 matt       (501) staff       (20)      568 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/redirect.html
--rw-r--r--   0 matt       (501) staff       (20)     2120 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/toolbar.py
--rw-r--r--   0 matt       (501) staff       (20)     1614 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/flask_debugtoolbar/utils.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)        1 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2014-11-23 23:47:00.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)     5492 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)       40 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)     9841 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)       19 2014-11-24 21:28:55.000000 Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)      100 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/MANIFEST.in
--rw-r--r--   0 matt       (501) staff       (20)     5492 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     1094 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/README.rst
--rw-r--r--   0 matt       (501) staff       (20)       59 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1362 2014-11-24 21:15:08.000000 Flask-DebugToolbar-0.9.1/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-11-24 21:28:56.000000 Flask-DebugToolbar-0.9.1/test/
--rw-r--r--   0 matt       (501) staff       (20)     1054 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.1/test/test_toolbar.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/
+-rw-r--r--   0 matt       (501) staff       (20)     8034 2014-12-04 22:13:10.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      141 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/compat.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/
+-rw-r--r--   0 matt       (501) staff       (20)     1520 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      607 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/config_vars.py
+-rw-r--r--   0 matt       (501) staff       (20)     1317 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/headers.py
+-rw-r--r--   0 matt       (501) staff       (20)     3258 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/logger.py
+-rw-r--r--   0 matt       (501) staff       (20)     3609 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/profiler.py
+-rw-r--r--   0 matt       (501) staff       (20)     1458 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/request_vars.py
+-rw-r--r--   0 matt       (501) staff       (20)     3868 2014-12-05 23:37:20.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/sqlalchemy.py
+-rw-r--r--   0 matt       (501) staff       (20)     3916 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/template.py
+-rw-r--r--   0 matt       (501) staff       (20)     3262 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/timer.py
+-rw-r--r--   0 matt       (501) staff       (20)      515 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/versions.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/
+-rw-r--r--   0 matt       (501) staff       (20)     2980 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/codemirror.css
+-rw-r--r--   0 matt       (501) staff       (20)   121448 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/codemirror.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clike/
+-rw-r--r--   0 matt       (501) staff       (20)     8404 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clike/clike.js
+-rw-r--r--   0 matt       (501) staff       (20)     3054 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clike/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clojure/
+-rw-r--r--   0 matt       (501) staff       (20)    12435 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clojure/clojure.js
+-rw-r--r--   0 matt       (501) staff       (20)     1981 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clojure/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/
+-rw-r--r--   0 matt       (501) staff       (20)    10731 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/coffeescript.js
+-rw-r--r--   0 matt       (501) staff       (20)    21995 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1151 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/LICENSE
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/css/
+-rw-r--r--   0 matt       (501) staff       (20)     3646 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/css/css.js
+-rw-r--r--   0 matt       (501) staff       (20)     1051 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/css/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/diff/
+-rw-r--r--   0 matt       (501) staff       (20)       89 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/diff/diff.css
+-rw-r--r--   0 matt       (501) staff       (20)      316 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/diff/diff.js
+-rw-r--r--   0 matt       (501) staff       (20)     3860 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/diff/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ecl/
+-rw-r--r--   0 matt       (501) staff       (20)     8721 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ecl/ecl.js
+-rw-r--r--   0 matt       (501) staff       (20)     1164 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ecl/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/gfm/
+-rw-r--r--   0 matt       (501) staff       (20)     3023 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/gfm/gfm.js
+-rw-r--r--   0 matt       (501) staff       (20)     1297 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/gfm/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/go/
+-rw-r--r--   0 matt       (501) staff       (20)     5471 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/go/go.js
+-rw-r--r--   0 matt       (501) staff       (20)     1765 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/go/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/groovy/
+-rw-r--r--   0 matt       (501) staff       (20)     7154 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/groovy/groovy.js
+-rw-r--r--   0 matt       (501) staff       (20)     1760 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/groovy/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/haskell/
+-rw-r--r--   0 matt       (501) staff       (20)     7478 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/haskell/haskell.js
+-rw-r--r--   0 matt       (501) staff       (20)     1780 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/haskell/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlembedded/
+-rw-r--r--   0 matt       (501) staff       (20)     2280 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlembedded/htmlembedded.js
+-rw-r--r--   0 matt       (501) staff       (20)     1703 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlembedded/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlmixed/
+-rw-r--r--   0 matt       (501) staff       (20)     2839 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlmixed/htmlmixed.js
+-rw-r--r--   0 matt       (501) staff       (20)     1558 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlmixed/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/javascript/
+-rw-r--r--   0 matt       (501) staff       (20)     2539 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/javascript/index.html
+-rw-r--r--   0 matt       (501) staff       (20)    12693 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/javascript/javascript.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/jinja2/
+-rw-r--r--   0 matt       (501) staff       (20)     1040 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/jinja2/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1909 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/jinja2/jinja2.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/less/
+-rw-r--r--   0 matt       (501) staff       (20)    14320 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/less/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     8250 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/less/less.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/lua/
+-rw-r--r--   0 matt       (501) staff       (20)     1693 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/lua/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     5347 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/lua/lua.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/markdown/
+-rw-r--r--   0 matt       (501) staff       (20)     9858 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/markdown/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     6140 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/markdown/markdown.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/mysql/
+-rw-r--r--   0 matt       (501) staff       (20)     1132 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/mysql/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     7776 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/mysql/mysql.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ntriples/
+-rw-r--r--   0 matt       (501) staff       (20)      998 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ntriples/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     6348 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ntriples/ntriples.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/
+-rw-r--r--   0 matt       (501) staff       (20)     1108 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1078 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     2605 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/pascal.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/
+-rw-r--r--   0 matt       (501) staff       (20)     1212 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1094 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)    29358 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/perl.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/php/
+-rw-r--r--   0 matt       (501) staff       (20)     1499 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/php/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     6076 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/php/php.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/plsql/
+-rw-r--r--   0 matt       (501) staff       (20)     1553 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/plsql/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     8430 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/plsql/plsql.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/properties/
+-rwxr-xr-x   0 matt       (501) staff       (20)     1189 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/properties/index.html
+-rwxr-xr-x   0 matt       (501) staff       (20)     1734 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/properties/properties.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/
+-rw-r--r--   0 matt       (501) staff       (20)     2835 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1075 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/LICENSE.txt
+-rw-r--r--   0 matt       (501) staff       (20)    12178 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/python.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/
+-rw-r--r--   0 matt       (501) staff       (20)     2263 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1486 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     4936 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/r.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/changes/
+-rw-r--r--   0 matt       (501) staff       (20)      654 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/changes/changes.js
+-rw-r--r--   0 matt       (501) staff       (20)     1793 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/changes/index.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/spec/
+-rw-r--r--   0 matt       (501) staff       (20)     3037 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/spec/index.html
+-rw-r--r--   0 matt       (501) staff       (20)      267 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/spec/spec.css
+-rw-r--r--   0 matt       (501) staff       (20)     2698 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/spec/spec.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rst/
+-rw-r--r--   0 matt       (501) staff       (20)    17578 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rst/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     8429 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rst/rst.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/
+-rw-r--r--   0 matt       (501) staff       (20)     5412 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1487 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     7400 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/ruby.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rust/
+-rw-r--r--   0 matt       (501) staff       (20)     1071 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rust/index.html
+-rw-r--r--   0 matt       (501) staff       (20)    15457 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rust/rust.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/scheme/
+-rw-r--r--   0 matt       (501) staff       (20)     2198 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/scheme/index.html
+-rw-r--r--   0 matt       (501) staff       (20)    10562 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/scheme/scheme.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smalltalk/
+-rw-r--r--   0 matt       (501) staff       (20)     1484 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smalltalk/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     3448 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smalltalk/smalltalk.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smarty/
+-rw-r--r--   0 matt       (501) staff       (20)     2306 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smarty/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     3852 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smarty/smarty.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/sparql/
+-rw-r--r--   0 matt       (501) staff       (20)     1196 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/sparql/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     4605 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/sparql/sparql.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/
+-rw-r--r--   0 matt       (501) staff       (20)     3610 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     4413 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/stex.js
+-rw-r--r--   0 matt       (501) staff       (20)     5785 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/test.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/
+-rw-r--r--   0 matt       (501) staff       (20)     4187 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/index.html
+-rw-r--r--   0 matt       (501) staff       (20)      840 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.css
+-rw-r--r--   0 matt       (501) staff       (20)     9500 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/vbscript/
+-rw-r--r--   0 matt       (501) staff       (20)     1161 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/vbscript/index.html
+-rw-r--r--   0 matt       (501) staff       (20)      867 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/vbscript/vbscript.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/velocity/
+-rw-r--r--   0 matt       (501) staff       (20)     2761 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/velocity/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     4959 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/velocity/velocity.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/verilog/
+-rw-r--r--   0 matt       (501) staff       (20)     6782 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/verilog/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     6996 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/verilog/verilog.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xml/
+-rw-r--r--   0 matt       (501) staff       (20)     1617 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xml/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     7984 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xml/xml.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xmlpure/
+-rw-r--r--   0 matt       (501) staff       (20)     2332 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xmlpure/index.html
+-rw-r--r--   0 matt       (501) staff       (20)    17763 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xmlpure/xmlpure.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/
+-rw-r--r--   0 matt       (501) staff       (20)     9447 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     1109 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/LICENSE
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/
+-rw-r--r--   0 matt       (501) staff       (20)     1171 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     6114 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testBase.js
+-rw-r--r--   0 matt       (501) staff       (20)      639 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testEmptySequenceKeyword.js
+-rw-r--r--   0 matt       (501) staff       (20)      789 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testMultiAttr.js
+-rw-r--r--   0 matt       (501) staff       (20)     5494 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testNamespaces.js
+-rw-r--r--   0 matt       (501) staff       (20)      719 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testProcessingInstructions.js
+-rw-r--r--   0 matt       (501) staff       (20)     1070 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testQuotes.js
+-rw-r--r--   0 matt       (501) staff       (20)    15976 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/xquery.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/yaml/
+-rw-r--r--   0 matt       (501) staff       (20)     1744 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/yaml/index.html
+-rw-r--r--   0 matt       (501) staff       (20)     2677 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/yaml/yaml.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/
+-rw-r--r--   0 matt       (501) staff       (20)     1037 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/cobalt.css
+-rw-r--r--   0 matt       (501) staff       (20)     1050 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/eclipse.css
+-rw-r--r--   0 matt       (501) staff       (20)      593 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/elegant.css
+-rw-r--r--   0 matt       (501) staff       (20)     2066 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/lesser-dark.css
+-rw-r--r--   0 matt       (501) staff       (20)     1151 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/monokai.css
+-rw-r--r--   0 matt       (501) staff       (20)      524 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/neat.css
+-rw-r--r--   0 matt       (501) staff       (20)     1118 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/night.css
+-rw-r--r--   0 matt       (501) staff       (20)     1300 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/rubyblue.css
+-rw-r--r--   0 matt       (501) staff       (20)     2296 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/xq-dark.css
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/
+-rw-r--r--   0 matt       (501) staff       (20)     5868 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/closetag.js
+-rw-r--r--   0 matt       (501) staff       (20)      401 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/dialog.css
+-rw-r--r--   0 matt       (501) staff       (20)     1962 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/dialog.js
+-rw-r--r--   0 matt       (501) staff       (20)     5950 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/foldcode.js
+-rw-r--r--   0 matt       (501) staff       (20)    10183 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/formatting.js
+-rw-r--r--   0 matt       (501) staff       (20)     5385 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/javascript-hint.js
+-rw-r--r--   0 matt       (501) staff       (20)     1656 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/match-highlighter.js
+-rw-r--r--   0 matt       (501) staff       (20)     1862 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/overlay.js
+-rw-r--r--   0 matt       (501) staff       (20)     1611 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/runmode.js
+-rw-r--r--   0 matt       (501) staff       (20)     4725 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/search.js
+-rw-r--r--   0 matt       (501) staff       (20)     4717 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/searchcursor.js
+-rw-r--r--   0 matt       (501) staff       (20)      368 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/simple-hint.css
+-rw-r--r--   0 matt       (501) staff       (20)     2943 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/simple-hint.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/css/
+-rw-r--r--   0 matt       (501) staff       (20)     7868 2014-12-05 23:37:20.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/css/toolbar.css
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/
+-rw-r--r--   0 matt       (501) staff       (20)       54 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/asc.gif
+-rw-r--r--   0 matt       (501) staff       (20)      575 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/back.png
+-rw-r--r--   0 matt       (501) staff       (20)      614 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/back_hover.png
+-rw-r--r--   0 matt       (501) staff       (20)       64 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/bg.gif
+-rw-r--r--   0 matt       (501) staff       (20)      604 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/close.png
+-rw-r--r--   0 matt       (501) staff       (20)      711 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/close_hover.png
+-rw-r--r--   0 matt       (501) staff       (20)       54 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/desc.gif
+-rw-r--r--   0 matt       (501) staff       (20)      404 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/djdt_vertical.png
+-rw-r--r--   0 matt       (501) staff       (20)      444 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/indicator.png
+-rw-r--r--   0 matt       (501) staff       (20)       70 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/panel_bg.png
+-rwxr-xr-x   0 matt       (501) staff       (20)      538 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/tick-red.png
+-rwxr-xr-x   0 matt       (501) staff       (20)      569 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/tick.png
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/
+-rw-r--r--   0 matt       (501) staff       (20)    84362 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/jquery.js
+-rw-r--r--   0 matt       (501) staff       (20)    40914 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/jquery.tablesorter.js
+-rw-r--r--   0 matt       (501) staff       (20)     7074 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/toolbar.js
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/
+-rw-r--r--   0 matt       (501) staff       (20)     2045 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/base.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/
+-rw-r--r--   0 matt       (501) staff       (20)      398 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/config_vars.html
+-rw-r--r--   0 matt       (501) staff       (20)      327 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/headers.html
+-rw-r--r--   0 matt       (501) staff       (20)      614 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/logger.html
+-rw-r--r--   0 matt       (501) staff       (20)      716 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/profiler.html
+-rw-r--r--   0 matt       (501) staff       (20)     1888 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/request_vars.html
+-rw-r--r--   0 matt       (501) staff       (20)     1046 2014-12-05 23:37:20.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/sqlalchemy.html
+-rw-r--r--   0 matt       (501) staff       (20)      886 2014-11-24 23:02:00.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/sqlalchemy_select.html
+-rw-r--r--   0 matt       (501) staff       (20)      696 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/template.html
+-rw-r--r--   0 matt       (501) staff       (20)     5757 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/template_editor.html
+-rw-r--r--   0 matt       (501) staff       (20)      388 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/timer.html
+-rw-r--r--   0 matt       (501) staff       (20)      568 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/redirect.html
+-rw-r--r--   0 matt       (501) staff       (20)     2120 2014-12-04 01:41:53.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/toolbar.py
+-rw-r--r--   0 matt       (501) staff       (20)     2177 2014-12-04 22:13:10.000000 Flask-DebugToolbar-0.9.2/flask_debugtoolbar/utils.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)        1 2014-12-05 23:43:00.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2014-11-23 23:47:00.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)     5810 2014-12-05 23:43:00.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)       40 2014-12-05 23:43:00.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)     9800 2014-12-05 23:43:01.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)       19 2014-12-05 23:43:00.000000 Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)      100 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/MANIFEST.in
+-rw-r--r--   0 matt       (501) staff       (20)     5810 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     1094 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/README.rst
+-rw-r--r--   0 matt       (501) staff       (20)       59 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1362 2014-12-05 23:42:06.000000 Flask-DebugToolbar-0.9.2/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-12-05 23:43:02.000000 Flask-DebugToolbar-0.9.2/test/
+-rw-r--r--   0 matt       (501) staff       (20)     1054 2014-11-23 23:46:21.000000 Flask-DebugToolbar-0.9.2/test/test_toolbar.py
+-rw-r--r--   0 matt       (501) staff       (20)     3827 2014-12-04 22:13:10.000000 Flask-DebugToolbar-0.9.2/test/test_utils.py
```

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/__init__.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 
-from flask import current_app, request, g
+from flask import Blueprint, current_app, request, g, send_from_directory
 from flask.globals import _request_ctx_stack
-from flask import send_from_directory
 from jinja2 import Environment, PackageLoader
 from werkzeug.exceptions import HTTPException
 from werkzeug.urls import url_quote_plus
 
-from flask_debugtoolbar.toolbar import DebugToolbar
 from flask_debugtoolbar.compat import iteritems
-from flask import Blueprint
+from flask_debugtoolbar.toolbar import DebugToolbar
+from flask_debugtoolbar.utils import decode_text
 
 
 module = Blueprint('debugtoolbar', __name__)
 
 
 def replace_insensitive(string, target, replacement):
     """Similar to string.replace() but is case insensitive
@@ -26,18 +25,15 @@
         return string[:index] + replacement + string[index + len(target):]
     else:  # no results so return the original string
         return string
 
 
 def _printable(value):
     try:
-        value = repr(value)
-        if isinstance(value, bytes):
-            value = value.decode('ascii', 'replace')
-        return value
+        return decode_text(repr(value))
     except Exception as e:
         return '<repr(%s) raised %s: %s>' % (
                object.__repr__(value), type(e).__name__, e)
 
 
 class DebugToolbarExtension(object):
     _static_dir = os.path.realpath(
```

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/__init__.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/config_vars.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/config_vars.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/headers.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/logger.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/logger.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/profiler.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/profiler.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/request_vars.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/request_vars.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/sqlalchemy.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,37 +106,26 @@
             })
         return self.render('panels/sqlalchemy.html', {'queries': data})
 
 # Panel views
 
 
 @module.route('/sqlalchemy/sql_select', methods=['GET', 'POST'])
-def sql_select():
+@module.route('/sqlalchemy/sql_explain', methods=['GET', 'POST'],
+              defaults=dict(explain=True))
+def sql_select(explain=False):
     statement, params = load_query(request.args['query'])
     engine = SQLAlchemy().get_engine(current_app)
 
+    if explain:
+        if engine.driver == 'pysqlite':
+            statement = 'EXPLAIN QUERY PLAN\n%s' % statement
+        else:
+            statement = 'EXPLAIN\n%s' % statement
+
     result = engine.execute(statement, params)
     return g.debug_toolbar.render('panels/sqlalchemy_select.html', {
         'result': result.fetchall(),
         'headers': result.keys(),
         'sql': format_sql(statement, params),
         'duration': float(request.args['duration']),
-    })
-
-
-@module.route('/sqlalchemy/sql_explain', methods=['GET', 'POST'])
-def sql_explain():
-    statement, params = load_query(request.args['query'])
-    engine = SQLAlchemy().get_engine(current_app)
-
-    if engine.driver == 'pysqlite':
-        query = 'EXPLAIN QUERY PLAN %s' % statement
-    else:
-        query = 'EXPLAIN %s' % statement
-
-    result = engine.execute(query, params)
-    return g.debug_toolbar.render('panels/sqlalchemy_explain.html', {
-        'result': result.fetchall(),
-        'headers': result.keys(),
-        'sql': format_sql(statement, params),
-        'duration': float(request.args['duration']),
-    })
+    })
```

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/template.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/template.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/timer.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/panels/versions.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/codemirror.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/codemirror.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clike/clike.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clike/clike.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clike/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clike/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clojure/clojure.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clojure/clojure.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/clojure/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/clojure/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/coffeescript.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/coffeescript.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/coffeescript/LICENSE` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/coffeescript/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/css/css.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/css/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/css/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/diff/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/diff/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ecl/ecl.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ecl/ecl.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ecl/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ecl/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/gfm/gfm.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/gfm/gfm.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/gfm/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/gfm/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/go/go.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/go/go.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/go/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/go/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/groovy/groovy.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/groovy/groovy.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/groovy/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/groovy/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/haskell/haskell.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/haskell/haskell.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/haskell/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/haskell/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlembedded/htmlembedded.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlembedded/htmlembedded.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlembedded/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlembedded/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlmixed/htmlmixed.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/htmlmixed/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/htmlmixed/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/javascript/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/javascript/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/javascript/javascript.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/jinja2/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/jinja2/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/jinja2/jinja2.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/jinja2/jinja2.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/less/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/less/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/less/less.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/less/less.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/lua/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/lua/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/lua/lua.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/lua/lua.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/markdown/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/markdown/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/markdown/markdown.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/mysql/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/mysql/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/mysql/mysql.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/mysql/mysql.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ntriples/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ntriples/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ntriples/ntriples.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ntriples/ntriples.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/LICENSE` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/pascal/pascal.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/pascal/pascal.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/LICENSE` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/perl/perl.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/perl/perl.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/php/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/php/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/php/php.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/php/php.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/plsql/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/plsql/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/plsql/plsql.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/plsql/plsql.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/properties/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/properties/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/properties/properties.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/properties/properties.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/LICENSE.txt` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/python/python.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/LICENSE` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/r/r.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/r/r.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/changes/changes.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/changes/changes.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/changes/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/changes/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/spec/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/spec/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rpm/spec/spec.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rpm/spec/spec.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rst/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rst/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rst/rst.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rst/rst.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/LICENSE` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/ruby/ruby.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/ruby/ruby.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rust/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rust/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/rust/rust.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/rust/rust.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/scheme/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/scheme/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/scheme/scheme.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/scheme/scheme.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smalltalk/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smalltalk/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smalltalk/smalltalk.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smalltalk/smalltalk.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smarty/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smarty/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/smarty/smarty.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/smarty/smarty.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/sparql/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/sparql/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/sparql/sparql.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/sparql/sparql.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/stex.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/stex.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/stex/test.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/stex/test.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/tiddlywiki/tiddlywiki.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/vbscript/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/vbscript/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/vbscript/vbscript.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/vbscript/vbscript.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/velocity/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/velocity/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/velocity/velocity.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/velocity/velocity.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/verilog/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/verilog/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/verilog/verilog.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/verilog/verilog.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xml/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xml/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xml/xml.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xmlpure/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xmlpure/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xmlpure/xmlpure.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xmlpure/xmlpure.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/LICENSE` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testBase.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testBase.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testEmptySequenceKeyword.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testEmptySequenceKeyword.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testMultiAttr.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testMultiAttr.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testNamespaces.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testNamespaces.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testProcessingInstructions.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testProcessingInstructions.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/test/testQuotes.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/test/testQuotes.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/xquery/xquery.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/xquery/xquery.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/yaml/index.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/yaml/index.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/mode/yaml/yaml.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/mode/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/cobalt.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/cobalt.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/eclipse.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/eclipse.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/elegant.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/elegant.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/lesser-dark.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/lesser-dark.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/monokai.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/monokai.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/neat.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/neat.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/night.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/night.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/rubyblue.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/rubyblue.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/theme/xq-dark.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/theme/xq-dark.css`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/closetag.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/closetag.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/dialog.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/dialog.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/foldcode.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/foldcode.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/formatting.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/formatting.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/javascript-hint.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/javascript-hint.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/match-highlighter.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/match-highlighter.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/overlay.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/overlay.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/runmode.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/runmode.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/search.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/search.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/searchcursor.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/searchcursor.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/codemirror/util/simple-hint.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/codemirror/util/simple-hint.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/css/toolbar.css` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/css/toolbar.css`

 * *Files 1% similar despite different names*

```diff
@@ -318,18 +318,14 @@
   z-index:100000002;
 }
 
 #flDebug .flSQLHideStacktraceDiv tbody th {
   text-align: left;
 }
 
-#flDebug .flSqlExplain td {
-  white-space: pre;
-}
-
 #flDebug span.flDebugLineChart {
   background-color:#777;
   height:3px;
   position:absolute;
   bottom:0;
   top:0;
   left:0;
```

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/back.png` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/back.png`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/back_hover.png` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/back_hover.png`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/close.png` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/close.png`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/close_hover.png` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/close_hover.png`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/tick-red.png` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/tick-red.png`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/img/tick.png` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/img/tick.png`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/jquery.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/jquery.tablesorter.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/static/js/toolbar.js` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/static/js/toolbar.js`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/base.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/logger.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/logger.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/profiler.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/profiler.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/request_vars.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/request_vars.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/sqlalchemy_explain.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/sqlalchemy_select.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 <div class="flDebugPanelTitle">
   <a class="flDebugClose flDebugBack" href="">Back</a>
-  <h3>SQL Explained</h3>
+  <h3>SQL Details</h3>
 </div>
 <div class="flDebugPanelContent">
   <div class="scroll">
     <dl>
       <dt>Executed SQL</dt>
-      <dd>{{ sql|safe }}</dd>
-      <dt>Time</dt>
-      <dd>{{ '%.4f'|format(duration) }} ms</dd>
+      <dd>{{ sql }}</dd>
+      <dt>Original query duration</dt>
+      <dd>{{ '%.4f'|format(duration * 1000) }} ms</dd>
     </dl>
-    <table class="flSqlExplain">
+    {% if result %}
+    <table class="flSqlSelect">
       <thead>
         <tr>
           {% for h in headers %}
             <th>{{ h|upper }}</th>
           {% endfor %}
         </tr>
       </thead>
       <tbody>
         {% for row in result %}
-            <tr class="{{ loop.cycle('fjDebugOdd', 'fjDebugEven') }}">
+            <tr class="{{ loop.cycle('flDebugOdd', 'flDebugEven') }}">
             {% for column in row %}
               <td>{{ column }}</td>
             {% endfor %}
           </tr>
         {% endfor %}
       </tbody>
     </table>
+    {% else %}
+    <p>Empty set</p>
+    {% endif %}
   </div>
 </div>
-
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
 Back
-******** SSQQLL EExxppllaaiinneedd ********
+******** SSQQLL DDeettaaiillss ********
   Executed SQL
-      {{ sql|safe }}
-  Time
-      {{ '%.4f'|format(duration) }} ms
+      {{ sql }}
+  Original query duration
+      {{ '%.4f'|format(duration * 1000) }} ms
+{% if result %}
 {{{{ hh||uuppppeerr }}}}
 {{ column }}
+{% else %}
+Empty set
+{% endif %}
```

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/template.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/template.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/panels/template_editor.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/panels/template_editor.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/templates/redirect.html` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/flask_debugtoolbar/toolbar.py` & `Flask-DebugToolbar-0.9.2/flask_debugtoolbar/toolbar.py`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/PKG-INFO` & `Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Flask-DebugToolbar
-Version: 0.9.1
+Version: 0.9.2
 Summary: A port of the Django debug toolbar to Flask
 Home-page: http://flask-debugtoolbar.rtfd.org/
 Author: Matt Good
 Author-email: matt@matt-good.net
 License: BSD
 Description: Flask Debug-toolbar
         ===================
@@ -50,14 +50,23 @@
         
         .. _documentation: http://flask-debugtoolbar.readthedocs.org
         
         
         Changes
         =======
         
+        0.9.2 (2014-12-05)
+        ------------------
+        
+        Fixes:
+        
+        - HTML escape SQL queries when syntax highlighting is not available
+        - Use case-insensitive comparison to normalize filenames on Windows
+        - Fix exception when SQL query contained non-ASCII characters
+        
         0.9.1 (2014-11-24)
         ------------------
         
         Fixes:
         
         - Fix SQL queries with byte strings on Python 3
         - Fix displaying values whose `repr()` contains unprintable characters
```

### Comparing `Flask-DebugToolbar-0.9.1/Flask_DebugToolbar.egg-info/SOURCES.txt` & `Flask-DebugToolbar-0.9.2/Flask_DebugToolbar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -171,13 +171,13 @@
 flask_debugtoolbar/templates/redirect.html
 flask_debugtoolbar/templates/panels/config_vars.html
 flask_debugtoolbar/templates/panels/headers.html
 flask_debugtoolbar/templates/panels/logger.html
 flask_debugtoolbar/templates/panels/profiler.html
 flask_debugtoolbar/templates/panels/request_vars.html
 flask_debugtoolbar/templates/panels/sqlalchemy.html
-flask_debugtoolbar/templates/panels/sqlalchemy_explain.html
 flask_debugtoolbar/templates/panels/sqlalchemy_select.html
 flask_debugtoolbar/templates/panels/template.html
 flask_debugtoolbar/templates/panels/template_editor.html
 flask_debugtoolbar/templates/panels/timer.html
-test/test_toolbar.py
+test/test_toolbar.py
+test/test_utils.py
```

### Comparing `Flask-DebugToolbar-0.9.1/PKG-INFO` & `Flask-DebugToolbar-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Flask-DebugToolbar
-Version: 0.9.1
+Version: 0.9.2
 Summary: A port of the Django debug toolbar to Flask
 Home-page: http://flask-debugtoolbar.rtfd.org/
 Author: Matt Good
 Author-email: matt@matt-good.net
 License: BSD
 Description: Flask Debug-toolbar
         ===================
@@ -50,14 +50,23 @@
         
         .. _documentation: http://flask-debugtoolbar.readthedocs.org
         
         
         Changes
         =======
         
+        0.9.2 (2014-12-05)
+        ------------------
+        
+        Fixes:
+        
+        - HTML escape SQL queries when syntax highlighting is not available
+        - Use case-insensitive comparison to normalize filenames on Windows
+        - Fix exception when SQL query contained non-ASCII characters
+        
         0.9.1 (2014-11-24)
         ------------------
         
         Fixes:
         
         - Fix SQL queries with byte strings on Python 3
         - Fix displaying values whose `repr()` contains unprintable characters
```

### Comparing `Flask-DebugToolbar-0.9.1/README.rst` & `Flask-DebugToolbar-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-DebugToolbar-0.9.1/setup.py` & `Flask-DebugToolbar-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 except:
     README = ''
     CHANGES = ''
 
 
 setup(
     name='Flask-DebugToolbar',
-    version='0.9.1',
+    version='0.9.2',
     url='http://flask-debugtoolbar.rtfd.org/',
     license='BSD',
     author='Michael van Tellingen',
     author_email='michaelvantellingen@gmail.com',
     maintainer='Matt Good',
     maintainer_email='matt@matt-good.net',
     description='A port of the Django debug toolbar to Flask',
```

### Comparing `Flask-DebugToolbar-0.9.1/test/test_toolbar.py` & `Flask-DebugToolbar-0.9.2/test/test_toolbar.py`

 * *Files identical despite different names*

