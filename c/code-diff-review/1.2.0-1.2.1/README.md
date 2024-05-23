# Comparing `tmp/code_diff_review-1.2.0.tar.gz` & `tmp/code_diff_review-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_diff_review-1.2.0.tar", last modified: Wed May 22 16:52:09 2024, max compression
+gzip compressed data, was "code_diff_review-1.2.1.tar", last modified: Wed May 22 16:57:15 2024, max compression
```

## Comparing `code_diff_review-1.2.0.tar` & `code_diff_review-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/code_diff_review.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/src/publishers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/src/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:57:15.355441 code_diff_review-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:57:15.351441 code_diff_review-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:57:15.351441 code_diff_review-1.2.1/code_diff_review.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:57:15.000000 code_diff_review-1.2.1/code_diff_review.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 16:57:15.000000 code_diff_review-1.2.1/code_diff_review.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:57:15.000000 code_diff_review-1.2.1/code_diff_review.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 16:57:15.000000 code_diff_review-1.2.1/code_diff_review.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 16:57:15.000000 code_diff_review-1.2.1/code_diff_review.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 16:57:15.000000 code_diff_review-1.2.1/code_diff_review.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:57:15.355441 code_diff_review-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:57:15.351441 code_diff_review-1.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/src/publishers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-22 16:57:10.000000 code_diff_review-1.2.1/src/script.py
```

### Comparing `code_diff_review-1.2.0/LICENSE` & `code_diff_review-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.2.0/PKG-INFO` & `code_diff_review-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-diff-review
-Version: 1.2.0
+Version: 1.2.1
 Summary: Review your code diff.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `code_diff_review-1.2.0/README.md` & `code_diff_review-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.2.0/code_diff_review.egg-info/PKG-INFO` & `code_diff_review-1.2.1/code_diff_review.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-diff-review
-Version: 1.2.0
+Version: 1.2.1
 Summary: Review your code diff.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `code_diff_review-1.2.0/setup.py` & `code_diff_review-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='code-diff-review',
-    version='1.2.0',
+    version='1.2.1',
     author='Agustin Rios',
     author_email='arios6@uc.cl',
     description='Review your code diff.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=open("./requirements.txt").read().splitlines(),
```

### Comparing `code_diff_review-1.2.0/src/publishers.py` & `code_diff_review-1.2.1/src/publishers.py`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.2.0/src/script.py` & `code_diff_review-1.2.1/src/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def extract_message(text):
     pattern = r'\[C:START\](.*?)\[C:END\]'
     matcher = re.search(pattern, text, re.DOTALL)
     if matcher:
         return matcher.group(1)
     return None
 
-def main(openai_key, assistant_id, token, repo, message, gh_before, sha, author, webhook, websecret):
+def review(openai_key, assistant_id, token, repo, message, gh_before, sha, author, webhook, websecret):
     git_publisher = GitIssuePublisher(repo, token, sha, author)
     web_publisher = WebPublisher(webhook, websecret)
 
     try:
         diff = subprocess.check_output(['git', 'diff', gh_before, sha, "--word-diff"]).decode('utf-8')
     except subprocess.CalledProcessError as e:
         print(f"Error generating git diff: {e}")
@@ -51,15 +51,15 @@
         print(f"Error decoding JSON response: {response}")
         print(response)
     except Exception as e:
         print(f"Unexpected error: {e}")
 
 
         
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(description="Commit message and diff handler with OpenAI assistance.")
 
     #### Need tokens
     parser.add_argument('--openai-key', default=os.getenv('OPENAI_API_KEY'), help='OpenAI API key')
     parser.add_argument('--assistant-id', default=os.getenv('OPENAI_ASSISTANT_ID'), help='OpenAI assistant ID')
     parser.add_argument('--token', default=os.getenv('GH_TOKEN'), help='GitHub token')
 
@@ -74,8 +74,11 @@
 
     #### External Api to post
     parser.add_argument('--webhook', default=os.getenv('WEBHOOK'), help='Webhook URL')
     parser.add_argument('--websecret', default=os.getenv('WEBSECRET'), help='Webhook secret')
 
     args = parser.parse_args()
 
-    main(args.openai_key, args.assistant_id, args.token, args.repo, args.message, args.gh_before, args.sha, args.author, args.webhook, args.websecret)
+    review(args.openai_key, args.assistant_id, args.token, args.repo, args.message, args.gh_before, args.sha, args.author, args.webhook, args.websecret)
+
+if __name__ == "__main__":
+    main()
```

