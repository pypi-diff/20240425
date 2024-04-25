# Comparing `tmp/QEasyWidgets-0.1.3.tar.gz` & `tmp/QEasyWidgets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QEasyWidgets-0.1.3.tar", last modified: Mon Apr 15 23:59:50 2024, max compression
+gzip compressed data, was "QEasyWidgets-0.1.5.tar", last modified: Thu Apr 25 13:35:13 2024, max compression
```

## Comparing `QEasyWidgets-0.1.3.tar` & `QEasyWidgets-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:50.972901 QEasyWidgets-0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       82 2024-04-05 05:40:53.000000 QEasyWidgets-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1759 2024-04-15 23:59:50.972901 QEasyWidgets-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:50.962900 QEasyWidgets-0.1.3/QEasyWidgets/
--rw-rw-rw-   0        0        0    16537 2024-04-13 13:23:45.000000 QEasyWidgets-0.1.3/QEasyWidgets/ComponentsCustomizer.py
--rw-rw-rw-   0        0        0     9386 2024-04-12 10:21:49.000000 QEasyWidgets-0.1.3/QEasyWidgets/QFunctions.py
--rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.3/QEasyWidgets/QTasks.py
--rw-rw-rw-   0        0        0   208088 2024-04-15 13:27:01.000000 QEasyWidgets-0.1.3/QEasyWidgets/Sources.py
--rw-rw-rw-   0        0        0    27436 2024-04-11 01:50:15.000000 QEasyWidgets-0.1.3/QEasyWidgets/Utils.py
--rw-rw-rw-   0        0        0    23215 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.3/QEasyWidgets/WindowCustomizer.py
--rw-rw-rw-   0        0        0       22 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.3/QEasyWidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:50.970902 QEasyWidgets-0.1.3/QEasyWidgets.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-04-15 23:59:50.000000 QEasyWidgets-0.1.3/QEasyWidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-04-15 23:59:50.000000 QEasyWidgets-0.1.3/QEasyWidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 23:59:50.000000 QEasyWidgets-0.1.3/QEasyWidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-15 23:59:50.000000 QEasyWidgets-0.1.3/QEasyWidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-15 23:59:50.000000 QEasyWidgets-0.1.3/QEasyWidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:06.000000 QEasyWidgets-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 23:59:50.972901 QEasyWidgets-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1570 2024-04-15 13:32:40.000000 QEasyWidgets-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:35:13.480997 QEasyWidgets-0.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       82 2024-04-05 05:40:53.000000 QEasyWidgets-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-04-25 13:35:13.480997 QEasyWidgets-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 13:35:13.375997 QEasyWidgets-0.1.5/QEasyWidgets/
+-rw-rw-rw-   0        0        0    17410 2024-04-25 13:32:13.000000 QEasyWidgets-0.1.5/QEasyWidgets/ComponentsCustomizer.py
+-rw-rw-rw-   0        0        0    11971 2024-04-25 13:31:08.000000 QEasyWidgets-0.1.5/QEasyWidgets/QFunctions.py
+-rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.5/QEasyWidgets/QTasks.py
+-rw-rw-rw-   0        0        0    64535 2024-04-25 12:03:24.000000 QEasyWidgets-0.1.5/QEasyWidgets/Sources.py
+-rw-rw-rw-   0        0        0    27496 2024-04-22 03:22:31.000000 QEasyWidgets-0.1.5/QEasyWidgets/Utils.py
+-rw-rw-rw-   0        0        0    22730 2024-04-24 13:50:51.000000 QEasyWidgets-0.1.5/QEasyWidgets/WindowCustomizer.py
+-rw-rw-rw-   0        0        0       22 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.5/QEasyWidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:35:13.478994 QEasyWidgets-0.1.5/QEasyWidgets.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-04-25 13:35:13.000000 QEasyWidgets-0.1.5/QEasyWidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-04-25 13:35:13.000000 QEasyWidgets-0.1.5/QEasyWidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 13:35:13.000000 QEasyWidgets-0.1.5/QEasyWidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-25 13:35:13.000000 QEasyWidgets-0.1.5/QEasyWidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-25 13:35:13.000000 QEasyWidgets-0.1.5/QEasyWidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:06.000000 QEasyWidgets-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 13:35:13.481998 QEasyWidgets-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2024-04-25 13:30:19.000000 QEasyWidgets-0.1.5/setup.py
```

### Comparing `QEasyWidgets-0.1.3/LICENSE` & `QEasyWidgets-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.3/PKG-INFO` & `QEasyWidgets-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.3
+Version: 0.1.5
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
```

### Comparing `QEasyWidgets-0.1.3/QEasyWidgets/ComponentsCustomizer.py` & `QEasyWidgets-0.1.5/QEasyWidgets/ComponentsCustomizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,117 +8,173 @@
 
 ##############################################################################################################################
 
 class ButtonBase(QPushButton):
     '''
     '''
     def __init__(self,
-        text: Optional[str] = None,
         parent: Optional[QWidget] = None
     ):
         super().__init__(parent)
 
