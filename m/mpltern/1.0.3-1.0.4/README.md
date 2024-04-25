# Comparing `tmp/mpltern-1.0.3.tar.gz` & `tmp/mpltern-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltern-1.0.3.tar", last modified: Sat Mar 23 19:03:23 2024, max compression
+gzip compressed data, was "mpltern-1.0.4.tar", last modified: Thu Apr 25 20:52:30 2024, max compression
```

## Comparing `mpltern-1.0.3.tar` & `mpltern-1.0.4.tar`

### file list

```diff
@@ -1,547 +1,551 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.253045 mpltern-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.157044 mpltern-1.0.3/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-23 19:03:19.000000 mpltern-1.0.3/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-23 19:03:19.000000 mpltern-1.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.149044 mpltern-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.157044 mpltern-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-23 19:03:19.000000 mpltern-1.0.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-23 19:03:19.000000 mpltern-1.0.3/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-03-23 19:03:19.000000 mpltern-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-23 19:03:19.000000 mpltern-1.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-23 19:03:19.000000 mpltern-1.0.3/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-23 19:03:19.000000 mpltern-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-23 19:03:19.000000 mpltern-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-23 19:03:23.253045 mpltern-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-23 19:03:19.000000 mpltern-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.157044 mpltern-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-23 19:03:19.000000 mpltern-1.0.3/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.161044 mpltern-1.0.3/docsrc/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.161044 mpltern-1.0.3/docsrc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/_static/logo_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/_static/logo_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/_static/mpl.css
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/corner_based_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    50242 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/corner_based_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/corner_based_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    52879 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/corner_based_2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/create_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/implemented_methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/publications.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/side_based_ccw.py
--rw-r--r--   0 runner    (1001) docker     (127)    54814 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/side_based_ccw.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/side_based_cw.py
--rw-r--r--   0 runner    (1001) docker     (127)    53409 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/side_based_cw.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.161044 mpltern-1.0.3/docsrc/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/sphinxext/custom_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.165044 mpltern-1.0.3/docsrc/users/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/users/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/users/mpltern_1.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/users/mpltern_1.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/users/mpltern_1.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/users/mpltern_1.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-23 19:03:19.000000 mpltern-1.0.3/docsrc/users/release_notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.165044 mpltern-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.165044 mpltern-1.0.3/examples/axis_and_tick/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/00.axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/01.axis_label_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/10.tick_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/11.tick_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/12.tick_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/20.tick-formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/21.tick-locators.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/30.manual_tick_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/31.manual_ticklabels.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/98.colored_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/99.tick_labels_inside_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/axis_and_tick/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.165044 mpltern-1.0.3/examples/intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/intermediate/00.with_normal_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/intermediate/01.style_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/intermediate/99.inset.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/intermediate/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.169044 mpltern-1.0.3/examples/introductory/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/00.line_and_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/01.scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/02.contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/03.pseudocolor.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/04.normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/05.span.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/06.text.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/07.polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/08.quiver.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/09.grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/10.axis_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/11.triangular_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/axline.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/introductory/legend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.169044 mpltern-1.0.3/examples/limits/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/limits/00.triangular_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/limits/01.hexagonal_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/limits/02.fit.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/limits/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.169044 mpltern-1.0.3/examples/miscellaneous/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/miscellaneous/00.logos.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/miscellaneous/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/miscellaneous/dirichlet_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/miscellaneous/evolutionary_game_theory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/miscellaneous/soil_texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.169044 mpltern-1.0.3/examples/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/statistics/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/statistics/hexbin.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/statistics/tribin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/statistics/with_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.173044 mpltern-1.0.3/examples/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/transforms/00.cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/transforms/01.ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/transforms/06.plot_fixed_onto_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/transforms/99.arrows_along_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/transforms/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.173044 mpltern-1.0.3/examples/triangle/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/triangle/00.aspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/triangle/01.triangle_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/triangle/02.arbitrary_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 19:03:19.000000 mpltern-1.0.3/examples/triangle/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.173044 mpltern-1.0.3/mpltern/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/_ternary_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/hexbin_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.177044 mpltern-1.0.3/mpltern/ternary/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28616 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)    32605 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/spines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/tick.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/ternary/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-03-23 19:03:19.000000 mpltern-1.0.3/mpltern/tribin_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.253045 mpltern-1.0.3/mpltern.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-23 19:03:23.000000 mpltern-1.0.3/mpltern.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28785 2024-03-23 19:03:23.000000 mpltern-1.0.3/mpltern.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 19:03:23.000000 mpltern-1.0.3/mpltern.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 19:03:23.000000 mpltern-1.0.3/mpltern.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-23 19:03:23.000000 mpltern-1.0.3/mpltern.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-23 19:03:19.000000 mpltern-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-23 19:03:19.000000 mpltern-1.0.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 19:03:23.253045 mpltern-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-03-23 19:03:19.000000 mpltern-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.181044 mpltern-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/Dirichlet_PDF_1.0_2.0_2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/Dirichlet_PDF_1.5_1.5_1.5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/Dirichlet_PDF_2.0_4.0_8.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/Dirichlet_PDF_5.0_5.0_5.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.153044 mpltern-1.0.3/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.181044 mpltern-1.0.3/tests/baseline_images/test_constrainedlayout/
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.181044 mpltern-1.0.3/tests/baseline_images/test_given_triangles/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.181044 mpltern-1.0.3/tests/baseline_images/test_hexbin/
--rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_hexbin/base.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_hexbin/extent.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_hexbin/given_triangles.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    20041 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_hexbin/ternary_lim.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.193045 mpltern-1.0.3/tests/baseline_images/test_ternary/
--rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/arguments_6.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/arguments_7.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_axes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_data.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_xy_axes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_xy_data.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/aspect.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/axis_label_position_corner.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/axis_label_position_tick1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/axis_label_position_tick2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/fit_none.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/fit_rectangle.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/fit_triangle.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/legend.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/manual_ticklabels.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/manual_ticks.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/negative_ticks.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/opposite_ticks.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/plot.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/quiver.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    16075 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/quiver_color.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/quiver_xy_axes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/quiver_xy_data.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/scatter.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    19943 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/scatter_color.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/spans.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    65470 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected.png
--rw-r--r--   0 runner    (1001) docker     (127)    38681 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png
--rw-r--r--   0 runner    (1001) docker     (127)    63063 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    65470 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim.png
--rw-r--r--   0 runner    (1001) docker     (127)    38681 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png
--rw-r--r--   0 runner    (1001) docker     (127)    63063 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim_svg.png
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/text.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/tick_direction_in.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/tick_direction_inout.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/tick_direction_out.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/titie_center.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/titie_left.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/titie_right.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_ternary/transAxes.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.193045 mpltern-1.0.3/tests/baseline_images/test_tightlayout/
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_tightlayout/tight_layout1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.213045 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.233044 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.249045 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:03:23.253045 mpltern-1.0.3/tests/baseline_images/test_tribin/
--rw-r--r--   0 runner    (1001) docker     (127)   114587 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_tribin/base.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    27785 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_tribin/extent.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   121032 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_tribin/given_triangles.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   115121 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/baseline_images/test_tribin/ternary_lim.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/hexbin_indices.txt
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/make_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    25306 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_constrainedlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_given_triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_hexbin.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_hexbin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_spines.py
--rw-r--r--   0 runner    (1001) docker     (127)    29734 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    25669 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_tick.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_tightlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_triangle_rotation_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_triangle_rotation_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_triangle_rotation_tick.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_tribin.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/test_tribin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-23 19:03:19.000000 mpltern-1.0.3/tests/tribin_indices.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-23 19:03:19.000000 mpltern-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.609536 mpltern-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.517535 mpltern-1.0.4/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-25 20:52:26.000000 mpltern-1.0.4/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 20:52:26.000000 mpltern-1.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.513535 mpltern-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.517535 mpltern-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-25 20:52:26.000000 mpltern-1.0.4/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-25 20:52:26.000000 mpltern-1.0.4/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-25 20:52:26.000000 mpltern-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 20:52:26.000000 mpltern-1.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 20:52:26.000000 mpltern-1.0.4/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 20:52:26.000000 mpltern-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 20:52:26.000000 mpltern-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-25 20:52:30.609536 mpltern-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-25 20:52:26.000000 mpltern-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.517535 mpltern-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 20:52:26.000000 mpltern-1.0.4/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.521535 mpltern-1.0.4/docsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.521535 mpltern-1.0.4/docsrc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/_static/logo_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/_static/logo_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/_static/mpl.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/corner_based_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50242 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/corner_based_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/corner_based_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52879 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/corner_based_2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/create_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/implemented_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/publications.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/side_based_ccw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54814 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/side_based_ccw.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/side_based_cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53409 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/side_based_cw.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.521535 mpltern-1.0.4/docsrc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/sphinxext/custom_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.521535 mpltern-1.0.4/docsrc/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/mpltern_1.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/mpltern_1.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/mpltern_1.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/mpltern_1.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/mpltern_1.0.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-25 20:52:26.000000 mpltern-1.0.4/docsrc/users/release_notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.521535 mpltern-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.525535 mpltern-1.0.4/examples/axis_and_tick/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/00.axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/01.axis_label_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/10.tick_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/11.tick_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/12.tick_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/20.tick-formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/21.tick-locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/30.manual_tick_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/31.manual_ticklabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/98.colored_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/99.tick_labels_inside_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/axis_and_tick/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.525535 mpltern-1.0.4/examples/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/intermediate/00.with_normal_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/intermediate/01.style_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/intermediate/99.inset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/intermediate/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.529535 mpltern-1.0.4/examples/introductory/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/00.line_and_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/01.scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/02.contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/03.pseudocolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/04.normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/05.span.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/06.text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/07.polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/08.quiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/09.grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/10.axis_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/11.triangular_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/axline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/introductory/legend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.529535 mpltern-1.0.4/examples/limits/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/limits/00.triangular_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/limits/01.hexagonal_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/limits/02.fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/limits/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.529535 mpltern-1.0.4/examples/miscellaneous/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/miscellaneous/00.logos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/miscellaneous/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/miscellaneous/dirichlet_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/miscellaneous/evolutionary_game_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/miscellaneous/soil_texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.529535 mpltern-1.0.4/examples/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/statistics/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/statistics/hexbin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/statistics/tribin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/statistics/with_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.529535 mpltern-1.0.4/examples/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/transforms/00.cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/transforms/01.ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/transforms/06.plot_fixed_onto_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/transforms/99.arrows_along_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/transforms/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.529535 mpltern-1.0.4/examples/triangle/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/triangle/00.aspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/triangle/01.triangle_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/triangle/02.arbitrary_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 20:52:26.000000 mpltern-1.0.4/examples/triangle/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.533535 mpltern-1.0.4/mpltern/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/_ternary_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/hexbin_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.533535 mpltern-1.0.4/mpltern/ternary/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28582 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32748 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/spines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/tick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/ternary/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-25 20:52:26.000000 mpltern-1.0.4/mpltern/tribin_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.609536 mpltern-1.0.4/mpltern.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-25 20:52:30.000000 mpltern-1.0.4/mpltern.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29006 2024-04-25 20:52:30.000000 mpltern-1.0.4/mpltern.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:52:30.000000 mpltern-1.0.4/mpltern.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 20:52:30.000000 mpltern-1.0.4/mpltern.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 20:52:30.000000 mpltern-1.0.4/mpltern.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 20:52:26.000000 mpltern-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 20:52:26.000000 mpltern-1.0.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:52:30.609536 mpltern-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-25 20:52:26.000000 mpltern-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.537535 mpltern-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/Dirichlet_PDF_1.0_2.0_2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/Dirichlet_PDF_1.5_1.5_1.5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/Dirichlet_PDF_2.0_4.0_8.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/Dirichlet_PDF_5.0_5.0_5.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.513535 mpltern-1.0.4/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.537535 mpltern-1.0.4/tests/baseline_images/test_constrainedlayout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.541535 mpltern-1.0.4/tests/baseline_images/test_given_triangles/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.541535 mpltern-1.0.4/tests/baseline_images/test_hexbin/
+-rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_hexbin/base.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_hexbin/extent.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_hexbin/given_triangles.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    20041 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_hexbin/ternary_lim.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.553535 mpltern-1.0.4/tests/baseline_images/test_ternary/
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/arguments_6.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/arguments_7.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_axes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_data.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_xy_axes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_xy_data.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/aspect.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_corner_axis.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_corner_horizontal.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_tick1_axis.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_tick1_horizontal.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_tick2_axis.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_tick2_horizontal.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/fit_none.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/fit_rectangle.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/fit_triangle.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/legend.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/manual_ticklabels.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/manual_ticks.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/negative_ticks.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/opposite_ticks.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/plot.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/quiver.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    16075 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/quiver_color.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/quiver_xy_axes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/quiver_xy_data.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/scatter.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    19943 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/scatter_color.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/spans.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    65470 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38681 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63063 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    65470 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38681 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63063 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim_svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/text.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/tick_direction_in.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/tick_direction_inout.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/tick_direction_out.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/titie_center.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/titie_left.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/titie_right.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_ternary/transAxes.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.553535 mpltern-1.0.4/tests/baseline_images/test_tightlayout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_tightlayout/tight_layout1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.569536 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.589536 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.609536 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:52:30.609536 mpltern-1.0.4/tests/baseline_images/test_tribin/
+-rw-r--r--   0 runner    (1001) docker     (127)   114587 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_tribin/base.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    27785 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_tribin/extent.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   121032 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_tribin/given_triangles.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   115121 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/baseline_images/test_tribin/ternary_lim.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/hexbin_indices.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/make_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25306 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_constrainedlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_given_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_hexbin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_hexbin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_spines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30233 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25669 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_tick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_tightlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_triangle_rotation_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_triangle_rotation_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_triangle_rotation_tick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_tribin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/test_tribin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 20:52:26.000000 mpltern-1.0.4/tests/tribin_indices.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 20:52:26.000000 mpltern-1.0.4/tox.ini
```

### Comparing `mpltern-1.0.3/.circleci/config.yml` & `mpltern-1.0.4/.circleci/config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             sudo apt -qq update
             sudo apt-get -y install ghostscript inkscape
       - run:
           name: Install dependencies
           command: |
             python -m pip install --upgrade pip
             python -m pip install setuptools==59.8.0 # Matplotlib 3.4
