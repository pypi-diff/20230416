# Comparing `tmp/QtPy-Frameless-Window-0.0.9.tar.gz` & `tmp/QtPy-Frameless-Window-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.9.tar", last modified: Sat Apr 15 18:03:34 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.1.0.tar", last modified: Sun Apr 16 17:52:19 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.9.tar` & `QtPy-Frameless-Window-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.0.9/LICENSE
--rw-r--r--   0        0        0      812 2023-04-15 17:58:32.279110 QtPy-Frameless-Window-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.0.9/qt_api/__init__.py
--rw-r--r--   0        0        0      174 2023-04-15 17:29:48.930752 QtPy-Frameless-Window-0.0.9/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0     6143 2023-04-15 17:22:48.263396 QtPy-Frameless-Window-0.0.9/qtframelesswindow/buttons.py
--rw-r--r--   0        0        0     1747 2023-04-15 17:15:46.251860 QtPy-Frameless-Window-0.0.9/qtframelesswindow/manager.py
--rw-r--r--   0        0        0        0 2023-04-15 17:14:22.678018 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/__init__.py
--rw-r--r--   0        0        0      389 2023-04-15 05:44:35.457997 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/close.svg
--rw-r--r--   0        0        0      300 2023-04-15 05:44:35.526063 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/maximize.svg
--rw-r--r--   0        0        0      157 2023-04-15 05:44:35.461990 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/minimize.svg
--rw-r--r--   0        0        0      393 2023-04-15 05:44:35.461002 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/normalize.svg
--rw-r--r--   0        0        0      389 2023-04-15 05:45:07.996660 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/close.svg
--rw-r--r--   0        0        0      300 2023-04-15 05:45:07.996660 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/maximize.svg
--rw-r--r--   0        0        0      157 2023-04-15 05:45:08.057658 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/minimize.svg
--rw-r--r--   0        0        0      393 2023-04-15 05:45:07.987656 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/normalize.svg
--rw-r--r--   0        0        0      214 2023-04-15 09:26:53.084385 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/qss/button.qss
--rw-r--r--   0        0        0      222 2023-04-15 14:57:53.483029 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/qss/button_close.qss
--rw-r--r--   0        0        0     7069 2023-04-15 17:13:26.713324 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource.py
--rw-r--r--   0        0        0      479 2023-04-15 17:13:16.687205 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource.qrc
--rw-r--r--   0        0        0     7072 2023-04-15 18:02:59.241478 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource_rc.py
--rw-r--r--   0        0        0     7026 2023-04-15 17:32:36.258010 QtPy-Frameless-Window-0.0.9/qtframelesswindow/window.py
--rw-r--r--   0        0        0     1578 2023-04-15 18:02:09.368876 QtPy-Frameless-Window-0.0.9/README.md
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.1.0/LICENSE
+-rw-r--r--   0        0        0      812 2023-04-16 17:52:01.464663 QtPy-Frameless-Window-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.1.0/qt_api/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-15 17:29:48.930752 QtPy-Frameless-Window-0.1.0/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0     6143 2023-04-15 17:22:48.263396 QtPy-Frameless-Window-0.1.0/qtframelesswindow/buttons.py
+-rw-r--r--   0        0        0     1747 2023-04-15 17:15:46.251860 QtPy-Frameless-Window-0.1.0/qtframelesswindow/manager.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:14:22.678018 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-15 05:44:35.457997 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/black/close.svg
+-rw-r--r--   0        0        0      300 2023-04-15 05:44:35.526063 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/black/maximize.svg
+-rw-r--r--   0        0        0      157 2023-04-15 05:44:35.461990 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/black/minimize.svg
+-rw-r--r--   0        0        0      393 2023-04-15 05:44:35.461002 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/black/normalize.svg
+-rw-r--r--   0        0        0      389 2023-04-15 05:45:07.996660 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/white/close.svg
+-rw-r--r--   0        0        0      300 2023-04-15 05:45:07.996660 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/white/maximize.svg
+-rw-r--r--   0        0        0      157 2023-04-15 05:45:08.057658 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/white/minimize.svg
+-rw-r--r--   0        0        0      393 2023-04-15 05:45:07.987656 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/images/white/normalize.svg
+-rw-r--r--   0        0        0      214 2023-04-15 09:26:53.084385 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/qss/button.qss
+-rw-r--r--   0        0        0      222 2023-04-15 14:57:53.483029 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/qss/button_close.qss
+-rw-r--r--   0        0        0     7069 2023-04-15 17:13:26.713324 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/resource.py
+-rw-r--r--   0        0        0      479 2023-04-15 17:13:16.687205 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/resource.qrc
+-rw-r--r--   0        0        0     7072 2023-04-16 17:49:14.222635 QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/resource_rc.py
+-rw-r--r--   0        0        0     7111 2023-04-16 17:50:03.180230 QtPy-Frameless-Window-0.1.0/qtframelesswindow/window.py
+-rw-r--r--   0        0        0     1763 2023-04-15 18:12:30.624038 QtPy-Frameless-Window-0.1.0/README.md
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.1.0/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.9/LICENSE` & `QtPy-Frameless-Window-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.9/pyproject.toml` & `QtPy-Frameless-Window-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.7,<3.10"
-version = "0.0.9"
+version = "0.1.0"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.0.9/qtframelesswindow/buttons.py` & `QtPy-Frameless-Window-0.1.0/qtframelesswindow/buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.9/qtframelesswindow/manager.py` & `QtPy-Frameless-Window-0.1.0/qtframelesswindow/manager.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource.py` & `QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/resource.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource_rc.py` & `QtPy-Frameless-Window-0.1.0/qtframelesswindow/resource/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.9/qtframelesswindow/window.py` & `QtPy-Frameless-Window-0.1.0/qtframelesswindow/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,16 @@
         )
 
     def eventFilter(self, obj, event):
         # resize, refer to https://github.com/zhiyiYo/PyQt-Frameless-Window
         et = event.type()
         if et != QEvent.MouseButtonPress and et != QEvent.MouseMove:
             return False
