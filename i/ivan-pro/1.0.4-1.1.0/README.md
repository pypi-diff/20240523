# Comparing `tmp/ivan_pro-1.0.4-py3-none-any.whl.zip` & `tmp/ivan_pro-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 17700 bytes, number of entries: 20
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:35 ivan/__init__.py
--rw-r--r--  2.0 unx      219 b- defN 24-Apr-23 16:35 ivan/cli.py
--rw-r--r--  2.0 unx      400 b- defN 24-Apr-23 16:35 ivan/plugins/__init__.py
--rw-r--r--  2.0 unx     2766 b- defN 24-Apr-23 16:35 ivan/plugins/database.py
--rw-r--r--  2.0 unx     8153 b- defN 24-Apr-23 16:35 ivan/plugins/dbconfig.py
--rw-r--r--  2.0 unx     3664 b- defN 24-Apr-23 16:35 ivan/plugins/display.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-23 16:35 ivan/plugins/export.py
--rw-r--r--  2.0 unx     9092 b- defN 24-Apr-23 16:35 ivan/plugins/find.py
--rw-r--r--  2.0 unx     8853 b- defN 24-Apr-23 16:35 ivan/plugins/ip.py
--rw-r--r--  2.0 unx     1727 b- defN 24-Apr-23 16:35 ivan/plugins/keys.py
--rw-r--r--  2.0 unx     1131 b- defN 24-Apr-23 16:35 ivan/plugins/query_export.py
--rw-r--r--  2.0 unx     8734 b- defN 24-Apr-23 16:35 ivan/plugins/sc_vuln_export.py
--rw-r--r--  2.0 unx      573 b- defN 24-Apr-23 16:35 ivan/plugins/scan.py
--rw-r--r--  2.0 unx     7016 b- defN 24-Apr-23 16:35 ivan/plugins/scan_evaluation.py
--rw-r--r--  2.0 unx      240 b- defN 24-Apr-23 16:35 ivan/plugins/update.py
--rw-r--r--  2.0 unx     2338 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/RECORD
-20 files, 57922 bytes uncompressed, 15146 bytes compressed:  73.9%
+Zip file size: 20400 bytes, number of entries: 21
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 16:36 ivan/__init__.py
+-rw-r--r--  2.0 unx      219 b- defN 24-May-23 16:36 ivan/cli.py
+-rw-r--r--  2.0 unx      400 b- defN 24-May-23 16:36 ivan/plugins/__init__.py
+-rw-r--r--  2.0 unx     4175 b- defN 24-May-23 16:36 ivan/plugins/database.py
+-rw-r--r--  2.0 unx     5219 b- defN 24-May-23 16:36 ivan/plugins/dbconfig.py
+-rw-r--r--  2.0 unx     5203 b- defN 24-May-23 16:36 ivan/plugins/display.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-23 16:36 ivan/plugins/export.py
+-rw-r--r--  2.0 unx     9092 b- defN 24-May-23 16:36 ivan/plugins/find.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-23 16:36 ivan/plugins/ip.py
+-rw-r--r--  2.0 unx     1727 b- defN 24-May-23 16:36 ivan/plugins/keys.py
+-rw-r--r--  2.0 unx     1131 b- defN 24-May-23 16:36 ivan/plugins/query_export.py
+-rw-r--r--  2.0 unx     9049 b- defN 24-May-23 16:36 ivan/plugins/sc_vuln_export.py
+-rw-r--r--  2.0 unx     5960 b- defN 24-May-23 16:36 ivan/plugins/scan.py
+-rw-r--r--  2.0 unx     7397 b- defN 24-May-23 16:36 ivan/plugins/scan_evaluation.py
+-rw-r--r--  2.0 unx     8878 b- defN 24-May-23 16:36 ivan/plugins/scanidv_vuln_export.py
+-rw-r--r--  2.0 unx      341 b- defN 24-May-23 16:36 ivan/plugins/update.py
+-rw-r--r--  2.0 unx     2338 b- defN 24-May-23 16:37 ivan_pro-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 16:37 ivan_pro-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 24-May-23 16:37 ivan_pro-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-23 16:37 ivan_pro-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1671 b- defN 24-May-23 16:37 ivan_pro-1.1.0.dist-info/RECORD
+21 files, 73091 bytes uncompressed, 17700 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -36,26 +36,29 @@
 
 Filename: ivan/plugins/scan.py
 Comment: 
 
 Filename: ivan/plugins/scan_evaluation.py
 Comment: 
 