-            python -m pip install numpy==1.24
+            python -m pip install numpy==1.26.4
             python -m pip install pillow==9.0
             python -m pip install matplotlib==<< parameters.matplotlib-version >>
             python -m pip install pytest>=4.6
             python -m pip install pytest-cov
             python -m pip install codecov coverage
       - run:
           name: Test with pytest
```

### Comparing `mpltern-1.0.3/.github/workflows/publish-to-test-pypi.yml` & `mpltern-1.0.4/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/.github/workflows/tests.yml` & `mpltern-1.0.4/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           sudo apt-get update -yy
           sudo apt-get install -yy \
             inkscape
       - name: Install Python dependencies
         run: |
           python -m pip install --upgrade pip
 
-          python -m pip install numpy==1.24.4
+          python -m pip install numpy==1.26.4
           python -m pip install pillow==9.0
           python -m pip install matplotlib==${{ matrix.matplotlib-version }}
           python -m pip install pytest>=4.6
           python -m pip install pytest-cov
           python -m pip install codecov coverage
       - name: Run pytest
         run: |
```

### Comparing `mpltern-1.0.3/.gitignore` & `mpltern-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/LICENSE` & `mpltern-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/PKG-INFO` & `mpltern-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltern
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ternary plots as projections of Matplotlib
 Home-page: https://github.com/yuzie007/mpltern
 Author: Yuji Ikeda
 Author-email: yuji.ikeda.ac.jp@gmail.com
 Project-URL: Bug Reports, https://github.com/yuzie007/mpltern/issues
 Project-URL: Source, https://github.com/yuzie007/mpltern
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mpltern-1.0.3/README.rst` & `mpltern-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/Makefile` & `mpltern-1.0.4/docsrc/Makefile`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/_static/favicon.ico` & `mpltern-1.0.4/docsrc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/_static/logo_dark.svg` & `mpltern-1.0.4/docsrc/_static/logo_dark.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/_static/logo_light.svg` & `mpltern-1.0.4/docsrc/_static/logo_light.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/alternatives.rst` & `mpltern-1.0.4/docsrc/alternatives.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/api.rst` & `mpltern-1.0.4/docsrc/api.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/basic_usage.rst` & `mpltern-1.0.4/docsrc/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/conf.py` & `mpltern-1.0.4/docsrc/conf.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/conventions.rst` & `mpltern-1.0.4/docsrc/conventions.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/corner_based_1.py` & `mpltern-1.0.4/docsrc/corner_based_1.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/corner_based_1.svg` & `mpltern-1.0.4/docsrc/corner_based_1.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/corner_based_2.py` & `mpltern-1.0.4/docsrc/corner_based_2.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/corner_based_2.svg` & `mpltern-1.0.4/docsrc/corner_based_2.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/implemented_methods.rst` & `mpltern-1.0.4/docsrc/implemented_methods.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/installation.rst` & `mpltern-1.0.4/docsrc/installation.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/make.bat` & `mpltern-1.0.4/docsrc/make.bat`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/publications.rst` & `mpltern-1.0.4/docsrc/publications.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/side_based_ccw.py` & `mpltern-1.0.4/docsrc/side_based_ccw.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/side_based_ccw.svg` & `mpltern-1.0.4/docsrc/side_based_ccw.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/side_based_cw.py` & `mpltern-1.0.4/docsrc/side_based_cw.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/side_based_cw.svg` & `mpltern-1.0.4/docsrc/side_based_cw.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/sphinxext/custom_roles.py` & `mpltern-1.0.4/docsrc/sphinxext/custom_roles.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/docsrc/users/release_notes.rst` & `mpltern-1.0.4/docsrc/users/release_notes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #############
 Release notes
 #############
 
