# Comparing `tmp/staticjinjaplus-1.1.2.tar.gz` & `tmp/staticjinjaplus-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-1.1.2.tar", last modified: Tue Apr 16 07:38:06 2024, max compression
+gzip compressed data, was "staticjinjaplus-2.0.0.tar", last modified: Thu Apr 25 06:55:53 2024, max compression
```

## Comparing `staticjinjaplus-1.1.2.tar` & `staticjinjaplus-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 epoc      (1001) epoc      (1001)        0 2024-04-16 07:38:06.706238 staticjinjaplus-1.1.2/
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     1135 2024-04-12 18:10:51.000000 staticjinjaplus-1.1.2/LICENSE.md
--rw-rw-r--   0 epoc      (1001) epoc      (1001)       28 2024-04-12 18:10:51.000000 staticjinjaplus-1.1.2/MANIFEST.in
--rw-r--r--   0 epoc      (1001) epoc      (1001)    20318 2024-04-16 07:38:06.706238 staticjinjaplus-1.1.2/PKG-INFO
--rw-rw-r--   0 epoc      (1001) epoc      (1001)    18577 2024-04-16 07:21:52.000000 staticjinjaplus-1.1.2/README.md
--rw-rw-r--   0 epoc      (1001) epoc      (1001)       38 2024-04-16 07:38:06.706238 staticjinjaplus-1.1.2/setup.cfg
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     4027 2024-04-16 07:37:39.000000 staticjinjaplus-1.1.2/setup.py
-drwxrwxr-x   0 epoc      (1001) epoc      (1001)        0 2024-04-16 07:38:06.702239 staticjinjaplus-1.1.2/staticjinjaplus/
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     6345 2024-04-16 07:19:53.000000 staticjinjaplus-1.1.2/staticjinjaplus/__init__.py
--rw-rw-r--   0 epoc      (1001) epoc      (1001)       21 2024-04-16 07:32:49.000000 staticjinjaplus-1.1.2/staticjinjaplus/__version__.py
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     1253 2024-04-16 07:19:53.000000 staticjinjaplus-1.1.2/staticjinjaplus/cli.py
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     2864 2024-04-12 18:10:51.000000 staticjinjaplus-1.1.2/staticjinjaplus/http.py
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     1243 2024-04-16 07:19:53.000000 staticjinjaplus-1.1.2/staticjinjaplus/jinja_helpers.py
--rw-rw-r--   0 epoc      (1001) epoc      (1001)     1138 2024-04-16 07:19:53.000000 staticjinjaplus-1.1.2/staticjinjaplus/staticjinja_helpers.py
-drwxrwxr-x   0 epoc      (1001) epoc      (1001)        0 2024-04-16 07:38:06.706238 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/
--rw-r--r--   0 epoc      (1001) epoc      (1001)    20318 2024-04-16 07:38:06.000000 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-r--   0 epoc      (1001) epoc      (1001)      455 2024-04-16 07:38:06.000000 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-r--   0 epoc      (1001) epoc      (1001)        1 2024-04-16 07:38:06.000000 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-r--   0 epoc      (1001) epoc      (1001)       60 2024-04-16 07:38:06.000000 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-r--   0 epoc      (1001) epoc      (1001)      132 2024-04-16 07:38:06.000000 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/requires.txt
--rw-rw-r--   0 epoc      (1001) epoc      (1001)       16 2024-04-16 07:38:06.000000 staticjinjaplus-1.1.2/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-2.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    27015 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    25252 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     4150 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/staticjinjaplus/
+-rw-rw-rw-   0        0        0     4300 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     6240 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     3084 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1051 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0     4039 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0    27015 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      146 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-1.1.2/LICENSE.md` & `staticjinjaplus-2.0.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# DON'T BE A DICK PUBLIC LICENSE
-
-> Version 1.1, December 2016
-
-> Copyright (C) 2024 Maxime "Epoc" Gross
-
-Everyone is permitted to copy and distribute verbatim or modified
-copies of this license document.
-
-> DON'T BE A DICK PUBLIC LICENSE
-> TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-1. Do whatever you like with the original work, just don't be a dick.
-
-   Being a dick includes - but is not limited to - the following instances:
-
- 1a. Outright copyright infringement - Don't just copy this and change the name.
- 1b. Selling the unmodified original with no work done what-so-ever, that's REALLY being a dick.
- 1c. Modifying the original work to contain hidden harmful content. That would make you a PROPER dick.
-
-2. If you become rich through modifications, related works/services, or supporting the original work,
-share the love. Only a dick would make loads off this work and not buy the original work's
-creator(s) a pint.
-
-3. Code is provided with no warranty. Using somebody else's code and bitching when it goes wrong makes
-you a DONKEY dick. Fix the problem yourself. A non-dick would submit the fix back.
+# DON'T BE A DICK PUBLIC LICENSE
+
+> Version 1.1, December 2016
+
+> Copyright (C) 2024 Maxime "Epoc" Gross
+
+Everyone is permitted to copy and distribute verbatim or modified
+copies of this license document.
+
+> DON'T BE A DICK PUBLIC LICENSE
+> TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+1. Do whatever you like with the original work, just don't be a dick.
+
+   Being a dick includes - but is not limited to - the following instances:
+
+ 1a. Outright copyright infringement - Don't just copy this and change the name.
+ 1b. Selling the unmodified original with no work done what-so-ever, that's REALLY being a dick.
+ 1c. Modifying the original work to contain hidden harmful content. That would make you a PROPER dick.
+
+2. If you become rich through modifications, related works/services, or supporting the original work,
+share the love. Only a dick would make loads off this work and not buy the original work's
+creator(s) a pint.
+
+3. Code is provided with no warranty. Using somebody else's code and bitching when it goes wrong makes
+you a DONKEY dick. Fix the problem yourself. A non-dick would submit the fix back.
```

### Comparing `staticjinjaplus-1.1.2/PKG-INFO` & `staticjinjaplus-2.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,274 +1,301 @@
-Metadata-Version: 2.1
-Name: staticjinjaplus
-Version: 1.1.2
-Summary: A sweet spot between staticjinja and a full-blown static site generator.
-Home-page: https://github.com/EpocDotFr/staticjinjaplus
-Author: Maxime "Epoc" Gross
-Author-email: contact.nospam@epoc.nospam.fr
-License: DBAD
-Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme
-Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
-Project-URL: Tracker, https://github.com/EpocDotFr/staticjinjaplus/issues
-Project-URL: Changelog, https://github.com/EpocDotFr/staticjinjaplus/releases
-Keywords: static,website,site,generator,staticjinja,jinja,jinja2
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Text Processing :: Markup :: XML
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: staticjinja~=5.0
-Requires-Dist: webassets~=2.0
-Requires-Dist: htmlmin~=0.1
-Requires-Dist: cssutils~=2.10
-Requires-Dist: jsmin~=3.0
-Requires-Dist: environs~=11.0
-Provides-Extra: dev
-Requires-Dist: twine~=5.0; extra == "dev"
-Requires-Dist: build~=1.2; extra == "dev"
-Requires-Dist: setuptools~=69.5; extra == "dev"
-
-
-# staticjinjaplus
-
-A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
-
-![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
-
-[PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
-
-Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
-I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
-order to be able to generate a static website that will actually be ready for real world usage.
-
-staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
-Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
-static site generator.
-
-## Features
-
-All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
-
-  - Simple, file-based configuration to centralize *a handful* of configuration values
-  - Build improvements
-    - Set system locale before building anything (useful when formatting dates to localized strings)
-    - Automatically copy static files to output directory
-    - Define staticjinja contexts in config file
-    - Define [webassets](https://webassets.readthedocs.io/en/latest/) bundles to allow CSS/JS concatenation/minification
-    - Automatically minify XML (including HTML, RSS and Atom)/JSON output
-  - Jinja improvements
-    - A few new Jinja globals/filters to make your life easier
-    - Autoescape is enabled for XML, HTML, RSS and Atom templates
-  - Serve the generated site through a local HTTP server
-    - URL rewrite emulation (for HTML files)
-    - Custom HTTP error pages emulation
-    - IPv6 loopback address support
-  - Publish the generated site through rsync over SSH
-
-**Planned:**
-
-  - Generic support of Markdown-formatted templates collections (forget about the usual "pages" or "articles/blog posts" feature)
-
-## Prerequisites
-
-  - Python >= 3.9
-
-## Installation
-
-From PyPI:
-
-```bash
-$ pip install staticjinjaplus
-```
-
-Locally, after cloning/downloading the repo:
-
-```bash
-$ pip install .
-```
-
-A CLI (`staticjinjaplus`) will be made available upon installation.
-
-## Usage
-
-### Templates
-
-You'll want to write your site's Jinja templates first: write them as usual. By default, staticjinjaplus searches for
-Jinja templates in the `templates` directory where it is invoked. You can change that by using the `TEMPLATES_DIR`
-[configuration value](#configpy).
-
-staticjinjaplus offers the following additional Jinja facilities.
-
-#### Globals
-
-| Name/signature                                  | Type     | Description                                                                                                                                                                                                         |
-|-------------------------------------------------|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `config`                                        | Dict     | Configuration values loaded from [`config.py`](#configpy) (defaults are guaranteed to be provided for built-in values). Only uppercase variables are loaded by staticjinjaplus                                      |
-| `url(path: str, absolute: bool = False) -> str` | Callable | Build (by default) a relative URL to a file located in the `OUTPUT_DIR` directory. Setting `absolute` to `True` prefixes the URL with `BASE_URL`. See [configuration values](#configpy)                             |
-| `icon(name: str) -> markupsafe.Markup`          | Callable | Return the file content of the given SVG icon, marked as safe to be rendered by Jinja. Icons must be saved in the form of `{ASSETS_DIR}/icons/{name}.svg`. Useful to embed SVG icons directly in the generated HTML |
-
-**Usage examples:**
-
-```html+jinja
-{{ config.BASE_URL }}         {# http://localhost:8080/ (by default) #}
-{{ config.MY_CUSTOM_CONFIG }} {# Whatever you defined in your config.py (uppercase variables only) #}
-
-{# url() doesn't care whether an extension is given or not #}
-{{ url('/about.html') }} {# /about.html #}
-{{ url('/about') }}      {# /about #}
-{{ url('about') }}       {# /about #}
-
-{# url() doesn't care about whether a static file is targeted or not #}
-{{ url('/images/logo.png') }} {# /images/logo.png #}
-{{ url('images/logo.png') }}  {# /images/logo.png #}
-
-{# URL is simply prefixed with BASE_URL when generating absolute URLs #}
-{{ url('/images/logo.png', absolute=True) }} {# http://localhost:8080/images/logo.png (by default) #}
-{{ url('images/logo.png', absolute=True) }}  {# http://localhost:8080/images/logo.png (by default) #}
-
-{{ icon('github') }} {# <svg xmlns="http://www.w3.org/2000/svg" ... </svg> #}
-```
-
-#### Filters
-
-| Signature                                      | Description                                                                                                                                                                                                                                                         |
-|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `<data: Dict>\|tojsonm -> str`                 | Serialize the given dictionary to a JSON string. Automatically takes into account the `MINIFY_JSON` [configuration value](#configpy) to minify (or not) the resulting output. Useful for e.g serializing [Schema.org](https://schema.org/)'s JSON-LD-formatted data |
-| `<left: Dict>\|dictmerge(right: Dict) -> Dict` | Merge two dictionaries. Does not modify existing ones, a new one will be created. Does **not** merge deeply                                                                                                                                                         |
-
-**Usage examples:**
-
-```html+jinja
-{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == False:
-                                 {
-                                     "yes": true
-                                 }
-                             #}
-
-{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == True:
-                                 {"yes":true}
-                             #}
-
-{{ dict(yes=True)|dictmerge(dict(no=False)) }} {# {"yes": True, "no": False} #}
-```
-
-### Command line interface
-
-The `staticjinjaplus` CLI is your main and only way to interact with staticjinjaplus. The following commands are available.
-
-#### `staticjinjaplus build`
-
-Build the site by rendering your templates from the `TEMPLATES_DIR` directory in the `OUTPUT_DIR` directory.
-
-**Options:**
-
-  - `-w, --watch` Automatically rebuild the site when templates are modified
-
-staticjinjaplus will first try to set the system's locale to the first working locale identifier set in the `LOCALE`
-[configuration value](#configpy) (if set).
-
-It will then copy the tree contained in the `STATIC_DIR` directory in the `OUTPUT_DIR`, as-is.
-
-staticjinja will be then initialized with the given `CONTEXTS` and Jinja's `GLOBALS`/`FILTERS`/`EXTENSIONS`,
-[webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) will be registered, and the actual rendering
-process is started.
-
-`.html`, `.xml`, `.rss`, `.atom` and `.json` template output will be automatically minified, according to the `MINIFY_XML`
-and `MINIFY_JSON` configuration values.
-
-#### `staticjinjaplus clean`
-
-Delete and recreate the `OUTPUT_DIR` directory.
-
-#### `staticjinjaplus publish`
-
-> [!NOTE]
-> This feature requires a Linux-like environment.
-
-Apply configuration values override from [environment variables](#environment-variables), then successively run
-`staticjinjaplus build` and `staticjinjaplus clean` prior remotely syncing the `OUTPUT_DIR` directory content using
-`rsync` through SSH.
-
-#### `staticjinjaplus serve`
-
-Serve the `OUTPUT_DIR` directory using Python's built-in HTTP server, plus a couple improvements:
-
-  - URL rewrite for HTML files is emulated, i.e. both `/about.html` and `/about` will work
-  - Custom HTTP error pages are emulated, if they are found saved as `{status code}.html` in the output directory
-  - The server will listen to both IPv4 *and* IPv6 loopback addresses if possible
-
-By default, you can browse your generated site at http://localhost:8080/ or http://[::1]:8080/. Port can be changed
-by defining the `SERVE_PORT` [configuration value](#configpy).
-
-## Configuration
-
-### `config.py`
-
-Your project's configuration happens in a single `config.py` file in the root directory (where the `staticjinjaplus`
-CLI should be executed). You'll find the available configuration values below.
-
-> [!NOTE]
->   - All paths are relative to the root directory, unless otherwise stated.
->   - None of these configuration values are required, so is `config.py`.
->   - Only uppercase variables are loaded by staticjinjaplus.
-
-| Name             | Type                                            | Default                          | Description                                                                                                                                                                                                                                                                            |
-|------------------|-------------------------------------------------|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `LOCALE`         | List[str]                                       | `None`                           | Locale identifiers passed to [`locale.setlocale()`](https://docs.python.org/3.12/library/locale.html#locale.setlocale) before a build is executed. The first working identifier will be used                                                                                           |
-| `SERVE_PORT`     | int                                             | `8080`                           | Listening port of the HTTP server started by `staticjinjaplus serve`                                                                                                                                                                                                                   |
-| `BASE_URL`       | str                                             | `http://localhost:{SERVE_PORT}/` | Protocol and domain name to use to generate meaningful absolute URLs. Set host part to `[::1]` if you plan to use IPv6                                                                                                                                                                 |
-| `MINIFY_XML`     | bool                                            | `False`                          | Enable XML minification                                                                                                                                                                                                                                                                |
-| `MINIFY_JSON`    | bool                                            | `False`                          | Enable JSON minification                                                                                                                                                                                                                                                               |
-| `TEMPLATES_DIR`  | str                                             | `templates`                      | Directory containing the Jinja templates to be processed                                                                                                                                                                                                                               |
-| `OUTPUT_DIR`     | str                                             | `output`                         | Directory where the rendered site will be saved                                                                                                                                                                                                                                        |
-| `STATIC_DIR`     | str                                             | `static`                         | Directory containing static files                                                                                                                                                                                                                                                      |
-| `ASSETS_DIR`     | str                                             | `assets`                         | Directory containing assets, i.e. files that needs prior processing before being able to be used by the rendered site                                                                                                                                                                  |
-| `ASSETS_BUNDLES` | List[Tuple[str, Tuple[str,...], Dict[str, str]] | `[]`                             | [webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) to be registered. These are passed to [`register()`](https://webassets.readthedocs.io/en/latest/environment.html#registering-bundles). Sources are relative to `ASSETS_DIR`, destinations to `OUTPUT_DIR` |
-| `CONTEXTS`       | List[Tuple[str, Any]]                           | `[]`                             | [staticjinja contexts](https://staticjinja.readthedocs.io/en/stable/user/advanced.html#loading-data) to be used by templates                                                                                                                                                           |
-| `GLOBALS`        | Dict                                            | `{}`                             | [jinja globals](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.globals) to be made available in all templates                                                                                                                                                      |
-| `FILTERS`        | Dict                                            | `{}`                             | [jinja filters](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.filters) to be made available in all templates                                                                                                                                                      |
-| `EXTENSIONS`     | List[Union[str, jinja2.ext.Extension]]          | `[]`                             | [jinja extensions](https://jinja.palletsprojects.com/en/3.1.x/extensions/) to load                                                                                                                                                                                                     |
-
-### Environment variables
-
-Some configuration values may/must be overridden by environment variables of the same name when publishing your site
-(`staticjinjaplus publish` command), typically in a deployment environment. You'll find the list below.
-
-| Name          | Type   | Required?                      | Default                           | Description                                                          |
-|---------------|--------|--------------------------------|-----------------------------------|----------------------------------------------------------------------|
-| `BASE_URL`    | str    | Yes                            |                                   | Protocol and domain name to use to generate meaningful absolute URLs |
-| `MINIFY_XML`  | bool ¹ | No, but activation recommended | `MINIFY_XML` configuration value  | Enable XML minification                                              |
-| `MINIFY_JSON` | bool ¹ | No, but activation recommended | `MINIFY_JSON` configuration value | Enable JSON minification                                             |
-| `SSH_USER`    | str    | Yes                            |                                   | SSH username                                                         |
-| `SSH_HOST`    | str    | Yes                            |                                   | SSH hostname                                                         |
-| `SSH_PORT`    | int    | No                             | `22`                              | SSH port                                                             |
-| `SSH_PATH`    | str    | Yes                            |                                   | Absolute path to the deployment directory on the SSH host            |
-
-¹ Any [falsy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.falsy) or
-[truthy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.truthy) string
-representation of boolean values allowed by marshmallow
-
-## Development
-
-### Getting source code and installing the package with dev dependencies
-
-  1. Clone the repository
-  2. From the root directory, run: `pip install -e .[dev]` on Linux or `pip install -e ".[dev]"` on Windows
-
-### Releasing the package
-
-From the root directory, run `python setup.py upload`. This will build the package, create a git tag and publish on PyPI.
-
-`__version__` in `staticjinjaplus/__version__.py` must be updated beforehand. It should adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-
-An associated GitHub release must be created following the [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format.
+# staticjinjaplus
+
+A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
+
+![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
+
+[PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
+
+Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
+I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
+order to be able to generate a static website that will actually be ready for real world usage.
+
+staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
+Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
+static site generator.
+
+## Features
+
+All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
+
+  - Simple, file-based configuration to centralize *a handful* of configuration values
+  - Generic Markdown support (**not** your usual "pages" or "articles/blog posts" feature)
+  - Build improvements
+    - Automatically copy static files to output directory
+    - Define Jinja and staticjinja initialization parameters in a config file
+    - Define [webassets](https://webassets.readthedocs.io/en/latest/) bundles to allow CSS/JS concatenation/minification
+    - Automatically minify XML (including HTML, RSS and Atom)/JSON output
+  - Jinja improvements
+    - A few new Jinja globals/filters to make your life easier
+    - Autoescape is enabled for XML, HTML, RSS and Atom templates
+  - Serve the generated site through a local HTTP server
+    - URL rewrite emulation (for HTML files)
+    - Custom HTTP error pages emulation
+    - IPv6 loopback address support
+    - Serve proper MIME type for RSS and Atom files
+  - Publish the generated site through rsync over SSH
+
+**Planned:**
+
+  - Rebuild site on assets/static files change
+  - Generic i18n and l10n support (powered by Babel)
+
+## Prerequisites
+
+  - Python >= 3.10
+
+## Installation
+
+From PyPI:
+
+```bash
+$ pip install staticjinjaplus
+```
+
+Locally, after cloning/downloading the repo:
+
+```bash
+$ pip install .
+```
+
+A CLI (`staticjinjaplus`) will be made available upon installation.
+
+## Usage
+
+### Templates
+
+You'll want to write your site's Jinja templates first: write them as usual. By default, staticjinjaplus searches for
+Jinja templates in the `templates` directory where it is invoked. You can change that by using the `TEMPLATES_DIR`
+[configuration value](#configpy).
+
+Remember staticjinjaplus still stick with staticjinja's idiom: one Jinja template equal one rendered file, nothing more,
+nothing less.
+
+> [!WARNING]
+> HTML templates which extension is not `.html` will **not** be properly handled by staticjinjaplus for the sake of
+> simplicity. Please use `.html` only.
+
+staticjinjaplus offers the following additional Jinja facilities.
+
+#### Globals
+
+| Name/signature                              | Type                 | Description                                                                                                                                                                                                                         |
+|---------------------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `config`                                    | Dict[str, Any]       | Configuration values loaded from [`config.py`](#configpy) (defaults are guaranteed to be provided for built-in values). Only uppercase variables are loaded by staticjinjaplus                                                      |
+| `absurl(resource: str) -> str`              | Callable             | Build an absolute URL relative to a file located in the `OUTPUT_DIR` directory. The resource path is prefixed by `BASE_URL` (see [configuration values](#configpy))                                                                 |
+| `embed(filename: str) -> markupsafe.Markup` | Callable             | Return the file content of the given file, marked as safe to be rendered by Jinja. `filename` is relative to the `{ASSETS_DIR}` directory. Useful to e.g embed SVG icons directly in the generated HTML                             |
+| `collected`                                 | List[Dict[str, Any]] | List of all valid template files (as seen by staticjinja) found in the `TEMPLATES_DIR` directory. Dictionary include source filename, rendered template URL, file extension, and for Markdown (`.md`) files their parsed metadata. |
+
+**Usage examples:**
+
+```html+jinja
+{{ config.BASE_URL }}         {# http://localhost:8080/ (by default) #}
+{{ config.MY_CUSTOM_CONFIG }} {# Whatever you defined in your config.py (uppercase variables only) #}
+
+{# absurl() doesn't care whether an extension is given or not #}
+{{ absurl('/about.html') }} {# http://localhost:8080/about.html #}
+{{ absurl('/about') }}      {# http://localhost:8080/about #}
+{{ absurl('about') }}       {# http://localhost:8080/about #}
+
+{# absurl() doesn't care about whether a static file is targeted or not #}
+{{ absurl('/images/logo.png') }} {# http://localhost:8080/images/logo.png #}
+{{ absurl('images/logo.png') }}  {# http://localhost:8080/images/logo.png #}
+
+{{ embed('icons/github.svg') }} {# <svg xmlns="http://www.w3.org/2000/svg" ... </svg> #}
+
+{{ collected }}
+{#
+    [
+      {'source': 'index.html', 'type': 'html', url': '/'},
+      {'source': 'site/about.html', 'type': 'html', 'url': '/site/about.html'},
+      {'source': 'categories/index.html', 'type': 'html', 'url': '/categories/'},
+      {'source': 'woah.md', 'type': 'md', 'url': '/woah.html', 'meta': { ... }},
+      {'source': 'index.md', 'type': 'md', 'url': '/', 'meta': { ... }},
+      {'source': 'blog/an-article.md', 'type': 'md', 'url': '/blog/an-article.html', 'meta': { ... }},
+      {'source': 'blog/index.md', 'type': 'md', 'url': '/blog/', 'meta': { ... }}
+    ]
+#}
+```
+
+#### Filters
+
+| Signature                                      | Description                                                                                                                                                                                                                                                         |
+|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `<data: Dict>\|tojsonm -> markupsafe.Markup`   | Serialize the given dictionary to a JSON string. Automatically takes into account the `MINIFY_JSON` [configuration value](#configpy) to minify (or not) the resulting output. Useful for e.g serializing [Schema.org](https://schema.org/)'s JSON-LD-formatted data |
+| `<left: Dict>\|dictmerge(right: Dict) -> Dict` | Merge two dictionaries. Does not modify existing ones, a new one will be created. Does **not** merge deeply                                                                                                                                                         |
+
+**Usage examples:**
+
+```html+jinja
+{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == False:
+                                 {
+                                     "yes": true
+                                 }
+                             #}
+
+{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == True:
+                                 {"yes":true}
+                             #}
+
+{{ dict(yes=True)|dictmerge(dict(no=False)) }} {# {"yes": True, "no": False} #}
+```
+
+#### Markdown
+
+> [!WARNING]
+> Markdown templates which extension is not `.md` will **not** be properly handled by staticjinjaplus for the sake of
+> simplicity. Please use `.md` only.
+
+staticjinjaplus has generic support for working with Markdown-formatted files. Write your Markdown files (`.md`) as usual
+in the `TEMPLATES_DIR` directory: they will be rendered to HTML using the appropriate template partial, and saved using
+the source root pathname to the `OUTPUT_DIR` directory; i.e. `{TEMPLATES_DIR}/blog/awesome.md` will be rendered to
+`{OUTPUT_DIR}/blog/awesome.html`.
+
+staticjinjaplus do read metadata fields of Markdown files. Supported syntax is documented [here](https://python-markdown.github.io/extensions/meta_data/#syntax).
+The only reserved metadata field is `partial`, which tells staticjinjaplus which template partial (relative to the
+`TEMPLATES_DIR` directory) to use when rendering the Markdown file. See example below.
+
+It fallbacks to the `MARKDOWN_DEFAULT_PARTIAL` [configuration value](#configpy) if the field was not found. An error will
+be logged if staticjinjaplus can't determine which template partial to use, and rendering of the Markdown file will be
+canceled.
+
+This template partial will be given a Markdown-specific variable named `markdown` containing a dictionary which keys and
+values are detailed below.
+
+| Name                 | Type              | Description                                                                                                            |
+|----------------------|-------------------|------------------------------------------------------------------------------------------------------------------------|
+| `markdown.converted` | markupsafe.Markup | The resulting HTML, marked as safe to be rendered by Jinja. Metadata are of course not included in this output         |
+| `markdown.source`    | str               | The Markdown template filename                                                                                         |
+| `markdown.url`       | str               | The rendered Markdown template URL                                                                                     |
+| `markdown.meta`      | Dict[str, str]    | Metadata parsed from the source Markdown file. Multiline values have been concatenated using `\n` without extra spaces |
+
+Internal URLs must be written using the rendered version of the templates/assets/static files, i.e. URLs relative to what
+will be rendered in the `OUTPUT_DIR` directory. staticjinjaplus will not rewrite any URLs in any manner: you must provide
+the right ones by yourself. See example below.
+
+See also the `collected` [Jinja global](#globals) which contain - among others - all Markdown files found in the
+`TEMPLATES_DIR` directory (as seen by staticjinja) along their parsed metadata, and more.
+
+**Example Markdown file:**
+
+```markdown
+partial: blog/_post.html
+
+My awesome blog post. It has internal [links](/blog/my-article.html), and one image:
+
+![](/images/attachment.png)
+
+This image may come from the `STATIC_DIR` directory.
+```
+
+### Command line interface
+
+The `staticjinjaplus` CLI is your main and only way to interact with staticjinjaplus. The following commands are available.
+
+#### `staticjinjaplus build`
+
+Build the site by rendering your templates from the `TEMPLATES_DIR` directory in the `OUTPUT_DIR` directory.
+
+**Options:**
+
+  - `-w, --watch` Automatically rebuild the site when templates are modified. **This option does not watch for assets or static files changes (yet?)**
+
+It will then copy the tree contained in the `STATIC_DIR` directory in the `OUTPUT_DIR`, as-is.
+
+staticjinja will be then initialized with the given `CONTEXTS` and Jinja's `JINJA_GLOBALS`/`JINJA_FILTERS`/`JINJA_EXTENSIONS`,
+[webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) (`WEBASSETS_BUNDLES`) will be registered, and
+the actual rendering process is started.
+
+`.html`, `.xml`, `.rss`, `.atom` and `.json` template output will be automatically minified, according to the `MINIFY_XML`
+and `MINIFY_JSON` configuration values. `.md` files will be converted to HTML and rendered using the appropriate template
+partial, which output will be automatically minified as well if configured so.
+
+#### `staticjinjaplus clean`
+
+Delete and recreate the `OUTPUT_DIR` directory.
+
+#### `staticjinjaplus publish`
+
+> [!NOTE]
+> This feature requires a Linux-like environment.
+
+Apply configuration values override from [environment variables](#environment-variables), then successively run
+`staticjinjaplus clean` and `staticjinjaplus build` prior remotely syncing the `OUTPUT_DIR` directory content using
+`rsync` through SSH.
+
+#### `staticjinjaplus serve`
+
+Serve the `OUTPUT_DIR` directory using Python's built-in HTTP server, plus a couple improvements:
+
+  - URL rewrite for HTML files is emulated, i.e. both `/about.html` and `/about` will work
+  - Custom HTTP error pages are emulated, if they are found saved as `{status code}.html` in the output directory
+  - The server will listen to both IPv4 *and* IPv6 loopback addresses if possible
+  - RSS and Atom files will be served using the appropriate MIME type in the `Content-Type` response header
+
+By default, you can browse your generated site at http://localhost:8080/ or [http://[::1]:8080/](http://[::1]:8080/).
+Port can be changed by defining the `SERVE_PORT` [configuration value](#configpy).
+
+## Configuration
+
+### `config.py`
+
+Your project's configuration happens in a single `config.py` file in the root directory (where the `staticjinjaplus`
+CLI should be executed). You'll find the available configuration values below.
+
+> [!NOTE]
+>   - All paths are relative to the root directory, unless otherwise stated.
+>   - None of these configuration values are required, so is `config.py`.
+>   - Only uppercase variables are loaded by staticjinjaplus.
+
+| Name                       | Type                                              | Default                          | Description                                                                                                                                                                                                                                                                                                                           |
+|----------------------------|---------------------------------------------------|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `SERVE_PORT`               | int                                               | `8080`                           | Listening port of the HTTP server started by `staticjinjaplus serve`                                                                                                                                                                                                                                                                  |
+| `BASE_URL`                 | str                                               | `http://localhost:{SERVE_PORT}/` | Protocol and domain name to use to generate meaningful absolute URLs. Set host part to `[::1]` if you plan to use IPv6                                                                                                                                                                                                                |
+| `MINIFY_XML`               | bool                                              | `False`                          | Enable XML minification                                                                                                                                                                                                                                                                                                               |
+| `MINIFY_JSON`              | bool                                              | `False`                          | Enable JSON minification                                                                                                                                                                                                                                                                                                              |
+| `TEMPLATES_DIR`            | str                                               | `templates`                      | Directory containing the Jinja templates to be processed                                                                                                                                                                                                                                                                              |
+| `OUTPUT_DIR`               | str                                               | `output`                         | Directory where the rendered site will be saved                                                                                                                                                                                                                                                                                       |
+| `STATIC_DIR`               | str                                               | `static`                         | Directory containing static files                                                                                                                                                                                                                                                                                                     |
+| `ASSETS_DIR`               | str                                               | `assets`                         | Directory containing assets, i.e. files that needs prior processing before being able to be used by the rendered site                                                                                                                                                                                                                 |
+| `CONTEXTS`                 | List[Tuple[str, Union[Dict[str, Any], Callable]]] | `[]`                             | [staticjinja contexts](https://staticjinja.readthedocs.io/en/stable/user/advanced.html#loading-data) to be used by templates                                                                                                                                                                                                          |
+| `WEBASSETS_BUNDLES`        | List[Tuple[str, Tuple[str,...], Dict[str, str]]   | `[]`                             | [webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) to be registered. These are passed to [`register()`](https://webassets.readthedocs.io/en/latest/environment.html#registering-bundles). Sources are relative to `ASSETS_DIR`, destinations to `OUTPUT_DIR`                                                |
+| `JINJA_GLOBALS`            | Dict[str, Any]                                    | `{}`                             | [jinja globals](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.globals) to be made available in all templates                                                                                                                                                                                                     |
+| `JINJA_FILTERS`            | Dict[str, Callable]                               | `{}`                             | [jinja filters](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.filters) to be made available in all templates                                                                                                                                                                                                     |
+| `JINJA_EXTENSIONS`         | List[Union[str, jinja2.ext.Extension]]            | `[]`                             | [jinja extensions](https://jinja.palletsprojects.com/en/3.1.x/extensions/) to load                                                                                                                                                                                                                                                    |
+| `MARKDOWN_EXTENSIONS`      | Dict[str, Dict]                                   | `{}`                             | [Markdown extensions](https://python-markdown.github.io/extensions/) to load and their respective configuration. Keys are passed to [`extensions`](https://python-markdown.github.io/reference/#extensions); the entire dictionary is passed to [`extension_configs`](https://python-markdown.github.io/reference/#extension_configs) |
+| `MARKDOWN_DEFAULT_PARTIAL` | Optional[str]                                     | `None`                           | Default template partial to use when rendering Markdown files when the `partial` metadata is not present                                                                                                                                                                                                                              |
+| `USE_HTML_EXTENSION`       | bool                                              | `True`                           | If your site's links are using URLs without `.html` extension (URL rewrite), you must set this config value to `False`. This config value does **not** alter the behavior of `absurl()` in any way                                                                                                                                    |
+
+### Environment variables
+
+Some configuration values may/must be overridden by environment variables of the same name when publishing your site
+(`staticjinjaplus publish` command), typically in a deployment environment. You'll find the list below.
+
+| Name          | Type   | Required?                      | Default                           | Description                                                          |
+|---------------|--------|--------------------------------|-----------------------------------|----------------------------------------------------------------------|
+| `BASE_URL`    | str    | Yes                            |                                   | Protocol and domain name to use to generate meaningful absolute URLs |
+| `MINIFY_XML`  | bool ¹ | No, but activation recommended | `MINIFY_XML` configuration value  | Enable XML minification                                              |
+| `MINIFY_JSON` | bool ¹ | No, but activation recommended | `MINIFY_JSON` configuration value | Enable JSON minification                                             |
+| `SSH_USER`    | str    | Yes                            |                                   | SSH username                                                         |
+| `SSH_HOST`    | str    | Yes                            |                                   | SSH hostname                                                         |
+| `SSH_PORT`    | int    | No                             | `22`                              | SSH port                                                             |
+| `SSH_PATH`    | str    | Yes                            |                                   | Absolute path to the deployment directory on the SSH host            |
+
+¹ Any [falsy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.falsy) or
+[truthy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.truthy) string
+representation of boolean values allowed by marshmallow
+
+## Development
+
+### Getting source code and installing the package with dev dependencies
+
+  1. Clone the repository
+  2. From the root directory, run: `pip install -e .[dev]` on Linux or `pip install -e ".[dev]"` on Windows
+
+### Releasing the package
+
+From the root directory, run `python setup.py upload`. This will build the package, create a git tag and publish on PyPI.
+
+`__version__` in `staticjinjaplus/__version__.py` must be updated beforehand. It should adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+An associated GitHub release must be created following the [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format.
```

### Comparing `staticjinjaplus-1.1.2/README.md` & `staticjinjaplus-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,233 +1,342 @@
-# staticjinjaplus
-
-A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
-
-![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
-
-[PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
-
-Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
-I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
-order to be able to generate a static website that will actually be ready for real world usage.
-
-staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
-Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
-static site generator.
-
-## Features
-
-All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
-
-  - Simple, file-based configuration to centralize *a handful* of configuration values
-  - Build improvements
-    - Set system locale before building anything (useful when formatting dates to localized strings)
-    - Automatically copy static files to output directory
-    - Define staticjinja contexts in config file
-    - Define [webassets](https://webassets.readthedocs.io/en/latest/) bundles to allow CSS/JS concatenation/minification
-    - Automatically minify XML (including HTML, RSS and Atom)/JSON output
-  - Jinja improvements
-    - A few new Jinja globals/filters to make your life easier
-    - Autoescape is enabled for XML, HTML, RSS and Atom templates
-  - Serve the generated site through a local HTTP server
-    - URL rewrite emulation (for HTML files)
-    - Custom HTTP error pages emulation
-    - IPv6 loopback address support
-  - Publish the generated site through rsync over SSH
-
-**Planned:**
-
-  - Generic support of Markdown-formatted templates collections (forget about the usual "pages" or "articles/blog posts" feature)
-
-## Prerequisites
-
-  - Python >= 3.9
-
-## Installation
-
-From PyPI:
-
-```bash
-$ pip install staticjinjaplus
-```
-
-Locally, after cloning/downloading the repo:
-
-```bash
-$ pip install .
-```
-
-A CLI (`staticjinjaplus`) will be made available upon installation.
-
-## Usage
-
-### Templates
-
-You'll want to write your site's Jinja templates first: write them as usual. By default, staticjinjaplus searches for
-Jinja templates in the `templates` directory where it is invoked. You can change that by using the `TEMPLATES_DIR`
-[configuration value](#configpy).
-
-staticjinjaplus offers the following additional Jinja facilities.
-
-#### Globals
-
-| Name/signature                                  | Type     | Description                                                                                                                                                                                                         |
-|-------------------------------------------------|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `config`                                        | Dict     | Configuration values loaded from [`config.py`](#configpy) (defaults are guaranteed to be provided for built-in values). Only uppercase variables are loaded by staticjinjaplus                                      |
-| `url(path: str, absolute: bool = False) -> str` | Callable | Build (by default) a relative URL to a file located in the `OUTPUT_DIR` directory. Setting `absolute` to `True` prefixes the URL with `BASE_URL`. See [configuration values](#configpy)                             |
-| `icon(name: str) -> markupsafe.Markup`          | Callable | Return the file content of the given SVG icon, marked as safe to be rendered by Jinja. Icons must be saved in the form of `{ASSETS_DIR}/icons/{name}.svg`. Useful to embed SVG icons directly in the generated HTML |
-
-**Usage examples:**
-
-```html+jinja
-{{ config.BASE_URL }}         {# http://localhost:8080/ (by default) #}
-{{ config.MY_CUSTOM_CONFIG }} {# Whatever you defined in your config.py (uppercase variables only) #}
-
-{# url() doesn't care whether an extension is given or not #}
-{{ url('/about.html') }} {# /about.html #}
-{{ url('/about') }}      {# /about #}
-{{ url('about') }}       {# /about #}
-
-{# url() doesn't care about whether a static file is targeted or not #}
-{{ url('/images/logo.png') }} {# /images/logo.png #}
-{{ url('images/logo.png') }}  {# /images/logo.png #}
-
-{# URL is simply prefixed with BASE_URL when generating absolute URLs #}
-{{ url('/images/logo.png', absolute=True) }} {# http://localhost:8080/images/logo.png (by default) #}
-{{ url('images/logo.png', absolute=True) }}  {# http://localhost:8080/images/logo.png (by default) #}
-
-{{ icon('github') }} {# <svg xmlns="http://www.w3.org/2000/svg" ... </svg> #}
-```
-
-#### Filters
-
-| Signature                                      | Description                                                                                                                                                                                                                                                         |
-|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `<data: Dict>\|tojsonm -> str`                 | Serialize the given dictionary to a JSON string. Automatically takes into account the `MINIFY_JSON` [configuration value](#configpy) to minify (or not) the resulting output. Useful for e.g serializing [Schema.org](https://schema.org/)'s JSON-LD-formatted data |
-| `<left: Dict>\|dictmerge(right: Dict) -> Dict` | Merge two dictionaries. Does not modify existing ones, a new one will be created. Does **not** merge deeply                                                                                                                                                         |
-
-**Usage examples:**
-
-```html+jinja
-{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == False:
-                                 {
-                                     "yes": true
-                                 }
-                             #}
-
-{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == True:
-                                 {"yes":true}
-                             #}
-
-{{ dict(yes=True)|dictmerge(dict(no=False)) }} {# {"yes": True, "no": False} #}
-```
-
-### Command line interface
-
-The `staticjinjaplus` CLI is your main and only way to interact with staticjinjaplus. The following commands are available.
-
-#### `staticjinjaplus build`
-
-Build the site by rendering your templates from the `TEMPLATES_DIR` directory in the `OUTPUT_DIR` directory.
-
-**Options:**
-
-  - `-w, --watch` Automatically rebuild the site when templates are modified
-
-staticjinjaplus will first try to set the system's locale to the first working locale identifier set in the `LOCALE`
-[configuration value](#configpy) (if set).
-
-It will then copy the tree contained in the `STATIC_DIR` directory in the `OUTPUT_DIR`, as-is.
-
-staticjinja will be then initialized with the given `CONTEXTS` and Jinja's `GLOBALS`/`FILTERS`/`EXTENSIONS`,
-[webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) will be registered, and the actual rendering
-process is started.
-
-`.html`, `.xml`, `.rss`, `.atom` and `.json` template output will be automatically minified, according to the `MINIFY_XML`
-and `MINIFY_JSON` configuration values.
-
-#### `staticjinjaplus clean`
-
-Delete and recreate the `OUTPUT_DIR` directory.
-
-#### `staticjinjaplus publish`
-
-> [!NOTE]
-> This feature requires a Linux-like environment.
-
-Apply configuration values override from [environment variables](#environment-variables), then successively run
-`staticjinjaplus build` and `staticjinjaplus clean` prior remotely syncing the `OUTPUT_DIR` directory content using
-`rsync` through SSH.
-
-#### `staticjinjaplus serve`
-
-Serve the `OUTPUT_DIR` directory using Python's built-in HTTP server, plus a couple improvements:
-
-  - URL rewrite for HTML files is emulated, i.e. both `/about.html` and `/about` will work
-  - Custom HTTP error pages are emulated, if they are found saved as `{status code}.html` in the output directory
-  - The server will listen to both IPv4 *and* IPv6 loopback addresses if possible
-
-By default, you can browse your generated site at http://localhost:8080/ or http://[::1]:8080/. Port can be changed
-by defining the `SERVE_PORT` [configuration value](#configpy).
-
-## Configuration
-
-### `config.py`
-
-Your project's configuration happens in a single `config.py` file in the root directory (where the `staticjinjaplus`
-CLI should be executed). You'll find the available configuration values below.
-
-> [!NOTE]
->   - All paths are relative to the root directory, unless otherwise stated.
->   - None of these configuration values are required, so is `config.py`.
->   - Only uppercase variables are loaded by staticjinjaplus.
-
-| Name             | Type                                            | Default                          | Description                                                                                                                                                                                                                                                                            |
-|------------------|-------------------------------------------------|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `LOCALE`         | List[str]                                       | `None`                           | Locale identifiers passed to [`locale.setlocale()`](https://docs.python.org/3.12/library/locale.html#locale.setlocale) before a build is executed. The first working identifier will be used                                                                                           |
-| `SERVE_PORT`     | int                                             | `8080`                           | Listening port of the HTTP server started by `staticjinjaplus serve`                                                                                                                                                                                                                   |
-| `BASE_URL`       | str                                             | `http://localhost:{SERVE_PORT}/` | Protocol and domain name to use to generate meaningful absolute URLs. Set host part to `[::1]` if you plan to use IPv6                                                                                                                                                                 |
-| `MINIFY_XML`     | bool                                            | `False`                          | Enable XML minification                                                                                                                                                                                                                                                                |
-| `MINIFY_JSON`    | bool                                            | `False`                          | Enable JSON minification                                                                                                                                                                                                                                                               |
-| `TEMPLATES_DIR`  | str                                             | `templates`                      | Directory containing the Jinja templates to be processed                                                                                                                                                                                                                               |
-| `OUTPUT_DIR`     | str                                             | `output`                         | Directory where the rendered site will be saved                                                                                                                                                                                                                                        |
-| `STATIC_DIR`     | str                                             | `static`                         | Directory containing static files                                                                                                                                                                                                                                                      |
-| `ASSETS_DIR`     | str                                             | `assets`                         | Directory containing assets, i.e. files that needs prior processing before being able to be used by the rendered site                                                                                                                                                                  |
-| `ASSETS_BUNDLES` | List[Tuple[str, Tuple[str,...], Dict[str, str]] | `[]`                             | [webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) to be registered. These are passed to [`register()`](https://webassets.readthedocs.io/en/latest/environment.html#registering-bundles). Sources are relative to `ASSETS_DIR`, destinations to `OUTPUT_DIR` |
-| `CONTEXTS`       | List[Tuple[str, Any]]                           | `[]`                             | [staticjinja contexts](https://staticjinja.readthedocs.io/en/stable/user/advanced.html#loading-data) to be used by templates                                                                                                                                                           |
-| `GLOBALS`        | Dict                                            | `{}`                             | [jinja globals](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.globals) to be made available in all templates                                                                                                                                                      |
-| `FILTERS`        | Dict                                            | `{}`                             | [jinja filters](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.filters) to be made available in all templates                                                                                                                                                      |
-| `EXTENSIONS`     | List[Union[str, jinja2.ext.Extension]]          | `[]`                             | [jinja extensions](https://jinja.palletsprojects.com/en/3.1.x/extensions/) to load                                                                                                                                                                                                     |
-
-### Environment variables
-
-Some configuration values may/must be overridden by environment variables of the same name when publishing your site
-(`staticjinjaplus publish` command), typically in a deployment environment. You'll find the list below.
-
-| Name          | Type   | Required?                      | Default                           | Description                                                          |
-|---------------|--------|--------------------------------|-----------------------------------|----------------------------------------------------------------------|
-| `BASE_URL`    | str    | Yes                            |                                   | Protocol and domain name to use to generate meaningful absolute URLs |
-| `MINIFY_XML`  | bool ¹ | No, but activation recommended | `MINIFY_XML` configuration value  | Enable XML minification                                              |
-| `MINIFY_JSON` | bool ¹ | No, but activation recommended | `MINIFY_JSON` configuration value | Enable JSON minification                                             |
-| `SSH_USER`    | str    | Yes                            |                                   | SSH username                                                         |
-| `SSH_HOST`    | str    | Yes                            |                                   | SSH hostname                                                         |
-| `SSH_PORT`    | int    | No                             | `22`                              | SSH port                                                             |
-| `SSH_PATH`    | str    | Yes                            |                                   | Absolute path to the deployment directory on the SSH host            |
-
-¹ Any [falsy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.falsy) or
-[truthy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.truthy) string
-representation of boolean values allowed by marshmallow
-
-## Development
-
-### Getting source code and installing the package with dev dependencies
-
-  1. Clone the repository
-  2. From the root directory, run: `pip install -e .[dev]` on Linux or `pip install -e ".[dev]"` on Windows
-
-### Releasing the package
-
-From the root directory, run `python setup.py upload`. This will build the package, create a git tag and publish on PyPI.
-
-`__version__` in `staticjinjaplus/__version__.py` must be updated beforehand. It should adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-
-An associated GitHub release must be created following the [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format.
+Metadata-Version: 2.1
+Name: staticjinjaplus
+Version: 2.0.0
+Summary: A sweet spot between staticjinja and a full-blown static site generator.
+Home-page: https://github.com/EpocDotFr/staticjinjaplus
+Author: Maxime "Epoc" Gross
+Author-email: contact.nospam@epoc.nospam.fr
+License: DBAD
+Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme
+Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
+Project-URL: Tracker, https://github.com/EpocDotFr/staticjinjaplus/issues
+Project-URL: Changelog, https://github.com/EpocDotFr/staticjinjaplus/releases
+Keywords: static,website,site,generator,staticjinja,jinja,jinja2
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: staticjinja~=5.0
+Requires-Dist: webassets~=2.0
+Requires-Dist: htmlmin~=0.1
+Requires-Dist: cssutils~=2.10
+Requires-Dist: jsmin~=3.0
+Requires-Dist: environs~=11.0
+Requires-Dist: markdown~=3.6
+Provides-Extra: dev
+Requires-Dist: build~=1.2; extra == "dev"
+Requires-Dist: twine~=5.0; extra == "dev"
+Requires-Dist: setuptools~=69.5; extra == "dev"
+
+
+# staticjinjaplus
+
+A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
+
+![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
+
+[PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
+
+Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
+I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
+order to be able to generate a static website that will actually be ready for real world usage.
+
+staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
+Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
+static site generator.
+
+## Features
+
+All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
+
+  - Simple, file-based configuration to centralize *a handful* of configuration values
+  - Generic Markdown support (**not** your usual "pages" or "articles/blog posts" feature)
+  - Build improvements
+    - Automatically copy static files to output directory
+    - Define Jinja and staticjinja initialization parameters in a config file
+    - Define [webassets](https://webassets.readthedocs.io/en/latest/) bundles to allow CSS/JS concatenation/minification
+    - Automatically minify XML (including HTML, RSS and Atom)/JSON output
+  - Jinja improvements
+    - A few new Jinja globals/filters to make your life easier
+    - Autoescape is enabled for XML, HTML, RSS and Atom templates
+  - Serve the generated site through a local HTTP server
+    - URL rewrite emulation (for HTML files)
+    - Custom HTTP error pages emulation
+    - IPv6 loopback address support
+    - Serve proper MIME type for RSS and Atom files
+  - Publish the generated site through rsync over SSH
+
+**Planned:**
+
+  - Rebuild site on assets/static files change
+  - Generic i18n and l10n support (powered by Babel)
+
+## Prerequisites
+
+  - Python >= 3.10
+
+## Installation
+
+From PyPI:
+
+```bash
+$ pip install staticjinjaplus
+```
+
+Locally, after cloning/downloading the repo:
+
+```bash
+$ pip install .
+```
+
+A CLI (`staticjinjaplus`) will be made available upon installation.
+
+## Usage
+
+### Templates
+
+You'll want to write your site's Jinja templates first: write them as usual. By default, staticjinjaplus searches for
+Jinja templates in the `templates` directory where it is invoked. You can change that by using the `TEMPLATES_DIR`
+[configuration value](#configpy).
+
+Remember staticjinjaplus still stick with staticjinja's idiom: one Jinja template equal one rendered file, nothing more,
+nothing less.
+
+> [!WARNING]
+> HTML templates which extension is not `.html` will **not** be properly handled by staticjinjaplus for the sake of
+> simplicity. Please use `.html` only.
+
+staticjinjaplus offers the following additional Jinja facilities.
+
+#### Globals
+
+| Name/signature                              | Type                 | Description                                                                                                                                                                                                                         |
+|---------------------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `config`                                    | Dict[str, Any]       | Configuration values loaded from [`config.py`](#configpy) (defaults are guaranteed to be provided for built-in values). Only uppercase variables are loaded by staticjinjaplus                                                      |
+| `absurl(resource: str) -> str`              | Callable             | Build an absolute URL relative to a file located in the `OUTPUT_DIR` directory. The resource path is prefixed by `BASE_URL` (see [configuration values](#configpy))                                                                 |
+| `embed(filename: str) -> markupsafe.Markup` | Callable             | Return the file content of the given file, marked as safe to be rendered by Jinja. `filename` is relative to the `{ASSETS_DIR}` directory. Useful to e.g embed SVG icons directly in the generated HTML                             |
+| `collected`                                 | List[Dict[str, Any]] | List of all valid template files (as seen by staticjinja) found in the `TEMPLATES_DIR` directory. Dictionary include source filename, rendered template URL, file extension, and for Markdown (`.md`) files their parsed metadata. |
+
+**Usage examples:**
+
+```html+jinja
+{{ config.BASE_URL }}         {# http://localhost:8080/ (by default) #}
+{{ config.MY_CUSTOM_CONFIG }} {# Whatever you defined in your config.py (uppercase variables only) #}
+
+{# absurl() doesn't care whether an extension is given or not #}
+{{ absurl('/about.html') }} {# http://localhost:8080/about.html #}
+{{ absurl('/about') }}      {# http://localhost:8080/about #}
+{{ absurl('about') }}       {# http://localhost:8080/about #}
+
+{# absurl() doesn't care about whether a static file is targeted or not #}
+{{ absurl('/images/logo.png') }} {# http://localhost:8080/images/logo.png #}
+{{ absurl('images/logo.png') }}  {# http://localhost:8080/images/logo.png #}
+
+{{ embed('icons/github.svg') }} {# <svg xmlns="http://www.w3.org/2000/svg" ... </svg> #}
+
+{{ collected }}
+{#
+    [
+      {'source': 'index.html', 'type': 'html', url': '/'},
+      {'source': 'site/about.html', 'type': 'html', 'url': '/site/about.html'},
+      {'source': 'categories/index.html', 'type': 'html', 'url': '/categories/'},
+      {'source': 'woah.md', 'type': 'md', 'url': '/woah.html', 'meta': { ... }},
+      {'source': 'index.md', 'type': 'md', 'url': '/', 'meta': { ... }},
+      {'source': 'blog/an-article.md', 'type': 'md', 'url': '/blog/an-article.html', 'meta': { ... }},
+      {'source': 'blog/index.md', 'type': 'md', 'url': '/blog/', 'meta': { ... }}
+    ]
+#}
+```
+
+#### Filters
+
+| Signature                                      | Description                                                                                                                                                                                                                                                         |
+|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `<data: Dict>\|tojsonm -> markupsafe.Markup`   | Serialize the given dictionary to a JSON string. Automatically takes into account the `MINIFY_JSON` [configuration value](#configpy) to minify (or not) the resulting output. Useful for e.g serializing [Schema.org](https://schema.org/)'s JSON-LD-formatted data |
+| `<left: Dict>\|dictmerge(right: Dict) -> Dict` | Merge two dictionaries. Does not modify existing ones, a new one will be created. Does **not** merge deeply                                                                                                                                                         |
+
+**Usage examples:**
+
+```html+jinja
+{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == False:
+                                 {
+                                     "yes": true
+                                 }
+                             #}
+
+{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == True:
+                                 {"yes":true}
+                             #}
+
+{{ dict(yes=True)|dictmerge(dict(no=False)) }} {# {"yes": True, "no": False} #}
+```
+
+#### Markdown
+
+> [!WARNING]
+> Markdown templates which extension is not `.md` will **not** be properly handled by staticjinjaplus for the sake of
+> simplicity. Please use `.md` only.
+
+staticjinjaplus has generic support for working with Markdown-formatted files. Write your Markdown files (`.md`) as usual
+in the `TEMPLATES_DIR` directory: they will be rendered to HTML using the appropriate template partial, and saved using
+the source root pathname to the `OUTPUT_DIR` directory; i.e. `{TEMPLATES_DIR}/blog/awesome.md` will be rendered to
+`{OUTPUT_DIR}/blog/awesome.html`.
+
+staticjinjaplus do read metadata fields of Markdown files. Supported syntax is documented [here](https://python-markdown.github.io/extensions/meta_data/#syntax).
+The only reserved metadata field is `partial`, which tells staticjinjaplus which template partial (relative to the
+`TEMPLATES_DIR` directory) to use when rendering the Markdown file. See example below.
+
+It fallbacks to the `MARKDOWN_DEFAULT_PARTIAL` [configuration value](#configpy) if the field was not found. An error will
+be logged if staticjinjaplus can't determine which template partial to use, and rendering of the Markdown file will be
+canceled.
+
+This template partial will be given a Markdown-specific variable named `markdown` containing a dictionary which keys and
+values are detailed below.
+
+| Name                 | Type              | Description                                                                                                            |
+|----------------------|-------------------|------------------------------------------------------------------------------------------------------------------------|
+| `markdown.converted` | markupsafe.Markup | The resulting HTML, marked as safe to be rendered by Jinja. Metadata are of course not included in this output         |
+| `markdown.source`    | str               | The Markdown template filename                                                                                         |
+| `markdown.url`       | str               | The rendered Markdown template URL                                                                                     |
+| `markdown.meta`      | Dict[str, str]    | Metadata parsed from the source Markdown file. Multiline values have been concatenated using `\n` without extra spaces |
+
+Internal URLs must be written using the rendered version of the templates/assets/static files, i.e. URLs relative to what
+will be rendered in the `OUTPUT_DIR` directory. staticjinjaplus will not rewrite any URLs in any manner: you must provide
+the right ones by yourself. See example below.
+
+See also the `collected` [Jinja global](#globals) which contain - among others - all Markdown files found in the
+`TEMPLATES_DIR` directory (as seen by staticjinja) along their parsed metadata, and more.
+
+**Example Markdown file:**
+
+```markdown
+partial: blog/_post.html
+
+My awesome blog post. It has internal [links](/blog/my-article.html), and one image:
+
+![](/images/attachment.png)
+
+This image may come from the `STATIC_DIR` directory.
+```
+
+### Command line interface
+
+The `staticjinjaplus` CLI is your main and only way to interact with staticjinjaplus. The following commands are available.
+
+#### `staticjinjaplus build`
+
+Build the site by rendering your templates from the `TEMPLATES_DIR` directory in the `OUTPUT_DIR` directory.
+
+**Options:**
+
+  - `-w, --watch` Automatically rebuild the site when templates are modified. **This option does not watch for assets or static files changes (yet?)**
+
+It will then copy the tree contained in the `STATIC_DIR` directory in the `OUTPUT_DIR`, as-is.
+
+staticjinja will be then initialized with the given `CONTEXTS` and Jinja's `JINJA_GLOBALS`/`JINJA_FILTERS`/`JINJA_EXTENSIONS`,
+[webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) (`WEBASSETS_BUNDLES`) will be registered, and
+the actual rendering process is started.
+
+`.html`, `.xml`, `.rss`, `.atom` and `.json` template output will be automatically minified, according to the `MINIFY_XML`
+and `MINIFY_JSON` configuration values. `.md` files will be converted to HTML and rendered using the appropriate template
+partial, which output will be automatically minified as well if configured so.
+
+#### `staticjinjaplus clean`
+
+Delete and recreate the `OUTPUT_DIR` directory.
+
+#### `staticjinjaplus publish`
+
+> [!NOTE]
+> This feature requires a Linux-like environment.
+
+Apply configuration values override from [environment variables](#environment-variables), then successively run
+`staticjinjaplus clean` and `staticjinjaplus build` prior remotely syncing the `OUTPUT_DIR` directory content using
+`rsync` through SSH.
+
+#### `staticjinjaplus serve`
+
+Serve the `OUTPUT_DIR` directory using Python's built-in HTTP server, plus a couple improvements:
+
+  - URL rewrite for HTML files is emulated, i.e. both `/about.html` and `/about` will work
+  - Custom HTTP error pages are emulated, if they are found saved as `{status code}.html` in the output directory
+  - The server will listen to both IPv4 *and* IPv6 loopback addresses if possible
+  - RSS and Atom files will be served using the appropriate MIME type in the `Content-Type` response header
+
+By default, you can browse your generated site at http://localhost:8080/ or [http://[::1]:8080/](http://[::1]:8080/).
+Port can be changed by defining the `SERVE_PORT` [configuration value](#configpy).
+
+## Configuration
+
+### `config.py`
+
+Your project's configuration happens in a single `config.py` file in the root directory (where the `staticjinjaplus`
+CLI should be executed). You'll find the available configuration values below.
+
+> [!NOTE]
+>   - All paths are relative to the root directory, unless otherwise stated.
+>   - None of these configuration values are required, so is `config.py`.
+>   - Only uppercase variables are loaded by staticjinjaplus.
+
+| Name                       | Type                                              | Default                          | Description                                                                                                                                                                                                                                                                                                                           |
+|----------------------------|---------------------------------------------------|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `SERVE_PORT`               | int                                               | `8080`                           | Listening port of the HTTP server started by `staticjinjaplus serve`                                                                                                                                                                                                                                                                  |
+| `BASE_URL`                 | str                                               | `http://localhost:{SERVE_PORT}/` | Protocol and domain name to use to generate meaningful absolute URLs. Set host part to `[::1]` if you plan to use IPv6                                                                                                                                                                                                                |
+| `MINIFY_XML`               | bool                                              | `False`                          | Enable XML minification                                                                                                                                                                                                                                                                                                               |
+| `MINIFY_JSON`              | bool                                              | `False`                          | Enable JSON minification                                                                                                                                                                                                                                                                                                              |
+| `TEMPLATES_DIR`            | str                                               | `templates`                      | Directory containing the Jinja templates to be processed                                                                                                                                                                                                                                                                              |
+| `OUTPUT_DIR`               | str                                               | `output`                         | Directory where the rendered site will be saved                                                                                                                                                                                                                                                                                       |
+| `STATIC_DIR`               | str                                               | `static`                         | Directory containing static files                                                                                                                                                                                                                                                                                                     |
+| `ASSETS_DIR`               | str                                               | `assets`                         | Directory containing assets, i.e. files that needs prior processing before being able to be used by the rendered site                                                                                                                                                                                                                 |
+| `CONTEXTS`                 | List[Tuple[str, Union[Dict[str, Any], Callable]]] | `[]`                             | [staticjinja contexts](https://staticjinja.readthedocs.io/en/stable/user/advanced.html#loading-data) to be used by templates                                                                                                                                                                                                          |
+| `WEBASSETS_BUNDLES`        | List[Tuple[str, Tuple[str,...], Dict[str, str]]   | `[]`                             | [webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) to be registered. These are passed to [`register()`](https://webassets.readthedocs.io/en/latest/environment.html#registering-bundles). Sources are relative to `ASSETS_DIR`, destinations to `OUTPUT_DIR`                                                |
+| `JINJA_GLOBALS`            | Dict[str, Any]                                    | `{}`                             | [jinja globals](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.globals) to be made available in all templates                                                                                                                                                                                                     |
+| `JINJA_FILTERS`            | Dict[str, Callable]                               | `{}`                             | [jinja filters](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.filters) to be made available in all templates                                                                                                                                                                                                     |
+| `JINJA_EXTENSIONS`         | List[Union[str, jinja2.ext.Extension]]            | `[]`                             | [jinja extensions](https://jinja.palletsprojects.com/en/3.1.x/extensions/) to load                                                                                                                                                                                                                                                    |
+| `MARKDOWN_EXTENSIONS`      | Dict[str, Dict]                                   | `{}`                             | [Markdown extensions](https://python-markdown.github.io/extensions/) to load and their respective configuration. Keys are passed to [`extensions`](https://python-markdown.github.io/reference/#extensions); the entire dictionary is passed to [`extension_configs`](https://python-markdown.github.io/reference/#extension_configs) |
+| `MARKDOWN_DEFAULT_PARTIAL` | Optional[str]                                     | `None`                           | Default template partial to use when rendering Markdown files when the `partial` metadata is not present                                                                                                                                                                                                                              |
+| `USE_HTML_EXTENSION`       | bool                                              | `True`                           | If your site's links are using URLs without `.html` extension (URL rewrite), you must set this config value to `False`. This config value does **not** alter the behavior of `absurl()` in any way                                                                                                                                    |
+
+### Environment variables
+
+Some configuration values may/must be overridden by environment variables of the same name when publishing your site
+(`staticjinjaplus publish` command), typically in a deployment environment. You'll find the list below.
+
+| Name          | Type   | Required?                      | Default                           | Description                                                          |
+|---------------|--------|--------------------------------|-----------------------------------|----------------------------------------------------------------------|
+| `BASE_URL`    | str    | Yes                            |                                   | Protocol and domain name to use to generate meaningful absolute URLs |
+| `MINIFY_XML`  | bool ¹ | No, but activation recommended | `MINIFY_XML` configuration value  | Enable XML minification                                              |
+| `MINIFY_JSON` | bool ¹ | No, but activation recommended | `MINIFY_JSON` configuration value | Enable JSON minification                                             |
+| `SSH_USER`    | str    | Yes                            |                                   | SSH username                                                         |
+| `SSH_HOST`    | str    | Yes                            |                                   | SSH hostname                                                         |
+| `SSH_PORT`    | int    | No                             | `22`                              | SSH port                                                             |
+| `SSH_PATH`    | str    | Yes                            |                                   | Absolute path to the deployment directory on the SSH host            |
+
+¹ Any [falsy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.falsy) or
+[truthy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.truthy) string
+representation of boolean values allowed by marshmallow
+
+## Development
+
+### Getting source code and installing the package with dev dependencies
+
+  1. Clone the repository
+  2. From the root directory, run: `pip install -e .[dev]` on Linux or `pip install -e ".[dev]"` on Windows
+
+### Releasing the package
+
+From the root directory, run `python setup.py upload`. This will build the package, create a git tag and publish on PyPI.
+
+`__version__` in `staticjinjaplus/__version__.py` must be updated beforehand. It should adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+An associated GitHub release must be created following the [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format.
```

### Comparing `staticjinjaplus-1.1.2/setup.py` & `staticjinjaplus-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# Original setup.py template: https://github.com/kennethreitz/setup.py
-
-from setuptools import find_packages, setup, Command
-from importlib import util as importlib_util
-from subprocess import call
-from shutil import rmtree
-from os import path
-import sys
-
-NAME = 'staticjinjaplus'
-DESCRIPTION = 'A sweet spot between staticjinja and a full-blown static site generator.'
-URL = 'https://github.com/EpocDotFr/staticjinjaplus'
-EMAIL = 'contact.nospam@epoc.nospam.fr'
-AUTHOR = 'Maxime "Epoc" Gross'
-REQUIRES_PYTHON = '>=3.9'
-VERSION = None  # Pulled from staticjinjaplus/__version__.py
-
-REQUIRED = [
-    'staticjinja~=5.0',
-    'webassets~=2.0',
-    'htmlmin~=0.1',
-    'cssutils~=2.10',
-    'jsmin~=3.0',
-    'environs~=11.0',
-]
-
-EXTRAS = {
-    'dev': {
-        'build~=1.2',
-        'twine~=5.0',
-        'setuptools~=69.5',
-    }
-}
-
-CLASSIFIERS = [
-    'Development Status :: 5 - Production/Stable',
-    'Operating System :: OS Independent',
-    'Environment :: Console',
-    'Environment :: Web Environment',
-    'Topic :: Internet :: WWW/HTTP :: Site Management',
-    'Topic :: Text Processing :: Markup :: XML',
-    'Topic :: Text Processing :: Markup :: HTML',
-    'Topic :: Text Processing :: Markup :: Markdown',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'Programming Language :: Python :: 3.12',
-    'Intended Audience :: Developers',
-]
-
-PROJECT_URLS = {
-    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme',
-    'Source': 'https://github.com/EpocDotFr/staticjinjaplus',
-    'Tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
-    'Changelog': 'https://github.com/EpocDotFr/staticjinjaplus/releases',
-}
-
-KEYWORDS = ['static', 'website', 'site', 'generator', 'staticjinja', 'jinja', 'jinja2']
-
-here = path.abspath(path.dirname(__file__))
-
-try:
-    with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-about = {}
-
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-
-    spec = importlib_util.spec_from_file_location('__version__', path.join(here, project_slug, '__version__.py'))
-    module = importlib_util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-
-    about['__version__'] = module.__version__
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-
-            rmtree(path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel distribution…')
-
-        call('"{0}" -m build --sdist --wheel'.format(sys.executable), shell=True)
-
-        self.status('Uploading the package to PyPI via Twine…')
-
-        call('twine upload dist/*', shell=True)
-
-        self.status('Pushing git tags…')
-
-        call('git tag v{0}'.format(about['__version__']), shell=True)
-        call('git push --tags', shell=True)
-
-        exit()
-
-
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(),
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license='DBAD',
-    entry_points={
-        'console_scripts': [
-            'staticjinjaplus = staticjinjaplus.cli:cli',
-        ]
-    },
-    classifiers=CLASSIFIERS,
-    cmdclass={
-        'upload': UploadCommand,
-    },
-    project_urls=PROJECT_URLS,
-    keywords=KEYWORDS
-)
+# Original setup.py template: https://github.com/kennethreitz/setup.py
+
+from setuptools import find_packages, setup, Command
+from importlib import util as importlib_util
+from subprocess import call
+from shutil import rmtree
+from os import path
+import sys
+
+NAME = 'staticjinjaplus'
+DESCRIPTION = 'A sweet spot between staticjinja and a full-blown static site generator.'
+URL = 'https://github.com/EpocDotFr/staticjinjaplus'
+EMAIL = 'contact.nospam@epoc.nospam.fr'
+AUTHOR = 'Maxime "Epoc" Gross'
+REQUIRES_PYTHON = '>=3.10'
+VERSION = None  # Pulled from staticjinjaplus/__version__.py
+
+REQUIRED = [
+    'staticjinja~=5.0',
+    'webassets~=2.0',
+    'htmlmin~=0.1',
+    'cssutils~=2.10',
+    'jsmin~=3.0',
+    'environs~=11.0',
+    'markdown~=3.6',
+]
+
+EXTRAS = {
+    'dev': {
+        'build~=1.2',
+        'twine~=5.0',
+        'setuptools~=69.5',
+    }
+}
+
+CLASSIFIERS = [
+    'Development Status :: 5 - Production/Stable',
+    'Operating System :: OS Independent',
+    'Environment :: Console',
+    'Environment :: Web Environment',
+    'Topic :: Internet :: WWW/HTTP :: Site Management',
+    'Topic :: Text Processing :: Markup :: XML',
+    'Topic :: Text Processing :: Markup :: HTML',
+    'Topic :: Text Processing :: Markup :: Markdown',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
+    'Intended Audience :: Developers',
+]
+
+PROJECT_URLS = {
+    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme',
+    'Source': 'https://github.com/EpocDotFr/staticjinjaplus',
+    'Tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
+    'Changelog': 'https://github.com/EpocDotFr/staticjinjaplus/releases',
+}
+
+KEYWORDS = ['static', 'website', 'site', 'generator', 'staticjinja', 'jinja', 'jinja2']
+
+here = path.abspath(path.dirname(__file__))
+
+try:
+    with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+about = {}
+
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+
+    spec = importlib_util.spec_from_file_location('__version__', path.join(here, project_slug, '__version__.py'))
+    module = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+
+    about['__version__'] = module.__version__
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+
+            rmtree(path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel distribution…')
+
+        call('"{0}" -m build --sdist --wheel'.format(sys.executable), shell=True)
+
+        self.status('Uploading the package to PyPI via Twine…')
+
+        call('twine upload dist/*', shell=True)
+
+        self.status('Pushing git tags…')
+
+        call('git tag v{0}'.format(about['__version__']), shell=True)
+        call('git push --tags', shell=True)
+
+        exit()
+
+
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(),
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license='DBAD',
+    entry_points={
+        'console_scripts': [
+            'staticjinjaplus = staticjinjaplus.cli:cli',
+        ]
+    },
+    classifiers=CLASSIFIERS,
+    cmdclass={
+        'upload': UploadCommand,
+    },
+    project_urls=PROJECT_URLS,
+    keywords=KEYWORDS
+)
```

### Comparing `staticjinjaplus-1.1.2/staticjinjaplus/__init__.py` & `staticjinjaplus-2.0.0/staticjinjaplus/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,212 +1,195 @@
-from staticjinjaplus.http import EnhancedThreadingHTTPServer, SimpleEnhancedHTTPRequestHandler
-from staticjinjaplus import staticjinja_helpers, jinja_helpers
-from webassets import Environment as AssetsEnvironment
-from importlib import util as importlib_util
-from jinja2 import select_autoescape
-from staticjinja import Site, logger
-from shutil import copytree, rmtree
-from os import makedirs, path
-from subprocess import call
-from environs import Env
-from typing import Dict
-import locale
-
-
-def load_config() -> Dict:
-    """Load configuration from both `config.py` in the directory where staticjinjaplus is executed and environment
-    variables, returning a dict representation of this configuration. Only uppercase variables are loaded"""
-
-    # Set default config values
-    serve_port = 8080
-
-    config = {
-        'LOCALE': None,
-        'SERVE_PORT': serve_port,
-        'BASE_URL': f'http://localhost:{serve_port}/',
-        'MINIFY_XML': False,
-        'MINIFY_JSON': False,
-        'TEMPLATES_DIR': 'templates',
-        'OUTPUT_DIR': 'output',
-        'STATIC_DIR': 'static',
-        'ASSETS_DIR': 'assets',
-        'ASSETS_BUNDLES': [],
-        'CONTEXTS': [],
-        'GLOBALS': {},
-        'FILTERS': {},
-        'EXTENSIONS': [],
-    }
-
-    # Load and erase default config values from config.py, if the file exists
-    try:
-        spec = importlib_util.spec_from_file_location('config', 'config.py')
-        actual_config = importlib_util.module_from_spec(spec)
-        spec.loader.exec_module(actual_config)
-
-        config.update({
-            k: v for k, v in vars(actual_config).items() if k.isupper()
-        })
-    except FileNotFoundError:
-        pass
-
-    return config
-
-
-def set_locale(config: Dict) -> None:
-    """Set the system locale based on the LOCALE config"""
-    if not config['LOCALE']:
-        return
-
-    locale_successfully_set = False
-
-    for code in config['LOCALE']:
-        try:
-            locale.setlocale(locale.LC_ALL, code)
-
-            locale_successfully_set = True
-
-            logger.info(f'System locale set to {code}')
-
-            break
-        except locale.Error:
-            pass
-
-    if not locale_successfully_set:
-        logger.error('Unable to set system locale')
-
-
-def build(config: Dict, watch: bool = False) -> None:
-    """Build the site"""
-    set_locale(config)
-
-    webassets_cache = path.join(config['ASSETS_DIR'], '.webassets-cache')
-
-    makedirs(webassets_cache, exist_ok=True)
-    makedirs(config['STATIC_DIR'], exist_ok=True)
-    makedirs(config['OUTPUT_DIR'], exist_ok=True)
-    makedirs(config['ASSETS_DIR'], exist_ok=True)
-
-    logger.info('Copying static files from "{STATIC_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
-
-    copytree(
-        config['STATIC_DIR'],
-        config['OUTPUT_DIR'],
-        dirs_exist_ok=True
-    )
-
-    logger.info('Building from "{TEMPLATES_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
-
-    rules = [
-        r for r in [
-            (r'.*\.(xml|html|rss|atom)', staticjinja_helpers.minify_xml_template) if config['MINIFY_XML'] else None,
-            (r'.*\.json', staticjinja_helpers.minify_json_template) if config['MINIFY_JSON'] else None,
-        ] if r is not None
-    ]
-
-    jinja_globals = {
-        'config': config,
-        'url': jinja_helpers.url(config),
-        'icon': jinja_helpers.icon(config),
-    }
-
-    jinja_globals.update(config['GLOBALS'])
-
-    jinja_filters = {
-        'tojsonm': jinja_helpers.tojsonm(config),
-        'dictmerge': jinja_helpers.dictmerge,
-    }
-
-    jinja_filters.update(config['FILTERS'])
-
-    jinja_extensions = [
-        'webassets.ext.jinja2.AssetsExtension',
-    ]
-
-    jinja_extensions.extend(config['EXTENSIONS'])
-
-    site = Site.make_site(
-        searchpath=config['TEMPLATES_DIR'],
-        outpath=config['OUTPUT_DIR'],
-        mergecontexts=True,
-        env_globals=jinja_globals,
-        filters=jinja_filters,
-        contexts=config['CONTEXTS'] or None,
-        rules=rules or None,
-        extensions=jinja_extensions,
-        env_kwargs={
-            'trim_blocks': True,
-            'lstrip_blocks': True,
-            'autoescape': select_autoescape(enabled_extensions=('html', 'htm', 'xml', 'rss', 'atom')),
-        }
-    )
-
-    site.env.assets_environment = AssetsEnvironment(
-        directory=config['OUTPUT_DIR'],
-        url='/',
-        cache=webassets_cache
-    )
-
-    site.env.assets_environment.append_path(config['ASSETS_DIR'])
-
-    for name, args, kwargs in config['ASSETS_BUNDLES']:
-        site.env.assets_environment.register(name, *args, **kwargs)
-
-    site.render(watch)
-
-
-def clean(config: Dict) -> None:
-    """Delete and recreate the output directory"""
-    logger.info('Deleting and recreating "{OUTPUT_DIR}"...'.format(**config))
-
-    if path.isdir(config['OUTPUT_DIR']):
-        rmtree(config['OUTPUT_DIR'])
-
-    makedirs(config['OUTPUT_DIR'], exist_ok=True)
-
-
-def publish(config: Dict) -> None:
-    """Build and publish the site (using `rsync` through SSH)"""
-    logger.info('Overriding some configuration values from environment variables...')
-
-    env = Env()
-
-    config.update({
-        'BASE_URL': env.str('BASE_URL'),
-        'MINIFY_XML': env.bool('MINIFY_XML', config['MINIFY_XML']),
-        'MINIFY_JSON': env.bool('MINIFY_JSON', config['MINIFY_JSON']),
-        'SSH_USER': env.str('SSH_USER'),
-        'SSH_HOST': env.str('SSH_HOST'),
-        'SSH_PORT': env.int('SSH_PORT', default=22),
-        'SSH_PATH': env.str('SSH_PATH'),
-    })
-
-    clean(config)
-    build(config)
-
-    exit(call(
-        'rsync --delete --exclude ".DS_Store" -pthrvz -c '
-        '-e "ssh -p {SSH_PORT}" '
-        '{} {SSH_USER}@{SSH_HOST}:{SSH_PATH}'.format(
-            config['OUTPUT_DIR'].rstrip('/') + '/', **config
-        ),
-        shell=True
-    ))
-
-
-def serve(config: Dict) -> None:
-    """Serve the rendered site directory through HTTP"""
-    with EnhancedThreadingHTTPServer(
-            ('', config['SERVE_PORT']),
-            SimpleEnhancedHTTPRequestHandler,
-            directory=config['OUTPUT_DIR']
-    ) as server:
-        msg = 'Serving "{OUTPUT_DIR}" on http://localhost:{SERVE_PORT}/'.format(**config)
-
-        if server.has_dualstack_ipv6:
-            msg += ' and http://[::1]:{SERVE_PORT}/'.format(**config)
-
-        logger.info(msg)
-
-        try:
-            server.serve_forever()
-        except KeyboardInterrupt:
-            pass
+from staticjinjaplus import config, collect_templates, staticjinja_helpers, jinja_helpers, __generator__
+from staticjinjaplus.http import EnhancedThreadingHTTPServer, SimpleEnhancedHTTPRequestHandler
+from webassets import Environment as AssetsEnvironment
+from staticjinja import Site, logger
+from jinja2 import select_autoescape
+from argparse import ArgumentParser
+from shutil import copytree, rmtree
+from os import makedirs, path
+from subprocess import call
+from environs import Env
+
+
+def build(watch: bool = False) -> None:
+    """Build the site"""
+    webassets_cache = path.join(config['ASSETS_DIR'], '.webassets-cache')
+
+    makedirs(webassets_cache, exist_ok=True)
+    makedirs(config['TEMPLATES_DIR'], exist_ok=True)
+    makedirs(config['OUTPUT_DIR'], exist_ok=True)
+    makedirs(config['STATIC_DIR'], exist_ok=True)
+    makedirs(config['ASSETS_DIR'], exist_ok=True)
+
+    logger.info('Copying static files from "{STATIC_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
+
+    copytree(
+        config['STATIC_DIR'],
+        config['OUTPUT_DIR'],
+        dirs_exist_ok=True
+    )
+
+    logger.info('Building from "{TEMPLATES_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
+
+    rules = [
+        r for r in [
+            (r'.*\.(xml|html|rss|atom)', staticjinja_helpers.minify_xml_template) if config['MINIFY_XML'] else None,
+            (r'.*\.json', staticjinja_helpers.minify_json_template) if config['MINIFY_JSON'] else None,
+            (r'.*\.md', staticjinja_helpers.render_markdown_template),
+        ] if r is not None
+    ]
+
+    jinja_globals = {
+        'config': config,
+        'absurl': jinja_helpers.absurl,
+        'embed': jinja_helpers.embed,
+        'collected': list(collect_templates()),
+        '__generator__': __generator__,
+    }
+
+    jinja_globals.update(config['JINJA_GLOBALS'])
+
+    jinja_filters = {
+        'tojsonm': jinja_helpers.tojsonm,
+        'dictmerge': jinja_helpers.dictmerge,
+    }
+
+    jinja_filters.update(config['JINJA_FILTERS'])
+
+    contexts = [
+        (r'.*\.md', staticjinja_helpers.convert_markdown_file)
+    ]
+
+    if config['CONTEXTS']:
+        contexts.extend(config['CONTEXTS'])
+
+    jinja_extensions = [
+        'webassets.ext.jinja2.AssetsExtension',
+    ]
+
+    jinja_extensions.extend(config['JINJA_EXTENSIONS'])
+
+    site = Site.make_site(
+        searchpath=config['TEMPLATES_DIR'],
+        outpath=config['OUTPUT_DIR'],
+        mergecontexts=True,
+        env_globals=jinja_globals,
+        filters=jinja_filters,
+        contexts=contexts,
+        rules=rules or None,
+        extensions=jinja_extensions,
+        env_kwargs={
+            'trim_blocks': True,
+            'lstrip_blocks': True,
+            'autoescape': select_autoescape(enabled_extensions=('html', 'xml', 'rss', 'atom')),
+        }
+    )
+
+    site.env.assets_environment = AssetsEnvironment(
+        directory=config['OUTPUT_DIR'],
+        url='/',
+        cache=webassets_cache
+    )
+
+    site.env.assets_environment.append_path(config['ASSETS_DIR'])
+
+    for name, args, kwargs in config['WEBASSETS_BUNDLES']:
+        site.env.assets_environment.register(name, *args, **kwargs)
+
+    site.render(watch)
+
+
+def clean() -> None:
+    """Delete and recreate the output directory"""
+    logger.info('Deleting and recreating "{OUTPUT_DIR}"...'.format(**config))
+
+    if path.isdir(config['OUTPUT_DIR']):
+        rmtree(config['OUTPUT_DIR'])
+
+    makedirs(config['OUTPUT_DIR'], exist_ok=True)
+
+
+def publish() -> None:
+    """Build and publish the site (using `rsync` through SSH)"""
+    logger.info('Overriding some configuration values from environment variables...')
+
+    env = Env()
+
+    config.update({
+        'BASE_URL': env.str('BASE_URL'),
+        'MINIFY_XML': env.bool('MINIFY_XML', config['MINIFY_XML']),
+        'MINIFY_JSON': env.bool('MINIFY_JSON', config['MINIFY_JSON']),
+        'SSH_USER': env.str('SSH_USER'),
+        'SSH_HOST': env.str('SSH_HOST'),
+        'SSH_PORT': env.int('SSH_PORT', default=22),
+        'SSH_PATH': env.str('SSH_PATH'),
+    })
+
+    clean()
+    build()
+
+    exit(call(
+        'rsync --delete --exclude ".DS_Store" -pthrvz -c '
+        '-e "ssh -p {SSH_PORT}" '
+        '{} {SSH_USER}@{SSH_HOST}:{SSH_PATH}'.format(
+            config['OUTPUT_DIR'].rstrip('/') + '/', **config
+        ),
+        shell=True
+    ))
+
+
+def serve() -> None:
+    """Serve the rendered site directory through HTTP"""
+    with EnhancedThreadingHTTPServer(
+            ('', config['SERVE_PORT']),
+            SimpleEnhancedHTTPRequestHandler,
+            directory=config['OUTPUT_DIR']
+    ) as server:
+        msg = 'Serving "{OUTPUT_DIR}" on http://localhost:{SERVE_PORT}/'.format(**config)
+
+        if server.has_dualstack_ipv6:
+            msg += ' and http://[::1]:{SERVE_PORT}/'.format(**config)
+
+        logger.info(msg)
+
+        try:
+            server.serve_forever()
+        except KeyboardInterrupt:
+            pass
+
+
+def cli() -> None:
+    arg_parser = ArgumentParser(
+        description='The staticjinjaplus CLI which should be your main and only way to interact with staticjinjaplus.'
+    )
+
+    arg_parser.add_argument(
+        '-v', '--version',
+        action='version',
+        version=__generator__
+    )
+
+    command_arg_parser = arg_parser.add_subparsers(dest='command', required=True)
+
+    build_arg_parser = command_arg_parser.add_parser('build', help='Build the site')
+    build_arg_parser.add_argument(
+        '-w', '--watch',
+        help='Automatically rebuild the site when templates are modified',
+        action='store_true'
+    )
+
+    command_arg_parser.add_parser('clean', help='Delete and recreate the output directory')
+
+    command_arg_parser.add_parser('publish', help='Build and publish the site (using `rsync` through SSH)')
+
+    command_arg_parser.add_parser('serve', help='Serve the output directory through HTTP')
+
+    args = arg_parser.parse_args()
+
+    if args.command == 'build':
+        build(args.watch)
+    elif args.command == 'clean':
+        clean()
+    elif args.command == 'publish':
+        publish()
+    elif args.command == 'serve':
+        serve()
```

### Comparing `staticjinjaplus-1.1.2/staticjinjaplus/http.py` & `staticjinjaplus-2.0.0/staticjinjaplus/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,83 @@
-from __future__ import annotations
-from http.server import ThreadingHTTPServer, SimpleHTTPRequestHandler
-from typing import Optional
-from http import HTTPStatus
-from os import fstat, path
-import socket
-
-
-class EnhancedThreadingHTTPServer(ThreadingHTTPServer):
-    """Same as ThreadingHTTPServer but the directory to be served may be passed to its constructor. It also tries to
-    listen to both IPv4 and IPv6 loopback addresses"""
-    allow_reuse_address = True
-    daemon_threads = True
-    has_dualstack_ipv6: bool
-    directory: str
-    RequestHandlerClass: SimpleEnhancedHTTPRequestHandler
-
-    def __init__(self, *args, directory: str, **kvargs):
-        self.has_dualstack_ipv6 = socket.has_dualstack_ipv6()
-        self.address_family = socket.AF_INET6 if self.has_dualstack_ipv6 else socket.AF_INET
-        self.directory = directory
-
-        super().__init__(*args, **kvargs)
-
-    def server_bind(self) -> None:
-        if self.has_dualstack_ipv6:
-            self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
-
-        super().server_bind()
-
-    def finish_request(self, request, client_address) -> None:
-        self.RequestHandlerClass(request, client_address, self, directory=self.directory)
-
-
-class SimpleEnhancedHTTPRequestHandler(SimpleHTTPRequestHandler):
-    """A simple HTTP server handler which is meant to serve the output directory, with some enhancements (emulates URL
-    rewrite for HTML files without .html extension; emulates custom 404 error page"""
-    protocol_version = 'HTTP/1.1'
-    server: EnhancedThreadingHTTPServer
-
-    def __init__(self, *args, **kvargs):
-        try:
-            super().__init__(*args, **kvargs)
-        except (ConnectionAbortedError, BrokenPipeError):
-            pass
-
-    def translate_path(self, p: str) -> str:
-        p = super().translate_path(p)
-
-        if not p.endswith(('\\', '/')):
-            _, extension = path.splitext(p)
-
-            if not extension:
-                p += '.html'
-
-        return p
-
-    def send_error(self, code: int, message: Optional[str] = None, explain: Optional[str] = None) -> None:
-        status = HTTPStatus(code)
-
-        if self.command != 'HEAD' and (status.is_client_error or status.is_server_error):
-            try:
-                f = open(path.join(self.directory, f'{status.value}.html'), 'rb')
-            except OSError:
-                return super().send_error(code, message=message, explain=explain)
-
-            fs = fstat(f.fileno())
-
-            self.send_response(code, message)
-            self.send_header('Connection', 'close')
-
-            self.send_header('Content-Type', self.error_content_type)
-            self.send_header('Content-Length', str(fs[6]))
-            self.end_headers()
-
-            self.copyfile(f, self.wfile)
-        else:
-            return super().send_error(code, message=message, explain=explain)
+from __future__ import annotations
+from http.server import ThreadingHTTPServer, SimpleHTTPRequestHandler
+from typing import Optional
+from http import HTTPStatus
+from os import fstat, path
+import socket
+
+
+class EnhancedThreadingHTTPServer(ThreadingHTTPServer):
+    """Same as ThreadingHTTPServer but the directory to be served may be passed to its constructor. It also tries to
+    listen to both IPv4 and IPv6 loopback addresses"""
+    allow_reuse_address = True
+    daemon_threads = True
+    has_dualstack_ipv6: bool
+    directory: str
+    RequestHandlerClass: SimpleEnhancedHTTPRequestHandler
+
+    def __init__(self, *args, directory: str, **kwargs):
+        self.has_dualstack_ipv6 = socket.has_dualstack_ipv6()
+        self.address_family = socket.AF_INET6 if self.has_dualstack_ipv6 else socket.AF_INET
+        self.directory = directory
+
+        super().__init__(*args, **kwargs)
+
+    def server_bind(self) -> None:
+        if self.has_dualstack_ipv6:
+            self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
+
+        super().server_bind()
+
+    def finish_request(self, request, client_address) -> None:
+        self.RequestHandlerClass(request, client_address, self, directory=self.directory)
+
+
+class SimpleEnhancedHTTPRequestHandler(SimpleHTTPRequestHandler):
+    """A simple HTTP server handler which is meant to serve the output directory, with some enhancements (emulates URL
+    rewrite for HTML files without .html extension; emulates custom 404 error page"""
+    protocol_version = 'HTTP/1.1'
+    server: EnhancedThreadingHTTPServer
+
+    def __init__(self, *args, **kwargs):
+        self.extensions_map.update({
+            '.rss': 'application/rss+xml',
+            '.atom': 'application/atom+xml',
+        })
+
+        try:
+            super().__init__(*args, **kwargs)
+        except (ConnectionAbortedError, BrokenPipeError):
+            pass
+
+    def translate_path(self, p: str) -> str:
+        p = super().translate_path(p)
+
+        if not p.endswith(('\\', '/')):
+            _, extension = path.splitext(p)
+
+            if not extension:
+                p += '.html'
+
+        return p
+
+    def send_error(self, code: int, message: Optional[str] = None, explain: Optional[str] = None) -> None:
+        status = HTTPStatus(code)
+
+        if self.command != 'HEAD' and (status.is_client_error or status.is_server_error):
+            try:
+                f = open(path.join(self.directory, f'{status.value}.html'), 'rb')
+            except OSError:
+                return super().send_error(code, message=message, explain=explain)
+
+            fs = fstat(f.fileno())
+
+            self.send_response(code, message)
+            self.send_header('Connection', 'close')
+
+            self.send_header('Content-Type', self.error_content_type)
+            self.send_header('Content-Length', str(fs[6]))
+            self.end_headers()
+
+            self.copyfile(f, self.wfile)
+        else:
+            return super().send_error(code, message=message, explain=explain)
```

### Comparing `staticjinjaplus-1.1.2/staticjinjaplus/jinja_helpers.py` & `staticjinjaplus-2.0.0/staticjinjaplus/jinja_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-from jinja2.utils import htmlsafe_json_dumps
-from typing import Dict, Callable
-from markupsafe import Markup
-from os import path
-
-
-def url(config: Dict) -> Callable:
-    """Build a relative or absolute URL to a file relative to the output dir"""
-    def inner(p: str, absolute: bool = False) -> str:
-        ret = config['BASE_URL'].rstrip('/') + '/' if absolute else '/'
-        ret += p.lstrip('/')
-
-        return ret
-
-    return inner
-
-
-def icon(config: Dict) -> Callable:
-    """Embed the SVG markup of an SVG icon relative to the `{assets dir}/icons` directory"""
-    def inner(name: str) -> Markup:
-        with open(path.join(config['ASSETS_DIR'], 'icons', f'{name}.svg'), 'r') as f:
-            return Markup(f.read())
-
-    return inner
-
-
-def tojsonm(config: Dict) -> Callable:
-    """Serialize the given data to JSON, minifying (or not) the output in function of current configuration"""
-    def inner(data: Dict) -> Markup:
-        return htmlsafe_json_dumps(
-            data,
-            indent=None if config['MINIFY_JSON'] else 4,
-            separators=(',', ':') if config['MINIFY_JSON'] else None
-        )
-
-    return inner
-
-
-def dictmerge(left: Dict, right: Dict) -> Dict:
-    """Merge two dicts"""
-    return left | right
+from jinja2.utils import htmlsafe_json_dumps
+from staticjinjaplus import config
+from markupsafe import Markup
+from typing import Dict
+from os import path
+
+
+def absurl(resource: str) -> str:
+    """Build an absolute URL to a file relative to the output dir"""
+    return config['BASE_URL'].rstrip('/') + '/' + resource.lstrip('/')
+
+
+def embed(filename: str) -> Markup:
+    """Read and return the content of the given file, marked as safe to be rendered by Jinja, relative to the assets
+    directory"""
+    with open(path.join(config['ASSETS_DIR'], filename), 'r') as f:
+        return Markup(f.read())
+
+
+def tojsonm(data: Dict) -> Markup:
+    """Serialize the given data to JSON, minifying (or not) the output in function of current configuration"""
+    return htmlsafe_json_dumps(
+        data,
+        indent=None if config['MINIFY_JSON'] else 4,
+        separators=(',', ':') if config['MINIFY_JSON'] else None
+    )
+
+
+def dictmerge(left: Dict, right: Dict) -> Dict:
+    """Merge two dicts"""
+    return left | right
```

### Comparing `staticjinjaplus-1.1.2/staticjinjaplus.egg-info/PKG-INFO` & `staticjinjaplus-2.0.0/staticjinjaplus.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,274 +1,342 @@
-Metadata-Version: 2.1
-Name: staticjinjaplus
-Version: 1.1.2
-Summary: A sweet spot between staticjinja and a full-blown static site generator.
-Home-page: https://github.com/EpocDotFr/staticjinjaplus
-Author: Maxime "Epoc" Gross
-Author-email: contact.nospam@epoc.nospam.fr
-License: DBAD
-Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme
-Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
-Project-URL: Tracker, https://github.com/EpocDotFr/staticjinjaplus/issues
-Project-URL: Changelog, https://github.com/EpocDotFr/staticjinjaplus/releases
-Keywords: static,website,site,generator,staticjinja,jinja,jinja2
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Text Processing :: Markup :: XML
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: staticjinja~=5.0
-Requires-Dist: webassets~=2.0
-Requires-Dist: htmlmin~=0.1
-Requires-Dist: cssutils~=2.10
-Requires-Dist: jsmin~=3.0
-Requires-Dist: environs~=11.0
-Provides-Extra: dev
-Requires-Dist: twine~=5.0; extra == "dev"
-Requires-Dist: build~=1.2; extra == "dev"
-Requires-Dist: setuptools~=69.5; extra == "dev"
-
-
-# staticjinjaplus
-
-A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
-
-![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
-
-[PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
-
-Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
-I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
-order to be able to generate a static website that will actually be ready for real world usage.
-
-staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
-Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
-static site generator.
-
-## Features
-
-All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
-
-  - Simple, file-based configuration to centralize *a handful* of configuration values
-  - Build improvements
-    - Set system locale before building anything (useful when formatting dates to localized strings)
-    - Automatically copy static files to output directory
-    - Define staticjinja contexts in config file
-    - Define [webassets](https://webassets.readthedocs.io/en/latest/) bundles to allow CSS/JS concatenation/minification
-    - Automatically minify XML (including HTML, RSS and Atom)/JSON output
-  - Jinja improvements
-    - A few new Jinja globals/filters to make your life easier
-    - Autoescape is enabled for XML, HTML, RSS and Atom templates
-  - Serve the generated site through a local HTTP server
-    - URL rewrite emulation (for HTML files)
-    - Custom HTTP error pages emulation
-    - IPv6 loopback address support
-  - Publish the generated site through rsync over SSH
-
-**Planned:**
-
-  - Generic support of Markdown-formatted templates collections (forget about the usual "pages" or "articles/blog posts" feature)
-
-## Prerequisites
-
-  - Python >= 3.9
-
-## Installation
-
-From PyPI:
-
-```bash
-$ pip install staticjinjaplus
-```
-
-Locally, after cloning/downloading the repo:
-
-```bash
-$ pip install .
-```
-
-A CLI (`staticjinjaplus`) will be made available upon installation.
-
-## Usage
-
-### Templates
-
-You'll want to write your site's Jinja templates first: write them as usual. By default, staticjinjaplus searches for
-Jinja templates in the `templates` directory where it is invoked. You can change that by using the `TEMPLATES_DIR`
-[configuration value](#configpy).
-
-staticjinjaplus offers the following additional Jinja facilities.
-
-#### Globals
-
-| Name/signature                                  | Type     | Description                                                                                                                                                                                                         |
-|-------------------------------------------------|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `config`                                        | Dict     | Configuration values loaded from [`config.py`](#configpy) (defaults are guaranteed to be provided for built-in values). Only uppercase variables are loaded by staticjinjaplus                                      |
-| `url(path: str, absolute: bool = False) -> str` | Callable | Build (by default) a relative URL to a file located in the `OUTPUT_DIR` directory. Setting `absolute` to `True` prefixes the URL with `BASE_URL`. See [configuration values](#configpy)                             |
-| `icon(name: str) -> markupsafe.Markup`          | Callable | Return the file content of the given SVG icon, marked as safe to be rendered by Jinja. Icons must be saved in the form of `{ASSETS_DIR}/icons/{name}.svg`. Useful to embed SVG icons directly in the generated HTML |
-
-**Usage examples:**
-
-```html+jinja
-{{ config.BASE_URL }}         {# http://localhost:8080/ (by default) #}
-{{ config.MY_CUSTOM_CONFIG }} {# Whatever you defined in your config.py (uppercase variables only) #}
-
-{# url() doesn't care whether an extension is given or not #}
-{{ url('/about.html') }} {# /about.html #}
-{{ url('/about') }}      {# /about #}
-{{ url('about') }}       {# /about #}
-
-{# url() doesn't care about whether a static file is targeted or not #}
-{{ url('/images/logo.png') }} {# /images/logo.png #}
-{{ url('images/logo.png') }}  {# /images/logo.png #}
-
-{# URL is simply prefixed with BASE_URL when generating absolute URLs #}
-{{ url('/images/logo.png', absolute=True) }} {# http://localhost:8080/images/logo.png (by default) #}
-{{ url('images/logo.png', absolute=True) }}  {# http://localhost:8080/images/logo.png (by default) #}
-
-{{ icon('github') }} {# <svg xmlns="http://www.w3.org/2000/svg" ... </svg> #}
-```
-
-#### Filters
-
-| Signature                                      | Description                                                                                                                                                                                                                                                         |
-|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `<data: Dict>\|tojsonm -> str`                 | Serialize the given dictionary to a JSON string. Automatically takes into account the `MINIFY_JSON` [configuration value](#configpy) to minify (or not) the resulting output. Useful for e.g serializing [Schema.org](https://schema.org/)'s JSON-LD-formatted data |
-| `<left: Dict>\|dictmerge(right: Dict) -> Dict` | Merge two dictionaries. Does not modify existing ones, a new one will be created. Does **not** merge deeply                                                                                                                                                         |
-
-**Usage examples:**
-
-```html+jinja
-{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == False:
-                                 {
-                                     "yes": true
-                                 }
-                             #}
-
-{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == True:
-                                 {"yes":true}
-                             #}
-
-{{ dict(yes=True)|dictmerge(dict(no=False)) }} {# {"yes": True, "no": False} #}
-```
-
-### Command line interface
-
-The `staticjinjaplus` CLI is your main and only way to interact with staticjinjaplus. The following commands are available.
-
-#### `staticjinjaplus build`
-
-Build the site by rendering your templates from the `TEMPLATES_DIR` directory in the `OUTPUT_DIR` directory.
-
-**Options:**
-
-  - `-w, --watch` Automatically rebuild the site when templates are modified
-
-staticjinjaplus will first try to set the system's locale to the first working locale identifier set in the `LOCALE`
-[configuration value](#configpy) (if set).
-
-It will then copy the tree contained in the `STATIC_DIR` directory in the `OUTPUT_DIR`, as-is.
-
-staticjinja will be then initialized with the given `CONTEXTS` and Jinja's `GLOBALS`/`FILTERS`/`EXTENSIONS`,
-[webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) will be registered, and the actual rendering
-process is started.
-
-`.html`, `.xml`, `.rss`, `.atom` and `.json` template output will be automatically minified, according to the `MINIFY_XML`
-and `MINIFY_JSON` configuration values.
-
-#### `staticjinjaplus clean`
-
-Delete and recreate the `OUTPUT_DIR` directory.
-
-#### `staticjinjaplus publish`
-
-> [!NOTE]
-> This feature requires a Linux-like environment.
-
-Apply configuration values override from [environment variables](#environment-variables), then successively run
-`staticjinjaplus build` and `staticjinjaplus clean` prior remotely syncing the `OUTPUT_DIR` directory content using
-`rsync` through SSH.
-
-#### `staticjinjaplus serve`
-
-Serve the `OUTPUT_DIR` directory using Python's built-in HTTP server, plus a couple improvements:
-
-  - URL rewrite for HTML files is emulated, i.e. both `/about.html` and `/about` will work
-  - Custom HTTP error pages are emulated, if they are found saved as `{status code}.html` in the output directory
-  - The server will listen to both IPv4 *and* IPv6 loopback addresses if possible
-
-By default, you can browse your generated site at http://localhost:8080/ or http://[::1]:8080/. Port can be changed
-by defining the `SERVE_PORT` [configuration value](#configpy).
-
-## Configuration
-
-### `config.py`
-
-Your project's configuration happens in a single `config.py` file in the root directory (where the `staticjinjaplus`
-CLI should be executed). You'll find the available configuration values below.
-
-> [!NOTE]
->   - All paths are relative to the root directory, unless otherwise stated.
->   - None of these configuration values are required, so is `config.py`.
->   - Only uppercase variables are loaded by staticjinjaplus.
-
-| Name             | Type                                            | Default                          | Description                                                                                                                                                                                                                                                                            |
-|------------------|-------------------------------------------------|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `LOCALE`         | List[str]                                       | `None`                           | Locale identifiers passed to [`locale.setlocale()`](https://docs.python.org/3.12/library/locale.html#locale.setlocale) before a build is executed. The first working identifier will be used                                                                                           |
-| `SERVE_PORT`     | int                                             | `8080`                           | Listening port of the HTTP server started by `staticjinjaplus serve`                                                                                                                                                                                                                   |
-| `BASE_URL`       | str                                             | `http://localhost:{SERVE_PORT}/` | Protocol and domain name to use to generate meaningful absolute URLs. Set host part to `[::1]` if you plan to use IPv6                                                                                                                                                                 |
-| `MINIFY_XML`     | bool                                            | `False`                          | Enable XML minification                                                                                                                                                                                                                                                                |
-| `MINIFY_JSON`    | bool                                            | `False`                          | Enable JSON minification                                                                                                                                                                                                                                                               |
-| `TEMPLATES_DIR`  | str                                             | `templates`                      | Directory containing the Jinja templates to be processed                                                                                                                                                                                                                               |
-| `OUTPUT_DIR`     | str                                             | `output`                         | Directory where the rendered site will be saved                                                                                                                                                                                                                                        |
-| `STATIC_DIR`     | str                                             | `static`                         | Directory containing static files                                                                                                                                                                                                                                                      |
-| `ASSETS_DIR`     | str                                             | `assets`                         | Directory containing assets, i.e. files that needs prior processing before being able to be used by the rendered site                                                                                                                                                                  |
-| `ASSETS_BUNDLES` | List[Tuple[str, Tuple[str,...], Dict[str, str]] | `[]`                             | [webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) to be registered. These are passed to [`register()`](https://webassets.readthedocs.io/en/latest/environment.html#registering-bundles). Sources are relative to `ASSETS_DIR`, destinations to `OUTPUT_DIR` |
-| `CONTEXTS`       | List[Tuple[str, Any]]                           | `[]`                             | [staticjinja contexts](https://staticjinja.readthedocs.io/en/stable/user/advanced.html#loading-data) to be used by templates                                                                                                                                                           |
-| `GLOBALS`        | Dict                                            | `{}`                             | [jinja globals](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.globals) to be made available in all templates                                                                                                                                                      |
-| `FILTERS`        | Dict                                            | `{}`                             | [jinja filters](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.filters) to be made available in all templates                                                                                                                                                      |
-| `EXTENSIONS`     | List[Union[str, jinja2.ext.Extension]]          | `[]`                             | [jinja extensions](https://jinja.palletsprojects.com/en/3.1.x/extensions/) to load                                                                                                                                                                                                     |
-
-### Environment variables
-
-Some configuration values may/must be overridden by environment variables of the same name when publishing your site
-(`staticjinjaplus publish` command), typically in a deployment environment. You'll find the list below.
-
-| Name          | Type   | Required?                      | Default                           | Description                                                          |
-|---------------|--------|--------------------------------|-----------------------------------|----------------------------------------------------------------------|
-| `BASE_URL`    | str    | Yes                            |                                   | Protocol and domain name to use to generate meaningful absolute URLs |
-| `MINIFY_XML`  | bool ¹ | No, but activation recommended | `MINIFY_XML` configuration value  | Enable XML minification                                              |
-| `MINIFY_JSON` | bool ¹ | No, but activation recommended | `MINIFY_JSON` configuration value | Enable JSON minification                                             |
-| `SSH_USER`    | str    | Yes                            |                                   | SSH username                                                         |
-| `SSH_HOST`    | str    | Yes                            |                                   | SSH hostname                                                         |
-| `SSH_PORT`    | int    | No                             | `22`                              | SSH port                                                             |
-| `SSH_PATH`    | str    | Yes                            |                                   | Absolute path to the deployment directory on the SSH host            |
-
-¹ Any [falsy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.falsy) or
-[truthy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.truthy) string
-representation of boolean values allowed by marshmallow
-
-## Development
-
-### Getting source code and installing the package with dev dependencies
-
-  1. Clone the repository
-  2. From the root directory, run: `pip install -e .[dev]` on Linux or `pip install -e ".[dev]"` on Windows
-
-### Releasing the package
-
-From the root directory, run `python setup.py upload`. This will build the package, create a git tag and publish on PyPI.
-
-`__version__` in `staticjinjaplus/__version__.py` must be updated beforehand. It should adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-
-An associated GitHub release must be created following the [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format.
+Metadata-Version: 2.1
+Name: staticjinjaplus
+Version: 2.0.0
+Summary: A sweet spot between staticjinja and a full-blown static site generator.
+Home-page: https://github.com/EpocDotFr/staticjinjaplus
+Author: Maxime "Epoc" Gross
+Author-email: contact.nospam@epoc.nospam.fr
+License: DBAD
+Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme
+Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
+Project-URL: Tracker, https://github.com/EpocDotFr/staticjinjaplus/issues
+Project-URL: Changelog, https://github.com/EpocDotFr/staticjinjaplus/releases
+Keywords: static,website,site,generator,staticjinja,jinja,jinja2
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: staticjinja~=5.0
+Requires-Dist: webassets~=2.0
+Requires-Dist: htmlmin~=0.1
+Requires-Dist: cssutils~=2.10
+Requires-Dist: jsmin~=3.0
+Requires-Dist: environs~=11.0
+Requires-Dist: markdown~=3.6
+Provides-Extra: dev
+Requires-Dist: build~=1.2; extra == "dev"
+Requires-Dist: twine~=5.0; extra == "dev"
+Requires-Dist: setuptools~=69.5; extra == "dev"
+
+
+# staticjinjaplus
+
+A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
+
+![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
+
+[PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
+
+Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
+I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
+order to be able to generate a static website that will actually be ready for real world usage.
+
+staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
+Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
+static site generator.
+
+## Features
+
+All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
+
+  - Simple, file-based configuration to centralize *a handful* of configuration values
+  - Generic Markdown support (**not** your usual "pages" or "articles/blog posts" feature)
+  - Build improvements
+    - Automatically copy static files to output directory
+    - Define Jinja and staticjinja initialization parameters in a config file
+    - Define [webassets](https://webassets.readthedocs.io/en/latest/) bundles to allow CSS/JS concatenation/minification
+    - Automatically minify XML (including HTML, RSS and Atom)/JSON output
+  - Jinja improvements
+    - A few new Jinja globals/filters to make your life easier
+    - Autoescape is enabled for XML, HTML, RSS and Atom templates
+  - Serve the generated site through a local HTTP server
+    - URL rewrite emulation (for HTML files)
+    - Custom HTTP error pages emulation
+    - IPv6 loopback address support
+    - Serve proper MIME type for RSS and Atom files
+  - Publish the generated site through rsync over SSH
+
+**Planned:**
+
+  - Rebuild site on assets/static files change
+  - Generic i18n and l10n support (powered by Babel)
+
+## Prerequisites
+
+  - Python >= 3.10
+
+## Installation
+
+From PyPI:
+
+```bash
+$ pip install staticjinjaplus
+```
+
+Locally, after cloning/downloading the repo:
+
+```bash
+$ pip install .
+```
+
+A CLI (`staticjinjaplus`) will be made available upon installation.
+
+## Usage
+
+### Templates
+
+You'll want to write your site's Jinja templates first: write them as usual. By default, staticjinjaplus searches for
+Jinja templates in the `templates` directory where it is invoked. You can change that by using the `TEMPLATES_DIR`
+[configuration value](#configpy).
+
+Remember staticjinjaplus still stick with staticjinja's idiom: one Jinja template equal one rendered file, nothing more,
+nothing less.
+
+> [!WARNING]
+> HTML templates which extension is not `.html` will **not** be properly handled by staticjinjaplus for the sake of
+> simplicity. Please use `.html` only.
+
+staticjinjaplus offers the following additional Jinja facilities.
+
+#### Globals
+
+| Name/signature                              | Type                 | Description                                                                                                                                                                                                                         |
+|---------------------------------------------|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `config`                                    | Dict[str, Any]       | Configuration values loaded from [`config.py`](#configpy) (defaults are guaranteed to be provided for built-in values). Only uppercase variables are loaded by staticjinjaplus                                                      |
+| `absurl(resource: str) -> str`              | Callable             | Build an absolute URL relative to a file located in the `OUTPUT_DIR` directory. The resource path is prefixed by `BASE_URL` (see [configuration values](#configpy))                                                                 |
+| `embed(filename: str) -> markupsafe.Markup` | Callable             | Return the file content of the given file, marked as safe to be rendered by Jinja. `filename` is relative to the `{ASSETS_DIR}` directory. Useful to e.g embed SVG icons directly in the generated HTML                             |
+| `collected`                                 | List[Dict[str, Any]] | List of all valid template files (as seen by staticjinja) found in the `TEMPLATES_DIR` directory. Dictionary include source filename, rendered template URL, file extension, and for Markdown (`.md`) files their parsed metadata. |
+
+**Usage examples:**
+
+```html+jinja
+{{ config.BASE_URL }}         {# http://localhost:8080/ (by default) #}
+{{ config.MY_CUSTOM_CONFIG }} {# Whatever you defined in your config.py (uppercase variables only) #}
+
+{# absurl() doesn't care whether an extension is given or not #}
+{{ absurl('/about.html') }} {# http://localhost:8080/about.html #}
+{{ absurl('/about') }}      {# http://localhost:8080/about #}
+{{ absurl('about') }}       {# http://localhost:8080/about #}
+
+{# absurl() doesn't care about whether a static file is targeted or not #}
+{{ absurl('/images/logo.png') }} {# http://localhost:8080/images/logo.png #}
+{{ absurl('images/logo.png') }}  {# http://localhost:8080/images/logo.png #}
+
+{{ embed('icons/github.svg') }} {# <svg xmlns="http://www.w3.org/2000/svg" ... </svg> #}
+
+{{ collected }}
+{#
+    [
+      {'source': 'index.html', 'type': 'html', url': '/'},
+      {'source': 'site/about.html', 'type': 'html', 'url': '/site/about.html'},
+      {'source': 'categories/index.html', 'type': 'html', 'url': '/categories/'},
+      {'source': 'woah.md', 'type': 'md', 'url': '/woah.html', 'meta': { ... }},
+      {'source': 'index.md', 'type': 'md', 'url': '/', 'meta': { ... }},
+      {'source': 'blog/an-article.md', 'type': 'md', 'url': '/blog/an-article.html', 'meta': { ... }},
+      {'source': 'blog/index.md', 'type': 'md', 'url': '/blog/', 'meta': { ... }}
+    ]
+#}
+```
+
+#### Filters
+
+| Signature                                      | Description                                                                                                                                                                                                                                                         |
+|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `<data: Dict>\|tojsonm -> markupsafe.Markup`   | Serialize the given dictionary to a JSON string. Automatically takes into account the `MINIFY_JSON` [configuration value](#configpy) to minify (or not) the resulting output. Useful for e.g serializing [Schema.org](https://schema.org/)'s JSON-LD-formatted data |
+| `<left: Dict>\|dictmerge(right: Dict) -> Dict` | Merge two dictionaries. Does not modify existing ones, a new one will be created. Does **not** merge deeply                                                                                                                                                         |
+
+**Usage examples:**
+
+```html+jinja
+{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == False:
+                                 {
+                                     "yes": true
+                                 }
+                             #}
+
+{{ dict(yes=True)|tojsonm }} {# With config['MINIFY_JSON'] == True:
+                                 {"yes":true}
+                             #}
+
+{{ dict(yes=True)|dictmerge(dict(no=False)) }} {# {"yes": True, "no": False} #}
+```
+
+#### Markdown
+
+> [!WARNING]
+> Markdown templates which extension is not `.md` will **not** be properly handled by staticjinjaplus for the sake of
+> simplicity. Please use `.md` only.
+
+staticjinjaplus has generic support for working with Markdown-formatted files. Write your Markdown files (`.md`) as usual
+in the `TEMPLATES_DIR` directory: they will be rendered to HTML using the appropriate template partial, and saved using
+the source root pathname to the `OUTPUT_DIR` directory; i.e. `{TEMPLATES_DIR}/blog/awesome.md` will be rendered to
+`{OUTPUT_DIR}/blog/awesome.html`.
+
+staticjinjaplus do read metadata fields of Markdown files. Supported syntax is documented [here](https://python-markdown.github.io/extensions/meta_data/#syntax).
+The only reserved metadata field is `partial`, which tells staticjinjaplus which template partial (relative to the
+`TEMPLATES_DIR` directory) to use when rendering the Markdown file. See example below.
+
+It fallbacks to the `MARKDOWN_DEFAULT_PARTIAL` [configuration value](#configpy) if the field was not found. An error will
+be logged if staticjinjaplus can't determine which template partial to use, and rendering of the Markdown file will be
+canceled.
+
+This template partial will be given a Markdown-specific variable named `markdown` containing a dictionary which keys and
+values are detailed below.
+
+| Name                 | Type              | Description                                                                                                            |
+|----------------------|-------------------|------------------------------------------------------------------------------------------------------------------------|
+| `markdown.converted` | markupsafe.Markup | The resulting HTML, marked as safe to be rendered by Jinja. Metadata are of course not included in this output         |
+| `markdown.source`    | str               | The Markdown template filename                                                                                         |
+| `markdown.url`       | str               | The rendered Markdown template URL                                                                                     |
+| `markdown.meta`      | Dict[str, str]    | Metadata parsed from the source Markdown file. Multiline values have been concatenated using `\n` without extra spaces |
+
+Internal URLs must be written using the rendered version of the templates/assets/static files, i.e. URLs relative to what
+will be rendered in the `OUTPUT_DIR` directory. staticjinjaplus will not rewrite any URLs in any manner: you must provide
+the right ones by yourself. See example below.
+
+See also the `collected` [Jinja global](#globals) which contain - among others - all Markdown files found in the
+`TEMPLATES_DIR` directory (as seen by staticjinja) along their parsed metadata, and more.
+
+**Example Markdown file:**
+
+```markdown
+partial: blog/_post.html
+
+My awesome blog post. It has internal [links](/blog/my-article.html), and one image:
+
+![](/images/attachment.png)
+
+This image may come from the `STATIC_DIR` directory.
+```
+
+### Command line interface
+
+The `staticjinjaplus` CLI is your main and only way to interact with staticjinjaplus. The following commands are available.
+
+#### `staticjinjaplus build`
+
+Build the site by rendering your templates from the `TEMPLATES_DIR` directory in the `OUTPUT_DIR` directory.
+
+**Options:**
+
+  - `-w, --watch` Automatically rebuild the site when templates are modified. **This option does not watch for assets or static files changes (yet?)**
+
+It will then copy the tree contained in the `STATIC_DIR` directory in the `OUTPUT_DIR`, as-is.
+
+staticjinja will be then initialized with the given `CONTEXTS` and Jinja's `JINJA_GLOBALS`/`JINJA_FILTERS`/`JINJA_EXTENSIONS`,
+[webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) (`WEBASSETS_BUNDLES`) will be registered, and
+the actual rendering process is started.
+
+`.html`, `.xml`, `.rss`, `.atom` and `.json` template output will be automatically minified, according to the `MINIFY_XML`
+and `MINIFY_JSON` configuration values. `.md` files will be converted to HTML and rendered using the appropriate template
+partial, which output will be automatically minified as well if configured so.
+
+#### `staticjinjaplus clean`
+
+Delete and recreate the `OUTPUT_DIR` directory.
+
+#### `staticjinjaplus publish`
+
+> [!NOTE]
+> This feature requires a Linux-like environment.
+
+Apply configuration values override from [environment variables](#environment-variables), then successively run
+`staticjinjaplus clean` and `staticjinjaplus build` prior remotely syncing the `OUTPUT_DIR` directory content using
+`rsync` through SSH.
+
+#### `staticjinjaplus serve`
+
+Serve the `OUTPUT_DIR` directory using Python's built-in HTTP server, plus a couple improvements:
+
+  - URL rewrite for HTML files is emulated, i.e. both `/about.html` and `/about` will work
+  - Custom HTTP error pages are emulated, if they are found saved as `{status code}.html` in the output directory
+  - The server will listen to both IPv4 *and* IPv6 loopback addresses if possible
+  - RSS and Atom files will be served using the appropriate MIME type in the `Content-Type` response header
+
+By default, you can browse your generated site at http://localhost:8080/ or [http://[::1]:8080/](http://[::1]:8080/).
+Port can be changed by defining the `SERVE_PORT` [configuration value](#configpy).
+
+## Configuration
+
+### `config.py`
+
+Your project's configuration happens in a single `config.py` file in the root directory (where the `staticjinjaplus`
+CLI should be executed). You'll find the available configuration values below.
+
+> [!NOTE]
+>   - All paths are relative to the root directory, unless otherwise stated.
+>   - None of these configuration values are required, so is `config.py`.
+>   - Only uppercase variables are loaded by staticjinjaplus.
+
+| Name                       | Type                                              | Default                          | Description                                                                                                                                                                                                                                                                                                                           |
+|----------------------------|---------------------------------------------------|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `SERVE_PORT`               | int                                               | `8080`                           | Listening port of the HTTP server started by `staticjinjaplus serve`                                                                                                                                                                                                                                                                  |
+| `BASE_URL`                 | str                                               | `http://localhost:{SERVE_PORT}/` | Protocol and domain name to use to generate meaningful absolute URLs. Set host part to `[::1]` if you plan to use IPv6                                                                                                                                                                                                                |
+| `MINIFY_XML`               | bool                                              | `False`                          | Enable XML minification                                                                                                                                                                                                                                                                                                               |
+| `MINIFY_JSON`              | bool                                              | `False`                          | Enable JSON minification                                                                                                                                                                                                                                                                                                              |
+| `TEMPLATES_DIR`            | str                                               | `templates`                      | Directory containing the Jinja templates to be processed                                                                                                                                                                                                                                                                              |
+| `OUTPUT_DIR`               | str                                               | `output`                         | Directory where the rendered site will be saved                                                                                                                                                                                                                                                                                       |
+| `STATIC_DIR`               | str                                               | `static`                         | Directory containing static files                                                                                                                                                                                                                                                                                                     |
+| `ASSETS_DIR`               | str                                               | `assets`                         | Directory containing assets, i.e. files that needs prior processing before being able to be used by the rendered site                                                                                                                                                                                                                 |
+| `CONTEXTS`                 | List[Tuple[str, Union[Dict[str, Any], Callable]]] | `[]`                             | [staticjinja contexts](https://staticjinja.readthedocs.io/en/stable/user/advanced.html#loading-data) to be used by templates                                                                                                                                                                                                          |
+| `WEBASSETS_BUNDLES`        | List[Tuple[str, Tuple[str,...], Dict[str, str]]   | `[]`                             | [webassets bundles](https://webassets.readthedocs.io/en/latest/bundles.html) to be registered. These are passed to [`register()`](https://webassets.readthedocs.io/en/latest/environment.html#registering-bundles). Sources are relative to `ASSETS_DIR`, destinations to `OUTPUT_DIR`                                                |
+| `JINJA_GLOBALS`            | Dict[str, Any]                                    | `{}`                             | [jinja globals](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.globals) to be made available in all templates                                                                                                                                                                                                     |
+| `JINJA_FILTERS`            | Dict[str, Callable]                               | `{}`                             | [jinja filters](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment.filters) to be made available in all templates                                                                                                                                                                                                     |
+| `JINJA_EXTENSIONS`         | List[Union[str, jinja2.ext.Extension]]            | `[]`                             | [jinja extensions](https://jinja.palletsprojects.com/en/3.1.x/extensions/) to load                                                                                                                                                                                                                                                    |
+| `MARKDOWN_EXTENSIONS`      | Dict[str, Dict]                                   | `{}`                             | [Markdown extensions](https://python-markdown.github.io/extensions/) to load and their respective configuration. Keys are passed to [`extensions`](https://python-markdown.github.io/reference/#extensions); the entire dictionary is passed to [`extension_configs`](https://python-markdown.github.io/reference/#extension_configs) |
+| `MARKDOWN_DEFAULT_PARTIAL` | Optional[str]                                     | `None`                           | Default template partial to use when rendering Markdown files when the `partial` metadata is not present                                                                                                                                                                                                                              |
+| `USE_HTML_EXTENSION`       | bool                                              | `True`                           | If your site's links are using URLs without `.html` extension (URL rewrite), you must set this config value to `False`. This config value does **not** alter the behavior of `absurl()` in any way                                                                                                                                    |
+
+### Environment variables
+
+Some configuration values may/must be overridden by environment variables of the same name when publishing your site
+(`staticjinjaplus publish` command), typically in a deployment environment. You'll find the list below.
+
+| Name          | Type   | Required?                      | Default                           | Description                                                          |
+|---------------|--------|--------------------------------|-----------------------------------|----------------------------------------------------------------------|
+| `BASE_URL`    | str    | Yes                            |                                   | Protocol and domain name to use to generate meaningful absolute URLs |
+| `MINIFY_XML`  | bool ¹ | No, but activation recommended | `MINIFY_XML` configuration value  | Enable XML minification                                              |
+| `MINIFY_JSON` | bool ¹ | No, but activation recommended | `MINIFY_JSON` configuration value | Enable JSON minification                                             |
+| `SSH_USER`    | str    | Yes                            |                                   | SSH username                                                         |
+| `SSH_HOST`    | str    | Yes                            |                                   | SSH hostname                                                         |
+| `SSH_PORT`    | int    | No                             | `22`                              | SSH port                                                             |
+| `SSH_PATH`    | str    | Yes                            |                                   | Absolute path to the deployment directory on the SSH host            |
+
+¹ Any [falsy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.falsy) or
+[truthy](https://marshmallow.readthedocs.io/en/stable/marshmallow.fields.html#marshmallow.fields.Boolean.truthy) string
+representation of boolean values allowed by marshmallow
+
+## Development
+
+### Getting source code and installing the package with dev dependencies
+
+  1. Clone the repository
+  2. From the root directory, run: `pip install -e .[dev]` on Linux or `pip install -e ".[dev]"` on Windows
+
+### Releasing the package
+
+From the root directory, run `python setup.py upload`. This will build the package, create a git tag and publish on PyPI.
+
+`__version__` in `staticjinjaplus/__version__.py` must be updated beforehand. It should adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+An associated GitHub release must be created following the [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format.
```

