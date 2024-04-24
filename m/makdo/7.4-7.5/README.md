# Comparing `tmp/makdo-7.4.tar.gz` & `tmp/makdo-7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makdo-7.4.tar", last modified: Wed Apr  3 23:53:31 2024, max compression
+gzip compressed data, was "makdo-7.5.tar", last modified: Wed Apr 24 22:35:56 2024, max compression
```

## Comparing `makdo-7.4.tar` & `makdo-7.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwx------   0 say       (1000) say       (1000)        0 2024-04-03 23:53:31.155840 makdo-7.4/
--rw-------   0 say       (1000) say       (1000)    22533 2024-04-03 23:53:31.155840 makdo-7.4/PKG-INFO
--rw-------   0 say       (1000) say       (1000)    18501 2024-04-03 23:53:23.000000 makdo-7.4/README.txt
-drwx------   0 say       (1000) say       (1000)        0 2024-04-03 23:53:31.151840 makdo-7.4/makdo/
--rw-------   0 say       (1000) say       (1000)      137 2024-04-03 23:53:23.000000 makdo-7.4/makdo/__init__.py
--rwx------   0 say       (1000) say       (1000)   262582 2024-04-03 23:53:23.000000 makdo-7.4/makdo/makdo_docx2md.py
--rwx------   0 say       (1000) say       (1000)     4201 2024-04-03 23:53:23.000000 makdo-7.4/makdo/makdo_gui.py
--rwx------   0 say       (1000) say       (1000)   237761 2024-04-03 23:53:23.000000 makdo-7.4/makdo/makdo_md2docx.py
-drwx------   0 say       (1000) say       (1000)        0 2024-04-03 23:53:31.155840 makdo-7.4/makdo.egg-info/
--rw-------   0 say       (1000) say       (1000)    22533 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/PKG-INFO
--rw-------   0 say       (1000) say       (1000)      246 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/SOURCES.txt
--rw-------   0 say       (1000) say       (1000)        1 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/dependency_links.txt
--rw-------   0 say       (1000) say       (1000)       32 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/requires.txt
--rw-------   0 say       (1000) say       (1000)        6 2024-04-03 23:53:31.000000 makdo-7.4/makdo.egg-info/top_level.txt
--rw-------   0 say       (1000) say       (1000)       38 2024-04-03 23:53:31.155840 makdo-7.4/setup.cfg
--rw-------   0 say       (1000) say       (1000)      567 2024-04-03 23:53:23.000000 makdo-7.4/setup.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-24 22:35:56.419130 makdo-7.5/
+-rw-------   0 say       (1000) say       (1000)    35149 2024-04-24 22:35:35.000000 makdo-7.5/LICENSE
+-rw-------   0 say       (1000) say       (1000)    19384 2024-04-24 22:35:56.419130 makdo-7.5/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)    18997 2024-04-24 22:35:35.000000 makdo-7.5/README.txt
+drwx------   0 say       (1000) say       (1000)        0 2024-04-24 22:35:56.419130 makdo-7.5/makdo/
+-rw-------   0 say       (1000) say       (1000)      137 2024-04-24 22:35:35.000000 makdo-7.5/makdo/__init__.py
+-rwx------   0 say       (1000) say       (1000)   262582 2024-04-24 22:35:35.000000 makdo-7.5/makdo/makdo_docx2md.py
+-rwx------   0 say       (1000) say       (1000)     4201 2024-04-24 22:35:35.000000 makdo-7.5/makdo/makdo_gui.py
+-rwx------   0 say       (1000) say       (1000)   237761 2024-04-24 22:35:35.000000 makdo-7.5/makdo/makdo_md2docx.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-24 22:35:56.419130 makdo-7.5/makdo.egg-info/
+-rw-------   0 say       (1000) say       (1000)    19384 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)      254 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/SOURCES.txt
+-rw-------   0 say       (1000) say       (1000)        1 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/dependency_links.txt
+-rw-------   0 say       (1000) say       (1000)       32 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/requires.txt
+-rw-------   0 say       (1000) say       (1000)        6 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/top_level.txt
+-rw-------   0 say       (1000) say       (1000)       38 2024-04-24 22:35:56.419130 makdo-7.5/setup.cfg
+-rw-------   0 say       (1000) say       (1000)      567 2024-04-24 22:35:35.000000 makdo-7.5/setup.py
```

### Comparing `makdo-7.4/README.txt` & `makdo-7.5/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,34 @@
-<!-- Time-stamp:   <2024.04.03-09:00:13-JST> -->
+<!-- Time-stamp:   <2024.04.04-13:26:58-JST> -->
 
 # MAKDO（MS Wordの互換アプリ）
 
 ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
 
 〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
 
 〜〜 MS Wordがなくても、MS Word形式のファイルを読み書きできます 〜〜
 
 〜〜 わずらわしいナンバリング（番号付け）やインデント（字下げ）から、あなたを解放します 〜〜
 
 ## 注意事項
 
+### 簡易実行ファイルについて
+
+githubのレポジトリは、開発者向けです。
+
+一般の方は、下記のリンクから簡易実行ファイルをダウンロードして使ってください。
+
+[簡易実行ファイルのダウンロードページ](https://hata-o.jp/kian/index?tools#makdo)
+
+環境の設定やアプリのインストールが不要で使えます。
+
+※ 現在、macOSの開発環境がないため、macOS用の簡易実行ファイルはありません。
+macOSの方は`python`の設定が必要です。
+
 ### Python3について
 
 簡易実行ファイルは単独で実行できますので不要ですが、
 このアプリ（ライブラリ）は、Python3（Pythonのバージョン3）以上を想定しています。
 
 以下の説明では`python`という表記は、システムによっては`python3`等を意味する場合があります。
 
@@ -41,16 +54,15 @@
 
 とりあえず使いたい方のために、簡易実行ファイルを用意しました。
 
 簡易実行ファイルであれば、環境の設定やアプリのインストールが不要で、
 しかも、コマンドプロンプト（Windowsの場合）やターミナル（macOSの場合）上のコマンドではなく、
 マウスを使ってドラッグ＆ドロップで実行できます。
 
-とりあえず使いたい方は、下記にアクセスして、
-OSに合ったZIPファイルをダウンロードして、展開してください。
+下記にアクセスしてZIPファイルをダウンロードし、展開してください。
 
 [簡易実行ファイルのダウンロードページ](https://hata-o.jp/kian/index?tools#makdo)
 
 展開したフォルダの中に実行ファイル
 （Windowsの場合は`makdo_win.exe`、macOSの場合は`makdo_mac`。）があります。
 
 これを起動するとウィンドウが開きますので、そのウィンドウに、
```

### Comparing `makdo-7.4/makdo/makdo_docx2md.py` & `makdo-7.5/makdo/makdo_docx2md.py`

 * *Files identical despite different names*

### Comparing `makdo-7.4/makdo/makdo_gui.py` & `makdo-7.5/makdo/makdo_gui.py`

 * *Files identical despite different names*

### Comparing `makdo-7.4/makdo/makdo_md2docx.py` & `makdo-7.5/makdo/makdo_md2docx.py`

 * *Files identical despite different names*

### Comparing `makdo-7.4/setup.py` & `makdo-7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='makdo',
-    version='07.04',
+    version='07.05',
     description='日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Seiichiro HATA',
     author_email='hata48915b@post.nifty.jp',
     url='https://github.com/hata48915b/makdo/',
     license='GPLv3+',
```