+.. include:: mpltern_1.0.4.rst
 .. include:: mpltern_1.0.3.rst
 .. include:: mpltern_1.0.2.rst
 .. include:: mpltern_1.0.1.rst
 .. include:: mpltern_1.0.0.rst
 
 mpltern 0.5.0 (2023-02-22)
 ==========================
```

### Comparing `mpltern-1.0.3/examples/axis_and_tick/00.axis_label_position.py` & `mpltern-1.0.4/examples/axis_and_tick/00.axis_label_position.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/01.axis_label_rotation.py` & `mpltern-1.0.4/examples/axis_and_tick/01.axis_label_rotation.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/10.tick_position.py` & `mpltern-1.0.4/examples/axis_and_tick/10.tick_position.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/11.tick_direction.py` & `mpltern-1.0.4/examples/axis_and_tick/11.tick_direction.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/12.tick_rotation.py` & `mpltern-1.0.4/examples/axis_and_tick/12.tick_rotation.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/20.tick-formatters.py` & `mpltern-1.0.4/examples/axis_and_tick/20.tick-formatters.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/21.tick-locators.py` & `mpltern-1.0.4/examples/axis_and_tick/21.tick-locators.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/30.manual_tick_positions.py` & `mpltern-1.0.4/examples/axis_and_tick/30.manual_tick_positions.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/31.manual_ticklabels.py` & `mpltern-1.0.4/examples/axis_and_tick/31.manual_ticklabels.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/98.colored_axes.py` & `mpltern-1.0.4/examples/axis_and_tick/98.colored_axes.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/axis_and_tick/99.tick_labels_inside_triangle.py` & `mpltern-1.0.4/examples/axis_and_tick/99.tick_labels_inside_triangle.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/intermediate/00.with_normal_plots.py` & `mpltern-1.0.4/examples/intermediate/00.with_normal_plots.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/intermediate/01.style_sheets.py` & `mpltern-1.0.4/examples/intermediate/01.style_sheets.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/intermediate/99.inset.py` & `mpltern-1.0.4/examples/intermediate/99.inset.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/01.scatter.py` & `mpltern-1.0.4/examples/introductory/01.scatter.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/02.contour.py` & `mpltern-1.0.4/examples/introductory/02.contour.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/03.pseudocolor.py` & `mpltern-1.0.4/examples/introductory/03.pseudocolor.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/04.normalization.py` & `mpltern-1.0.4/examples/introductory/04.normalization.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/05.span.py` & `mpltern-1.0.4/examples/introductory/05.span.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/07.polygon.py` & `mpltern-1.0.4/examples/introductory/07.polygon.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/08.quiver.py` & `mpltern-1.0.4/examples/introductory/08.quiver.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/introductory/axline.py` & `mpltern-1.0.4/examples/introductory/axline.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/limits/00.triangular_limits.py` & `mpltern-1.0.4/examples/limits/00.triangular_limits.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/limits/01.hexagonal_limits.py` & `mpltern-1.0.4/examples/limits/01.hexagonal_limits.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/limits/02.fit.py` & `mpltern-1.0.4/examples/limits/02.fit.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/miscellaneous/00.logos.py` & `mpltern-1.0.4/examples/miscellaneous/00.logos.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/miscellaneous/dirichlet_pdf.py` & `mpltern-1.0.4/examples/miscellaneous/dirichlet_pdf.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/miscellaneous/evolutionary_game_theory.py` & `mpltern-1.0.4/examples/miscellaneous/evolutionary_game_theory.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/miscellaneous/soil_texture.py` & `mpltern-1.0.4/examples/miscellaneous/soil_texture.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/statistics/hexbin.py` & `mpltern-1.0.4/examples/statistics/hexbin.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/statistics/tribin.py` & `mpltern-1.0.4/examples/statistics/tribin.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/statistics/with_scatter.py` & `mpltern-1.0.4/examples/statistics/with_scatter.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/transforms/00.cartesian.py` & `mpltern-1.0.4/examples/transforms/00.cartesian.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/transforms/01.ticks.py` & `mpltern-1.0.4/examples/transforms/01.ticks.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/transforms/06.plot_fixed_onto_triangle.py` & `mpltern-1.0.4/examples/transforms/06.plot_fixed_onto_triangle.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/transforms/99.arrows_along_axes.py` & `mpltern-1.0.4/examples/transforms/99.arrows_along_axes.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/transforms/README.rst` & `mpltern-1.0.4/examples/transforms/README.rst`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/examples/triangle/01.triangle_rotation.py` & `mpltern-1.0.4/examples/triangle/01.triangle_rotation.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern/__init__.py` & `mpltern-1.0.4/mpltern/__init__.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern/_ternary_parsers.py` & `mpltern-1.0.4/mpltern/_ternary_parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import functools
+from collections.abc import Iterable
 
 import numpy as np
 import matplotlib as mpl
 
 
 def _get_xy(ax, this, trans):
     t, l, r = this
     tlr = np.column_stack((t, l, r))
     if trans == ax.transTernaryAxes:
         trans_xy = ax.transOuterAxes
         x, y = ax.transAxesProjection.transform(tlr).T
     else:
         trans_xy = ax.transData
         x, y = ax.transProjection.transform(tlr).T
+    # If t, l, r are scalar, x, y are also converted to scalar.
+    # This is to address `DeprecationWarning` raised since NumPy 1.25.0.
+    # https://github.com/numpy/numpy/pull/10615
+    if not any(isinstance(_, Iterable) for _ in (t, l, r)):
+        x = x.item()
+        y = y.item()
     return x, y, trans_xy
 
 
 def parse_ternary_single(f):
     """
     Parse ternary data from the first 3 arguments.
     """
@@ -85,42 +92,14 @@
     """
     Parse ternary data from the first 6 arguments.
     """
     @functools.wraps(f)
     def parse(ax, *args, **kwargs):
         trans = kwargs.pop('transform', None)
         # If no `args` are given, return an empty list like Matplotlib
-        # by calling the superclass method via `f`.
-        if not args or (trans is not None and trans.input_dims == 2):
-            kwargs['transform'] = trans
-            return f(ax, *args, **kwargs)
-
-        tlr0, args = args[:3], args[3:]
-        tlr1, args = args[:3], args[3:]
-        tlr0 = np.asarray(tlr0)
-        tlr1 = np.asarray(tlr1)
-        tlr1 += tlr0
-        x0, y0, kwargs['transform'] = _get_xy(ax, tlr0, trans)
-        x1, y1, kwargs['transform'] = _get_xy(ax, tlr1, trans)
-        dx = x1 - x0
-        dy = y1 - y0
-        args = (x0.item(), y0.item(), dx.item(), dy.item(), *args)
-        return f(ax, *args, **kwargs)
-
-    return parse
-
-
-def parse_ternary_vector_field(f):
-    """
-    Parse ternary data from the first 6 arguments.
-    """
-    @functools.wraps(f)
-    def parse(ax, *args, **kwargs):
-        trans = kwargs.pop('transform', None)
-        # If no `args` are given, return an empty list like Matplotlib
         # by calling the superclass method via `f`.
         if not args or (trans is not None and trans.input_dims == 2):
             kwargs['transform'] = trans
             return f(ax, *args, **kwargs)
 
         tlr0, args = args[:3], args[3:]
         tlr1, args = args[:3], args[3:]
```

