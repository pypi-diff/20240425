# Comparing `tmp/srsgui-0.4.3.tar.gz` & `tmp/srsgui-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-wr6qzki4\srsgui-0.4.3.tar", last modified: Tue Aug  8 21:41:58 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-g3028gea\srsgui-0.4.4.tar", last modified: Tue Apr 23 20:33:47 2024, max compression
```

## Comparing `srsgui-0.4.3.tar` & `srsgui-0.4.4.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.723148 srsgui-0.4.3/
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.590935 srsgui-0.4.3/.github/
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.600903 srsgui-0.4.3/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-07-14 19:39:01.000000 srsgui-0.4.3/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-07-14 19:39:01.000000 srsgui-0.4.3/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-07-14 19:39:01.000000 srsgui-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4626 2023-08-08 21:41:58.723148 srsgui-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3595 2023-07-14 20:50:24.000000 srsgui-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.628717 srsgui-0.4.3/docs/
--rw-rw-rw-   0        0        0      654 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    88057 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/dock_widget_floating.png
--rw-rw-rw-   0        0        0    97266 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/dock_widgets_expanded.png
--rw-rw-rw-   0        0        0    71070 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    52123 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/lockin-capture.png
--rw-rw-rw-   0        0        0    29667 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    38581 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/task_selection.png
--rw-rw-rw-   0        0        0    39412 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     8703 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/application.rst
--rw-rw-rw-   0        0        0      840 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/changelog.rst
--rw-rw-rw-   0        0        0     1921 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/conf.py
--rw-rw-rw-   0        0        0     6270 2023-07-14 20:50:24.000000 srsgui-0.4.3/docs/create-project.rst
--rw-rw-rw-   0        0        0     7546 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/create-task.rst
--rw-rw-rw-   0        0        0     6547 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    16790 2023-07-14 20:50:24.000000 srsgui-0.4.3/docs/example.rst
--rw-rw-rw-   0        0        0     3837 2023-07-14 20:50:24.000000 srsgui-0.4.3/docs/index.rst
--rw-rw-rw-   0        0        0     4539 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      930 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1101 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1539 2023-07-14 20:50:24.000000 srsgui-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-07-14 19:39:01.000000 srsgui-0.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 21:41:58.733143 srsgui-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-07-14 19:39:01.000000 srsgui-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/srsgui/
--rw-rw-rw-   0        0        0     1552 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.590935 srsgui-0.4.3/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.658701 srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1829 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3147 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1998 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.658701 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     4101 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/captured_fft.py
--rw-rw-rw-   0        0        0     1662 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/identify.py
--rw-rw-rw-   0        0        0     2585 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/plot_example.py
--rw-rw-rw-   0        0        0     1946 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/scope_capture.py
--rw-rw-rw-   0        0        0     2549 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/simulated_fft.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.670172 srsgui-0.4.3/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9908 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.680169 srsgui-0.4.3/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8309 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1277 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8775 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11334 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    19292 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      845 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10411 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9992 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.690163 srsgui-0.4.3/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0     1313 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6990 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5858 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6939 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    25314 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4226 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.713154 srsgui-0.4.3/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3895 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6881 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.723148 srsgui-0.4.3/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1604 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12606 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8670 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5697 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3453 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4853 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9797 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3976 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15881 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    15296 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.723148 srsgui-0.4.3/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      800 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      678 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      778 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1372 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2769 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1006 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    26324 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/srsgui.egg-info/
--rw-rw-rw-   0        0        0     4626 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3201 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.476046 srsgui-0.4.4/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.306006 srsgui-0.4.4/.github/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.329614 srsgui-0.4.4/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-07-14 19:39:01.000000 srsgui-0.4.4/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-07-14 19:39:01.000000 srsgui-0.4.4/.gitignore
+-rw-rw-rw-   0        0        0     1112 2024-04-18 18:10:34.000000 srsgui-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4927 2024-04-23 20:33:47.476046 srsgui-0.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.359598 srsgui-0.4.4/docs/
+-rw-rw-rw-   0        0        0      654 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.379587 srsgui-0.4.4/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8703 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/application.rst
+-rw-rw-rw-   0        0        0     1023 2024-04-19 17:13:32.000000 srsgui-0.4.4/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1920 2024-04-18 18:11:27.000000 srsgui-0.4.4/docs/conf.py
+-rw-rw-rw-   0        0        0     6270 2023-07-14 20:50:24.000000 srsgui-0.4.4/docs/create-project.rst
+-rw-rw-rw-   0        0        0     7546 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6547 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    16790 2023-07-14 20:50:24.000000 srsgui-0.4.4/docs/example.rst
+-rw-rw-rw-   0        0        0     3837 2023-07-14 20:50:24.000000 srsgui-0.4.4/docs/index.rst
+-rw-rw-rw-   0        0        0     4539 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-07-14 19:39:01.000000 srsgui-0.4.4/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1091 2023-08-10 16:57:38.000000 srsgui-0.4.4/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1539 2023-07-14 20:50:24.000000 srsgui-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0     3595 2023-07-14 20:50:24.000000 srsgui-0.4.4/readme.md
+-rw-rw-rw-   0        0        0       37 2023-07-14 19:39:01.000000 srsgui-0.4.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 20:33:47.476046 srsgui-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-07-14 19:39:01.000000 srsgui-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.389581 srsgui-0.4.4/srsgui/
+-rw-rw-rw-   0        0        0     1552 2024-04-18 17:48:07.000000 srsgui-0.4.4/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.319616 srsgui-0.4.4/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.389581 srsgui-0.4.4/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.399576 srsgui-0.4.4/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1829 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3147 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1998 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.406080 srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     4101 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/captured_fft.py
+-rw-rw-rw-   0        0        0     1662 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/identify.py
+-rw-rw-rw-   0        0        0     2585 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/plot_example.py
+-rw-rw-rw-   0        0        0     1946 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/scope_capture.py
+-rw-rw-rw-   0        0        0     2549 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/simulated_fft.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.416078 srsgui-0.4.4/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9910 2023-11-30 18:30:47.000000 srsgui-0.4.4/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.426072 srsgui-0.4.4/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8309 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1277 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8775 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11334 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    19500 2023-12-01 23:54:01.000000 srsgui-0.4.4/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      845 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10411 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0    10007 2024-04-18 16:51:06.000000 srsgui-0.4.4/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.436066 srsgui-0.4.4/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0     1313 2023-08-08 21:25:52.000000 srsgui-0.4.4/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6990 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5858 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6939 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    25323 2023-12-02 00:09:10.000000 srsgui-0.4.4/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4226 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.456056 srsgui-0.4.4/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     4189 2023-08-29 23:22:58.000000 srsgui-0.4.4/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6881 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.466051 srsgui-0.4.4/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1604 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12606 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8670 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5697 2023-08-08 21:25:52.000000 srsgui-0.4.4/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3453 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4853 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9797 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3976 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15881 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    15296 2023-08-08 21:25:52.000000 srsgui-0.4.4/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.476046 srsgui-0.4.4/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      800 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      678 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      778 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1372 2023-08-08 21:25:52.000000 srsgui-0.4.4/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2769 2023-08-08 21:25:52.000000 srsgui-0.4.4/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1006 2023-07-14 20:50:24.000000 srsgui-0.4.4/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    26324 2023-08-08 21:25:52.000000 srsgui-0.4.4/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-07-14 19:39:01.000000 srsgui-0.4.4/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:33:47.476046 srsgui-0.4.4/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     4927 2024-04-23 20:33:47.000000 srsgui-0.4.4/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3201 2024-04-23 20:33:47.000000 srsgui-0.4.4/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:33:47.000000 srsgui-0.4.4/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-23 20:33:47.000000 srsgui-0.4.4/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2024-04-23 20:33:47.000000 srsgui-0.4.4/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 20:33:47.000000 srsgui-0.4.4/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.4.3/.gitignore` & `srsgui-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/LICENSE.txt` & `srsgui-0.4.4/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 The MIT License
 
