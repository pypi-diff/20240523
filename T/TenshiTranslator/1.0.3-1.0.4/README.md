# Comparing `tmp/tenshitranslator-1.0.3.tar.gz` & `tmp/tenshitranslator-1.0.4.tar.gz`

## Comparing `tenshitranslator-1.0.3.tar` & `tenshitranslator-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/__init__.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/OutputFormat/LineByLineFormat.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/OutputFormat/OutputFormat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/OutputFormat/__init__.py
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Translator/BatchTranslator.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Translator/OfflineTranslator.py
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Translator/OnlineTranslator.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Translator/Translator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Translator/__init__.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Util/Glossary.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Util/TextProcessor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/TenshiTranslator/Util/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/LICENSE
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    46305 2020-02-02 00:00:00.000000 tenshitranslator-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/CSVGlossary.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/Glossary.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/PassthroughGlossary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/LineByLineFormat.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/OutputFormat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/__init__.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/BatchTranslator.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/OfflineTranslator.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/OnlineTranslator.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/Translator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/__init__.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Util/TextProcessor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Util/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/README.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    46305 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/PKG-INFO
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py` & `tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
-import TenshiTranslator.Util.TextProcessor
-
-class EnglishOnlyFormat(OutputFormat):
-    """ Output format that mimics the structure of the input file, but only contains the translated lines
-    """
-
-    def writeFile(self, outputFilePath: str, japaneseLines: list[str], englishLines: list[str]):
-        """ Writes the translated lines to a file. file will be overwritten if it already exists
-        
-        :param outputFilePath: path to the output file. 
-        :param japaneseLines: list of japanese lines
-        :param englishLines: list of translated lines
-        """
-                
-        with open(outputFilePath, 'w', encoding='utf8') as output:
-            for japanese, english in zip(japaneseLines, englishLines):
-                if TenshiTranslator.Util.TextProcessor.isEmptyLine(japanese):
-                    output.write('\n')
-                    continue
-
-                if TenshiTranslator.Util.TextProcessor.noJapaneseCharacters(japanese):
-                    output.write(japanese)
-                    continue
-                    
-                output.write(english)
+from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
+import TenshiTranslator.Util.TextProcessor
+
+class EnglishOnlyFormat(OutputFormat):
+    """ Output format that mimics the structure of the input file, but only contains the translated lines
+    """
+
+    def writeFile(self, outputFilePath: str, japaneseLines: list[str], englishLines: list[str]):
+        """ Writes the translated lines to a file. file will be overwritten if it already exists
+        
+        :param outputFilePath: path to the output file. 
+        :param japaneseLines: list of japanese lines
+        :param englishLines: list of translated lines
+        """
+                
+        with open(outputFilePath, 'w', encoding='utf8') as output:
+            for japanese, english in zip(japaneseLines, englishLines):
+                if TenshiTranslator.Util.TextProcessor.isEmptyLine(japanese):
+                    output.write('\n')
+                    continue
+
+                if TenshiTranslator.Util.TextProcessor.noJapaneseCharacters(japanese):
+                    output.write(japanese)
+                    continue
+                    
+                output.write(english)
                 output.write('\n')
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/OutputFormat/LineByLineFormat.py` & `tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/LineByLineFormat.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
-import TenshiTranslator.Util.TextProcessor
-
-class LineByLineFormat(OutputFormat):
-    """ Output format that outputs the japanese lines followed by the translated lines.
-
-    The format follows the following fules: \n
-    - An empty line between two japanese line and translations \n
-    - If the japanese line is empty, there will be two empty lines in the output \n
-    - If the japanese line contains no japanese characters, it will be outputted as is with no translation \n
-    
-    This format is intended for translators to quickly reference and check translations
-    """
-
-    def writeFile(self, outputFilePath: str, japaneseLines: list[str], englishLines: list[str]):
-        """ Writes the translated lines to a file. file will be overwritten if it already exists
-        
-        :param outputFilePath: path to the output file. 
-        :param japaneseLines: list of japanese lines
-        :param englishLines: list of translated lines
-        """
-                
-        with open(outputFilePath, 'w', encoding='utf8') as output:
-            for japanese, english in zip(japaneseLines, englishLines):
-                if TenshiTranslator.Util.TextProcessor.isEmptyLine(japanese):
-                    output.write('\n')
-                    continue
-
-                if TenshiTranslator.Util.TextProcessor.noJapaneseCharacters(japanese):
-                    output.write(japanese)
-                    output.write('\n')
-                    continue
-                    
-                output.write(japanese)
-                output.write(english)
+from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
+import TenshiTranslator.Util.TextProcessor
+
+class LineByLineFormat(OutputFormat):
+    """ Output format that outputs the japanese lines followed by the translated lines.
+
+    The format follows the following fules: \n
+    - An empty line between two japanese line and translations \n
+    - If the japanese line is empty, there will be two empty lines in the output \n
+    - If the japanese line contains no japanese characters, it will be outputted as is with no translation \n
+    
+    This format is intended for translators to quickly reference and check translations
+    """
+
+    def writeFile(self, outputFilePath: str, japaneseLines: list[str], englishLines: list[str]):
+        """ Writes the translated lines to a file. file will be overwritten if it already exists
+        
+        :param outputFilePath: path to the output file. 
+        :param japaneseLines: list of japanese lines
+        :param englishLines: list of translated lines
+        """
+                
+        with open(outputFilePath, 'w', encoding='utf8') as output:
+            for japanese, english in zip(japaneseLines, englishLines):
+                if TenshiTranslator.Util.TextProcessor.isEmptyLine(japanese):
+                    output.write('\n')
+                    continue
+
+                if TenshiTranslator.Util.TextProcessor.noJapaneseCharacters(japanese):
+                    output.write(japanese)
+                    output.write('\n')
+                    continue
+                    
+                output.write(japanese)
+                output.write(english)
                 output.write('\n\n')
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/Translator/BatchTranslator.py` & `tenshitranslator-1.0.4/TenshiTranslator/Translator/BatchTranslator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,107 @@
-from TenshiTranslator.Translator.Translator import Translator
-from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
-from TenshiTranslator.Util.Glossary import Glossary
-import TenshiTranslator.Util.TextProcessor
-
-from time import perf_counter, sleep
-import requests
-import json
-import sys
-import subprocess
-import os
-
-class BatchTranslator(Translator):
-    """ Translator that send batches to sugoi toolkit's offline translation server.
-    
-    Files are translated in batches through http requests, optimizating translation time by maximizing 
-    GPU utilization. This translator requires sugoi toolkit and a Nvidia GPU to be useful, but is magnitudes 
-    faster than the other translators. You will have to install CUDA and run the setup script to allow the 
-    sugoi toolkit to accept batch translation requests. This translator is recommended if you have an Nvidia GPU.
-    The object takes around 12 seconds to initialize, as it starts the sugoi offline translator server.
-    
-    :param outputOption: the output format to use
-    :param glossary: the glossary to use
-    :param sugoiDirectory: the path to the sugoi toolkit
-    :param batchSize: the number of lines to translate per request, defaults to 64
-    """
-
-    def __init__(self, outputOption: OutputFormat, glossary: Glossary, sugoiDirectory: str, batchSize: int = 64):
-        super().__init__(outputOption, glossary)
-        self.batchSize = batchSize
-        self.sugoiDirectory = sugoiDirectory
-        self.host = '127.0.0.1:14366'
-
-        print("BatchTranslator: Starting Server...", flush=True)
-        self.server = subprocess.Popen(
-            self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation\\activateOfflineTranslationServer.bat", 
-            cwd=self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation", 
-            creationflags=subprocess.CREATE_NO_WINDOW
-        )
-        sleep(12)
-        print("BatchTranslator: Server Started", flush=True)
-
-    def __del__(self):
-        """ Destructor, stops the sugoi offline translator server    
-        """
-
-        print("BatchTranslator: Stopping Server...", flush=True)
-        headers = {'content-type': 'application/json'}
-        data = {'message': 'close server', 'content': 1}
-        requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
-        sleep(3)
-        print("BatchTranslator: Server Stopped", flush=True)
-
-    def sendTranslationRequest(self, batch: list[str]) -> list[str]:
-        """ Translates a batch from japanese to english using the sugoi offline translator server
-
-        :param batch: list of japanese lines to be translated
-        :return: the translated batch
-        """
-
-        data = {'message': 'batch translate', 'content': batch}
-        headers = {'content-type': 'application/json'}
-        response = requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
-
-        if response.status_code != 200:
-            print(f"Translation request failed with status code {response.status_code}", flush=True)
-            return []
-        
-        return response.json()
-
-    def translate(self, inputFilePath: str):
-        """ Translates a file and writes to inputFilePath-Translated.txt
-        
-        :param inputFilePath: path to the file to be translated
-        :raises: FileNotFoundError if the file is not found
-        :raises: Exception if any other error occurs
-        """
-
-        startTime = perf_counter()
-        japaneseLines = TenshiTranslator.Util.TextProcessor.retrieveLines(inputFilePath)
-        englishLines = []
-
-        try:
-            batch = []
-
-            for index, japanese in enumerate(japaneseLines):
-                japanese = self.glossary.replaceNames(japanese)
-                japanese = TenshiTranslator.Util.TextProcessor.removeIndent(japanese)
-
-                batch.append(japanese)
-
-                if(len(batch) >= self.batchSize or index == len(japaneseLines)-1):
-                    englishLines.extend(self.sendTranslationRequest(batch))
-                    print(f'Current File: {os.path.basename(inputFilePath)}, Progress: {index+1}/{len(japaneseLines)} lines', flush=True)
-                    batch.clear()
-
-            englishLines = [self.glossary.applyCorrections(english) for english in englishLines]
-
-        except Exception as e:
-            print(f"An error occurred: {str(e)}", flush=True)
-            sys.exit(1)
-
-        print(f"Translation Complete. Took {perf_counter() - startTime:.3f} seconds, with an average speed of {len(japaneseLines) / (perf_counter() - startTime):.3f} lines per second\n", flush=True)
-
-        outputFilePath = TenshiTranslator.Util.TextProcessor.makeOutputFilePath(inputFilePath)
+from TenshiTranslator.Translator.Translator import Translator
+from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
+from TenshiTranslator.Glossary.Glossary import Glossary
+import TenshiTranslator.Util.TextProcessor
+
+from time import perf_counter, sleep
+import requests
+import json
+import sys
+import subprocess
+import os
+
+class BatchTranslator(Translator):
+    """ Translator that send batches to sugoi toolkit's offline translation server.
+    
+    Files are translated in batches through http requests, optimizating translation time by maximizing 
+    GPU utilization. This translator requires sugoi toolkit and a Nvidia GPU to be useful, but is magnitudes 
+    faster than the other translators. You will have to install CUDA and run the setup script to allow the 
+    sugoi toolkit to accept batch translation requests. This translator is recommended if you have an Nvidia GPU.
+    The object takes around 12 seconds to initialize, as it starts the sugoi offline translator server.
+    
+    :param outputOption: the output format to use
+    :param preprocessGlossary: the glossary to use for preprocessing
+    :param postProcessGlossary: the glossary to use for postprocessing
+    :param sugoiDirectory: the path to the sugoi toolkit
+    :param batchSize: the number of lines to translate per request, defaults to 64
+    """
+
+    def __init__(self, outputOption: OutputFormat, preprocessGlossary: Glossary, postProcessGlossary: Glossary, sugoiDirectory: str, batchSize: int = 64):
+        super().__init__(outputOption, preprocessGlossary, postProcessGlossary)
+        self.batchSize = batchSize
+        self.sugoiDirectory = sugoiDirectory
+        self.host = '127.0.0.1:14366'
+
+        print("BatchTranslator: Starting Server...", flush=True)
+        self.server = subprocess.Popen(
+            self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation\\activateOfflineTranslationServer.bat", 
+            cwd=self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation", 
+            creationflags=subprocess.CREATE_NO_WINDOW
+        )
+        sleep(12)
+        print("BatchTranslator: Server Started", flush=True)
+
+    def __del__(self):
+        """ Destructor, stops the sugoi offline translator server    
+        """
+
+        print("BatchTranslator: Stopping Server...", flush=True)
+        headers = {'content-type': 'application/json'}
+        data = {'message': 'close server', 'content': 1}
+        requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
+        sleep(3)
+        print("BatchTranslator: Server Stopped", flush=True)
+
+    def sendTranslationRequest(self, batch: list[str]) -> list[str]:
+        """ Translates a batch from japanese to english using the sugoi offline translator server
+
+        :param batch: list of japanese lines to be translated
+        :return: the translated batch
+        """
+
+        data = {'message': 'batch translate', 'content': batch}
+        headers = {'content-type': 'application/json'}
+        response = requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
+
+        if response.status_code != 200:
+            print(f"Translation request failed with status code {response.status_code}", flush=True)
+            return []
+        
+        return response.json()
+
+    def translate(self, inputFilePath: str):
+        """ Translates a file and writes to inputFilePath-Translated.txt
+        
+        :param inputFilePath: path to the file to be translated
+        :raises: FileNotFoundError if the file is not found
+        :raises: Exception if any other error occurs
+        """
+
+        startTime = perf_counter()
+        japaneseLines = TenshiTranslator.Util.TextProcessor.retrieveLines(inputFilePath)
+        englishLines = []
+
+        try:
+            batch = []
+
+            for index, japanese in enumerate(japaneseLines):
+                japanese = self.preprocessGlossary.process(japanese)
+                japanese = TenshiTranslator.Util.TextProcessor.removeIndent(japanese)
+
+                batch.append(japanese)
+
+                if(len(batch) >= self.batchSize or index == len(japaneseLines)-1):
+                    englishLines.extend(self.sendTranslationRequest(batch))
+                    print(f'Current File: {os.path.basename(inputFilePath)}, Progress: {index+1}/{len(japaneseLines)} lines', flush=True)
+                    batch.clear()
+
+            englishLines = [self.postProcessGlossary.process(english) for english in englishLines]
+
+        except Exception as e:
+            print(f"An error occurred: {str(e)}", flush=True)
+            sys.exit(1)
+
+        print(f"Translation Complete. Took {perf_counter() - startTime:.3f} seconds, with an average speed of {len(japaneseLines) / (perf_counter() - startTime):.3f} lines per second\n", flush=True)
+
+        outputFilePath = TenshiTranslator.Util.TextProcessor.makeOutputFilePath(inputFilePath)
         self.outputOption.writeFile(outputFilePath, japaneseLines, englishLines)
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/Translator/OfflineTranslator.py` & `tenshitranslator-1.0.4/TenshiTranslator/Translator/OfflineTranslator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,99 @@
-from TenshiTranslator.Translator.Translator import Translator
-from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
-from TenshiTranslator.Util.Glossary import Glossary
-import TenshiTranslator.Util.TextProcessor
-
-from time import perf_counter, sleep
-import requests
-import json
-import sys
-import subprocess
-import os
-
-class OfflineTranslator(Translator):
-    """ Translator that uses sugoi toolkit's offline translation server. 
-    
-    Files are translated line by line through http requests. This translator requires sugoi toolkit but is faster than the online 
-    translator. It is also more accurate as it uses a newer model and has no character limits. The speed of this translator is 
-    dependent on your computer's hardware, and is generally recommended if you don't have an Nvidia GPU. The object takes around
-    12 seconds to initialize, as it starts the sugoi offline translator server.
-    
-    :param outputOption: the output format to use
-    :param glossary: the glossary to use
-    :param sugoiDirectory: the path to the sugoi toolkit
-    """
-
-    def __init__(self, outputOption: OutputFormat, glossary: Glossary, sugoiDirectory: str):
-        super().__init__(outputOption, glossary)
-        self.sugoiDirectory = sugoiDirectory
-        self.host = '127.0.0.1:14366'
-
-        print("OfflineTranslator: Starting Server...", flush=True)
-        self.server = subprocess.Popen(
-            self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation\\activateOfflineTranslationServer.bat", 
-            cwd=self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation", 
-            creationflags=subprocess.CREATE_NO_WINDOW
-        )
-        sleep(12)
-        print("OfflineTranslator: Server Started", flush=True)
-
-    def __del__(self):
-        """ Destructor, stops the sugoi offline translator server
-        """
-
-        print("OfflineTranslator: Stopping Server...", flush=True)
-        headers = {'content-type': 'application/json'}
-        data = {'message': 'close server', 'content': 1}
-        requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
-        sleep(3)
-        print("OfflineTranslator: Server Stopped", flush=True)
-
-    def sendTranslationRequest(self, japanese: str) -> str:
-        """ Translates a string from japanese to english using the sugoi offline translator server
-
-        :param japanese: the string to be translated
-        :return: the translated string
-        """
-        
-        data = {'message': 'translate sentences', 'content': japanese}
-        headers = {'content-type': 'application/json'}
-        response = requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
-
-        if response.status_code != 200:
-            print(f"Translation request failed with status code {response.status_code}", flush=True)
-            return []
-        
-        return response.json()
-
-    def translate(self, inputFilePath: str):
-        """ Translates a file and writes to inputFilePath-Translated.txt
-        
-        :param inputFilePath: path to the file to be translated
-        :raises: FileNotFoundError if the file is not found
-        :raises: Exception if any other error occurs
-        """
-                
-        startTime = perf_counter()
-        japaneseLines = TenshiTranslator.Util.TextProcessor.retrieveLines(inputFilePath)
-        englishLines = []
-
-        try:
-            for index, japanese in enumerate(japaneseLines):
-                print(f'Current File: {os.path.basename(inputFilePath)}, Progress: {index+1}/{len(japaneseLines)} lines', flush=True)
-
-                japanese = self.glossary.replaceNames(japanese)
-                japanese = TenshiTranslator.Util.TextProcessor.removeIndent(japanese)
-
-                english = self.sendTranslationRequest(japanese)
-                english = self.glossary.applyCorrections(english)
-                englishLines.append(english)
-
-        except Exception as e:
-            print(f"An error occurred: {str(e)}", flush=True)
-            sys.exit(1)
-
-        print(f"Translation Complete. Took {perf_counter() - startTime:.3f} seconds, with an average speed of {len(japaneseLines) / (perf_counter() - startTime):.3f} lines per second\n", flush=True)
-
-        outputFilePath = TenshiTranslator.Util.TextProcessor.makeOutputFilePath(inputFilePath)
+from TenshiTranslator.Translator.Translator import Translator
+from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
+from TenshiTranslator.Glossary.Glossary import Glossary
+import TenshiTranslator.Util.TextProcessor
+
+from time import perf_counter, sleep
+import requests
+import json
+import sys
+import subprocess
+import os
+
+class OfflineTranslator(Translator):
+    """ Translator that uses sugoi toolkit's offline translation server. 
+    
+    Files are translated line by line through http requests. This translator requires sugoi toolkit but is faster than the online 
+    translator. It is also more accurate as it uses a newer model and has no character limits. The speed of this translator is 
+    dependent on your computer's hardware, and is generally recommended if you don't have an Nvidia GPU. The object takes around
+    12 seconds to initialize, as it starts the sugoi offline translator server.
+    
+    :param outputOption: the output format to use
+    :param preprocessGlossary: the glossary to use for preprocessing
+    :param postProcessGlossary: the glossary to use for postprocessing
+    :param sugoiDirectory: the path to the sugoi toolkit
+    """
+
+    def __init__(self, outputOption: OutputFormat, preprocessGlossary: Glossary, postProcessGlossary: Glossary, sugoiDirectory: str):
+        super().__init__(outputOption, preprocessGlossary, postProcessGlossary)
+        self.sugoiDirectory = sugoiDirectory
+        self.host = '127.0.0.1:14366'
+
+        print("OfflineTranslator: Starting Server...", flush=True)
+        self.server = subprocess.Popen(
+            self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation\\activateOfflineTranslationServer.bat", 
+            cwd=self.sugoiDirectory + "\\Code\\backendServer\\Program-Backend\\Sugoi-Japanese-Translator\\offlineTranslation", 
+            creationflags=subprocess.CREATE_NO_WINDOW
+        )
+        sleep(12)
+        print("OfflineTranslator: Server Started", flush=True)
+
+    def __del__(self):
+        """ Destructor, stops the sugoi offline translator server
+        """
+
+        print("OfflineTranslator: Stopping Server...", flush=True)
+        headers = {'content-type': 'application/json'}
+        data = {'message': 'close server', 'content': 1}
+        requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
+        sleep(3)
+        print("OfflineTranslator: Server Stopped", flush=True)
+
+    def sendTranslationRequest(self, japanese: str) -> str:
+        """ Translates a string from japanese to english using the sugoi offline translator server
+
+        :param japanese: the string to be translated
+        :return: the translated string
+        """
+        
+        data = {'message': 'translate sentences', 'content': japanese}
+        headers = {'content-type': 'application/json'}
+        response = requests.post(f'http://{self.host}/', data=json.dumps(data), headers=headers)
+
+        if response.status_code != 200:
+            print(f"Translation request failed with status code {response.status_code}", flush=True)
+            return []
+        
+        return response.json()
+
+    def translate(self, inputFilePath: str):
+        """ Translates a file and writes to inputFilePath-Translated.txt
+        
+        :param inputFilePath: path to the file to be translated
+        :raises: FileNotFoundError if the file is not found
+        :raises: Exception if any other error occurs
+        """
+                
+        startTime = perf_counter()
+        japaneseLines = TenshiTranslator.Util.TextProcessor.retrieveLines(inputFilePath)
+        englishLines = []
+
+        try:
+            for index, japanese in enumerate(japaneseLines):
+                print(f'Current File: {os.path.basename(inputFilePath)}, Progress: {index+1}/{len(japaneseLines)} lines', flush=True)
+
+                japanese = self.preprocessGlossary.process(japanese)
+                japanese = TenshiTranslator.Util.TextProcessor.removeIndent(japanese)
+
+                english = self.sendTranslationRequest(japanese)
+                english = self.postProcessGlossary.process(english)
+                englishLines.append(english)
+
+        except Exception as e:
+            print(f"An error occurred: {str(e)}", flush=True)
+            sys.exit(1)
+
+        print(f"Translation Complete. Took {perf_counter() - startTime:.3f} seconds, with an average speed of {len(japaneseLines) / (perf_counter() - startTime):.3f} lines per second\n", flush=True)
+
+        outputFilePath = TenshiTranslator.Util.TextProcessor.makeOutputFilePath(inputFilePath)
         self.outputOption.writeFile(outputFilePath, japaneseLines, englishLines)
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/Translator/OnlineTranslator.py` & `tenshitranslator-1.0.4/TenshiTranslator/Translator/OnlineTranslator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,137 @@
-from TenshiTranslator.Translator.Translator import Translator
-from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
-from TenshiTranslator.Util.Glossary import Glossary
-import TenshiTranslator.Util.TextProcessor
-
-from time import perf_counter, sleep
-import sys
-import os
-
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-
-import chromedriver_autoinstaller
-
-class OnlineTranslator(Translator):
-    """ Translator that translates by automating sugoitranslator.com using selenium
-    
-    As sugoi translator has a rate limit, this translator automatically waits for the timeout to end before resuming.
-    The advantage of this translator is that it is free and does not require any setup. However, it is both the slowest 
-    and the least accurate as it uses an older model and has a character limit of 100 characters per request. Long 
-    sentences will be split into multiple requests, and contexts will not be taken into account.
-
-    :param outputOption: the output format to use
-    :param glossary: the glossary to use
-    :param timeoutWait: the time to wait in seconds when a timeout is detected, defaults to 315 seconds
-    """
-
-    def __init__(self, outputOption: OutputFormat, glossary: Glossary, timeoutWait: int = 315):
-        super().__init__(outputOption, glossary)
-        self.timeoutWait = timeoutWait
-
-        self.url = "https://sugoitranslator.com/"
-        self.swapLanguageButtonXPath = "//*[@id=\"routify-app\"]/div[1]/div/div[1]/div/div/div[2]/button"
-        self.translateButtonXPath = "//*[@id=\"routify-app\"]/div[1]/div/div[1]/div/button"
-        self.inputBoxPath = "//*[@id=\"routify-app\"]/div[1]/div/div[2]/div/div[1]"
-        self.outputBoxPath = "//*[@id=\"routify-app\"]/div[1]/div/div[2]/div/div[2]"
-
-        chromedriver_autoinstaller.install()
-
-        options = Options()
-        options.add_argument("--headless=new")
-        self.driver = webdriver.Chrome(options = options)
-        self.initWebsite()
-
-    def __del__(self):
-        """ Destructor, closes the selenium driver
-        """
-
-        self.driver.quit()
-
-    def initWebsite(self):
-        """ Initializes the website by opening the site then swapping the language to japanese
-        """
-
-        self.driver.get("https://sugoitranslator.com/")
-
-        WebDriverWait(self.driver, 5).until(
-            EC.presence_of_element_located((By.XPATH, self.swapLanguageButtonXPath))
-        )
-
-        swapLanguageButton = self.driver.find_element(By.XPATH, self.swapLanguageButtonXPath)
-        swapLanguageButton.click()
-
-    def japaneseToEnglish(self, japanese: str | list[str]) -> str:
-        """ Translates a string or a list of strings from japanese to english using the sugoitranslator website and selenium
-    
-        :param japanese: the string or list of strings to be translated
-        :return: the translated string
-        """
-
-        if(type(japanese) is list):
-            return " ".join([self.japaneseToEnglish(lines) for lines in japanese])
-        
-        inputBox = self.driver.find_element(By.XPATH, self.inputBoxPath)
-        inputBox.clear()
-        inputBox.send_keys(japanese)
-
-        outputBox = self.driver.find_element(By.XPATH, self.outputBoxPath)
-        currentText = outputBox.text
-
-        translateButton = self.driver.find_element(By.XPATH, self.translateButtonXPath)
-        translateButton.click()
-
-        WebDriverWait(self.driver, 5).until(
-            lambda parent: outputBox.text != '' and outputBox.text != 'Waiting for translation' and outputBox.text != currentText
-        )
-
-        if TenshiTranslator.Util.TextProcessor.isTimeoutMessage(outputBox.text):
-            print("Detected timeout, resuming once timeout is over.", flush=True)
-            sleep(self.timeoutWait)
-            return self.japaneseToEnglish(japanese)
-        
-        sleep(5)
-        return outputBox.text
-
-    def translate(self, inputFilePath: str):
-        """ Translates a file and writes to inputFilePath-Translated.txt
-    
-        :param inputFilePath: path to the file to be translated
-        :raises: FileNotFoundError if the file is not found
-        :raises: Exception if any other error occurs
-        """
-            
-        startTime = perf_counter()
-        japaneseLines = TenshiTranslator.Util.TextProcessor.retrieveLines(inputFilePath)
-        englishLines = []
-
-        try:
-            for index, japanese in enumerate(japaneseLines):
-                print(f'Current File: {os.path.basename(inputFilePath)}, Progress: {index+1}/{len(japaneseLines)} lines', flush=True)
-
-                if TenshiTranslator.Util.TextProcessor.isEmptyLine(japanese):
-                    englishLines.append('\n')
-                    # Makes sure output is not too fast
-                    sleep(0.1)
-                    continue
-                
-                japanese = self.glossary.replaceNames(japanese)
-                japanese = TenshiTranslator.Util.TextProcessor.removeIndent(japanese)
-
-                # Sugoi web translator has a character limit of 150 characters per request
-                english = self.japaneseToEnglish(TenshiTranslator.Util.TextProcessor.splitToSentence(japanese, 150))
-                english = self.glossary.applyCorrections(english)
-                englishLines.append(english)
-    
-        except Exception as e:
-            print(f"An error occurred: {str(e)}", flush=True)
-            sys.exit(1)
-        
-        print(f'Translation Complete. Took {perf_counter() - startTime:.3f} seconds, with an average speed of {len(japaneseLines) / (perf_counter() - startTime):.3f} lines per second\n', flush=True)
-        
-        outputFilePath = TenshiTranslator.Util.TextProcessor.makeOutputFilePath(inputFilePath)
+from TenshiTranslator.Translator.Translator import Translator
+from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
+from TenshiTranslator.Glossary.Glossary import Glossary
+import TenshiTranslator.Util.TextProcessor
+
+from time import perf_counter, sleep
+import sys
+import os
+
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+
+import chromedriver_autoinstaller
+
+class OnlineTranslator(Translator):
+    """ Translator that translates by automating sugoitranslator.com using selenium
+    
+    As sugoi translator has a rate limit, this translator automatically waits for the timeout to end before resuming.
+    The advantage of this translator is that it is free and does not require any setup. However, it is both the slowest 
+    and the least accurate as it uses an older model and has a character limit of 100 characters per request. Long 
+    sentences will be split into multiple requests, and contexts will not be taken into account.
+
+    :param outputOption: the output format to use
+    :param preprocessGlossary: the glossary to use for preprocessing
+    :param postProcessGlossary: the glossary to use for postprocessing
+    :param timeoutWait: the time to wait in seconds when a timeout is detected, defaults to 315 seconds
+    """
+
+    def __init__(self, outputOption: OutputFormat, preprocessGlossary: Glossary, postProcessGlossary: Glossary, timeoutWait: int = 315):
+        super().__init__(outputOption, preprocessGlossary, postProcessGlossary)
+        self.timeoutWait = timeoutWait
+
+        self.url = "https://sugoitranslator.com/"
+        self.swapLanguageButtonXPath = "//*[@id=\"routify-app\"]/div[1]/div/div[1]/div/div/div[2]/button"
+        self.translateButtonXPath = "//*[@id=\"routify-app\"]/div[1]/div/div[1]/div/button"
+        self.inputBoxPath = "//*[@id=\"routify-app\"]/div[1]/div/div[2]/div/div[1]"
+        self.outputBoxPath = "//*[@id=\"routify-app\"]/div[1]/div/div[2]/div/div[2]"
+
+        chromedriver_autoinstaller.install()
+
+        options = Options()
+        options.add_argument("--headless=new")
+        self.driver = webdriver.Chrome(options = options)
+        self.initWebsite()
+
+    def __del__(self):
+        """ Destructor, closes the selenium driver
+        """
+
+        self.driver.quit()
+
+    def initWebsite(self):
+        """ Initializes the website by opening the site then swapping the language to japanese
+        """
+
+        self.driver.get("https://sugoitranslator.com/")
+
+        WebDriverWait(self.driver, 5).until(
+            EC.presence_of_element_located((By.XPATH, self.swapLanguageButtonXPath))
+        )
+
+        swapLanguageButton = self.driver.find_element(By.XPATH, self.swapLanguageButtonXPath)
+        swapLanguageButton.click()
+
+    def japaneseToEnglish(self, japanese: str | list[str]) -> str:
+        """ Translates a string or a list of strings from japanese to english using the sugoitranslator website and selenium
+    
+        :param japanese: the string or list of strings to be translated
+        :return: the translated string
+        """
+
+        if(type(japanese) is list):
+            return " ".join([self.japaneseToEnglish(lines) for lines in japanese])
+        
+        inputBox = self.driver.find_element(By.XPATH, self.inputBoxPath)
+        inputBox.clear()
+        inputBox.send_keys(japanese)
+
+        outputBox = self.driver.find_element(By.XPATH, self.outputBoxPath)
+        currentText = outputBox.text
+
+        translateButton = self.driver.find_element(By.XPATH, self.translateButtonXPath)
+        translateButton.click()
+
+        WebDriverWait(self.driver, 5).until(
+            lambda parent: outputBox.text != '' and outputBox.text != 'Waiting for translation' and outputBox.text != currentText
+        )
+
+        if TenshiTranslator.Util.TextProcessor.isTimeoutMessage(outputBox.text):
+            print("Detected timeout, resuming once timeout is over.", flush=True)
+            sleep(self.timeoutWait)
+            return self.japaneseToEnglish(japanese)
+        
+        sleep(5)
+        return outputBox.text
+
+    def translate(self, inputFilePath: str):
+        """ Translates a file and writes to inputFilePath-Translated.txt
+    
+        :param inputFilePath: path to the file to be translated
+        :raises: FileNotFoundError if the file is not found
+        :raises: Exception if any other error occurs
+        """
+            
+        startTime = perf_counter()
+        japaneseLines = TenshiTranslator.Util.TextProcessor.retrieveLines(inputFilePath)
+        englishLines = []
+
+        try:
+            for index, japanese in enumerate(japaneseLines):
+                print(f'Current File: {os.path.basename(inputFilePath)}, Progress: {index+1}/{len(japaneseLines)} lines', flush=True)
+
+                if TenshiTranslator.Util.TextProcessor.isEmptyLine(japanese):
+                    englishLines.append('\n')
+                    # Makes sure output is not too fast
+                    sleep(0.1)
+                    continue
+                
+                japanese = self.preprocessGlossary.process(japanese)
+                japanese = TenshiTranslator.Util.TextProcessor.removeIndent(japanese)
+
+                # Sugoi web translator has a character limit of 150 characters per request
+                english = self.japaneseToEnglish(TenshiTranslator.Util.TextProcessor.splitToSentence(japanese, 150))
+                english = self.postProcessGlossary.process(english)
+                englishLines.append(english)
+    
+        except Exception as e:
+            print(f"An error occurred: {str(e)}", flush=True)
+            sys.exit(1)
+        
+        print(f'Translation Complete. Took {perf_counter() - startTime:.3f} seconds, with an average speed of {len(japaneseLines) / (perf_counter() - startTime):.3f} lines per second\n', flush=True)
+        
+        outputFilePath = TenshiTranslator.Util.TextProcessor.makeOutputFilePath(inputFilePath)
         self.outputOption.writeFile(outputFilePath, japaneseLines, englishLines)
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/Translator/Translator.py` & `tenshitranslator-1.0.4/TenshiTranslator/Translator/Translator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from abc import ABC, abstractmethod
-from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
-from TenshiTranslator.Util.Glossary import Glossary
-
-
-class Translator(ABC):  
-    """ Abstract class for translators that translates a file
-    
-    :param outputOption: the output format to use
-    :param glossary: the glossary to use
-    """
-
-    def __init__(self, outputOption: OutputFormat, glossary: Glossary):
-        self.outputOption = outputOption
-        self.glossary = glossary
-        
-
-    def translate(self, inputFilePath: str):
-        """ Translates a file and writes to inputFilePath-Translated.txt
-    
-        :param inputFilePath: path to the file to be translated
-        """
-
+from abc import ABC, abstractmethod
+from TenshiTranslator.OutputFormat.OutputFormat import OutputFormat
+from TenshiTranslator.Glossary.Glossary import Glossary
+
+
+class Translator(ABC):  
+    """ Abstract class for translators that translates a file
+    
+    :param outputOption: the output format to use
+    :param preprocessGlossary: the glossary to use for preprocessing
+    :param postProcessGlossary: the glossary to use for postprocessing
+    """
+
+    def __init__(self, outputOption: OutputFormat, preprocessGlossary: Glossary, postProcessGlossary: Glossary):
+        self.outputOption = outputOption
+        self.preprocessGlossary = preprocessGlossary
+        self.postProcessGlossary = postProcessGlossary
+        
+
+    def translate(self, inputFilePath: str):
+        """ Translates a file and writes to inputFilePath-Translated.txt
+    
+        :param inputFilePath: path to the file to be translated
+        """
+
         pass