### Comparing `mpltern-1.0.3/mpltern/datasets.py` & `mpltern-1.0.4/mpltern/datasets.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern/hexbin_helpers.py` & `mpltern-1.0.4/mpltern/hexbin_helpers.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern/ternary/_axes.py` & `mpltern-1.0.4/mpltern/ternary/_axes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import matplotlib.collections as mcoll
 import matplotlib.colors as mcolors
 import matplotlib.lines as mlines
 import matplotlib.patches as mpatches
 import matplotlib.transforms as mtransforms
 from matplotlib import _api
 from mpltern._ternary_parsers import (
-    parse_ternary_single, parse_ternary_multiple,
-    parse_ternary_vector, parse_ternary_vector_field)
+    parse_ternary_single,
+    parse_ternary_multiple,
+    parse_ternary_vector,
+)
 from mpltern import hexbin_helpers
 from mpltern import tribin_helpers
 from mpltern.ternary._base import TernaryAxesBase
 
 
 class TernaryAxes(TernaryAxesBase):
     """
@@ -416,26 +418,26 @@
 
             %(PolyCollection:kwdoc)s
 
         See Also
         --------
         tribin : 2D histogram triangular bins
         """
-        t, l, r = _normalize_tlr(t, l, r, self.ternary_sum)
-
         self._process_unit_info(
             [("t", t), ("l", l), ("r", r)], kwargs, convert=False)
 
         t, l, r, C = cbook.delete_masked_points(t, l, r, C)
 
         # Count the number of data in each hexagon
         t = np.asarray(t, float)
         l = np.asarray(l, float)
         r = np.asarray(r, float)
 
+        t, l, r = _normalize_tlr(t, l, r, self.ternary_sum)
+
         if extent is not None:
             tmin, tmax, lmin, lmax, rmin, rmax = extent
         else:
             tmin, tmax = self.get_tlim()
             lmin, lmax = self.get_llim()
             rmin, rmax = self.get_rlim()
 