-Copyright (c) 2022, 2023 Stanford Research Systems
+Copyright (c) 2022-2024 Stanford Research Systems
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `srsgui-0.4.3/PKG-INFO` & `srsgui-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.3
+Version: 0.4.4
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
@@ -15,17 +15,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pyserial>=3
 Provides-Extra: full
+Requires-Dist: matplotlib>=3.6.2; extra == "full"
+Requires-Dist: pyside6; extra == "full"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: matplotlib; extra == "docs"
+Requires-Dist: pyside2; extra == "docs"
+Requires-Dist: sphinx>=5; extra == "docs"
+Requires-Dist: sphinx-rtd-theme>=1; extra == "docs"
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication, based on the 
      [`Instrument`](https://thinksrs.github.io/srsgui/srsgui.inst.html#module-srsgui.inst.instrument)
```

### Comparing `srsgui-0.4.3/README.md` & `srsgui-0.4.4/readme.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/Makefile` & `srsgui-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.4.4/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.4.4/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.4.4/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/dock_widget_floating.png` & `srsgui-0.4.4/docs/_static/dock_widget_floating.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/dock_widgets_expanded.png` & `srsgui-0.4.4/docs/_static/dock_widgets_expanded.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/example-screen-capture-1.png` & `srsgui-0.4.4/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/example-screen-capture-2.png` & `srsgui-0.4.4/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/initial-screen-capture.png` & `srsgui-0.4.4/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/lockin-capture.png` & `srsgui-0.4.4/docs/_static/lockin-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.4.4/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/second-task-screen-capture.png` & `srsgui-0.4.4/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/task_selection.png` & `srsgui-0.4.4/docs/_static/task_selection.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/terminal-with-example-2.png` & `srsgui-0.4.4/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/_static/terminal-with-example.png` & `srsgui-0.4.4/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/application.rst` & `srsgui-0.4.4/docs/application.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/changelog.rst` & `srsgui-0.4.4/docs/changelog.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Changelog
 ==========
