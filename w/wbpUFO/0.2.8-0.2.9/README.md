# Comparing `tmp/wbpUFO-0.2.8.tar.gz` & `tmp/wbpUFO-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpUFO-0.2.8.tar", last modified: Mon Jan 22 10:25:15 2024, max compression
+gzip compressed data, was "wbpUFO-0.2.9.tar", last modified: Fri Feb  2 16:24:52 2024, max compression
```

## Comparing `wbpUFO-0.2.8.tar` & `wbpUFO-0.2.9.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.717492 wbpUFO-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.679492 wbpUFO-0.2.8/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.683492 wbpUFO-0.2.8/Lib/wbpUFO/
--rw-rw-rw-   0 root         (0) root         (0)    10601 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.687492 wbpUFO-0.2.8/Lib/wbpUFO/control/
--rw-rw-rw-   0 root         (0) root         (0)     1290 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/dialogItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/dialogItemPickerUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/findGlyphListCtrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.688492 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24639 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)    20703 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.689492 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8756 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3465 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/font.py
--rw-rw-rw-   0 root         (0) root         (0)    28062 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)     5759 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/editPanel.py
--rw-rw-rw-   0 root         (0) root         (0)    21510 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/menu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.693492 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py
--rw-rw-rw-   0 root         (0) root         (0)    14003 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2079 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py
--rw-rw-rw-   0 root         (0) root         (0)     2953 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py
--rw-rw-rw-   0 root         (0) root         (0)    17167 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py
--rw-rw-rw-   0 root         (0) root         (0)     7101 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2756 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py
--rw-rw-rw-   0 root         (0) root         (0)     4094 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/glyphGridStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5122 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/kerningViewCanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/kerningViewPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5038 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/libControl.py
--rw-rw-rw-   0 root         (0) root         (0)     2798 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/panelItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     5686 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/control/panelItemPickerUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.699492 wbpUFO-0.2.8/Lib/wbpUFO/dialog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/anchorDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4887 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/anchorDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3351 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/assignLayerDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     6012 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/assignLayerDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/componentDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4425 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/componentDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/deleteGlyphsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     6368 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/findGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5036 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/findGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/guidelineDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5816 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/guidelineDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/layerDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2511 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/layerDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/newFontDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/newFontDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/newGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/newGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     8386 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/renameGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     9608 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/renameGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5367 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/revertFontDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7261 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/revertFontDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/selectFontsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     1967 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/dialog/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    19544 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.702492 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/
--rw-rw-rw-   0 root         (0) root         (0)     3040 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2307 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)     4530 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/base.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/commandListCtrl.py
--rw-rw-rw-   0 root         (0) root         (0)    13260 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/commandListDialog.py
--rw-rw-rw-   0 root         (0) root         (0)    12967 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/commandListDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     6822 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2070 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/guideline.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     7342 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/metric.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     5157 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/parameter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.703492 wbpUFO-0.2.8/Lib/wbpUFO/panel/
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/panel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16132 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/panel/glyphViewCanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/panel/glyphViewPanel.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/panel/glyphViewPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.704492 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/
--rw-rw-rw-   0 root         (0) root         (0)     1980 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/command.py
--rw-rw-rw-   0 root         (0) root         (0)     4790 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/editTool.py
--rw-rw-rw-   0 root         (0) root         (0)     4521 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/glyphLock.py
--rw-rw-rw-   0 root         (0) root         (0)     7625 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/glyphShow.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/toolbar/markColor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.705492 wbpUFO-0.2.8/Lib/wbpUFO/view/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.715492 wbpUFO-0.2.8/Lib/wbpUFO/view/font/
--rw-rw-rw-   0 root         (0) root         (0)     5480 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19462 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/feature.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoBase.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoCaret.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoCaretUI.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoClassification.py
--rw-rw-rw-   0 root         (0) root         (0)     4073 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoClassificationUI.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoCodepage.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoCodepageUI.py
--rw-rw-rw-   0 root         (0) root         (0)     8952 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoControl.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoEmbedding.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoEncodingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHinting.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHintingPS.py
--rw-rw-rw-   0 root         (0) root         (0)    10731 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py
--rw-rw-rw-   0 root         (0) root         (0)     6830 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHintingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoIdentification.py
--rw-rw-rw-   0 root         (0) root         (0)     6714 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoLegal.py
--rw-rw-rw-   0 root         (0) root         (0)     6955 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoLegalUI.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoLine.py
--rw-rw-rw-   0 root         (0) root         (0)     4862 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoLineUI.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoMetric.py
--rw-rw-rw-   0 root         (0) root         (0)    13226 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoMetricUI.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoName.py
--rw-rw-rw-   0 root         (0) root         (0)    13730 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNameUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNote.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNoteUI.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoSuperSubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     7207 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoUnicode.py
--rw-rw-rw-   0 root         (0) root         (0)     2453 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoValidator.py
--rw-rw-rw-   0 root         (0) root         (0)    42659 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/glyphGrid.py
--rw-rw-rw-   0 root         (0) root         (0)    14736 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/groupsStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/hintPSlistCtrl.py
--rw-rw-rw-   0 root         (0) root         (0)     7302 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/hintPSpanel.py
--rw-rw-rw-   0 root         (0) root         (0)    16330 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/info.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/kerning.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/kerningStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/stemPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/font/zonePanelUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.715492 wbpUFO-0.2.8/Lib/wbpUFO/view/fontinfo/
--rw-rw-rw-   0 root         (0) root         (0)     5646 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/fontinfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5139 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/Lib/wbpUFO/view/glyph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.717492 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2356 2024-01-22 10:25:15.000000 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5957 2024-01-22 10:25:15.000000 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 10:25:15.000000 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-22 10:25:15.000000 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-22 10:25:15.000000 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-22 10:25:15.000000 wbpUFO-0.2.8/Lib/wbpUFO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2356 2024-01-22 10:25:15.717492 wbpUFO-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2276 2024-01-22 10:25:15.718492 wbpUFO-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 10:25:15.717492 wbpUFO-0.2.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/tests/test_dialogs.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/tests/test_documents.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/tests/test_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-01-22 10:25:14.000000 wbpUFO-0.2.8/tests/test_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.957738 wbpUFO-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.922738 wbpUFO-0.2.9/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.926738 wbpUFO-0.2.9/Lib/wbpUFO/
+-rw-rw-rw-   0 root         (0) root         (0)    10601 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.929738 wbpUFO-0.2.9/Lib/wbpUFO/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/dialogItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/dialogItemPickerUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/findGlyphListCtrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.930738 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24639 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)    20703 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.931738 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8756 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3465 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/font.py
+-rw-rw-rw-   0 root         (0) root         (0)    28062 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5759 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/editPanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    21510 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/menu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.935738 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py
+-rw-rw-rw-   0 root         (0) root         (0)    14003 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py
+-rw-rw-rw-   0 root         (0) root         (0)     2953 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py
+-rw-rw-rw-   0 root         (0) root         (0)    17167 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py
+-rw-rw-rw-   0 root         (0) root         (0)     7101 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2756 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py
+-rw-rw-rw-   0 root         (0) root         (0)     4709 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/glyphGridStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5122 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/kerningViewCanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/kerningViewPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/libControl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/panelItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/control/panelItemPickerUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.941738 wbpUFO-0.2.9/Lib/wbpUFO/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/anchorDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4887 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/anchorDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/assignLayerDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/assignLayerDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/componentDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/componentDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/deleteGlyphsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6368 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/findGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5036 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/findGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/guidelineDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/guidelineDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/layerDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/layerDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/newFontDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/newFontDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/newGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/newGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     8386 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/renameGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     9608 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/renameGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5367 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/revertFontDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7261 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/revertFontDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/selectFontsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/dialog/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    19544 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.943738 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4530 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/commandListCtrl.py
+-rw-rw-rw-   0 root         (0) root         (0)    13260 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/commandListDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    12967 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/commandListDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/guideline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7342 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/metric.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5157 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/parameter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.944738 wbpUFO-0.2.9/Lib/wbpUFO/panel/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/panel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16132 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/panel/glyphViewCanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/panel/glyphViewPanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/panel/glyphViewPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.946738 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/editTool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/glyphLock.py
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/glyphShow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/toolbar/markColor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.946738 wbpUFO-0.2.9/Lib/wbpUFO/view/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.956738 wbpUFO-0.2.9/Lib/wbpUFO/view/font/
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20645 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoCaret.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoCaretUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoClassification.py
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoClassificationUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoCodepage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoCodepageUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     8952 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoControl.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoEmbedding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoEncodingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHinting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHintingPS.py
+-rw-rw-rw-   0 root         (0) root         (0)    10731 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6830 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHintingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoIdentification.py
+-rw-rw-rw-   0 root         (0) root         (0)     6714 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoLegal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6955 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoLegalUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoLine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4862 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoLineUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoMetric.py
+-rw-rw-rw-   0 root         (0) root         (0)    13226 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoMetricUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoName.py
+-rw-rw-rw-   0 root         (0) root         (0)    13730 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNameUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNoteUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoSuperSubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     7207 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoUnicode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2453 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoValidator.py
+-rw-rw-rw-   0 root         (0) root         (0)    44194 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/glyphGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    14736 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/groupsStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/hintPSlistCtrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7302 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/hintPSpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    16330 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/kerning.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/kerningStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/stemPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/font/zonePanelUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.956738 wbpUFO-0.2.9/Lib/wbpUFO/view/fontinfo/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/fontinfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/Lib/wbpUFO/view/glyph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.957738 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-02-02 16:24:52.000000 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5957 2024-02-02 16:24:52.000000 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 16:24:52.000000 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-02 16:24:52.000000 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-02-02 16:24:52.000000 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-02-02 16:24:52.000000 wbpUFO-0.2.9/Lib/wbpUFO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-02-02 16:24:52.957738 wbpUFO-0.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2024-02-02 16:24:52.958738 wbpUFO-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 16:24:52.957738 wbpUFO-0.2.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/tests/test_dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/tests/test_documents.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/tests/test_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-02-02 16:24:51.000000 wbpUFO-0.2.9/tests/test_views.py
```

### Comparing `wbpUFO-0.2.8/LICENSE` & `wbpUFO-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .toolbar.markColor import GlyphMarkToolbar
 from .view.font import UfoFontView
 from .view.glyph import UfoGlyphView
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 
 def getApp() -> App:
     """
     The currently running Workbench application.
     """
     return wx.GetApp()