+Filename: ivan/plugins/scanidv_vuln_export.py
+Comment: 
+
 Filename: ivan/plugins/update.py
 Comment: 
 
-Filename: ivan_pro-1.0.4.dist-info/METADATA
+Filename: ivan_pro-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: ivan_pro-1.0.4.dist-info/WHEEL
+Filename: ivan_pro-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: ivan_pro-1.0.4.dist-info/entry_points.txt
+Filename: ivan_pro-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ivan_pro-1.0.4.dist-info/top_level.txt
+Filename: ivan_pro-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ivan_pro-1.0.4.dist-info/RECORD
+Filename: ivan_pro-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ivan/plugins/database.py

```diff
@@ -86,7 +86,45 @@
                             OSes
     ) VALUES(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)'''
 
     cur = conn.cursor()
     cur.execute('pragma journal_mode=wal;')
     cur.execute(sql, vulns)
 
+
+def insert_scanid(conn, scanid):
+    sql = '''INSERT or IGNORE into scanid(
+                            asset_ip, 
+                            asset_uuid, 
+                            asset_hostname, 
+                            first_found, 
+                            last_found, 
+                            output, 
+                            plugin_id, 
+                            plugin_name, 
+                            plugin_family, 
+                            port, 
+                            protocol, 
+                            severity,
+                            repo_name,
+                            repo_id,
+                            uniqueness,
+                            cves,
+                            score,
+                            exploit,
+                            xrefs,
+                            synopsis, 
+                            see_also,
+                            solution,
+                            version, 
+                            description, 
+                            cvss3_base_score,
+                            cvss3_temporal_score,
+                            cvss_base_score,
+                            cvss_temporal_score,
+                            OSes
+    ) VALUES(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)'''
+
+    cur = conn.cursor()
+    cur.execute('pragma journal_mode=wal;')
+    cur.execute(sql, scanid)
+
```

## ivan/plugins/dbconfig.py

