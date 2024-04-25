# Comparing `tmp/superqt-0.6.2.tar.gz` & `tmp/superqt-0.6.3.tar.gz`

## Comparing `superqt-0.6.2.tar` & `superqt-0.6.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0    22819 2020-02-02 00:00:00.000000 superqt-0.6.2/CHANGELOG.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/py.typed
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/cmap/__init__.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/cmap/_catalog_combo.py
--rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/cmap/_cmap_combo.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/cmap/_cmap_item_delegate.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/cmap/_cmap_line_edit.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/cmap/_cmap_utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/collapsible/__init__.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/collapsible/_collapsible.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/combobox/__init__.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/combobox/_color_combobox.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/combobox/_enum_combobox.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/combobox/_searchable_combo_box.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/elidable/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/elidable/_eliding.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/elidable/_eliding_label.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/elidable/_eliding_line_edit.py
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/fonticon/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/fonticon/_animations.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/fonticon/_iconfont.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/fonticon/_plugins.py
--rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/fonticon/_qfont_icon.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/iconify/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/qtcompat/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/selection/__init__.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/selection/_searchable_list_widget.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/selection/_searchable_tree_widget.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/sliders/__init__.py
--rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/sliders/_generic_range_slider.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/sliders/_generic_slider.py
--rw-r--r--   0        0        0    23298 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/sliders/_labeled.py
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/sliders/_range_style.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/sliders/_sliders.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/spinbox/__init__.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/spinbox/_intspin.py
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/spinbox/_quantity.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/__init__.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_code_syntax_highlight.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_ensure_thread.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_errormsg_context.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_img_utils.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_message_handler.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_misc.py
--rw-r--r--   0        0        0    30760 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_qthreading.py
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_throttler.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.2/src/superqt/utils/_util.py
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_cmap.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_code_highlight.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_collapsible.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_color_combo.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_eliding_label.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_eliding_line_edit.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_ensure_thread.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_enum_comb_box.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_iconify.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_large_int_spinbox.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_qmessage_handler.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_quantity.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_searchable_combobox.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_searchable_list.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_searchable_tree.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_threadworker.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_throttler.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_utils.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/test_fonticon.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/test_plugins.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/fixtures/fake_plugin/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/__init__.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/_testutil.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/test_float.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/test_generic_slider.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/test_labeled_slider.py
--rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/test_range_slider.py
--rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/test_single_value_sliders.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.6.2/tests/zz_test_sliders/test_slider.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.6.2/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.6.2/LICENSE
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.6.2/README.md
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 superqt-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 superqt-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 superqt-0.6.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/py.typed
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/cmap/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/cmap/_catalog_combo.py
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/cmap/_cmap_combo.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/cmap/_cmap_item_delegate.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/cmap/_cmap_line_edit.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/cmap/_cmap_utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/collapsible/__init__.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/collapsible/_collapsible.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/combobox/__init__.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/combobox/_color_combobox.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/combobox/_enum_combobox.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/combobox/_searchable_combo_box.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/elidable/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/elidable/_eliding.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/elidable/_eliding_label.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/elidable/_eliding_line_edit.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/fonticon/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/fonticon/_animations.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/fonticon/_iconfont.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/fonticon/_plugins.py
+-rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/fonticon/_qfont_icon.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/iconify/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/qtcompat/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/selection/__init__.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/selection/_searchable_list_widget.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/selection/_searchable_tree_widget.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/sliders/__init__.py
+-rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/sliders/_generic_range_slider.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/sliders/_generic_slider.py
+-rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/sliders/_labeled.py
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/sliders/_range_style.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/sliders/_sliders.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/spinbox/__init__.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/spinbox/_intspin.py
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/spinbox/_quantity.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/__init__.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_code_syntax_highlight.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_ensure_thread.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_errormsg_context.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_img_utils.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_message_handler.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_misc.py
+-rw-r--r--   0        0        0    30760 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_qthreading.py
+-rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_throttler.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.3/src/superqt/utils/_util.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_cmap.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_code_highlight.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_collapsible.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_color_combo.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_eliding_label.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_eliding_line_edit.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_ensure_thread.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_enum_comb_box.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_iconify.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_large_int_spinbox.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_qmessage_handler.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_quantity.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_searchable_combobox.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_searchable_list.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_searchable_tree.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_threadworker.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_throttler.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_utils.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/test_fonticon.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/test_plugins.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/fixtures/fake_plugin/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/__init__.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/_testutil.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/test_float.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/test_generic_slider.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/test_labeled_slider.py
+-rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/test_range_slider.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/test_single_value_sliders.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.6.3/tests/zz_test_sliders/test_slider.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.6.3/README.md
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 superqt-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 superqt-0.6.3/PKG-INFO
```

### Comparing `superqt-0.6.2/CHANGELOG.md` & `superqt-0.6.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [v0.6.3](https://github.com/pyapp-kit/superqt/tree/v0.6.3) (2024-03-27)
+
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.6.2...v0.6.3)
+
+**Fixed bugs:**
+
+- fix: fix sliderReleased, sliderPressed signals, and setTracking [\#237](https://github.com/pyapp-kit/superqt/pull/237) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- ci\(dependabot\): bump softprops/action-gh-release from 1 to 2 [\#236](https://github.com/pyapp-kit/superqt/pull/236) ([dependabot[bot]](https://github.com/apps/dependabot))
+
 ## [v0.6.2](https://github.com/pyapp-kit/superqt/tree/v0.6.2) (2024-03-06)
 
 [Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.6.1...v0.6.2)
 
 **Implemented enhancements:**
 
 - feat: make toggle button public in QCollapsible [\#232](https://github.com/pyapp-kit/superqt/pull/232) ([tlambert03](https://github.com/tlambert03))
@@ -404,21 +416,17 @@
 
 **Documentation updates:**
 
 - fix broken link [\#18](https://github.com/pyapp-kit/superqt/pull/18) ([haesleinhuepf](https://github.com/haesleinhuepf))
 
 ## [v0.2.1](https://github.com/pyapp-kit/superqt/tree/v0.2.1) (2021-07-10)
 
-[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0rc0...v0.2.1)
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0...v0.2.1)
 
 **Fixed bugs:**
 
 - Fix QLabeledRangeSlider API \(fix slider proxy\) [\#10](https://github.com/pyapp-kit/superqt/pull/10) ([tlambert03](https://github.com/tlambert03))
 - Fix range slider with negative min range [\#9](https://github.com/pyapp-kit/superqt/pull/9) ([tlambert03](https://github.com/tlambert03))
 
-## [v0.2.0rc0](https://github.com/pyapp-kit/superqt/tree/v0.2.0rc0) (2021-06-26)
-
-[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0...v0.2.0rc0)
-
 
 
 \* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
```

### Comparing `superqt-0.6.2/src/superqt/__init__.py` & `superqt-0.6.3/src/superqt/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/cmap/__init__.py` & `superqt-0.6.3/src/superqt/cmap/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/cmap/_catalog_combo.py` & `superqt-0.6.3/src/superqt/cmap/_catalog_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/cmap/_cmap_combo.py` & `superqt-0.6.3/src/superqt/cmap/_cmap_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/cmap/_cmap_item_delegate.py` & `superqt-0.6.3/src/superqt/cmap/_cmap_item_delegate.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/cmap/_cmap_line_edit.py` & `superqt-0.6.3/src/superqt/cmap/_cmap_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/cmap/_cmap_utils.py` & `superqt-0.6.3/src/superqt/cmap/_cmap_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/collapsible/_collapsible.py` & `superqt-0.6.3/src/superqt/collapsible/_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/combobox/__init__.py` & `superqt-0.6.3/src/superqt/combobox/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/combobox/_color_combobox.py` & `superqt-0.6.3/src/superqt/combobox/_color_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/combobox/_enum_combobox.py` & `superqt-0.6.3/src/superqt/combobox/_enum_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/combobox/_searchable_combo_box.py` & `superqt-0.6.3/src/superqt/combobox/_searchable_combo_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/elidable/_eliding.py` & `superqt-0.6.3/src/superqt/elidable/_eliding.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/elidable/_eliding_label.py` & `superqt-0.6.3/src/superqt/elidable/_eliding_label.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/elidable/_eliding_line_edit.py` & `superqt-0.6.3/src/superqt/elidable/_eliding_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/fonticon/__init__.py` & `superqt-0.6.3/src/superqt/fonticon/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/fonticon/_animations.py` & `superqt-0.6.3/src/superqt/fonticon/_animations.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/fonticon/_iconfont.py` & `superqt-0.6.3/src/superqt/fonticon/_iconfont.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/fonticon/_plugins.py` & `superqt-0.6.3/src/superqt/fonticon/_plugins.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/fonticon/_qfont_icon.py` & `superqt-0.6.3/src/superqt/fonticon/_qfont_icon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/iconify/__init__.py` & `superqt-0.6.3/src/superqt/iconify/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/qtcompat/__init__.py` & `superqt-0.6.3/src/superqt/qtcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/selection/_searchable_list_widget.py` & `superqt-0.6.3/src/superqt/selection/_searchable_list_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/selection/_searchable_tree_widget.py` & `superqt-0.6.3/src/superqt/selection/_searchable_tree_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/sliders/_generic_range_slider.py` & `superqt-0.6.3/src/superqt/sliders/_generic_range_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/sliders/_generic_slider.py` & `superqt-0.6.3/src/superqt/sliders/_generic_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/sliders/_labeled.py` & `superqt-0.6.3/src/superqt/sliders/_labeled.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,44 @@
 
     def tickPosition(self) -> QSlider.TickPosition:
         return self._slider.tickPosition()
 
     def setTickPosition(self, pos: QSlider.TickPosition) -> None:
         self._slider.setTickPosition(pos)
 
+    def triggerAction(self, action: QAbstractSlider.SliderAction) -> None:
+        return self._slider.triggerAction(action)
+
+    def invertedControls(self) -> bool:
+        return self._slider.invertedControls()
+
+    def setInvertedControls(self, a0: bool) -> None:
+        return self._slider.setInvertedControls(a0)
+
+    def invertedAppearance(self) -> bool:
+        return self._slider.invertedAppearance()
+
+    def setInvertedAppearance(self, a0: bool) -> None:
+        return self._slider.setInvertedAppearance(a0)
+
+    def isSliderDown(self) -> bool:
+        return self._slider.isSliderDown()
+
+    def setSliderDown(self, a0: bool) -> None:
+        return self._slider.setSliderDown(a0)
+
+    def hasTracking(self) -> bool:
+        return self._slider.hasTracking()
+
+    def setTracking(self, enable: bool) -> None:
+        return self._slider.setTracking(enable)
+
+    def orientation(self) -> Qt.Orientation:
+        return self._slider.orientation()
+
     def __getattr__(self, name: Any) -> Any:
         return getattr(self._slider, name)
 
 
 def _handle_overloaded_slider_sig(
     args: tuple, kwargs: dict
 ) -> tuple[QWidget | None, Qt.Orientation]:
@@ -286,14 +316,16 @@
 
     def setDecimals(self, prec: int) -> None:
         self._label.setDecimals(prec)
 
 
 class QLabeledRangeSlider(_SliderProxy, QAbstractSlider):
     _valueChanged = Signal(tuple)
+    _sliderPressed = Signal()
+    _sliderReleased = Signal()
     editingFinished = Signal()
 
     _slider_class = QRangeSlider
     _slider: QRangeSlider
 
     @overload
     def __init__(self, parent: QWidget | None = ...) -> None: ...
@@ -314,14 +346,16 @@
 
         # for fine tuning label position
         self.label_shift_x = 0
         self.label_shift_y = 0
 
         self._slider = self._slider_class()
         self._slider.valueChanged.connect(self.valueChanged.emit)
+        self._slider.sliderPressed.connect(self.sliderPressed.emit)
+        self._slider.sliderReleased.connect(self.sliderReleased.emit)
         self._slider.rangeChanged.connect(self.rangeChanged.emit)
         self.sliderMoved = self._slider._slidersMoved
 
         self._min_label = SliderLabel(
             self._slider,
             alignment=Qt.AlignmentFlag.AlignLeft,
             connect=self._min_label_edited,
@@ -435,14 +469,16 @@
     # putting this after methods above for the sake of mypy
     LabelPosition = LabelPosition
     EdgeLabelMode = EdgeLabelMode
 
     # ------------- private methods ----------------
     def _rename_signals(self) -> None:
         self.valueChanged = self._valueChanged
+        self.sliderReleased = self._sliderReleased
+        self.sliderPressed = self._sliderPressed
 
     def _reposition_labels(self) -> None:
         if (
             not self._handle_labels
             or self._handle_label_position == LabelPosition.NoLabel
         ):
             return
```

### Comparing `superqt-0.6.2/src/superqt/sliders/_range_style.py` & `superqt-0.6.3/src/superqt/sliders/_range_style.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/sliders/_sliders.py` & `superqt-0.6.3/src/superqt/sliders/_sliders.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/spinbox/_intspin.py` & `superqt-0.6.3/src/superqt/spinbox/_intspin.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/spinbox/_quantity.py` & `superqt-0.6.3/src/superqt/spinbox/_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/__init__.py` & `superqt-0.6.3/src/superqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_code_syntax_highlight.py` & `superqt-0.6.3/src/superqt/utils/_code_syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_ensure_thread.py` & `superqt-0.6.3/src/superqt/utils/_ensure_thread.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_errormsg_context.py` & `superqt-0.6.3/src/superqt/utils/_errormsg_context.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_img_utils.py` & `superqt-0.6.3/src/superqt/utils/_img_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_message_handler.py` & `superqt-0.6.3/src/superqt/utils/_message_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_misc.py` & `superqt-0.6.3/src/superqt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_qthreading.py` & `superqt-0.6.3/src/superqt/utils/_qthreading.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_throttler.py` & `superqt-0.6.3/src/superqt/utils/_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/src/superqt/utils/_util.py` & `superqt-0.6.3/src/superqt/utils/_util.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_cmap.py` & `superqt-0.6.3/tests/test_cmap.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_code_highlight.py` & `superqt-0.6.3/tests/test_code_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_collapsible.py` & `superqt-0.6.3/tests/test_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_color_combo.py` & `superqt-0.6.3/tests/test_color_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_eliding_label.py` & `superqt-0.6.3/tests/test_eliding_label.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_eliding_line_edit.py` & `superqt-0.6.3/tests/test_eliding_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_ensure_thread.py` & `superqt-0.6.3/tests/test_ensure_thread.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_enum_comb_box.py` & `superqt-0.6.3/tests/test_enum_comb_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_iconify.py` & `superqt-0.6.3/tests/test_iconify.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_large_int_spinbox.py` & `superqt-0.6.3/tests/test_large_int_spinbox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_qmessage_handler.py` & `superqt-0.6.3/tests/test_qmessage_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_quantity.py` & `superqt-0.6.3/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_searchable_combobox.py` & `superqt-0.6.3/tests/test_searchable_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_searchable_list.py` & `superqt-0.6.3/tests/test_searchable_list.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_searchable_tree.py` & `superqt-0.6.3/tests/test_searchable_tree.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_threadworker.py` & `superqt-0.6.3/tests/test_threadworker.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_throttler.py` & `superqt-0.6.3/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_utils.py` & `superqt-0.6.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_fonticon/test_fonticon.py` & `superqt-0.6.3/tests/test_fonticon/test_fonticon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_fonticon/test_plugins.py` & `superqt-0.6.3/tests/test_fonticon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf` & `superqt-0.6.3/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/_testutil.py` & `superqt-0.6.3/tests/zz_test_sliders/_testutil.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/test_float.py` & `superqt-0.6.3/tests/zz_test_sliders/test_float.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/test_generic_slider.py` & `superqt-0.6.3/tests/zz_test_sliders/test_generic_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/test_labeled_slider.py` & `superqt-0.6.3/tests/zz_test_sliders/test_labeled_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/test_range_slider.py` & `superqt-0.6.3/tests/zz_test_sliders/test_range_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/test_single_value_sliders.py` & `superqt-0.6.3/tests/zz_test_sliders/test_single_value_sliders.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/tests/zz_test_sliders/test_slider.py` & `superqt-0.6.3/tests/zz_test_sliders/test_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/.gitignore` & `superqt-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/LICENSE` & `superqt-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/README.md` & `superqt-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/pyproject.toml` & `superqt-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `superqt-0.6.2/PKG-INFO` & `superqt-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: superqt
-Version: 0.6.2
+Version: 0.6.3
 Summary: Missing widgets and components for PyQt/PySide
 Project-URL: Documentation, https://pyapp-kit.github.io/superqt/
 Project-URL: Source, https://github.com/pyapp-kit/superqt
 Project-URL: Tracker, https://github.com/pyapp-kit/superqt/issues
 Project-URL: Changelog, https://github.com/pyapp-kit/superqt/blob/main/CHANGELOG.md
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
```