```

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/config.py` & `wbpUFO-0.2.9/Lib/wbpUFO/config.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/dialogItemPicker.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/dialogItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/dialogItemPickerUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/dialogItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/findGlyphListCtrl.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/findGlyphListCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/canvas.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/canvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/cursor.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/cursor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/base.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/font.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/font.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/editPanel.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/editPanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/menu.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/menu.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/base.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/glyphGridStatusPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/glyphGridStatusPanelUI.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,22 @@
 		self.button_fontinfo.SetToolTip( u"Open Font Info" )
 
 		sizer.Add( self.button_fontinfo, 0, wx.ALL|wx.ALIGN_CENTER_VERTICAL, 5 )
 
 
 		sizer.Add( ( 0, 0), 1, wx.EXPAND, 0 )
 
+		self.searchCtrl = wx.SearchCtrl( self, wx.ID_ANY, wx.EmptyString, wx.DefaultPosition, wx.DefaultSize, wx.TE_NOHIDESEL )
+		self.searchCtrl.ShowSearchButton( True )
+		self.searchCtrl.ShowCancelButton( True )
+		self.searchCtrl.SetMinSize( wx.Size( 100,-1 ) )
+		self.searchCtrl.SetMaxSize( wx.Size( 250,-1 ) )
+
+		sizer.Add( self.searchCtrl, 1, wx.ALL|wx.ALIGN_CENTER_VERTICAL, 5 )
+
 		self.text_glyph = wx.StaticText( self, wx.ID_ANY, u"Glyph", wx.DefaultPosition, wx.Size( -1,-1 ), 0 )
 		self.text_glyph.Wrap( -1 )
 
 		sizer.Add( self.text_glyph, 0, wx.ALL|wx.ALIGN_CENTER_VERTICAL, 2 )
 
 		self.text_current = wx.StaticText( self, wx.ID_ANY, wx.EmptyString, wx.DefaultPosition, wx.Size( 150,-1 ), wx.ST_ELLIPSIZE_MIDDLE|wx.BORDER_THEME )
 		self.text_current.Wrap( -1 )
@@ -77,27 +85,35 @@
 
 		self.SetSizer( sizer )
 		self.Layout()
 		sizer.Fit( self )
 
 		# Connect Events
 		self.button_fontinfo.Bind( wx.EVT_BUTTON, self.on_button_fontinfo )
+		self.searchCtrl.Bind( wx.EVT_SEARCHCTRL_CANCEL_BTN, self.onSearchCancel )
+		self.searchCtrl.Bind( wx.EVT_TEXT, self.onSearchText )
 		self.text_current.Bind( wx.EVT_UPDATE_UI, self.update_current )
 		self.text_unicodes.Bind( wx.EVT_UPDATE_UI, self.update_unicodes )
 		self.text_selected_count.Bind( wx.EVT_UPDATE_UI, self.update_selected_count )
 		self.text_total_count.Bind( wx.EVT_UPDATE_UI, self.update_total_count )
 
 	def __del__( self ):
 		pass
 
 
 	# Virtual event handlers, override them in your derived class
 	def on_button_fontinfo( self, event ):
 		event.Skip()
 
+	def onSearchCancel( self, event ):
+		event.Skip()
+
+	def onSearchText( self, event ):
+		event.Skip()
+
 	def update_current( self, event ):
 		event.Skip()
 
 	def update_unicodes( self, event ):
 		event.Skip()
 
 	def update_selected_count( self, event ):
```

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/kerningViewCanvas.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/kerningViewCanvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/kerningViewPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/kerningViewPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/libControl.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/libControl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/panelItemPicker.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/panelItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/control/panelItemPickerUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/control/panelItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/anchorDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/anchorDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/anchorDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/anchorDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/assignLayerDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/assignLayerDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/assignLayerDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/assignLayerDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/componentDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/componentDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/componentDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/componentDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/deleteGlyphsDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/deleteGlyphsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/findGlyphDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/findGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/findGlyphDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/findGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/guidelineDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/guidelineDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/guidelineDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/guidelineDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/layerDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/layerDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/layerDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/layerDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/newFontDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/newFontDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/newGlyphDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/newGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/newGlyphDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/newGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/renameGlyphDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/renameGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/renameGlyphDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/renameGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/revertFontDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/revertFontDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/revertFontDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/revertFontDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/selectFontsDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/selectFontsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/dialog/selectFontsDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/dialog/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/document.py` & `wbpUFO-0.2.9/Lib/wbpUFO/document.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/anchor.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/anchor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/base.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/commandListCtrl.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/commandListCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/commandListDialog.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/commandListDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/commandListDialogUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/commandListDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/composite.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/composite.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/contour.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/contour.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/guideline.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/guideline.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/layer.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/layer.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/metric.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/metric.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/misc.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/misc.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/glyphCommand/parameter.py` & `wbpUFO-0.2.9/Lib/wbpUFO/glyphCommand/parameter.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/panel/glyphViewCanvas.py` & `wbpUFO-0.2.9/Lib/wbpUFO/panel/glyphViewCanvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/panel/glyphViewPanel.py` & `wbpUFO-0.2.9/Lib/wbpUFO/panel/glyphViewPanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/panel/glyphViewPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/panel/glyphViewPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/template.py` & `wbpUFO-0.2.9/Lib/wbpUFO/template.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/command.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/command.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/editTool.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/editTool.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/glyphLock.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/glyphLock.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/glyphShow.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/glyphShow.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/layer.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/layer.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/toolbar/markColor.py` & `wbpUFO-0.2.9/Lib/wbpUFO/toolbar/markColor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/feature.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 feature
 ===============================================================================
 
 """
+from __future__ import annotations
+
 import logging
+from typing import Optional
 
-import fontTools.feaLib.ast as ast
 import wx
-import wx.stc as stc
 from feaASTools.inspect import isFeatureAutomatic, setFeatureAutomatic
+from fontTools.feaLib import ast
 from wbBase.control.textEditControl import STCfindReplaceMixin
 from wbBase.scripting import MacroButtonMixin
-from wbDefcon import Font
+from wbDefcon import Features, Font
+from wx import stc
 
 log = logging.getLogger(__name__)
 
 feaKeywords = """
 anchor anchorDef anon anonymous by contour cursive device 
 enum enumerate excludeDFLT exclude_dflt feature featureNames from 
 ignore IgnoreBaseGlyphs IgnoreLigatures IgnoreMarks 