@@ -658,26 +660,26 @@
 
             %(PolyCollection:kwdoc)s
 
         See Also
         --------
         hexbin : 2D histogram hexagonal bins
         """
-        t, l, r = _normalize_tlr(t, l, r, self.ternary_sum)
-
         self._process_unit_info(
             [("t", t), ("l", l), ("r", r)], kwargs, convert=False)
 
         t, l, r, C = cbook.delete_masked_points(t, l, r, C)
 
         # Count the number of data in each triangle
         t = np.asarray(t, float)
         l = np.asarray(l, float)
         r = np.asarray(r, float)
 
+        t, l, r = _normalize_tlr(t, l, r, self.ternary_sum)
+
         if extent is not None:
             tmin, tmax, lmin, lmax, rmin, rmax = extent
         else:
             tmin, tmax = self.get_tlim()
             lmin, lmax = self.get_llim()
             rmin, rmax = self.get_rlim()
 
@@ -784,16 +786,16 @@
         collection._scale_norm(norm, vmin, vmax)
 
         # add the collection last
         self.add_collection(collection, autolim=False)
         return collection
 
     arrow = parse_ternary_vector(TernaryAxesBase.arrow)
-    quiver = parse_ternary_vector_field(TernaryAxesBase.quiver)
-    barbs = parse_ternary_vector_field(TernaryAxesBase.barbs)
+    quiver = parse_ternary_vector(TernaryAxesBase.quiver)
+    barbs = parse_ternary_vector(TernaryAxesBase.barbs)
     fill = parse_ternary_multiple(TernaryAxesBase.fill)
     hist2d = parse_ternary_single(TernaryAxesBase.hist2d)
     tricontour = parse_ternary_single(TernaryAxesBase.tricontour)
     tricontourf = parse_ternary_single(TernaryAxesBase.tricontourf)
     tripcolor = parse_ternary_single(TernaryAxesBase.tripcolor)
     triplot = parse_ternary_single(TernaryAxesBase.triplot)
```

### Comparing `mpltern-1.0.3/mpltern/ternary/_base.py` & `mpltern-1.0.4/mpltern/ternary/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from matplotlib.axes import Axes
 from matplotlib import _api
 from mpltern.ternary.spines import Spine
 from mpltern.ternary.transforms import (
     TernaryAxisTransform, TernaryTickLabelShift,
     TernaryAxisLabelSTransform, TernaryAxisLabelCTransform,
     H2THeightTransform, H2TWidthTransform,
+    TernaryLinearTransform,
     BarycentricTransform)
 from mpltern.ternary.axis import TAxis, LAxis, RAxis
 
 _log = logging.getLogger(__name__)
 
 
 def _create_corners(corners=None, rotation=None):
@@ -92,15 +93,15 @@
             0.0, ternary_sum,
             0.0, ternary_sum,
             0.0, ternary_sum,
         )
 
     @property
     def callbacks(self):
-        if tuple(int(_) for _ in mpl.__version__.split('.'))[:2] < (3, 6):
+        if tuple(int(_) for _ in mpl.__version__.split('.')[:2]) < (3, 6):
             return cbook.CallbackRegistry()
         else:
             return cbook.CallbackRegistry(
                signals=[f"{name}lim_changed" for name in self._axis_names])
 
     @callbacks.setter
     def callbacks(self, value):
@@ -147,14 +148,17 @@
         self.spines['lcorner'].register_axis(self.laxis)
         self.spines['rcorner'].register_axis(self.raxis)
 
         self._update_transScale()
 
     def _set_lim_and_transforms(self):
         super()._set_lim_and_transforms()
+
+        self.transTernaryScale = TernaryLinearTransform(self.ternary_sum)
+
         transTLimits = mtransforms.BboxTransformFrom(
             mtransforms.TransformedBbox(self.viewOuterTLim, self.transScale))
         transLLimits = mtransforms.BboxTransformFrom(
             mtransforms.TransformedBbox(self.viewOuterLLim, self.transScale))
         transRLimits = mtransforms.BboxTransformFrom(
             mtransforms.TransformedBbox(self.viewOuterRLim, self.transScale))
 
@@ -189,15 +193,16 @@
         self._llabel_s_transform = TernaryAxisLabelSTransform(laxis_tr, h2t_l)
         self._rlabel_s_transform = TernaryAxisLabelSTransform(raxis_tr, h2t_r)
         self._tlabel_c_transform = TernaryAxisLabelCTransform(taxis_tr, h2t_t)
         self._llabel_c_transform = TernaryAxisLabelCTransform(laxis_tr, h2t_l)
         self._rlabel_c_transform = TernaryAxisLabelCTransform(raxis_tr, h2t_r)
 
         # From ternary coordinates to the original data coordinates
-        self.transProjection = BarycentricTransform(self.corners_data)
+        self.transProjection = \
+            self.transTernaryScale + BarycentricTransform(self.corners_data)
 
         # From ternary coordinates to the original Axes coordinates
         self._ternary_axes_transform = self.transProjection + self.transLimits
 
         # From ternary coordinates to display coordinates
         self._ternary2display_transform = self.transProjection + self.transData
 
@@ -287,24 +292,24 @@
         """Return the RAxis instance"""
         return self.raxis
 
     def clear(self):
         self.viewTLim.intervalx = 0.0, self.ternary_sum
         self.viewLLim.intervalx = 0.0, self.ternary_sum
         self.viewRLim.intervalx = 0.0, self.ternary_sum
-        if tuple(int(_) for _ in mpl.__version__.split('.'))[:2] < (3, 6):
+        if tuple(int(_) for _ in mpl.__version__.split('.')[:2]) < (3, 6):
             super().cla()
         else:
             super().clear()
         xmin = -1.0 / np.sqrt(3.0)
         xmax = +1.0 / np.sqrt(3.0)
         self.set_xlim(xmin, xmax)
         self.set_ylim(0.0, 1.0)
 
-    if tuple(int(_) for _ in mpl.__version__.split('.'))[:2] < (3, 6):
+    if tuple(int(_) for _ in mpl.__version__.split('.')[:2]) < (3, 6):
         cla = clear
 
     def autoscale_view(self, *args, **kwargs):
         pass
 
     def _update_title_position(self, renderer):
         """
```

### Comparing `mpltern-1.0.3/mpltern/ternary/axis.py` & `mpltern-1.0.4/mpltern/ternary/axis.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern/ternary/spines.py` & `mpltern-1.0.4/mpltern/ternary/spines.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,17 @@
             low, high = self.axes.get_tlim()
         elif self.spine_type in ["lside", "lcorner"]:
             low, high = self.axes.get_llim()
         elif self.spine_type in ["rside", "rcorner"]:
             low, high = self.axes.get_rlim()
 
         if self.spine_type in ["tside", "lside", "rside"]:
-            self._path.vertices = [[low, 0.0], [low, 1.0]]
+            self._path.vertices[:, 0] = low
         elif self.spine_type in ["tcorner", "lcorner", "rcorner"]:
-            self._path.vertices = [[high, 0.0], [high, 1.0]]
+            self._path.vertices[:, 0] = high
 
     def get_spine_transform(self):
         return self.get_transform()
 
     @classmethod
     def linear_spine(cls, axes, spine_type, **kwargs):
         """Create and return a linear `Spine`."""
```

### Comparing `mpltern-1.0.3/mpltern/ternary/tick.py` & `mpltern-1.0.4/mpltern/ternary/tick.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern/ternary/transforms.py` & `mpltern-1.0.4/mpltern/ternary/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,52 @@
 values are forced to be the same as ``input_dims``.
 """
 import numpy as np
 
 from matplotlib.transforms import Affine2DBase, Transform
 
 
+class TernaryLinearTransform(Transform):
+    """Transform to modify ternary coordinates.
+
+    Its inverse is particularly important to get back the original ternary
+    coordinates from barycentric coordinates.
+
+    Parameters
+    ----------
+    ternary_sum : float
+        Value by which ternary coordinates are divided to be suitable for the
+        input to BarycentricTransform.
+    """
+    input_dims = output_dims = 3
+    has_inverse = True
+
+    def __init__(self, ternary_sum: float, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.ternary_sum = ternary_sum
+
+    def transform_non_affine(self, values):
+        """Transform ternary coordinates.
+
+        Parameters
+        ----------
+        values : (N, 3) array_like
+            Ternary coordinates before division.
+
+        Returns
+        -------
+        (N, 3) np.ndarray
+            Ternary coordinates after division.
+        """
+        return values / self.ternary_sum
+
+    def inverted(self):
+        return TernaryLinearTransform(1.0 / self.ternary_sum)
+
+
 class TernaryAxisTransform(Transform):
     """Transform convenient for ticks in TernaryAxis.
 
     Parameters
     ----------
     corners : (3, 2) array_like
         Corners of the triangle in Cartesian coordinates.