+        if self.isMaximized():
+            return False
         edges = Qt.Edge(0)
         pos = event.globalPos() - self.pos()
         if pos.x() < BORDER:
             edges |= Qt.LeftEdge
         if pos.x() >= self.width() - BORDER:
             edges |= Qt.RightEdge
         if pos.y() < BORDER:
@@ -105,46 +107,48 @@
                 self.width() - (BORDER - i) * 2,
                 self.height() - (BORDER - i) * 2,
                 4,
                 4,
             )
 
     def __set_animation_toggle(self):
-        self.__w_normal = 800
-        self.__h_normal = 600
+        self.__record:QRect=None
         self.__animation_toggle = QPropertyAnimation(self, b"geometry")
-        self.__animation_toggle.setStartValue(
-            QRect(self.pos().x(), self.pos().y(), self.__w_normal, self.__h_normal)
-        )
-        self.__animation_toggle.setEndValue(self.get_screen())
+        self.__animation_toggle.setDuration(100)
+        
+    def show(self) -> None:
+        super().show()
+        self.__record=self.geometry()
+        
+    def resize(self,*args,**kwds):
+        super().resize(*args,**kwds)
 
-    def showMaximized(self,record=True) -> None:
-        if not self.isVisible():
-            self.show()
+    def showMaximized(self) -> None:
         self.titlebar.show()
         self.layout().setContentsMargins(*([0] * 4))
         self.set_border_radius(0)
-        if record:
-            self.__h_normal = self.height()
-            self.__w_normal = self.width()
-        self.__animation_toggle.setStartValue(
-            QRect(self.pos().x(), self.pos().y(), self.__w_normal, self.__h_normal)
-        )
+        if not self.isVisible():
+            self.setGeometry(self.get_screen())
+            return
+        if self.geometry().height()!=self.get_screen().height() or \
+            self.geometry().width()!=self.get_screen().width():
+            self.__record=self.geometry()
+        self.__animation_toggle.setStartValue(self.geometry())
         self.__animation_toggle.setEndValue(self.get_screen())
-        self.__animation_toggle.setDirection(QPropertyAnimation.Direction.Forward)
-        self.__animation_toggle.setDuration(100)
         self.__animation_toggle.start()
 
     def showNormal(self) -> None:
-        if not self.isVisible():
-            self.show()
         self.titlebar.show()
         self.layout().setContentsMargins(*([BORDER] * 4))
         self.set_border_radius(BORDER)
-        self.__animation_toggle.setDirection(QPropertyAnimation.Direction.Backward)
+        if not self.isVisible():
+            super().showNormal()
+            self.__record=self.geometry()
+        self.__animation_toggle.setStartValue(self.geometry())
+        self.__animation_toggle.setEndValue(self.__record)
         self.__animation_toggle.start()
         
     def showFullScreen(self) -> None:
         self.titlebar.hide()
         self.showMaximized()
 
     def isMaximized(self) -> bool:
@@ -174,8 +178,9 @@
         self.main_window=QMainWindow()
         
 class FramelessDialog(FramelessWindow):
     def __init__(self) -> None:
         super().__init__()
         self.main_window=QDialog()
         self.titlebar.buttons.minBtn.hide()
-        self.titlebar.buttons.toggleBtn.hide()
+        self.titlebar.buttons.toggleBtn.hide()
+        self.titlebar.buttons.setFixedWidth(45)
```

### Comparing `QtPy-Frameless-Window-0.0.9/README.md` & `QtPy-Frameless-Window-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -50,8 +50,12 @@
         if args.api is not None:
             api=args.api
     os.environ["QT_API"]=api
 ```
 
 ![light_demo](assets/light_demo.png)
 
-![dark_demo](assets/dark_demo.png)
+![dark_demo](assets/dark_demo.png)
+
+## Reference
+1. [PyQt-Frameless-Window](https://github.com/zhiyiYo/PyQt-Frameless-Window)
+2. [draw window shadow](https://blog.csdn.net/goforwardtostep/article/details/99549750)
```

### Comparing `QtPy-Frameless-Window-0.0.9/PKG-INFO` & `QtPy-Frameless-Window-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.9
+Version: 0.1.0
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -66,7 +66,12 @@
             api=args.api
     os.environ["QT_API"]=api
 ```
 
 ![light_demo](assets/light_demo.png)
 
 ![dark_demo](assets/dark_demo.png)
+
+## Reference
+1. [PyQt-Frameless-Window](https://github.com/zhiyiYo/PyQt-Frameless-Window)
+2. [draw window shadow](https://blog.csdn.net/goforwardtostep/article/details/99549750)
+
```