@@ -149,14 +152,15 @@
         self.StyleSetSpec(STC_FEA_WORD, "fore:#0000FF,face:Consolas,size:11")
         self.StyleSetSpec(STC_FEA_CLASSNAME, "fore:#009900,face:Consolas,size:11")
         self.StyleSetSpec(
             STC_FEA_COMMENTLINE, "fore:#808080,back:#E0FCF0,face:Consolas,size:11"
         )
 
         self.updateFont = False
+        self.reloadFeatureText = True
 
         self.Bind(stc.EVT_STC_CHANGE, self.on_CHANGE)
         self.Bind(stc.EVT_STC_STYLENEEDED, self.on_STYLENEEDED)
 
     @property
     def font(self):
         """The wbDefcon Font object of this FeatureTextCtrl"""
@@ -187,26 +191,30 @@
 
     @property
     def features(self):
         if self._font:
             return self._font.features
 
     def handleNotification(self, notification):
-        if notification.name == "Features.TextChanged":
+        if notification.name == "Features.TextChanged" and self.reloadFeatureText:
             newText = notification.data["newValue"]
             if self.GetText() != newText:
                 self.SetText(newText)
+                print("reloadFeatureText done")
 
     def on_CHANGE(self, event):
         if self.updateFont:
             wx.LogDebug("FeatureTextCtrl.on_CHANGE")
             text = self.GetText()
             features = self.features
             if text != features.text:
+                self.reloadFeatureText = False
                 features.text = text
+                self.reloadFeatureText = True
+                self.SetFocus()
 
     def on_STYLENEEDED(self, event):
         self._lexer.styleText(event)
 
 
 class FeatureCtxMenue(wx.Menu):
     """Context Menu for feature items in the tree control"""
@@ -315,34 +323,37 @@
 
         # Connect Events
         self.Bind(wx.EVT_TREE_SEL_CHANGED, self.on_selectionChanged)
         self.Bind(wx.EVT_RIGHT_DOWN, self.on_rightDown)
         self.Bind(wx.EVT_RIGHT_UP, self.on_rightUp)
 
     @property
-    def font(self):
+    def font(self) -> Font:
         """The wbDefcon Font object of this FeatureTextCtrl"""
         return self._font
 
     @font.setter
-    def font(self, value):
+    def font(self, value: Font):
         assert self._font is None
         assert isinstance(value, Font)
         assert value == self.GrandParent._font
         self._font = value
-        # todo: start observation
+        self._font.features.addObserver(
+            self, "handleNotification", Features.changeNotificationName
+        )
         self.buildTree()
 
     @font.deleter
     def font(self):
-        # todo: stop observation
+        if isinstance(self._font, Font):
+            self._font.features.removeObserver(self, Features.changeNotificationName)
         self._font = None
 
     @property