```diff
@@ -60,129 +60,51 @@
                             OSes text,
                             url text
                             );"""
     vuln_conn.execute('pragma journal_mode=wal;')
     create_table(vuln_conn, vuln_table)
 
 
-def create_assets_table():
+def create_scanid_table():
     database = r"ivan.db"
-    asset_conn = new_db_connection(database)
-    create_asset_table = """CREATE TABLE IF NOT EXISTS assets (
-                            ip_address text,
-                            hostname text,
-                            fqdn text,
-                            uuid text PRIMARY KEY,
-                            first_found text,
+    scanid_conn = new_db_connection(database)
+    scanid_table = """CREATE TABLE IF NOT EXISTS scanid (
+                            asset_ip text, 
+                            asset_uuid text, 
+                            asset_hostname text, 
+                            first_found text, 
                             last_found text, 
-                            operating_system text,
-                            mac_address text, 
-                            agent_uuid text,
-                            last_licensed_scan_date text,
-                            network text,
-                            acr text,
-                            aes text,
-                            aws_id text,
-                            aws_ec2_instance_state text,
-                            aws_ec2_name text,
-                            aws_ec2_region text,
-                            aws_availability_zone text,
-                            gcp_instance_id text,
-                            gcp_project_id text,
-                            gcp_zone text,
-                            url text
-                            );"""
-    asset_conn.execute('pragma journal_mode=wal;')
-    create_table(asset_conn, create_asset_table)
-
-
-def create_tag_table():
-    database = r"ivan.db"
-    tag_conn = new_db_connection(database)
-    create_tags_table = """CREATE TABLE IF NOT EXISTS tags (
-                        tag_id integer PRIMARY KEY,
-                        asset_uuid text,
-                        asset_ip,
-                        tag_key text,
-                        tag_uuid text,
-                        tag_value text,
-                        tag_added_date text
-                        );"""
-    tag_conn.execute('pragma journal_mode=wal;')
-    create_table(tag_conn, create_tags_table)
-
-
-def create_apps_table():
-    database = r"ivan.db"
-    app_conn = new_db_connection(database)
-    create_apps = """CREATE TABLE IF NOT EXISTS apps (
-                            name text,
-                            uuid text PRIMARY KEY, 
-                            target text, 
-                            scan_completed_time text,
-                            pages_crawled text,
-                            requests_made text, 
-                            critical_count text,
-                            high_count text,
-                            medium_count text,
-                            low_count text, 
-                            info_count text,
-                            owasp text,
-                            tech_list text,
-                            config_id text,
-                            notes text,
-                            asset_uuid text
-                            );"""
-    app_conn.execute('pragma journal_mode=wal;')
-
-    create_table(app_conn, create_apps)
-
-
-def create_compliance_table():
-    database = r"ivan.db"
-    compliance_conn = new_db_connection(database)
-    create_compliance = """CREATE TABLE IF NOT EXISTS compliance (
-                            asset_uuid text,
-                            actual_value text,
-                            audit_file text,
-                            check_id text,
-                            check_info text,
-                            check_name text,
-                            expected_value text,
-                            first_seen text,
-                            last_seen text,
-                            plugin_id text,
-                            reference text,
-                            see_also text,
-                            solution text,
-                            status text 
-                            );"""
-
-    create_table(compliance_conn, create_compliance)
-
-
-def create_fixed_table():
-    database = r"ivan.db"
-    fixed_conn = new_db_connection(database)
-    fixed_table = """CREATE TABLE IF NOT EXISTS fixed (
-                            asset_uuid text,  
                             output text, 
                             plugin_id text, 
-                            plugin_name text,  
-                            port text,
-                            first_found text,
-                            last_fixed text,
-                            last_found text,
-                            severity text,
-                            delta text,
-                            pass_fail text,
-                            state text,
-                            special_url text
+                            plugin_name text, 
+                            plugin_family text, 
+                            port text, 
+                            protocol text, 
+                            severity text, 
+                            repo_name text, 
+                            repo_id text, 
+                            uniqueness text, 
+                            cves text,
+                            score text,
+                            exploit text,
+                            xrefs text,
+                            synopsis text, 
+                            see_also text,
+                            solution text,
+                            version text, 
+                            description text, 
+                            cvss3_base_score text,
+                            cvss3_temporal_score text,
+                            cvss_base_score text,
+                            cvss_temporal_score text,
+                            OSes text,
+                            url text
                             );"""
-    fixed_conn.execute(fixed_table)
+    scanid_conn.execute('pragma journal_mode=wal;')
+    create_table(scanid_conn, scanid_table)
 
 
 def create_plugins_table():
     database = r"ivan.db"
     app_conn = new_db_connection(database)
     create_plugins = """CREATE TABLE IF NOT EXISTS plugins (
                             scan_uuid text,
```

## ivan/plugins/display.py