```

### Comparing `tenshitranslator-1.0.3/TenshiTranslator/Util/TextProcessor.py` & `tenshitranslator-1.0.4/TenshiTranslator/Util/TextProcessor.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-"""
-Contains functions that process text, such as removing indent, splitting sentences, etc.
-"""
- 
-import re
-import os
-import sys
-
-def retrieveLines(inputFilePath: str) -> list[str]:
-    """ Retrieves every line from a .txt file. The code terminates if the file is not found.
-
-    :param inputFilePath: path to the desired file
-    :raises: FileNotFoundError if the file is not found
-    :return: list of lines from the file
-    """
-
-    lines = []
-    try:
-        with open(inputFilePath, 'r', encoding='utf8') as file:
-            for line in file:
-                lines.append(line)
-
-    except Exception as e:
-        print(f"An error occurred: {str(e)}", flush=True)
-        sys.exit(1)
-
-    return lines
-
-def makeOutputFilePath(inputFilePath: str) -> str:
-    """ Builds the output file path from the input file path
-
-    :param inputFilePath: path to the desired file
-    :return: path of the output file, in format of <input file name>-Translated.<extension>
-    """
-
-    return os.path.splitext(inputFilePath)[0] + "-Translated.txt"
-
-def isEmptyLine(line: str) -> bool:
-    """ Checks if a line is empty
-
-    :param line: line to be checked
-    :return: 'True' if the line is empty, 'False' otherwise
-    """
-
-    return not line.strip()
-
-def removeIndent(line: str) -> str:
-    """ Removes indent from a sentence
-
-    :param line: line to be modified
-    :return: line without indent
-    """
-
-    return line[1:] if line[0] == '　' else line
-
-def isTimeoutMessage(line: str) -> bool:
-    """ Checks if the line is a timeout message from the Sugoi Translator site
-
-    :param line: line to be checked
-    :return: 'True' if the line is a timeout message, 'False' otherwise
-    """
-
-    return line.count('discord.gg') != 0
-
-def splitToSentence(line: str, maxLength: int) -> list:
-    """ If the japanese paragraph is longer than the max allowed length, splits it into smaller sentences.
-
-    The sentences are split by the period character. This is used to comply with Sugoi translator site's 
-    100 character limit.
-
-    :param line: lline to be split
-    :param maxLength: max allowed length of a sentence
-    :return: list of sentences
-    """
-
-    if len(line) <= maxLength:
-        return [line]
-    
-    return [sentence + '。' for sentence in line.split('。') if sentence and sentence != '\n']
-
-def noJapaneseCharacters(line: str) -> bool:
-    """ Checks if string contains no Japanese characters
-
-    :param line: line to be checked
-    :return: 'True' if the line contains no Japanese characters, 'False' otherwise
-    """
-    
-    pattern = re.compile(r'[\u3040-\u30ff\u3400-\u4dbf\u4e00-\u9fff\uf900-\ufaff\uff66-\uff9f]')
+"""
+Contains functions that process text, such as removing indent, splitting sentences, etc.
+"""
+ 
+import re
+import os
+import sys
+
+def retrieveLines(inputFilePath: str) -> list[str]:
+    """ Retrieves every line from a .txt file. The code terminates if the file is not found.
+
+    :param inputFilePath: path to the desired file
+    :raises: FileNotFoundError if the file is not found
+    :return: list of lines from the file
+    """
+
+    lines = []
+    try:
+        with open(inputFilePath, 'r', encoding='utf8') as file:
+            for line in file:
+                lines.append(line)
+
+    except Exception as e:
+        print(f"An error occurred: {str(e)}", flush=True)
+        sys.exit(1)
+
+    return lines
+
+def makeOutputFilePath(inputFilePath: str) -> str:
+    """ Builds the output file path from the input file path
+
+    :param inputFilePath: path to the desired file
+    :return: path of the output file, in format of <input file name>-Translated.<extension>
+    """
+
+    return os.path.splitext(inputFilePath)[0] + "-Translated.txt"
+
+def isEmptyLine(line: str) -> bool:
+    """ Checks if a line is empty
+
+    :param line: line to be checked
+    :return: 'True' if the line is empty, 'False' otherwise
+    """
+
+    return not line.strip()
+
+def removeIndent(line: str) -> str:
+    """ Removes indent from a sentence
+
+    :param line: line to be modified
+    :return: line without indent
+    """
+
+    return line[1:] if line[0] == '　' else line
+
+def isTimeoutMessage(line: str) -> bool:
+    """ Checks if the line is a timeout message from the Sugoi Translator site
+
+    :param line: line to be checked
+    :return: 'True' if the line is a timeout message, 'False' otherwise
+    """
+
+    return line.count('discord.gg') != 0
+
+def splitToSentence(line: str, maxLength: int) -> list:
+    """ If the japanese paragraph is longer than the max allowed length, splits it into smaller sentences.
+
+    The sentences are split by the period character. This is used to comply with Sugoi translator site's 
+    100 character limit.
+
+    :param line: lline to be split
+    :param maxLength: max allowed length of a sentence
+    :return: list of sentences
+    """
+
+    if len(line) <= maxLength:
+        return [line]
+    
+    return [sentence + '。' for sentence in line.split('。') if sentence and sentence != '\n']
+
+def noJapaneseCharacters(line: str) -> bool:
+    """ Checks if string contains no Japanese characters
+
+    :param line: line to be checked
+    :return: 'True' if the line contains no Japanese characters, 'False' otherwise
+    """
+    
+    pattern = re.compile(r'[\u3040-\u30ff\u3400-\u4dbf\u4e00-\u9fff\uf900-\ufaff\uff66-\uff9f]')
     return re.search(pattern, line) is None
