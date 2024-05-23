# Comparing `tmp/audioalchemist-0.5.0.tar.gz` & `tmp/audioalchemist-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioalchemist-0.5.0.tar", last modified: Thu May 23 00:15:02 2024, max compression
+gzip compressed data, was "audioalchemist-0.5.5.tar", last modified: Thu May 23 00:54:52 2024, max compression
```

## Comparing `audioalchemist-0.5.0.tar` & `audioalchemist-0.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/
-drwxrwxrwx   0        0        0        0 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/AudioAlchemist/
--rw-rw-rw-   0        0        0       45 2024-05-23 00:11:59.000000 audioalchemist-0.5.0/AudioAlchemist/__init__.py
--rw-rw-rw-   0        0        0     2412 2024-05-22 14:10:21.000000 audioalchemist-0.5.0/AudioAlchemist/audio_alchemist.py
-drwxrwxrwx   0        0        0        0 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/AudioAlchemist.egg-info/
--rw-rw-rw-   0        0        0     2233 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2233 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1421 2024-05-23 00:14:45.000000 audioalchemist-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:54:52.264571 audioalchemist-0.5.5/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:54:52.248890 audioalchemist-0.5.5/AudioAlchemist/
+-rw-rw-rw-   0        0        0       45 2024-05-23 00:11:59.000000 audioalchemist-0.5.5/AudioAlchemist/__init__.py
+-rw-rw-rw-   0        0        0     2412 2024-05-22 14:10:21.000000 audioalchemist-0.5.5/AudioAlchemist/audio_alchemist.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:54:52.248890 audioalchemist-0.5.5/AudioAlchemist.egg-info/
+-rw-rw-rw-   0        0        0     3108 2024-05-23 00:54:52.000000 audioalchemist-0.5.5/AudioAlchemist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-23 00:54:52.000000 audioalchemist-0.5.5/AudioAlchemist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:54:52.000000 audioalchemist-0.5.5/AudioAlchemist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 00:54:52.000000 audioalchemist-0.5.5/AudioAlchemist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 00:54:52.000000 audioalchemist-0.5.5/AudioAlchemist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3108 2024-05-23 00:54:52.248890 audioalchemist-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:54:52.264571 audioalchemist-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2024-05-23 00:54:34.000000 audioalchemist-0.5.5/setup.py
```

### Comparing `audioalchemist-0.5.0/AudioAlchemist/audio_alchemist.py` & `audioalchemist-0.5.5/AudioAlchemist/audio_alchemist.py`

 * *Files identical despite different names*

### Comparing `audioalchemist-0.5.0/AudioAlchemist.egg-info/PKG-INFO` & `audioalchemist-0.5.5/AudioAlchemist.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.5.0
+Version: 0.5.5
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
 License: MIT
-Keywords: audio,pydub,glob,pandas,mp3,wav,flac,m4a
+Keywords: audio,pydub,glob,mp3,wav,flac,m4a,audio_convert,converter,audio_converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas>=2.2.2
 Requires-Dist: pydub>=0.25.1
 Requires-Dist: ffmpeg>=1.4
 
-## 概要
+# 概要
 
 音色変換は、Pydub を利用した音声変換ツールです。WAVやm4aを MP3 ファイルなどの形式に変換することができます。
 
-## 機能
+# 機能
 
 * WAVやm4aを MP3 ファイルなどの形式に変換する
 * 複数のファイルをまとめて変換する
 * 変換後のファイル名を連番で出力
+* 変換前のファイルはすべて残ります
 
 ## インストール
 
 ```
 pip3 install AudioAlchemist
 ```
 
 ## 使い方 example
+* ライブラリのインポート
+```
+import AudioAlchemist as aa
+```
+* 処理の設定
+* input_extansion="変換したいファイルの拡張子"（'.'はいりません）
+* output_extansion="変換後のファイルの拡張子の指定"（'.'はいりません）
+* input_forder="フォルダーの場所"
+* →一つのファイルの場合、パスを'C:/Users/data/melody/music.wav'のように完全に設定してください
+* →複数の場合、パスを'C:/Users/data/melody/*.wav'と*をつけるとフォルダーより下のすべてのファイルを変換します。
+* output_forder="排出先のフォルダー場所"
+* →このとき、排出先のフォルダーを新規で指定するとフォルダーが自動生成されます
 
+* プログラム例
 ```
 # フォルダパスを設定
 input_folder = 'C:/Users/data/melody/*.wav'
 output_folder = 'C:/Users/data/melody/'
 input_extension = "wav"
 output_extension = "mp3"
 
 # 変換処理を実行
 audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
 audio_alchemist.process_files()
 ```
 
 このコマンドは、`C:/Users/data/melody` フォルダ内のすべての WAV ファイルを MP3 ファイルに変換し、`C:/Users/data/melody` フォルダに出力します。
 