```diff
@@ -63,33 +63,36 @@
 
     try:
         click.echo("\n{:60s} {:10s} {:30s} {}".format("Scan Name", "Scan ID", "Status", "UUID"))
         click.echo("-" * 150)
 
         for scan in sc.scans.list()['usable']:
             try:
-                click.echo("{:60s} {:10s} {:30s} {}".format(str(scan['name']), str(scan['id']), str(scan['status']),
+                click.echo("{:60s} {:10s} {:30s} {}".format(str(scan['name']), str(scan['id']),
+                                                            str(scan['status']),
                                                             str(scan['uuid'])))
             except KeyError:
-                click.echo("{:60s} {:10s} {:30s} {}".format(str(scan['name']), str(scan['id']), str(scan['status']),
+                click.echo("{:60s} {:10s} {:30s} {}".format(str(scan['name']), str(scan['id']),
+                                                            str(scan['status']),
                                                             "No UUID"))
         click.echo()
     except AttributeError:
         click.echo("\nCheck your permissions or your API keys\n")
 
 
 @display.command(help="Display  all of the Users")
 def users():
     sc = tenb_connection()
 
     try:
         click.echo("\n{:34s} {:40s} {:40s} {:10s} {}".format("User Name", "Login Email", "UUID", "ID", "Locked"))
         click.echo("-" * 150)
         for user in sc.users.list():
-            click.echo("{:34s} {:40s} {:40s} {:10s} {}".format(str(user["username"]), str(user["email"]), str(user['uuid']), str(user['id']), str(user['locked'])))
+            click.echo("{:34s} {:40s} {:40s} {:10s} {}".format(str(user["username"]), str(user["email"]),
+                                                               str(user['uuid']), str(user['id']), str(user['locked'])))
         click.echo()
     except AttributeError:
         click.echo("\nCheck your permissions or your API keys\n")
 
 
 @display.command(help="Display All Assets found in the last 30 days")
 def assets():
@@ -107,7 +110,33 @@
         for asset in asset_list:
 
             click.echo("{:16} {:65} {:40}".format(asset[0], asset[1], asset[2]))
 
         click.echo("\nTotal: {}\n\n".format(len(asset_list)))
     except AttributeError:
         click.echo("\nCheck your permissions or your API keys\n")
+
+
+@display.command(help="Display Scan Instances")
+def instances():
+    sc = tenb_connection()
+    try:
+        click.echo("\n{:60s} {:10s} {:15s} {:20s} {:20s} {}".format("Scan Name", "Scan ID", "Status",
+                                                                    "Start Time", "Finish Time", "Assets Scanned"))
+        click.echo("-" * 150)
+        usable_list = []
+        for scan in sc.scan_instances.list()['usable']:
+            usable_list.append(scan['id'])
+
+        for scanid in usable_list:
+            scan = sc.scan_instances.details(id=scanid)
+            try:
+                click.echo("{:60s} {:10s} {:15s} {:20s} {:20s} {}".format(str(scan['name']), str(scan['id']),
+                                                                          str(scan['status']), str(scan['startTime']),
+                                                                          str(scan['finishTime']),
+                                                                          str(scan['progress']['scannedSize'])))
+            except KeyError:
+                click.echo("{:60s} {:10s} {:30s} {}".format(str(scan['name']), str(scan['id']),
+                                                            str(scan['status']), "No UUID"))
+        click.echo()
+    except AttributeError:
+        click.echo("\nCheck your permissions or your API keys\n")
```

## ivan/plugins/sc_vuln_export.py

```diff
@@ -21,26 +21,32 @@
             sc = TenableSC(hostname, port=port)
             # login to SC
             sc.login(access_key=access_key, secret_key=secret_key)
 
             return sc
 
 
-def parse_data():
+def parse_data(scan_id):
     sc = tenb_connection()
     database = r"ivan.db"
     vuln_conn = new_db_connection(database)
     vuln_conn.execute('pragma journal_mode=wal;')
     vuln_conn.execute('pragma cashe_size=-10000')
     vuln_conn.execute('pragma synchronous=OFF')
+
     with vuln_conn:
         try:
+            if scan_id:
+                click.echo("\nPulling Vuln Data from scan {} from Tenable.sc\n".format(scan_id))
+                scan_list = sc.analysis.vulns(tools='vulndetails', scan_id=scan_id)
+            else:
+                click.echo("\nPulling All Vulnerability Data from Tenable.sc\n")
+                scan_list = sc.analysis.vulns(tools='vulndetails')
 
-            # loop through all of the vulns in this chunk
-            for vulns in sc.analysis.vulns(tool='vulndetails'):
+            for vulns in scan_list:
                 # create a blank list to append asset details
                 vuln_list = []
                 # Try block to ignore assets without IPs
                 try:
                     try:
                         ipv4 = vulns['ip']
                         vuln_list.append(ipv4)
@@ -232,27 +238,27 @@
         except TypeError:
             click.echo("Your Export has no data.  It may have expired")
 
     vuln_conn.close()
     sc.logout()
 
 
-def vuln_export():
+def vuln_export(scan_id):
     start = time.time()
 
     database = r"ivan.db"
     drop_conn = new_db_connection(database)
     drop_conn.execute('pragma journal_mode=wal;')
 
     # Right now we just drop the table.  Eventually I will actually update the database
     drop_tables(drop_conn, 'vulns')
 
     create_vulns_table()
 
-    parse_data()
+    parse_data(scan_id=scan_id)
 
     click.echo("\nCreating a few indexes to make queries faster.\n")
     db_query("CREATE INDEX vulns_plugin_id on vulns (plugin_id);")
     db_query("CREATE INDEX vulns_ports on vulns (port);")
     db_query("CREATE INDEX vulns_cves on vulns (cves);")
     end = time.time()
```

## ivan/plugins/scan.py