```

### Comparing `tenshitranslator-1.0.3/LICENSE` & `tenshitranslator-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `tenshitranslator-1.0.3/README.md` & `tenshitranslator-1.0.4/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-[![Docs](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/docs.yml/badge.svg)](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/docs.yml)
-[![Unit Test](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml/badge.svg)](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/Ryan4253/TenshiTranslator/graph/badge.svg?token=G04BIXZ45E)](https://codecov.io/gh/Ryan4253/TenshiTranslator)
-[![PyPI version](https://badge.fury.io/py/TenshiTranslator.svg)](https://badge.fury.io/py/TenshiTranslator)
-
-# TenshiTranslator
-Sugoi Toolkit's [Sugoi Translator](https://sugoitoolkit.com/) is very effective for ACG (Anime, Comit, Games) media translation as the model is trained with data from the same medium. However, the project lacks automation support as all the features require manual control, which makes large file translation incredibly daunting. This project implements automation utility that interfaces with the translator to both automate the translation process and increase the translation accuracy. This project has since then been adopted by over 10 novel series to generate preliminary machine translations for new novels.  
-
-![project](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/263efe3b-5062-4ec2-961e-943658f54ec7)  
-
-
-## Getting Started
-You can install the project using ```pip install TenshiTranslator```  
-For more information, visit the documentation [here](https://ryan4253.github.io/TenshiTranslator/)
-
-## Translator Options
-
-### Online Translator
-This translator automates Sugoi Toolkit's [web translator](sugoitranslator.com) with zero extra setup required. However, it is both the slowest and the least accurate due to an older model, api limits, and a character limit.  
-![online](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/ee3a442d-a03e-4e27-9075-d0d9a8c627d7)
-
-### Offline Translator
-This translator uses Sugoi Toolkit’s offline translation server to perform translations. This translator requires Sugoi Toolkit but is faster than the online translator. It is also more accurate as it uses a newer model and has no character limits. The speed of this translator is dependent on your computer’s hardware, and is generally recommended if you don’t have an Nvidia GPU.   
-
-### Batch Translator
-This translator uses Sugoi Toolkit’s offline translation server to perform translations. Files are translated in batches, optimizating translation time by maximizing GPU utilization. This translator requires Sugoi Toolkit and a Nvidia GPU to be useful, but is magnitudes faster than the other translators. You will have to install CUDA and run the setup script to allow the sugoi toolkit to accept batch translation requests. This translator is recommended if you have an Nvidia GPU.
-
-## Features
-### Multiple format support  
-The translator offers two output formats: english only where the original stucture of the file is preserved, and line by line where each line of Japanese is followed by its translation, accelerating translation checking speed. The package also provide abstraction over outputs so you are free to implement your own formats.  
-<br>
-![english](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/818d7173-2d3f-49bf-822c-1494beb50dea)  
-Example English only format
-<br>  
-![lbl](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/1b685a9c-6bfd-4274-b894-8e45070d8486)  
-Example line by line format
-
-### High level glossary  
-You can specify translations for specific phrases and also apply corrections to the translated text to improve translation accuracy. This is commonly used for names and other jargons that may not be translated correctly.  
-<br>
-![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/2be406f1-ed6a-4eef-979f-24940f342ab3)
-![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/04264b62-1be2-4506-9889-7bb048533723)  
-Example replacement & correction with regex
-
-## Requirements
-To run the program, you need Python >= 3.10  
-To use the offline and batch translator, you need Windows, and download Sugoi Toolkit from [here](https://www.patreon.com/mingshiba/about)  
-To use the batch translator, you need a computer with a Nvidia GPU and [CUDA](https://developer.nvidia.com/cuda-downloads)
-
-## Benchmarks
-![benchmark](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/e12ce131-ec07-4de8-a3bb-46bac0a13f41)  
-Benchmark is done by measuring the time taken to translate 125 lines. Benchmark is run with an Intel i7-13700k and a Nvidia RTX 3060ti 8G
-
-## Credits
-CUDA Installation script is adapted from the work by Tenerezza from the Sugoi Toolkit Discord  
-Batch translation is first implemented by [@EagleEye17](https://github.com/EagleEye17), who also gave a lot of suggestions to the overall project  
+[![Docs](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/docs.yml/badge.svg)](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/docs.yml)
+[![Unit Test](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml/badge.svg)](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/Ryan4253/TenshiTranslator/graph/badge.svg?token=G04BIXZ45E)](https://codecov.io/gh/Ryan4253/TenshiTranslator)
+[![PyPI version](https://badge.fury.io/py/TenshiTranslator.svg)](https://badge.fury.io/py/TenshiTranslator)
+
+# TenshiTranslator
+Sugoi Toolkit's [Sugoi Translator](https://sugoitoolkit.com/) is very effective for ACG (Anime, Comit, Games) media translation as the model is trained with data from the same medium. However, the project lacks automation support as all the features require manual control, which makes large file translation incredibly daunting. This project implements automation utility that interfaces with the translator to both automate the translation process and increase the translation accuracy. This project has since then been adopted by over 10 novel series to generate preliminary machine translations for new novels.  
+
+![project](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/263efe3b-5062-4ec2-961e-943658f54ec7)  
+
+
+## Getting Started
+You can install the project using ```pip install TenshiTranslator```  
+For more information, visit the documentation [here](https://ryan4253.github.io/TenshiTranslator/)
+
+## Translator Options
+
+### Online Translator
+This translator automates Sugoi Toolkit's [web translator](sugoitranslator.com) with zero extra setup required. However, it is both the slowest and the least accurate due to an older model, api limits, and a character limit.  
+![online](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/ee3a442d-a03e-4e27-9075-d0d9a8c627d7)
+
+### Offline Translator
+This translator uses Sugoi Toolkit’s offline translation server to perform translations. This translator requires Sugoi Toolkit but is faster than the online translator. It is also more accurate as it uses a newer model and has no character limits. The speed of this translator is dependent on your computer’s hardware, and is generally recommended if you don’t have an Nvidia GPU.   
+
+### Batch Translator
+This translator uses Sugoi Toolkit’s offline translation server to perform translations. Files are translated in batches, optimizating translation time by maximizing GPU utilization. This translator requires Sugoi Toolkit and a Nvidia GPU to be useful, but is magnitudes faster than the other translators. You will have to install CUDA and run the setup script to allow the sugoi toolkit to accept batch translation requests. This translator is recommended if you have an Nvidia GPU.
+
+## Features
+### Multiple format support  
+The translator offers two output formats: english only where the original stucture of the file is preserved, and line by line where each line of Japanese is followed by its translation, accelerating translation checking speed. The package also provide abstraction over outputs so you are free to implement your own formats.  
+<br>
+![english](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/818d7173-2d3f-49bf-822c-1494beb50dea)  
+Example English only format
+<br>  
+![lbl](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/1b685a9c-6bfd-4274-b894-8e45070d8486)  
+Example line by line format
+
+### High level glossary  
+You can specify translations for specific phrases and also apply corrections to the translated text to improve translation accuracy. This is commonly used for names and other jargons that may not be translated correctly.  
+<br>
+![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/2be406f1-ed6a-4eef-979f-24940f342ab3)
+![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/04264b62-1be2-4506-9889-7bb048533723)  
+Example replacement & correction with regex
+
+## Requirements
+To run the program, you need Python >= 3.10  
+To use the offline and batch translator, you need Windows, and download Sugoi Toolkit from [here](https://www.patreon.com/mingshiba/about)  
+To use the batch translator, you need a computer with a Nvidia GPU and [CUDA](https://developer.nvidia.com/cuda-downloads)
+
+## Benchmarks
+![benchmark](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/e12ce131-ec07-4de8-a3bb-46bac0a13f41)  
+Benchmark is done by measuring the time taken to translate 125 lines. Benchmark is run with an Intel i7-13700k and a Nvidia RTX 3060ti 8G
+
+## Credits
+CUDA Installation script is adapted from the work by Tenerezza from the Sugoi Toolkit Discord  
+Batch translation is first implemented by [@EagleEye17](https://github.com/EagleEye17), who also gave a lot of suggestions to the overall project
```

