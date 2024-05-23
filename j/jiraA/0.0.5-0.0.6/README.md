# Comparing `tmp/jiraA-0.0.5-py3-none-any.whl.zip` & `tmp/jiraA-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 9684 bytes, number of entries: 16
+Zip file size: 9841 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 16:23 jiraX/__init__.py
 -rw-r--r--  2.0 unx      784 b- defN 24-May-15 15:53 jiraX/backlog.py
 -rw-r--r--  2.0 unx      308 b- defN 24-May-14 16:23 jiraX/base.py
--rw-r--r--  2.0 unx     1321 b- defN 24-May-15 15:28 jiraX/board.py
+-rw-r--r--  2.0 unx     1901 b- defN 24-May-23 16:43 jiraX/board.py
 -rw-r--r--  2.0 unx      823 b- defN 24-May-15 15:28 jiraX/comment.py
 -rw-r--r--  2.0 unx     1499 b- defN 24-May-14 16:23 jiraX/factories.py
--rw-r--r--  2.0 unx     5037 b- defN 24-May-22 18:28 jiraX/issue.py
+-rw-r--r--  2.0 unx     5041 b- defN 24-May-23 15:54 jiraX/issue.py
 -rw-r--r--  2.0 unx     2630 b- defN 24-May-22 17:28 jiraX/project.py
 -rw-r--r--  2.0 unx     1306 b- defN 24-May-15 15:28 jiraX/role.py
 -rw-r--r--  2.0 unx     1184 b- defN 24-May-22 16:55 jiraX/sprint.py
 -rw-r--r--  2.0 unx      787 b- defN 24-May-15 15:28 jiraX/sprintbacklog.py
 -rw-r--r--  2.0 unx     2895 b- defN 24-May-15 16:21 jiraX/user.py
--rw-r--r--  2.0 unx     3296 b- defN 24-May-22 18:28 jiraA-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-22 18:28 jiraA-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-May-22 18:28 jiraA-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1153 b- defN 24-May-22 18:28 jiraA-0.0.5.dist-info/RECORD
-16 files, 23121 bytes uncompressed, 7832 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx     3296 b- defN 24-May-23 16:46 jiraA-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 16:46 jiraA-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-May-23 16:46 jiraA-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1153 b- defN 24-May-23 16:46 jiraA-0.0.6.dist-info/RECORD
+16 files, 23705 bytes uncompressed, 7989 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: jiraX/sprintbacklog.py
 Comment: 
 
 Filename: jiraX/user.py
 Comment: 
 
-Filename: jiraA-0.0.5.dist-info/METADATA
+Filename: jiraA-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: jiraA-0.0.5.dist-info/WHEEL
+Filename: jiraA-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: jiraA-0.0.5.dist-info/top_level.txt
+Filename: jiraA-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: jiraA-0.0.5.dist-info/RECORD
+Filename: jiraA-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jiraX/board.py

```diff
@@ -6,14 +6,36 @@
 	"""
 	Class responsable for documentation boards in Jira
 	"""
 	ERROR = "OS error: {0}"
 
 	def __init__(self, user, apikey, server):
 		Base.__init__(self, user, apikey, server)
+
+	def get_by_project_function(self, project_key, **kwargs):
+		result = []
+		boards = []
+		
+		try:
+			
+			function = kwargs["function"]
+
+			logging.info("Start function: get_by_project_function")
+			result = self.find_by_project(project_key)
+			for board in result:
+				boards.append(board.__dict__)
+				if function is not None:
+					function (data=board.__dict__, topic=kwargs["topic"], extra_data=kwargs["extra_data"])
+				
+		except Exception as e: 
+			logging.error("OS error: {0}".format(e))
+			logging.error(e.__dict__) 
+
+		logging.info("Retrieve All Boards")
+		return boards
 		
 	def find_by_project(self, project_key):
 		"""
 		Responsible for finding all project's boards that user has access
 
 		Arguments:
```

