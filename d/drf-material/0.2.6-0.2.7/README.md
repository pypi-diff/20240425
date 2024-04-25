# Comparing `tmp/drf_material-0.2.6.tar.gz` & `tmp/drf_material-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_material-0.2.6.tar", max compression
+gzip compressed data, was "drf_material-0.2.7.tar", max compression
```

## Comparing `drf_material-0.2.6.tar` & `drf_material-0.2.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-03-14 12:03:31.504243 drf_material-0.2.6/LICENSE
--rw-r--r--   0        0        0     2906 2024-03-14 12:03:31.504243 drf_material-0.2.6/README.md
--rw-r--r--   0        0        0       87 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/__init__.py
--rw-r--r--   0        0        0      235 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/apps.py
--rw-r--r--   0        0        0    23331 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1059 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      613 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1373 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1411 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      962 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1481 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1077 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     3638 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1926 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      298 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1455 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1473 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-03-14 12:03:31.504243 drf_material-0.2.6/drf_material/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-03-14 12:03:31.508243 drf_material-0.2.6/drf_material/templatetags/__init__.py
--rw-r--r--   0        0        0     1681 2024-03-14 12:03:31.508243 drf_material-0.2.6/drf_material/templatetags/rest_framework_material.py
--rw-r--r--   0        0        0      548 2024-03-14 12:03:31.508243 drf_material-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 drf_material-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-25 17:30:29.707480 drf_material-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3012 2024-04-25 17:30:29.707480 drf_material-0.2.7/README.md
+-rw-r--r--   0        0        0       87 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/apps.py
+-rw-r--r--   0        0        0    23233 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1052 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      606 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1373 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1411 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      962 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1481 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1077 2024-04-25 17:30:29.707480 drf_material-0.2.7/drf_material/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     3631 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1926 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      298 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1455 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1473 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templatetags/__init__.py
+-rw-r--r--   0        0        0     1681 2024-04-25 17:30:29.711480 drf_material-0.2.7/drf_material/templatetags/rest_framework_material.py
+-rw-r--r--   0        0        0      548 2024-04-25 17:30:29.711480 drf_material-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3867 1970-01-01 00:00:00.000000 drf_material-0.2.7/PKG-INFO
```

### Comparing `drf_material-0.2.6/LICENSE` & `drf_material-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/README.md` & `drf_material-0.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # 🎨 drf-material
 