+V.0.4.4 -- Apr 18, 2024
+    * Changed :meth:`Instrument.get_available_interfaces <srsgui.inst.instrument.Instrument.get_available_interfaces>`
+      to a class method.
+
 V.0.4.0 -- Jun 21, 2023
     * Changed :mod:`IndexCommand <srsgui.inst.indexcommands>`
       to instance variable to handle multiple instances correctly.
       It requires a subclass of IndexCommand to be defined in __init__() of the subclass.
       self.add_parent_to_index_commands() should be called after the definition of index commands.
 
 V.0.3.4 -- Jun 20, 2023
-    * Removed default_value from :class:`CommandInput <srsgui.task.inputs.CommandInput>`.__init__.
-      cmd_instance argument is not necessary, either.
+    * Removed *default_value* from :class:`CommandInput <srsgui.task.inputs.CommandInput>`.__init__().
+      The *cmd_instance* argument is not necessary, either.
 
 V.0.3.1 -- May 22, 2023
     * Changed task result file name extension to .sgdata.
 
 V.0.3.0 -- May 16, 2023
     * Moved documentation to Github Pages.
     * Added boilerplate license header to source files.
```

### Comparing `srsgui-0.4.3/docs/conf.py` & `srsgui-0.4.4/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from srsgui import __version__
 
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'srsgui'
-copyright = '2022, 2023, Stanford Research Systems'
+copyright = '2022-2024, Stanford Research Systems'
 author = 'Chulhoon Kim'
 version = __version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
