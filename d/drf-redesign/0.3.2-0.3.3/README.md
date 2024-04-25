# Comparing `tmp/drf_redesign-0.3.2.tar.gz` & `tmp/drf_redesign-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_redesign-0.3.2.tar", max compression
+gzip compressed data, was "drf_redesign-0.3.3.tar", max compression
```

## Comparing `drf_redesign-0.3.2.tar` & `drf_redesign-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/LICENSE
--rw-r--r--   0        0        0     3585 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/README.md
--rw-r--r--   0        0        0       91 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/__init__.py
--rw-r--r--   0        0        0      235 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/apps.py
--rw-r--r--   0        0        0    26938 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1063 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      592 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1398 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1433 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0     1006 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-03-14 11:55:22.410796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1487 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1054 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     5230 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     2065 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      296 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1461 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1474 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templatetags/__init__.py
--rw-r--r--   0        0        0     1682 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/drf_redesign/templatetags/rest_framework_redesign.py
--rw-r--r--   0        0        0      576 2024-03-14 11:55:22.414796 drf_redesign-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 drf_redesign-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3566 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/README.md
+-rw-r--r--   0        0        0       91 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/apps.py
+-rw-r--r--   0        0        0    26838 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1056 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      585 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1398 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1433 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0     1006 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1487 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1054 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     5226 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     2065 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      296 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1461 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1474 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templatetags/__init__.py
+-rw-r--r--   0        0        0     1682 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templatetags/rest_framework_redesign.py
+-rw-r--r--   0        0        0      576 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 drf_redesign-0.3.3/PKG-INFO
```

### Comparing `drf_redesign-0.3.2/LICENSE` & `drf_redesign-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/README.md` & `drf_redesign-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 🚀 drf-redesign
 