-    def syntaxtree(self):
+    def syntaxtree(self) -> Optional[ast.FeatureFile]:
         if self._font:
             return self._font.features.getSyntaxtree(useGlyphNames=False)
 
     @property
     def textCtrl(self):
         return self.GrandParent.featureTextCtrl
 
@@ -381,27 +392,44 @@
             for statement in tree.statements:
                 self.appendStatement(self.root, statement)
             # self.ExpandAllChildren(self.root)
         else:
             log.debug("No syntaxtree")
         self.Thaw()
 
+    def handleNotification(self, notification):
+        if self.syntaxtree:
+            self.buildTree()
+
     # --------------------------------------------------------------------------
     # Event handler
     # --------------------------------------------------------------------------
 
     def on_selectionChanged(self, event):
+        if self.FindFocus() != self:
+            # event.Skip()
+            return
+        if self.IsFrozen():
+            return
         try:
             data = self.GetItemData(event.Item)
         except RuntimeError:
             return
         if data:
-            self.textCtrl.GotoLine(data.location[1])
-            self.textCtrl.LineUpExtend()
-        event.Skip()
+            ctrl = self.textCtrl
+            # print(self.FindFocus())
+            # print(f"line before {ctrl.GetCurrentLine()}")
+            ctrl.GotoLine(data.location[1] + int(ctrl.LinesOnScreen() / 2))
+            ctrl.GotoLine(data.location[1])
+            ctrl.Home()
+            # ctrl.GotoPos(ctrl.PositionFromLine(ctrl.GetCurrentLine()))
+            ctrl.LineUpExtend()
+            ctrl.SetFocus()
+            # print(f"line after {ctrl.GetCurrentLine()}")
+        # event.Skip()
 
     def on_rightDown(self, event):
         position = event.GetPosition()
         item, __ = self.HitTest(position)
         if item:
             self.SelectItem(item)
 
@@ -422,17 +450,19 @@
 
 
 class FeatureStatusPanel(wx.Panel, MacroButtonMixin):
     """
     Tree Status Panel in the Feature Panel
     """
 
+    Parent: FeaturePage
+
     def __init__(
         self,
-        parent,
+        parent: FeaturePage,
         id=wx.ID_ANY,
         pos=wx.DefaultPosition,
         size=wx.DefaultSize,
         style=wx.BORDER_NONE,
     ):
         super().__init__(parent, id, pos, size, style, name="FeatureStatusPanel")
         sizer_outer = wx.BoxSizer(wx.VERTICAL)