@@ -245,17 +283,15 @@
         values : (N, 3) array_like
             Points in the barycentric coordinates.
 
         Returns
         -------
         (x, y) : Cartesian coordinates
         """
-        values = np.asarray(values, float)
-        values /= np.sum(values, axis=1)[:, np.newaxis]
-        return np.dot(values, self.corners)
+        return (values / np.sum(values, axis=1)[:, None]) @ self.corners
 
     def inverted(self):
         return InvertedBarycentricTransform(self.corners)
 
 
 class InvertedBarycentricTransform(Transform):
     input_dims = 2
```

### Comparing `mpltern-1.0.3/mpltern/tribin_helpers.py` & `mpltern-1.0.4/mpltern/tribin_helpers.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/mpltern.egg-info/PKG-INFO` & `mpltern-1.0.4/mpltern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltern
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ternary plots as projections of Matplotlib
 Home-page: https://github.com/yuzie007/mpltern
 Author: Yuji Ikeda
 Author-email: yuji.ikeda.ac.jp@gmail.com
 Project-URL: Bug Reports, https://github.com/yuzie007/mpltern/issues
 Project-URL: Source, https://github.com/yuzie007/mpltern
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mpltern-1.0.3/mpltern.egg-info/SOURCES.txt` & `mpltern-1.0.4/mpltern.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 docsrc/sphinxext/__init__.py
 docsrc/sphinxext/custom_roles.py
 docsrc/users/index.rst
 docsrc/users/mpltern_1.0.0.rst
 docsrc/users/mpltern_1.0.1.rst
 docsrc/users/mpltern_1.0.2.rst
 docsrc/users/mpltern_1.0.3.rst
+docsrc/users/mpltern_1.0.4.rst
 docsrc/users/release_notes.rst
 examples/README.rst
 examples/axis_and_tick/00.axis_label_position.py
 examples/axis_and_tick/01.axis_label_rotation.py
 examples/axis_and_tick/10.tick_position.py
 examples/axis_and_tick/11.tick_direction.py
 examples/axis_and_tick/12.tick_rotation.py
@@ -164,17 +165,20 @@
 tests/baseline_images/test_ternary/arguments_6.pdf
 tests/baseline_images/test_ternary/arguments_7.pdf
 tests/baseline_images/test_ternary/arrow_axes.pdf
 tests/baseline_images/test_ternary/arrow_data.pdf
 tests/baseline_images/test_ternary/arrow_xy_axes.pdf
 tests/baseline_images/test_ternary/arrow_xy_data.pdf
 tests/baseline_images/test_ternary/aspect.pdf
-tests/baseline_images/test_ternary/axis_label_position_corner.pdf
-tests/baseline_images/test_ternary/axis_label_position_tick1.pdf
-tests/baseline_images/test_ternary/axis_label_position_tick2.pdf
+tests/baseline_images/test_ternary/axis_label_corner_axis.pdf
+tests/baseline_images/test_ternary/axis_label_corner_horizontal.pdf
+tests/baseline_images/test_ternary/axis_label_tick1_axis.pdf
+tests/baseline_images/test_ternary/axis_label_tick1_horizontal.pdf
+tests/baseline_images/test_ternary/axis_label_tick2_axis.pdf
+tests/baseline_images/test_ternary/axis_label_tick2_horizontal.pdf
 tests/baseline_images/test_ternary/fit_none.pdf
 tests/baseline_images/test_ternary/fit_rectangle.pdf
 tests/baseline_images/test_ternary/fit_triangle.pdf
 tests/baseline_images/test_ternary/legend.pdf
 tests/baseline_images/test_ternary/manual_ticklabels.pdf
 tests/baseline_images/test_ternary/manual_ticks.pdf
 tests/baseline_images/test_ternary/negative_ticks.pdf
```

### Comparing `mpltern-1.0.3/setup.py` & `mpltern-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/Dirichlet_PDF_1.0_2.0_2.0.txt` & `mpltern-1.0.4/tests/Dirichlet_PDF_1.0_2.0_2.0.txt`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/Dirichlet_PDF_1.5_1.5_1.5.txt` & `mpltern-1.0.4/tests/Dirichlet_PDF_1.5_1.5_1.5.txt`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/Dirichlet_PDF_2.0_4.0_8.0.txt` & `mpltern-1.0.4/tests/Dirichlet_PDF_2.0_4.0_8.0.txt`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/Dirichlet_PDF_5.0_5.0_5.0.txt` & `mpltern-1.0.4/tests/Dirichlet_PDF_5.0_5.0_5.0.txt`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf` & `mpltern-1.0.4/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_hexbin/base.pdf` & `mpltern-1.0.4/tests/baseline_images/test_hexbin/base.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_hexbin/extent.pdf` & `mpltern-1.0.4/tests/baseline_images/test_hexbin/extent.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_hexbin/given_triangles.pdf` & `mpltern-1.0.4/tests/baseline_images/test_hexbin/given_triangles.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_hexbin/ternary_lim.pdf` & `mpltern-1.0.4/tests/baseline_images/test_hexbin/ternary_lim.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/arguments_6.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/arguments_6.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/arguments_7.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/arguments_7.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_axes.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_axes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_data.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_data.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_xy_axes.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_xy_axes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/arrow_xy_data.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/arrow_xy_data.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/aspect.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/aspect.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/axis_label_position_corner.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_corner_axis.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/axis_label_position_tick1.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_tick1_axis.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/axis_label_position_tick2.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/axis_label_tick2_axis.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/fit_none.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/fit_none.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/fit_rectangle.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/fit_rectangle.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/fit_triangle.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/fit_triangle.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/legend.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/legend.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/manual_ticklabels.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/manual_ticklabels.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/manual_ticks.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/manual_ticks.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/negative_ticks.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/negative_ticks.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/opposite_ticks.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/opposite_ticks.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/plot.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/plot.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/quiver.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/quiver.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/quiver_color.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/quiver_color.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/quiver_xy_axes.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/quiver_xy_axes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/quiver_xy_data.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/quiver_xy_data.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/scatter.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/scatter.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/scatter_color.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/scatter_color.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/spans.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/spans.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected.png` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected.png`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim.png` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim.png`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim.svg` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim.svg`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/test_ternary_lim_svg.png` & `mpltern-1.0.4/tests/baseline_images/test_ternary/test_ternary_lim_svg.png`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/text.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/text.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/tick_direction_in.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/tick_direction_in.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/tick_direction_inout.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/tick_direction_inout.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/tick_direction_out.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/tick_direction_out.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/titie_center.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/titie_center.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/titie_left.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/titie_left.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/titie_right.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/titie_right.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_ternary/transAxes.pdf` & `mpltern-1.0.4/tests/baseline_images/test_ternary/transAxes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_tightlayout/tight_layout1.pdf` & `mpltern-1.0.4/tests/baseline_images/test_tightlayout/tight_layout1.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf` & `mpltern-1.0.4/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_tribin/base.pdf` & `mpltern-1.0.4/tests/baseline_images/test_tribin/base.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_tribin/extent.pdf` & `mpltern-1.0.4/tests/baseline_images/test_tribin/extent.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_tribin/given_triangles.pdf` & `mpltern-1.0.4/tests/baseline_images/test_tribin/given_triangles.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/baseline_images/test_tribin/ternary_lim.pdf` & `mpltern-1.0.4/tests/baseline_images/test_tribin/ternary_lim.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/hexbin_indices.txt` & `mpltern-1.0.4/tests/hexbin_indices.txt`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_axis.py` & `mpltern-1.0.4/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_datasets.py` & `mpltern-1.0.4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_given_triangles.py` & `mpltern-1.0.4/tests/test_given_triangles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-import numpy as np
+"""Tests for custom triangles."""
+from itertools import product
 
+import matplotlib.pyplot as plt
 import pytest
-from itertools import product
 from matplotlib.testing.decorators import image_comparison
-import matplotlib.pyplot as plt
+
 from mpltern.datasets import get_spiral
 
 
 class TestGivenTriangles:
+    """Tests for custom triangles."""
     labelrotations = ["tick", "axis", "horizontal"]
     rotations = range(0, 360, 90)
     expected = [
         (lr, r, [f"given_triangles_{lr}_{r}"])
         for lr, r in product(labelrotations, rotations)
     ]
 
-    @pytest.mark.parametrize("labelrotation, rotation, baseline_images", expected)
+    @pytest.mark.parametrize(
+        "labelrotation, rotation, baseline_images",
+        expected,
+    )
     @image_comparison(baseline_images=None, extensions=["pdf"], style="mpl20")
     def test_given_triangles(self, labelrotation, rotation, baseline_images):
-        # Check if the tick-markers, tick-labels, and axis-labels are shown as
-        # expected.
+        """Test custom triangles.
+
+        Test if tick-markers, tick-labels, and axis-labels are shown as
+        expected for custom triangles.
+        """
         if "text.kerning_factor" in plt.rcParams:
             plt.rcParams["text.kerning_factor"] = 6
 
         corners = ((0.5, 0.0), (1.0, 0.5), (0.0, 1.0))
-        ax = plt.subplot(projection="ternary", corners=corners, rotation=rotation)
-        t, l, r = get_spiral()
-        ax.plot(t, l, r)
+        ax = plt.subplot(
+            projection="ternary",
+            corners=corners,
+            rotation=rotation,
+        )
+        tn0, tn1, tn2 = get_spiral()
+        ax.plot(tn0, tn1, tn2)
 
         ax.set_tlabel("Top")
         ax.set_llabel("Left")
         ax.set_rlabel("Right")
 
         ax.tick_params(labelrotation=labelrotation)
```

### Comparing `mpltern-1.0.3/tests/test_hexbin.py` & `mpltern-1.0.4/tests/test_hexbin.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,7 +105,22 @@
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
 
     ax = fig_test.add_subplot(projection="ternary")
     ax.hexbin(t, l, r, bins="log")
 
     ax = fig_ref.add_subplot(projection="ternary")
     ax.hexbin(t, l, r, norm=LogNorm())
+
+
+def test_ndarray_cast():
+    """Test if non-float ndarray can be passed without errors.
+
+    https://github.com/yuzie007/mpltern/issues/15
+    https://numpy.org/doc/stable/reference/arrays.dtypes.html
+    """
+    tn0 = np.array((1,), dtype='>u2')
+    tn1 = np.array((0,), dtype='>u2')
+    tn2 = np.array((0,), dtype='>u2')
+
+    fig = plt.figure()
+    ax = fig.add_subplot(projection="ternary")
+    ax.hexbin(tn0, tn1, tn2, gridsize=10, edgecolors="none")
```

### Comparing `mpltern-1.0.3/tests/test_hexbin_helpers.py` & `mpltern-1.0.4/tests/test_hexbin_helpers.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_ternary.py` & `mpltern-1.0.4/tests/test_ternary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import itertools
 
 import numpy as np
 
 import pytest
 import matplotlib as mpl
 from matplotlib.testing.decorators import (
     image_comparison, check_figures_equal)
@@ -116,35 +117,44 @@
     def test_tranform_1(self):
         """Test if `plot` recognizes and handle `ax.transAxes` as expected."""
         fig_test = plt.figure()
         ax = fig_test.add_subplot(111, projection='ternary')
         ax.plot([0, 1], [0, 1], transform=ax.transAxes)
 
 
-class TestAxisLabelPosition:
+class TestAxisLabel:
+    """Test for axis-label position and rotation."""
     positions = ['corner', 'tick1', 'tick2']
-    baseline_images_list = [[f'axis_label_position_{p}'] for p in positions]
+    rotations = ['axis', 'horizontal']
+    expected = [
+        (p, r, [f'axis_label_{p}_{r}'])
+        for p, r in itertools.product(positions, rotations)
+    ]
 
-    @pytest.mark.parametrize('position, baseline_images',
-                             zip(positions, baseline_images_list))
+    @pytest.mark.parametrize('position, rotation, baseline_images', expected)
     @image_comparison(baseline_images=None, extensions=['pdf'], style='mpl20')
-    def test_axis_label_position(self, position, baseline_images):
+    def test_axis_label(self, position, rotation, baseline_images):
+        """Test axis-label position and rotation."""
         fix_text_kerning_factor()
 
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
 
         ax.set_tlabel('Top')
         ax.set_llabel('Left')
         ax.set_rlabel('Right')
 
         ax.taxis.set_label_position(position)
         ax.laxis.set_label_position(position)
         ax.raxis.set_label_position(position)
 
+        ax.taxis.set_label_rotation_mode(rotation)
+        ax.laxis.set_label_rotation_mode(rotation)
+        ax.raxis.set_label_rotation_mode(rotation)
+
 
 class TestTitle:
     locs = ['center', 'left', 'right']
     baseline_images_list = [[f'titie_{loc}'] for loc in locs]
 
     @pytest.mark.parametrize('loc, baseline_images',
                              zip(locs, baseline_images_list),)
@@ -807,33 +817,35 @@
 
     for seed in [1, 9, 6, 8]:
         ax.scatter(*get_scatter_points(11, seed=seed), alpha=0.5, label=seed)
 
     ax.legend()
 
 
+@pytest.mark.parametrize('ternary_sum', (1.0, 2.0, -1.0, -2.0))
 @check_figures_equal(extensions=('pdf',))
-def test_set_view(fig_test, fig_ref):
+def test_set_view(fig_test, fig_ref, ternary_sum: float):
     """Test if `_set_view` works correctly."""
     tn0, tn1, tn2 = get_spiral()
 
-    ax = fig_test.add_subplot(projection='ternary')
+    ax = fig_test.add_subplot(projection='ternary', ternary_sum=ternary_sum)
     ax.plot(tn0, tn1, tn2)
     xmin = -0.6 / np.sqrt(3.0)
     xmax = +1.4 / np.sqrt(3.0)
     ymin = 0.0
     ymax = 1.0
-    if tuple(int(_) for _ in mpl.__version__.split('.'))[:2] < (3, 8):
+    if tuple(int(_) for _ in mpl.__version__.split('.')[:2]) < (3, 8):
         ax._set_view((xmin, xmax, ymin, ymax))
     else:
         ax._set_view({"xlim": (xmin, xmax), "ylim": (ymin, ymax)})
 
-    ax = fig_ref.add_subplot(projection='ternary')
+    ax = fig_ref.add_subplot(projection='ternary', ternary_sum=ternary_sum)
     ax.plot(tn0, tn1, tn2)
-    ax.set_ternary_lim(0.0, 1.0, -0.2, 0.8, 0.2, 1.2)
+    ternary_lim = ternary_sum * np.array((0.0, 1.0, -0.2, 0.8, 0.2, 1.2))
+    ax.set_ternary_lim(*ternary_lim)
 
 
 class TestSignature:
     """Test signatures of methods."""
     methods = [
         "text",
         "plot",
```

### Comparing `mpltern-1.0.3/tests/test_text.py` & `mpltern-1.0.4/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_tick.py` & `mpltern-1.0.4/tests/test_tick.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_transforms.py` & `mpltern-1.0.4/tests/test_transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Test transforms for ternary plots."""
 import numpy as np
 import pytest
 
 from matplotlib.transforms import Bbox, IdentityTransform