```diff
@@ -1,24 +1,159 @@
 import click
 from .scan_evaluation import evaluate_a_scan
 from .sc_vuln_export import tenb_connection
+from .scanidv_vuln_export import tenb_connection, scanid_export
 
 
 @click.group(help="Start and Evaluate Scans")
 def scan():
     pass
 
 
-@scan.command()
-def evaluate():
-    evaluate_a_scan()
+@scan.command(help="Evaluate a specific scan or the entire database")
+@click.option("--scanid", default=None, help="A Scan ID you want to evaluate")
+@click.option("-full", is_flag=True, help="Evaluate entire available history")
+def evaluate(full, scanid):
+
+    if full:
+        evaluate_a_scan(table="vulns")
+
+    elif scanid:
+        # Create new table named scan_id
+        # download data into new table
+        scanid_export(scanid)
+
+        evaluate_a_scan(table=scanid)
+    else:
+        click.echo("\nYou must select full or select a scanid to evaluate\n")
 
 
 @scan.command(help="Start a valid Scan by Scan ID")
 @click.argument('scan_id')
 @click.option('--targets', default=None, help="Start the scan with alternative targets")
 def start(scan_id, targets):
     tsc = tenb_connection()
     if targets is None:
         tsc.scans.launch(scan_id)
     else:
         tsc.scans.launch(scan_id, targets=targets)
+
+
+@scan.command(help="Get details on a Scan")
+@click.argument('scan_id')
+def details(scan_id):
+    sc = tenb_connection()
+    scan_details = sc.scan_instances.details(id=scan_id)
+    import pprint
+    #pprint.pprint(scan_details)
+
+    click.echo("\nScan Details")
+    click.echo("-" * 75)
+    click.echo()
+
+    # Grab scan data
+    scan_duration = scan_details['scanDuration']
+    scanned_ips = scan_details['scannedIPs']
+    start_time = scan_details['startTime']
+    current_status = scan_details['status']
+    total_checks = scan_details['totalChecks']
+    total_ips = scan_details['totalIPs']
+    completed_checks = scan_details['progress']['completedChecks']
+    completed_ips = scan_details['progress']['completedIPs']
+    checks_per_host = scan_details['progress']['checksPerHost']
+    scanned_size = scan_details['progress']['scannedSize']
+    deadhost_size = scan_details['progress']['deadHostSize']
+    distributed_size = scan_details['progress']['distributedSize']
+    average = (int(scan_duration) / int(scanned_size)) / 60
+
+    click.echo("{:40s}{}".format("Current Status: ", current_status))
+    click.echo("{:40s}{}".format("Scanned Start time: ", start_time))
+    click.echo("{:40s}{}{}".format("Scan Duration: ", scan_duration, " Seconds"))
+
+    click.echo("-" * 50)
+    click.echo("-" * 50)
+
+    click.echo("\nTarget Details")
+    click.echo("-" * 75)
+    click.echo()
+
+    click.echo("{:40s}{}".format("Total IPs Targeted: ", total_ips))
+    click.echo("{:40s}{}".format("Total number of IPs scanned:",scanned_ips))
+    click.echo("{:40s}{}".format("Assets found in the scan", scanned_size))
+    click.echo("{:40s}{}".format("Total number of Dead Hosts", deadhost_size))
+    click.echo("{:40s}{}".format("Total Distributed Size", distributed_size))
+    click.echo("{:40s}{}".format("Total Completed IPs", completed_ips))
+
+    click.echo("-" * 50)
+    click.echo("-" * 50)
+
+    click.echo("\nPlugin Details")
+    click.echo("-" * 75)
+    click.echo()
+    click.echo("{:40s}{}".format("Total plugins performed: ",total_checks))
+    click.echo("{:40s}{}".format("Total Completed Plugins: ", completed_checks))
+    click.echo("{:40s}{}".format("Total Plugins per host: ", checks_per_host))
+    click.echo("{:40s}{}{}".format("Avg Duration per asset: ", str(average), " mins"))
+
+    click.echo("-" * 50)
+    click.echo("-" * 50)
+
+    click.echo("\nScanner Details")
+    click.echo("-" * 75)
+    click.echo()
+    scanner_details = scan_details['progress']['scanners']
+
+    for scanners in scanner_details:
+        chunk_completed = scanners['chunkCompleted']
+        completed_checks = scanners['completedChecks']
+        dead_host_size = scanners['deadHostSize']
+        distributed_size_by_scanner = scanners['distributedSize']
+        scanner_name = scanners['name']
+        asset_count = scanners['scannedSize']
+
+        click.echo("{:40s}{}".format("Scanner Name", scanner_name))
+        click.echo("-" * 50)
+        click.echo("{:40s}{}".format("   -Total Chunks Completed", chunk_completed))
+        click.echo("{:40s}{}".format("   -Total Checks Completed", completed_checks))
+        click.echo("{:40s}{}".format("   -Dead hosts found by the Scanner", dead_host_size))
+        click.echo("{:40s}{}".format("   -IPs distributed to the scanner", distributed_size_by_scanner))
+        click.echo("{:40s}{}".format("   -Assets found by the scanner", asset_count))
+        click.echo("-" * 50)
+        click.echo()
+    click.echo("-" * 50)
+    click.echo("-" * 50)
+
+    click.echo("\nImport Details")
+    click.echo("-" * 75)
+    click.echo()
+
+    import_duration = scan_details['importDuration']
+    import_finish = scan_details['importFinish']
+    import_start = scan_details['importStart']
+    import_status = scan_details['importStatus']
+
+    click.echo("{:40s}{}{}".format("Import Duration", import_duration, " Seconds"))
+    click.echo("{:40s}{}".format("Import Start Time", import_start))
+    click.echo("{:40s}{}".format("Import Finish Time", import_finish))
+    click.echo("{:40s}{}".format("Import Status", import_status))
+    click.echo("-" * 50)
+    click.echo("-" * 50)
+
+    click.echo("\nError Details")
+    click.echo("-" * 75)
+    click.echo()
+
+    error_details = scan_details['errorDetails']
+    error_sync_details = scan_details['ioSyncErrorDetails']
+    import_errors = scan_details['importErrorDetails']
+
+    click.echo("{:40s}{}".format("Error Details:\n", error_details))
+    click.echo("{:40s}{}".format("Tenable VM Sync Error Details:\n", error_sync_details))
+    click.echo("{:40s}{}".format("Import Error Details:\n", import_errors))
+
+
+@scan.command(help="Export a Scan")
+@click.argument('scan_id')
+def export(scan_id):
+    tsc = tenb_connection()
+    with open('scan-id-{}.nessus'.format(scan_id), 'wb') as fobj:
+        tsc.scan_instances.export_scan(scan_id, fobj)
```