```

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoBase.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoBase.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoCaretUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoCaretUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoClassificationUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoClassificationUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoCodepageUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoCodepageUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoControl.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoControl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoEncodingUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoEncodingUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHintingPS.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHintingPS.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoHintingUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoHintingUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoLegalUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoLegalUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoLineUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoLineUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoMetricUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoMetricUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNameUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNameUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoNoteUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoNoteUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/fontInfoValidator.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/fontInfoValidator.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/glyphGrid.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/glyphGrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 glyphGrid
 ===============================================================================
 
 """
+from __future__ import annotations
 import logging
 import os
 import pickle
 import zlib
 from math import sqrt
+from typing import List, Optional, TYPE_CHECKING
 
 import wx
 from defcon import registerRepresentationFactory
 from fontTools.misc.transform import Transform
 from fontTools.pens.boundsPen import ControlBoundsPen
 from fontTools.pens.transformPen import TransformPen
 from wbBase.scripting import MacroMenu
@@ -23,14 +25,17 @@
 from ...dialog.deleteGlyphsDialog import DeleteGlyphsDialog
 from ...dialog.findGlyphDialog import FindGlyphDialog
 from ...dialog.newGlyphDialog import NewGlyphDialog
 from ...dialog.renameGlyphDialog import RenameGlyphDialog
 from ...glyphCommand.commandListDialog import CommandListDialog
 from ..fontinfo import UfoFontInfoView
 
+if TYPE_CHECKING:
+    from wbBase.application import App
+
 log = logging.getLogger(__name__)
 
 
 def glyphBitmapRepresentationFactory(
     glyph: Glyph, width: int = 72, height: int = 88, captionHeight: int = 16
 ) -> bytes:
     imageHeight = height - captionHeight
@@ -92,15 +97,15 @@
             cut -= 1
         tx = (width - w) / 2
         ty = -1
         gc.DrawText(text, tx, ty)
 
     # draw border
     gc.SetPen(wx.ThePenList.FindOrCreatePen(wx.Colour(245, 245, 245, 255), 2, wx.SOLID))
-    border:wx.GraphicsPath = gc.CreatePath()
+    border: wx.GraphicsPath = gc.CreatePath()
     border.MoveToPoint(width, 0)
     border.AddLineToPoint(width, height)
     border.AddLineToPoint(0, height)
     gc.StrokePath(border)
 
     # return the bitmap as zlib compressed bytes
     dc.SelectObject(wx.NullBitmap)
@@ -171,15 +176,15 @@
         if any(os.path.isdir(p) for p in self.macroFolderPath):
             macroMenu = MacroMenu(folderList=self.macroFolderPath)
             item = self.AppendSubMenu(macroMenu, "Macros")
             item.SetBitmap(wx.ArtProvider.GetBitmap("PYTHON", wx.ART_MENU, (16, 16)))
             item.SetFont(app.TopWindow.Font)
 
     @property
-    def app(self):
+    def app(self) -> App:
         return wx.GetApp()
 
     @property
     def font(self):
         return self.glyphGrid.font
 
     @property
@@ -270,48 +275,67 @@
                 if commandList:
                     dialog.executeCommandList()
                     # self.glyphGrid.Refresh()
 
 
 class GlyphGridStatusPanel(GlyphGridStatusPanelUI):
     """Status Panel for GlyphGrid"""
+    def __init__(
+        self,
+        parent:GlyphGridPage,
+        id:int=wx.ID_ANY,
+        pos=wx.DefaultPosition,
+        size=wx.DefaultSize,
+        style:int=0,
+        name="GlyphGridStatusPanel",
+    ):
+        super().__init__(parent, id, pos, size, style, name)
+        self.searchCtrl.SetHint("filter glyphs")
 
     @property
-    def font(self):
+    def font(self) -> Font:
         return self.glyphGrid.font
 
     @property
-    def glyphGrid(self):
+    def glyphGrid(self) -> GlyphGrid:
         return self.GrandParent.glyphGridPanel
 
     # -------------------------------------------------------------------------
     # event handler
     # -------------------------------------------------------------------------
 
     def on_button_fontinfo(self, event):
-        wait = wx.BusyCursor()
-        window = wx.GetApp().TopWindow.panelManager.centerPane.window
-        window.Freeze()
-        doc = self.font.document
-        view = None
-        for v in doc.views:
-            if v.typeName == "UFO Font Info View":
-                view = v
-                break
-        if not view:
-            view = UfoFontInfoView()
-            if view.OnCreate(doc, None):
-                doc.AddView(view)
-                view.frame.font = self.font
-            else:
-                wx.LogError(f"Can not create view for {self.font}")
-                view.Destroy()
-                return
-        view.Activate()
-        window.Thaw()
+        with wx.BusyCursor():
+            window = wx.GetApp().TopWindow.panelManager.centerPane.window
+            window.Freeze()
+            doc = self.font.document
+            view = None
+            for v in doc.views:
+                if v.typeName == "UFO Font Info View":
+                    view = v
+                    break
+            if not view:
+                view = UfoFontInfoView()
+                if view.OnCreate(doc, None):
+                    doc.AddView(view)
+                    view.frame.font = self.font
+                else:
+                    wx.LogError(f"Can not create view for {self.font}")
+                    view.Destroy()
+                    window.Thaw()
+                    return
+            view.Activate()
+            window.Thaw()
+
+    def onSearchCancel(self, event:wx.CommandEvent):
+        del self.glyphGrid.searchText
+        event.Skip()
+
+    def onSearchText(self, event:wx.CommandEvent):
+        self.glyphGrid.searchText = event.GetString()
 
     def update_current(self, event):
         if self.glyphGrid.selectedIndex >= 0:
             try:
                 label = self.glyphGrid.glyphNames[self.glyphGrid.selectedIndex]
             except IndexError:
                 label = ""
@@ -369,22 +393,23 @@
         self.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_LISTBOX))
         self._imageSize = 48
         self._cellCaption = "name"
         self._cellCaptionHeight = 12
         self._visibleGlyphs = set()
         self._observedGlyphs = set()
         self._font = None
-        self._glyphNames = None
+        self._glyphNames: List[str] = []
         self._cells = []
         self._pointed = -1
         self._selector = None
         self._currenter = None
         self._skipExportMarker = None
         self._selectedIndex = -1
         self._mouseeventhandled = False
+        self._searchText = ""
 
         self._showTooltip = False
         self._tooltipWin = None
         self._menu = None
         self._notifications = ("Glyph.Changed", "Glyph.NameChanged")
 
         self.brushBackground = wx.TheBrushList.FindOrCreateBrush(
@@ -426,19 +451,19 @@
     # -------------------------------------------------------------------------
 
     @property
     def app(self):
         return wx.GetApp()
 
     @property
-    def font(self):
+    def font(self) -> Font:
         return self._font
 
     @font.setter
-    def font(self, value):
+    def font(self, value: Font):
         assert self._font is None
         assert isinstance(value, Font)
         assert (
             value == self.GrandParent._document._data
         ), f"expected {self.GrandParent.font}, got {value}"
         self._font = value
         self._font.addObserver(self, "handleNotification", "Font.GlyphOrderChanged")
@@ -475,25 +500,27 @@
         return self.GrandParent.view
 
     @property
     def cells(self):
         return self._cells
 
     @property
-    def glyphNames(self):
+    def glyphNames(self) -> List[str]:
         font = self.font
-        if font:
-            if self._glyphNames is None:
-                names = [g for g in set(font.glyphOrder) if g in font]
-                names.sort(key=font.glyphOrder.index)
-                other = list(font.keys() - set(names))
-                other.sort()
-                self._glyphNames = names + other
-            return self._glyphNames
-        return []
+        if not font:
+            return []
+        if not self._glyphNames:
+            names = [g for g in set(font.glyphOrder) if g in font]
+            names.sort(key=font.glyphOrder.index)
+            other = list(font.keys() - set(names))
+            other.sort()
+            self._glyphNames = names + other
+        if self._searchText:
+            self._glyphNames = [g for g in self._glyphNames if self._searchText in g]
+        return self._glyphNames
 
     @property
     def selectedIndex(self):
         return self._selectedIndex
 
     @selectedIndex.setter
     def selectedIndex(self, index):
@@ -502,46 +529,46 @@
                 raise IndexError
             old = self._selectedIndex
             self._selectedIndex = index
             self.refreshCellIndex(old)
             self.refreshCellIndex(self._selectedIndex)
 
     @property
-    def currentGlyph(self):
+    def currentGlyph(self) -> Optional[Glyph]:
         if self._font:
             index = self._selectedIndex
             if index >= 0:
                 name = self.glyphNames[index]
                 if name in self._font:
                     return self._font[name]
 
     @property
-    def cellWidth(self):
+    def cellWidth(self) -> int:
         return self._imageSize
 
     @property
-    def cellHeight(self):
+    def cellHeight(self) -> int:
         if self._cellCaption is None:
             return self._imageSize
         else:
             return self._imageSize + self._cellCaptionHeight
 
     @property
-    def captionHeight(self):
+    def captionHeight(self) -> int:
         return self._cellCaptionHeight
 
     @property
-    def collCount(self):
+    def collCount(self) -> int:
         cols = int(self.GetClientSize().GetWidth() / self.cellWidth)
         if cols == 0:
             cols = 1
         return cols
 
     @property
-    def rowCount(self):
+    def rowCount(self) -> int:
         cols = self.collCount
         count = len(self.glyphNames)
         rows = int(count / cols)
         if cols * rows < count:
             rows += 1
         return rows
 
@@ -617,47 +644,66 @@
             gc.SetBrush(wx.TRANSPARENT_BRUSH)
             gc.DrawEllipse(1, 1, size - 2, size - 2)
             gc.DrawLines([(1, size / 2), (size - 1, size / 2)])
             dc.SelectObject(wx.NullBitmap)
         return self._skipExportMarker
 
     @property
-    def showTooltip(self):
+    def showTooltip(self) -> bool:
         return self._showTooltip
 
     @showTooltip.setter
     def showTooltip(self, value):
         assert isinstance(value, bool)
         self._showTooltip = value
         if value and self._tooltipWin is None:
             self._tooltipWin = wx.ToolTip(" " * 100 + "\n" * 50)
             self._tooltipWin.SetDelay(1000)
             self.SetToolTip(self._tooltipWin)
         if self._tooltipWin is not None:
             self._tooltipWin.Enable(value)
 
     @property
-    def contextMenu(self):
+    def contextMenu(self) -> GlyphGridContextMenu:
         if self._menu is None:
             self._menu = GlyphGridContextMenu(self)
         return self._menu
 
     @property
-    def paintRect(self):
+    def paintRect(self) -> wx.Rect:
         """
         Returns The Paint Bounding Rect For The on_PAINT() Method.
         """
         size = self.GetClientSize()
         rect = wx.Rect(0, 0, size.GetWidth(), size.GetHeight())
         rect.x, rect.y = self.GetViewStart()
         xu, yu = self.GetScrollPixelsPerUnit()
         rect.x = rect.x * xu
         rect.y = rect.y * yu
         return rect
 
+    @property
+    def searchText(self) -> str:
+        return self._searchText
+
+    @searchText.setter
+    def searchText(self, text: str) -> None:
+        del self.font.selectedGlyphs
+        self._searchText = text
+        self._glyphNames = []
+        self.SendSizeEvent()
+        # self.Refresh()
+
+    @searchText.deleter
+    def searchText(self):
+        self._searchText = ""
+        self._glyphNames = []
+        self.SendSizeEvent()
+        # self.Refresh()
+
     # -------------------------------------------------------------------------
     # notification handling
     # -------------------------------------------------------------------------
 
     def updateObservation(self):
         font = self.font
         for glyphName in self._observedGlyphs - self._visibleGlyphs:
@@ -679,36 +725,36 @@
             ]:
                 self.refreshGlyphName(name)
             for name in [
                 n for n in notification.data["selected"] if n in self._observedGlyphs
             ]:
                 self.refreshGlyphName(name)
         elif notification.name in ("Layer.GlyphAdded", "Layer.GlyphDeleted"):
-            self._glyphNames = None
+            self._glyphNames = []
             self.updateProp()
             self.SendSizeEvent()
         elif notification.name == "Glyph.NameChanged":
             old = notification.data["oldValue"]
             new = notification.data["newValue"]
             if old in self._visibleGlyphs:
                 self._visibleGlyphs.remove(old)
                 self._visibleGlyphs.add(new)
             if old in self._observedGlyphs:
                 self._observedGlyphs.remove(old)
                 self._observedGlyphs.add(new)
-            self._glyphNames = None
+            self._glyphNames = []
         elif notification.name == "Glyph.Changed":
             self.refreshGlyphName(notification.object.name)
         elif notification.name == "Layer.GlyphNameChanged":
-            self._glyphNames = None
+            self._glyphNames = []
         elif notification.name == "Font.GlyphOrderChanged":
-            self._glyphNames = None
+            self._glyphNames = []
         else:
             print(f"unhandled notification: {notification}")
-        if self._glyphNames is None:
+        if not self._glyphNames:
             self.Refresh()
 
     # -------------------------------------------------------------------------
     # Public methods
     # -------------------------------------------------------------------------
 
     def CanCopy(self):
@@ -789,17 +835,16 @@
             self.updateProp(False)
 
     def IsSelected(self, index):
         """Returns Whether A Cell Is Selected Or Not."""
         return self.font[self.glyphNames[index]].selected
 
     def SelectAll(self):
-        wx.BeginBusyCursor()
-        self.font.selectAll()
-        wx.EndBusyCursor()
+        with wx.BusyCursor():
+            self.font.selectedGlyphNames = self.glyphNames
 
     def refreshCellIndex(self, index):
         """refresh cell with given index"""
         width = self.cellWidth
         height = self.cellHeight
         col = index % self.collCount
         row = int(index / self.collCount)
```

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/groups.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/groups.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/groupsStatusPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/groupsStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/hintPSlistCtrl.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/hintPSlistCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/hintPSpanel.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/hintPSpanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/info.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/info.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/kerning.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/kerning.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/kerningStatusPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/kerningStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/stemPanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/stemPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/font/zonePanelUI.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/font/zonePanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/fontinfo/__init__.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/fontinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO/view/glyph.py` & `wbpUFO-0.2.9/Lib/wbpUFO/view/glyph.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO.egg-info/PKG-INFO` & `wbpUFO-0.2.9/Lib/wbpUFO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUFO
-Version: 0.2.8
+Version: 0.2.9
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUFO
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUFO/-/issues
```

### Comparing `wbpUFO-0.2.8/Lib/wbpUFO.egg-info/SOURCES.txt` & `wbpUFO-0.2.9/Lib/wbpUFO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/PKG-INFO` & `wbpUFO-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUFO
-Version: 0.2.8
+Version: 0.2.9
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUFO
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUFO/-/issues
```

### Comparing `wbpUFO-0.2.8/README.md` & `wbpUFO-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/setup.cfg` & `wbpUFO-0.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.8
+current_version = 0.2.9
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

### Comparing `wbpUFO-0.2.8/tests/test_dialogs.py` & `wbpUFO-0.2.9/tests/test_dialogs.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/tests/test_documents.py` & `wbpUFO-0.2.9/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/tests/test_imports.py` & `wbpUFO-0.2.9/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/tests/test_templates.py` & `wbpUFO-0.2.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.8/tests/test_views.py` & `wbpUFO-0.2.9/tests/test_views.py`

 * *Files identical despite different names*