```

### Comparing `srsgui-0.4.3/docs/create-project.rst` & `srsgui-0.4.4/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/create-task.rst` & `srsgui-0.4.4/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/define-instrument.rst` & `srsgui-0.4.4/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/example.rst` & `srsgui-0.4.4/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/index.rst` & `srsgui-0.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/installation.rst` & `srsgui-0.4.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/make.bat` & `srsgui-0.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/srsgui.inst.communications.rst` & `srsgui-0.4.4/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/srsgui.inst.rst` & `srsgui-0.4.4/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/srsgui.task.rst` & `srsgui-0.4.4/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/srsgui.ui.commandtree.rst` & `srsgui-0.4.4/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/srsgui.ui.qt.rst` & `srsgui-0.4.4/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/srsgui.ui.rst` & `srsgui-0.4.4/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/docs/troubleshooting.rst` & `srsgui-0.4.4/docs/troubleshooting.rst`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 General
 --------
 'PySide6.QtGui.QAction' object has no attribute 'menu'.
 `````````````````````````````````````````````````````````
 
     It happens with PySide6 V.6.2.4. or earlier.
-    It is fixed with V.6.5.1 or possibly before.
+    It is fixed with V.6.3.0 or later.
     If 'pip' does not allow to upgrade to a newer version, upgrade 'pip' first.
 
 .. code-block::
 
     # Upgrade pip, if necessary.
     python -m pip install pip --upgrade
```

### Comparing `srsgui-0.4.3/pyproject.toml` & `srsgui-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/__init__.py` & `srsgui-0.4.4/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst.communications import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.4.3"  # Global version number
+__version__ = "0.4.4"  # Global version number
```

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/captured_fft.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/captured_fft.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/identify.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/identify.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/plot_example.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/plot_example.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/scope_capture.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/scope_capture.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/simulated_fft.py` & `srsgui-0.4.4/srsgui/examples/oscilloscope example/tasks/simulated_fft.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/__init__.py` & `srsgui-0.4.4/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/commands.py` & `srsgui-0.4.4/srsgui/inst/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,10 +302,11 @@
 
 class DictGetCommand(DictCommand):
     """
     Descriptor for  a remote command only to **query** a **dict** value.
     To **set** a value is not allowed.
     """
     _set_enable = False
+
     def __set__(self, instance, value):
         raise AttributeError('No set command for {}'
                              .format(self.remote_command))
```

### Comparing `srsgui-0.4.3/srsgui/inst/communications/interface.py` & `srsgui-0.4.4/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/communications/serial_ports.py` & `srsgui-0.4.4/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/communications/serialinterface.py` & `srsgui-0.4.4/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.4.4/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/component.py` & `srsgui-0.4.4/srsgui/inst/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,23 @@
                     continue
                 current_attributes.append(key)
                 if callable(child):
                     method_list.append('{}'.format(key))
         return method_list
 
     def get_command_info(self, command_name):
+        """
+        get detailed information on the command with command_name
+
+        returns
+        --------
+            dict
+                dictionary of information on the command
+        """
+
         if hasattr(self.__class__, command_name):
             cmd = self.__class__.__dict__[command_name]
         elif hasattr(self, command_name):
             cmd = self.__dict__[command_name]
         else:
             raise AttributeError("No command named '{}' in {}".format(command_name, self.__class__.__name__))
```

### Comparing `srsgui-0.4.3/srsgui/inst/exceptions.py` & `srsgui-0.4.4/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/indexcommands.py` & `srsgui-0.4.4/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/inst/instrument.py` & `srsgui-0.4.4/srsgui/inst/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,30 +214,31 @@
                               .format(self._IdString, reply))
         self._id_string = reply
         self._model_name = model_name
         self._serial_number = serial_number
         self._firmware_version = firmware_version
         return self._model_name, self._serial_number, self._firmware_version
 
-    def get_available_interfaces(self):
+    @classmethod
+    def get_available_interfaces(cls):
         """
         Get available communication interfaces for the instrument
 
         :rtype: dict
         """
         d = {}
-        for interface in self.available_interfaces:
+        for interface in cls.available_interfaces:
             d[interface[0].NAME] = interface
         return d
 
     def get_info(self):
         """
         Get the instrument information
 
-        default return value is a dictionalry containing model name, serial number,
+        default return value is a dictionary containing model name, serial number,
         firmware version. A subclass can add more information into the dictionary
         as needed.
 
         :rtype: dict
         """
         d = self.comm.get_info()
         if type(d) is dict:
```

### Comparing `srsgui-0.4.3/srsgui/task/callbacks.py` & `srsgui-0.4.4/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/task/config.py` & `srsgui-0.4.4/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/task/inputs.py` & `srsgui-0.4.4/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/task/sessionhandler.py` & `srsgui-0.4.4/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/task/task.py` & `srsgui-0.4.4/srsgui/task/task.py`

 * *Files identical despite different names*

```diff
@@ -118,15 +118,15 @@
         it runs test(), the main routine of the task.
         If setup() finished with an error, test() will not even start.
         """
         self.logger.warning("Task.setup() is not overridden.")
 
     def test(self):
         """
-        Test() is the main part of a Task. And a lot of times, test() takes long time to finish.
+        Test() is the main part of a Task subclass. And a lot of times, test() takes long time to finish.
         Check frequently if is_running() is true. If not, test() should finish voluntarily
         as soon as possible.
         """
         raise NotImplementedError("A test() should be implemented!")
 
     def cleanup(self):
         """
```

### Comparing `srsgui-0.4.3/srsgui/task/taskresult.py` & `srsgui-0.4.4/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandhandler.py` & `srsgui-0.4.4/srsgui/ui/commandhandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,11 +100,19 @@
         self.worker_thread.start()
 
     def process_command(self, cmd, reply):
         self.worker.inst_dict = self.parent.inst_dict
         self.worker.figure_dict = self.parent.dock_handler.get_figure_dict()
         self.request_command.emit(cmd, reply)
 
+    def process_command_without_figure_dict(self, cmd, reply):
+        """
+        Handles a command from a parent without dock_handler
+        """
+        self.worker.inst_dict = self.parent.inst_dict
+        self.worker.figure_dict = {}
+        self.request_command.emit(cmd, reply)
+
     def stop(self):
         self.worker_thread.quit()
         self.worker_thread.wait()
```

### Comparing `srsgui-0.4.3/srsgui/ui/commandterminal.py` & `srsgui-0.4.4/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.4.4/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.4.4/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/connectdlg.py` & `srsgui-0.4.4/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/deviceinfohandler.py` & `srsgui-0.4.4/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/dockhandler.py` & `srsgui-0.4.4/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/inputpanel.py` & `srsgui-0.4.4/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/qt/QtCore.py` & `srsgui-0.4.4/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/qt/QtGui.py` & `srsgui-0.4.4/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.4.4/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/qt/__init__.py` & `srsgui-0.4.4/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/qtloghandler.py` & `srsgui-0.4.4/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/resource_rc.py` & `srsgui-0.4.4/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/signalhandler.py` & `srsgui-0.4.4/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/srslogo.jpg` & `srsgui-0.4.4/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/stdout.py` & `srsgui-0.4.4/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/taskmain.py` & `srsgui-0.4.4/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/taskmain.ui` & `srsgui-0.4.4/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui/ui/ui_taskmain.py` & `srsgui-0.4.4/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.3/srsgui.egg-info/PKG-INFO` & `srsgui-0.4.4/srsgui.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.3
+Version: 0.4.4
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
@@ -15,17 +15,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pyserial>=3
 Provides-Extra: full
+Requires-Dist: matplotlib>=3.6.2; extra == "full"
+Requires-Dist: pyside6; extra == "full"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: matplotlib; extra == "docs"
+Requires-Dist: pyside2; extra == "docs"
+Requires-Dist: sphinx>=5; extra == "docs"
+Requires-Dist: sphinx-rtd-theme>=1; extra == "docs"
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication, based on the 
      [`Instrument`](https://thinksrs.github.io/srsgui/srsgui.inst.html#module-srsgui.inst.instrument)
```

### Comparing `srsgui-0.4.3/srsgui.egg-info/SOURCES.txt` & `srsgui-0.4.4/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

