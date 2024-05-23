# Comparing `tmp/code_diff_review-1.2.2.tar.gz` & `tmp/code_diff_review-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_diff_review-1.2.2.tar", last modified: Thu May 23 16:54:29 2024, max compression
+gzip compressed data, was "code_diff_review-1.3.0.tar", last modified: Thu May 23 17:22:44 2024, max compression
```

## Comparing `code_diff_review-1.2.2.tar` & `code_diff_review-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:54:29.076049 code_diff_review-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-23 16:54:29.076049 code_diff_review-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:54:29.076049 code_diff_review-1.2.2/code_diff_review.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-23 16:54:29.000000 code_diff_review-1.2.2/code_diff_review.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 16:54:29.000000 code_diff_review-1.2.2/code_diff_review.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:54:29.000000 code_diff_review-1.2.2/code_diff_review.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 16:54:29.000000 code_diff_review-1.2.2/code_diff_review.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 16:54:29.000000 code_diff_review-1.2.2/code_diff_review.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 16:54:29.000000 code_diff_review-1.2.2/code_diff_review.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:54:29.076049 code_diff_review-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:54:29.076049 code_diff_review-1.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/src/publishers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-23 16:54:25.000000 code_diff_review-1.2.2/src/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:22:44.856990 code_diff_review-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-23 17:22:44.856990 code_diff_review-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:22:44.852990 code_diff_review-1.3.0/code_diff_review.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-23 17:22:44.000000 code_diff_review-1.3.0/code_diff_review.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 17:22:44.000000 code_diff_review-1.3.0/code_diff_review.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:22:44.000000 code_diff_review-1.3.0/code_diff_review.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 17:22:44.000000 code_diff_review-1.3.0/code_diff_review.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 17:22:44.000000 code_diff_review-1.3.0/code_diff_review.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 17:22:44.000000 code_diff_review-1.3.0/code_diff_review.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:22:44.856990 code_diff_review-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:22:44.852990 code_diff_review-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/src/publishers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-23 17:22:40.000000 code_diff_review-1.3.0/src/script.py
```

### Comparing `code_diff_review-1.2.2/LICENSE` & `code_diff_review-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.2.2/PKG-INFO` & `code_diff_review-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-diff-review
-Version: 1.2.2
+Version: 1.3.0
 Summary: Review your code diff.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `code_diff_review-1.2.2/README.md` & `code_diff_review-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.2.2/code_diff_review.egg-info/PKG-INFO` & `code_diff_review-1.3.0/code_diff_review.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-diff-review
-Version: 1.2.2
+Version: 1.3.0
 Summary: Review your code diff.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `code_diff_review-1.2.2/setup.py` & `code_diff_review-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='code-diff-review',
-    version='1.2.2',
+    version='1.3.0',
     author='Agustin Rios',
     author_email='arios6@uc.cl',
     description='Review your code diff.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=open("./requirements.txt").read().splitlines(),
```

### Comparing `code_diff_review-1.2.2/src/publishers.py` & `code_diff_review-1.3.0/src/publishers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.user = user
 
     def __get_repo(self):
         return self.github.get_repo(self.repo)
     
     def publish(self, body: str):
         title = f"Automated Issue for {self.user};\n [commit {self.sha}]"
-        return self.__get_repo().create_issue(title, body=body, assignee=self.user)
+        return self.__get_repo().create_issue(title, body=body) # assignee=self.user)
     
     def generate_report(self, data):
         report = [
             f"### Commit Review Summary\n",
             f"**Commit SHA:** {self.sha}\n",
             f"**Message:**\n- **Written:** {data['message']['message']}"
         ]
```

### Comparing `code_diff_review-1.2.2/src/script.py` & `code_diff_review-1.3.0/src/script.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,19 +44,26 @@
         print("No response extracted from the note.")
         return
 
     try:
         response = json.loads(response)
         response['message']['suggested'] = response['message']['message']
         response['message']['message'] = message
-        git_publisher.publish(git_publisher.generate_report(response))
-        web_publisher.publish(web_publisher.sort_data(response, {"user": author, "sha": sha, "repo": repo}))
     except json.JSONDecodeError:
         print(f"Error decoding JSON response: {response}")
-        print(response)
+    except Exception as e:
+        print(f"Unexpected error: {e}")
+
+    try:
+        git_publisher.publish(git_publisher.generate_report(response))
+    except Exception as e:
+        print(f"Unexpected error: {e}")
+
+    try:
+        web_publisher.publish(web_publisher.sort_data(response, {"user": author, "sha": sha, "repo": repo}))
     except Exception as e:
         print(f"Unexpected error: {e}")
 
 
         
 def main():
     parser = argparse.ArgumentParser(description="Commit message and diff handler with OpenAI assistance.")
```