-from mpltern.ternary.transforms import (BarycentricTransform,
-                                        T2HHeightTransform,
-                                        T2HWidthTransform,
-                                        TernaryAxisLabelSTransform,
-                                        TernaryAxisLabelCTransform,
-                                        TernaryAxisTransform)
+from mpltern.ternary.transforms import (
+    BarycentricTransform,
+    InvertedBarycentricTransform,
+    InvertedTernaryAxisTransform,
+    T2HHeightTransform,
+    T2HWidthTransform,
+    TernaryAxisLabelSTransform,
+    TernaryAxisLabelCTransform,
+    TernaryAxisTransform,
+    TernaryLinearTransform,
+)
 
 corners_list = [
     ((0.5, 0.0), (1.0, 0.5), (0.0, 1.0)),
     ((0.0, 0.0), (1.0, 0.0), (0.5, 1.0)),
 ]
 
 
@@ -29,14 +34,29 @@
     points_inverted = trans.inverted().transform(points_transformed)
 
     np.testing.assert_almost_equal(points_inverted, points)
 
 
 @pytest.mark.parametrize("corners", corners_list)
 @pytest.mark.parametrize("index", [0, 1, 2])
+def test_inverted_ternary_transform(corners, index):
+    """Test InvertedTernaryTransform."""
+    np.random.seed(1986)
+    points = np.random.rand(300).reshape(-1, 2)
+    points /= np.sum(points, axis=1)[:, None]
+
+    trans = InvertedTernaryAxisTransform(corners, index)
+    points_transformed = trans.transform(points)
+    points_inverted = trans.inverted().transform(points_transformed)
+
+    np.testing.assert_almost_equal(points_inverted, points)
+
+
+@pytest.mark.parametrize("corners", corners_list)
+@pytest.mark.parametrize("index", [0, 1, 2])
 def test_label_s_transform(corners, index):
     """Test TernaryPerpendicularTransform."""
     np.random.seed(1986)
     points = np.random.rand(300).reshape(-1, 2)
     points /= np.sum(points, axis=1)[:, None]
 
     trans = TernaryAxisLabelSTransform(TernaryAxisTransform(corners, index), IdentityTransform())
