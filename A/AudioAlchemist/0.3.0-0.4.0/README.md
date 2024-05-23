# Comparing `tmp/audioalchemist-0.3.0.tar.gz` & `tmp/audioalchemist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioalchemist-0.3.0.tar", last modified: Wed May 22 13:54:07 2024, max compression
+gzip compressed data, was "audioalchemist-0.4.0.tar", last modified: Wed May 22 14:11:02 2024, max compression
```

## Comparing `audioalchemist-0.3.0.tar` & `audioalchemist-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/
-drwxrwxrwx   0        0        0        0 2024-05-22 13:54:07.030199 audioalchemist-0.3.0/AudioAlchemist/
--rw-rw-rw-   0        0        0       43 2024-05-22 12:04:05.000000 audioalchemist-0.3.0/AudioAlchemist/__int__.py
--rw-rw-rw-   0        0        0     2607 2024-05-22 13:52:00.000000 audioalchemist-0.3.0/AudioAlchemist/audio_alchemist.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/AudioAlchemist.egg-info/
--rw-rw-rw-   0        0        0     2308 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 13:54:06.000000 audioalchemist-0.3.0/AudioAlchemist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2308 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 13:54:07.045963 audioalchemist-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1421 2024-05-22 13:50:31.000000 audioalchemist-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/
+drwxrwxrwx   0        0        0        0 2024-05-22 14:11:02.394437 audioalchemist-0.4.0/AudioAlchemist/
+-rw-rw-rw-   0        0        0       43 2024-05-22 12:04:05.000000 audioalchemist-0.4.0/AudioAlchemist/__int__.py
+-rw-rw-rw-   0        0        0     2412 2024-05-22 14:10:21.000000 audioalchemist-0.4.0/AudioAlchemist/audio_alchemist.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/AudioAlchemist.egg-info/
+-rw-rw-rw-   0        0        0     2233 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2233 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2024-05-22 14:06:27.000000 audioalchemist-0.4.0/setup.py
```

### Comparing `audioalchemist-0.3.0/AudioAlchemist/audio_alchemist.py` & `audioalchemist-0.4.0/AudioAlchemist/audio_alchemist.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,60 +7,55 @@
 # for o in filelist:
 #   sourceAudio = AudioSegment.from_file(o,"wav")
 #   # 結果を出力
 #   i+=1
 #   audio="C:/Users/hikar/ds/data/melody/"+str(i)+".mp3"
 #   sourceAudio.export(audio, format="mp3")
 # print("処理が完了しました")
-
-import pydub
-import glob
-import pandas as pd
-
 # def AusioAlchemist(input_folder, output_folder, input_extension, output_extension):
 #   filelist = glob.glob(input_folder)
 #   i = 0
 #   # 各ファイルを読み込み、連番を追加して出力
 #   for file in filelist:
 #     source_audio = pydub.AudioSegment.from_file(file, input_extension)
 #     # 結果を出力
 #     output_file = output_folder + str(i) +"."+ output_extension
 #     source_audio.export(output_file, format=output_extension)
 #     i += 1
 #   print("処理が完了しました")
 
 import pydub
 import glob
-import pandas as pd
+# import pandas as pd
+
+class AudioAlchemist:
+    def __init__(self, input_folder, output_folder, input_extension, output_extension):
+        self.input_folder = input_folder
+        self.output_folder = output_folder
+        self.input_extension = input_extension
+        self.output_extension = output_extension
+
+    def process_files(self):
+        filelist = glob.glob(self.input_folder)
+        i = 0
+        # Each file is read and a serial number is added and output
+        for file in filelist:
+            source_audio = pydub.AudioSegment.from_file(file, self.input_extension)
+            # Output the result
+            output_file = self.output_folder + str(i) +"."+ self.output_extension
+            source_audio.export(output_file, format=self.output_extension)
+            i += 1
+        print("Processing completed")
+
+# Create an instance of the AudioAlchemist class and call the process_files method
+
+# # フォルダパスを設定
+# input_folder = 'C:/Users/hikar/ds/data/melody/*.wav'
+# output_folder = 'C:/Users/hikar/ds/data/melody/'
+# input_extension = "wav"
+# output_extension = "mp3"
 
-def AudioAlchemist(input_folder, output_folder, input_extension, output_extension):
-    class AudioAlchemist:
-        def __init__(self, input_folder, output_folder, input_extension, output_extension):
-            self.input_folder = input_folder
-            self.output_folder = output_folder
-            self.input_extension = input_extension
-            self.output_extension = output_extension
-
-        def process_files(self):
-            filelist = glob.glob(self.input_folder)
-            i = 0
-            # Each file is read and a serial number is added and output
-            for file in filelist:
-                source_audio = pydub.AudioSegment.from_file(file, self.input_extension)
-                # Output the result
-                output_file = self.output_folder + str(i) +"."+ self.output_extension
-                source_audio.export(output_file, format=self.output_extension)
-                i += 1
-            print("Processing completed")
-
-    # Create an instance of the AudioAlchemist class and call the process_files method
-    audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
-    audio_alchemist.process_files()
-
-# フォルダパスを設定
-input_folder = 'C:/Users/hikar/ds/data/melody/*.wav'
-output_folder = 'C:/Users/hikar/ds/data/melody/'
-input_extension = "wav"
-output_extension = "mp3"
+# audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
+# audio_alchemist.process_files()
 