## ivan/plugins/scan_evaluation.py

```diff
@@ -1,41 +1,57 @@
 import click
 from .database import db_query
 import csv
 
 
-def grab_hop_count(uuid):
+def grab_hop_count(table, ipaddy):
+
+    if table != "vulns":
+        # Set the table properly
+        table = "scanid"
     # grab the output of 10287 - Trace Route
     try:
-        hop_count_data = db_query("select output from vulns where asset_uuid='{}' and plugin_id='10287';".format(uuid))
+        hop_count_data = db_query("select output from {} where asset_ip='{}' and plugin_id='10287';".format(table, ipaddy))
         # Send the raw data back
-        return hop_count_data
+        hopcount = hop_count_data[0][-1].split(" ")[-1]
+
+        if "way" in hopcount:
+            hopcount = hop_count_data[0][-1].split(" ")[-7]
+            if "an" in hopcount:
+                print("Error")
+                return "error"
+
+            return hopcount
+        else:
+            return hopcount
     except:
         return "none"
 
 
-def evaluate_a_scan():
-    # Since no scanid was provided we assume the user wants stats on all scans
+def evaluate_a_scan(table):
     click.echo("*" * 100)
     click.echo("\nThis command uses the 19506 plugin data found in the navi.db\n"
                "Run a navi update command to refresh the database.\n")
     click.echo("*" * 100)
     # Pull all 19506 Plugins from the DB
-    plugin_data = db_query("select asset_ip, asset_uuid, output from vulns where plugin_id='19506';")
+    if table != "vulns":
+        table = "scanid"
+    plugin_data = db_query("select asset_ip, output from {} where plugin_id='19506';".format(table))
 
     # Set some dicts for organizing Data
     scan_policy_dict = {}
     scanner_dict = {}
     scan_name_dict = {}
     scanner_list = []
     # Open a CSV for export
-    with open('evaluate.csv', mode='w', encoding='utf-8', newline="") as csv_file:
+    with open('evaluate-{}.csv'.format(table), mode='w', encoding='utf-8', newline="") as csv_file:
         agent_writer = csv.writer(csv_file, delimiter=',', quotechar='"')
 
-        header_list = ["Asset IP Address", "Asset UUID", "Scan Name", "Scan Policy", "Scanner IP", "Scan Time", "Max Checks", "Max Hosts", "Minutes", "RTT", "Hop Count"]
+        header_list = ["Asset IP Address", "Scan Name", "Scan Policy", "Scanner IP", "Scan Time", "Max Checks",
+                       "Max Hosts", "Minutes", "RTT", "Hop Count"]
 
         # Write the header to the csv
         agent_writer.writerow(header_list)
 
         # This function is used to parse the data
         # Getting the length of the Category and using it to get the average
         def average_by_policy(name, scan_info):
@@ -65,16 +81,16 @@
 
             click.echo("-" * 150)
 
         # Loop through each plugin 19506 and Parse data from it
         for vulns in plugin_data:
             plugin_dict = {}
 
-            # Output is the third item in the tuple from the DB
-            plugin_output = vulns[2]
+            # Output is the second item in the tuple from the DB
+            plugin_output = vulns[1]
 
             # split the output by return
             parsed_output = plugin_output.split("\n")
 
             for info_line in parsed_output:
                 try:
                     new_split = info_line.split(" : ")
@@ -83,15 +99,16 @@
                 except:
                     pass
             try:
                 intial_seconds = plugin_dict['Scan duration']
             except KeyError:
                 intial_seconds = 'unknown'
 
-            # For an unknown reason, the scanner will print unknown for some assets leaving no way to calculate the time.
+            # For an unknown reason, the scanner will print unknown
+            # for some assets leaving no way to calculate the time.
             if intial_seconds != 'unknown':
                 try:
                     # Numerical value in seconds parsed from the plugin
                     try:
                         seconds = int(intial_seconds[:-3])
                         minutes = seconds / 60
                     except ValueError:
@@ -131,15 +148,15 @@
                         rtt = plugin_dict['Ping RTT']
                     except KeyError:
                         rtt = "none"
 
                     try:
                         # Grab the last line in the Trace route Plugin output
                         # Split on the space and grab the numerical value.
-                        hopcount = grab_hop_count(vulns[0])[0][-1].split(" ")[-1]
+                        hopcount = grab_hop_count(table, vulns[0])
                     except IndexError:
                         hopcount = "Unknown"
 
                     parsed_data_organized = [vulns[0], scan_name, scan_policy, scanner_ip, start_time, max_checks, max_hosts, minutes, rtt, hopcount]
 
                     agent_writer.writerow(parsed_data_organized)
```