## jiraX/issue.py

```diff
@@ -58,15 +58,15 @@
 		issues = []
 		
 		try:
 			
 			function = kwargs["function"]
 
 			logging.info("Start function: get_by_project_function")
-			result = self.find_by_project('SCRUM')
+			result = self.find_by_project(project_key)
 			for issue in result:
 				issues.append(issue.__dict__)
 				if function is not None:
 					function (data=issue.__dict__, topic=kwargs["topic"], extra_data=kwargs["extra_data"])
 				
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
```

## Comparing `jiraA-0.0.5.dist-info/METADATA` & `jiraA-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiraA
-Version: 0.0.5
+Version: 0.0.6
 Summary: Lib created based on documentaion https://docs.atlassian.com/DAC/rest/jira/6.1.html
 Home-page: https://gitlab.com/integration_seon/libs/application/jira
 Author: Paulo Sérgio dos Santos Júnior
 Author-email: paulossjunior@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `jiraA-0.0.5.dist-info/RECORD` & `jiraA-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 jiraX/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jiraX/backlog.py,sha256=UPSnztuP5_UqSjE5qnhKqwqN91ntFYKnKjPSJNpWfLQ,784
 jiraX/base.py,sha256=jt2W8EInTdgEkCHa91Fupp_vjCjUZrNrwChC-osb0tE,308
-jiraX/board.py,sha256=NlZbWIqpwl7grHv50VABSrDqoU47Yf7snyP0tpfflsM,1321
+jiraX/board.py,sha256=hmyBqWsyiHfvcm4868rlBfiamdeqTllTPhqp2eD3b30,1901
 jiraX/comment.py,sha256=jf3A-g9DgjGQyQqQIMICfMQSUSfUZK7DffEmiKmvETw,823
 jiraX/factories.py,sha256=Ug9FHIpctrJxv1FwEOHqtjJ7iHbCvnBYptucLygvOgE,1499
-jiraX/issue.py,sha256=OIr0yc8JvEfPYCRTlteglXFyijLwHkU22nKikK-7UVw,5037
+jiraX/issue.py,sha256=e9hezRSV-6cJb5d96-s0pG4cP69WPvsqzjiIF66jYBA,5041
 jiraX/project.py,sha256=gTFcwD-uCEV-3v8t2Gq21kKC2ku9zjLIeR6WGFS-ajo,2630
 jiraX/role.py,sha256=amFxvL3Ij4Rzwl5CuKwpAPHgw2EMgWmlstsQZUQwJs0,1306
 jiraX/sprint.py,sha256=MB7SocPAcBTeSQSUQX1NdQRphJjZ-wtswmaxulTgraY,1184
 jiraX/sprintbacklog.py,sha256=UTtOxNDY_NVmlhCBkwa1LSFgx-hDMYI9StfD0jK2aQs,787
 jiraX/user.py,sha256=RTQsx7RVm0j4zyNyjaDRrNLM5DcwVpbJKeRxCUv9IoE,2895
-jiraA-0.0.5.dist-info/METADATA,sha256=W9GEAFJquaSyq6M1J9zQy9PTG3k2ubbezYaDHFMzsgM,3296
-jiraA-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-jiraA-0.0.5.dist-info/top_level.txt,sha256=ALK1II_rDaF8gAa1lmDaKiZ7nr23rPPmgEtSXv03tyY,6
-jiraA-0.0.5.dist-info/RECORD,,
+jiraA-0.0.6.dist-info/METADATA,sha256=G9n9z6IQLB81eELQgob6VMttfQDOSQ344knuYinviAE,3296
+jiraA-0.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+jiraA-0.0.6.dist-info/top_level.txt,sha256=ALK1II_rDaF8gAa1lmDaKiZ7nr23rPPmgEtSXv03tyY,6
+jiraA-0.0.6.dist-info/RECORD,,
```

