# Comparing `tmp/shipyard_mode-0.2.0a0.tar.gz` & `tmp/shipyard_mode-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_mode-0.2.0a0.tar", max compression
+gzip compressed data, was "shipyard_mode-0.2.1.tar", max compression
```

## Comparing `shipyard_mode-0.2.0a0.tar` & `shipyard_mode-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      468 2024-04-19 15:30:35.566956 shipyard_mode-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-05-12 18:48:21.835911 shipyard_mode-0.2.0a0/shipyard_mode/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.748654 shipyard_mode-0.2.0a0/shipyard_mode/cli/__init__.py
--rw-r--r--   0        0        0      319 2024-02-05 20:53:35.439318 shipyard_mode-0.2.0a0/shipyard_mode/cli/authtest.py
--rw-r--r--   0        0        0     5237 2024-04-19 15:30:17.496214 shipyard_mode-0.2.0a0/shipyard_mode/cli/download_result_as_file.py
--rw-r--r--   0        0        0      417 2024-03-25 14:04:18.953400 shipyard_mode-0.2.0a0/shipyard_mode/cli/exit_codes.py
--rw-r--r--   0        0        0     5767 2024-04-19 15:30:19.450962 shipyard_mode-0.2.0a0/shipyard_mode/cli/run_report.py
--rw-r--r--   0        0        0     1483 2024-04-19 15:23:26.272268 shipyard_mode-0.2.0a0/shipyard_mode/mode.py
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 shipyard_mode-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0      528 2024-05-23 14:38:11.475017 shipyard_mode-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-05-12 18:48:21.835911 shipyard_mode-0.2.1/shipyard_mode/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.748654 shipyard_mode-0.2.1/shipyard_mode/cli/__init__.py
+-rw-r--r--   0        0        0      319 2024-02-05 20:53:35.439318 shipyard_mode-0.2.1/shipyard_mode/cli/authtest.py
+-rw-r--r--   0        0        0     5215 2024-04-19 17:48:30.549286 shipyard_mode-0.2.1/shipyard_mode/cli/download_result_as_file.py
+-rw-r--r--   0        0        0      417 2024-04-19 17:48:30.549565 shipyard_mode-0.2.1/shipyard_mode/cli/exit_codes.py
+-rw-r--r--   0        0        0     5745 2024-04-19 17:48:30.550082 shipyard_mode-0.2.1/shipyard_mode/cli/run_report.py
+-rw-r--r--   0        0        0     1397 2024-05-23 14:38:11.475370 shipyard_mode-0.2.1/shipyard_mode/mode.py
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 shipyard_mode-0.2.1/PKG-INFO
```

### Comparing `shipyard_mode-0.2.0a0/shipyard_mode/cli/download_result_as_file.py` & `shipyard_mode-0.2.1/shipyard_mode/cli/download_result_as_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,18 +98,17 @@
         f"{mode_api_base}/reports/{report_id}/exports/runs/{run_id}/pdf/download"
         if file_type == "pdf"
         else f"{mode_api_base}/reports/{report_id}/runs/{run_id}/results/content.{file_type}"
     )
 
 
 def run_mode_request(token_id, token_password, report_url):
-    headers = {"Content-Type": "application/json", "Accept": "application/hal+json"}
     report_request = requests.get(
         report_url,
-        headers=headers,
+        headers={"Content-Type": "application/json", "Accept": "application/hal+json"},
         auth=HTTPBasicAuth(token_id, token_password),
         stream=True,
     )
 
     assess_request_status(report_request)
     return report_request
```

### Comparing `shipyard_mode-0.2.0a0/shipyard_mode/cli/run_report.py` & `shipyard_mode-0.2.1/shipyard_mode/cli/run_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 def execute_run_report(account_name, report_id, token_id, token_password):
     """Executes a mode report run
     see: https://mode.com/developer/api-reference/analytics/report-runs/#runReport
     """
     mode_api_base = f"https://app.mode.com/api/{account_name}"
     run_report_endpoint = f"{mode_api_base}/reports/{report_id}/runs"
 
-    headers = {"Content-Type": "application/json", "Accept": "application/hal+json"}
     report_request = requests.post(
         run_report_endpoint,
         data={},
-        headers=headers,
+        headers={"Content-Type": "application/json", "Accept": "application/hal+json"},
         auth=HTTPBasicAuth(token_id, token_password),
     )
 
     status_code = report_request.status_code
     # save report data
     run_report_data = report_request.json()
```

### Comparing `shipyard_mode-0.2.0a0/shipyard_mode/mode.py` & `shipyard_mode-0.2.1/shipyard_mode/mode.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class ModeClient(DataVisualization):
     def __init__(self, api_token: str, api_secret: str, account: str) -> None:
         self.api_token = api_token
         self.api_secret = api_secret
         self.account = account
         self.mode_api_base = f"https://app.mode.com/api/{self.account}"
-        super().__init__(api_token=api_token, api_secret=api_secret, account=account)
 
     def connect(self):
         try:
             response = requests.get(
                 url=f"{self.mode_api_base}/spaces",
                 headers={
                     "Content-Type": "application/json",
```

### Comparing `shipyard_mode-0.2.0a0/PKG-INFO` & `shipyard_mode-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-mode
-Version: 0.2.0a0
+Version: 0.2.1
 Summary: A local client for connecting and working with Mode
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