## ivan/plugins/update.py

```diff
@@ -4,9 +4,10 @@
 
 @click.group(help="Update the local Ivan repository - saved in your current dir")
 def update():
     pass
 
 
 @update.command(help="Update the vulns Table")
-def vulns():
-    vuln_export()
+@click.option('--scan_id', default=None, help='Download only a specific scan')
+def vulns(scan_id):
+    vuln_export(scan_id=scan_id)
```

## Comparing `ivan_pro-1.0.4.dist-info/METADATA` & `ivan_pro-1.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivan-pro
-Version: 1.0.4
+Version: 1.1.0
 Summary: A command-line interface to Tenable Security Center
 Home-page: https://github.com/packetchaos/ivan
 Author: Casey Reid
 Author-email: itprofguru@gmail.com
 License: GNUv3
 Keywords: tenable securitycenter ivan tsc,automation
 Platform: UNKNOWN
```

## Comparing `ivan_pro-1.0.4.dist-info/RECORD` & `ivan_pro-1.1.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ivan/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ivan/cli.py,sha256=3goU3FeQcu6Ux2ECWQiYc0LjDRllAtCwYy25mawaXaQ,219
 ivan/plugins/__init__.py,sha256=AVNOkBZT2BXi0sENXslXbZklM3XAZcB31wih8ssR80A,400
