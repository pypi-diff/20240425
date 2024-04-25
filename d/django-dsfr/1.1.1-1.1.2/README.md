# Comparing `tmp/django_dsfr-1.1.1.tar.gz` & `tmp/django_dsfr-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dsfr-1.1.1.tar", max compression
+gzip compressed data, was "django_dsfr-1.1.2.tar", max compression
```

## Comparing `django_dsfr-1.1.1.tar` & `django_dsfr-1.1.2.tar`

### file list

```diff
@@ -1,1220 +1,1220 @@
--rw-r--r--   0        0        0     1235 2024-04-17 13:31:36.141838 django_dsfr-1.1.1/LICENSE
--rw-r--r--   0        0        0     2567 2024-04-17 13:31:36.141838 django_dsfr-1.1.1/README.rst
--rw-r--r--   0        0        0        0 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/__init__.py
--rw-r--r--   0        0        0     1650 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/admin.py
--rw-r--r--   0        0        0      193 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/apps.py
--rw-r--r--   0        0        0     1545 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/checksums.py
--rw-r--r--   0        0        0     1733 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/constants.py
--rw-r--r--   0        0        0      421 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/context_processors.py
--rw-r--r--   0        0        0      455 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/fixtures/init.json
--rw-r--r--   0        0        0     1684 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/forms.py
--rw-r--r--   0        0        0     6899 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10506 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/management/commands/__init__.py
--rw-r--r--   0        0        0     2189 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/management/commands/integrity_checksums.py
--rw-r--r--   0        0        0     1508 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/management/commands/make_icon_picker_files.py
--rw-r--r--   0        0        0     2385 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/management/commands/trim_dist.py
--rw-r--r--   0        0        0     3301 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0001_initial.py
--rw-r--r--   0        0        0     2885 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0002_auto_20211209_1557.py
--rw-r--r--   0        0        0      710 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py
--rw-r--r--   0        0        0     1765 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0004_dsfrconfig_beta_tag_dsfrconfig_operator_logo_alt_and_more.py
--rw-r--r--   0        0        0      579 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0005_dsfrconfig_notice.py
--rw-r--r--   0        0        0      621 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0006_alter_dsfrconfig_accessibility_status.py
--rw-r--r--   0        0        0     2326 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0007_dsfrconfig_newsletter_description_and_more.py
--rw-r--r--   0        0        0     5872 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/0008_alter_dsfrsocialmedia_options_dsfrconfig_language_and_more.py
--rw-r--r--   0        0        0        0 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/migrations/__init__.py
--rw-r--r--   0        0        0     4415 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/models.py
--rw-r--r--   0        0        0     6152 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/css/dsfr-code.css
--rw-r--r--   0        0        0      125 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/css/dsfr-django-overrides.css
--rw-r--r--   0        0        0      278 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/README.md
--rw-r--r--   0        0        0      465 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-buildings.json
--rw-r--r--   0        0        0     1063 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-business.json
--rw-r--r--   0        0        0      533 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-communication.json
--rw-r--r--   0        0        0      793 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-design.json
--rw-r--r--   0        0        0      671 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-development.json
--rw-r--r--   0        0        0      639 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-device.json
--rw-r--r--   0        0        0      575 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-document.json
--rw-r--r--   0        0        0      401 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-editor.json
--rw-r--r--   0        0        0      454 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-finance.json
--rw-r--r--   0        0        0      843 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-health.json
--rw-r--r--   0        0        0      917 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-logo.json
--rw-r--r--   0        0        0      897 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-map.json
--rw-r--r--   0        0        0      814 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-media.json
--rw-r--r--   0        0        0      337 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-others.json
--rw-r--r--   0        0        0     2158 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-system.json
--rw-r--r--   0        0        0      537 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-user.json
--rw-r--r--   0        0        0      237 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-weather.json
--rw-r--r--   0        0        0      632 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0        0        0      872 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/images/star-of-life-solid.svg
--rw-r--r--   0        0        0      645 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/images/xmark-solid.svg
--rw-r--r--   0        0        0    22397 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.js
--rw-r--r--   0        0        0    11414 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.min.js
--rw-r--r--   0        0        0    10670 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/scss/universal-icon-picker.scss
--rw-r--r--   0        0        0    10767 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.css
--rw-r--r--   0        0        0     9324 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.min.css
--rw-r--r--   0        0        0      469 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/README.md
--rw-r--r--   0        0        0     3461 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/analytics/README.md
--rw-r--r--   0        0        0    69425 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/analytics/analytics.module.min.js
--rw-r--r--   0        0        0    96039 2024-04-17 13:31:36.145838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/analytics/analytics.nomodule.min.js
--rw-r--r--   0        0        0    16409 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/background/ovoid.svg
--rw-r--r--   0        0        0     3884 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/dark.svg
--rw-r--r--   0        0        0     4750 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/light.svg
--rw-r--r--   0        0        0     5712 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/city-hall.svg
--rw-r--r--   0        0        0     6612 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/factory.svg
--rw-r--r--   0        0        0     3564 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/house.svg
--rw-r--r--   0        0        0    10932 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/nuclear-plant.svg
--rw-r--r--   0        0        0     5534 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/school.svg
--rw-r--r--   0        0        0     5409 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/application.svg
--rw-r--r--   0        0        0     4327 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/avatar.svg
--rw-r--r--   0        0        0     4158 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/calendar.svg
--rw-r--r--   0        0        0     4015 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/coding.svg
--rw-r--r--   0        0        0     5502 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/data-visualization.svg
--rw-r--r--   0        0        0     7230 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/internet.svg
--rw-r--r--   0        0        0     3993 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/mail-send.svg
--rw-r--r--   0        0        0     3191 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/search.svg
--rw-r--r--   0        0        0     4823 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/contract.svg
--rw-r--r--   0        0        0     2599 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document-add.svg
--rw-r--r--   0        0        0     3905 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document-download.svg
--rw-r--r--   0        0        0     3201 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document-signature.svg
--rw-r--r--   0        0        0     2453 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document.svg
--rw-r--r--   0        0        0     4716 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/driving-licence.svg
--rw-r--r--   0        0        0     4210 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/national-identity-card.svg
--rw-r--r--   0        0        0     3572 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/passport.svg
--rw-r--r--   0        0        0    10659 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/tax-stamp.svg
--rw-r--r--   0        0        0     5360 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/vehicle-registration.svg
--rw-r--r--   0        0        0     8630 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/environment.svg
--rw-r--r--   0        0        0     5177 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/food.svg
--rw-r--r--   0        0        0     6131 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/grocery.svg
--rw-r--r--   0        0        0    10973 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/human-cooperation.svg
--rw-r--r--   0        0        0     5704 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/leaf.svg
--rw-r--r--   0        0        0     2809 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/moon.svg
--rw-r--r--   0        0        0     4263 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/mountain.svg
--rw-r--r--   0        0        0     3555 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/sun.svg
--rw-r--r--   0        0        0     6161 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/tree.svg
--rw-r--r--   0        0        0     7177 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/health.svg
--rw-r--r--   0        0        0     3577 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/hospital.svg
--rw-r--r--   0        0        0     7720 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/vaccine.svg
--rw-r--r--   0        0        0     8264 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/virus.svg
--rw-r--r--   0        0        0     8682 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/firefighter.svg
--rw-r--r--   0        0        0     5880 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/gendarmerie.svg
--rw-r--r--   0        0        0     4778 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/justice.svg
--rw-r--r--   0        0        0    16555 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/money.svg
--rw-r--r--   0        0        0     8621 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/police.svg
--rw-r--r--   0        0        0     7856 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/book.svg
--rw-r--r--   0        0        0     4138 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/community.svg
--rw-r--r--   0        0        0     6782 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/culture.svg
--rw-r--r--   0        0        0     4973 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/digital-art.svg
--rw-r--r--   0        0        0     6890 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/paint.svg
--rw-r--r--   0        0        0     6799 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/airport.svg
--rw-r--r--   0        0        0    15123 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/location-france.svg
--rw-r--r--   0        0        0     4427 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/luggage.svg
--rw-r--r--   0        0        0     7293 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/map.svg
--rw-r--r--   0        0        0     2791 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/connection-lost.svg
--rw-r--r--   0        0        0     2098 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/error.svg
--rw-r--r--   0        0        0     3506 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/information.svg
--rw-r--r--   0        0        0     4103 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/notification.svg
--rw-r--r--   0        0        0     2592 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/padlock.svg
--rw-r--r--   0        0        0     1985 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/success.svg
--rw-r--r--   0        0        0    15162 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/system.svg
--rw-r--r--   0        0        0     4442 2024-04-17 13:31:36.149838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/technical-error.svg
--rw-r--r--   0        0        0     1577 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/warning.svg
--rw-r--r--   0        0        0    15015 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/system.svg
--rw-r--r--   0        0        0      964 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/README.md
--rw-r--r--   0        0        0     1143 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/README.md
--rw-r--r--   0        0        0     1085 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css
--rw-r--r--   0        0        0     2396 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css
--rw-r--r--   0        0        0     3635 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.min.css
--rw-r--r--   0        0        0     1129 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js
--rw-r--r--   0        0        0     1734 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js
--rw-r--r--   0        0        0      512 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.print.min.css
--rw-r--r--   0        0        0      749 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/README.md
--rw-r--r--   0        0        0     2317 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css
--rw-r--r--   0        0        0     5141 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.main.min.css
--rw-r--r--   0        0        0     8387 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.min.css
--rw-r--r--   0        0        0     1287 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.print.min.css
--rw-r--r--   0        0        0      685 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/README.md
--rw-r--r--   0        0        0     3117 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css
--rw-r--r--   0        0        0    10533 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.main.min.css
--rw-r--r--   0        0        0    14869 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.min.css
--rw-r--r--   0        0        0     1577 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.print.min.css
--rw-r--r--   0        0        0     1176 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/README.md
--rw-r--r--   0        0        0      858 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css
--rw-r--r--   0        0        0     3015 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css
--rw-r--r--   0        0        0     3772 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css
--rw-r--r--   0        0        0     1600 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js
--rw-r--r--   0        0        0     2179 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js
--rw-r--r--   0        0        0      257 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.print.min.css
--rw-r--r--   0        0        0     1114 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/README.md
--rw-r--r--   0        0        0    10821 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.legacy.min.css
--rw-r--r--   0        0        0    29226 2024-04-17 13:31:36.153838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.main.min.css
--rw-r--r--   0        0        0    44554 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.min.css
--rw-r--r--   0        0        0      514 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.module.min.js
--rw-r--r--   0        0        0      536 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js
--rw-r--r--   0        0        0     4865 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.print.min.css
--rw-r--r--   0        0        0      790 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/README.md
--rw-r--r--   0        0        0     2398 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css
--rw-r--r--   0        0        0     7111 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.main.min.css
--rw-r--r--   0        0        0    11273 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.min.css
--rw-r--r--   0        0        0     2122 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.print.min.css
--rw-r--r--   0        0        0     1492 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/README.md
--rw-r--r--   0        0        0     2785 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.legacy.min.css
--rw-r--r--   0        0        0    10531 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.main.min.css
--rw-r--r--   0        0        0    14122 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.min.css
--rw-r--r--   0        0        0      825 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.module.min.js
--rw-r--r--   0        0        0     1093 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.nomodule.min.js
--rw-r--r--   0        0        0     1164 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.print.min.css
--rw-r--r--   0        0        0      971 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/README.md
--rw-r--r--   0        0        0     9140 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css
--rw-r--r--   0        0        0    10611 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css
--rw-r--r--   0        0        0    19908 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css
--rw-r--r--   0        0        0     8689 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.print.min.css
--rw-r--r--   0        0        0   115826 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.legacy.min.css
--rw-r--r--   0        0        0   323926 2024-04-17 13:31:36.157838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.main.min.css
--rw-r--r--   0        0        0   503919 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.min.css
--rw-r--r--   0        0        0    47336 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.module.min.js
--rw-r--r--   0        0        0    63661 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.nomodule.min.js
--rw-r--r--   0        0        0    74103 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.print.min.css
--rw-r--r--   0        0        0      733 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/README.md
--rw-r--r--   0        0        0      576 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css
--rw-r--r--   0        0        0     6927 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.main.min.css
--rw-r--r--   0        0        0     7571 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.min.css
--rw-r--r--   0        0        0      426 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.print.min.css
--rw-r--r--   0        0        0     1628 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/README.md
--rw-r--r--   0        0        0     1685 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css
--rw-r--r--   0        0        0     6729 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.main.min.css
--rw-r--r--   0        0        0     8897 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.min.css
--rw-r--r--   0        0        0      841 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.print.min.css
--rw-r--r--   0        0        0     1056 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/README.md
--rw-r--r--   0        0        0     1125 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.legacy.min.css
--rw-r--r--   0        0        0     2593 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.main.min.css
--rw-r--r--   0        0        0     3811 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.min.css
--rw-r--r--   0        0        0      451 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.print.min.css
--rw-r--r--   0        0        0     1640 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/display/README.md
--rw-r--r--   0        0        0     1332 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/display/display.module.min.js
--rw-r--r--   0        0        0     1843 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js
--rw-r--r--   0        0        0      781 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/download/README.md
--rw-r--r--   0        0        0     3529 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/download/download.min.css
--rw-r--r--   0        0        0     1183 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/README.md
--rw-r--r--   0        0        0     6194 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css
--rw-r--r--   0        0        0    10271 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.main.min.css
--rw-r--r--   0        0        0    17329 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.min.css
--rw-r--r--   0        0        0     1222 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.print.min.css
--rw-r--r--   0        0        0      934 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/README.md
--rw-r--r--   0        0        0     1119 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css
--rw-r--r--   0        0        0     7718 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.main.min.css
--rw-r--r--   0        0        0     9214 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.min.css
--rw-r--r--   0        0        0      735 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.print.min.css
--rw-r--r--   0        0        0      563 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/README.md
--rw-r--r--   0        0        0     3650 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.legacy.min.css
--rw-r--r--   0        0        0     9618 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.main.min.css
--rw-r--r--   0        0        0    14995 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.min.css
--rw-r--r--   0        0        0     2085 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.print.min.css
--rw-r--r--   0        0        0     2240 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/README.md
--rw-r--r--   0        0        0     7240 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.legacy.min.css
--rw-r--r--   0        0        0    17301 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.main.min.css
--rw-r--r--   0        0        0    29441 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.min.css
--rw-r--r--   0        0        0     2618 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.module.min.js
--rw-r--r--   0        0        0     3201 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js
--rw-r--r--   0        0        0     5258 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.print.min.css
--rw-r--r--   0        0        0      702 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/README.md
--rw-r--r--   0        0        0     1877 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css
--rw-r--r--   0        0        0     3046 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css
--rw-r--r--   0        0        0     6224 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.min.css
--rw-r--r--   0        0        0     1659 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.print.min.css
--rw-r--r--   0        0        0      560 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/README.md
--rw-r--r--   0        0        0      837 2024-04-17 13:31:36.161838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/README.md
--rw-r--r--   0        0        0     1927 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.legacy.min.css
--rw-r--r--   0        0        0     5557 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.main.min.css
--rw-r--r--   0        0        0     8684 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.min.css
--rw-r--r--   0        0        0     1665 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.print.min.css
--rw-r--r--   0        0        0      795 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-email/README.md
--rw-r--r--   0        0        0      790 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-tel/README.md
--rw-r--r--   0        0        0     1999 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.legacy.min.css
--rw-r--r--   0        0        0     5629 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.main.min.css
--rw-r--r--   0        0        0     8828 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.min.css
--rw-r--r--   0        0        0     1665 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.print.min.css
--rw-r--r--   0        0        0      786 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/README.md
--rw-r--r--   0        0        0     1401 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.legacy.min.css
--rw-r--r--   0        0        0    11309 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.main.min.css
--rw-r--r--   0        0        0    12645 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.min.css
--rw-r--r--   0        0        0      293 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.print.min.css
--rw-r--r--   0        0        0      435 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/README.md
--rw-r--r--   0        0        0      381 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css
--rw-r--r--   0        0        0    11536 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/logo.main.min.css
--rw-r--r--   0        0        0    11791 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/logo.min.css
--rw-r--r--   0        0        0      232 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/logo.print.min.css
--rw-r--r--   0        0        0     1391 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/README.md
--rw-r--r--   0        0        0      584 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css
--rw-r--r--   0        0        0     2839 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.main.min.css
--rw-r--r--   0        0        0     3550 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.min.css
--rw-r--r--   0        0        0     7482 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.module.min.js
--rw-r--r--   0        0        0     9236 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js
--rw-r--r--   0        0        0      485 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.print.min.css
--rw-r--r--   0        0        0     1412 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/README.md
--rw-r--r--   0        0        0     2559 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css
--rw-r--r--   0        0        0     6849 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css
--rw-r--r--   0        0        0     9221 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.min.css
--rw-r--r--   0        0        0     3656 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js
--rw-r--r--   0        0        0     4678 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js
--rw-r--r--   0        0        0      171 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.print.min.css
--rw-r--r--   0        0        0      827 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/README.md
--rw-r--r--   0        0        0      871 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css
--rw-r--r--   0        0        0     1890 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.main.min.css
--rw-r--r--   0        0        0     2649 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.min.css
--rw-r--r--   0        0        0      246 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.print.min.css
--rw-r--r--   0        0        0      706 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/README.md
--rw-r--r--   0        0        0     2870 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css
--rw-r--r--   0        0        0     9995 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css
--rw-r--r--   0        0        0    13186 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.min.css
--rw-r--r--   0        0        0      679 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.print.min.css
--rw-r--r--   0        0        0     1462 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/README.md
--rw-r--r--   0        0        0     2594 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.legacy.min.css
--rw-r--r--   0        0        0     3658 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.main.min.css
--rw-r--r--   0        0        0     7200 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.min.css
--rw-r--r--   0        0        0     2564 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.module.min.js
--rw-r--r--   0        0        0     3887 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.nomodule.min.js
--rw-r--r--   0        0        0     2413 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.print.min.css
--rw-r--r--   0        0        0      749 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/README.md
--rw-r--r--   0        0        0     1656 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css
--rw-r--r--   0        0        0     3961 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.main.min.css
--rw-r--r--   0        0        0     6413 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.min.css
--rw-r--r--   0        0        0     1154 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.print.min.css
--rw-r--r--   0        0        0      894 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/README.md
--rw-r--r--   0        0        0     9327 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css
--rw-r--r--   0        0        0    19243 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.main.min.css
--rw-r--r--   0        0        0    36596 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.min.css
--rw-r--r--   0        0        0     8384 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.print.min.css
--rw-r--r--   0        0        0     1260 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/README.md
--rw-r--r--   0        0        0     4633 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.legacy.min.css
--rw-r--r--   0        0        0     6745 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.main.min.css
--rw-r--r--   0        0        0    11149 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.min.css
--rw-r--r--   0        0        0    10167 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.module.min.js
--rw-r--r--   0        0        0    13729 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.nomodule.min.js
--rw-r--r--   0        0        0      976 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/README.md
--rw-r--r--   0        0        0     1222 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.legacy.min.css
--rw-r--r--   0        0        0     2831 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.main.min.css
--rw-r--r--   0        0        0     4558 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.min.css
--rw-r--r--   0        0        0      863 2024-04-17 13:31:36.165838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.print.min.css
--rw-r--r--   0        0        0     1307 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/README.md
--rw-r--r--   0        0        0      942 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.legacy.min.css
--rw-r--r--   0        0        0     5053 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.main.min.css
--rw-r--r--   0        0        0     5766 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.min.css
--rw-r--r--   0        0        0     1849 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.module.min.js
--rw-r--r--   0        0        0     2375 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.nomodule.min.js
--rw-r--r--   0        0        0      753 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/README.md
--rw-r--r--   0        0        0     1630 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.legacy.min.css
--rw-r--r--   0        0        0     3178 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.main.min.css
--rw-r--r--   0        0        0     5937 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.min.css
--rw-r--r--   0        0        0     1487 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.print.min.css
--rw-r--r--   0        0        0      896 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/README.md
--rw-r--r--   0        0        0     2879 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.legacy.min.css
--rw-r--r--   0        0        0     6655 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.main.min.css
--rw-r--r--   0        0        0    10075 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.min.css
--rw-r--r--   0        0        0      899 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.print.min.css
--rw-r--r--   0        0        0     1150 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/README.md
--rw-r--r--   0        0        0     1842 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css
--rw-r--r--   0        0        0     5902 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css
--rw-r--r--   0        0        0     8693 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css
--rw-r--r--   0        0        0     1171 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js
--rw-r--r--   0        0        0     1780 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js
--rw-r--r--   0        0        0     1307 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.print.min.css
--rw-r--r--   0        0        0      844 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/README.md
--rw-r--r--   0        0        0      466 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css
--rw-r--r--   0        0        0     1307 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css
--rw-r--r--   0        0        0     1620 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css
--rw-r--r--   0        0        0      205 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/skiplink.print.min.css
--rw-r--r--   0        0        0      723 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/README.md
--rw-r--r--   0        0        0      788 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css
--rw-r--r--   0        0        0     3603 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css
--rw-r--r--   0        0        0     4643 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.min.css
--rw-r--r--   0        0        0      610 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.print.min.css
--rw-r--r--   0        0        0      707 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/README.md
--rw-r--r--   0        0        0      445 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css
--rw-r--r--   0        0        0     1186 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/summary.main.min.css
--rw-r--r--   0        0        0     1513 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/summary.min.css
--rw-r--r--   0        0        0      240 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/summary.print.min.css
--rw-r--r--   0        0        0     1092 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/README.md
--rw-r--r--   0        0        0     1926 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css
--rw-r--r--   0        0        0     6080 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.main.min.css
--rw-r--r--   0        0        0     8486 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.min.css
--rw-r--r--   0        0        0     5911 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.module.min.js
--rw-r--r--   0        0        0     7820 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js
--rw-r--r--   0        0        0      838 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.print.min.css
--rw-r--r--   0        0        0     1084 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/README.md
--rw-r--r--   0        0        0     6961 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.legacy.min.css
--rw-r--r--   0        0        0    20082 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.main.min.css
--rw-r--r--   0        0        0    33509 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.min.css
--rw-r--r--   0        0        0     2303 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.module.min.js
--rw-r--r--   0        0        0     3220 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js
--rw-r--r--   0        0        0     6824 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.print.min.css
--rw-r--r--   0        0        0     1122 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/README.md
--rw-r--r--   0        0        0    13862 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css
--rw-r--r--   0        0        0    17311 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.main.min.css
--rw-r--r--   0        0        0    42083 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.min.css
--rw-r--r--   0        0        0     1082 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.module.min.js
--rw-r--r--   0        0        0     1376 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js
--rw-r--r--   0        0        0    11268 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.print.min.css
--rw-r--r--   0        0        0     1119 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/README.md
--rw-r--r--   0        0        0     2838 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css
--rw-r--r--   0        0        0     9417 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.main.min.css
--rw-r--r--   0        0        0    13352 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.min.css
--rw-r--r--   0        0        0      785 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.module.min.js
--rw-r--r--   0        0        0     1052 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.nomodule.min.js
--rw-r--r--   0        0        0     1455 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.print.min.css
--rw-r--r--   0        0        0     1205 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/README.md
--rw-r--r--   0        0        0     4846 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css
--rw-r--r--   0        0        0    11190 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css
--rw-r--r--   0        0        0    20338 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.min.css
--rw-r--r--   0        0        0     1291 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js
--rw-r--r--   0        0        0     1998 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js
--rw-r--r--   0        0        0     4660 2024-04-17 13:31:36.169838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.print.min.css
--rw-r--r--   0        0        0     1038 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/README.md
--rw-r--r--   0        0        0     1206 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.legacy.min.css
--rw-r--r--   0        0        0     2311 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.main.min.css
--rw-r--r--   0        0        0     3534 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.min.css
--rw-r--r--   0        0        0     2785 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.module.min.js
--rw-r--r--   0        0        0     3728 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.nomodule.min.js
--rw-r--r--   0        0        0      375 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.print.min.css
--rw-r--r--   0        0        0     1276 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/README.md
--rw-r--r--   0        0        0     1421 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.legacy.min.css
--rw-r--r--   0        0        0     5128 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.main.min.css
--rw-r--r--   0        0        0     6684 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.min.css
--rw-r--r--   0        0        0      617 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.module.min.js
--rw-r--r--   0        0        0      974 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.nomodule.min.js
--rw-r--r--   0        0        0      493 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.print.min.css
--rw-r--r--   0        0        0     1441 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/README.md
--rw-r--r--   0        0        0     1082 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css
--rw-r--r--   0        0        0     2642 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.main.min.css
--rw-r--r--   0        0        0     3808 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.min.css
--rw-r--r--   0        0        0      632 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.print.min.css
--rw-r--r--   0        0        0      574 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/README.md
--rw-r--r--   0        0        0      799 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/upload.main.min.css
--rw-r--r--   0        0        0      858 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/upload.min.css
--rw-r--r--   0        0        0      188 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/upload.print.min.css
--rw-r--r--   0        0        0     2503 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/README.md
--rw-r--r--   0        0        0     3496 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.legacy.min.css
--rw-r--r--   0        0        0   169254 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.main.min.css
--rw-r--r--   0        0        0   174542 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.min.css
--rw-r--r--   0        0        0    52971 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.module.min.js
--rw-r--r--   0        0        0    69953 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.nomodule.min.js
--rw-r--r--   0        0        0     2150 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.print.min.css
--rw-r--r--   0        0        0      557 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/README.md
--rw-r--r--   0        0        0   118833 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css
--rw-r--r--   0        0        0   505020 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css
--rw-r--r--   0        0        0   614046 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.min.css
--rw-r--r--   0        0        0   103658 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js
--rw-r--r--   0        0        0   264441 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js
--rw-r--r--   0        0        0   118518 2024-04-17 13:31:36.173838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.legacy.min.css
--rw-r--r--   0        0        0   504300 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.main.min.css
--rw-r--r--   0        0        0   688992 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.min.css
--rw-r--r--   0        0        0   103658 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.module.min.js
--rw-r--r--   0        0        0   264441 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.nomodule.min.js
--rw-r--r--   0        0        0    76110 2024-04-17 13:31:36.177838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.print.min.css
--rw-r--r--   0        0        0     3631 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0     9190 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     3448 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0     7406 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/favicon.ico
--rw-r--r--   0        0        0     6360 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/favicon.svg
--rw-r--r--   0        0        0      292 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/manifest.webmanifest
--rwxr-xr-x   0        0        0    52216 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff
--rwxr-xr-x   0        0        0    42092 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2
--rwxr-xr-x   0        0        0    56436 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff
--rwxr-xr-x   0        0        0    45300 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2
--rwxr-xr-x   0        0        0    50440 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff
--rwxr-xr-x   0        0        0    41368 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2
--rwxr-xr-x   0        0        0    54492 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff
--rwxr-xr-x   0        0        0    43916 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2
--rwxr-xr-x   0        0        0    51292 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff
--rwxr-xr-x   0        0        0    41940 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2
--rwxr-xr-x   0        0        0    54680 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff
--rwxr-xr-x   0        0        0    44572 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2
--rwxr-xr-x   0        0        0    51140 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff
--rwxr-xr-x   0        0        0    41328 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2
--rwxr-xr-x   0        0        0    54328 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff
--rwxr-xr-x   0        0        0    44284 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2
--rw-r--r--   0        0        0   114508 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff
--rw-r--r--   0        0        0    80368 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2
--rw-r--r--   0        0        0   114016 2024-04-17 13:31:36.181838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff
--rw-r--r--   0        0        0    79472 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2
--rw-r--r--   0        0        0      397 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-fill.svg
--rw-r--r--   0        0        0      789 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg
--rw-r--r--   0        0        0      280 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-fill.svg
--rw-r--r--   0        0        0      416 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-line.svg
--rw-r--r--   0        0        0      232 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/bank-fill.svg
--rw-r--r--   0        0        0      262 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/bank-line.svg
--rw-r--r--   0        0        0      204 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/building-fill.svg
--rw-r--r--   0        0        0      225 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/building-line.svg
--rw-r--r--   0        0        0      316 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/community-fill.svg
--rw-r--r--   0        0        0      388 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/community-line.svg
--rw-r--r--   0        0        0      232 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/government-fill.svg
--rw-r--r--   0        0        0      227 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/government-line.svg
--rw-r--r--   0        0        0      209 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/home-4-fill.svg
--rw-r--r--   0        0        0      239 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/home-4-line.svg
--rw-r--r--   0        0        0      212 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/hospital-fill.svg
--rw-r--r--   0        0        0      228 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/hospital-line.svg
--rw-r--r--   0        0        0      224 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/hotel-fill.svg
--rw-r--r--   0        0        0      243 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/hotel-line.svg
--rw-r--r--   0        0        0      437 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/store-fill.svg
--rw-r--r--   0        0        0      546 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/store-line.svg
--rw-r--r--   0        0        0      254 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/archive-fill.svg
--rw-r--r--   0        0        0      288 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/archive-line.svg
--rw-r--r--   0        0        0      330 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/attachment-fill.svg
--rw-r--r--   0        0        0      241 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/attachment-line.svg
--rw-r--r--   0        0        0      289 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/award-fill.svg
--rw-r--r--   0        0        0      338 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/award-line.svg
--rw-r--r--   0        0        0      218 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/bar-chart-box-fill.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/bar-chart-box-line.svg
--rw-r--r--   0        0        0      208 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/bookmark-fill.svg
--rw-r--r--   0        0        0      242 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/bookmark-line.svg
--rw-r--r--   0        0        0      253 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/briefcase-fill.svg
--rw-r--r--   0        0        0      267 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/briefcase-line.svg
--rw-r--r--   0        0        0      248 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/calendar-2-fill.svg
--rw-r--r--   0        0        0      281 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/calendar-2-line.svg
--rw-r--r--   0        0        0      218 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/calendar-event-fill.svg
--rw-r--r--   0        0        0      251 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/calendar-event-line.svg
--rw-r--r--   0        0        0      203 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/calendar-fill.svg
--rw-r--r--   0        0        0      244 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/calendar-line.svg
--rw-r--r--   0        0        0      254 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/cloud-fill.svg
--rw-r--r--   0        0        0      356 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/cloud-line.svg
--rw-r--r--   0        0        0      290 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/copyright-fill.svg
--rw-r--r--   0        0        0      346 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/copyright-line.svg
--rw-r--r--   0        0        0      341 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/customer-service-fill.svg
--rw-r--r--   0        0        0      375 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/customer-service-line.svg
--rw-r--r--   0        0        0      210 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/flag-fill.svg
--rw-r--r--   0        0        0      255 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/flag-line.svg
--rw-r--r--   0        0        0      540 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/global-fill.svg
--rw-r--r--   0        0        0      607 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/global-line.svg
--rw-r--r--   0        0        0      200 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/line-chart-fill.svg
--rw-r--r--   0        0        0      218 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/line-chart-line.svg
--rw-r--r--   0        0        0      409 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/links-fill.svg
--rw-r--r--   0        0        0      418 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/links-line.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/mail-fill.svg
--rw-r--r--   0        0        0      247 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/mail-line.svg
--rw-r--r--   0        0        0      318 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/mail-open-fill.svg
--rw-r--r--   0        0        0      359 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/mail-open-line.svg
--rw-r--r--   0        0        0      355 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/medal-fill.svg
--rw-r--r--   0        0        0      389 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/medal-line.svg
--rw-r--r--   0        0        0      248 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/pie-chart-2-fill.svg
--rw-r--r--   0        0        0      378 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/pie-chart-2-line.svg
--rw-r--r--   0        0        0      273 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/pie-chart-box-fill.svg
--rw-r--r--   0        0        0      289 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/pie-chart-box-line.svg
--rw-r--r--   0        0        0      256 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/printer-fill.svg
--rw-r--r--   0        0        0      341 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/printer-line.svg
--rw-r--r--   0        0        0      296 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/profil-fill.svg
--rw-r--r--   0        0        0      312 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/profil-line.svg
--rw-r--r--   0        0        0      356 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/projector-2-fill.svg
--rw-r--r--   0        0        0      350 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/projector-2-line.svg
--rw-r--r--   0        0        0      248 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/send-plane-fill.svg
--rw-r--r--   0        0        0      301 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/send-plane-line.svg
--rw-r--r--   0        0        0      226 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/slideshow-fill.svg
--rw-r--r--   0        0        0      241 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/slideshow-line.svg
--rw-r--r--   0        0        0      215 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/window-fill.svg
--rw-r--r--   0        0        0      230 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/window-line.svg
--rw-r--r--   0        0        0      199 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-2-fill.svg
--rw-r--r--   0        0        0      237 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-2-line.svg
--rw-r--r--   0        0        0      236 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-3-fill.svg
--rw-r--r--   0        0        0      360 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-3-line.svg
--rw-r--r--   0        0        0      256 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-check-fill.svg
--rw-r--r--   0        0        0      283 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-check-line.svg
--rw-r--r--   0        0        0      321 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-delete-fill.svg
--rw-r--r--   0        0        0      348 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-delete-line.svg
--rw-r--r--   0        0        0      243 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-poll-fill.svg
--rw-r--r--   0        0        0      214 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/chat-poll-line.svg
--rw-r--r--   0        0        0      236 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/discuss-fill.svg
--rw-r--r--   0        0        0      282 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/discuss-line.svg
--rw-r--r--   0        0        0      201 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/feedback-fill.svg
--rw-r--r--   0        0        0      229 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/feedback-line.svg
--rw-r--r--   0        0        0      215 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/message-2-fill.svg
--rw-r--r--   0        0        0      245 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/message-2-line.svg
--rw-r--r--   0        0        0      231 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/question-answer-fill.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.185838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/question-answer-line.svg
--rw-r--r--   0        0        0      263 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/questionnaire-fill.svg
--rw-r--r--   0        0        0      327 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/questionnaire-line.svg
--rw-r--r--   0        0        0      206 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/video-chat-fill.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/communication/video-chat-line.svg
--rw-r--r--   0        0        0      318 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/ball-pen-fill.svg
--rw-r--r--   0        0        0      372 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/ball-pen-line.svg
--rw-r--r--   0        0        0      252 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/brush-3-fill.svg
--rw-r--r--   0        0        0      266 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/brush-3-line.svg
--rw-r--r--   0        0        0      449 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/brush-fill.svg
--rw-r--r--   0        0        0      689 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/brush-line.svg
--rw-r--r--   0        0        0      195 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/contrast-fill.svg
--rw-r--r--   0        0        0      230 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/contrast-line.svg
--rw-r--r--   0        0        0      173 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/crop-fill.svg
--rw-r--r--   0        0        0      184 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/crop-line.svg
--rw-r--r--   0        0        0      399 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/drag-move-2-fill.svg
--rw-r--r--   0        0        0      178 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/drag-move-2-line.svg
--rw-r--r--   0        0        0      153 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/drop-fill.svg
--rw-r--r--   0        0        0      190 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/drop-line.svg
--rw-r--r--   0        0        0      275 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/edit-box-fill.svg
--rw-r--r--   0        0        0      255 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/edit-box-line.svg
--rw-r--r--   0        0        0      206 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/edit-fill.svg
--rw-r--r--   0        0        0      258 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/edit-line.svg
--rw-r--r--   0        0        0      266 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/ink-bottle-fill.svg
--rw-r--r--   0        0        0      323 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/ink-bottle-line.svg
--rw-r--r--   0        0        0      241 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/layout-grid-fill.svg
--rw-r--r--   0        0        0      232 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/layout-grid-line.svg
--rw-r--r--   0        0        0      401 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/mark-pen-fill.svg
--rw-r--r--   0        0        0      503 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/mark-pen-line.svg
--rw-r--r--   0        0        0      292 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/paint-brush-fill.svg
--rw-r--r--   0        0        0      305 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/paint-brush-line.svg
--rw-r--r--   0        0        0      339 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/paint-fill.svg
--rw-r--r--   0        0        0      362 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/paint-line.svg
--rw-r--r--   0        0        0      437 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/palette-fill.svg
--rw-r--r--   0        0        0      584 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/palette-line.svg
--rw-r--r--   0        0        0      386 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pantone-fill.svg
--rw-r--r--   0        0        0      505 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pantone-line.svg
--rw-r--r--   0        0        0      389 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pen-nib-fill.svg
--rw-r--r--   0        0        0      510 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pen-nib-line.svg
--rw-r--r--   0        0        0      254 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pencil-fill.svg
--rw-r--r--   0        0        0      310 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pencil-line.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pencil-ruler-fill.svg
--rw-r--r--   0        0        0      255 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/pencil-ruler-line.svg
--rw-r--r--   0        0        0      302 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/sip-fill.svg
--rw-r--r--   0        0        0      352 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/sip-line.svg
--rw-r--r--   0        0        0      221 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/table-fill.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/table-line.svg
--rw-r--r--   0        0        0      500 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/bug-fill.svg
--rw-r--r--   0        0        0      632 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/bug-line.svg
--rw-r--r--   0        0        0      360 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/code-box-fill.svg
--rw-r--r--   0        0        0      374 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/code-box-line.svg
--rw-r--r--   0        0        0      281 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/code-s-slash-line.svg
--rw-r--r--   0        0        0      197 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/cursor-fill.svg
--rw-r--r--   0        0        0      283 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/cursor-line.svg
--rw-r--r--   0        0        0      307 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-branch-fill.svg
--rw-r--r--   0        0        0      425 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-branch-line.svg
--rw-r--r--   0        0        0      187 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-commit-fill.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-commit-line.svg
--rw-r--r--   0        0        0      330 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-merge-fill.svg
--rw-r--r--   0        0        0      455 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-merge-line.svg
--rw-r--r--   0        0        0      233 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-pull-request-fill.svg
--rw-r--r--   0        0        0      356 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-pull-request-line.svg
--rw-r--r--   0        0        0      294 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-repository-commits-fill.svg
--rw-r--r--   0        0        0      320 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-repository-commits-line.svg
--rw-r--r--   0        0        0      285 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-repository-fill.svg
--rw-r--r--   0        0        0      328 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-repository-line.svg
--rw-r--r--   0        0        0      288 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-repository-private-fill.svg
--rw-r--r--   0        0        0      304 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/git-repository-private-line.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/terminal-box-fill.svg
--rw-r--r--   0        0        0      287 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/terminal-box-line.svg
--rw-r--r--   0        0        0      186 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/terminal-line.svg
--rw-r--r--   0        0        0      230 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/terminal-window-fill.svg
--rw-r--r--   0        0        0      245 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/terminal-window-line.svg
--rw-r--r--   0        0        0      343 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/bluetooth-fill.svg
--rw-r--r--   0        0        0      343 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/bluetooth-line.svg
--rw-r--r--   0        0        0      256 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/computer-fill.svg
--rw-r--r--   0        0        0      275 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/computer-line.svg
--rw-r--r--   0        0        0      514 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg
--rw-r--r--   0        0        0      552 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg
--rw-r--r--   0        0        0      266 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/database-fill.svg
--rw-r--r--   0        0        0      296 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/database-line.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/device-fill.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/device-line.svg
--rw-r--r--   0        0        0      206 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/hard-drive-2-fill.svg
--rw-r--r--   0        0        0      222 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/hard-drive-2-line.svg
--rw-r--r--   0        0        0      290 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/mac-fill.svg
--rw-r--r--   0        0        0      288 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/mac-line.svg
--rw-r--r--   0        0        0      485 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/phone-fill.svg
--rw-r--r--   0        0        0      719 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/phone-line.svg
--rw-r--r--   0        0        0      272 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/qr-code-fill.svg
--rw-r--r--   0        0        0      315 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/qr-code-line.svg
--rw-r--r--   0        0        0      229 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/rss-fill.svg
--rw-r--r--   0        0        0      230 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/rss-line.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/save-3-fill.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/save-3-line.svg
--rw-r--r--   0        0        0      195 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/save-fill.svg
--rw-r--r--   0        0        0      219 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/save-line.svg
--rw-r--r--   0        0        0      219 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/server-fill.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/server-line.svg
--rw-r--r--   0        0        0      208 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/smartphone-fill.svg
--rw-r--r--   0        0        0      224 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/smartphone-line.svg
--rw-r--r--   0        0        0      208 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/tablet-fill.svg
--rw-r--r--   0        0        0      224 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/tablet-line.svg
--rw-r--r--   0        0        0      285 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/tv-fill.svg
--rw-r--r--   0        0        0      304 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/tv-line.svg
--rw-r--r--   0        0        0      618 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg
--rw-r--r--   0        0        0      630 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/wifi-line.svg
--rw-r--r--   0        0        0      233 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/article-fill.svg
--rw-r--r--   0        0        0      249 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/article-line.svg
--rw-r--r--   0        0        0      181 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/book-2-fill.svg
--rw-r--r--   0        0        0      227 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/book-2-line.svg
--rw-r--r--   0        0        0      226 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/booklet-fill.svg
--rw-r--r--   0        0        0      242 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/booklet-line.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/clipboard-fill.svg
--rw-r--r--   0        0        0      274 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/clipboard-line.svg
--rw-r--r--   0        0        0      317 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/draft-fill.svg
--rw-r--r--   0        0        0      303 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/draft-line.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-add-fill.svg
--rw-r--r--   0        0        0      251 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-add-line.svg
--rw-r--r--   0        0        0      227 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-download-fill.svg
--rw-r--r--   0        0        0      245 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-download-line.svg
--rw-r--r--   0        0        0      230 2024-04-17 13:31:36.189839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-fill.svg
--rw-r--r--   0        0        0      225 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-line.svg
--rw-r--r--   0        0        0      255 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-pdf-fill.svg
--rw-r--r--   0        0        0      273 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-pdf-line.svg
--rw-r--r--   0        0        0      281 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-text-fill.svg
--rw-r--r--   0        0        0      272 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/file-text-line.svg
--rw-r--r--   0        0        0      198 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/folder-2-fill.svg
--rw-r--r--   0        0        0      234 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/folder-2-line.svg
--rw-r--r--   0        0        0      262 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/newspaper-fill.svg
--rw-r--r--   0        0        0      290 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/newspaper-line.svg
--rw-r--r--   0        0        0      292 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/survey-fill.svg
--rw-r--r--   0        0        0      317 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/survey-line.svg
--rw-r--r--   0        0        0      217 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/todo-fill.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/document/todo-line.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/code-view.svg
--rw-r--r--   0        0        0      250 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/font-size.svg
--rw-r--r--   0        0        0      314 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/fr--bold.svg
--rw-r--r--   0        0        0      160 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/fr--highlight.svg
--rw-r--r--   0        0        0      278 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/fr--quote-fill.svg
--rw-r--r--   0        0        0      344 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/fr--quote-line.svg
--rw-r--r--   0        0        0      223 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-1.svg
--rw-r--r--   0        0        0      387 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-2.svg
--rw-r--r--   0        0        0      542 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-3.svg
--rw-r--r--   0        0        0      268 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-4.svg
--rw-r--r--   0        0        0      393 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-5.svg
--rw-r--r--   0        0        0      538 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-6.svg
--rw-r--r--   0        0        0      298 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/hashtag.svg
--rw-r--r--   0        0        0      158 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/italic.svg
--rw-r--r--   0        0        0      468 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/link-unlink.svg
--rw-r--r--   0        0        0      408 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/link.svg
--rw-r--r--   0        0        0      246 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/list-ordered.svg
--rw-r--r--   0        0        0      275 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/list-unordered.svg
--rw-r--r--   0        0        0      341 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/question-mark.svg
--rw-r--r--   0        0        0      147 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/separator.svg
--rw-r--r--   0        0        0      151 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/space.svg
--rw-r--r--   0        0        0      317 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/subscript.svg
--rw-r--r--   0        0        0      315 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/superscript.svg
--rw-r--r--   0        0        0      263 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/table-2.svg
--rw-r--r--   0        0        0      505 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/translate-2.svg
--rw-r--r--   0        0        0      206 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/bank-card-fill.svg
--rw-r--r--   0        0        0      220 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/bank-card-line.svg
--rw-r--r--   0        0        0      277 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/coin-fill.svg
--rw-r--r--   0        0        0      393 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/gift-fill.svg
--rw-r--r--   0        0        0      406 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/gift-line.svg
--rw-r--r--   0        0        0      366 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/money-euro-box-fill.svg
--rw-r--r--   0        0        0      344 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/money-euro-box-line.svg
--rw-r--r--   0        0        0      365 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-fill.svg
--rw-r--r--   0        0        0      362 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-line.svg
--rw-r--r--   0        0        0      397 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/secure-payment-fill.svg
--rw-r--r--   0        0        0      427 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/secure-payment-line.svg
--rw-r--r--   0        0        0      348 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/shopping-bag-fill.svg
--rw-r--r--   0        0        0      282 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/shopping-bag-line.svg
--rw-r--r--   0        0        0      311 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-fill.svg
--rw-r--r--   0        0        0      343 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-line.svg
--rw-r--r--   0        0        0      200 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/trophy-fill.svg
--rw-r--r--   0        0        0      222 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/finance/trophy-line.svg
--rw-r--r--   0        0        0      289 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/capsule-fill.svg
--rw-r--r--   0        0        0      379 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/capsule-line.svg
--rw-r--r--   0        0        0      336 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/dislike-fill.svg
--rw-r--r--   0        0        0      543 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/dislike-line.svg
--rw-r--r--   0        0        0      243 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/dossier-fill.svg
--rw-r--r--   0        0        0      265 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/dossier-line.svg
--rw-r--r--   0        0        0      269 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/first-aid-kit-fill.svg
--rw-r--r--   0        0        0      283 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/first-aid-kit-line.svg
--rw-r--r--   0        0        0      317 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-fill.svg
--rw-r--r--   0        0        0      359 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-line.svg
--rw-r--r--   0        0        0      258 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/health-book-fill.svg
--rw-r--r--   0        0        0      273 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/health-book-line.svg
--rw-r--r--   0        0        0      209 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/heart-fill.svg
--rw-r--r--   0        0        0      365 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/heart-line.svg
--rw-r--r--   0        0        0      331 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/heart-pulse-fill.svg
--rw-r--r--   0        0        0      661 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg
--rw-r--r--   0        0        0      476 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/lungs-fill.svg
--rw-r--r--   0        0        0      909 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/lungs-line.svg
--rw-r--r--   0        0        0      241 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/medicine-bottle-fill.svg
--rw-r--r--   0        0        0      293 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/medicine-bottle-line.svg
--rw-r--r--   0        0        0      395 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/mental-health-fill.svg
--rw-r--r--   0        0        0      503 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/mental-health-line.svg
--rw-r--r--   0        0        0      519 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg
--rw-r--r--   0        0        0      618 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/microscope-line.svg
--rw-r--r--   0        0        0      370 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/psychotherapy-fill.svg
--rw-r--r--   0        0        0      504 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/psychotherapy-line.svg
--rw-r--r--   0        0        0      181 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/pulse-line.svg
--rw-r--r--   0        0        0      311 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/stethoscope-fill.svg
--rw-r--r--   0        0        0      346 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/stethoscope-line.svg
--rw-r--r--   0        0        0      446 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/surgical-mask-fill.svg
--rw-r--r--   0        0        0      567 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg
--rw-r--r--   0        0        0      466 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/syringe-fill.svg
--rw-r--r--   0        0        0      486 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/syringe-line.svg
--rw-r--r--   0        0        0      237 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/test-tube-fill.svg
--rw-r--r--   0        0        0      264 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/test-tube-line.svg
--rw-r--r--   0        0        0      484 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/thermometer-fill.svg
--rw-r--r--   0        0        0      576 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg
--rw-r--r--   0        0        0     1055 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/virus-fill.svg
--rw-r--r--   0        0        0     1112 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/virus-line.svg
--rw-r--r--   0        0        0      552 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg
--rw-r--r--   0        0        0      594 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg
--rw-r--r--   0        0        0      591 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg
--rw-r--r--   0        0        0      411 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/edge-line.svg
--rw-r--r--   0        0        0      368 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/facebook-circle-fill.svg
--rw-r--r--   0        0        0      458 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/facebook-circle-line.svg
--rw-r--r--   0        0        0      708 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg
--rw-r--r--   0        0        0     1003 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg
--rw-r--r--   0        0        0      685 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg
--rw-r--r--   0        0        0      806 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg
--rw-r--r--   0        0        0      561 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg
--rw-r--r--   0        0        0      428 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-line.svg
--rw-r--r--   0        0        0      790 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/github-fill.svg
--rw-r--r--   0        0        0     1485 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/github-line.svg
--rw-r--r--   0        0        0      530 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/google-fill.svg
--rw-r--r--   0        0        0      371 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/google-line.svg
--rw-r--r--   0        0        0      965 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg
--rw-r--r--   0        0        0      796 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/ie-line.svg
--rw-r--r--   0        0        0      917 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg
--rw-r--r--   0        0        0     2014 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg
--rw-r--r--   0        0        0      552 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg
--rw-r--r--   0        0        0      366 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/linkedin-box-line.svg
--rw-r--r--   0        0        0      948 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg
--rw-r--r--   0        0        0     1259 2024-04-17 13:31:36.193838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg
--rw-r--r--   0        0        0      202 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/npmjs-fill.svg
--rw-r--r--   0        0        0      220 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/npmjs-line.svg
--rw-r--r--   0        0        0      331 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/remixicon-fill.svg
--rw-r--r--   0        0        0      391 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/remixicon-line.svg
--rw-r--r--   0        0        0      972 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg
--rw-r--r--   0        0        0      574 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/safari-line.svg
--rw-r--r--   0        0        0     1133 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg
--rw-r--r--   0        0        0      514 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/slack-line.svg
--rw-r--r--   0        0        0     1494 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg
--rw-r--r--   0        0        0     1848 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg
--rw-r--r--   0        0        0      398 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/telegram-fill.svg
--rw-r--r--   0        0        0      440 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/telegram-line.svg
--rw-r--r--   0        0        0     1726 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/threads-fill.svg
--rw-r--r--   0        0        0     1630 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/threads-line.svg
--rw-r--r--   0        0        0      332 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitch-fill.svg
--rw-r--r--   0        0        0      241 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitch-line.svg
--rw-r--r--   0        0        0      586 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg
--rw-r--r--   0        0        0      690 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg
--rw-r--r--   0        0        0      324 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitter-x-fill.svg
--rw-r--r--   0        0        0      254 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitter-x-line.svg
--rw-r--r--   0        0        0      726 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg
--rw-r--r--   0        0        0     1001 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg
--rw-r--r--   0        0        0      178 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/vuejs-fill.svg
--rw-r--r--   0        0        0      198 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/vuejs-line.svg
--rw-r--r--   0        0        0      418 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/youtube-fill.svg
--rw-r--r--   0        0        0      899 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg
--rw-r--r--   0        0        0      385 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/anchor-fill.svg
--rw-r--r--   0        0        0      350 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/anchor-line.svg
--rw-r--r--   0        0        0      359 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/bike-fill.svg
--rw-r--r--   0        0        0      359 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/bike-line.svg
--rw-r--r--   0        0        0      284 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/bus-fill.svg
--rw-r--r--   0        0        0      299 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/bus-line.svg
--rw-r--r--   0        0        0      372 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/car-fill.svg
--rw-r--r--   0        0        0      387 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/car-line.svg
--rw-r--r--   0        0        0      317 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/caravan-fill.svg
--rw-r--r--   0        0        0      383 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/caravan-line.svg
--rw-r--r--   0        0        0      253 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/charging-pile-2-fill.svg
--rw-r--r--   0        0        0      265 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/charging-pile-2-line.svg
--rw-r--r--   0        0        0      246 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/compass-3-fill.svg
--rw-r--r--   0        0        0      281 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/compass-3-line.svg
--rw-r--r--   0        0        0      222 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/cup-fill.svg
--rw-r--r--   0        0        0      264 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/cup-line.svg
--rw-r--r--   0        0        0      945 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/earth-fill.svg
--rw-r--r--   0        0        0      905 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/earth-line.svg
--rw-r--r--   0        0        0     2305 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/france-fill.svg
--rw-r--r--   0        0        0     4459 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/france-line.svg
--rw-r--r--   0        0        0      303 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/gas-station-fill.svg
--rw-r--r--   0        0        0      318 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/gas-station-line.svg
--rw-r--r--   0        0        0      179 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/goblet-fill.svg
--rw-r--r--   0        0        0      208 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/goblet-line.svg
--rw-r--r--   0        0        0      214 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/map-pin-2-fill.svg
--rw-r--r--   0        0        0      280 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/map-pin-2-line.svg
--rw-r--r--   0        0        0      277 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/map-pin-user-fill.svg
--rw-r--r--   0        0        0      363 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/map-pin-user-line.svg
--rw-r--r--   0        0        0      378 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/motorbike-fill.svg
--rw-r--r--   0        0        0      447 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/motorbike-line.svg
--rw-r--r--   0        0        0      256 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/passport-fill.svg
--rw-r--r--   0        0        0      272 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/passport-line.svg
--rw-r--r--   0        0        0      221 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/restaurant-fill.svg
--rw-r--r--   0        0        0      257 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/restaurant-line.svg
--rw-r--r--   0        0        0      381 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/road-map-fill.svg
--rw-r--r--   0        0        0      405 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/road-map-line.svg
--rw-r--r--   0        0        0      278 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/sailboat-fill.svg
--rw-r--r--   0        0        0      333 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/sailboat-line.svg
--rw-r--r--   0        0        0      580 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg
--rw-r--r--   0        0        0      562 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg
--rw-r--r--   0        0        0      351 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/signal-tower-fill.svg
--rw-r--r--   0        0        0      348 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/signal-tower-line.svg
--rw-r--r--   0        0        0      271 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/suitcase-2-fill.svg
--rw-r--r--   0        0        0      286 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/suitcase-2-line.svg
--rw-r--r--   0        0        0      374 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/taxi-fill.svg
--rw-r--r--   0        0        0      386 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/taxi-line.svg
--rw-r--r--   0        0        0      251 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/train-fill.svg
--rw-r--r--   0        0        0      293 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/train-line.svg
--rw-r--r--   0        0        0      160 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/align-left.svg
--rw-r--r--   0        0        0      253 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/camera-fill.svg
--rw-r--r--   0        0        0      311 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/camera-line.svg
--rw-r--r--   0        0        0      294 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/clapperboard-fill.svg
--rw-r--r--   0        0        0      312 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/clapperboard-line.svg
--rw-r--r--   0        0        0      334 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/equalizer-fill.svg
--rw-r--r--   0        0        0      505 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/equalizer-line.svg
--rw-r--r--   0        0        0      340 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/film-fill.svg
--rw-r--r--   0        0        0      355 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/film-line.svg
--rw-r--r--   0        0        0      184 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/fullscreen-line.svg
--rw-r--r--   0        0        0      388 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/gallery-fill.svg
--rw-r--r--   0        0        0      466 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/gallery-line.svg
--rw-r--r--   0        0        0      261 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/headphone-fill.svg
--rw-r--r--   0        0        0      300 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/headphone-line.svg
--rw-r--r--   0        0        0      394 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/image-add-fill.svg
--rw-r--r--   0        0        0      316 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/image-add-line.svg
--rw-r--r--   0        0        0      398 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/image-edit-fill.svg
--rw-r--r--   0        0        0      415 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/image-edit-line.svg
--rw-r--r--   0        0        0      307 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/image-fill.svg
--rw-r--r--   0        0        0      334 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/image-line.svg
--rw-r--r--   0        0        0      394 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/live-fill.svg
--rw-r--r--   0        0        0      408 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/live-line.svg
--rw-r--r--   0        0        0      269 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/mic-fill.svg
--rw-r--r--   0        0        0      320 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/mic-line.svg
--rw-r--r--   0        0        0      158 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/music-2-fill.svg
--rw-r--r--   0        0        0      226 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/music-2-line.svg
--rw-r--r--   0        0        0      154 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/notification-3-fill.svg
--rw-r--r--   0        0        0      208 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/notification-3-line.svg
--rw-r--r--   0        0        0      201 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/pause-circle-fill.svg
--rw-r--r--   0        0        0      236 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/pause-circle-line.svg
--rw-r--r--   0        0        0      281 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/play-circle-fill.svg
--rw-r--r--   0        0        0      313 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/play-circle-line.svg
--rw-r--r--   0        0        0      186 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/stop-circle-fill.svg
--rw-r--r--   0        0        0      221 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/stop-circle-line.svg
--rw-r--r--   0        0        0      403 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-down-fill.svg
--rw-r--r--   0        0        0      489 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-down-line.svg
--rw-r--r--   0        0        0      407 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-mute-fill.svg
--rw-r--r--   0        0        0      490 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-mute-line.svg
--rw-r--r--   0        0        0      551 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg
--rw-r--r--   0        0        0      630 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg
--rw-r--r--   0        0        0      334 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/leaf-fill.svg
--rw-r--r--   0        0        0      467 2024-04-17 13:31:36.197838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/leaf-line.svg
--rw-r--r--   0        0        0      253 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/lightbulb-fill.svg
--rw-r--r--   0        0        0      406 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/lightbulb-line.svg
--rw-r--r--   0        0        0      277 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/plant-fill.svg
--rw-r--r--   0        0        0      362 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/plant-line.svg
--rw-r--r--   0        0        0      573 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg
--rw-r--r--   0        0        0      558 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/recycle-line.svg
--rw-r--r--   0        0        0      454 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/scales-3-fill.svg
--rw-r--r--   0        0        0      552 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg
--rw-r--r--   0        0        0      258 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/seedling-fill.svg
--rw-r--r--   0        0        0      326 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/seedling-line.svg
--rw-r--r--   0        0        0      232 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/umbrella-fill.svg
--rw-r--r--   0        0        0      315 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/umbrella-line.svg
--rw-r--r--   0        0        0      209 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/add-circle-fill.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/add-circle-line.svg
--rw-r--r--   0        0        0      136 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/add-line.svg
--rw-r--r--   0        0        0      319 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/alarm-warning-fill.svg
--rw-r--r--   0        0        0      360 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/alarm-warning-line.svg
--rw-r--r--   0        0        0      224 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/alert-fill.svg
--rw-r--r--   0        0        0      257 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/alert-line.svg
--rw-r--r--   0        0        0      127 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-down-fill.svg
--rw-r--r--   0        0        0      188 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-down-line.svg
--rw-r--r--   0        0        0      120 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-down-s-fill.svg
--rw-r--r--   0        0        0      173 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-down-s-line.svg
--rw-r--r--   0        0        0      159 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-go-back-fill.svg
--rw-r--r--   0        0        0      213 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-go-back-line.svg
--rw-r--r--   0        0        0      161 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-fill.svg
--rw-r--r--   0        0        0      218 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-line.svg
--rw-r--r--   0        0        0      128 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-left-fill.svg
--rw-r--r--   0        0        0      184 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-left-line.svg
--rw-r--r--   0        0        0      119 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-left-s-fill.svg
--rw-r--r--   0        0        0      173 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-left-s-line.svg
--rw-r--r--   0        0        0      128 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-right-fill.svg
--rw-r--r--   0        0        0      189 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-right-line.svg
--rw-r--r--   0        0        0      118 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-right-s-fill.svg
--rw-r--r--   0        0        0      175 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-right-s-line.svg
--rw-r--r--   0        0        0      197 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-right-up-line.svg
--rw-r--r--   0        0        0      129 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-up-fill.svg
--rw-r--r--   0        0        0      186 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-up-line.svg
--rw-r--r--   0        0        0      117 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-up-s-fill.svg
--rw-r--r--   0        0        0      173 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/arrow-up-s-line.svg
--rw-r--r--   0        0        0      177 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/check-line.svg
--rw-r--r--   0        0        0      252 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/checkbox-circle-fill.svg
--rw-r--r--   0        0        0      288 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/checkbox-circle-line.svg
--rw-r--r--   0        0        0      252 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/checkbox-fill.svg
--rw-r--r--   0        0        0      288 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/checkbox-line.svg
--rw-r--r--   0        0        0      321 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/close-circle-fill.svg
--rw-r--r--   0        0        0      342 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/close-circle-line.svg
--rw-r--r--   0        0        0      210 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/close-line.svg
--rw-r--r--   0        0        0      189 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/delete-bin-fill.svg
--rw-r--r--   0        0        0      203 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/delete-bin-line.svg
--rw-r--r--   0        0        0      142 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/download-fill.svg
--rw-r--r--   0        0        0      198 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/download-line.svg
--rw-r--r--   0        0        0      203 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/error-warning-fill.svg
--rw-r--r--   0        0        0      238 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/error-warning-line.svg
--rw-r--r--   0        0        0      228 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/external-link-fill.svg
--rw-r--r--   0        0        0      230 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/external-link-line.svg
--rw-r--r--   0        0        0      281 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/eye-fill.svg
--rw-r--r--   0        0        0      380 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/eye-line.svg
--rw-r--r--   0        0        0      481 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/eye-off-fill.svg
--rw-r--r--   0        0        0      678 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg
--rw-r--r--   0        0        0      136 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/filter-fill.svg
--rw-r--r--   0        0        0      187 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/filter-line.svg
--rw-r--r--   0        0        0      196 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-first-line.svg
--rw-r--r--   0        0        0      197 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-line-double.svg
--rw-r--r--   0        0        0      377 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-down-circle-fill.svg
--rw-r--r--   0        0        0      201 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-last-line.svg
--rw-r--r--   0        0        0      201 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-line-double.svg
--rw-r--r--   0        0        0      377 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-up-circle-fill.svg
--rw-r--r--   0        0        0      327 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--capslock-line.svg
--rw-r--r--   0        0        0      329 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--equal-circle-fill.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--error-fill.svg
--rw-r--r--   0        0        0      309 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--error-line.svg
--rw-r--r--   0        0        0      237 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--info-fill.svg
--rw-r--r--   0        0        0      328 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--info-line.svg
--rw-r--r--   0        0        0      253 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--success-fill.svg
--rw-r--r--   0        0        0      289 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--success-line.svg
--rw-r--r--   0        0        0      482 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--theme-fill.svg
--rw-r--r--   0        0        0      225 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--warning-fill.svg
--rw-r--r--   0        0        0      258 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/fr--warning-line.svg
--rw-r--r--   0        0        0      205 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/information-fill.svg
--rw-r--r--   0        0        0      239 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/information-line.svg
--rw-r--r--   0        0        0      238 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/lock-fill.svg
--rw-r--r--   0        0        0      252 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/lock-line.svg
--rw-r--r--   0        0        0      252 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/lock-unlock-fill.svg
--rw-r--r--   0        0        0      268 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/lock-unlock-line.svg
--rw-r--r--   0        0        0      197 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/logout-box-r-fill.svg
--rw-r--r--   0        0        0      219 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/logout-box-r-line.svg
--rw-r--r--   0        0        0      145 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/menu-2-fill.svg
--rw-r--r--   0        0        0      145 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/menu-fill.svg
--rw-r--r--   0        0        0      248 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/more-fill.svg
--rw-r--r--   0        0        0      348 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/more-line.svg
--rw-r--r--   0        0        0      220 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/notification-badge-fill.svg
--rw-r--r--   0        0        0      288 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/notification-badge-line.svg
--rw-r--r--   0        0        0      311 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/question-fill.svg
--rw-r--r--   0        0        0      325 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/question-line.svg
--rw-r--r--   0        0        0      280 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/refresh-fill.svg
--rw-r--r--   0        0        0      244 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/refresh-line.svg
--rw-r--r--   0        0        0      247 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/search-fill.svg
--rw-r--r--   0        0        0      382 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/search-line.svg
--rw-r--r--   0        0        0      864 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg
--rw-r--r--   0        0        0     1599 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg
--rw-r--r--   0        0        0      241 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/shield-fill.svg
--rw-r--r--   0        0        0      332 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/shield-line.svg
--rw-r--r--   0        0        0      217 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/star-fill.svg
--rw-r--r--   0        0        0      333 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/star-line.svg
--rw-r--r--   0        0        0      203 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/star-s-fill.svg
--rw-r--r--   0        0        0      325 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/star-s-line.svg
--rw-r--r--   0        0        0      117 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/subtract-line.svg
--rw-r--r--   0        0        0      341 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/thumb-down-fill.svg
--rw-r--r--   0        0        0      442 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/thumb-down-line.svg
--rw-r--r--   0        0        0      340 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/thumb-up-fill.svg
--rw-r--r--   0        0        0      459 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/thumb-up-line.svg
--rw-r--r--   0        0        0      193 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/time-fill.svg
--rw-r--r--   0        0        0      226 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/time-line.svg
--rw-r--r--   0        0        0      201 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/timer-fill.svg
--rw-r--r--   0        0        0      236 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/timer-line.svg
--rw-r--r--   0        0        0      180 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/upload-2-fill.svg
--rw-r--r--   0        0        0      180 2024-04-17 13:31:36.201838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/upload-2-line.svg
--rw-r--r--   0        0        0      144 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/upload-fill.svg
--rw-r--r--   0        0        0      206 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/upload-line.svg
--rw-r--r--   0        0        0      279 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/zoom-in-fill.svg
--rw-r--r--   0        0        0      407 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/zoom-in-line.svg
--rw-r--r--   0        0        0      260 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/zoom-out-fill.svg
--rw-r--r--   0        0        0      388 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/zoom-out-line.svg
--rw-r--r--   0        0        0      337 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/account-circle-fill.svg
--rw-r--r--   0        0        0      462 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/account-circle-line.svg
--rw-r--r--   0        0        0      383 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/account-pin-circle-fill.svg
--rw-r--r--   0        0        0      575 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg
--rw-r--r--   0        0        0      279 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/admin-fill.svg
--rw-r--r--   0        0        0      349 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/admin-line.svg
--rw-r--r--   0        0        0      357 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/group-fill.svg
--rw-r--r--   0        0        0      462 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/group-line.svg
--rw-r--r--   0        0        0      279 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/parent-fill.svg
--rw-r--r--   0        0        0      413 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/parent-line.svg
--rw-r--r--   0        0        0      424 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/team-fill.svg
--rw-r--r--   0        0        0      750 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/team-line.svg
--rw-r--r--   0        0        0      235 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-add-fill.svg
--rw-r--r--   0        0        0      316 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-add-line.svg
--rw-r--r--   0        0        0      186 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-fill.svg
--rw-r--r--   0        0        0      314 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-heart-fill.svg
--rw-r--r--   0        0        0      439 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-heart-line.svg
--rw-r--r--   0        0        0      275 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-line.svg
--rw-r--r--   0        0        0      314 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-search-fill.svg
--rw-r--r--   0        0        0      384 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-search-line.svg
--rw-r--r--   0        0        0      529 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg
--rw-r--r--   0        0        0      625 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-setting-line.svg
--rw-r--r--   0        0        0      298 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-star-fill.svg
--rw-r--r--   0        0        0      367 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-star-line.svg
--rw-r--r--   0        0        0      167 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/cloudy-2-fill.svg
--rw-r--r--   0        0        0      291 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/cloudy-2-line.svg
--rw-r--r--   0        0        0      128 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/flashlight-fill.svg
--rw-r--r--   0        0        0      172 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/flashlight-line.svg
--rw-r--r--   0        0        0      226 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/moon-fill.svg
--rw-r--r--   0        0        0      286 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/moon-line.svg
--rw-r--r--   0        0        0      449 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/sun-fill.svg
--rw-r--r--   0        0        0      482 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/weather/sun-line.svg
--rw-r--r--   0        0        0      466 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/legacy/README.md
--rw-r--r--   0        0        0   127166 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js
--rw-r--r--   0        0        0     1524 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/README.md
--rw-r--r--   0        0        0     1588 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/account/README.md
--rw-r--r--   0        0        0     1576 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/account/login/README.md
--rw-r--r--   0        0        0     1764 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/account/register/README.md
--rw-r--r--   0        0        0      926 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/README.md
--rw-r--r--   0        0        0      701 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/not-found/README.md
--rw-r--r--   0        0        0       13 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/unavailable/README.md
--rw-r--r--   0        0        0      704 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/unexpected/README.md
--rw-r--r--   0        0        0      418 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/patch/README.md
--rw-r--r--   0        0        0      425 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/patch/patch.module.min.js
--rw-r--r--   0        0        0      459 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/patch/patch.nomodule.min.js
--rw-r--r--   0        0        0      363 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/README.md
--rw-r--r--   0        0        0      450 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/address/README.md
--rw-r--r--   0        0        0      666 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/civility/README.md
--rw-r--r--   0        0        0      674 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/company/README.md
--rw-r--r--   0        0        0      613 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/date/README.md
--rw-r--r--   0        0        0      640 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/name/README.md
--rw-r--r--   0        0        0      462 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/nationality/README.md
--rw-r--r--   0        0        0      855 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/scheme/README.md
--rw-r--r--   0        0        0    12280 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/scheme/scheme.min.css
--rw-r--r--   0        0        0     3274 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/scheme/scheme.module.min.js
--rw-r--r--   0        0        0     1003 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/README.md
--rw-r--r--   0        0        0      421 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/README.md
--rw-r--r--   0        0        0    32005 2024-04-17 13:31:36.205839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css
--rw-r--r--   0        0        0    39455 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css
--rw-r--r--   0        0        0   103161 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.min.css
--rw-r--r--   0        0        0    31959 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.print.min.css
--rw-r--r--   0        0        0      748 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/README.md
--rw-r--r--   0        0        0      794 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md
--rw-r--r--   0        0        0     3037 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css
--rw-r--r--   0        0        0     4371 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css
--rw-r--r--   0        0        0     7179 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css
--rw-r--r--   0        0        0      788 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md
--rw-r--r--   0        0        0     8089 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css
--rw-r--r--   0        0        0    12244 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css
--rw-r--r--   0        0        0    20104 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css
--rw-r--r--   0        0        0      818 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md
--rw-r--r--   0        0        0     3273 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css
--rw-r--r--   0        0        0     4675 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css
--rw-r--r--   0        0        0     7719 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css
--rw-r--r--   0        0        0      776 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md
--rw-r--r--   0        0        0     5505 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css
--rw-r--r--   0        0        0     8001 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css
--rw-r--r--   0        0        0    13277 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css
--rw-r--r--   0        0        0      806 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md
--rw-r--r--   0        0        0     3955 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css
--rw-r--r--   0        0        0     5639 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css
--rw-r--r--   0        0        0     9365 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css
--rw-r--r--   0        0        0      776 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md
--rw-r--r--   0        0        0     4811 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css
--rw-r--r--   0        0        0     7133 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css
--rw-r--r--   0        0        0    11715 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css
--rw-r--r--   0        0        0      788 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md
--rw-r--r--   0        0        0     4307 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css
--rw-r--r--   0        0        0     6435 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css
--rw-r--r--   0        0        0    10513 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css
--rw-r--r--   0        0        0      776 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md
--rw-r--r--   0        0        0     3577 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css
--rw-r--r--   0        0        0     5397 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css
--rw-r--r--   0        0        0     8745 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css
--rw-r--r--   0        0        0      782 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md
--rw-r--r--   0        0        0     2585 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css
--rw-r--r--   0        0        0     3578 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css
--rw-r--r--   0        0        0     5934 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css
--rw-r--r--   0        0        0      776 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md
--rw-r--r--   0        0        0     5281 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css
--rw-r--r--   0        0        0     7550 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css
--rw-r--r--   0        0        0    12602 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css
--rw-r--r--   0        0        0      764 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md
--rw-r--r--   0        0        0     8677 2024-04-17 13:31:36.209838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css
--rw-r--r--   0        0        0    13727 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css
--rw-r--r--   0        0        0    22175 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css
--rw-r--r--   0        0        0      758 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md
--rw-r--r--   0        0        0     6299 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css
--rw-r--r--   0        0        0     9185 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css
--rw-r--r--   0        0        0    15255 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css
--rw-r--r--   0        0        0      770 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md
--rw-r--r--   0        0        0     6786 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css
--rw-r--r--   0        0        0    10313 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css
--rw-r--r--   0        0        0    16870 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css
--rw-r--r--   0        0        0      776 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md
--rw-r--r--   0        0        0     2013 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css
--rw-r--r--   0        0        0     2751 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css
--rw-r--r--   0        0        0     4535 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css
--rw-r--r--   0        0        0      776 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md
--rw-r--r--   0        0        0    20774 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css
--rw-r--r--   0        0        0    33241 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css
--rw-r--r--   0        0        0    53786 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css
--rw-r--r--   0        0        0      764 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md
--rw-r--r--   0        0        0     3921 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css
--rw-r--r--   0        0        0     5623 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css
--rw-r--r--   0        0        0     9315 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css
--rw-r--r--   0        0        0      782 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md
--rw-r--r--   0        0        0     1485 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css
--rw-r--r--   0        0        0     2063 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css
--rw-r--r--   0        0        0     3319 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css
--rw-r--r--   0        0        0    87540 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css
--rw-r--r--   0        0        0   133768 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css
--rw-r--r--   0        0        0   221079 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons.min.css
--rw-r--r--   0        0        0      372 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/README.md
--rw-r--r--   0        0        0      402 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-buildings/README.md
--rw-r--r--   0        0        0      396 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-digital/README.md
--rw-r--r--   0        0        0      399 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-document/README.md
--rw-r--r--   0        0        0      408 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-environment/README.md
--rw-r--r--   0        0        0      393 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-health/README.md
--rw-r--r--   0        0        0      411 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-institutions/README.md
--rw-r--r--   0        0        0      396 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-leisure/README.md
--rw-r--r--   0        0        0      384 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-map/README.md
--rw-r--r--   0        0        0      393 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/pictograms/pictograms-system/README.md
--rw-r--r--   0        0        0   117145 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.legacy.min.css
--rw-r--r--   0        0        0   168600 2024-04-17 13:31:36.213838 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.main.min.css
--rw-r--r--   0        0        0   317346 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.min.css
--rw-r--r--   0        0        0    31959 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.print.min.css
--rw-r--r--   0        0        0     3845 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/static/js/formsets.js
--rw-r--r--   0        0        0      199 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/django/forms/errors/dict/ul.html
--rw-r--r--   0        0        0      181 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/django/forms/errors/list/ul.html
--rw-r--r--   0        0        0      554 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/checkbox_option.html
--rw-r--r--   0        0        0      644 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/input_option.html
--rw-r--r--   0        0        0      222 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/multiple_input.html
--rw-r--r--   0        0        0      551 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/radio_option.html
--rw-r--r--   0        0        0      407 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/accordion.html
--rw-r--r--   0        0        0      138 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/accordion_group.html
--rw-r--r--   0        0        0      699 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/alert.html
--rw-r--r--   0        0        0      108 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/badge.html
--rw-r--r--   0        0        0      148 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/badge_group.html
--rw-r--r--   0        0        0     1673 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/base.html
--rw-r--r--   0        0        0      851 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/breadcrumb.html
--rw-r--r--   0        0        0      316 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/button.html
--rw-r--r--   0        0        0      211 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/button_group.html
--rw-r--r--   0        0        0      635 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/callout.html
--rw-r--r--   0        0        0     3359 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/card.html
--rw-r--r--   0        0        0     1214 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/consent.html
--rw-r--r--   0        0        0     1366 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/content.html
--rw-r--r--   0        0        0      707 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/favicon.html
--rw-r--r--   0        0        0     2069 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/follow.html
--rw-r--r--   0        0        0     5856 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/footer.html
--rw-r--r--   0        0        0     2273 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_base.html
--rw-r--r--   0        0        0      826 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/checkbox_snippet.html
--rw-r--r--   0        0        0     1414 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html
--rw-r--r--   0        0        0      471 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/field_snippet.html
--rw-r--r--   0        0        0      984 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/input_snippet.html
--rw-r--r--   0        0        0     1028 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/radioselect_snippet.html
--rw-r--r--   0        0        0      335 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/form_snippet.html
--rw-r--r--   0        0        0     1845 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/formset_base.html
--rw-r--r--   0        0        0      999 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/france_connect.html
--rw-r--r--   0        0        0      469 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/global_css.html
--rw-r--r--   0        0        0      433 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/global_js.html
--rw-r--r--   0        0        0     4619 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/header.html
--rw-r--r--   0        0        0      205 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/highlight.html
--rw-r--r--   0        0        0      565 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/input.html
--rw-r--r--   0        0        0      427 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/link.html
--rw-r--r--   0        0        0      576 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/notice.html
--rw-r--r--   0        0        0     2187 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/pagination.html
--rw-r--r--   0        0        0     1208 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/quote.html
--rw-r--r--   0        0        0      892 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/select.html
--rw-r--r--   0        0        0     3969 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/sidemenu.html
--rw-r--r--   0        0        0      403 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/skiplinks.html
--rw-r--r--   0        0        0      766 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/stepper.html
--rw-r--r--   0        0        0      420 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/summary.html
--rw-r--r--   0        0        0      264 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/summary_list.html
--rw-r--r--   0        0        0      620 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/table.html
--rw-r--r--   0        0        0      745 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/tag.html
--rw-r--r--   0        0        0     3939 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/theme_modale.html
--rw-r--r--   0        0        0     2127 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/tile.html
--rw-r--r--   0        0        0      734 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/toggle.html
--rw-r--r--   0        0        0      524 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/tooltip.html
--rw-r--r--   0        0        0     1936 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templates/dsfr/transcription.html
--rw-r--r--   0        0        0        0 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templatetags/__init__.py
--rw-r--r--   0        0        0    43549 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/templatetags/dsfr_tags.py
--rw-r--r--   0        0        0        0 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/test/__init__.py
--rw-r--r--   0        0        0     2064 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/test/test_config.py
--rw-r--r--   0        0        0    42738 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/test/test_templatetags.py
--rw-r--r--   0        0        0     1116 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/test/test_utils.py
--rw-r--r--   0        0        0     4149 2024-04-17 13:31:36.217839 django_dsfr-1.1.1/dsfr/utils.py
--rw-r--r--   0        0        0     2213 2024-04-17 13:31:36.221839 django_dsfr-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4090 1970-01-01 00:00:00.000000 django_dsfr-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1235 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2567 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/__init__.py
+-rw-r--r--   0        0        0     1650 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/admin.py
+-rw-r--r--   0        0        0      193 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/apps.py
+-rw-r--r--   0        0        0     1545 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/checksums.py
+-rw-r--r--   0        0        0     1733 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/constants.py
+-rw-r--r--   0        0        0      421 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/context_processors.py
+-rw-r--r--   0        0        0      455 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/fixtures/init.json
+-rw-r--r--   0        0        0     1684 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/forms.py
+-rw-r--r--   0        0        0     6899 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10506 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/management/commands/__init__.py
+-rw-r--r--   0        0        0     2189 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/management/commands/integrity_checksums.py
+-rw-r--r--   0        0        0     1508 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/management/commands/make_icon_picker_files.py
+-rw-r--r--   0        0        0     2385 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/management/commands/trim_dist.py
+-rw-r--r--   0        0        0     3301 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2885 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0002_auto_20211209_1557.py
+-rw-r--r--   0        0        0      710 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py
+-rw-r--r--   0        0        0     1765 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0004_dsfrconfig_beta_tag_dsfrconfig_operator_logo_alt_and_more.py
+-rw-r--r--   0        0        0      579 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0005_dsfrconfig_notice.py
+-rw-r--r--   0        0        0      621 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0006_alter_dsfrconfig_accessibility_status.py
+-rw-r--r--   0        0        0     2326 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0007_dsfrconfig_newsletter_description_and_more.py
+-rw-r--r--   0        0        0     5872 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/0008_alter_dsfrsocialmedia_options_dsfrconfig_language_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/migrations/__init__.py
+-rw-r--r--   0        0        0     4415 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/models.py
+-rw-r--r--   0        0        0     6152 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/css/dsfr-code.css
+-rw-r--r--   0        0        0      125 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/css/dsfr-django-overrides.css
+-rw-r--r--   0        0        0      278 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/README.md
+-rw-r--r--   0        0        0      465 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-buildings.json
+-rw-r--r--   0        0        0     1063 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-business.json
+-rw-r--r--   0        0        0      533 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-communication.json
+-rw-r--r--   0        0        0      793 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-design.json
+-rw-r--r--   0        0        0      671 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-development.json
+-rw-r--r--   0        0        0      639 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-device.json
+-rw-r--r--   0        0        0      575 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-document.json
+-rw-r--r--   0        0        0      401 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-editor.json
+-rw-r--r--   0        0        0      454 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-finance.json
+-rw-r--r--   0        0        0      843 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-health.json
+-rw-r--r--   0        0        0      917 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-logo.json
+-rw-r--r--   0        0        0      897 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-map.json
+-rw-r--r--   0        0        0      814 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-media.json
+-rw-r--r--   0        0        0      337 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-others.json
+-rw-r--r--   0        0        0     2158 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-system.json
+-rw-r--r--   0        0        0      537 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-user.json
+-rw-r--r--   0        0        0      237 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-weather.json
+-rw-r--r--   0        0        0      632 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0        0        0      872 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/images/star-of-life-solid.svg
+-rw-r--r--   0        0        0      645 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/images/xmark-solid.svg
+-rw-r--r--   0        0        0    22397 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.js
+-rw-r--r--   0        0        0    11414 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0        0        0    10670 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/scss/universal-icon-picker.scss
+-rw-r--r--   0        0        0    10767 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.css
+-rw-r--r--   0        0        0     9324 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.min.css
+-rw-r--r--   0        0        0      469 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/README.md
+-rw-r--r--   0        0        0     3461 2024-04-25 13:02:07.280325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/analytics/README.md
+-rw-r--r--   0        0        0    69425 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/analytics/analytics.module.min.js
+-rw-r--r--   0        0        0    96039 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/analytics/analytics.nomodule.min.js
+-rw-r--r--   0        0        0    16409 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/background/ovoid.svg
+-rw-r--r--   0        0        0     3884 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/dark.svg
+-rw-r--r--   0        0        0     4750 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/light.svg
+-rw-r--r--   0        0        0     5712 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/city-hall.svg
+-rw-r--r--   0        0        0     6612 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/factory.svg
+-rw-r--r--   0        0        0     3564 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/house.svg
+-rw-r--r--   0        0        0    10932 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/nuclear-plant.svg
+-rw-r--r--   0        0        0     5534 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/school.svg
+-rw-r--r--   0        0        0     5409 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/application.svg
+-rw-r--r--   0        0        0     4327 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/avatar.svg
+-rw-r--r--   0        0        0     4158 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/calendar.svg
+-rw-r--r--   0        0        0     4015 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/coding.svg
+-rw-r--r--   0        0        0     5502 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/data-visualization.svg
+-rw-r--r--   0        0        0     7230 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/internet.svg
+-rw-r--r--   0        0        0     3993 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/mail-send.svg
+-rw-r--r--   0        0        0     3191 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/search.svg
+-rw-r--r--   0        0        0     4823 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/contract.svg
+-rw-r--r--   0        0        0     2599 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document-add.svg
+-rw-r--r--   0        0        0     3905 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document-download.svg
+-rw-r--r--   0        0        0     3201 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document-signature.svg
+-rw-r--r--   0        0        0     2453 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document.svg
+-rw-r--r--   0        0        0     4716 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/driving-licence.svg
+-rw-r--r--   0        0        0     4210 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/national-identity-card.svg
+-rw-r--r--   0        0        0     3572 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/passport.svg
+-rw-r--r--   0        0        0    10659 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/tax-stamp.svg
+-rw-r--r--   0        0        0     5360 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/vehicle-registration.svg
+-rw-r--r--   0        0        0     8630 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/environment.svg
+-rw-r--r--   0        0        0     5177 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/food.svg
+-rw-r--r--   0        0        0     6131 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/grocery.svg
+-rw-r--r--   0        0        0    10973 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/human-cooperation.svg
+-rw-r--r--   0        0        0     5704 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/leaf.svg
+-rw-r--r--   0        0        0     2809 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/moon.svg
+-rw-r--r--   0        0        0     4263 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/mountain.svg
+-rw-r--r--   0        0        0     3555 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/sun.svg
+-rw-r--r--   0        0        0     6161 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/tree.svg
+-rw-r--r--   0        0        0     7177 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/health.svg
+-rw-r--r--   0        0        0     3577 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/hospital.svg
+-rw-r--r--   0        0        0     7720 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/vaccine.svg
+-rw-r--r--   0        0        0     8264 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/virus.svg
+-rw-r--r--   0        0        0     8682 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/firefighter.svg
+-rw-r--r--   0        0        0     5880 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/gendarmerie.svg
+-rw-r--r--   0        0        0     4778 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/justice.svg
+-rw-r--r--   0        0        0    16555 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/money.svg
+-rw-r--r--   0        0        0     8621 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/police.svg
+-rw-r--r--   0        0        0     7856 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/book.svg
+-rw-r--r--   0        0        0     4138 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/community.svg
+-rw-r--r--   0        0        0     6782 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/culture.svg
+-rw-r--r--   0        0        0     4973 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/digital-art.svg
+-rw-r--r--   0        0        0     6890 2024-04-25 13:02:07.284325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/paint.svg
+-rw-r--r--   0        0        0     6799 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/airport.svg
+-rw-r--r--   0        0        0    15123 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/location-france.svg
+-rw-r--r--   0        0        0     4427 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/luggage.svg
+-rw-r--r--   0        0        0     7293 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/map.svg
+-rw-r--r--   0        0        0     2791 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/connection-lost.svg
+-rw-r--r--   0        0        0     2098 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/error.svg
+-rw-r--r--   0        0        0     3506 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/information.svg
+-rw-r--r--   0        0        0     4103 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/notification.svg
+-rw-r--r--   0        0        0     2592 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/padlock.svg
+-rw-r--r--   0        0        0     1985 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/success.svg
+-rw-r--r--   0        0        0    15162 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/system.svg
+-rw-r--r--   0        0        0     4442 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/technical-error.svg
+-rw-r--r--   0        0        0     1577 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/warning.svg
+-rw-r--r--   0        0        0    15015 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/system.svg
+-rw-r--r--   0        0        0      964 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/README.md
+-rw-r--r--   0        0        0     1143 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/README.md
+-rw-r--r--   0        0        0     1085 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css
+-rw-r--r--   0        0        0     2396 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css
+-rw-r--r--   0        0        0     3635 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.min.css
+-rw-r--r--   0        0        0     1129 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js
+-rw-r--r--   0        0        0     1734 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js
+-rw-r--r--   0        0        0      512 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.print.min.css
+-rw-r--r--   0        0        0      749 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/README.md
+-rw-r--r--   0        0        0     2317 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css
+-rw-r--r--   0        0        0     5141 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.main.min.css
+-rw-r--r--   0        0        0     8387 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.min.css
+-rw-r--r--   0        0        0     1287 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.print.min.css
+-rw-r--r--   0        0        0      685 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/README.md
+-rw-r--r--   0        0        0     3117 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css
+-rw-r--r--   0        0        0    10533 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.main.min.css
+-rw-r--r--   0        0        0    14869 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.min.css
+-rw-r--r--   0        0        0     1577 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.print.min.css
+-rw-r--r--   0        0        0     1176 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/README.md
+-rw-r--r--   0        0        0      858 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css
+-rw-r--r--   0        0        0     3015 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css
+-rw-r--r--   0        0        0     3772 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css
+-rw-r--r--   0        0        0     1600 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js
+-rw-r--r--   0        0        0     2179 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js
+-rw-r--r--   0        0        0      257 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.print.min.css
+-rw-r--r--   0        0        0     1114 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/README.md
+-rw-r--r--   0        0        0    10821 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.legacy.min.css
+-rw-r--r--   0        0        0    29226 2024-04-25 13:02:07.288325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.main.min.css
+-rw-r--r--   0        0        0    44554 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.min.css
+-rw-r--r--   0        0        0      514 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.module.min.js
+-rw-r--r--   0        0        0      536 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js
+-rw-r--r--   0        0        0     4865 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.print.min.css
+-rw-r--r--   0        0        0      790 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/README.md
+-rw-r--r--   0        0        0     2398 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css
+-rw-r--r--   0        0        0     7111 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.main.min.css
+-rw-r--r--   0        0        0    11273 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.min.css
+-rw-r--r--   0        0        0     2122 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.print.min.css
+-rw-r--r--   0        0        0     1492 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/README.md
+-rw-r--r--   0        0        0     2785 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.legacy.min.css
+-rw-r--r--   0        0        0    10531 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.main.min.css
+-rw-r--r--   0        0        0    14122 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.min.css
+-rw-r--r--   0        0        0      825 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.module.min.js
+-rw-r--r--   0        0        0     1093 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.nomodule.min.js
+-rw-r--r--   0        0        0     1164 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.print.min.css
+-rw-r--r--   0        0        0      971 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/README.md
+-rw-r--r--   0        0        0     9140 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css
+-rw-r--r--   0        0        0    10611 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css
+-rw-r--r--   0        0        0    19908 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css
+-rw-r--r--   0        0        0     8689 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.print.min.css
+-rw-r--r--   0        0        0   115826 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.legacy.min.css
+-rw-r--r--   0        0        0   323926 2024-04-25 13:02:07.292325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.main.min.css
+-rw-r--r--   0        0        0   503919 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.min.css
+-rw-r--r--   0        0        0    47336 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.module.min.js
+-rw-r--r--   0        0        0    63661 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.nomodule.min.js
+-rw-r--r--   0        0        0    74103 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.print.min.css
+-rw-r--r--   0        0        0      733 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/README.md
+-rw-r--r--   0        0        0      576 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css
+-rw-r--r--   0        0        0     6927 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.main.min.css
+-rw-r--r--   0        0        0     7571 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.min.css
+-rw-r--r--   0        0        0      426 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.print.min.css
+-rw-r--r--   0        0        0     1628 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/README.md
+-rw-r--r--   0        0        0     1685 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css
+-rw-r--r--   0        0        0     6729 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.main.min.css
+-rw-r--r--   0        0        0     8897 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.min.css
+-rw-r--r--   0        0        0      841 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.print.min.css
+-rw-r--r--   0        0        0     1056 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/README.md
+-rw-r--r--   0        0        0     1125 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.legacy.min.css
+-rw-r--r--   0        0        0     2593 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.main.min.css
+-rw-r--r--   0        0        0     3811 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.min.css
+-rw-r--r--   0        0        0      451 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.print.min.css
+-rw-r--r--   0        0        0     1640 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/display/README.md
+-rw-r--r--   0        0        0     1332 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/display/display.module.min.js
+-rw-r--r--   0        0        0     1843 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js
+-rw-r--r--   0        0        0      781 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/download/README.md
+-rw-r--r--   0        0        0     3529 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/download/download.min.css
+-rw-r--r--   0        0        0     1183 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/README.md
+-rw-r--r--   0        0        0     6194 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css
+-rw-r--r--   0        0        0    10271 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.main.min.css
+-rw-r--r--   0        0        0    17329 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.min.css
+-rw-r--r--   0        0        0     1222 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.print.min.css
+-rw-r--r--   0        0        0      934 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/README.md
+-rw-r--r--   0        0        0     1119 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css
+-rw-r--r--   0        0        0     7718 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.main.min.css
+-rw-r--r--   0        0        0     9214 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.min.css
+-rw-r--r--   0        0        0      735 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.print.min.css
+-rw-r--r--   0        0        0      563 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/README.md
+-rw-r--r--   0        0        0     3650 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.legacy.min.css
+-rw-r--r--   0        0        0     9618 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.main.min.css
+-rw-r--r--   0        0        0    14995 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.min.css
+-rw-r--r--   0        0        0     2085 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.print.min.css
+-rw-r--r--   0        0        0     2240 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/README.md
+-rw-r--r--   0        0        0     7240 2024-04-25 13:02:07.296325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.legacy.min.css
+-rw-r--r--   0        0        0    17301 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.main.min.css
+-rw-r--r--   0        0        0    29441 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.min.css
+-rw-r--r--   0        0        0     2618 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.module.min.js
+-rw-r--r--   0        0        0     3201 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js
+-rw-r--r--   0        0        0     5258 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.print.min.css
+-rw-r--r--   0        0        0      702 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/README.md
+-rw-r--r--   0        0        0     1877 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css
+-rw-r--r--   0        0        0     3046 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css
+-rw-r--r--   0        0        0     6224 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.min.css
+-rw-r--r--   0        0        0     1659 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.print.min.css
+-rw-r--r--   0        0        0      560 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/README.md
+-rw-r--r--   0        0        0      837 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/README.md
+-rw-r--r--   0        0        0     1927 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.legacy.min.css
+-rw-r--r--   0        0        0     5557 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.main.min.css
+-rw-r--r--   0        0        0     8684 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.min.css
+-rw-r--r--   0        0        0     1665 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.print.min.css
+-rw-r--r--   0        0        0      795 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-email/README.md
+-rw-r--r--   0        0        0      790 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-tel/README.md
+-rw-r--r--   0        0        0     1999 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.legacy.min.css
+-rw-r--r--   0        0        0     5629 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.main.min.css
+-rw-r--r--   0        0        0     8828 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.min.css
+-rw-r--r--   0        0        0     1665 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.print.min.css
+-rw-r--r--   0        0        0      786 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/README.md
+-rw-r--r--   0        0        0     1401 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.legacy.min.css
+-rw-r--r--   0        0        0    11309 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.main.min.css
+-rw-r--r--   0        0        0    12645 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.min.css
+-rw-r--r--   0        0        0      293 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.print.min.css
+-rw-r--r--   0        0        0      435 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/README.md
+-rw-r--r--   0        0        0      381 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css
+-rw-r--r--   0        0        0    11536 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/logo.main.min.css
+-rw-r--r--   0        0        0    11791 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/logo.min.css
+-rw-r--r--   0        0        0      232 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/logo.print.min.css
+-rw-r--r--   0        0        0     1391 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/README.md
+-rw-r--r--   0        0        0      584 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css
+-rw-r--r--   0        0        0     2839 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.main.min.css
+-rw-r--r--   0        0        0     3550 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.min.css
+-rw-r--r--   0        0        0     7482 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.module.min.js
+-rw-r--r--   0        0        0     9236 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js
+-rw-r--r--   0        0        0      485 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.print.min.css
+-rw-r--r--   0        0        0     1412 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/README.md
+-rw-r--r--   0        0        0     2559 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css
+-rw-r--r--   0        0        0     6849 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css
+-rw-r--r--   0        0        0     9221 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.min.css
+-rw-r--r--   0        0        0     3656 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js
+-rw-r--r--   0        0        0     4678 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js
+-rw-r--r--   0        0        0      171 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.print.min.css
+-rw-r--r--   0        0        0      827 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/README.md
+-rw-r--r--   0        0        0      871 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css
+-rw-r--r--   0        0        0     1890 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.main.min.css
+-rw-r--r--   0        0        0     2649 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.min.css
+-rw-r--r--   0        0        0      246 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.print.min.css
+-rw-r--r--   0        0        0      706 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/README.md
+-rw-r--r--   0        0        0     2870 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css
+-rw-r--r--   0        0        0     9995 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css
+-rw-r--r--   0        0        0    13186 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.min.css
+-rw-r--r--   0        0        0      679 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.print.min.css
+-rw-r--r--   0        0        0     1462 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/README.md
+-rw-r--r--   0        0        0     2594 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.legacy.min.css
+-rw-r--r--   0        0        0     3658 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.main.min.css
+-rw-r--r--   0        0        0     7200 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.min.css
+-rw-r--r--   0        0        0     2564 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.module.min.js
+-rw-r--r--   0        0        0     3887 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.nomodule.min.js
+-rw-r--r--   0        0        0     2413 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.print.min.css
+-rw-r--r--   0        0        0      749 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/README.md
+-rw-r--r--   0        0        0     1656 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css
+-rw-r--r--   0        0        0     3961 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.main.min.css
+-rw-r--r--   0        0        0     6413 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.min.css
+-rw-r--r--   0        0        0     1154 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.print.min.css
+-rw-r--r--   0        0        0      894 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/README.md
+-rw-r--r--   0        0        0     9327 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css
+-rw-r--r--   0        0        0    19243 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.main.min.css
+-rw-r--r--   0        0        0    36596 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.min.css
+-rw-r--r--   0        0        0     8384 2024-04-25 13:02:07.300325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.print.min.css
+-rw-r--r--   0        0        0     1260 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/README.md
+-rw-r--r--   0        0        0     4633 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.legacy.min.css
+-rw-r--r--   0        0        0     6745 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.main.min.css
+-rw-r--r--   0        0        0    11149 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.min.css
+-rw-r--r--   0        0        0    10167 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.module.min.js
+-rw-r--r--   0        0        0    13729 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.nomodule.min.js
+-rw-r--r--   0        0        0      976 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/README.md
+-rw-r--r--   0        0        0     1222 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.legacy.min.css
+-rw-r--r--   0        0        0     2831 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.main.min.css
+-rw-r--r--   0        0        0     4558 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.min.css
+-rw-r--r--   0        0        0      863 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.print.min.css
+-rw-r--r--   0        0        0     1307 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/README.md
+-rw-r--r--   0        0        0      942 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.legacy.min.css
+-rw-r--r--   0        0        0     5053 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.main.min.css
+-rw-r--r--   0        0        0     5766 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.min.css
+-rw-r--r--   0        0        0     1849 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.module.min.js
+-rw-r--r--   0        0        0     2375 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.nomodule.min.js
+-rw-r--r--   0        0        0      753 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/README.md
+-rw-r--r--   0        0        0     1630 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.legacy.min.css
+-rw-r--r--   0        0        0     3178 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.main.min.css
+-rw-r--r--   0        0        0     5937 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.min.css
+-rw-r--r--   0        0        0     1487 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.print.min.css
+-rw-r--r--   0        0        0      896 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/README.md
+-rw-r--r--   0        0        0     2879 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.legacy.min.css
+-rw-r--r--   0        0        0     6655 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.main.min.css
+-rw-r--r--   0        0        0    10075 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.min.css
+-rw-r--r--   0        0        0      899 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.print.min.css
+-rw-r--r--   0        0        0     1150 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/README.md
+-rw-r--r--   0        0        0     1842 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css
+-rw-r--r--   0        0        0     5902 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css
+-rw-r--r--   0        0        0     8693 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css
+-rw-r--r--   0        0        0     1171 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js
+-rw-r--r--   0        0        0     1780 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js
+-rw-r--r--   0        0        0     1307 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.print.min.css
+-rw-r--r--   0        0        0      844 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/README.md
+-rw-r--r--   0        0        0      466 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css
+-rw-r--r--   0        0        0     1307 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css
+-rw-r--r--   0        0        0     1620 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css
+-rw-r--r--   0        0        0      205 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/skiplink.print.min.css
+-rw-r--r--   0        0        0      723 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/README.md
+-rw-r--r--   0        0        0      788 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css
+-rw-r--r--   0        0        0     3603 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css
+-rw-r--r--   0        0        0     4643 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.min.css
+-rw-r--r--   0        0        0      610 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.print.min.css
+-rw-r--r--   0        0        0      707 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/README.md
+-rw-r--r--   0        0        0      445 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css
+-rw-r--r--   0        0        0     1186 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/summary.main.min.css
+-rw-r--r--   0        0        0     1513 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/summary.min.css
+-rw-r--r--   0        0        0      240 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/summary.print.min.css
+-rw-r--r--   0        0        0     1092 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/README.md
+-rw-r--r--   0        0        0     1926 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css
+-rw-r--r--   0        0        0     6080 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.main.min.css
+-rw-r--r--   0        0        0     8486 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.min.css
+-rw-r--r--   0        0        0     5911 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.module.min.js
+-rw-r--r--   0        0        0     7820 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js
+-rw-r--r--   0        0        0      838 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.print.min.css
+-rw-r--r--   0        0        0     1084 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/README.md
+-rw-r--r--   0        0        0     6961 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.legacy.min.css
+-rw-r--r--   0        0        0    20082 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.main.min.css
+-rw-r--r--   0        0        0    33509 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.min.css
+-rw-r--r--   0        0        0     2303 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.module.min.js
+-rw-r--r--   0        0        0     3220 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js
+-rw-r--r--   0        0        0     6824 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.print.min.css
+-rw-r--r--   0        0        0     1122 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/README.md
+-rw-r--r--   0        0        0    13862 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css
+-rw-r--r--   0        0        0    17311 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.main.min.css
+-rw-r--r--   0        0        0    42083 2024-04-25 13:02:07.304325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.min.css
+-rw-r--r--   0        0        0     1082 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.module.min.js
+-rw-r--r--   0        0        0     1376 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js
+-rw-r--r--   0        0        0    11268 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.print.min.css
+-rw-r--r--   0        0        0     1119 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/README.md
+-rw-r--r--   0        0        0     2838 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css
+-rw-r--r--   0        0        0     9417 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.main.min.css
+-rw-r--r--   0        0        0    13352 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.min.css
+-rw-r--r--   0        0        0      785 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.module.min.js
+-rw-r--r--   0        0        0     1052 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.nomodule.min.js
+-rw-r--r--   0        0        0     1455 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.print.min.css
+-rw-r--r--   0        0        0     1205 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/README.md
+-rw-r--r--   0        0        0     4846 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css
+-rw-r--r--   0        0        0    11190 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css
+-rw-r--r--   0        0        0    20338 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.min.css
+-rw-r--r--   0        0        0     1291 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js
+-rw-r--r--   0        0        0     1998 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js
+-rw-r--r--   0        0        0     4660 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.print.min.css
+-rw-r--r--   0        0        0     1038 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/README.md
+-rw-r--r--   0        0        0     1206 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.legacy.min.css
+-rw-r--r--   0        0        0     2311 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.main.min.css
+-rw-r--r--   0        0        0     3534 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.min.css
+-rw-r--r--   0        0        0     2785 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.module.min.js
+-rw-r--r--   0        0        0     3728 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.nomodule.min.js
+-rw-r--r--   0        0        0      375 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.print.min.css
+-rw-r--r--   0        0        0     1276 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/README.md
+-rw-r--r--   0        0        0     1421 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.legacy.min.css
+-rw-r--r--   0        0        0     5128 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.main.min.css
+-rw-r--r--   0        0        0     6684 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.min.css
+-rw-r--r--   0        0        0      617 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.module.min.js
+-rw-r--r--   0        0        0      974 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.nomodule.min.js
+-rw-r--r--   0        0        0      493 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.print.min.css
+-rw-r--r--   0        0        0     1441 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/README.md
+-rw-r--r--   0        0        0     1082 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css
+-rw-r--r--   0        0        0     2642 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.main.min.css
+-rw-r--r--   0        0        0     3808 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.min.css
+-rw-r--r--   0        0        0      632 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.print.min.css
+-rw-r--r--   0        0        0      574 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/README.md
+-rw-r--r--   0        0        0      799 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/upload.main.min.css
+-rw-r--r--   0        0        0      858 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/upload.min.css
+-rw-r--r--   0        0        0      188 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/upload.print.min.css
+-rw-r--r--   0        0        0     2503 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/README.md
+-rw-r--r--   0        0        0     3496 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.legacy.min.css
+-rw-r--r--   0        0        0   169254 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.main.min.css
+-rw-r--r--   0        0        0   174542 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.min.css
+-rw-r--r--   0        0        0    52971 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.module.min.js
+-rw-r--r--   0        0        0    69953 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.nomodule.min.js
+-rw-r--r--   0        0        0     2150 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.print.min.css
+-rw-r--r--   0        0        0      557 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/README.md
+-rw-r--r--   0        0        0   118833 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css
+-rw-r--r--   0        0        0   505020 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css
+-rw-r--r--   0        0        0   614046 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.min.css
+-rw-r--r--   0        0        0   103658 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js
+-rw-r--r--   0        0        0   264441 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js
+-rw-r--r--   0        0        0   118518 2024-04-25 13:02:07.308325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.legacy.min.css
+-rw-r--r--   0        0        0   504300 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.main.min.css
+-rw-r--r--   0        0        0   688992 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.min.css
+-rw-r--r--   0        0        0   103658 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.module.min.js
+-rw-r--r--   0        0        0   264441 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.nomodule.min.js
+-rw-r--r--   0        0        0    76110 2024-04-25 13:02:07.312325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.print.min.css
+-rw-r--r--   0        0        0     3631 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0     9190 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3448 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0     7406 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/favicon.ico
+-rw-r--r--   0        0        0     6360 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/favicon.svg
+-rw-r--r--   0        0        0      292 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/manifest.webmanifest
+-rwxr-xr-x   0        0        0    52216 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff
+-rwxr-xr-x   0        0        0    42092 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2
+-rwxr-xr-x   0        0        0    56436 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff
+-rwxr-xr-x   0        0        0    45300 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2
+-rwxr-xr-x   0        0        0    50440 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff
+-rwxr-xr-x   0        0        0    41368 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2
+-rwxr-xr-x   0        0        0    54492 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff
+-rwxr-xr-x   0        0        0    43916 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2
+-rwxr-xr-x   0        0        0    51292 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff
+-rwxr-xr-x   0        0        0    41940 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2
+-rwxr-xr-x   0        0        0    54680 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff
+-rwxr-xr-x   0        0        0    44572 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2
+-rwxr-xr-x   0        0        0    51140 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff
+-rwxr-xr-x   0        0        0    41328 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2
+-rwxr-xr-x   0        0        0    54328 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff
+-rwxr-xr-x   0        0        0    44284 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2
+-rw-r--r--   0        0        0   114508 2024-04-25 13:02:07.316325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff
+-rw-r--r--   0        0        0    80368 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2
+-rw-r--r--   0        0        0   114016 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff
+-rw-r--r--   0        0        0    79472 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2
+-rw-r--r--   0        0        0      397 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-fill.svg
+-rw-r--r--   0        0        0      789 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg
+-rw-r--r--   0        0        0      280 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-fill.svg
+-rw-r--r--   0        0        0      416 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-line.svg
+-rw-r--r--   0        0        0      232 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/bank-fill.svg
+-rw-r--r--   0        0        0      262 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/bank-line.svg
+-rw-r--r--   0        0        0      204 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/building-fill.svg
+-rw-r--r--   0        0        0      225 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/building-line.svg
+-rw-r--r--   0        0        0      316 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/community-fill.svg
+-rw-r--r--   0        0        0      388 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/community-line.svg
+-rw-r--r--   0        0        0      232 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/government-fill.svg
+-rw-r--r--   0        0        0      227 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/government-line.svg
+-rw-r--r--   0        0        0      209 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/home-4-fill.svg
+-rw-r--r--   0        0        0      239 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/home-4-line.svg
+-rw-r--r--   0        0        0      212 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/hospital-fill.svg
+-rw-r--r--   0        0        0      228 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/hospital-line.svg
+-rw-r--r--   0        0        0      224 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/hotel-fill.svg
+-rw-r--r--   0        0        0      243 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/hotel-line.svg
+-rw-r--r--   0        0        0      437 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/store-fill.svg
+-rw-r--r--   0        0        0      546 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/store-line.svg
+-rw-r--r--   0        0        0      254 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/archive-fill.svg
+-rw-r--r--   0        0        0      288 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/archive-line.svg
+-rw-r--r--   0        0        0      330 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/attachment-fill.svg
+-rw-r--r--   0        0        0      241 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/attachment-line.svg
+-rw-r--r--   0        0        0      289 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/award-fill.svg
+-rw-r--r--   0        0        0      338 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/award-line.svg
+-rw-r--r--   0        0        0      218 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/bar-chart-box-fill.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/bar-chart-box-line.svg
+-rw-r--r--   0        0        0      208 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/bookmark-fill.svg
+-rw-r--r--   0        0        0      242 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/bookmark-line.svg
+-rw-r--r--   0        0        0      253 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/briefcase-fill.svg
+-rw-r--r--   0        0        0      267 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/briefcase-line.svg
+-rw-r--r--   0        0        0      248 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/calendar-2-fill.svg
+-rw-r--r--   0        0        0      281 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/calendar-2-line.svg
+-rw-r--r--   0        0        0      218 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/calendar-event-fill.svg
+-rw-r--r--   0        0        0      251 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/calendar-event-line.svg
+-rw-r--r--   0        0        0      203 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/calendar-fill.svg
+-rw-r--r--   0        0        0      244 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/calendar-line.svg
+-rw-r--r--   0        0        0      254 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/cloud-fill.svg
+-rw-r--r--   0        0        0      356 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/cloud-line.svg
+-rw-r--r--   0        0        0      290 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/copyright-fill.svg
+-rw-r--r--   0        0        0      346 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/copyright-line.svg
+-rw-r--r--   0        0        0      341 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/customer-service-fill.svg
+-rw-r--r--   0        0        0      375 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/customer-service-line.svg
+-rw-r--r--   0        0        0      210 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/flag-fill.svg
+-rw-r--r--   0        0        0      255 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/flag-line.svg
+-rw-r--r--   0        0        0      540 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/global-fill.svg
+-rw-r--r--   0        0        0      607 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/global-line.svg
+-rw-r--r--   0        0        0      200 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/line-chart-fill.svg
+-rw-r--r--   0        0        0      218 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/line-chart-line.svg
+-rw-r--r--   0        0        0      409 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/links-fill.svg
+-rw-r--r--   0        0        0      418 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/links-line.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/mail-fill.svg
+-rw-r--r--   0        0        0      247 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/mail-line.svg
+-rw-r--r--   0        0        0      318 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/mail-open-fill.svg
+-rw-r--r--   0        0        0      359 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/mail-open-line.svg
+-rw-r--r--   0        0        0      355 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/medal-fill.svg
+-rw-r--r--   0        0        0      389 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/medal-line.svg
+-rw-r--r--   0        0        0      248 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/pie-chart-2-fill.svg
+-rw-r--r--   0        0        0      378 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/pie-chart-2-line.svg
+-rw-r--r--   0        0        0      273 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/pie-chart-box-fill.svg
+-rw-r--r--   0        0        0      289 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/pie-chart-box-line.svg
+-rw-r--r--   0        0        0      256 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/printer-fill.svg
+-rw-r--r--   0        0        0      341 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/printer-line.svg
+-rw-r--r--   0        0        0      296 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/profil-fill.svg
+-rw-r--r--   0        0        0      312 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/profil-line.svg
+-rw-r--r--   0        0        0      356 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/projector-2-fill.svg
+-rw-r--r--   0        0        0      350 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/projector-2-line.svg
+-rw-r--r--   0        0        0      248 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/send-plane-fill.svg
+-rw-r--r--   0        0        0      301 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/send-plane-line.svg
+-rw-r--r--   0        0        0      226 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/slideshow-fill.svg
+-rw-r--r--   0        0        0      241 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/slideshow-line.svg
+-rw-r--r--   0        0        0      215 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/window-fill.svg
+-rw-r--r--   0        0        0      230 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/window-line.svg
+-rw-r--r--   0        0        0      199 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-2-fill.svg
+-rw-r--r--   0        0        0      237 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-2-line.svg
+-rw-r--r--   0        0        0      236 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-3-fill.svg
+-rw-r--r--   0        0        0      360 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-3-line.svg
+-rw-r--r--   0        0        0      256 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-check-fill.svg
+-rw-r--r--   0        0        0      283 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-check-line.svg
+-rw-r--r--   0        0        0      321 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-delete-fill.svg
+-rw-r--r--   0        0        0      348 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-delete-line.svg
+-rw-r--r--   0        0        0      243 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-poll-fill.svg
+-rw-r--r--   0        0        0      214 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/chat-poll-line.svg
+-rw-r--r--   0        0        0      236 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/discuss-fill.svg
+-rw-r--r--   0        0        0      282 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/discuss-line.svg
+-rw-r--r--   0        0        0      201 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/feedback-fill.svg
+-rw-r--r--   0        0        0      229 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/feedback-line.svg
+-rw-r--r--   0        0        0      215 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/message-2-fill.svg
+-rw-r--r--   0        0        0      245 2024-04-25 13:02:07.320325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/message-2-line.svg
+-rw-r--r--   0        0        0      231 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/question-answer-fill.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/question-answer-line.svg
+-rw-r--r--   0        0        0      263 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/questionnaire-fill.svg
+-rw-r--r--   0        0        0      327 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/questionnaire-line.svg
+-rw-r--r--   0        0        0      206 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/video-chat-fill.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/communication/video-chat-line.svg
+-rw-r--r--   0        0        0      318 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/ball-pen-fill.svg
+-rw-r--r--   0        0        0      372 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/ball-pen-line.svg
+-rw-r--r--   0        0        0      252 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/brush-3-fill.svg
+-rw-r--r--   0        0        0      266 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/brush-3-line.svg
+-rw-r--r--   0        0        0      449 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/brush-fill.svg
+-rw-r--r--   0        0        0      689 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/brush-line.svg
+-rw-r--r--   0        0        0      195 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/contrast-fill.svg
+-rw-r--r--   0        0        0      230 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/contrast-line.svg
+-rw-r--r--   0        0        0      173 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/crop-fill.svg
+-rw-r--r--   0        0        0      184 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/crop-line.svg
+-rw-r--r--   0        0        0      399 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/drag-move-2-fill.svg
+-rw-r--r--   0        0        0      178 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/drag-move-2-line.svg
+-rw-r--r--   0        0        0      153 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/drop-fill.svg
+-rw-r--r--   0        0        0      190 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/drop-line.svg
+-rw-r--r--   0        0        0      275 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/edit-box-fill.svg
+-rw-r--r--   0        0        0      255 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/edit-box-line.svg
+-rw-r--r--   0        0        0      206 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/edit-fill.svg
+-rw-r--r--   0        0        0      258 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/edit-line.svg
+-rw-r--r--   0        0        0      266 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/ink-bottle-fill.svg
+-rw-r--r--   0        0        0      323 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/ink-bottle-line.svg
+-rw-r--r--   0        0        0      241 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/layout-grid-fill.svg
+-rw-r--r--   0        0        0      232 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/layout-grid-line.svg
+-rw-r--r--   0        0        0      401 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/mark-pen-fill.svg
+-rw-r--r--   0        0        0      503 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/mark-pen-line.svg
+-rw-r--r--   0        0        0      292 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/paint-brush-fill.svg
+-rw-r--r--   0        0        0      305 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/paint-brush-line.svg
+-rw-r--r--   0        0        0      339 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/paint-fill.svg
+-rw-r--r--   0        0        0      362 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/paint-line.svg
+-rw-r--r--   0        0        0      437 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/palette-fill.svg
+-rw-r--r--   0        0        0      584 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/palette-line.svg
+-rw-r--r--   0        0        0      386 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pantone-fill.svg
+-rw-r--r--   0        0        0      505 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pantone-line.svg
+-rw-r--r--   0        0        0      389 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pen-nib-fill.svg
+-rw-r--r--   0        0        0      510 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pen-nib-line.svg
+-rw-r--r--   0        0        0      254 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pencil-fill.svg
+-rw-r--r--   0        0        0      310 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pencil-line.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pencil-ruler-fill.svg
+-rw-r--r--   0        0        0      255 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/pencil-ruler-line.svg
+-rw-r--r--   0        0        0      302 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/sip-fill.svg
+-rw-r--r--   0        0        0      352 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/sip-line.svg
+-rw-r--r--   0        0        0      221 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/table-fill.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/table-line.svg
+-rw-r--r--   0        0        0      500 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/bug-fill.svg
+-rw-r--r--   0        0        0      632 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/bug-line.svg
+-rw-r--r--   0        0        0      360 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/code-box-fill.svg
+-rw-r--r--   0        0        0      374 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/code-box-line.svg
+-rw-r--r--   0        0        0      281 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/code-s-slash-line.svg
+-rw-r--r--   0        0        0      197 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/cursor-fill.svg
+-rw-r--r--   0        0        0      283 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/cursor-line.svg
+-rw-r--r--   0        0        0      307 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-branch-fill.svg
+-rw-r--r--   0        0        0      425 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-branch-line.svg
+-rw-r--r--   0        0        0      187 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-commit-fill.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-commit-line.svg
+-rw-r--r--   0        0        0      330 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-merge-fill.svg
+-rw-r--r--   0        0        0      455 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-merge-line.svg
+-rw-r--r--   0        0        0      233 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-pull-request-fill.svg
+-rw-r--r--   0        0        0      356 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-pull-request-line.svg
+-rw-r--r--   0        0        0      294 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-repository-commits-fill.svg
+-rw-r--r--   0        0        0      320 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-repository-commits-line.svg
+-rw-r--r--   0        0        0      285 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-repository-fill.svg
+-rw-r--r--   0        0        0      328 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-repository-line.svg
+-rw-r--r--   0        0        0      288 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-repository-private-fill.svg
+-rw-r--r--   0        0        0      304 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/git-repository-private-line.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/terminal-box-fill.svg
+-rw-r--r--   0        0        0      287 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/terminal-box-line.svg
+-rw-r--r--   0        0        0      186 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/terminal-line.svg
+-rw-r--r--   0        0        0      230 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/terminal-window-fill.svg
+-rw-r--r--   0        0        0      245 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/terminal-window-line.svg
+-rw-r--r--   0        0        0      343 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/bluetooth-fill.svg
+-rw-r--r--   0        0        0      343 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/bluetooth-line.svg
+-rw-r--r--   0        0        0      256 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/computer-fill.svg
+-rw-r--r--   0        0        0      275 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/computer-line.svg
+-rw-r--r--   0        0        0      514 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg
+-rw-r--r--   0        0        0      552 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg
+-rw-r--r--   0        0        0      266 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/database-fill.svg
+-rw-r--r--   0        0        0      296 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/database-line.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/device-fill.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/device-line.svg
+-rw-r--r--   0        0        0      206 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/hard-drive-2-fill.svg
+-rw-r--r--   0        0        0      222 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/hard-drive-2-line.svg
+-rw-r--r--   0        0        0      290 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/mac-fill.svg
+-rw-r--r--   0        0        0      288 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/mac-line.svg
+-rw-r--r--   0        0        0      485 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/phone-fill.svg
+-rw-r--r--   0        0        0      719 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/phone-line.svg
+-rw-r--r--   0        0        0      272 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/qr-code-fill.svg
+-rw-r--r--   0        0        0      315 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/qr-code-line.svg
+-rw-r--r--   0        0        0      229 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/rss-fill.svg
+-rw-r--r--   0        0        0      230 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/rss-line.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/save-3-fill.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/save-3-line.svg
+-rw-r--r--   0        0        0      195 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/save-fill.svg
+-rw-r--r--   0        0        0      219 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/save-line.svg
+-rw-r--r--   0        0        0      219 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/server-fill.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/server-line.svg
+-rw-r--r--   0        0        0      208 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/smartphone-fill.svg
+-rw-r--r--   0        0        0      224 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/smartphone-line.svg
+-rw-r--r--   0        0        0      208 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/tablet-fill.svg
+-rw-r--r--   0        0        0      224 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/tablet-line.svg
+-rw-r--r--   0        0        0      285 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/tv-fill.svg
+-rw-r--r--   0        0        0      304 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/tv-line.svg
+-rw-r--r--   0        0        0      618 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg
+-rw-r--r--   0        0        0      630 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/wifi-line.svg
+-rw-r--r--   0        0        0      233 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/article-fill.svg
+-rw-r--r--   0        0        0      249 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/article-line.svg
+-rw-r--r--   0        0        0      181 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/book-2-fill.svg
+-rw-r--r--   0        0        0      227 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/book-2-line.svg
+-rw-r--r--   0        0        0      226 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/booklet-fill.svg
+-rw-r--r--   0        0        0      242 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/booklet-line.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/clipboard-fill.svg
+-rw-r--r--   0        0        0      274 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/clipboard-line.svg
+-rw-r--r--   0        0        0      317 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/draft-fill.svg
+-rw-r--r--   0        0        0      303 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/draft-line.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-add-fill.svg
+-rw-r--r--   0        0        0      251 2024-04-25 13:02:07.324325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-add-line.svg
+-rw-r--r--   0        0        0      227 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-download-fill.svg
+-rw-r--r--   0        0        0      245 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-download-line.svg
+-rw-r--r--   0        0        0      230 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-fill.svg
+-rw-r--r--   0        0        0      225 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-line.svg
+-rw-r--r--   0        0        0      255 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-pdf-fill.svg
+-rw-r--r--   0        0        0      273 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-pdf-line.svg
+-rw-r--r--   0        0        0      281 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-text-fill.svg
+-rw-r--r--   0        0        0      272 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/file-text-line.svg
+-rw-r--r--   0        0        0      198 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/folder-2-fill.svg
+-rw-r--r--   0        0        0      234 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/folder-2-line.svg
+-rw-r--r--   0        0        0      262 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/newspaper-fill.svg
+-rw-r--r--   0        0        0      290 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/newspaper-line.svg
+-rw-r--r--   0        0        0      292 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/survey-fill.svg
+-rw-r--r--   0        0        0      317 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/survey-line.svg
+-rw-r--r--   0        0        0      217 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/todo-fill.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/document/todo-line.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/code-view.svg
+-rw-r--r--   0        0        0      250 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/font-size.svg
+-rw-r--r--   0        0        0      314 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/fr--bold.svg
+-rw-r--r--   0        0        0      160 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/fr--highlight.svg
+-rw-r--r--   0        0        0      278 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/fr--quote-fill.svg
+-rw-r--r--   0        0        0      344 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/fr--quote-line.svg
+-rw-r--r--   0        0        0      223 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-1.svg
+-rw-r--r--   0        0        0      387 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-2.svg
+-rw-r--r--   0        0        0      542 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-3.svg
+-rw-r--r--   0        0        0      268 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-4.svg
+-rw-r--r--   0        0        0      393 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-5.svg
+-rw-r--r--   0        0        0      538 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-6.svg
+-rw-r--r--   0        0        0      298 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/hashtag.svg
+-rw-r--r--   0        0        0      158 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/italic.svg
+-rw-r--r--   0        0        0      468 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/link-unlink.svg
+-rw-r--r--   0        0        0      408 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/link.svg
+-rw-r--r--   0        0        0      246 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/list-ordered.svg
+-rw-r--r--   0        0        0      275 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/list-unordered.svg
+-rw-r--r--   0        0        0      341 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/question-mark.svg
+-rw-r--r--   0        0        0      147 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/separator.svg
+-rw-r--r--   0        0        0      151 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/space.svg
+-rw-r--r--   0        0        0      317 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/subscript.svg
+-rw-r--r--   0        0        0      315 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/superscript.svg
+-rw-r--r--   0        0        0      263 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/table-2.svg
+-rw-r--r--   0        0        0      505 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/translate-2.svg
+-rw-r--r--   0        0        0      206 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/bank-card-fill.svg
+-rw-r--r--   0        0        0      220 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/bank-card-line.svg
+-rw-r--r--   0        0        0      277 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/coin-fill.svg
+-rw-r--r--   0        0        0      393 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/gift-fill.svg
+-rw-r--r--   0        0        0      406 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/gift-line.svg
+-rw-r--r--   0        0        0      366 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/money-euro-box-fill.svg
+-rw-r--r--   0        0        0      344 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/money-euro-box-line.svg
+-rw-r--r--   0        0        0      365 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-fill.svg
+-rw-r--r--   0        0        0      362 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-line.svg
+-rw-r--r--   0        0        0      397 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/secure-payment-fill.svg
+-rw-r--r--   0        0        0      427 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/secure-payment-line.svg
+-rw-r--r--   0        0        0      348 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/shopping-bag-fill.svg
+-rw-r--r--   0        0        0      282 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/shopping-bag-line.svg
+-rw-r--r--   0        0        0      311 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-fill.svg
+-rw-r--r--   0        0        0      343 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-line.svg
+-rw-r--r--   0        0        0      200 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/trophy-fill.svg
+-rw-r--r--   0        0        0      222 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/finance/trophy-line.svg
+-rw-r--r--   0        0        0      289 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/capsule-fill.svg
+-rw-r--r--   0        0        0      379 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/capsule-line.svg
+-rw-r--r--   0        0        0      336 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/dislike-fill.svg
+-rw-r--r--   0        0        0      543 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/dislike-line.svg
+-rw-r--r--   0        0        0      243 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/dossier-fill.svg
+-rw-r--r--   0        0        0      265 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/dossier-line.svg
+-rw-r--r--   0        0        0      269 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/first-aid-kit-fill.svg
+-rw-r--r--   0        0        0      283 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/first-aid-kit-line.svg
+-rw-r--r--   0        0        0      317 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-fill.svg
+-rw-r--r--   0        0        0      359 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-line.svg
+-rw-r--r--   0        0        0      258 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/health-book-fill.svg
+-rw-r--r--   0        0        0      273 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/health-book-line.svg
+-rw-r--r--   0        0        0      209 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/heart-fill.svg
+-rw-r--r--   0        0        0      365 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/heart-line.svg
+-rw-r--r--   0        0        0      331 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/heart-pulse-fill.svg
+-rw-r--r--   0        0        0      661 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg
+-rw-r--r--   0        0        0      476 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/lungs-fill.svg
+-rw-r--r--   0        0        0      909 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/lungs-line.svg
+-rw-r--r--   0        0        0      241 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/medicine-bottle-fill.svg
+-rw-r--r--   0        0        0      293 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/medicine-bottle-line.svg
+-rw-r--r--   0        0        0      395 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/mental-health-fill.svg
+-rw-r--r--   0        0        0      503 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/mental-health-line.svg
+-rw-r--r--   0        0        0      519 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg
+-rw-r--r--   0        0        0      618 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/microscope-line.svg
+-rw-r--r--   0        0        0      370 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/psychotherapy-fill.svg
+-rw-r--r--   0        0        0      504 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/psychotherapy-line.svg
+-rw-r--r--   0        0        0      181 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/pulse-line.svg
+-rw-r--r--   0        0        0      311 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/stethoscope-fill.svg
+-rw-r--r--   0        0        0      346 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/stethoscope-line.svg
+-rw-r--r--   0        0        0      446 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/surgical-mask-fill.svg
+-rw-r--r--   0        0        0      567 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg
+-rw-r--r--   0        0        0      466 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/syringe-fill.svg
+-rw-r--r--   0        0        0      486 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/syringe-line.svg
+-rw-r--r--   0        0        0      237 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/test-tube-fill.svg
+-rw-r--r--   0        0        0      264 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/test-tube-line.svg
+-rw-r--r--   0        0        0      484 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/thermometer-fill.svg
+-rw-r--r--   0        0        0      576 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg
+-rw-r--r--   0        0        0     1055 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/virus-fill.svg
+-rw-r--r--   0        0        0     1112 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/virus-line.svg
+-rw-r--r--   0        0        0      552 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg
+-rw-r--r--   0        0        0      594 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg
+-rw-r--r--   0        0        0      591 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg
+-rw-r--r--   0        0        0      411 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/edge-line.svg
+-rw-r--r--   0        0        0      368 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/facebook-circle-fill.svg
+-rw-r--r--   0        0        0      458 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/facebook-circle-line.svg
+-rw-r--r--   0        0        0      708 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg
+-rw-r--r--   0        0        0     1003 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg
+-rw-r--r--   0        0        0      685 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg
+-rw-r--r--   0        0        0      806 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg
+-rw-r--r--   0        0        0      561 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg
+-rw-r--r--   0        0        0      428 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-line.svg
+-rw-r--r--   0        0        0      790 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/github-fill.svg
+-rw-r--r--   0        0        0     1485 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/github-line.svg
+-rw-r--r--   0        0        0      530 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/google-fill.svg
+-rw-r--r--   0        0        0      371 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/google-line.svg
+-rw-r--r--   0        0        0      965 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg
+-rw-r--r--   0        0        0      796 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/ie-line.svg
+-rw-r--r--   0        0        0      917 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg
+-rw-r--r--   0        0        0     2014 2024-04-25 13:02:07.328325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg
+-rw-r--r--   0        0        0      552 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg
+-rw-r--r--   0        0        0      366 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/linkedin-box-line.svg
+-rw-r--r--   0        0        0      948 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg
+-rw-r--r--   0        0        0     1259 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg
+-rw-r--r--   0        0        0      202 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/npmjs-fill.svg
+-rw-r--r--   0        0        0      220 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/npmjs-line.svg
+-rw-r--r--   0        0        0      331 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/remixicon-fill.svg
+-rw-r--r--   0        0        0      391 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/remixicon-line.svg
+-rw-r--r--   0        0        0      972 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg
+-rw-r--r--   0        0        0      574 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/safari-line.svg
+-rw-r--r--   0        0        0     1133 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg
+-rw-r--r--   0        0        0      514 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/slack-line.svg
+-rw-r--r--   0        0        0     1494 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg
+-rw-r--r--   0        0        0     1848 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg
+-rw-r--r--   0        0        0      398 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/telegram-fill.svg
+-rw-r--r--   0        0        0      440 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/telegram-line.svg
+-rw-r--r--   0        0        0     1726 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/threads-fill.svg
+-rw-r--r--   0        0        0     1630 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/threads-line.svg
+-rw-r--r--   0        0        0      332 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitch-fill.svg
+-rw-r--r--   0        0        0      241 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitch-line.svg
+-rw-r--r--   0        0        0      586 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg
+-rw-r--r--   0        0        0      690 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg
+-rw-r--r--   0        0        0      324 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitter-x-fill.svg
+-rw-r--r--   0        0        0      254 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitter-x-line.svg
+-rw-r--r--   0        0        0      726 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg
+-rw-r--r--   0        0        0     1001 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg
+-rw-r--r--   0        0        0      178 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/vuejs-fill.svg
+-rw-r--r--   0        0        0      198 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/vuejs-line.svg
+-rw-r--r--   0        0        0      418 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/youtube-fill.svg
+-rw-r--r--   0        0        0      899 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg
+-rw-r--r--   0        0        0      385 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/anchor-fill.svg
+-rw-r--r--   0        0        0      350 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/anchor-line.svg
+-rw-r--r--   0        0        0      359 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/bike-fill.svg
+-rw-r--r--   0        0        0      359 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/bike-line.svg
+-rw-r--r--   0        0        0      284 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/bus-fill.svg
+-rw-r--r--   0        0        0      299 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/bus-line.svg
+-rw-r--r--   0        0        0      372 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/car-fill.svg
+-rw-r--r--   0        0        0      387 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/car-line.svg
+-rw-r--r--   0        0        0      317 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/caravan-fill.svg
+-rw-r--r--   0        0        0      383 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/caravan-line.svg
+-rw-r--r--   0        0        0      253 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/charging-pile-2-fill.svg
+-rw-r--r--   0        0        0      265 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/charging-pile-2-line.svg
+-rw-r--r--   0        0        0      246 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/compass-3-fill.svg
+-rw-r--r--   0        0        0      281 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/compass-3-line.svg
+-rw-r--r--   0        0        0      222 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/cup-fill.svg
+-rw-r--r--   0        0        0      264 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/cup-line.svg
+-rw-r--r--   0        0        0      945 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/earth-fill.svg
+-rw-r--r--   0        0        0      905 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/earth-line.svg
+-rw-r--r--   0        0        0     2305 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/france-fill.svg
+-rw-r--r--   0        0        0     4459 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/france-line.svg
+-rw-r--r--   0        0        0      303 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/gas-station-fill.svg
+-rw-r--r--   0        0        0      318 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/gas-station-line.svg
+-rw-r--r--   0        0        0      179 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/goblet-fill.svg
+-rw-r--r--   0        0        0      208 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/goblet-line.svg
+-rw-r--r--   0        0        0      214 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/map-pin-2-fill.svg
+-rw-r--r--   0        0        0      280 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/map-pin-2-line.svg
+-rw-r--r--   0        0        0      277 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/map-pin-user-fill.svg
+-rw-r--r--   0        0        0      363 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/map-pin-user-line.svg
+-rw-r--r--   0        0        0      378 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/motorbike-fill.svg
+-rw-r--r--   0        0        0      447 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/motorbike-line.svg
+-rw-r--r--   0        0        0      256 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/passport-fill.svg
+-rw-r--r--   0        0        0      272 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/passport-line.svg
+-rw-r--r--   0        0        0      221 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/restaurant-fill.svg
+-rw-r--r--   0        0        0      257 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/restaurant-line.svg
+-rw-r--r--   0        0        0      381 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/road-map-fill.svg
+-rw-r--r--   0        0        0      405 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/road-map-line.svg
+-rw-r--r--   0        0        0      278 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/sailboat-fill.svg
+-rw-r--r--   0        0        0      333 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/sailboat-line.svg
+-rw-r--r--   0        0        0      580 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg
+-rw-r--r--   0        0        0      562 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg
+-rw-r--r--   0        0        0      351 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/signal-tower-fill.svg
+-rw-r--r--   0        0        0      348 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/signal-tower-line.svg
+-rw-r--r--   0        0        0      271 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/suitcase-2-fill.svg
+-rw-r--r--   0        0        0      286 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/suitcase-2-line.svg
+-rw-r--r--   0        0        0      374 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/taxi-fill.svg
+-rw-r--r--   0        0        0      386 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/taxi-line.svg
+-rw-r--r--   0        0        0      251 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/train-fill.svg
+-rw-r--r--   0        0        0      293 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/train-line.svg
+-rw-r--r--   0        0        0      160 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/align-left.svg
+-rw-r--r--   0        0        0      253 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/camera-fill.svg
+-rw-r--r--   0        0        0      311 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/camera-line.svg
+-rw-r--r--   0        0        0      294 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/clapperboard-fill.svg
+-rw-r--r--   0        0        0      312 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/clapperboard-line.svg
+-rw-r--r--   0        0        0      334 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/equalizer-fill.svg
+-rw-r--r--   0        0        0      505 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/equalizer-line.svg
+-rw-r--r--   0        0        0      340 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/film-fill.svg
+-rw-r--r--   0        0        0      355 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/film-line.svg
+-rw-r--r--   0        0        0      184 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/fullscreen-line.svg
+-rw-r--r--   0        0        0      388 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/gallery-fill.svg
+-rw-r--r--   0        0        0      466 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/gallery-line.svg
+-rw-r--r--   0        0        0      261 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/headphone-fill.svg
+-rw-r--r--   0        0        0      300 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/headphone-line.svg
+-rw-r--r--   0        0        0      394 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/image-add-fill.svg
+-rw-r--r--   0        0        0      316 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/image-add-line.svg
+-rw-r--r--   0        0        0      398 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/image-edit-fill.svg
+-rw-r--r--   0        0        0      415 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/image-edit-line.svg
+-rw-r--r--   0        0        0      307 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/image-fill.svg
+-rw-r--r--   0        0        0      334 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/image-line.svg
+-rw-r--r--   0        0        0      394 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/live-fill.svg
+-rw-r--r--   0        0        0      408 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/live-line.svg
+-rw-r--r--   0        0        0      269 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/mic-fill.svg
+-rw-r--r--   0        0        0      320 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/mic-line.svg
+-rw-r--r--   0        0        0      158 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/music-2-fill.svg
+-rw-r--r--   0        0        0      226 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/music-2-line.svg
+-rw-r--r--   0        0        0      154 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/notification-3-fill.svg
+-rw-r--r--   0        0        0      208 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/notification-3-line.svg
+-rw-r--r--   0        0        0      201 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/pause-circle-fill.svg
+-rw-r--r--   0        0        0      236 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/pause-circle-line.svg
+-rw-r--r--   0        0        0      281 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/play-circle-fill.svg
+-rw-r--r--   0        0        0      313 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/play-circle-line.svg
+-rw-r--r--   0        0        0      186 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/stop-circle-fill.svg
+-rw-r--r--   0        0        0      221 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/stop-circle-line.svg
+-rw-r--r--   0        0        0      403 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-down-fill.svg
+-rw-r--r--   0        0        0      489 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-down-line.svg
+-rw-r--r--   0        0        0      407 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-mute-fill.svg
+-rw-r--r--   0        0        0      490 2024-04-25 13:02:07.332325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-mute-line.svg
+-rw-r--r--   0        0        0      551 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg
+-rw-r--r--   0        0        0      630 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg
+-rw-r--r--   0        0        0      334 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/leaf-fill.svg
+-rw-r--r--   0        0        0      467 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/leaf-line.svg
+-rw-r--r--   0        0        0      253 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/lightbulb-fill.svg
+-rw-r--r--   0        0        0      406 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/lightbulb-line.svg
+-rw-r--r--   0        0        0      277 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/plant-fill.svg
+-rw-r--r--   0        0        0      362 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/plant-line.svg
+-rw-r--r--   0        0        0      573 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg
+-rw-r--r--   0        0        0      558 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/recycle-line.svg
+-rw-r--r--   0        0        0      454 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/scales-3-fill.svg
+-rw-r--r--   0        0        0      552 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg
+-rw-r--r--   0        0        0      258 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/seedling-fill.svg
+-rw-r--r--   0        0        0      326 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/seedling-line.svg
+-rw-r--r--   0        0        0      232 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/umbrella-fill.svg
+-rw-r--r--   0        0        0      315 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/umbrella-line.svg
+-rw-r--r--   0        0        0      209 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/add-circle-fill.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/add-circle-line.svg
+-rw-r--r--   0        0        0      136 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/add-line.svg
+-rw-r--r--   0        0        0      319 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/alarm-warning-fill.svg
+-rw-r--r--   0        0        0      360 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/alarm-warning-line.svg
+-rw-r--r--   0        0        0      224 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/alert-fill.svg
+-rw-r--r--   0        0        0      257 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/alert-line.svg
+-rw-r--r--   0        0        0      127 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-down-fill.svg
+-rw-r--r--   0        0        0      188 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-down-line.svg
+-rw-r--r--   0        0        0      120 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-down-s-fill.svg
+-rw-r--r--   0        0        0      173 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-down-s-line.svg
+-rw-r--r--   0        0        0      159 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-go-back-fill.svg
+-rw-r--r--   0        0        0      213 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-go-back-line.svg
+-rw-r--r--   0        0        0      161 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-fill.svg
+-rw-r--r--   0        0        0      218 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-line.svg
+-rw-r--r--   0        0        0      128 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-left-fill.svg
+-rw-r--r--   0        0        0      184 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-left-line.svg
+-rw-r--r--   0        0        0      119 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-left-s-fill.svg
+-rw-r--r--   0        0        0      173 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-left-s-line.svg
+-rw-r--r--   0        0        0      128 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-right-fill.svg
+-rw-r--r--   0        0        0      189 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-right-line.svg
+-rw-r--r--   0        0        0      118 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-right-s-fill.svg
+-rw-r--r--   0        0        0      175 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-right-s-line.svg
+-rw-r--r--   0        0        0      197 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-right-up-line.svg
+-rw-r--r--   0        0        0      129 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-up-fill.svg
+-rw-r--r--   0        0        0      186 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-up-line.svg
+-rw-r--r--   0        0        0      117 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-up-s-fill.svg
+-rw-r--r--   0        0        0      173 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/arrow-up-s-line.svg
+-rw-r--r--   0        0        0      177 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/check-line.svg
+-rw-r--r--   0        0        0      252 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/checkbox-circle-fill.svg
+-rw-r--r--   0        0        0      288 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/checkbox-circle-line.svg
+-rw-r--r--   0        0        0      252 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/checkbox-fill.svg
+-rw-r--r--   0        0        0      288 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/checkbox-line.svg
+-rw-r--r--   0        0        0      321 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/close-circle-fill.svg
+-rw-r--r--   0        0        0      342 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/close-circle-line.svg
+-rw-r--r--   0        0        0      210 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/close-line.svg
+-rw-r--r--   0        0        0      189 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/delete-bin-fill.svg
+-rw-r--r--   0        0        0      203 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/delete-bin-line.svg
+-rw-r--r--   0        0        0      142 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/download-fill.svg
+-rw-r--r--   0        0        0      198 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/download-line.svg
+-rw-r--r--   0        0        0      203 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/error-warning-fill.svg
+-rw-r--r--   0        0        0      238 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/error-warning-line.svg
+-rw-r--r--   0        0        0      228 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/external-link-fill.svg
+-rw-r--r--   0        0        0      230 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/external-link-line.svg
+-rw-r--r--   0        0        0      281 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/eye-fill.svg
+-rw-r--r--   0        0        0      380 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/eye-line.svg
+-rw-r--r--   0        0        0      481 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/eye-off-fill.svg
+-rw-r--r--   0        0        0      678 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg
+-rw-r--r--   0        0        0      136 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/filter-fill.svg
+-rw-r--r--   0        0        0      187 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/filter-line.svg
+-rw-r--r--   0        0        0      196 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-first-line.svg
+-rw-r--r--   0        0        0      197 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-line-double.svg
+-rw-r--r--   0        0        0      377 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-down-circle-fill.svg
+-rw-r--r--   0        0        0      201 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-last-line.svg
+-rw-r--r--   0        0        0      201 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-line-double.svg
+-rw-r--r--   0        0        0      377 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-up-circle-fill.svg
+-rw-r--r--   0        0        0      327 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--capslock-line.svg
+-rw-r--r--   0        0        0      329 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--equal-circle-fill.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--error-fill.svg
+-rw-r--r--   0        0        0      309 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--error-line.svg
+-rw-r--r--   0        0        0      237 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--info-fill.svg
+-rw-r--r--   0        0        0      328 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--info-line.svg
+-rw-r--r--   0        0        0      253 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--success-fill.svg
+-rw-r--r--   0        0        0      289 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--success-line.svg
+-rw-r--r--   0        0        0      482 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--theme-fill.svg
+-rw-r--r--   0        0        0      225 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--warning-fill.svg
+-rw-r--r--   0        0        0      258 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/fr--warning-line.svg
+-rw-r--r--   0        0        0      205 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/information-fill.svg
+-rw-r--r--   0        0        0      239 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/information-line.svg
+-rw-r--r--   0        0        0      238 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/lock-fill.svg
+-rw-r--r--   0        0        0      252 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/lock-line.svg
+-rw-r--r--   0        0        0      252 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/lock-unlock-fill.svg
+-rw-r--r--   0        0        0      268 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/lock-unlock-line.svg
+-rw-r--r--   0        0        0      197 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/logout-box-r-fill.svg
+-rw-r--r--   0        0        0      219 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/logout-box-r-line.svg
+-rw-r--r--   0        0        0      145 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/menu-2-fill.svg
+-rw-r--r--   0        0        0      145 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/menu-fill.svg
+-rw-r--r--   0        0        0      248 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/more-fill.svg
+-rw-r--r--   0        0        0      348 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/more-line.svg
+-rw-r--r--   0        0        0      220 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/notification-badge-fill.svg
+-rw-r--r--   0        0        0      288 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/notification-badge-line.svg
+-rw-r--r--   0        0        0      311 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/question-fill.svg
+-rw-r--r--   0        0        0      325 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/question-line.svg
+-rw-r--r--   0        0        0      280 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/refresh-fill.svg
+-rw-r--r--   0        0        0      244 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/refresh-line.svg
+-rw-r--r--   0        0        0      247 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/search-fill.svg
+-rw-r--r--   0        0        0      382 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/search-line.svg
+-rw-r--r--   0        0        0      864 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg
+-rw-r--r--   0        0        0     1599 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg
+-rw-r--r--   0        0        0      241 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/shield-fill.svg
+-rw-r--r--   0        0        0      332 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/shield-line.svg
+-rw-r--r--   0        0        0      217 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/star-fill.svg
+-rw-r--r--   0        0        0      333 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/star-line.svg
+-rw-r--r--   0        0        0      203 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/star-s-fill.svg
+-rw-r--r--   0        0        0      325 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/star-s-line.svg
+-rw-r--r--   0        0        0      117 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/subtract-line.svg
+-rw-r--r--   0        0        0      341 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/thumb-down-fill.svg
+-rw-r--r--   0        0        0      442 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/thumb-down-line.svg
+-rw-r--r--   0        0        0      340 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/thumb-up-fill.svg
+-rw-r--r--   0        0        0      459 2024-04-25 13:02:07.336325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/thumb-up-line.svg
+-rw-r--r--   0        0        0      193 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/time-fill.svg
+-rw-r--r--   0        0        0      226 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/time-line.svg
+-rw-r--r--   0        0        0      201 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/timer-fill.svg
+-rw-r--r--   0        0        0      236 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/timer-line.svg
+-rw-r--r--   0        0        0      180 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/upload-2-fill.svg
+-rw-r--r--   0        0        0      180 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/upload-2-line.svg
+-rw-r--r--   0        0        0      144 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/upload-fill.svg
+-rw-r--r--   0        0        0      206 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/upload-line.svg
+-rw-r--r--   0        0        0      279 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/zoom-in-fill.svg
+-rw-r--r--   0        0        0      407 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/zoom-in-line.svg
+-rw-r--r--   0        0        0      260 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/zoom-out-fill.svg
+-rw-r--r--   0        0        0      388 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/zoom-out-line.svg
+-rw-r--r--   0        0        0      337 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/account-circle-fill.svg
+-rw-r--r--   0        0        0      462 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/account-circle-line.svg
+-rw-r--r--   0        0        0      383 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/account-pin-circle-fill.svg
+-rw-r--r--   0        0        0      575 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg
+-rw-r--r--   0        0        0      279 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/admin-fill.svg
+-rw-r--r--   0        0        0      349 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/admin-line.svg
+-rw-r--r--   0        0        0      357 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/group-fill.svg
+-rw-r--r--   0        0        0      462 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/group-line.svg
+-rw-r--r--   0        0        0      279 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/parent-fill.svg
+-rw-r--r--   0        0        0      413 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/parent-line.svg
+-rw-r--r--   0        0        0      424 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/team-fill.svg
+-rw-r--r--   0        0        0      750 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/team-line.svg
+-rw-r--r--   0        0        0      235 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-add-fill.svg
+-rw-r--r--   0        0        0      316 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-add-line.svg
+-rw-r--r--   0        0        0      186 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-fill.svg
+-rw-r--r--   0        0        0      314 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-heart-fill.svg
+-rw-r--r--   0        0        0      439 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-heart-line.svg
+-rw-r--r--   0        0        0      275 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-line.svg
+-rw-r--r--   0        0        0      314 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-search-fill.svg
+-rw-r--r--   0        0        0      384 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-search-line.svg
+-rw-r--r--   0        0        0      529 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg
+-rw-r--r--   0        0        0      625 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-setting-line.svg
+-rw-r--r--   0        0        0      298 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-star-fill.svg
+-rw-r--r--   0        0        0      367 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-star-line.svg
+-rw-r--r--   0        0        0      167 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/cloudy-2-fill.svg
+-rw-r--r--   0        0        0      291 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/cloudy-2-line.svg
+-rw-r--r--   0        0        0      128 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/flashlight-fill.svg
+-rw-r--r--   0        0        0      172 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/flashlight-line.svg
+-rw-r--r--   0        0        0      226 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/moon-fill.svg
+-rw-r--r--   0        0        0      286 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/moon-line.svg
+-rw-r--r--   0        0        0      449 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/sun-fill.svg
+-rw-r--r--   0        0        0      482 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/weather/sun-line.svg
+-rw-r--r--   0        0        0      466 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/legacy/README.md
+-rw-r--r--   0        0        0   127166 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js
+-rw-r--r--   0        0        0     1524 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/README.md
+-rw-r--r--   0        0        0     1588 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/account/README.md
+-rw-r--r--   0        0        0     1576 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/account/login/README.md
+-rw-r--r--   0        0        0     1764 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/account/register/README.md
+-rw-r--r--   0        0        0      926 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/README.md
+-rw-r--r--   0        0        0      701 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/not-found/README.md
+-rw-r--r--   0        0        0       13 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/unavailable/README.md
+-rw-r--r--   0        0        0      704 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/unexpected/README.md
+-rw-r--r--   0        0        0      418 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/patch/README.md
+-rw-r--r--   0        0        0      425 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/patch/patch.module.min.js
+-rw-r--r--   0        0        0      459 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/patch/patch.nomodule.min.js
+-rw-r--r--   0        0        0      363 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/README.md
+-rw-r--r--   0        0        0      450 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/address/README.md
+-rw-r--r--   0        0        0      666 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/civility/README.md
+-rw-r--r--   0        0        0      674 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/company/README.md
+-rw-r--r--   0        0        0      613 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/date/README.md
+-rw-r--r--   0        0        0      640 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/name/README.md
+-rw-r--r--   0        0        0      462 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/nationality/README.md
+-rw-r--r--   0        0        0      855 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/scheme/README.md
+-rw-r--r--   0        0        0    12280 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/scheme/scheme.min.css
+-rw-r--r--   0        0        0     3274 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/scheme/scheme.module.min.js
+-rw-r--r--   0        0        0     1003 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/README.md
+-rw-r--r--   0        0        0      421 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/README.md
+-rw-r--r--   0        0        0    32005 2024-04-25 13:02:07.340325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css
+-rw-r--r--   0        0        0    39455 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css
+-rw-r--r--   0        0        0   103161 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.min.css
+-rw-r--r--   0        0        0    31959 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.print.min.css
+-rw-r--r--   0        0        0      748 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/README.md
+-rw-r--r--   0        0        0      794 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md
+-rw-r--r--   0        0        0     3037 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css
+-rw-r--r--   0        0        0     4371 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css
+-rw-r--r--   0        0        0     7179 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css
+-rw-r--r--   0        0        0      788 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md
+-rw-r--r--   0        0        0     8089 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css
+-rw-r--r--   0        0        0    12244 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css
+-rw-r--r--   0        0        0    20104 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css
+-rw-r--r--   0        0        0      818 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md
+-rw-r--r--   0        0        0     3273 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css
+-rw-r--r--   0        0        0     4675 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css
+-rw-r--r--   0        0        0     7719 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css
+-rw-r--r--   0        0        0      776 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md
+-rw-r--r--   0        0        0     5505 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css
+-rw-r--r--   0        0        0     8001 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css
+-rw-r--r--   0        0        0    13277 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css
+-rw-r--r--   0        0        0      806 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md
+-rw-r--r--   0        0        0     3955 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css
+-rw-r--r--   0        0        0     5639 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css
+-rw-r--r--   0        0        0     9365 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css
+-rw-r--r--   0        0        0      776 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md
+-rw-r--r--   0        0        0     4811 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css
+-rw-r--r--   0        0        0     7133 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css
+-rw-r--r--   0        0        0    11715 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css
+-rw-r--r--   0        0        0      788 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md
+-rw-r--r--   0        0        0     4307 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css
+-rw-r--r--   0        0        0     6435 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css
+-rw-r--r--   0        0        0    10513 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css
+-rw-r--r--   0        0        0      776 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md
+-rw-r--r--   0        0        0     3577 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css
+-rw-r--r--   0        0        0     5397 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css
+-rw-r--r--   0        0        0     8745 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css
+-rw-r--r--   0        0        0      782 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md
+-rw-r--r--   0        0        0     2585 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css
+-rw-r--r--   0        0        0     3578 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css
+-rw-r--r--   0        0        0     5934 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css
+-rw-r--r--   0        0        0      776 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md
+-rw-r--r--   0        0        0     5281 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css
+-rw-r--r--   0        0        0     7550 2024-04-25 13:02:07.344325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css
+-rw-r--r--   0        0        0    12602 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css
+-rw-r--r--   0        0        0      764 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md
+-rw-r--r--   0        0        0     8677 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css
+-rw-r--r--   0        0        0    13727 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css
+-rw-r--r--   0        0        0    22175 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css
+-rw-r--r--   0        0        0      758 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md
+-rw-r--r--   0        0        0     6299 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css
+-rw-r--r--   0        0        0     9185 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css
+-rw-r--r--   0        0        0    15255 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css
+-rw-r--r--   0        0        0      770 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md
+-rw-r--r--   0        0        0     6786 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css
+-rw-r--r--   0        0        0    10313 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css
+-rw-r--r--   0        0        0    16870 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css
+-rw-r--r--   0        0        0      776 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md
+-rw-r--r--   0        0        0     2013 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css
+-rw-r--r--   0        0        0     2751 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css
+-rw-r--r--   0        0        0     4535 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css
+-rw-r--r--   0        0        0      776 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md
+-rw-r--r--   0        0        0    20774 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css
+-rw-r--r--   0        0        0    33241 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css
+-rw-r--r--   0        0        0    53786 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css
+-rw-r--r--   0        0        0      764 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md
+-rw-r--r--   0        0        0     3921 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css
+-rw-r--r--   0        0        0     5623 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css
+-rw-r--r--   0        0        0     9315 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css
+-rw-r--r--   0        0        0      782 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md
+-rw-r--r--   0        0        0     1485 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css
+-rw-r--r--   0        0        0     2063 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css
+-rw-r--r--   0        0        0     3319 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css
+-rw-r--r--   0        0        0    87540 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css
+-rw-r--r--   0        0        0   133768 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css
+-rw-r--r--   0        0        0   221079 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons.min.css
+-rw-r--r--   0        0        0      372 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/README.md
+-rw-r--r--   0        0        0      402 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-buildings/README.md
+-rw-r--r--   0        0        0      396 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-digital/README.md
+-rw-r--r--   0        0        0      399 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-document/README.md
+-rw-r--r--   0        0        0      408 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-environment/README.md
+-rw-r--r--   0        0        0      393 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-health/README.md
+-rw-r--r--   0        0        0      411 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-institutions/README.md
+-rw-r--r--   0        0        0      396 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-leisure/README.md
+-rw-r--r--   0        0        0      384 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-map/README.md
+-rw-r--r--   0        0        0      393 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/pictograms/pictograms-system/README.md
+-rw-r--r--   0        0        0   117145 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.legacy.min.css
+-rw-r--r--   0        0        0   168600 2024-04-25 13:02:07.348325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.main.min.css
+-rw-r--r--   0        0        0   317346 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.min.css
+-rw-r--r--   0        0        0    31959 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.print.min.css
+-rw-r--r--   0        0        0     3845 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/static/js/formsets.js
+-rw-r--r--   0        0        0      199 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/django/forms/errors/dict/ul.html
+-rw-r--r--   0        0        0      181 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/django/forms/errors/list/ul.html
+-rw-r--r--   0        0        0      554 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/checkbox_option.html
+-rw-r--r--   0        0        0      644 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/input_option.html
+-rw-r--r--   0        0        0      222 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/multiple_input.html
+-rw-r--r--   0        0        0      551 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/radio_option.html
+-rw-r--r--   0        0        0      407 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/accordion.html
+-rw-r--r--   0        0        0      138 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/accordion_group.html
+-rw-r--r--   0        0        0      699 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/alert.html
+-rw-r--r--   0        0        0      108 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/badge.html
+-rw-r--r--   0        0        0      148 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/badge_group.html
+-rw-r--r--   0        0        0     1673 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/base.html
+-rw-r--r--   0        0        0      851 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/breadcrumb.html
+-rw-r--r--   0        0        0      316 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/button.html
+-rw-r--r--   0        0        0      211 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/button_group.html
+-rw-r--r--   0        0        0      635 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/callout.html
+-rw-r--r--   0        0        0     3359 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/card.html
+-rw-r--r--   0        0        0     1214 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/consent.html
+-rw-r--r--   0        0        0     1366 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/content.html
+-rw-r--r--   0        0        0      707 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/favicon.html
+-rw-r--r--   0        0        0     2069 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/follow.html
+-rw-r--r--   0        0        0     5767 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/footer.html
+-rw-r--r--   0        0        0     2258 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_base.html
+-rw-r--r--   0        0        0      826 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/checkbox_snippet.html
+-rw-r--r--   0        0        0     1414 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html
+-rw-r--r--   0        0        0      471 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/field_snippet.html
+-rw-r--r--   0        0        0      984 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/input_snippet.html
+-rw-r--r--   0        0        0     1028 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/radioselect_snippet.html
+-rw-r--r--   0        0        0      335 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/form_snippet.html
+-rw-r--r--   0        0        0     1845 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/formset_base.html
+-rw-r--r--   0        0        0      999 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/france_connect.html
+-rw-r--r--   0        0        0      469 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/global_css.html
+-rw-r--r--   0        0        0      433 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/global_js.html
+-rw-r--r--   0        0        0     4619 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/header.html
+-rw-r--r--   0        0        0      205 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/highlight.html
+-rw-r--r--   0        0        0      565 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/input.html
+-rw-r--r--   0        0        0      427 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/link.html
+-rw-r--r--   0        0        0      576 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/notice.html
+-rw-r--r--   0        0        0     2187 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/pagination.html
+-rw-r--r--   0        0        0     1208 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/quote.html
+-rw-r--r--   0        0        0      892 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/select.html
+-rw-r--r--   0        0        0     3969 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/sidemenu.html
+-rw-r--r--   0        0        0      403 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/skiplinks.html
+-rw-r--r--   0        0        0      766 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/stepper.html
+-rw-r--r--   0        0        0      420 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/summary.html
+-rw-r--r--   0        0        0      264 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/summary_list.html
+-rw-r--r--   0        0        0      620 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/table.html
+-rw-r--r--   0        0        0      745 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/tag.html
+-rw-r--r--   0        0        0     3930 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/theme_modale.html
+-rw-r--r--   0        0        0     2127 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/tile.html
+-rw-r--r--   0        0        0      734 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/toggle.html
+-rw-r--r--   0        0        0      524 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/tooltip.html
+-rw-r--r--   0        0        0     1936 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templates/dsfr/transcription.html
+-rw-r--r--   0        0        0        0 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templatetags/__init__.py
+-rw-r--r--   0        0        0    43549 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/templatetags/dsfr_tags.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/test/__init__.py
+-rw-r--r--   0        0        0     2064 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/test/test_config.py
+-rw-r--r--   0        0        0    42738 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/test/test_templatetags.py
+-rw-r--r--   0        0        0     1116 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/test/test_utils.py
+-rw-r--r--   0        0        0     4149 2024-04-25 13:02:07.352325 django_dsfr-1.1.2/dsfr/utils.py
+-rw-r--r--   0        0        0     2213 2024-04-25 13:02:07.356325 django_dsfr-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4090 1970-01-01 00:00:00.000000 django_dsfr-1.1.2/PKG-INFO
```

### Comparing `django_dsfr-1.1.1/LICENSE` & `django_dsfr-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/README.rst` & `django_dsfr-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/admin.py` & `django_dsfr-1.1.2/dsfr/admin.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/checksums.py` & `django_dsfr-1.1.2/dsfr/checksums.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/constants.py` & `django_dsfr-1.1.2/dsfr/constants.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/forms.py` & `django_dsfr-1.1.2/dsfr/forms.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/locale/fr/LC_MESSAGES/django.mo` & `django_dsfr-1.1.2/dsfr/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/locale/fr/LC_MESSAGES/django.po` & `django_dsfr-1.1.2/dsfr/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/management/commands/integrity_checksums.py` & `django_dsfr-1.1.2/dsfr/management/commands/integrity_checksums.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/management/commands/make_icon_picker_files.py` & `django_dsfr-1.1.2/dsfr/management/commands/make_icon_picker_files.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/management/commands/trim_dist.py` & `django_dsfr-1.1.2/dsfr/management/commands/trim_dist.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0001_initial.py` & `django_dsfr-1.1.2/dsfr/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0002_auto_20211209_1557.py` & `django_dsfr-1.1.2/dsfr/migrations/0002_auto_20211209_1557.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py` & `django_dsfr-1.1.2/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0004_dsfrconfig_beta_tag_dsfrconfig_operator_logo_alt_and_more.py` & `django_dsfr-1.1.2/dsfr/migrations/0004_dsfrconfig_beta_tag_dsfrconfig_operator_logo_alt_and_more.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0005_dsfrconfig_notice.py` & `django_dsfr-1.1.2/dsfr/migrations/0005_dsfrconfig_notice.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0006_alter_dsfrconfig_accessibility_status.py` & `django_dsfr-1.1.2/dsfr/migrations/0006_alter_dsfrconfig_accessibility_status.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0007_dsfrconfig_newsletter_description_and_more.py` & `django_dsfr-1.1.2/dsfr/migrations/0007_dsfrconfig_newsletter_description_and_more.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/migrations/0008_alter_dsfrsocialmedia_options_dsfrconfig_language_and_more.py` & `django_dsfr-1.1.2/dsfr/migrations/0008_alter_dsfrsocialmedia_options_dsfrconfig_language_and_more.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/models.py` & `django_dsfr-1.1.2/dsfr/models.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/css/dsfr-code.css` & `django_dsfr-1.1.2/dsfr/static/css/dsfr-code.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-business.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-business.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-communication.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-communication.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-design.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-design.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-development.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-development.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-device.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-device.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-document.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-document.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-health.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-health.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-logo.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-logo.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-map.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-map.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-media.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-media.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-system.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-system.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-user.json` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/icons-libraries/dsfr-user.json`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/images/magnifying-glass-solid.svg` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/images/star-of-life-solid.svg` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/images/xmark-solid.svg` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.js` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.min.js` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/scss/universal-icon-picker.scss` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.css` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.min.css` & `django_dsfr-1.1.2/dsfr/static/django-dsfr/icon-picker/assets/stylesheets/universal-icon-picker.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/analytics/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/analytics/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/analytics/analytics.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/analytics/analytics.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/analytics/analytics.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/analytics/analytics.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/background/ovoid.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/background/ovoid.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/dark.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/dark.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/light.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/light.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/city-hall.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/city-hall.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/factory.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/factory.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/house.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/house.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/nuclear-plant.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/nuclear-plant.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/buildings/school.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/buildings/school.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/application.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/application.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/avatar.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/avatar.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/calendar.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/calendar.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/coding.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/coding.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/data-visualization.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/data-visualization.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/internet.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/internet.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/mail-send.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/mail-send.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/digital/search.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/digital/search.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/contract.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/contract.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document-add.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document-add.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document-download.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document-download.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document-signature.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document-signature.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/document.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/document.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/driving-licence.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/driving-licence.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/national-identity-card.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/national-identity-card.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/passport.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/passport.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/tax-stamp.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/tax-stamp.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/document/vehicle-registration.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/document/vehicle-registration.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/environment.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/environment.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/food.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/food.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/grocery.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/grocery.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/human-cooperation.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/human-cooperation.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/leaf.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/leaf.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/moon.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/moon.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/mountain.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/mountain.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/sun.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/sun.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/environment/tree.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/environment/tree.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/health.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/health.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/hospital.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/hospital.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/vaccine.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/vaccine.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/health/virus.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/health/virus.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/firefighter.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/firefighter.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/gendarmerie.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/gendarmerie.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/justice.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/justice.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/money.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/money.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/institutions/police.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/institutions/police.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/book.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/book.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/community.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/community.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/culture.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/culture.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/digital-art.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/digital-art.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/leisure/paint.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/leisure/paint.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/airport.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/airport.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/location-france.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/location-france.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/luggage.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/luggage.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/map/map.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/map/map.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/connection-lost.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/connection-lost.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/error.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/error.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/information.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/information.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/notification.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/notification.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/padlock.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/padlock.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/success.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/success.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/system.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/system.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/technical-error.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/technical-error.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/pictograms/system/warning.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/pictograms/system/warning.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/artwork/system.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/artwork/system.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/accordion/accordion.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/accordion/accordion.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/alert/alert.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/alert/alert.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/badge/badge.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/badge/badge.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/button/button.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/button/button.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/callout/callout.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/callout/callout.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/card/card.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/card/card.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/checkbox/checkbox.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/checkbox/checkbox.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/component.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/component.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/connect/connect.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/connect/connect.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/consent/consent.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/consent/consent.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/content/content.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/content/content.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/display/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/display/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/display/display.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/display/display.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/download/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/download/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/download/download.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/download/download.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/follow/follow.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/follow/follow.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/footer/footer.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/footer/footer.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/form/form.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/form/form.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/header/header.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/header/header.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/highlight/highlight.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/highlight/highlight.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-base/input-base.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-base/input-base.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-email/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-email/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input-tel/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input-tel/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/input/input.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/input/input.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/link/link.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/link/link.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/logo.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/logo.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/logo/logo.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/logo/logo.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/notice/notice.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/notice/notice.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/pagination/pagination.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/pagination/pagination.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/password/password.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/password/password.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/quote/quote.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/quote/quote.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/radio/radio.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/radio/radio.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/range/range.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/range/range.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/search/search.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/search/search.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/segmented/segmented.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/segmented/segmented.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/select/select.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/select/select.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/share/share.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/share/share.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/stepper/stepper.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/stepper/stepper.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/summary.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/summary.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/summary/summary.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/summary/summary.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tab/tab.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tab/tab.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/table/table.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/table/table.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tag/tag.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tag/tag.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tile/tile.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tile/tile.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/toggle/toggle.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/toggle/toggle.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/tooltip/tooltip.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/tooltip/tooltip.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/transcription/transcription.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/transcription/transcription.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/translate/translate.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/translate/translate.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/upload.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/upload.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/component/upload/upload.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/component/upload/upload.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/core/core.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/core/core.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/dsfr.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/dsfr.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/favicon.ico` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/favicon/favicon.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/favicon/favicon.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/buildings/store-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/buildings/store-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/global-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/global-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/business/global-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/business/global-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/brush-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/brush-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/design/palette-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/design/palette-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/development/bug-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/development/bug-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/phone-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/phone-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/device/wifi-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/device/wifi-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-3.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-3.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/editor/h-6.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/editor/h-6.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/dislike-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/dislike-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/lungs-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/lungs-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/microscope-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/microscope-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/virus-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/virus-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/health/virus-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/health/virus-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/github-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/github-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/github-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/github-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/google-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/google-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/ie-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/ie-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/safari-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/safari-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/slack-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/slack-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/threads-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/threads-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/threads-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/threads-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/earth-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/earth-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/earth-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/earth-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/france-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/france-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/france-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/france-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/recycle-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/recycle-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/team-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/team-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/icons/user/user-setting-line.svg` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/icons/user/user-setting-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/account/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/account/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/account/login/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/account/login/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/account/register/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/account/register/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/not-found/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/not-found/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/page/response/unexpected/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/page/response/unexpected/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/civility/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/civility/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/company/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/company/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/date/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/date/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/pattern/name/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/pattern/name/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/scheme/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/scheme/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/scheme/scheme.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/scheme/scheme.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/scheme/scheme.module.min.js` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/scheme/scheme.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/colors/colors.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/colors/colors.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/icons/icons.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/icons/icons.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.legacy.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.main.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/dsfr/dist/utility/utility.print.min.css` & `django_dsfr-1.1.2/dsfr/static/dsfr/dist/utility/utility.print.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/static/js/formsets.js` & `django_dsfr-1.1.2/dsfr/static/js/formsets.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/checkbox_option.html` & `django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/input_option.html` & `django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/input_option.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/django/forms/widgets/radio_option.html` & `django_dsfr-1.1.2/dsfr/templates/django/forms/widgets/radio_option.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/alert.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/alert.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/base.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/base.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/breadcrumb.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/callout.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/callout.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/card.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/card.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/consent.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/consent.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/content.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/content.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/favicon.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/favicon.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/follow.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/follow.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/footer.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/footer.html`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,22 @@
             <a class="fr-footer__brand-link"
                href="/"
                title="{{ back_to_home_label }} - {{ SITE_CONFIG.operator_logo_alt }} - {{ SITE_CONFIG.footer_brand|default:'république française' }}">
               <img class="fr-footer__logo"
                    src="{{ SITE_CONFIG.operator_logo_file.url }}"
                    alt="{{ SITE_CONFIG.operator_logo_alt }}"
                    {% if SITE_CONFIG.operator_logo_width >= 1 %}style="max-width:{{ SITE_CONFIG.operator_logo_width }}rem;"{% endif %} />
-              <!-- L’alternative de l’image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l’image -->
+              {# L’alternative de l’image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l’image #}
             </a>
           </div>
         {% else %}
           <div class="fr-footer__brand fr-enlarge-link">
             <a id="footer-operator"
                href="/"
-               title="{{ back_to_home_label }} - {{ SITE_CONFIG.site_title }} - {{ SITE_CONFIG.footer_brand|default:'république française' }}"
-               None="{{ SITE_CONFIG.footer_brand|default:'république française' }}">
+               title="{{ back_to_home_label }} - {{ SITE_CONFIG.site_title }} - {{ SITE_CONFIG.footer_brand|default:'république française' }}">
               {% block brand %}
                 <p class="fr-logo">
                   {{ SITE_CONFIG.footer_brand_html| default_if_none:'république<br />française' | safe }}
                 </p>
               {% endblock brand %}
             </a>
           </div>
```

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/form_base.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/form_base.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-<!-- Created on Mon Jan 24 13:32:00 2022 @author: alica.burlot -->
-<!-- base template for all forms -->
-<!-- to be extended in the templates where a form is displayed -->
-<!-- Check django comments for more information -->
-<!-- extends your base.html template -->
+{# Created on Mon Jan 24 13:32:00 2022 @author: alica.burlot #}
+{# base template for all forms #}
+{# to be extended in the templates where a form is displayed #}
+{# Check django comments for more information #}
+{# extends your base.html template #}
 {% extends "dsfr/base.html" %}
 {% load static dsfr_tags widget_tweaks %}
 {% comment %}
 Radio button and multiple checkboxes :
     -Help text under each button/checkbox :
         In your forms.py, in the ChoiceField or MultipleChoiceField,
         instead of choices=(("a", "label a"), ("b", "label b"), ...),
```

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/checkbox_snippet.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/checkbox_snippet.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/input_snippet.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/input_snippet.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/form_field_snippets/radioselect_snippet.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/form_field_snippets/radioselect_snippet.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/formset_base.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/formset_base.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/france_connect.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/france_connect.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/header.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/header.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/input.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/input.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/notice.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/notice.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/pagination.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/pagination.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/quote.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/quote.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/select.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/select.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/sidemenu.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/sidemenu.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/stepper.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/stepper.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/table.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/table.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/tag.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/tag.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/theme_modale.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/theme_modale.html`

 * *Files 3% similar despite different names*

```diff
@@ -30,42 +30,42 @@
                              id="fr-radios-theme-light"
                              name="fr-radios-theme" />
                       <label class="fr-label" for="fr-radios-theme-light">
                         {% translate "Light theme" %}
                       </label>
                       <div class="fr-radio-rich__img" data-fr-inject-svg>
                         <img src="{% static 'dsfr/dist/artwork/light.svg' %}" alt="" />
-                        <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
+                        {# L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance #}
                       </div>
                     </div>
                     <div class="fr-radio-group fr-radio-rich">
                       <input value="dark"
                              type="radio"
                              id="fr-radios-theme-dark"
                              name="fr-radios-theme" />
                       <label class="fr-label" for="fr-radios-theme-dark">
                         {% translate "Dark theme" %}
                       </label>
                       <div class="fr-radio-rich__img" data-fr-inject-svg>
                         <img src="{% static 'dsfr/dist/artwork/dark.svg' %}" alt="" />
-                        <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
+                        {# L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance #}
                       </div>
                     </div>
                     <div class="fr-radio-group fr-radio-rich">
                       <input value="system"
                              type="radio"
                              id="fr-radios-theme-system"
                              name="fr-radios-theme" />
                       <label class="fr-label" for="fr-radios-theme-system">
                         {% translate "System" %}
                         <span class="fr-hint-text">{% translate "Uses system settings." %}</span>
                       </label>
                       <div class="fr-radio-rich__img" data-fr-inject-svg>
                         <img src="{% static 'dsfr/dist/artwork/system.svg' %}" alt="" />
-                        <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
+                        {# L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance #}
                       </div>
                     </div>
                   </div>
                 </fieldset>
               </div>
             </div>
           </div>
```

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/tile.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/tile.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/toggle.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/toggle.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/tooltip.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/tooltip.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templates/dsfr/transcription.html` & `django_dsfr-1.1.2/dsfr/templates/dsfr/transcription.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/templatetags/dsfr_tags.py` & `django_dsfr-1.1.2/dsfr/templatetags/dsfr_tags.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/test/test_config.py` & `django_dsfr-1.1.2/dsfr/test/test_config.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/test/test_templatetags.py` & `django_dsfr-1.1.2/dsfr/test/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/test/test_utils.py` & `django_dsfr-1.1.2/dsfr/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/dsfr/utils.py` & `django_dsfr-1.1.2/dsfr/utils.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-1.1.1/pyproject.toml` & `django_dsfr-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Sylvain Boissel <sylvain.boissel@beta.gouv.fr>"]
 description = "Integrate the French government Design System into a Django app"
 license = "MIT"
 name = "django-dsfr"
-version = "1.1.1"
+version = "1.1.2"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_dsfr-1.1.1/PKG-INFO` & `django_dsfr-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dsfr
-Version: 1.1.1
+Version: 1.1.2
 Summary: Integrate the French government Design System into a Django app
 Home-page: https://github.com/numerique-gouv/django-dsfr
 License: MIT
 Keywords: django
 Author: Sylvain Boissel
 Author-email: sylvain.boissel@beta.gouv.fr
 Requires-Python: >=3.8,<4.0
```