-        self.setFont('Microsoft YaHei')
-        self.setText(text) if text is not None else None
+        self.setIconSize(QSize(16, 16))
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        Function_SetFont(self)
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Button', Theme))
+        StyleSheetBase.Button.Apply(self)
+
+    def setIcon(self, icon: Optional[Union[QIcon, QPixmap, IconBase]]) -> None:
+        if icon is not None:
+            super().setProperty('hasIcon', True)
+            self._icon = icon
+        else:
+            super().setProperty('hasIcon', False)
+            self._icon = QIcon()
+        super().setStyle(QApplication.style())
+
+    def _drawIcon(self, icon, painter, rect):
+        Function_DrawIcon(icon, painter, rect)
+
+    def paintEvent(self, e: QPaintEvent) -> None:
+        super().paintEvent(e)
+        Width, Height = self.iconSize().width(), self.iconSize().height()
+        #MinWidth, MinHeight = self.minimumSizeHint().width(), self.minimumSizeHint().height()
+        LeftX = (self.width() - Width) /2
+        TopY = (self.height() - Height) / 2
+        Painter = QPainter(self)
+        Painter.setRenderHints(QPainter.Antialiasing | QPainter.SmoothPixmapTransform)
+        self._drawIcon(self._icon, Painter, QRectF(LeftX, TopY, Width, Height))
 
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Button.Deregistrate(self)
+
+
+class MenuButton(ButtonBase):
+    '''
+    '''
+    def __init__(self,
+        parent: Optional[QWidget] = None
+    ):
+        super().__init__(parent)
 