-ivan/plugins/database.py,sha256=RSaabhChewmXYJtWf_DYGwpHi0UPCqzut1OoZLx9FqI,2766
-ivan/plugins/dbconfig.py,sha256=COp-FsyiSVyceCirZ46PwrXwLDK2xMEZzcwzUbFCI4U,8153
-ivan/plugins/display.py,sha256=WkkrXMSzmllpehbzJxEDSmQBmqv54rGOE8R1icLKjyM,3664
+ivan/plugins/database.py,sha256=nsjPTLtl9W_0t8dzt9OR9qYVLxm3led242_z10WI85o,4175
+ivan/plugins/dbconfig.py,sha256=T4PhHR2GfF1ki5jjS6TAZpkXnP1pOPyaLK_woyxqDSM,5219
+ivan/plugins/display.py,sha256=gYPokFKOK9VxY2Q-sjFYuOJg8g90MGDpJkwWac68O2E,5203
 ivan/plugins/export.py,sha256=23UUrM4SkR42NYVcIJYYlW6tm_fmIP3xe1hes1AiWcU,1302
 ivan/plugins/find.py,sha256=qnH1RuwsrNVVaQbXRSkbJiwPs2mjgQsg3bPlaqdqitQ,9092
 ivan/plugins/ip.py,sha256=HjOtoUl7kb1oCaGT_Nkua9kulwuQaATqxd-bzLQLS0s,8853
 ivan/plugins/keys.py,sha256=KC4OXT7Rq7DTR_IgvaoP2BtInyvLvsZQbpA-pb8z7iM,1727
 ivan/plugins/query_export.py,sha256=f4qYQjrQe9hrLHF5OFlX3t6DePiKKVV47XUI7L_QQRc,1131
-ivan/plugins/sc_vuln_export.py,sha256=FD1R0bA9A1ENzsELx3hmT_c-Asdx07hHVpn1bdZnpFA,8734
-ivan/plugins/scan.py,sha256=bNW5SEyvYALeQ-dC2Sc0h9tzotRWh82Pz5zXixdy0zM,573
-ivan/plugins/scan_evaluation.py,sha256=jxfck1HHbskHZ_vegi1uHYRMu02Sl6EKfW8HnADqTyk,7016
-ivan/plugins/update.py,sha256=3hb9koJrbfFQxbor2WTwD4OLKLa6YC5G_gAsKSvEcJA,240
-ivan_pro-1.0.4.dist-info/METADATA,sha256=rIhN30owiuwqYCjleSLGN-GUn-y2l7jq-DyvMJGUgNA,2338
-ivan_pro-1.0.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ivan_pro-1.0.4.dist-info/entry_points.txt,sha256=LL3GUB9cAPkceQ1yevSr2Tol0ti7LnyBI0PBqNjJ810,39
-ivan_pro-1.0.4.dist-info/top_level.txt,sha256=woTedJTvuGD9qW1qtH4DAwO60Ztsxx37Fep0ka6mS-M,5
-ivan_pro-1.0.4.dist-info/RECORD,,
+ivan/plugins/sc_vuln_export.py,sha256=nSc0y9TEn8J-aq1Cl_-5o79ddvaZ_rJXVLBwqVGoHH0,9049
+ivan/plugins/scan.py,sha256=ygvTp7_yZCukQZlD5R261jSOAPTHbpOiv8CeH4nuI2A,5960
+ivan/plugins/scan_evaluation.py,sha256=ep9tbL8O6Q9iZjSaNC-FUCCrzui2axtdc9iats5rm1Q,7397
+ivan/plugins/scanidv_vuln_export.py,sha256=4wx4JCYpySPVSeC76KEb2oD2zbhzKeoH2I72qdmg6oc,8878
+ivan/plugins/update.py,sha256=T728CxNz-B6KdSe2BEDWhvtlAlCJ8yR0MfqxwRGx7N4,341
+ivan_pro-1.1.0.dist-info/METADATA,sha256=e5mslgToJ7ImoFfQLtXiSgz4NGGs20LP6SxR81Jhqug,2338
+ivan_pro-1.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+ivan_pro-1.1.0.dist-info/entry_points.txt,sha256=LL3GUB9cAPkceQ1yevSr2Tol0ti7LnyBI0PBqNjJ810,39
+ivan_pro-1.1.0.dist-info/top_level.txt,sha256=woTedJTvuGD9qW1qtH4DAwO60Ztsxx37Fep0ka6mS-M,5
+ivan_pro-1.1.0.dist-info/RECORD,,
```