@@ -101,20 +121,47 @@
     trans = T2HWidthTransform(scale, [viewTLim, viewLLim, viewRLim], index)
     points_transformed = trans.transform(points)
     points_inverted = trans.inverted().transform(points_transformed)
 
     np.testing.assert_almost_equal(points_inverted, points)
 
 
-@pytest.mark.parametrize("scale", [1.0, 2.0, -1.0, -2.0])
+@pytest.mark.parametrize('ternary_sum', (1.0, 2.0, -1.0, -2.0))
+def test_ternary_linear_transform(ternary_sum: float):
+    """Test TernaryLinearTransform."""
+    np.random.seed(1986)
+    points = np.random.rand(300).reshape(-1, 3)
+    points *= ternary_sum / np.sum(points, axis=1)[:, None]
+
+    trans = TernaryLinearTransform(ternary_sum)
+    points_transformed = trans.transform(points)
+    points_inverted = trans.inverted().transform(points_transformed)
+
+    np.testing.assert_almost_equal(points_transformed.sum(axis=1), 1.0)
+    np.testing.assert_almost_equal(points_inverted, points)
+
+
 @pytest.mark.parametrize("corners", corners_list)
-def test_barycentric_transform(scale, corners):
+def test_barycentric_transform(corners):
     """Test BarycentricTransform."""
     np.random.seed(1986)
     points = np.random.rand(300).reshape(-1, 3)
-    points *= scale / np.sum(points, axis=1)[:, None]
+    points /= np.sum(points, axis=1)[:, None]  # normalized
 
     trans = BarycentricTransform(corners)
     points_transformed = trans.transform(points)
     points_inverted = trans.inverted().transform(points_transformed)
 
     np.testing.assert_almost_equal(points_inverted, points)
+
+
+@pytest.mark.parametrize("corners", corners_list)
+def test_inverted_barycentric_transform(corners):
+    """Test InvertedBarycentricTransform."""
+    np.random.seed(1986)
+    points = np.random.rand(300).reshape(-1, 2)
+
+    trans = InvertedBarycentricTransform(corners)
+    points_transformed = trans.transform(points)
+    points_inverted = trans.inverted().transform(points_transformed)
+
+    np.testing.assert_almost_equal(points_inverted, points)
```

### Comparing `mpltern-1.0.3/tests/test_triangle_rotation_axis.py` & `mpltern-1.0.4/tests/test_triangle_rotation_axis.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_triangle_rotation_horizontal.py` & `mpltern-1.0.4/tests/test_triangle_rotation_horizontal.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_triangle_rotation_tick.py` & `mpltern-1.0.4/tests/test_triangle_rotation_tick.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/test_tribin_helpers.py` & `mpltern-1.0.4/tests/test_tribin_helpers.py`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tests/tribin_indices.txt` & `mpltern-1.0.4/tests/tribin_indices.txt`

 * *Files identical despite different names*

### Comparing `mpltern-1.0.3/tox.ini` & `mpltern-1.0.4/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # content of: tox.ini , put in same dir as setup.py
 [tox]
-envlist = py310-matplotlib{340,350,360,370}
+envlist = py311-matplotlib{340,350,360,370,380}
 
 [testenv]
 install_command =
     python -I -m pip install --use-pep517
 # install pytest in the virtualenv where commands will be executed
 deps =
     pytest
     setuptools<60
     pillow==9.0
     matplotlib340: matplotlib==3.4.0
     matplotlib350: matplotlib==3.5.0
     matplotlib360: matplotlib==3.6.0
     matplotlib370: matplotlib==3.7.0
-    matplotlib370: matplotlib==3.8.0
+    matplotlib380: matplotlib==3.8.0
 setenv =
     PYTHONPATH=
 commands =
     # NOTE: you can run any command line tool here - not just tests
     pytest {posargs}
```