-## 注意
+# 変換後の注意
 
 * 変換するファイルが存在していることを確認してください。
 * 出力フォルダが存在していることを確認してください。
 * 入力ファイルと出力ファイルの拡張子が一致していることを確認してください。
 
-## サポート
+# サポート
 
-バグ報告や機能リクエストは、GitHub までご連絡ください。
+バグ報告や機能リクエストは、GitHubまたは、メールにてご連絡ください。
 
-## ライセンス
+# ライセンス
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
 ## バージョン
 
-0.5.0
+0.5.5
```

### Comparing `audioalchemist-0.5.0/PKG-INFO` & `audioalchemist-0.5.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.5.0
+Version: 0.5.5
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
 License: MIT
-Keywords: audio,pydub,glob,pandas,mp3,wav,flac,m4a
+Keywords: audio,pydub,glob,mp3,wav,flac,m4a,audio_convert,converter,audio_converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas>=2.2.2
 Requires-Dist: pydub>=0.25.1
 Requires-Dist: ffmpeg>=1.4
 
-## 概要
+# 概要
 
 音色変換は、Pydub を利用した音声変換ツールです。WAVやm4aを MP3 ファイルなどの形式に変換することができます。
 
-## 機能
+# 機能
 
 * WAVやm4aを MP3 ファイルなどの形式に変換する
 * 複数のファイルをまとめて変換する
 * 変換後のファイル名を連番で出力
+* 変換前のファイルはすべて残ります
 
 ## インストール
 
 ```
 pip3 install AudioAlchemist
 ```
 
 ## 使い方 example
+* ライブラリのインポート
+```
+import AudioAlchemist as aa
+```
+* 処理の設定
+* input_extansion="変換したいファイルの拡張子"（'.'はいりません）
+* output_extansion="変換後のファイルの拡張子の指定"（'.'はいりません）
+* input_forder="フォルダーの場所"
+* →一つのファイルの場合、パスを'C:/Users/data/melody/music.wav'のように完全に設定してください
+* →複数の場合、パスを'C:/Users/data/melody/*.wav'と*をつけるとフォルダーより下のすべてのファイルを変換します。
+* output_forder="排出先のフォルダー場所"
+* →このとき、排出先のフォルダーを新規で指定するとフォルダーが自動生成されます
 
+* プログラム例
 ```
 # フォルダパスを設定
 input_folder = 'C:/Users/data/melody/*.wav'
 output_folder = 'C:/Users/data/melody/'
 input_extension = "wav"
 output_extension = "mp3"
 
 # 変換処理を実行
 audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
 audio_alchemist.process_files()
 ```
 
 このコマンドは、`C:/Users/data/melody` フォルダ内のすべての WAV ファイルを MP3 ファイルに変換し、`C:/Users/data/melody` フォルダに出力します。
 
-## 注意
+# 変換後の注意
 
 * 変換するファイルが存在していることを確認してください。
 * 出力フォルダが存在していることを確認してください。
 * 入力ファイルと出力ファイルの拡張子が一致していることを確認してください。
 
-## サポート
+# サポート
 
-バグ報告や機能リクエストは、GitHub までご連絡ください。
+バグ報告や機能リクエストは、GitHubまたは、メールにてご連絡ください。
 
-## ライセンス
+# ライセンス
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
 ## バージョン
 
-0.5.0
+0.5.5
```

### Comparing `audioalchemist-0.5.0/setup.py` & `audioalchemist-0.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 DESCRIPTION = 'Convert all files directly under the directory to any music file.'
 NAME = 'AudioAlchemist'
 AUTHOR = 'Kohki Suto'
 AUTHOR_EMAIL = 's2222019@stu.musashino-u.ac.jp'
 URL = 'https://github.com/Ryomo0797/AudioAlchemist.git'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.5.0'
+VERSION = '0.5.5'
 PYTHON_REQUIRES = '>=3.6'
 INSTALL_REQUIRES = [
-    "pandas>=2.2.2",
     "pydub>=0.25.1",
     "ffmpeg>=1.4"
     #ffmpeg-python==0.2.0
 ]
 PACKAGES = [
     'AudioAlchemist'
 ]
-KEYWORDS = 'audio, pydub, glob, pandas, mp3, wav, flac, m4a'
+KEYWORDS = 'audio, pydub, glob, mp3, wav, flac, m4a, audio_convert, converter, audio_converter'
 CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6'
 ]
 with open('README.md', 'r', encoding='utf-8') as fp:
     readme = fp.read()
 LONG_DESCRIPTION = readme
```