+        self.setIcon(IconBase.Ellipsis)
+
+    def setMenu(self, menu: QMenu) -> None:
+        def ShowMenu():
+            MenuWidth = menu.sizeHint().width()
+            XPos = MenuWidth - self.width()
+            YPos = self.height()
+            menu.exec(self.mapToGlobal(QPoint(XPos, YPos)))
+        self.clicked.connect(ShowMenu)
+
+    def SetMenu(self, ActionEvents: dict) -> None:
+        Menu = QMenu(self)
+        for Action in ActionEvents.keys():
+            if not isinstance(Action, str):
+                continue
+            MenuAction = QAction(text = Action, parent = self)
+            MenuAction.triggered.connect(ActionEvents.get(Action))
+            Menu.addAction(MenuAction)
+            #Menu.addSeparator()
+        self.setMenu(Menu)
+
+##############################################################################################################################
 
 class SpinBoxBase(QSpinBox):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
         super().__init__(parent)
 
         self.setFocusPolicy(Qt.StrongFocus)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.SpinBox.Apply(self)
 
     def wheelEvent(self, event: QWheelEvent) -> None:
         event.ignore()
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('SpinBox', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.SpinBox.Deregistrate(self)
 
 
 class DoubleSpinBoxBase(QDoubleSpinBox):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
         super().__init__(parent)
 
         self.setFocusPolicy(Qt.StrongFocus)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.SpinBox.Apply(self)
 
     def wheelEvent(self, event: QWheelEvent) -> None:
         event.ignore()
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('SpinBox', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.SpinBox.Deregistrate(self)
 
+##############################################################################################################################
 
 class ComboBoxBase(QComboBox):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
         super().__init__(parent)
 
         self.setFocusPolicy(Qt.StrongFocus)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.ComboBox.Apply(self)
 
     def wheelEvent(self, event: QWheelEvent) -> None:
         event.ignore()
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('ComboBox', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.ComboBox.Deregistrate(self)
 
+##############################################################################################################################
 
 class ScrollAreaBase(QScrollArea):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
         super().__init__(parent)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.ScrollArea.Apply(self)
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('ScrollArea', Theme))
+    def ClearDefaultStyleSheet(self) -> None:
+        StyleSheetBase.ScrollArea.Deregistrate(self)
+
+##############################################################################################################################
+
+class LabelBase(QLabel):
+    '''
+    '''
+    Resized = Signal()
+
+    def __init__(self,
+        parent: Optional[QWidget] = None
+    ):
+        super().__init__(parent)
+
+        StyleSheetBase.Label.Apply(self)
+
+    def resizeEvent(self, event: QResizeEvent) -> None:
+        self.Resized.emit()
+        super().resizeEvent(event)
 
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Label.Deregistrate(self)
 
 ##############################################################################################################################
 
 class TableBase(QTableView):
     '''
     '''
     sorted = Signal()
@@ -150,16 +206,15 @@
         self.model().rowsInserted.connect(self.SetIndex)
         self.model().rowsRemoved.connect(self.SetIndex)
         self.sorted.connect(self.SetIndex)
 
         self.IsIndexShown = False
         self.SetIndexHeaderVisible(True)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.Table.Apply(self)
 
     def model(self) -> QStandardItemModel:
         return self.StandardItemModel
 
     def currentRow(self) -> int:
         return super().currentIndex().row()
 
@@ -256,19 +311,16 @@
     def DelRow(self) -> None:
         self.removeRow(self.currentRow()) if self.rowCount() > 1 else None
 
     def ClearRows(self):
         while self.rowCount() > 0:
             self.removeRow(0)
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Table', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Table.Deregistrate(self)
 
 ##############################################################################################################################
 
 class LineEditBase(QFrame):
     '''
     '''
     textChanged = Signal(str)
@@ -286,16 +338,15 @@
 
         HBoxLayout = QHBoxLayout(self)
         HBoxLayout.setSpacing(0)
         HBoxLayout.setContentsMargins(0, 0, 0, 0)
         HBoxLayout.addWidget(self.LineEdit)
         HBoxLayout.addWidget(self.Button, alignment = Qt.AlignRight)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.Edit.Apply(self)
 
         self.Mask = QLabel(self)
         self.rectChanged.connect(self.Mask.setGeometry)
         self.Mask.setStyleSheet('background-color: rgba(0, 0, 0, 111);')
         self.Mask.setAlignment(Qt.AlignCenter)
         self.Mask.hide()
 
@@ -341,19 +392,16 @@
         )
         self.Button.setToolTip(ButtonTooltip)
 
     def RemoveFileDialogButton(self):
         self.Button.deleteLater()
         self.Button.hide()
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Edit', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Edit.Deregistrate(self)
 
     def Alert(self, Enable: bool, MaskContent: Optional[str] = None) -> None:
         AlertStyle = 'LineEditBase {border-color: red;}'
         self.setStyleSheet((self.styleSheet() + AlertStyle) if Enable else self.styleSheet().replace(AlertStyle, ''))
         self.Mask.setText(MaskContent) if MaskContent is not None else None
         self.Mask.show() if Enable else self.Mask.hide()
 
@@ -388,16 +436,15 @@
         HBoxLayout.addWidget(self.Slider, stretch = 5)
 
         AudioOutput = QAudioOutput(self)
         self.MediaPlayer = QMediaPlayer()
         self.MediaPlayer.setAudioOutput(AudioOutput)
         #self.MediaPlayer.mediaStatusChanged.connect(lambda Status: self.MediaPlayer.stop() if Status == QMediaPlayer.EndOfMedia else None)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.Player.Apply(self)
 
     def SetMediaPlayer(self, MediaPath: str):
         self.MediaPlayer.setSource(QUrl.fromLocalFile(MediaPath))
 
         self.PlayButton.clicked.connect(self.MediaPlayer.play)
         self.PauseButton.clicked.connect(self.MediaPlayer.pause)
         self.MediaPlayer.mediaStatusChanged.connect(lambda status: self.StackedWidget.setCurrentWidget(self.PlayButton) if status == QMediaPlayer.EndOfMedia else None)
@@ -407,14 +454,11 @@
         self.MediaPlayer.positionChanged.connect(lambda Position: self.Slider.setValue(int(Position / self.MediaPlayer.duration() * 100)))
 
     def ReleaseMediaPlayer(self):
         self.MediaPlayer.stop()
         self.MediaPlayer.setSource('')
         #self.MediaPlayer.deleteLater()
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Player', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Player.Deregistrate(self)
 
 ##############################################################################################################################
```

### Comparing `QEasyWidgets-0.1.3/QEasyWidgets/QFunctions.py` & `QEasyWidgets-0.1.5/QEasyWidgets/QFunctions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
 import darkdetect
+from enum import Enum
 from typing import Union, Optional
 from ctypes import c_int, byref, windll
 from PySide6.QtCore import Qt, QObject, QFile, QRect, QRectF, QSize, Signal, Slot, QPropertyAnimation, QParallelAnimationGroup, QEasingCurve, QUrl
-from PySide6.QtGui import QGuiApplication, QColor, QRgba64, QIcon, QPainter, QDesktopServices
+from PySide6.QtGui import QGuiApplication, QColor, QRgba64, QIcon, QIconEngine, QPainter, QFont, QDesktopServices
+from PySide6.QtSvg import QSvgRenderer
+from PySide6.QtXml import QDomDocument
 from PySide6.QtWidgets import *
 
 from .Utils import *
 from .Sources import *
 
 ##############################################################################################################################
 
@@ -22,68 +25,148 @@
     Signal_ClickedButton = Signal(QMessageBox.StandardButton)
     '''
 
 ComponentsSignals = CustomSignals_ComponentsCustomizer()
 
 ##############################################################################################################################
 
-def Function_GetStyleSheet(
-    Widget: str,
-    Theme: Optional[str] = None
-):
+class Theme:
+    '''
     '''
-    Get style sheet
+    Dark = 'Dark'
+    Light = 'Light'
 
-    Parameters
-    ----------
+    Auto = darkdetect.theme()
 
-    Widget: str
-        Name of widget (base)
 
-    Theme: str | None
-        Type of theme
+class ThemeBase:
+    '''
     '''
-    QApplication.processEvents()
+    THEME = Theme.Auto if Theme.Auto is not None else Theme.Dark
 
-    if Theme not in ('Dark', 'Light'):
-        SysTheme = darkdetect.theme()
-        Theme = SysTheme if SysTheme is not None else 'Dark'
+    def Update(self, theme: str):
+        if theme in (Theme.Dark, Theme.Light):
+            self.THEME = theme
 
-    Prefix = 'QSS'
-    FilePath = f'QSS/{Theme}/{Widget}.qss'
-    File = QFile(Path(f':/{Prefix}').joinpath(FilePath))
-    File.open(QFile.ReadOnly | QFile.Text)
-    QSS = str(File.readAll(), encoding = 'utf-8')
-    File.close()
 
-    return QSS
+EasyTheme = ThemeBase()
 
+##############################################################################################################################
 
-def Function_DrawIcon(
-    Icon: Union[str, QIcon],
-    Painter: QPainter,
-    Rect: Union[QRect, QRectF]
+RegistratedWidgets = {}
+
+
+class StyleSheetBase(Enum):
+    '''
+    '''
+    Label = 'Label'
+    ScrollArea = 'ScrollArea'
+    Button = 'Button'
+    SpinBox = 'SpinBox'
+    ComboBox = 'ComboBox'
+    Edit = 'Edit'
+    Player = 'Player'
+    Table = 'Table'
+
+    Bar = 'Bar'
+    Window = 'Window'
+    Dialog = 'Dialog'
+
+    def Path(self):
+        Path = f'QSS/{EasyTheme.THEME}/{self.value}.qss'
+        return Path
+    def Path(self):
+        return
+
+    def Registrate(self, widget, value):
+        RegistratedWidgets[widget] = value
+
+    def Deregistrate(self, widget):
+        RegistratedWidgets.pop(widget)
+
+    def Apply(self, widget: QWidget, theme: Optional[str] = None, registrate: bool = True):
+        QApplication.processEvents()
+
+        EasyTheme.Update(theme) if theme is not None else None
+
+        Prefix = 'QSS'
+        FilePath = f'QSS/{EasyTheme.THEME}/{self.value}.qss'
+        File = QFile(Path(f':/{Prefix}').joinpath(FilePath))
+        File.open(QFile.ReadOnly | QFile.Text)
+        QSS = str(File.readAll(), encoding = 'utf-8')
+        File.close()
+
+        widget.setStyleSheet(QSS)
+
+        self.Registrate(widget, self.value) if registrate else None
+
+
+def Function_UpdateStyleSheet(
+    theme: Optional[str] = None
 ):
     '''
-    Draw icon
+    '''
+    for Widget, value in list(RegistratedWidgets.items()):
+        for Value in StyleSheetBase:
+            if Value.value != value:
+                continue
+            try:
+                Value.Apply(Widget, theme)
+            except RuntimeError:
+                Value.Deregistrate(Widget)
+            finally:
+                continue
+
+
+ComponentsSignals.Signal_SetTheme.connect(Function_UpdateStyleSheet)
+
+##############################################################################################################################
 
-    Parameters
-    ----------
+class IconBase(Enum):
+    '''
+    '''
+    Ellipsis = 'Ellipsis'
 
-    Icon: str | QIcon
-        the icon to be drawn
+    def paint(self, painter: QPainter, rect: Union[QRect, QRectF], theme: Optional[str] = None):
+        Prefix = 'Icons'
+        IconPath = f'Icons/{theme if theme is not None else EasyTheme.THEME}/{self.value}.svg'
+        IconPath = Path(f':/{Prefix}').joinpath(IconPath).as_posix()
+        Renderer = QSvgRenderer(IconPath)
+        Renderer.render(painter, QRectF(rect))
 
-    Painter: QPainter
-        painter
 
-    Rect: QRect | QRectF
-        the rect to render icon
+def Function_DrawIcon(
+    icon: Union[str, QIcon],
+    painter: QPainter,
+    rect: Union[QRect, QRectF]
+):
+    '''
+    Draw icon
+    '''
+    if isinstance(icon, IconBase):
+        icon.paint(painter, rect, EasyTheme.THEME)
+    else:
+        icon = QIcon(icon)
+        icon.paint(painter, QRectF(rect).toRect(), Qt.AlignCenter, state = QIcon.Off)
+
+##############################################################################################################################
+
+def Function_SetFont(
+    Widget: QWidget,
+    FontSize:int = 12,
+    Weight = QFont.Normal
+):
+    '''
+    Set the font of widget
     '''
-    icon = QIcon(Icon)
-    icon.paint(Painter, QRectF(Rect).toRect(), Qt.AlignCenter, state = QIcon.Off)
+    Font = QFont()
+    Font.setFamilies(['Microsoft YaHei'])
+    Font.setPixelSize(FontSize)
+    Font.setWeight(Weight)
+    Widget.setFont(Font)
 
 ##############################################################################################################################
 
 def Function_SetRetainSizeWhenHidden(
     Widget: QWidget,
     RetainSize: bool = True
 ):
```

### Comparing `QEasyWidgets-0.1.3/QEasyWidgets/QTasks.py` & `QEasyWidgets-0.1.5/QEasyWidgets/QTasks.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.3/QEasyWidgets/Utils.py` & `QEasyWidgets-0.1.5/QEasyWidgets/Utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import win32gui
 import win32con
 import win32api
 import win32print
 import configparser
 from pathlib import Path
 from github import Github
+from packaging import version
 from tqdm import tqdm
 from typing import Tuple, Union, Optional
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from threading import currentThread
 from ctypes import windll
 
 #############################################################################################################
@@ -637,15 +638,15 @@
     try:
         PersonalGit = Github(AccessToken)
         Repo = PersonalGit.get_repo(f"{RepoOwner}/{RepoName}")
         Version_Latest = Repo.get_tags()[0].name
         LatestRelease = Repo.get_latest_release() #LatestRelease = Repo.get_release(Version_Latest)
         for Index, Asset in enumerate(LatestRelease.assets):
             if Asset.name == f"{FileName}.{FileFormat}":
-                IsUpdateNeeded = True if Version_Current != Version_Latest else False
+                IsUpdateNeeded = True if version.parse(Version_Current) < version.parse(Version_Latest) else False
                 DownloadURL = Asset.browser_download_url #DownloadURL = f"https://github.com/{RepoOwner}/{RepoName}/releases/download/{Version_Latest}/{FileName}.{FileFormat}"
                 return IsUpdateNeeded, DownloadURL
             elif Index + 1 == len(LatestRelease.assets):
                 raise Exception(f"No file found with name {FileName}.{FileFormat} in the latest release")
 
     except Exception as e:
         print(f"Error occurred while checking for updates: \n{e}")
```

### Comparing `QEasyWidgets-0.1.3/QEasyWidgets/WindowCustomizer.py` & `QEasyWidgets-0.1.5/QEasyWidgets/WindowCustomizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         self.HBoxLayout.setContentsMargins(0, 0, 0, 0)
         self.HBoxLayout.setSpacing(0)
         self.HBoxLayout.addStretch(1)
         self.HBoxLayout.addWidget(self.MinimizeButton, stretch = 0, alignment = Qt.AlignRight)
         self.HBoxLayout.addWidget(self.MaximizeButton, stretch = 0, alignment = Qt.AlignRight)
         self.HBoxLayout.addWidget(self.CloseButton, stretch = 0, alignment = Qt.AlignRight)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet) if self.isVisible() else None
-        self.InitDefaultStyleSheet('Auto')
+        StyleSheetBase.Bar.Apply(self)
 
     '''
     def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
         if 0 < event.position().y() < self.height() and event.buttons() == Qt.MouseButton.LeftButton:
             self.setMaximizeEvent()
     '''
 
@@ -65,15 +64,15 @@
         self.Window.showMinimized()
 
     def setCloseButton(self, parent):
         CloseButton = QPushButton("", parent)
         CloseButton.setSizePolicy(QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding))
         CloseButton.setStyleSheet(
             "QPushButton {"
-            "   image: url(:/Button_Icon/Sources/X.png);"
+            "   image: url(:/Button_Icon/Icons/X.png);"
             "   background-color: transparent;"
             "   padding: 6.6px;"
             "   border-width: 0px;"
             "}"
             "QPushButton:hover {"
             "   background-color: rgba(210, 123, 123, 210);"
             "}"
@@ -82,15 +81,15 @@
         return CloseButton
 
     def setMaximizeButton(self, parent):
         MaximizeButton = QPushButton("", parent)
         MaximizeButton.setSizePolicy(QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding))
         MaximizeButton.setStyleSheet(
             "QPushButton {"
-            "   image: url(:/Button_Icon/Sources/FullScreen.png);"
+            "   image: url(:/Button_Icon/Icons/FullScreen.png);"
             "   background-color: transparent;"
             "   padding: 6.6px;"
             "   border-width: 0px;"
             "}"
             "QPushButton:hover {"
             "   background-color: rgba(123, 123, 123, 123);"
             "}"
@@ -99,15 +98,15 @@
         return MaximizeButton
 
     def setMinimizeButton(self, parent):
         MinimizeButton = QPushButton("", parent)
         MinimizeButton.setSizePolicy(QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding))
         MinimizeButton.setStyleSheet(
             "QPushButton {"
-            "   image: url(:/Button_Icon/Sources/Dash.png);"
+            "   image: url(:/Button_Icon/Icons/Dash.png);"
             "   background-color: transparent;"
             "   padding: 6.6px;"
             "   border-width: 0px;"
             "}"
             "QPushButton:hover {"
             "   background-color: rgba(123, 123, 123, 123);"
             "}"
@@ -126,19 +125,16 @@
             "   border-width: 0px;"
             "   border-style: solid;"
             "}"
         )
         #TitleLabel.setFont(QFont("Microsoft YaHei", 11.1, QFont.Normal))
         TitleLabel.setAlignment(Qt.AlignLeft | Qt.AlignVCenter)
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Bar', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Bar.Deregistrate(self)
 
 ##############################################################################################################################
 
 class MARGINS(Structure):
     '''
     typedef struct _MARGINS {
         int cxLeftWidth;
@@ -330,17 +326,15 @@
             ExtendFrameIntoClientArea.argtypes = [c_int, PMARGINS]
             ExtendFrameIntoClientArea(hWnd, byref(MARGINS(-1, -1, -1, -1)))
 
     def setTitleBar(self, TitleBar: Optional[QWidget]) -> None:
         try:
             self.TitleBar.deleteLater()
             self.TitleBar.hide()
-            ComponentsSignals.Signal_SetTheme.disconnect(
-                lambda Theme: self.TitleBar.setStyleSheet(Function_GetStyleSheet('Bar', Theme))
-            )
+            StyleSheetBase.Bar.Deregistrate(self.TitleBar)
         except:
             pass
         if TitleBar is not None:
             self.TitleBar = TitleBar
             self.TitleBar.setParent(self) if self.TitleBar.parent() is None else None
             self.TitleBar.raise_() if self.TitleBar.isHidden() else None
 
@@ -369,16 +363,16 @@
         self.setFrameless()
 
         self.CentralLayout = QGridLayout()
         self.CentralWidget = QWidget(self)
         self.CentralWidget.setObjectName('CentralWidget')
         self.CentralWidget.setLayout(self.CentralLayout)
         self.setCentralWidget(self.CentralWidget)
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
+
+        StyleSheetBase.Window.Apply(self)
 
     def setCentralWidget(self, CentralWidget: Optional[QWidget]) -> None:
         try:
             super().takeCentralWidget(self.CentralWidget)
             self.CentralWidget.deleteLater()
             self.CentralWidget.hide()
             self.ClearDefaultStyleSheet()
@@ -386,19 +380,19 @@
             pass
         if CentralWidget is not None:
             self.CentralWidget = CentralWidget
             super().setCentralWidget(self.CentralWidget)
             self.CentralWidget.setParent(self) if self.CentralWidget.parent() is None else None
             self.CentralWidget.raise_() if self.CentralWidget.isHidden() else None
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Window', Theme).replace('#CentralWidget', f'#{self.CentralWidget.objectName()}'))
+    def setStyleSheet(self, styleSheet: str) -> None:
+        super().setStyleSheet(styleSheet.replace('#CentralWidget', f'#{self.CentralWidget.objectName()}'))
 
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Window.Deregistrate(self)
 
 
 class ChildWindowBase(WindowBase, QWidget):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None,
@@ -414,24 +408,32 @@
         self.setWindowModality(Qt.ApplicationModal)
 
         self.EventLoop = QEventLoop(self)
 
         self.showed.connect(lambda: parent.ShowMask(True)) if isinstance(parent, WindowBase) else None
         self.closed.connect(lambda: parent.ShowMask(False)) if isinstance(parent, WindowBase) else None
 
+        StyleSheetBase.Window.Apply(self)
+
     def exec(self) -> int:
         self.show()
         Result = self.EventLoop.exec()
         self.closed.emit()
         return Result
 
     def closeEvent(self, event: QCloseEvent) -> None:
         Result = self.EventLoop.exit()
         super().closeEvent(event)
 
+    def setStyleSheet(self, styleSheet: str) -> None:
+        super().setStyleSheet(styleSheet.replace('#CentralWidget', f'#{self.objectName()}'))
+
+    def ClearDefaultStyleSheet(self) -> None:
+        StyleSheetBase.Window.Deregistrate(self)
+
 
 class DialogBase(WindowBase, QDialog):
     '''
     '''
     def __init__(self,
         parent: Optional[QWidget] = None,
         f: Qt.WindowType = Qt.Dialog,
@@ -439,38 +441,34 @@
         min_height: int = 420
     ):
         QDialog.__init__(self, None, f) #QDialog.__init__(self, parent, f)
         WindowBase.__init__(self, min_width, min_height)
 
         self.setFrameless(SetStrechable = False)
 
-        ComponentsSignals.Signal_SetTheme.connect(self.InitDefaultStyleSheet)
-        self.InitDefaultStyleSheet('Auto')
-
         self.TitleBar.MinimizeButton.hide()
         self.TitleBar.MinimizeButton.deleteLater()
         self.TitleBar.MaximizeButton.hide()
         self.TitleBar.MaximizeButton.deleteLater()
 
         self.showed.connect(lambda: parent.ShowMask(True)) if isinstance(parent, WindowBase) else None
         self.closed.connect(lambda: parent.ShowMask(False)) if isinstance(parent, WindowBase) else None
 
+        StyleSheetBase.Dialog.Apply(self)
+
     def exec(self) -> int:
         Result = super().exec()
         self.closed.emit()
         return Result
 
     def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
         return
 
-    def InitDefaultStyleSheet(self, Theme: str) -> None:
-        super().setStyleSheet(Function_GetStyleSheet('Dialog', Theme))
-
     def ClearDefaultStyleSheet(self) -> None:
-        ComponentsSignals.Signal_SetTheme.disconnect(self.InitDefaultStyleSheet)
+        StyleSheetBase.Dialog.Deregistrate(self)
 
 ##############################################################################################################################
 
 class MessageBoxBase(DialogBase):
     '''
     '''
     ClickedButton = None
```

### Comparing `QEasyWidgets-0.1.3/QEasyWidgets.egg-info/PKG-INFO` & `QEasyWidgets-0.1.5/QEasyWidgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.3
+Version: 0.1.5
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
```

### Comparing `QEasyWidgets-0.1.3/README.md` & `QEasyWidgets-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.3/setup.py` & `QEasyWidgets-0.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('./README.md', encoding = 'utf-8') as f:
     LongDescription = f.read()
 
 ##############################################################################################################################
 
 setup(
     name = "QEasyWidgets",
-    version = '0.1.3',
+    version = '0.1.5',
     description = 'A simple widget library based on PySide6',
     long_description = LongDescription,
     long_description_content_type = 'text/markdown',
     license = 'GPLv3',
     author = "Spr_Aachen",
     author_email = '2835946988@qq.com',
     url = 'https://github.com/Spr-Aachen/QEasyWidgets',
```