-# 変換処理を実行
-AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
+# # 変換処理を実行
+# AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
```

### Comparing `audioalchemist-0.3.0/AudioAlchemist.egg-info/PKG-INFO` & `audioalchemist-0.4.0/AudioAlchemist.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.3.0
+Version: 0.4.0
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
@@ -13,59 +13,56 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: pydub>=0.25.1
 Requires-Dist: ffmpeg>=1.4
 
-## リードミーファイル
-
-**# 音色変換**
-
-**## 概要**
+## 概要
 
 音色変換は、Pydub を利用した音声変換ツールです。WAVやm4aを MP3 ファイルなどの形式に変換することができます。
 
-**## 機能**
+## 機能
 
 * WAVやm4aを MP3 ファイルなどの形式に変換する
 * 複数のファイルをまとめて変換する
 * 変換後のファイル名を連番で出力
 
-**## インストール**
+## インストール
 
 ```
 pip3 install AudioAlchemist
 ```
 
-**## 使い方 example**
+## 使い方 example
 
 ```
 # フォルダパスを設定
 input_folder = 'C:/Users/data/melody/*.wav'
 output_folder = 'C:/Users/data/melody/'
 input_extension = "wav"
 output_extension = "mp3"
 
 # 変換処理を実行
-AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
+audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
+audio_alchemist.process_files()
 ```
 
 このコマンドは、`C:/Users/data/melody` フォルダ内のすべての WAV ファイルを MP3 ファイルに変換し、`C:/Users/data/melody` フォルダに出力します。
 
-**## 注意**
+## 注意
 
 * 変換するファイルが存在していることを確認してください。
 * 出力フォルダが存在していることを確認してください。
 * 入力ファイルと出力ファイルの拡張子が一致していることを確認してください。
 
-**## サポート**
+## サポート
 
-バグ報告や機能リクエストは、GitHub [無効な URL を削除しました] までご連絡ください。
+バグ報告や機能リクエストは、GitHub までご連絡ください。
 
-**## ライセンス**
+## ライセンス
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
-**## バージョン**
+## バージョン
 
-0.3.0
+0.4.0
```

### Comparing `audioalchemist-0.3.0/PKG-INFO` & `audioalchemist-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.3.0
+Version: 0.4.0
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
@@ -13,59 +13,56 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: pydub>=0.25.1
 Requires-Dist: ffmpeg>=1.4
 
-## リードミーファイル
-
-**# 音色変換**
-
-**## 概要**
+## 概要
 
 音色変換は、Pydub を利用した音声変換ツールです。WAVやm4aを MP3 ファイルなどの形式に変換することができます。
 
-**## 機能**
+## 機能
 
 * WAVやm4aを MP3 ファイルなどの形式に変換する
 * 複数のファイルをまとめて変換する
 * 変換後のファイル名を連番で出力
 
-**## インストール**
+## インストール
 
 ```
 pip3 install AudioAlchemist
 ```
 
-**## 使い方 example**
+## 使い方 example
 
 ```
 # フォルダパスを設定
 input_folder = 'C:/Users/data/melody/*.wav'
 output_folder = 'C:/Users/data/melody/'
 input_extension = "wav"
 output_extension = "mp3"
 
 # 変換処理を実行
-AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
+audio_alchemist = AudioAlchemist(input_folder, output_folder, input_extension, output_extension)
+audio_alchemist.process_files()
 ```
 
 このコマンドは、`C:/Users/data/melody` フォルダ内のすべての WAV ファイルを MP3 ファイルに変換し、`C:/Users/data/melody` フォルダに出力します。
 
-**## 注意**
+## 注意
 
 * 変換するファイルが存在していることを確認してください。
 * 出力フォルダが存在していることを確認してください。
 * 入力ファイルと出力ファイルの拡張子が一致していることを確認してください。
 
-**## サポート**
+## サポート
 
-バグ報告や機能リクエストは、GitHub [無効な URL を削除しました] までご連絡ください。
+バグ報告や機能リクエストは、GitHub までご連絡ください。
 
-**## ライセンス**
+## ライセンス
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
-**## バージョン**
+## バージョン
 
-0.3.0
+0.4.0
```

### Comparing `audioalchemist-0.3.0/setup.py` & `audioalchemist-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = 'Convert all files directly under the directory to any music file.'
 NAME = 'AudioAlchemist'
 AUTHOR = 'Kohki Suto'
 AUTHOR_EMAIL = 's2222019@stu.musashino-u.ac.jp'
 URL = 'https://github.com/Ryomo0797/AudioAlchemist.git'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 PYTHON_REQUIRES = '>=3.6'
 INSTALL_REQUIRES = [
     "pandas>=2.2.2",
     "pydub>=0.25.1",
     "ffmpeg>=1.4"
     #ffmpeg-python==0.2.0
 ]
```