-[![Pylint](https://github.com/youzarsiph/drf-material/actions/workflows/pylint.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/pylint.yml)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+[![Ruff](https://github.com/youzarsiph/drf-material/actions/workflows/ruff.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/ruff.yml)
 [![Django CI](https://github.com/youzarsiph/drf-material/actions/workflows/django.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/django.yml)
 [![Upload Python Package](https://github.com/youzarsiph/drf-material/actions/workflows/python-publish.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/python-publish.yml)
 
 **drf-material** is a project that gives a sleek and elegant look to the browsable API of Django REST Framework using Material Design.
 
 We want to make the API more **appealing** and **intuitive** for developers and users alike.
 That's why we created a **beautiful** and **responsive** design that follows the Material Design principles and guidelines.
@@ -19,15 +20,15 @@
 
 - **Modern design**: drf-material uses Material Design, a design system based on Google's Material Design and
   Bootstrap's components, to create a sleek and elegant design for the API.
 - **Accessibility**: drf-material follows the best practices for web accessibility,
   ensuring that the API is easy to use for everyone, regardless of their abilities or preferences.
 - **Form input max length indicators**: drf-material shows the maximum length of each form input field,
   so you know how much data you can enter. The indicators also change color when you reach the limit, giving you visual feedback.
-- **Form inputs required indicators**: drf-material marks the required form input fields with an asterisk (*),
+- **Form inputs required indicators**: drf-material marks the required form input fields with an asterisk (\*),
   so you know which fields are mandatory to submit the form. The indicators also show an error message if you try to submit the form without filling the required fields.
 - **Browser form validation**: drf-material uses the built-in browser form validation features, such as HTML5 attributes
   to validate the form input data before sending it to the server. The validation checks for data types, formats, patterns, ranges, and more.
 
 ## 🛠️ Get started
 
 To use drf-material, follow these simple steps:
```

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/api.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/api.html`

 * *Files 2% similar despite different names*

```diff
@@ -171,23 +171,23 @@
     <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4"
       aria-label="{% translate 'Request form' %}">
       {% if 'GET' in allowed_methods %}
         <form id="get-form">
           <fieldset>
             {% if api_settings.URL_FORMAT_OVERRIDE %}
             <div class="btn-group w-100 gap-4 rounded-5" role="group">
-              <a class="btn btn-lg btn-primary w-100 rounded-5" href="{{ request.get_full_path }}" rel="nofollow"
+              <a class="btn btn-primary w-100 rounded-5" href="{{ request.get_full_path }}" rel="nofollow"
                 title="Make a GET request on the {{ name }} resource" data-mdb-toggle="tooltip">
                 <span class="d-flex align-items-center justify-content-center gap-4">
                   <i class="bi bi-arrow-clockwise"></i>
                   {% translate "GET" %}
                 </span>
               </a>
               <div class="dropdown">
-                <button class="btn btn-lg btn-outline-primary dropdown-toggle rounded-5" type="button" id="dropdownMenuButton"
+                <button class="btn btn-outline-primary dropdown-toggle rounded-5" type="button" id="dropdownMenuButton"
                   data-mdb-toggle="dropdown" aria-expanded="false">
                   <i class="bi bi-chevron-down"></i>
                 </button>
                 <ul class="dropdown-menu dropdown-menu-end rounded-5 shadow-sm w-100" aria-labelledby="dropdownMenuButton">
                   <li>
                     <h6 class="dropdown-header">
                       {% translate 'Select a format' %}
@@ -202,41 +202,41 @@
                     </a>
                   </li>
                   {% endfor %}
                 </ul>
               </div>
             </div>
             {% else %}
-            <a class="btn btn-lg btn-primary rounded-5" href="{{ request.get_full_path }}" rel="nofollow"
+            <a class="btn btn-primary rounded-5" href="{{ request.get_full_path }}" rel="nofollow"
               title="Make a GET request on the {{ name }} resource" data-mdb-toggle="tooltip">
               <span class="d-flex align-items-center justify-content-center gap-4">
                 <i class="bi bi-arrow-clockwise"></i>
                 {% translate "GET" %}
               </span>
             </a>
             {% endif %}
           </fieldset>
         </form>
       {% endif %}
 
       {% if options_form %}
         <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
-          <button type="submit" class="btn btn-lg btn-dark w-100 rounded-5"
+          <button type="submit" class="btn btn-info w-100 rounded-5"
             title="Make an OPTIONS request on the {{ name }} resource" data-mdb-toggle="tooltip">
             <span class="d-flex align-items-center justify-content-center gap-4">
               <i class="bi bi-info-square"></i>
               {% translate "OPTIONS" %}
             </span>
           </button>
         </form>
       {% endif %}
 
       {% if delete_form %}
         <div>
-          <button type="button" class="btn btn-lg btn-danger w-100 rounded-5" data-mdb-toggle="modal"
+          <button type="button" class="btn btn-danger w-100 rounded-5" data-mdb-toggle="modal"
             data-mdb-target="#deleteModal" title="Make a DELETE request on the {{ name }} resource">
             <span class="d-flex align-items-center justify-content-center gap-4">
               <i class="bi bi-trash"></i>
               {% translate "DELETE" %}
             </span>
           </button>
         </div>
@@ -252,37 +252,37 @@
               </div>
               <div class="modal-body">
                 <p class="mb-4">
                   {% translate "Are you sure you want to delete this" %} {{ name }}?
                 </p>
                 <div class="d-grid d-lg-flex align-items-lg-center gap-4">
                   <form class="button-form w-100" action="{{ request.get_full_path }}" data-method="DELETE">
-                    <button class="btn btn-lg btn-danger w-100 rounded-5">
+                    <button class="btn btn-danger w-100 rounded-5">
                       <span class="d-flex align-item-center justify-content-center gap-4">
                         <i class="bi bi-trash"></i>
                         {% translate "Delete" %}
                       </span>
                     </button>
                   </form>
-                  <button type="button" class="btn btn-lg btn-outline-secondary w-100 rounded-5" data-mdb-dismiss="modal">
+                  <button type="button" class="btn btn-outline-secondary w-100 rounded-5" data-mdb-dismiss="modal">
                     <span class="d-flex align-item-center justify-content-center gap-4">
                       <i class="bi bi-x-lg"></i>
                       {% translate "Cancel" %}
                     </span>
                   </button>
                 </div>
               </div>
             </div>
           </div>
         </div>
       {% endif %}
 
       {% if extra_actions %}
         <div class="dropdown">
-          <button class="btn btn-lg btn-info w-100 rounded-5" id="extra-actions-menu" data-mdb-toggle="dropdown"
+          <button class="btn btn-info w-100 rounded-5" id="extra-actions-menu" data-mdb-toggle="dropdown"
             aria-haspopup="true" aria-expanded="true">
             <span class="d-flex align-items-center justify-content-center gap-4">
               {% translate "Extra Actions" %}
               <i class="bi bi-chevron-down"></i>
             </span>
           </button>
           <ul class="dropdown-menu rounded-5 shadow-sm w-100" aria-labelledby="extra-actions-menu">
@@ -299,15 +299,15 @@
             </li>
             {% endfor %}
           </ul>
         </div>
       {% endif %}
 
       {% if filter_form %}
-        <button data-mdb-toggle="modal" data-mdb-target="#filtersModal" class="btn btn-lg btn-success rounded-5">
+        <button data-mdb-toggle="modal" data-mdb-target="#filtersModal" class="btn btn-success rounded-5">
           <span class="d-flex align-items-center justify-content-center gap-4">
             <i class="bi bi-filter"></i>
             {% translate "Filters" %}
           </span>
         </button>
       {% endif %}
     </section>
@@ -365,15 +365,15 @@
                   <div class="tab-pane active" id="form" role="tabpanel" aria-labelledby="form-tab" tabindex="0">
                     {% with form=post_form %}
                     <form action="{{ request.get_full_path }}" method="POST" enctype="multipart/form-data" class="form-horizontal">
                       <fieldset>
                         {% csrf_token %}
                         {{ post_form }}
                         <div class="form-actions">
-                          <button class="btn btn-lg btn-primary w-100 rounded-5"
+                          <button class="btn btn-primary w-100 rounded-5"
                             title="Make a POST request on the {{ name }} resource" data-mdb-toggle="tooltip">
                             <span class="d-flex align-items-center justify-content-center gap-4">
                               <i class="bi bi-send-fill"></i>
                               {% translate "POST" %}
                             </span>
                           </button>
                         </div>
@@ -385,15 +385,15 @@
 
                 <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
                   {% with form=raw_data_post_form %}
                   <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
                     <fieldset>
                       {% include "rest_framework/raw_data_form.html" %}
                       <div class="form-actions">
-                        <button class="btn btn-lg btn-primary w-100 rounded-5"
+                        <button class="btn btn-primary w-100 rounded-5"
                           title="Make a POST request on the {{ name }} resource" data-mdb-toggle="tooltip">
                           <span class="d-flex align-items-center justify-content-center gap-4">
                             <i class="bi bi-send-fill"></i>
                             {% translate "POST" %}
                           </span>
                         </button>
                       </div>
@@ -438,15 +438,15 @@
               <div class="tab-content">
                 {% if put_form %}
                   <div class="tab-pane active" id="put-object-form">
                     <form action="{{ request.get_full_path }}" data-method="PUT" enctype="multipart/form-data" class="form-horizontal">
                       <fieldset>
                         {{ put_form }}
                         <div class="form-actions">
-                          <button class="btn btn-lg btn-primary w-100 rounded-5"
+                          <button class="btn btn-primary w-100 rounded-5"
                             title="Make a PUT request on the {{ name }} resource" data-mdb-toggle="tooltip">
                             <span class="d-flex align-items-center justify-content-center gap-4">
                               <i class="bi bi-send-fill"></i>
                               {% translate "PUT" %}
                             </span>
                           </button>
                         </div>
@@ -458,24 +458,24 @@
                 <div {% if put_form %}class="tab-pane" {% endif %} id="put-generic-content-form">
                   {% with form=raw_data_put_or_patch_form %}
                   <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
                     <fieldset>
                       {% include "rest_framework/raw_data_form.html" %}
                       <div class="form-actions">
                         {% if raw_data_put_form %}
-                        <button class="btn btn-lg btn-primary w-100 rounded-5"
+                        <button class="btn btn-primary w-100 rounded-5"
                           title="Make a PUT request on the {{ name }} resource" data-mdb-toggle="tooltip">
                           <span class="d-flex align-items-center justify-content-center gap-4">
                             <i class="bi bi-send-fill"></i>
                             {% translate "PUT" %}
                           </span>
                         </button>
                         {% endif %}
                         {% if raw_data_patch_form %}
-                        <button data-method="PATCH" class="btn btn-lg btn-outline-primary w-100 mt-4 rounded-5"
+                        <button data-method="PATCH" class="btn btn-outline-primary w-100 mt-4 rounded-5"
                           title="Make a PATCH request on the {{ name }} resource" data-mdb-toggle="tooltip">
                           <span class="d-flex align-items-center justify-content-center gap-4">
                             <i class="bi bi-send-fill"></i>
                             {% translate "PATCH" %}
                           </span>
                         </button>
                         {% endif %}
```

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/filters/base.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/filters/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       <div class="modal-body">
         <div class="d-grid gap-4">
           {% for element in elements %}
           <div>
             {{ element }}
           </div>
           {% endfor %}
-          <button type="button" class="btn btn-lg btn-outline-secondary rounded-5" data-mdb-dismiss="modal">
+          <button type="button" class="btn btn-outline-secondary rounded-5" data-mdb-dismiss="modal">
             <span class="d-flex align-item-center justify-content-center gap-4">
               <i class="bi bi-x-lg"></i>
               {% translate "Cancel" %}
             </span>
           </button>
         </div>
       </div>
```

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/filters/ordering.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/filters/search.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/filters/search.html`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       <input
         type="search"
         class="form-control form-control-lg"
         name="{{ param }}"
         value="{{ term }}"
         placeholder="{% translate 'Type here to search...' %}"
       />
-      <button class="btn btn-lg btn-outline-primary" type="submit">
+      <button class="btn btn-outline-primary" type="submit">
         <span class="d-flex align-items-center gap-4">
           <i class="bi bi-search"></i>
           {% translate "Search" %}
         </span>
       </button>
     </div>
   </div>
```

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/checkbox.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/input.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/radio.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/select.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/select_multiple.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/horizontal/textarea.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/checkbox.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/checkbox_multiple.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/input.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/radio.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/select.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/select_multiple.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/inline/textarea.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/login.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/login.html`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
               {% if form.non_field_errors %}
               {% for error in form.non_field_errors %}
               <div class="alert alert-danger" role="alert">{{ error }}</div>
               {% endfor %}
               {% endif %}
 
-              <button type="submit" class="btn btn-lg btn-primary w-100 rounded-5">
+              <button type="submit" class="btn btn-primary w-100 rounded-5">
                 <strong class="d-flex align-items-center justify-content-center gap-3">
                   <i class="bi bi-box-arrow-in-right"></i>
                   {% translate "Login" %}
                 </strong>
               </button>
             </form>
           </main>
```

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/pagination/numbers.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/pagination/previous_and_next.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/checkbox.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/input.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/radio.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/select.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/select_multiple.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templates/rest_framework/vertical/textarea.html` & `drf_material-0.2.7/drf_material/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/drf_material/templatetags/rest_framework_material.py` & `drf_material-0.2.7/drf_material/templatetags/rest_framework_material.py`

 * *Files identical despite different names*

### Comparing `drf_material-0.2.6/pyproject.toml` & `drf_material-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-material"
-version = "0.2.6"
+version = "0.2.7"
 description = "Material design for Django REST Framework API"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_material"}]
 homepage = "https://github.com/youzarsiph/drf-material/"
 repository = "https://github.com/youzarsiph/drf-material/"
```

### Comparing `drf_material-0.2.6/PKG-INFO` & `drf_material-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-material
-Version: 0.2.6
+Version: 0.2.7
 Summary: Material design for Django REST Framework API
 Home-page: https://github.com/youzarsiph/drf-material/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,16 @@
 Requires-Dist: django (>=3.0)
 Requires-Dist: djangorestframework (>=3.14)
 Project-URL: Repository, https://github.com/youzarsiph/drf-material/
 Description-Content-Type: text/markdown
 
 # 🎨 drf-material
 
-[![Pylint](https://github.com/youzarsiph/drf-material/actions/workflows/pylint.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/pylint.yml)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+[![Ruff](https://github.com/youzarsiph/drf-material/actions/workflows/ruff.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/ruff.yml)
 [![Django CI](https://github.com/youzarsiph/drf-material/actions/workflows/django.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/django.yml)
 [![Upload Python Package](https://github.com/youzarsiph/drf-material/actions/workflows/python-publish.yml/badge.svg)](https://github.com/youzarsiph/drf-material/actions/workflows/python-publish.yml)
 
 **drf-material** is a project that gives a sleek and elegant look to the browsable API of Django REST Framework using Material Design.
 
 We want to make the API more **appealing** and **intuitive** for developers and users alike.
 That's why we created a **beautiful** and **responsive** design that follows the Material Design principles and guidelines.
@@ -41,15 +42,15 @@
 
 - **Modern design**: drf-material uses Material Design, a design system based on Google's Material Design and
   Bootstrap's components, to create a sleek and elegant design for the API.
 - **Accessibility**: drf-material follows the best practices for web accessibility,
   ensuring that the API is easy to use for everyone, regardless of their abilities or preferences.
 - **Form input max length indicators**: drf-material shows the maximum length of each form input field,
   so you know how much data you can enter. The indicators also change color when you reach the limit, giving you visual feedback.
-- **Form inputs required indicators**: drf-material marks the required form input fields with an asterisk (*),
+- **Form inputs required indicators**: drf-material marks the required form input fields with an asterisk (\*),
   so you know which fields are mandatory to submit the form. The indicators also show an error message if you try to submit the form without filling the required fields.
 - **Browser form validation**: drf-material uses the built-in browser form validation features, such as HTML5 attributes
   to validate the form input data before sending it to the server. The validation checks for data types, formats, patterns, ranges, and more.
 
 ## 🛠️ Get started
 
 To use drf-material, follow these simple steps:
```