-[![Pylint](https://github.com/youzarsiph/drf-redesign/actions/workflows/pylint.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/pylint.yml)
-[![Upload Python Package](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml)
+[![Ruff](https://github.com/youzarsiph/drf-redesign/actions/workflows/ruff.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/ruff.yml)
+[![Publish](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml)
 [![Django CI](https://github.com/youzarsiph/drf-redesign/actions/workflows/django.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/django.yml)
 
 **drf-redesign** is a project that gives a fresh look to the browse-able API of Django REST Framework using Bootstrap 5.
 
 We want to make the API more **appealing** and **intuitive** for developers and users alike.
 That's why we created a **stylish** and **modern** design that makes the API easier to navigate and interact with.
 One of the coolest features of drf-redesign is the **dark mode** option.
@@ -25,15 +25,15 @@
   ensuring that the API is easy to use for everyone, regardless of their abilities or preferences.
 - **Light and dark themes**: drf-redesign lets you choose between a light or a dark color scheme for the API,
   depending on your mood or environment. You can switch between the themes with a simple click of a button.
 - **Bootstrap icons**: drf-redesign uses Bootstrap icons, a set of open source icons designed for Bootstrap components,
   to add some visual flair to the API. The icons are scalable, customizable, and easy to use.
 - **Form input max length indicators**: drf-redesign shows the maximum length of each form input field,
   so you know how much data you can enter. The indicators also change color when you reach the limit, giving you visual feedback.
-- **Form inputs required indicators**: drf-redesign marks the required form input fields with an asterisk (*),
+- **Form inputs required indicators**: drf-redesign marks the required form input fields with an asterisk (\*),
   so you know which fields are mandatory to submit the form. The indicators also show an error message if you try to submit the form without filling the required fields.
 - **Browser form validation**: drf-redesign uses the built-in browser form validation features, such as HTML5 attributes,
   to validate the form input data before sending it to the server. The validation checks for formats, patterns, ranges, and more.
 
 ## Images
 
 ![DRF Redesign Dark Mode](assets/img/drf-redesign-dark.jpeg)
```

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/api.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 {% block meta %}
   {{ block.super }}
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
-  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" 
-    integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
+      integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@latest/font/bootstrap-icons.css">
   {% endblock %}
 
   <style>
     {% if code_style %}
       {{ code_style }}
     {% endif %}
@@ -245,22 +245,22 @@
     {% block request_forms %}
       <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4" aria-label="{% translate 'Request form' %}">
         {% if 'GET' in allowed_methods %}
           <form id="get-form">
             <fieldset>
               {% if api_settings.URL_FORMAT_OVERRIDE %}
                 <div class="btn-group w-100" role="group">
-                  <a class="btn btn-lg btn-primary w-100 shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
+                  <a class="btn btn-primary w-100 shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
                     title="Make a GET request on the {{ name }} resource" data-bs-toggle="tooltip">
                     <span class="d-flex align-items-center justify-content-center gap-4">
                       <i class="bi bi-arrow-clockwise"></i>
                       {% translate "GET" %}
                     </span>
                   </a>
-                  <button class="btn btn-lg btn-outline-primary dropdown-toggle shadow-sm" type="button" id="dropdownMenuButton"
+                  <button class="btn btn-outline-primary dropdown-toggle shadow-sm" type="button" id="dropdownMenuButton"
                     data-bs-toggle="dropdown" aria-expanded="false">
                     <i class="bi bi-chevron-down"></i>
                   </button>
                   <div class="dropdown">
                     <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3 w-100" aria-labelledby="dropdownMenuButton">
                       <li>
                         <h6 class="dropdown-header">
@@ -276,40 +276,40 @@
                         </a>
                       </li>
                       {% endfor %}
                     </ul>
                   </div>
                 </div>
               {% else %}
-                <a class="btn btn-lg btn-primary shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
+                <a class="btn btn-primary shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
                   title="Make a GET request on the {{ name }} resource" data-bs-toggle="tooltip">
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
-            <button type="submit" class="btn btn-lg btn-secondary w-100 shadow-sm" title="Make an OPTIONS request on the {{ name }} resource" data-bs-toggle="tooltip">
+            <button type="submit" class="btn btn-info w-100 shadow-sm" title="Make an OPTIONS request on the {{ name }} resource" data-bs-toggle="tooltip">
               <span class="d-flex align-items-center justify-content-center gap-4">
                 <i class="bi bi-info-square"></i>
                 {% translate "OPTIONS" %}
               </span>
             </button>
           </form>
         {% endif %}
 
         {% if delete_form %}
           <div>
-            <button type="button" class="btn btn-lg btn-danger w-100 shadow-sm" data-bs-toggle="modal" data-bs-target="#deleteModal"
+            <button type="button" class="btn btn-danger w-100 shadow-sm" data-bs-toggle="modal" data-bs-target="#deleteModal"
               title="Make a DELETE request on the {{ name }} resource">
               <span class="d-flex align-items-center justify-content-center gap-4">
                 <i class="bi bi-trash"></i>
                 {% translate "DELETE" %}
               </span>
             </button>
           </div>
@@ -325,37 +325,37 @@
                 </div>
                 <div class="modal-body">
                   <p class="mb-4">
                     {% translate "Are you sure you want to delete this" %} {{ name }}?
                   </p>
                   <div class="d-grid d-lg-flex align-items-lg-center gap-4">
                     <form class="button-form w-100" action="{{ request.get_full_path }}" data-method="DELETE">
-                      <button class="btn btn-lg btn-danger w-100 shadow-sm">
+                      <button class="btn btn-danger w-100 shadow-sm">
                         <span class="d-flex align-item-center justify-content-center gap-4">
                           <i class="bi bi-trash"></i>
                           {% translate "Delete" %}
                         </span>
                       </button>
                     </form>
-                    <button type="button" class="btn btn-lg btn-outline-secondary w-100 shadow-sm" data-bs-dismiss="modal">
+                    <button type="button" class="btn btn-outline-secondary w-100 shadow-sm" data-bs-dismiss="modal">
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
-            <button class="btn btn-lg btn-info w-100 shadow-sm" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
+            <button class="btn btn-info w-100 shadow-sm" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
               <span class="d-flex align-items-center justify-content-center gap-4">
                 {% translate "Extra Actions" %}
                 <i class="bi bi-chevron-down"></i>
               </span>
             </button>
             <ul class="dropdown-menu rounded-4 shadow-sm pb-3 w-100" aria-labelledby="extra-actions-menu">
@@ -372,15 +372,15 @@
                 </li>
               {% endfor %}
             </ul>
           </div>
         {% endif %}
 
         {% if filter_form %}
-          <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-lg btn-success shadow-sm">
+          <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-success shadow-sm">
             <span class="d-flex align-items-center justify-content-center gap-4">
               <i class="bi bi-filter"></i>
               {% translate "Filters" %}
             </span>
           </button>
         {% endif %}
       </section>
@@ -437,15 +437,15 @@
                   <div class="tab-pane active" id="form" role="tabpanel" aria-labelledby="form-tab" tabindex="0">
                     {% with form=post_form %}
                       <form action="{{ request.get_full_path }}" method="POST" enctype="multipart/form-data" class="form-horizontal">
                         <fieldset>
                           {% csrf_token %}
                           {{ post_form }}
                           <div class="form-actions">
-                            <button class="btn btn-lg btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource" data-bs-toggle="tooltip">
+                            <button class="btn btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource" data-bs-toggle="tooltip">
                               <span class="d-flex align-items-center justify-content-center gap-4">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "POST" %}
                               </span>
                             </button>
                           </div>
                         </fieldset>
@@ -456,15 +456,15 @@
 
                 <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
                   {% with form=raw_data_post_form %}
                     <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
-                          <button class="btn btn-lg btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource" data-bs-toggle="tooltip">
+                          <button class="btn btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource" data-bs-toggle="tooltip">
                             <span class="d-flex align-items-center justify-content-center gap-4">
                               <i class="bi bi-send-fill"></i>
                               {% translate "POST" %}
                             </span>
                           </button>
                         </div>
                       </fieldset>
@@ -507,15 +507,15 @@
               <div class="tab-content">
                 {% if put_form %}
                   <div class="tab-pane active" id="put-object-form">
                     <form action="{{ request.get_full_path }}" data-method="PUT" enctype="multipart/form-data" class="form-horizontal">
                       <fieldset>
                         {{ put_form }}
                         <div class="form-actions">
-                          <button class="btn btn-lg btn-primary w-100 shadow-sm" title="Make a PUT request on the {{ name }} resource" data-bs-toggle="tooltip">
+                          <button class="btn btn-primary w-100 shadow-sm" title="Make a PUT request on the {{ name }} resource" data-bs-toggle="tooltip">
                             <span class="d-flex align-items-center justify-content-center gap-4">
                               <i class="bi bi-send-fill"></i>
                               {% translate "PUT" %}
                             </span>
                           </button>
                         </div>
                       </fieldset>
@@ -526,24 +526,24 @@
                 <div {% if put_form %}class="tab-pane"{% endif %} id="put-generic-content-form">
                   {% with form=raw_data_put_or_patch_form %}
                     <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
                           {% if raw_data_put_form %}
-                            <button class="btn btn-lg btn-primary w-100 shadow-sm"
+                            <button class="btn btn-primary w-100 shadow-sm"
                               title="Make a PUT request on the {{ name }} resource" data-bs-toggle="tooltip">
                               <span class="d-flex align-items-center justify-content-center gap-4">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "PUT" %}
                               </span>
                             </button>
                           {% endif %}
                           {% if raw_data_patch_form %}
-                            <button data-method="PATCH" class="btn btn-lg btn-outline-primary w-100 mt-4 shadow-sm"
+                            <button data-method="PATCH" class="btn btn-outline-primary w-100 mt-4 shadow-sm"
                               title="Make a PATCH request on the {{ name }} resource" data-bs-toggle="tooltip">
                               <span class="d-flex align-items-center justify-content-center gap-4">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "PATCH" %}
                               </span>
                             </button>
                           {% endif %}
@@ -567,15 +567,15 @@
 
 {% if filter_form %}
   {{ filter_form }}
 {% endif %}
 
 {% block script %}
   {{ block.super }}
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
-    integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
+  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
+    integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
 
   <script>
     const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
     const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
   </script>
 {% endblock %}
```

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/filters/base.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       <div class="modal-body">
         <div class="d-grid gap-4">
           {% for element in elements %}
             <div>
               {{ element }}
             </div>
           {% endfor %}
-          <button type="button" class="btn btn-lg btn-outline-secondary shadow-sm" data-bs-dismiss="modal">
+          <button type="button" class="btn btn-outline-secondary shadow-sm" data-bs-dismiss="modal">
             <span class="d-flex align-item-center justify-content-center gap-4">
               <i class="bi bi-x-lg"></i>
               {% translate "Cancel" %}
             </span>
           </button>
         </div>
       </div>
```

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/filters/ordering.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/filters/search.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/search.html`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       <input
         type="search"
         class="form-control"
         name="{{ param }}"
         value="{{ term }}"
         placeholder="{% translate 'Type here to search...' %}"
       />
-      <button class="btn btn-lg btn-outline-primary shadow-sm" type="submit">
+      <button class="btn btn-outline-primary shadow-sm" type="submit">
         <span class="d-flex align-items-center gap-4">
           <i class="bi bi-search"></i>
           {% translate "Search" %}
         </span>
       </button>
     </div>
   </div>
```

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/checkbox.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/input.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/radio.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/select.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/select_multiple.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/horizontal/textarea.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/checkbox.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/input.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/radio.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/select.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/select_multiple.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/inline/textarea.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/login.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/login.html`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 {% block meta %}
   {{ block.super }}
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
-  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" 
-    integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
+      integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@latest/font/bootstrap-icons.css">
   {% endblock %}
 
   <script>
     /*!
     * Color mode toggler for Bootstrap's docs (https://getbootstrap.com/)
     * Copyright 2011-2023 The Bootstrap Authors
@@ -108,15 +108,15 @@
 
               {% if form.non_field_errors %}
                 {% for error in form.non_field_errors %}
                   <div class="alert alert-danger" role="alert">{{ error }}</div>
                 {% endfor %}
               {% endif %}
 
-              <button type="submit" class="btn btn-lg btn-primary w-100 shadow-sm">
+              <button type="submit" class="btn btn-primary w-100 shadow-sm">
                 <span class="d-flex align-items-center justify-content-center gap-4">
                   <i class="bi bi-box-arrow-in-right"></i>
                   {% translate "Login" %}
                 </span>
               </button>
             </form>
           </main>
@@ -126,10 +126,10 @@
     </div>
   </body>
 {% endblock %}
 
 
 {% block script %}
   {{ block.super }}
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
-    integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
+  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
+    integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
 {% endblock %}
```

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/pagination/numbers.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/pagination/previous_and_next.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/checkbox.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/input.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/radio.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/select.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/select_multiple.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templates/rest_framework/vertical/textarea.html` & `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/drf_redesign/templatetags/rest_framework_redesign.py` & `drf_redesign-0.3.3/drf_redesign/templatetags/rest_framework_redesign.py`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.2/pyproject.toml` & `drf_redesign-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-redesign"
-version = "0.3.2"
+version = "0.3.3"
 description = "Redesign of the browse-able api of Django REST Framework with Bootstrap 5"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_redesign"}]
 homepage = "https://github.com/youzarsiph/drf-redesign/"
 repository = "https://github.com/youzarsiph/drf-redesign/"
```

### Comparing `drf_redesign-0.3.2/PKG-INFO` & `drf_redesign-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-redesign
-Version: 0.3.2
+Version: 0.3.3
 Summary: Redesign of the browse-able api of Django REST Framework with Bootstrap 5
 Home-page: https://github.com/youzarsiph/drf-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -18,16 +18,16 @@
 Requires-Dist: django (>=3.0)
 Requires-Dist: djangorestframework (>=3.14)
 Project-URL: Repository, https://github.com/youzarsiph/drf-redesign/
 Description-Content-Type: text/markdown
 
 # 🚀 drf-redesign
 
-[![Pylint](https://github.com/youzarsiph/drf-redesign/actions/workflows/pylint.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/pylint.yml)
-[![Upload Python Package](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml)
+[![Ruff](https://github.com/youzarsiph/drf-redesign/actions/workflows/ruff.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/ruff.yml)
+[![Publish](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/python-publish.yml)
 [![Django CI](https://github.com/youzarsiph/drf-redesign/actions/workflows/django.yml/badge.svg)](https://github.com/youzarsiph/drf-redesign/actions/workflows/django.yml)
 
 **drf-redesign** is a project that gives a fresh look to the browse-able API of Django REST Framework using Bootstrap 5.
 
 We want to make the API more **appealing** and **intuitive** for developers and users alike.
 That's why we created a **stylish** and **modern** design that makes the API easier to navigate and interact with.
 One of the coolest features of drf-redesign is the **dark mode** option.
@@ -47,15 +47,15 @@
   ensuring that the API is easy to use for everyone, regardless of their abilities or preferences.
 - **Light and dark themes**: drf-redesign lets you choose between a light or a dark color scheme for the API,
   depending on your mood or environment. You can switch between the themes with a simple click of a button.
 - **Bootstrap icons**: drf-redesign uses Bootstrap icons, a set of open source icons designed for Bootstrap components,
   to add some visual flair to the API. The icons are scalable, customizable, and easy to use.
 - **Form input max length indicators**: drf-redesign shows the maximum length of each form input field,
   so you know how much data you can enter. The indicators also change color when you reach the limit, giving you visual feedback.
-- **Form inputs required indicators**: drf-redesign marks the required form input fields with an asterisk (*),
+- **Form inputs required indicators**: drf-redesign marks the required form input fields with an asterisk (\*),
   so you know which fields are mandatory to submit the form. The indicators also show an error message if you try to submit the form without filling the required fields.
 - **Browser form validation**: drf-redesign uses the built-in browser form validation features, such as HTML5 attributes,
   to validate the form input data before sending it to the server. The validation checks for formats, patterns, ranges, and more.
 
 ## Images
 
 ![DRF Redesign Dark Mode](assets/img/drf-redesign-dark.jpeg)
```

