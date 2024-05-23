# Comparing `tmp/medium_to_markdown_py-1.1.4.tar.gz` & `tmp/medium_to_markdown_py-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.1.4.tar", last modified: Thu May  2 14:55:30 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.1.5.tar", last modified: Thu May 23 04:50:03 2024, max compression
```

## Comparing `medium_to_markdown_py-1.1.4.tar` & `medium_to_markdown_py-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-02 14:55:30.707810 medium_to_markdown_py-1.1.4/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.4/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-05-02 14:55:30.707745 medium_to_markdown_py-1.1.4/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      670 2024-04-29 13:19:17.000000 medium_to_markdown_py-1.1.4/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-02 14:55:30.706376 medium_to_markdown_py-1.1.4/medium_to_markdown/
--rw-r--r--   0 shin       (501) staff       (20)     8414 2024-05-02 14:54:04.000000 medium_to_markdown_py-1.1.4/medium_to_markdown/Parser.py
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-05-02 14:54:35.000000 medium_to_markdown_py-1.1.4/medium_to_markdown/__init__.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-02 14:55:30.707534 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      364 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       19 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-05-02 14:55:30.708116 medium_to_markdown_py-1.1.4/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      612 2024-05-02 14:54:42.000000 medium_to_markdown_py-1.1.4/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-23 04:50:03.321530 medium_to_markdown_py-1.1.5/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.5/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-05-23 04:50:03.321421 medium_to_markdown_py-1.1.5/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      670 2024-04-29 13:19:17.000000 medium_to_markdown_py-1.1.5/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-23 04:50:03.319546 medium_to_markdown_py-1.1.5/medium_to_markdown/
+-rw-r--r--   0 shin       (501) staff       (20)     8758 2024-05-23 04:47:47.000000 medium_to_markdown_py-1.1.5/medium_to_markdown/Parser.py
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-05-23 04:47:47.000000 medium_to_markdown_py-1.1.5/medium_to_markdown/__init__.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-23 04:50:03.321114 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-05-23 04:50:03.000000 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      364 2024-05-23 04:50:03.000000 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-05-23 04:50:03.000000 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-05-23 04:50:03.000000 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       19 2024-05-23 04:50:03.000000 medium_to_markdown_py-1.1.5/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-05-23 04:50:03.321849 medium_to_markdown_py-1.1.5/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      612 2024-05-23 04:47:47.000000 medium_to_markdown_py-1.1.5/setup.py
```

### Comparing `medium_to_markdown_py-1.1.4/LICENSE` & `medium_to_markdown_py-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.4/README.md` & `medium_to_markdown_py-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.4/medium_to_markdown/Parser.py` & `medium_to_markdown_py-1.1.5/medium_to_markdown/Parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
                 if text:
                     parsed_content.append(f"\n## {text}\n")
             elif node.name == "p":
                 if 'pw-post-body-paragraph' in node.get('class', []):
                     text = self.extract_inline(node)
                     if text:
                         parsed_content.append(f"\n{text.strip()}\n")
+            elif node.name == "li":
+                text = self.extract_inline(node)
+                if text:
+                    parsed_content.append(f"\n- {text}\n\n")
             elif node.name == "pre":
                 text = self.extract_inline(node)
                 if text:
                     parsed_content.append(f"```\n{text}\n```\n")
             elif node.name == "source":
                 links_str = node.get('srcset')
                 if links_str:
@@ -178,14 +182,18 @@
                 text = self.parse_formatting_text(node)
                 return f"*{text.strip()}* "
             elif node.name == "br":
                 return "\n"
             elif node.name == "code":
                 text = self.parse_formatting_text(node)
                 return f"`{text.strip()}` "
+            elif node.name == "a":
+                text = self.parse_formatting_text(node)
+                url = node.get('href')
+                return f"[{text}]({url}) "
             else:
                 text = self.parse_formatting_text(node)
                 return text
         else:
             return None
 
     def parse_formatting_text(self,element):
```

### Comparing `medium_to_markdown_py-1.1.4/setup.py` & `medium_to_markdown_py-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium_to_markdown_py',
-    version='1.1.4',
+    version='1.1.5',
     description='medium-to-medium_to_markdown_py-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