### Comparing `tenshitranslator-1.0.3/pyproject.toml` & `tenshitranslator-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "TenshiTranslator"
-version = "1.0.3"
-requires-python = ">=3.10"
-authors = [{ name="Ryan4253", email="ryan.liao0305@gmail.com" }]
-description = "Novel Translation utility using Sugoi Translator"
-readme = "README.md"
-license = {file="LICENSE"}
-
-dependencies = [
-  "requests",
-  "selenium",
-  "chromedriver-autoinstaller",
-]
-
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Operating System :: Microsoft :: Windows",
-    "Development Status :: 4 - Beta",
-    "Framework :: Pytest",
-    "Framework :: Sphinx",
-    "Topic :: Text Processing :: Linguistic"
-]
-
-[project.urls]
-Homepage = "https://github.com/Ryan4253/TenshiTranslator"
-Issues = "https://github.com/Ryan4253/TenshiTranslator/issues"
-documentation = "https://ryan4253.github.io/TenshiTranslator/"
-
-[tool.hatch.build]
-include = [
-  "TenshiTranslator/*",
-]
-
-exclude = [
-  "TenshiTranslator/Backend.py"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "TenshiTranslator"
+version = "1.0.4"
+requires-python = ">=3.10"
+authors = [{ name="Ryan4253", email="ryan.liao0305@gmail.com" }]
+description = "Novel Translation utility using Sugoi Translator"
+readme = "README.md"
+license = {file="LICENSE"}
+
+dependencies = [
+  "requests",
+  "selenium",
+  "chromedriver-autoinstaller",
+]
+
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Operating System :: Microsoft :: Windows",
+    "Development Status :: 4 - Beta",
+    "Framework :: Pytest",
+    "Framework :: Sphinx",
+    "Topic :: Text Processing :: Linguistic"
+]
+
+[project.urls]
+Homepage = "https://github.com/Ryan4253/TenshiTranslator"
+Issues = "https://github.com/Ryan4253/TenshiTranslator/issues"
+documentation = "https://ryan4253.github.io/TenshiTranslator/"
+
+[tool.hatch.build]
+include = [
+  "TenshiTranslator/*",
+]
+
+exclude = [
+  "TenshiTranslator/Backend.py"
 ]
```

### Comparing `tenshitranslator-1.0.3/PKG-INFO` & `tenshitranslator-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: TenshiTranslator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Novel Translation utility using Sugoi Translator
 Project-URL: Homepage, https://github.com/Ryan4253/TenshiTranslator
 Project-URL: Issues, https://github.com/Ryan4253/TenshiTranslator/issues
 Project-URL: documentation, https://ryan4253.github.io/TenshiTranslator/
 Author-email: Ryan4253 <ryan.liao0305@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

