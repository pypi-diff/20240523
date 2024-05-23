# Comparing `tmp/smbmap-1.10.3.tar.gz` & `tmp/smbmap-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smbmap-1.10.3.tar", last modified: Thu May 23 12:02:05 2024, max compression
+gzip compressed data, was "smbmap-1.8.2.tar", last modified: Fri Mar 24 12:22:00 2023, max compression
```

## Comparing `smbmap-1.10.3.tar` & `smbmap-1.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 shawnevans  (1000) shawnevans  (1000)        0 2024-05-23 12:02:05.701652 smbmap-1.10.3/
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)    35121 2023-04-04 18:48:37.000000 smbmap-1.10.3/LICENSE
--rw-r--r--   0 shawnevans  (1000) shawnevans  (1000)    26869 2024-05-23 12:02:05.701652 smbmap-1.10.3/PKG-INFO
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)    26158 2024-05-23 02:30:27.000000 smbmap-1.10.3/README.md
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)       38 2024-05-23 12:02:05.701652 smbmap-1.10.3/setup.cfg
--rwxrwxr-x   0 shawnevans  (1000) shawnevans  (1000)     1100 2024-05-23 02:28:28.000000 smbmap-1.10.3/setup.py
-drwxrwxr-x   0 shawnevans  (1000) shawnevans  (1000)        0 2024-05-23 12:02:05.701652 smbmap-1.10.3/smbmap/
--rwxrwxr-x   0 shawnevans  (1000) shawnevans  (1000)        0 2023-04-04 18:48:37.000000 smbmap-1.10.3/smbmap/__init__.py
--rwxrwxr-x   0 shawnevans  (1000) shawnevans  (1000)    74288 2024-05-23 11:54:19.000000 smbmap-1.10.3/smbmap/smbmap.py
-drwxrwxr-x   0 shawnevans  (1000) shawnevans  (1000)        0 2024-05-23 12:02:05.701652 smbmap-1.10.3/smbmap.egg-info/
--rw-r--r--   0 shawnevans  (1000) shawnevans  (1000)    26869 2024-05-23 12:02:05.000000 smbmap-1.10.3/smbmap.egg-info/PKG-INFO
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)      244 2024-05-23 12:02:05.000000 smbmap-1.10.3/smbmap.egg-info/SOURCES.txt
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)        1 2024-05-23 12:02:05.000000 smbmap-1.10.3/smbmap.egg-info/dependency_links.txt
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)       46 2024-05-23 12:02:05.000000 smbmap-1.10.3/smbmap.egg-info/entry_points.txt
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)       52 2024-05-23 12:02:05.000000 smbmap-1.10.3/smbmap.egg-info/requires.txt
--rw-rw-r--   0 shawnevans  (1000) shawnevans  (1000)        7 2024-05-23 12:02:05.000000 smbmap-1.10.3/smbmap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 12:22:00.982889 smbmap-1.8.2/
+-rw-rw-r--   0 root         (0) root         (0)    35121 2023-03-24 11:49:57.000000 smbmap-1.8.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13584 2023-03-24 12:22:00.982889 smbmap-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    12964 2023-03-24 12:17:35.000000 smbmap-1.8.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 12:22:00.982889 smbmap-1.8.2/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1095 2023-03-24 12:21:58.000000 smbmap-1.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 12:22:00.978889 smbmap-1.8.2/smbmap/
+-rwxrwxr-x   0 root         (0) root         (0)        0 2023-03-24 11:56:29.000000 smbmap-1.8.2/smbmap/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    64886 2023-03-24 12:15:15.000000 smbmap-1.8.2/smbmap/smbmap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 12:22:00.978889 smbmap-1.8.2/smbmap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13584 2023-03-24 12:22:00.000000 smbmap-1.8.2/smbmap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      244 2023-03-24 12:22:00.000000 smbmap-1.8.2/smbmap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 12:22:00.000000 smbmap-1.8.2/smbmap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-03-24 12:22:00.000000 smbmap-1.8.2/smbmap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-03-24 12:22:00.000000 smbmap-1.8.2/smbmap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-03-24 12:22:00.000000 smbmap-1.8.2/smbmap.egg-info/top_level.txt
```

### Comparing `smbmap-1.10.3/LICENSE` & `smbmap-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smbmap-1.10.3/setup.py` & `smbmap-1.8.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "smbmap",
-    version = "1.10.3",
+    version = "1.8.2",
     author = "ShawnDEvans",
     author_email = "Shawn.Evans@knowledgeCG.com",
     description = " SMBMap is a handy SMB enumeration tool ",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/ShawnDEvans/smbmap",
     project_urls = {
@@ -22,15 +22,15 @@
         "Operating System :: OS Independent",
     ],
     packages =[ "smbmap" ],
     python_requires = ">=3.6",
     install_requires = [
         'impacket',
         'pyasn1',
-        'pycryptodome',
+        'pycrypto',
         'configparser',
         'termcolor',
     ],
     entry_points={
         'console_scripts': [
             'smbmap=smbmap.smbmap:main'
         ]
```

### Comparing `smbmap-1.10.3/smbmap/smbmap.py` & `smbmap-1.8.2/smbmap/smbmap.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,127 +11,103 @@
 import configparser
 import argparse
 import ipaddress
 import inspect
 import csv
 import getpass
 
-from threading import Thread, Event
-from multiprocessing.pool import Pool
+from threading import Thread
+from multiprocessing import Pool
 from impacket.examples import logger
 from impacket import version, smbserver
 from impacket.smbserver import SRVSServer
 from impacket.smbserver import WKSTServer
 from impacket.smbconnection import *
 from impacket.dcerpc.v5 import transport, scmr
 from impacket.dcerpc.v5.dcomrt import DCOMConnection
 from impacket.dcerpc.v5.dcom import wmi
 from impacket.dcerpc.v5.dtypes import NULL
-from impacket.smb3structs import *
+from impacket.smb3structs import FILE_WRITE_DATA
 
 import ntpath
 import cmd
 import os
 import re
 
 from termcolor import colored as termcolored
 
 # A lot of this code was taken from Impacket's own examples
 # https://github.com/SecureAuthCorp/impacket/
 # Seriously, the most amazing Python library ever!!
 # Many thanks to that dev team
 
-import resource
-rlimit = resource.getrlimit(resource.RLIMIT_NOFILE)
-resource.setrlimit(resource.RLIMIT_NOFILE, (4096, rlimit[1]))
-
 OUTPUT_FILENAME = ''.join(random.sample('ABCDEFGHIGJLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz',10))
 BATCH_FILENAME  = ''.join(random.sample('ABCDEFGHIGJLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz', 10)) + '.bat'
 SMBSERVER_DIR   = ''.join(random.sample('ABCDEFGHIGJLMNOPQRSTUVWXYZ', 10))
 DUMMY_SHARE     = 'TMP'
 PERM_DIR = ''.join(random.sample('ABCDEFGHIGJLMNOPQRSTUVWXYZ', 10))
 PSUTIL_DIR= 'psutils'
 PSUTIL_SHARE = ''.join(random.sample('ABCDEFGHIGJLMNOPQRSTUVWXYZ', 10))
 VERBOSE = False
 USE_TERMCOLOR=True
 SEND_UPDATE_MSG=True
-PORT_SCAN_TIMEOUT = .5
-USE_CCACHE = False
 
 banner = r"""
     ________  ___      ___  _______   ___      ___       __         _______
    /"       )|"  \    /"  ||   _  "\ |"  \    /"  |     /""\       |   __ "\
   (:   \___/  \   \  //   |(. |_)  :) \   \  //   |    /    \      (. |__) :)
    \___  \    /\  \/.    ||:     \/   /\   \/.    |   /' /\  \     |:  ____/
     __/  \   |: \.        |(|  _  \  |: \.        |  //  __'  \    (|  /
    /" \   :) |.  \    /:  ||: |_)  :)|.  \    /:  | /   /  \   \  /|__/ \
   (_______/  |___|\__/|___|(_______/ |___|\__/|___|(___/    \___)(_______)
------------------------------------------------------------------------------
-SMBMap - Samba Share Enumerator v1.10.3 | Shawn Evans - ShawnDEvans@gmail.com<mailto:ShawnDEvans@gmail.com>
+ -----------------------------------------------------------------------------
+     SMBMap - Samba Share Enumerator | Shawn Evans - ShawnDEvans@gmail.com
                      https://github.com/ShawnDEvans/smbmap
 """
 
 
 def colored(msg, *args, **kwargs):
     global USE_TERMCOLOR
     if USE_TERMCOLOR:
         return termcolored(msg, *args, **kwargs)
     return msg
 
 
 class Loader(Thread):
-    def __init__(self, msg='Working on it'):
+    def __init__(self):
         Thread.__init__(self)
-        self.__running = Event()
-        self.__running.set()
-        self.__flag = Event()
-        self.__flag.set()
+        self._running = True
         self._progress = '\\|/-\\|/-'
-        self._msg = '{}{}'.format(msg, ' '*100)
-
-    def update(self, msg):
-        self._msg = '{}{}'.format(msg, ' '*100)
 
     def terminate(self):
-        self.__flag.set()
-        self.__running.clear()
-
-    def pause(self):
-        self.__flag.clear()
-
-    def resume(self):
-        self.__flag.set()
+        self._running = False
 
     def cleanup(self):
-        print(' '*100, end='\r')
-        print('\r', end='\r')
+        print(' '*32, end='')
+        print('\r', end='')
 
     def run(self):
         global SEND_UPDATE_MSG
-        while self.__running.is_set():
+        while self._running:
             for char in self._progress:
                 if SEND_UPDATE_MSG:
-                    self.__flag.wait()
-                    print('[{}] {}'.format(char, self._msg), end='\r')
-                    print('\r', end='\r')
+                    print('[{}] Working on it...'.format(char), end='')
+                    print('\r', end='')
                     time.sleep(0.05)
 
 class SimpleSMBServer(Thread):
     def __init__(self, interface_address, port):
         Thread.__init__(self)
         self.smbserver = smbserver.SimpleSMBServer(listenAddress = interface_address, listenPort = int(port))
         self.smbserver.addShare(PSUTIL_SHARE, PSUTIL_DIR, shareComment='P0w3r$he11')
         self.smbserver.setSMB2Support(True)
 
     def run(self):
         self.smbserver.start()
 
-    def stop(self):
-        self.smbserver.stop()
-
 class SMBServer(Thread):
     def __init__(self):
         Thread.__init__(self)
         self.smb = None
         print('[+] Initializing SMB server..')
 
     def cleanup_server(self):
@@ -189,15 +165,15 @@
             print('[!] Error starting SMB server: ', e)
             pass
 
     def stop(self):
         self.cleanup_server()
         self.smb.socket.close()
         self.smb.server_close()
-        self._Thread__stop()
+        #self._Thread__stop()
 
 class WMIEXEC:
     def __init__(self, command='', username='', password='', domain='', hashes=None, aesKey=None, share=None,
                  noOutput=False, doKerberos=False, kdcHost=None, scr_output=True):
         self.__command = command
         self.__username = username
         self.__password = password
@@ -218,14 +194,15 @@
         if self.__noOutput is False:
             smbConnection = SMBConnection(addr, addr)
             if self.__doKerberos is False:
                 smbConnection.login(self.__username, self.__password, self.__domain, self.__lmhash, self.__nthash)
             else:
                 smbConnection.kerberosLogin(self.__username, self.__password, self.__domain, self.__lmhash,
                                             self.__nthash, self.__aesKey, kdcHost=self.__kdcHost)
+
             dialect = smbConnection.getDialect()
             if dialect == SMB_DIALECT:
                 logging.info("SMBv1 dialect used")
             elif dialect == SMB2_DIALECT_002:
                 logging.info("SMBv2.0 dialect used")
             elif dialect == SMB2_DIALECT_21:
                 logging.info("SMBv2.1 dialect used")
@@ -284,20 +261,20 @@
             self.__noOutput = True
 
     def do_shell(self, s):
         os.system(s)
 
     def do_help(self, line):
         print("""
-         lcd {path}                 - changes the current local directory to {path}
-         exit                       - terminates the server process (and this session)
-         put {src_file, dst_path}   - uploads a local file to the dst_path (dst_path = default current directory)
-         get {file}                 - downloads pathname to the current local dir
-         ! {cmd}                    - executes a local shell cmd
-        """)
+ lcd {path}                 - changes the current local directory to {path}
+ exit                       - terminates the server process (and this session)
+ put {src_file, dst_path}   - uploads a local file to the dst_path (dst_path = default current directory)
+ get {file}                 - downloads pathname to the current local dir
+ ! {cmd}                    - executes a local shell cmd
+""")
 
     def do_lcd(self, s):
         if s == '':
             print(os.getcwd())
         else:
             try:
                 os.chdir(s)
@@ -479,25 +456,25 @@
         self.__serviceName = serviceName
         self.__rpc = rpc
 
         self.__scmr = rpc.get_dce_rpc()
         try:
             self.__scmr.connect()
         except Exception as e:
-            logging.critical(str(e))
-            #print(e)
+            #logging.critical(str(e))
+            print(e)
             #sys.exit(1)
 
         s = rpc.get_smb_connection()
 
         # We don't wanna deal with timeouts from now on.
         s.setTimeout(100000)
         if mode == 'SERVER':
             myIPaddr = s.getSMBServer().get_socket().getsockname()[0]
-            self.__copyBack = 'copy %s \\\\%s\\%s<file://%25s/%25s>' % (self.__output, myIPaddr, DUMMY_SHARE)
+            self.__copyBack = 'copy %s \\\\%s\\%s' % (self.__output, myIPaddr, DUMMY_SHARE)
 
         self.__scmr.bind(scmr.MSRPC_UUID_SCMR)
         resp = scmr.hROpenSCManagerW(self.__scmr)
         self.__scHandle = resp['lpScHandle']
         self.transferClient = rpc.get_smb_connection()
         self.do_cd('')
 
@@ -588,65 +565,113 @@
         '445/SMB': (r'ncacn_np:%s[\pipe\svcctl]', 445),
         }
 
     def __init__(self):
         self.recursive = False
         self.dir_only = False
         self.list_files = False
-        self.admin_only = False
         self.loading = False
         self.verbose = True
-        self.shares = {}
+        self.smbconn = {}
         self.isLoggedIn = False
         self.pattern = None
         self.grepable = False
         self.outfile = None
         self.csv = False
         self.csv_writer = None
         self.hosts = {}
         self.jobs = {}
         self.search_output_buffer = ''
         self.loader = None
         self.exclude = []
 
-    def logout(self, host):
+    def login(self, host, username, password, domain, lmhash, nthash, port):
         try:
-            for session in self.hosts[host]['smbconn']:
-                session.logoff()
+            if port == 445:
+                smbconn = SMBConnection(host, host, sess_port=445, timeout=4)
+                smbconn.login(username, password, domain, lmhash, nthash)
+            else:
+                smbconn = SMBConnection('*SMBSERVER', host, sess_port=139, timeout=4)
+                smbconn.login(username, password, domain, lmhash, nthash)
+            '''
+            if self.smbconn[host].isGuestSession() > 0:
+                if verbose and not self.grepable:
+                    print('[+] Guest SMB session established on %s...' % (host))
+            else:
+                if verbose and not self.grepable:
+                    print('[+] User SMB session established on %s...' % (host))
+            '''
+            return smbconn
+
+        except Exception as e:
+            if self.verbose:
+                print('[!] Authentication error on %s' % (host))
+            return False
+
+    def logout(self, host):
+        self.smbconn[host].logoff()
+
+    def smart_login(self):
+        for host in list(self.hosts.keys()):
+            success = False
+
+            if self.hosts[host]['port'] == 445:
+                success = self.login(host, self.hosts[host]['user'], self.hosts[host]['passwd'], self.hosts[host]['domain'], self.hosts[host]['lmhash'], self.hosts[host]['nthash'], self.host[host]['port'])
+            else:
+                success = self.login_rpc(host, self.hosts[host]['user'], self.hosts[host]['passwd'], self.hosts[host]['domain'], self.hosts[host]['lmhash'], self.hosts[host]['nthash'])
+
+            if not success:
+                if self.verbose:
+                    print('[!] Authentication error on %s' % (host))
+                self.smbconn.pop(host,None)
+                self.hosts.pop(host, None)
+                continue
+
+    def login_rpc(self, host, username, password, domain):
+        try:
+            self.smbconn[host] = SMBConnection('*SMBSERVER', host, sess_port=139, timeout=4)
+            self.smbconn[host].login(username, password, domain)
+
+            '''
+            if self.smbconn[host].isGuestSession() > 0:
+                if verbose and not self.grepable:
+                    print('[+] Guest RPC session established on %s...' % (host))
+            else:
+                if verbose and not self.grepable:
+                    print('[+] User RPC session established on %s...' % (host))
+            '''
             return True
-        except:
+
+        except Exception as e:
+            print('[!] RPC Authentication error occurred')
             return False
 
     def start_smb_server(self):
         try:
-            smb_server = SimpleSMBServer('0.0.0.0', 445)
-            smb_server.daemon = True
-            smb_server.start()
-            return smb_server
-        except Exception as e:
+            serverThread = SimpleSMBServer('0.0.0.0', 445)
+            serverThread.daemon = True
+            serverThread.start()
+        except:
             print('[!] Run as r00t, or maybe something is using port 445...')
-            self.kill_loader()
-            return False
-            sys.exit(1)
-
+            sys.exit()
 
     def start_file_search(self, host, pattern, share, search_path):
         try:
             myIPaddr = self.get_ip_address()
             job_name = uuid.uuid4().hex
             tmp_dir = self.exec_command(host, share, 'echo %TEMP%', disp_output=False).strip()
             if len(tmp_dir) == 0:
                 tmp_dir = 'C:\\Windows\\Temp'
 
             tmp_bat_cmd = 'powershell -NoLogo -ExecutionPolicy bypass -Command " & {}Get-ChildItem {}\*.* -Recurse -Exclude *.dll,*.exe,*.msi,*.jpg,*.gif,*.bmp,*.png,*.mp3,*.wav | Select-String -Pattern \'{}\' | Select-Object -Unique Path | out-string -width 220{}" 2>nul > {}\{}.txt'.format('{', search_path, pattern, '}', tmp_dir, job_name)
             tmp_bat = open('./{}/{}.bat'.format(PSUTIL_DIR, job_name), 'w')
             tmp_bat.write(tmp_bat_cmd)
             tmp_bat.close()
 
-            ps_command = 'powershell -ExecutionPolicy bypass -NoLogo -command "Start-Process """cmd.exe""" """/c \\\\{}\\{}\\{}.bat<file://%7b%7d/%7b%7d/%7b%7d.bat>""" "'.format(myIPaddr, PSUTIL_SHARE, job_name)
+            ps_command = 'powershell -ExecutionPolicy bypass -NoLogo -command "Start-Process """cmd.exe""" """/c \\\\{}\\{}\\{}.bat""" "'.format(myIPaddr, PSUTIL_SHARE, job_name)
             success = self.exec_command(host, share, ps_command, disp_output=False)
             print('[+] Job {} started on {}, result will be stored at {}\{}.txt'.format(job_name, host, tmp_dir, job_name))
             proc_id = self.get_job_procid(host, share, tmp_dir, job_name)
             if len(proc_id) > 0:
                 proc_id = [j.strip() for j in proc_id.split('\n') if len(j) > 0]
             self.jobs[job_name] = { 'host' : host, 'share' : share, 'tmp' : tmp_dir , 'pattern' : pattern, 'start_time': time.perf_counter() , 'proc_id' : proc_id }
         except Exception as e:
@@ -656,15 +681,15 @@
             sys.stdout.flush()
             print('[!] Job creation failed on host: %s. Did you run as r00t?' % (host))
 
     def get_job_procid(self, host, share, path, job):
         try:
             myIPaddr = self.get_ip_address()
             file_path = '{}\{}.txt'.format(path, job)
-            command = 'powershell -NoLogo -ExecutionPolicy bypass -File \\\\{}\\{}\\Get-FileLockProcess.ps1<file://%7b%7d/%7b%7d/Get-FileLockProcess.ps1> "{}"'.format(myIPaddr, PSUTIL_SHARE, file_path)
+            command = 'powershell -NoLogo -ExecutionPolicy bypass -File "\\\\{}\\{}\\Get-FileLockProcess.ps1" "{}"'.format(myIPaddr, PSUTIL_SHARE, file_path)
             result = self.exec_command(host, share, command, disp_output=False)
             return result
         except Exception as e:
             exc_type, exc_obj, exc_tb = sys.exc_info()
             fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
             print('[!] WTF: {} on line {}'.format(e, exc_tb.tb_lineno))
             sys.stdout.flush()
@@ -677,15 +702,15 @@
         while len(list(self.jobs.keys())) > 0:
             try:
                 for job in list(self.jobs.keys()):
                     isItThere = self.exec_command(self.jobs[job]['host'], self.jobs[job]['share'], 'cmd /c "if exist {}\{}.txt echo ImHere"'.format(self.jobs[job]['tmp'], job), disp_output=False)
                     result = self.exec_command(self.jobs[job]['host'], self.jobs[job]['share'], 'cmd /c "2>nul (>>{}\{}.txt (call )) && (echo not locked) || (echo locked)"'.format(self.jobs[job]['tmp'], job), disp_output=False)
                     if 'not locked' ==  result.strip() and isItThere.strip() == 'ImHere':
                         dl_target = '%s%s\%s.txt' % (self.jobs[job]['share'], self.jobs[job]['tmp'][2:], job)
-                        host_dest = download_file(self.hosts[self.jobs[job]['host']]['smbconn'][0], dl_target)
+                        host_dest = self.download_file(self.jobs[job]['host'], dl_target)
                         counter += 1
                         self.search_output_buffer += 'Host: %s \t\tPattern: %s\n' % (self.jobs[job]['host'], self.jobs[job]['pattern'])
                         if os.stat(host_dest).st_size > 0:
                             results_file = open(host_dest)
                             self.search_output_buffer += results_file.read()
                             self.search_output_buffer += '\n'
                         else:
@@ -701,15 +726,15 @@
                             print('[!] Job {} is taking a long time....it\'s getting punted'.format(job))
                             for pid in self.jobs[job]['proc_id']:
                                 kill_job = 'taskkill /PID {} /F'.format(pid)
                                 success = self.exec_command(self.jobs[job]['host'], self.jobs[job]['share'], kill_job, disp_output=False)
                                 os.remove('./{}/{}.bat'.format(PSUTIL_DIR, job))
                         time.sleep(10)
             except Exception as e:
-                print('[!]', e)
+                print(e)
         print('[+] All jobs complete')
         print(self.search_output_buffer)
 
     def get_ip_address(self):
         myIPaddr = ''
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         try:
@@ -742,70 +767,330 @@
                     net_disks = ''
             print('[+] Host %s Local %s' % (host, local_disks.strip()))
             print('[+] Host %s Net Drive(s):' % (host))
             if len(disks) > 0:
                 for disk in disks:
                      print('\t%s' % (disk))
             else:
-                print('[*] No mapped network drives')
+                print('\tNo mapped network drives')
             pass
         except Exception as e:
             print('[!] Error on {}: {}'.format(host, e))
 
+    def output_shares(self, host, lsshare, lspath, write_check=True, depth=5):
+        shareList = [(lsshare,'')] if lsshare else self.get_shares(host)
+        share_privs = ''
+        share_tree = {}
+        for share in shareList:
+            if share[0].lower() not in self.exclude:
+                share_name = share[0]
+                share_comment = share[1]
+                share_tree[share_name] = {}
+                canWrite = False
+                readonly = False
+                noaccess = False
+                if write_check:
+                    try:
+                        root = PERM_DIR.replace('/','\\')
+                        root = ntpath.normpath(root)
+                        self.create_dir(host, share_name, root)
+                        share_tree[share_name]['privs'] = 'READ, WRITE'
+                        canWrite = True
+                        try:
+                            self.remove_dir(host, share_name, root)
+                        except Exception as e:
+                            print('\t[!] Unable to remove test directory at \\\\%s\\%s\\%s, please remove manually' % (host, share_name, root))
+                    except Exception as e:
+                        exc_type, exc_obj, exc_tb = sys.exc_info()
+                        fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                        #print(exc_type, fname, exc_tb.tb_lineno)
+                        sys.stdout.flush()
+                    if not canWrite:
+                        try:
+                            root = PERM_DIR.replace('/','\\')
+                            root = ntpath.normpath(root)
+                            self.create_file(host, share_name, root)
+                            share_tree[share_name]['privs'] = colored('READ, WRITE', 'green')
+                            canWrite = True
+                            try:
+                                self.remove_file(host, share_name, root)
+                            except Exception as e:
+                                print('\t[!] Unable to remove test file at \\\\%s\\%s\\%s, please remove manually' % (host, share_name, root))
+                        except Exception as e:
+                            exc_type, exc_obj, exc_tb = sys.exc_info()
+                            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                            #print(exc_type, fname, exc_tb.tb_lineno)
+                            sys.stdout.flush()
+
+                try:
+                    if self.smbconn[host].listPath(share_name, self.pathify('/')) and canWrite == False:
+                        readonly = True
+                        share_tree[share_name]['privs'] = 'READ ONLY'
+                except Exception as e:
+                    noaccess = True
+                    share_tree[share_name]['privs'] = 'NO ACCESS'
+
+                share_tree[share_name]['comment'] = share_comment
+                contents = {}
+
+                try:
+                    if noaccess == False:
+                        dirList = ''
+                        if lspath:
+                            path = lspath
+                        else:
+                            path = '/'
+                        if self.list_files:
+                            if self.pattern:
+                                print('[+] Starting search for files matching \'%s\' on share %s.' % (self.pattern, share[0]))
+                            contents = self.list_path(host, share_name, path, depth)
+                except Exception as e:
+                    exc_type, exc_obj, exc_tb = sys.exc_info()
+                    fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                    print('[!] Something weird happened: {} on line {}'.format(e, exc_tb.tb_lineno))
+                    sys.stdout.flush()
+                    sys.exit()
+                share_tree[share_name]['contents'] = contents
+
+        self.to_string(share_tree, host)
+
     def kill_loader(self):
         self.loading = False
-        if self.loader:
-            self.loader.terminate()
-            self.loader.join()
-            self.loader.cleanup()
-            self.loader = None
+        self.loader.terminate()
+        self.loader.join()
+        self.loader.cleanup()
+
+    def list_path(self, host, share, path, depth=5, path_list=None):
+        if path_list is None:
+            path_list = {}
+        pwd = self.pathify(path)
+        width = 16
+        try:
+            pathList = self.smbconn[host].listPath(share, pwd)
+            path_list[path] = []
+            for item in pathList:
+                filesize = item.get_filesize()
+                readonly = 'w' if item.is_readonly() > 0 else 'r'
+                date = time.ctime(float(item.get_mtime_epoch()))
+                isDir = 'd' if item.is_directory() > 0 else 'f'
+                filename = item.get_longname()
+                if isDir == 'f':
+                    if self.pattern:
+                        fileMatch = re.search(self.pattern.lower(), filename.lower())
+                        if fileMatch:
+                            dlThis = '%s\%s%s' % (share, pwd.strip('*'), filename)
+                            dlThis = dlThis.replace('/','\\')
+                            print('[+] Match found! Downloading: %s' % (dlThis))
+                            self.download_file(host, dlThis)
+                if (self.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and self.dir_only == False):
+                    path_list[path].append({'isDir': isDir, 'readonly': readonly, 'filesize': filesize, 'date': date, 'filename': filename})
+            if self.recursive:
+                for smbItem in path_list[path]:
+                    try:
+                        if smbItem['isDir'] == 'd' and smbItem['filename'] not in [ '.', '..']:
+                            subPath = '%s/%s' % (path, smbItem['filename'])
+                            subPath = self.pathify(subPath)
+                            pathList  = self.smbconn[host].listPath(share, subPath)
+                            if len(pathList) > 2 and '{}/{}'.format(path, smbItem['filename']) not in path_list.keys() and subPath.count('\\')-1 <= int(depth):
+                                self.list_path(host, share, '%s/%s' % (path, smbItem['filename']), depth, path_list)
+                    except SessionError as e:
+                        continue
+            return path_list
+        except Exception as e:
+            exc_type, exc_obj, exc_tb = sys.exc_info()
+            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+            print('[!] Something weird happened: {} on line {}'.format(e, exc_tb.tb_lineno))
+            sys.stdout.flush()
+            return {}
+
+    def to_string(self, share_tree, host):
+        self.kill_loader()
+        header = '\tDisk{}\tPermissions\tComment\n'.format(' '.ljust(50))
+        header += '\t----{}\t-----------\t-------'.format(' '.ljust(50))
+        heads_up = False
+        try:
+            for item in share_tree.keys():
+                if share_tree[item]['privs'] == 'READ, WRITE':
+                    share_name_privs = colored('READ, WRITE', 'green')
+                if share_tree[item]['privs'] == 'READ ONLY':
+                    share_name_privs = colored('READ ONLY', 'yellow')
+                if share_tree[item]['privs'] == 'NO ACCESS':
+                    share_name_privs = colored('NO ACCESS', 'red')
+                if self.csv and not self.list_files:
+                    row = {}
+                    row['Host'] = host
+                    row['Share'] = item
+                    row['Privs'] = share_tree[item]['privs'].replace(',','').replace(' ', '_')
+                    row['Comment'] = share_tree[item]['comment'].replace('\r','').replace('\n', '')
+                    self.writer.writerow(row)
+                if self.verbose == False and 'NO ACCESS' not in share_tree[item]['privs'] and self.grepable == False and not self.pattern and self.csv == False:
+                    if heads_up == False:
+                        print(header)
+                        heads_up = True
+                    print('\t{}\t{}\t{}'.format(item.ljust(50), share_name_privs, share_tree[item]['comment'] ) )
+                elif self.verbose and self.grepable == False and self.csv == False and  not self.pattern:
+                    if heads_up == False:
+                        print(header)
+                        heads_up = True
+                    print('\t{}\t{}\t{}'.format(item.ljust(50), share_name_privs, share_tree[item]['comment'] ) )
+                for path in share_tree[item]['contents'].keys():
+                    if self.grepable == False and self.csv == False and self.verbose:
+                        print('\t.\{}\{}'.format(item, self.pathify(path)))
+                    for file_info in share_tree[item]['contents'][path]:
+                        isDir = file_info['isDir']
+                        readonly = file_info['readonly']
+                        filesize = file_info['filesize']
+                        date = file_info['date']
+                        filename = file_info['filename']
+                        if (self.verbose and self.grepable == False and self.csv == False) and ((self.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and self.dir_only == False)):
+                            print('\t%s%s--%s--%s-- %s %s\t%s' % (isDir, readonly, readonly, readonly, str(filesize).rjust(16), date, filename))
+                        elif self.grepable:
+                            if filename != '.' and filename != '..':
+                                if (self.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and self.dir_only == False):
+                                    self.outfile.write('host:{}, share:{}, privs:{}, isDir:{}, path:{}{}\{}, fileSize:{}, date:{}\n'.format(host, item, share_tree[item]['privs'].replace(',','').replace(' ', '_'), isDir, item, self.pathify(path).replace('\*',''), filename, str(filesize), date))
+                        elif self.csv:
+                            if filename != '.' and filename != '..':
+                                if (self.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and self.dir_only == False):
+                                    row = {}
+                                    row['Host'] = host
+                                    row['Share'] = item
+                                    row['Privs'] = share_tree[item]['privs'].replace(',','').replace(' ', '_')
+                                    row['isDir'] = isDir
+                                    row['Path'] = '{}{}\{}'.format(item, self.pathify(path).replace('\*',''), filename)
+                                    row['fileSize'] = str(filesize)
+                                    row['Date'] = date
+                                    self.writer.writerow(row)
+        except Exception as e:
+            print('[!] Bummer: ', e)
+
+    def get_shares(self, host):
+        try:
+            shareList = self.smbconn[host].listShares()
+            shares = []
+            for item in range(len(shareList)):
+                shares.append( (shareList[item]['shi1_netname'][:-1], shareList[item]['shi1_remark'][:-1]) )
+            return shares
+        except Exception as e:
+            exc_type, exc_obj, exc_tb = sys.exc_info()
+            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+            print('[!] Something weird happened: {} on line {}'.format(e, exc_tb.tb_lineno))
+            sys.stdout.flush()
+            self.kill_loader()
+            #sys.exit()
+
+    def pathify(self, path):
+        root = ''
+        root = ntpath.join(path,'*')
+        root = root.replace('/','\\')
+        root = root.replace('\\\\','\\')
+        root = ntpath.normpath(root)
+        return root
+
+    def create_dir(self, host, share, path):
+        #path = self.pathify(path)
+        self.smbconn[host].createDirectory(share, path)
+
+    def remove_dir(self, host, share, path):
+        #path = self.pathify(path)
+        self.smbconn[host].deleteDirectory(share, path)
+
+    def create_file(self, host, share, path):
+        tid = self.smbconn[host].connectTree(share)
+        self.smbconn[host].createFile(tid, path, desiredAccess=FILE_WRITE_DATA)
+
+    def remove_file(self, host, share, path):
+        #path = self.pathify(path)
+        self.smbconn[host].deleteFile(share, path)
+
+    def valid_ip(self, address):
+        try:
+            socket.inet_aton(address)
+            return True
+        except:
+            return False
 
     def filter_results(self, pattern):
         pass
 
+    def download_file(self, host, path):
+        path = path.replace('/','\\')
+        path = ntpath.normpath(path)
+        filename = path.split('\\')[-1]
+        share = path.split('\\')[0]
+        path = path.replace(share, '')
+        try:
+            out = open(ntpath.basename('%s/%s' % (os.getcwd(), '%s-%s%s' % (host, share.replace('$',''), path.replace('\\','_')))),'wb')
+            dlFile = self.smbconn[host].listPath(share, path)
+            if self.verbose:
+                msg = '[+] Starting download: %s (%s bytes)' % ('%s%s' % (share, path), dlFile[0].get_filesize())
+                if self.pattern:
+                    msg = '\t' + msg
+                print(msg)
+            self.smbconn[host].getFile(share, path, out.write)
+            if self.verbose:
+                msg = '[+] File output to: %s/%s' % (os.getcwd(), ntpath.basename('%s/%s' % (os.getcwd(), '%s-%s%s' % (host, share.replace('$',''), path.replace('\\','_')))))
+                if self.pattern:
+                    msg = '\t'+msg
+                print(msg)
+        except SessionError as e:
+            if 'STATUS_ACCESS_DENIED' in str(e):
+                print('[!] Error retrieving file, access denied')
+            elif 'STATUS_INVALID_PARAMETER' in str(e):
+                print('[!] Error retrieving file, invalid path')
+            elif 'STATUS_SHARING_VIOLATION' in str(e):
+                print('[!] Error retrieving file %s, sharing violation' % (filename))
+                out.close()
+                os.remove(ntpath.basename('%s/%s' % (os.getcwd(), '%s-%s%s' % (host, share.replace('$',''), path.replace('\\','_')))))
+        except Exception as e:
+            print('[!] Error retrieving file, unknown error')
+            os.remove(filename)
+        out.close()
+        return '%s/%s' % (os.getcwd(), ntpath.basename('%s/%s' % (os.getcwd(), '%s-%s%s' % (host, share.replace('$',''), path.replace('\\','_')))))
+
     def exec_command(self, host, share, command, disp_output=True, host_name=None, mode='wmi'):
         try:
             if self.is_ntlm(self.hosts[host]['passwd']):
                 hashes = self.hosts[host]['passwd']
             else:
                 hashes = None
-
+            if self.loading:
+                self.kill_loader()
             if mode == 'wmi':
                 executer = WMIEXEC(username=self.hosts[host]['user'], password=self.hosts[host]['passwd'],  hashes=hashes, share=share, command=command, scr_output=disp_output)
                 result = executer.run(host)
             else:
                 executer = CMDEXEC(username=self.hosts[host]['user'], password=self.hosts[host]['passwd'],  hashes=hashes, share=share, command=command)
                 result = executer.run(host_name, host)
             return result
         except:
             exc_type, exc_obj, exc_tb = sys.exc_info()
-            print('[!] Something weird happened on ({}) {} on line {}'.format(host, e, exc_tb.tb_lineno))
+            print('[!] Something weird happened: {} on line {}'.format(e, exc_tb.tb_lineno))
             sys.stdout.flush()
             return none
 
     def delete_file(self, host, path):
         path = path.replace('/','\\')
         path = ntpath.normpath(path)
         filename = path.split('\\')[-1]
         share = path.split('\\')[0]
-        path = path.replace(share, '', 1)
+        path = path.replace(share, '')
         path = path.replace(filename, '')
         try:
-            self.hosts[host]['smbconn'][0].deleteFile(share, path + filename)
+            self.smbconn[host].deleteFile(share, path + filename)
             if self.verbose:
                 print('[+] File successfully deleted: %s%s%s' % (share, path, filename))
         except SessionError as e:
             if 'STATUS_ACCESS_DENIED' in str(e):
                 print('[!] Error deleting file, access denied')
             elif 'STATUS_INVALID_PARAMETER' in str(e):
                 print('[!] Error deleting file, invalid path')
             elif 'STATUS_SHARING_VIOLATION' in str(e):
-                print('[!] Error deleting file, sharing violation')
+                print('[!] Error retrieving file, sharing violation')
             elif 'STATUS_FILE_IS_A_DIRECTORY' in str(e):
-                self.hosts[host]['smbconn'][0].deleteDirectory(share, path)
+                self.smbconn[host].deleteDirectory(share, path)
                 #self.remove_dir(host, share, path)
             else:
                 print('[!] Error deleting file %s%s%s, unknown error' % (share, path, filename))
                 print('[!]', e)
         except Exception as e:
             print('[!] Error deleting file %s%s%s, unknown error' % (share, path, filename))
             print('[!]', e)
@@ -816,15 +1101,15 @@
         dst = dst.split('\\')
         share = dst[0]
         dst = '\\'.join(dst[1:])
         if os.path.exists(src):
             print('[+] Starting upload: %s (%s bytes)' % (src, os.path.getsize(src)))
             upFile = open(src, 'rb')
             try:
-                self.hosts[host]['smbconn'][0].putFile(share, dst, upFile.read)
+                self.smbconn[host].putFile(share, dst, upFile.read)
                 print('[+] Upload complete')
             except Exception as e:
                 print('[!]', e)
                 print('[!] Error uploading file, you need to include destination file name in the path')
             upFile.close()
         else:
             print('[!] Invalid source. File does not exist')
@@ -837,818 +1122,334 @@
                 if len(lm) == 32 and len(ntlm) == 32:
                     return True
                 else:
                     return False
         except Exception as e:
             return False
 
-def init_host( host_args ):
-    ip = host_args['ip']
-    port = host_args['port']
-    user = host_args['user']
-    passwd = host_args['passwd']
-    domain = host_args['domain']
-    lmhash = host_args['lmhash']
-    nthash = host_args['nthash']
-    kdc_host = host_args['kdc_host']
-    try:
-        return { 'ip' : socket.gethostbyname(ip), 'name' : socket.getnameinfo((ip, port),0)[0] , 'port' : port, 'user' : user, 'passwd' : passwd, 'domain' : domain, 'lmhash' : lmhash, 'nthash' : nthash, 'smbconn' : [] ,'kdc' : kdc_host }
-    except Exception as e:
-        return { 'ip' : socket.gethostbyname(ip), 'name' : ip, 'port' : 445, 'user' : user, 'passwd' : passwd, 'domain' : domain, 'lmhash' : lmhash, 'nthash' : nthash , 'smbconn' : [] , 'kdc' : kdc_host }
-
-
-def close_smb_connection( logoff_args ):
-    try:
-        smbconn = logoff_args['smbconn']
-        return smbconn.logoff()
-    except:
-        return False
-
-def get_version( version_args ):
-    smbconn = version_args['smbconn']
-    host = version_args['host']
-
-    domain = smbconn.getServerDomain()
-    if not domain:
-        domain = smbconn.getServerName()
-    version = smbconn.getServerOS()
-    name = smbconn.getServerName()
-
-    return { 'Host' : '{:<16}'.format(host), 'Version' : version, 'Name' : name, 'Domain' : domain }
+    def get_version(self, host):
+        domain = self.smbconn[host].getServerDomain()
+        if not domain:
+            domain = self.smbconn[host].getServerName()
+        print("[+] {}:{} is running {} (name:{}) (domain:{})".format(host, 445, self.smbconn[host].getServerOS(), self.smbconn[host].getServerName(), domain))
 
 def signal_handler(signal, frame):
-    print('[*] You pressed Ctrl+C!')
+    print('You pressed Ctrl+C!')
     os._exit(0)
 
 def find_open_ports(address):
     result = 1
     address = address.strip()
     try:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.settimeout(PORT_SCAN_TIMEOUT)
+        sock.settimeout(3)
         result = sock.connect_ex((address, 445))
         if result == 0:
             sock.close()
             return address
         else:
             return False
     except Exception as e:
         return False
 
-def to_string(smb_tree, mysmb):
-    header = '\tDisk{}\tPermissions\tComment\n'.format(' '.ljust(50))
-    header += '\t----{}\t-----------\t-------'.format(' '.ljust(50))
-    heads_up = False
-    priv_status = ''
-    try:
-        for host in smb_tree.keys():
-            if mysmb.hosts[host]['smbconn'][0].isGuestSession() > 0:
-                priv_status = 'Status: ' + colored('Guest session   \t', 'yellow')
-            try:
-                if smb_tree[host]['ADMIN$']['privs'] == 'READ, WRITE':
-                    priv_status = 'Status: ' + colored('ADMIN!!!', 'green', attrs=['bold','underline']) + '   \t'
-                    if mysmb.admin_only:
-                        print(' '*100)
-                        print('[+] IP: {}:{}\tName: {}\t{}'.format(host, mysmb.hosts[host]['port'], mysmb.hosts[host]['name'].ljust(20), priv_status ))
-                else:
-                    priv_status = 'Status: ' + colored ('Authenticated', 'green')
-            except:
-                priv_status = 'Status: ' + colored ('Authenticated', 'green')
-
-            for share in smb_tree[host].keys():
-                if smb_tree[host][share]['privs'] == 'READ, WRITE':
-                    share_name_privs = colored('READ, WRITE', 'green')
-                if smb_tree[host][share]['privs'] == 'READ ONLY':
-                    share_name_privs = colored('READ ONLY', 'yellow')
-                if smb_tree[host][share]['privs'] == 'NO ACCESS':
-                    share_name_privs = colored('NO ACCESS', 'red')
-
-                if mysmb.admin_only == False:
-                    if heads_up == False:
-                        print(' '*100)
-                        print('[+] IP: {}:{}\tName: {}\t{}'.format(host, mysmb.hosts[host]['port'], mysmb.hosts[host]['name'].ljust(20), priv_status ))
-                        print(header)
-                        heads_up = True
-
-                    if mysmb.verbose == True:
-                        print('\t{}\t{}\t{}'.format(share.ljust(50), share_name_privs, smb_tree[host][share]['comment'] ) )
-                    elif mysmb.verbose == False and smb_tree[host][share]['privs'] != 'NO ACCESS':
-                        print('\t{}\t{}\t{}'.format(share.ljust(50), share_name_privs, smb_tree[host][share]['comment'] ) )
-
-                    if mysmb.csv and mysmb.recursive == False:
-                        if ( mysmb.verbose == False and smb_tree[host][share]['privs'] != 'NO ACCESS') or mysmb.verbose == True:
-                            row = {}
-                            row['Host'] = host
-                            row['Share'] = share
-                            row['Privs'] = smb_tree[host][share]['privs'].replace(',','').replace(' ', '_')
-                            row['Comment'] = smb_tree[host][share]['comment']
-                            mysmb.writer.writerow(row)
-
-                    if mysmb.grepable and len(smb_tree[host][share]['contents'].keys()) == 0:
-                        mysmb.outfile.write('host:{}, share:{}, privs:{}\n'.format(host, share, smb_tree[host][share]['privs'].replace(',','').replace(' ', '_')))
-
-                    if mysmb.recursive:
-                        for path in smb_tree[host][share]['contents'].keys():
-                            if mysmb.grepable == False and mysmb.csv == False:
-                                if len(path) > 0 and path[0] == '/':
-                                    print('\t./{}/{}'.format(share, path))
-                                else:
-                                    print('\t./{}{}'.format(share, path))
-                            for file_info in smb_tree[host][share]['contents'][path]:
-                                isDir = file_info['isDir']
-                                readonly = file_info['readonly']
-                                filesize = file_info['filesize']
-                                date = file_info['date']
-                                filename = file_info['filename']
-                                if mysmb.grepable == False and mysmb.csv == False and ((mysmb.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and mysmb.dir_only == False)):
-                                    print('\t%s%s--%s--%s-- %s %s\t%s' % (isDir, readonly, readonly, readonly, str(filesize).rjust(16), date, filename))
-                                if mysmb.grepable:
-                                    if filename != '.' and filename != '..':
-                                        if (mysmb.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and mysmb.dir_only == False):
-                                            mysmb.outfile.write('host:{}, share:{}, privs:{}, isDir:{}, path:{}/{}/{}, fileSize:{}, date:{}\n'.format(host, share, smb_tree[host][share]['privs'].replace(',','').replace(' ', '_'), isDir, share, path, filename, str(filesize), date))
-
-                                elif mysmb.csv:
-                                    if filename != '.' and filename != '..':
-                                        if (mysmb.dir_only == True and isDir == 'd') or ( (isDir == 'f' or isDir == 'd') and mysmb.recursive ):
-                                            row = {}
-                                            row['Host'] = host
-                                            row['Share'] = share
-                                            row['Privs'] = smb_tree[host][share]['privs'].replace(',','').replace(' ', '_')
-                                            row['isDir'] = isDir
-                                            row['Path'] = '{}/{}/{}'.format(share, path, filename)
-                                            row['fileSize'] = str(filesize)
-                                            row['Date'] = date
-                                            mysmb.writer.writerow(row)
-
-            heads_up = False
-    except Exception as e:
-        print('[!] Bummer: ', e)
-
-def get_shares( share_args ):
-    # shares_args is a dict object with the following keys
-    #
-    # --Key--       --Description--
-    #
-    # smbconn       SMB connection object
-    # host          IP address
-    # write_check   determine if WRITE permissions are assisgned
-    # exclude       list of shares to exclude, like ipc$
-    #
-    # Returns a dict objects:
-    #   {ip_address : {share_name : {'privs': 'val', 'comment' : 'val'} } }
-    #
-    #   Example ThreadPool return set:
-    #   [{'192.168.86.48': {
-    #       'print$': {'privs': 'NO ACCESS', 'comment': 'Printer Drivers'},
-    #       'HP_LaserJet_1020': {'privs': 'NO ACCESS', 'comment': ''} }
-    #    },
-    #    {'192.168.86.106': {
-    #       'ADMIN$': {'privs': 'READ, WRITE', 'comment': 'Remote Admin'},
-    #       'C': {'privs': 'READ ONLY', 'comment': ''},
-    #       'C$': {'privs': 'READ, WRITE', 'comment': 'Default share'},
-    #       'Users': {'privs': 'READ, WRITE', 'comment': ''}}
-    #    } ]
-
-    share_tree = {}
-    if share_args['smbconn'].getSessionKey():
-        try:
-            shareList = share_args['smbconn'].listShares()
-            shares = []
-            for item in range(len(shareList)):
-                shares.append( (shareList[item]['shi1_netname'][:-1], shareList[item]['shi1_remark'][:-1]) )
-
-            share_privs = ''
-            share_comment = ''
-            host = share_args['host']
-            share_tree[host] = {}
-            for share in shares:
-                if share[0].lower() not in share_args['exclude']:
-                    share_name = share[0]
-                    share_comment = share[1]
-                    share_tree[host][share_name] = {}
-                    canWrite = False
-                    readonly = False
-                    noaccess = False
-                    if share_args['write_check']:
-                        try:
-                            root = PERM_DIR.replace('/','\\')
-                            root = ntpath.normpath(root)
-                            create_dir(share_args['smbconn'], share_name, root)
-                            share_tree[host][share_name]['privs'] = 'READ, WRITE'
-                            canWrite = True
-                            try:
-                                remove_dir(share_args['smbconn'], share_name, root)
-                            except Exception as e:
-                                print('[!] Unable to remove test directory at \\\\%s\\%s\\%s<file://%25s/%25s/%25s>, please remove manually' % (host, share_name, root))
-                        except Exception as e:
-                            exc_type, exc_obj, exc_tb = sys.exc_info()
-                            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                            #print(exc_type, fname, exc_tb.tb_lineno)
-                            sys.stdout.flush()
-
-                        if canWrite == False:
-                            try:
-                                root = PERM_DIR.replace('/','\\')
-                                root = '{}.txt'.format(ntpath.normpath(root))
-                                create_file(share_args['smbconn'], share_name, root)
-                                share_tree[host][share_name]['privs'] = 'READ, WRITE'
-                                canWrite = True
-                                try:
-                                    remove_file(share_args['smbconn'], share_name, root)
-                                except Exception as e:
-                                    if 'STATUS_OBJECT_NAME_NOT_FOUND' in str(e):
-                                        pass
-                                    else:
-                                        print('[!] Unable to remove test file at \\\\{}\\{}\\{}, please remove manually'.format(host, share_name, root))
-                            except Exception as e:
-                                exc_type, exc_obj, exc_tb = sys.exc_info()
-                                fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                                #print(exc_type, fname, exc_tb.tb_lineno)
-                                sys.stdout.flush()
-
-                    try:
-                        if share_args['smbconn'].listPath(share_name, pathify('/')) and canWrite == False:
-                            readonly = True
-                            share_tree[host][share_name]['privs'] = 'READ ONLY'
-                    except Exception as e:
-                        noaccess = True
-                        share_tree[host][share_name]['privs'] = 'NO ACCESS'
-                    share_tree[host][share_name]['comment'] = share_comment
-
-            return share_tree
-        except SessionError as e:
-            print('[!] Access denied on {}, no fun for you...'.format(share_args['host']))
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            print('[!] Something weird happened on ({}) {} on line {}'.format(share_args['host'], e, exc_tb.tb_lineno))
-            sys.stdout.flush()
-    return {}
-
-def list_path( list_args ):
-    # list_args is a dict object with the following keys
-    #
-    # --Key--       --Description--
-    #
-    # smbconn       SMB connection object
-    # share         share drive to list (ls)
-    # path          path on drive to list
-    # path_list     child path list (it's a recursive function)
-    # depth         how many nodes deep to traverse the tree
-    # pattern       pattern to match against file names
-    # dir_only      list only directories, skip files
-
-
-    pwd = pathify(list_args['path'])
-    width = 16
-    share = list_args['share']
-    depth = list_args['depth']
-    path = list_args['path']
-    host = list_args['host']
-
-    if list_args['path_list'] is None:
-        list_args['path_list'] = {}
-        path_list = { host : { share : {} } }
-    else:
-        path_list = list_args['path_list']
-
-    try:
-
-        raw_path_list = list_args['smbconn'].listPath(share, pwd)
-        path_list[host][share][path] = []
-        for item in raw_path_list:
-            filesize = item.get_filesize()
-            readonly = 'w' if item.is_readonly() > 0 else 'r'
-            date = time.ctime(float(item.get_mtime_epoch()))
-            isDir = 'd' if item.is_directory() > 0 else 'f'
-            filename = item.get_longname()
-            if isDir == 'f':
-                if list_args['pattern']:
-                    fileMatch = re.search(list_args['pattern'].lower(), filename.lower())
-                    if fileMatch:
-                        if len(path) > 0 and path[0] == '/':
-                            dlThis = '{}{}/{}'.format(share, path, filename)
-                        else:
-                            dlThis = '{}/{}/{}'.format(share, path, filename)
-                        #dlThis = dlThis.replace('/','\\')
-                        print('[+] Match found! Downloading: {}'.format(dlThis))
-                        download_file(list_args['smbconn'], dlThis)
-            if (list_args['dir_only'] and isDir == 'd') or ( list_args['dir_only'] == False):
-                path_list[host][share][path].append({'isDir': isDir, 'readonly': readonly, 'filesize': filesize, 'date': date, 'filename': filename})
-        if int(depth) > 1:
-            for smbItem in path_list[host][share][path]:
-                try:
-                    if smbItem['isDir'] == 'd' and smbItem['filename'] not in [ '.', '..']:
-                        subPath = '{}/{}'.format(path, smbItem['filename'])
-                        subPath = pathify(subPath)
-                        raw_path_list  = list_args['smbconn'].listPath(share, subPath)
-                        if len(raw_path_list) > 2 and '{}/{}'.format(path, smbItem['filename']) not in path_list[host][share].keys() and subPath.count('\\')-1 <= int(depth):
-                            list_args['path'] = '{}/{}'.format(path, smbItem['filename'])
-                            list_args['path_list'] = path_list
-                            list_path( list_args )
-                except SessionError as e:
-                    continue
-
-        return path_list
-    except Exception as e:
-        exc_type, exc_obj, exc_tb = sys.exc_info()
-        fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-        print('[!] Something weird happened on ({}) {} on line {}'.format(host, e, exc_tb.tb_lineno))
-        sys.stdout.flush()
-
-def download_file(smbconn, path):
-    path = path.replace('/','\\')
-    path = ntpath.normpath(path)
-    filename = path.split('\\')[-1]
-    share = path.split('\\')[0]
-    path = path.replace(share, '', 1)
-    host = socket.gethostbyname(smbconn.getRemoteHost())
-
-    try:
-        output_path = ntpath.basename('%s/%s' % (os.getcwd(), '%s-%s%s' % (host, share.replace('$',''), path.replace('\\','_'))))
-        dlFile = smbconn.listPath(share, path)
-        print('[+] Starting download: {}{} ({} bytes)'.format(share, path, dlFile[0].get_filesize()))
-        with open(output_path, 'wb') as out:
-            smbconn.getFile(share, path, out.write)
-        print('[+] File output to: %s/%s' % (os.getcwd(), output_path))
-
-    except SessionError as e:
-        if 'STATUS_ACCESS_DENIED' in str(e):
-            print('[!] Error retrieving file, access denied')
-        elif 'STATUS_INVALID_PARAMETER' in str(e):
-            print('[!] Error retrieving file, invalid path')
-        elif 'STATUS_SHARING_VIOLATION' in str(e):
-            print('[!] Error retrieving file %s, sharing violation' % (filename))
-        elif 'STATUS_NO_SUCH_FILE' in str(e):
-            print('[!] Error retrieving file, no such file')
-        #os.remove(ntpath.basename('%s/%s' % (os.getcwd(), '%s-%s%s' % (host, share.replace('$',''), path.replace('\\','_')))))
-    return '{}/{}'.format(os.getcwd(),output_path)
-
-def create_file(smbconn, share, path):
-    tid = smbconn.connectTree(share)
-    fid = smbconn.createFile(tid, path, desiredAccess=FILE_SHARE_WRITE, shareMode=FILE_SHARE_DELETE)
-    smbconn.closeFile(tid, fid)
-
-def remove_file(smbconn, share, path):
-    #path = self.pathify(path)
-    smbconn.deleteFile(share, path)
-
-def remove_dir(smbconn, share, path):
-    #path = self.pathify(path)
-    smbconn.deleteDirectory(share, path)
-
-def pathify(path):
-    root = ''
-    root = ntpath.join(path,'*')
-    root = root.replace('/','\\')
-    root = root.replace('\\\\','\\')
-    root = ntpath.normpath(root)
-    return root
-
-def login_kerberos(host):
-    smbconn = None
-    try:
-        if host['port'] == 445:
-            smbconn = SMBConnection(host['ip'], host['ip'], sess_port=host['port'], timeout=3)
-        else:
-            smbconn = SMBConnection('*SMBSERVER', host['host'], sess_port=host['port'], timeout=3)
-    except Exception as e:
-            print('[!] Connection error on {}'.format(host['ip']))
-
-    if smbconn:
-        try:
-            smbconn.kerberosLogin(host['user'], host['passwd'], host['domain'], host['lmhash'], host['nthash'], kdcHost=host['kdc'], useCache=USE_CCACHE)
-        except Exception as e:
-            print('[!] Authentication error on {}'.format(host['ip']), e)
-
-        return smbconn
-
-    return False
-
 def login(host):
-    smbconn = None
     try:
         if host['port'] == 445:
-            smbconn = SMBConnection(host['ip'], host['ip'], sess_port=host['port'], timeout=3)
+            smbconn = SMBConnection(host['ip'], host['ip'], sess_port=host['port'], timeout=10)
         else:
-            smbconn = SMBConnection('*SMBSERVER', host['host'], sess_port=host['port'], timeout=3)
-    except Exception as e:
-        print('[!] Connection error on {}'.format(host['ip']))
-
-    if smbconn:
-        try:
-            smbconn.login(host['user'], host['passwd'], host['domain'], host['lmhash'], host['nthash'])
-            return smbconn
-        except Exception as e:
-            if VERBOSE:
-                print('[!] Authentication error on {}'.format(host['ip']))
+            smbconn = SMBConnection('*SMBSERVER', host['host'], sess_port=host['port'], timeout=10)
 
-    return False
+        smbconn.login(host['user'], host['passwd'], host['domain'], host['lmhash'], host['nthash'])
 
-def check_smb_signing(signing_args):
-    ip = signing_args['host']
-    my_smb = None
+        return smbconn
 
-    #First try to negotiate a session with legacy SMB dialect
-    try:
-        my_smb = smb.SMB('.', ip)
     except Exception as e:
-        pass
-
-    #Then try to negotiate a session with SMB3 dialect
-    if my_smb == None:
-        try:
-            my_smb = smb3.SMB3('.', ip)
-        except Exception as e:
-            pass
-
-    if my_smb:
-        try:
-            if my_smb._Connection['RequireSigning'] == True:
-                return { 'Host' : f'{ip:<16}', 'signing_status' : 'signing required' }
-            elif isinstance(my_smb, smb3.SMB3) and my_smb._Connection['RequireSigning'] == False:
-                return { 'Host' : f'{ip:<16}', 'signing_status' : 'signing enabled (not required)' }
-        except AttributeError as e:
-            pass
+        if VERBOSE:
+            print('[!] Authentication error on {}'.format(host['ip']))
+        return False
 
-        try:
-            if isinstance(my_smb, smb.SMB):
-                if my_smb._dialects_parameters:
-                    if my_smb._dialects_parameters.fields['SecurityMode'] == 7:
-                        return { 'Host' : f'{ip:<16}', 'signing_status' : 'signing enabled (not required)' }
-                    elif my_smb._dialects_parameters.fields['SecurityMode'] == 3:
-                        return { 'Host' : f'{ip:<16}', 'signing_status' : 'signing disabled' }
-        except Exception as e:
-            pass
-    return { 'Host' : f'{ip:<16}', 'signing_status' : 'unkown (possibly Linux)...' }
 
 def main():
     example = 'Examples:\n\n'
     example += '$ python smbmap.py -u jsmith -p password1 -d workgroup -H 192.168.0.1\n'
     example += '$ python smbmap.py -u jsmith -p \'aad3b435b51404eeaad3b435b51404ee:da76f2c4c96028b7a6111aef4a50a94d\' -H 172.16.0.20\n'
     example += '$ python smbmap.py -u \'apadmin\' -p \'asdf1234!\' -d ACME -Hh 10.1.3.30 -x \'net group "Domain Admins" /domain\'\n'
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter, description=banner, epilog=example)
 
     sgroup = parser.add_argument_group("Main arguments")
     mex_group = sgroup.add_mutually_exclusive_group(required=True)
     pass_group = sgroup.add_mutually_exclusive_group()
-    kerb_group = parser.add_argument_group('Kereros settings')
-    mex_group.add_argument("-H", metavar="HOST", dest='host', type=str, help="IP or FQDN", default=False)
+    mex_group.add_argument("-H", metavar="HOST", dest='host', type=str, help="IP of host")
     mex_group.add_argument("--host-file", metavar="FILE", dest="hostfile", default=False, type=argparse.FileType('r'), help="File containing a list of hosts")
 
-    sgroup.add_argument("-u","--username", metavar="USERNAME", dest='user', default='', help="Username, if omitted null session assumed")
-    pass_group.add_argument("-p", "--password", metavar="PASSWORD", dest='passwd', default='', help="Password or NTLM hash, format is LMHASH:NTHASH")
+    sgroup.add_argument("-u", metavar="USERNAME", dest='user', default='', help="Username, if omitted null session assumed")
+    pass_group.add_argument("-p", metavar="PASSWORD", dest='passwd', default='', help="Password or NTLM hash")
     pass_group.add_argument("--prompt", action='store_true', default=False, help="Prompt for a password")
-    kerb_group.add_argument("-k", "--kerberos", action='store_true', dest='kerberos_auth', default=False, help="Use Kerberos authentication")
-    kerb_group.add_argument("--no-pass", dest='no_pass', action='store_true', default=False, help="Use CCache file (export KRB5CCNAME='~/current.ccache')")
-    kerb_group.add_argument("--dc-ip", metavar="IP or Host", dest='dc_ip', default=None, help="IP or FQDN of DC")
     sgroup.add_argument("-s", metavar="SHARE", dest='share', default='C$', help="Specify a share (default C$), ex 'C$'")
     sgroup.add_argument("-d", metavar="DOMAIN", dest='domain', default="WORKGROUP", help="Domain name (default WORKGROUP)")
     sgroup.add_argument("-P", metavar="PORT", dest='port', type=int, default=445, help="SMB port (default 445)")
-    sgroup.add_argument("-v","--version", dest='version', default=False, action='store_true', help="Return the OS version of the remote host")
-    sgroup.add_argument("--signing", dest='signing', default=False, action='store_true', help="Check if host has SMB signing disabled, enabled, or required")
+    sgroup.add_argument("-v", dest='version', default=False, action='store_true', help="Return the OS version of the remote host")
     sgroup.add_argument("--admin", dest='admin', default=False, action='store_true', help='Just report if the user is an admin')
     sgroup.add_argument("--no-banner", dest='nobanner', default=False, action='store_true', help='Removes the banner from the top of the output')
     sgroup.add_argument("--no-color", dest='nocolor', default=False, action='store_true', help='Removes the color from output')
     sgroup.add_argument("--no-update", dest='noupdate', default=False, action='store_true', help='Removes the "Working on it" message')
-    sgroup.add_argument("--timeout", dest='scan_timeout', type=float, default=.5, help='Set port scan socket timeout. Default is .5 seconds')
 
     sgroup2 = parser.add_argument_group("Command Execution", "Options for executing commands on the specified host")
 
     sgroup2.add_argument("-x", metavar="COMMAND", dest='command', help="Execute a command ex. 'ipconfig /all'")
     sgroup2.add_argument("--mode", metavar="CMDMODE", dest='mode', default='wmi', help="Set the execution method, wmi or psexec, default wmi", choices=['wmi','psexec'])
 
     sgroup3 = parser.add_argument_group("Shard drive Search", "Options for searching/enumerating the share of the specified host(s)")
     mex_group2 = sgroup3.add_mutually_exclusive_group()
     mex_group2.add_argument("-L", dest='list_drives', action="store_true", help="List all drives on the specified host, requires ADMIN rights.")
-    mex_group2.add_argument("-r", metavar="PATH", dest="recursive_dir_list", nargs="?", const='/', help="Recursively list dirs and files (no share\path lists the root of ALL shares), ex. 'email/backup'")
+    mex_group2.add_argument("-R", metavar="PATH", dest="recursive_dir_list", nargs="?", const='', help="Recursively list dirs, and files (no share\path lists ALL shares), ex. 'C$\\Finance'")
+    mex_group2.add_argument("-r", metavar="PATH", dest="dir_list", nargs="?", const='', help="List contents of directory, default is to list root of all shares, ex. -r 'C$\Documents and Settings\Administrator\Documents'")
     mex_group3 = sgroup3.add_mutually_exclusive_group()
-    mex_group3.add_argument("-g", metavar="FILE", dest="grepable", default=False, help="Output to a file in a grep friendly format, used with -r (otherwise it outputs nothing), ex -g grep_out.txt")
+    mex_group3.add_argument("-A", metavar="PATTERN", dest="pattern", help="Define a file name pattern (regex) that auto downloads a file on a match (requires -R or -r), not case sensitive, ex '(web|global).(asax|config)'")
+    mex_group3.add_argument("-g", metavar="FILE", dest="grepable", default=False, help="Output to a file in a grep friendly format, used with -r or -R (otherwise it outputs nothing), ex -g grep_out.txt")
     mex_group3.add_argument("--csv", metavar="FILE", dest="csv", default=False, help="Output to a CSV file, ex --csv shares.csv")
     sgroup3.add_argument("--dir-only", dest='dir_only', action='store_true', help="List only directories, ommit files.")
     sgroup3.add_argument("--no-write-check", dest='write_check', action='store_false', help="Skip check to see if drive grants WRITE access.")
     sgroup3.add_argument("-q", dest="verbose", default=True, action="store_false", help="Quiet verbose output. Only shows shares you have READ or WRITE on, and suppresses file listing when performing a search (-A).")
-    sgroup3.add_argument("--depth", dest="depth", default=1, help="Traverse a directory tree to a specific depth. Default is 1 (root node).")
+    sgroup3.add_argument("--depth", dest="depth", default=5, help="Traverse a directory tree to a specific depth. Default is 5.")
     sgroup3.add_argument("--exclude", metavar="SHARE", dest="exclude", nargs="+", const=None, help="Exclude share(s) from searching and listing, ex. --exclude ADMIN$ C$'")
-    sgroup3.add_argument("-A", metavar="PATTERN", dest="pattern", help="Define a file name pattern (regex) that auto downloads a file on a match (requires -r), not case sensitive, ex '(web|global).(asax|config)'")
 
     sgroup4 = parser.add_argument_group("File Content Search", "Options for searching the content of files (must run as root), kind of experimental")
     sgroup4.add_argument("-F", dest="file_content_search", metavar="PATTERN", help="File content search, -F '[Pp]assword' (requires admin access to execute commands, and PowerShell on victim host)")
     sgroup4.add_argument("--search-path", dest="search_path", default="C:\\Users", metavar="PATH", help="Specify drive/path to search (used with -F, default C:\\Users), ex 'D:\\HR\\'")
     sgroup4.add_argument('--search-timeout', dest='search_timeout', default='300', metavar='TIMEOUT', help='Specifcy a timeout (in seconds) before the file search job gets killed. Default is 300 seconds.')
 
     sgroup5 = parser.add_argument_group("Filesystem interaction", "Options for interacting with the specified host's filesystem")
     sgroup5.add_argument("--download", dest='dlPath', metavar="PATH", help="Download a file from the remote system, ex.'C$\\temp\\passwords.txt'")
     sgroup5.add_argument("--upload", nargs=2, dest='upload', metavar=('SRC', 'DST'), help="Upload a file to the remote system ex. '/tmp/payload.exe C$\\temp\\payload.exe'")
     sgroup5.add_argument("--delete", dest="delFile", metavar="PATH TO FILE", help="Delete a remote file, ex. 'C$\\temp\\msf.exe'")
     sgroup5.add_argument("--skip", default=False, action="store_true", help="Skip delete file confirmation prompt")
 
+
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
 
     args = parser.parse_args()
 
     signal.signal(signal.SIGINT, signal_handler)
 
-    hosts_auth = []
-    host_list = []
+    hosts = []
     mysmb = SMBMap()
 
     if not args.nobanner:
         print(banner)
 
     if args.nocolor:
         USE_TERMCOLOR=False
     if args.noupdate:
         SEND_UPDATE_MSG=False
 
     if args.prompt:
         args.passwd = getpass.getpass()
 
-    if args.scan_timeout:
-        if args.scan_timeout > 0 and args.scan_timeout < 10:
-            PORT_SCAN_TIMEOUT = args.scan_timeout
+    mysmb.loader = Loader()
+    mysmb.loading = True
+    mysmb.loader.start()
 
     lsshare = False
     lspath = False
 
     if args.grepable:
         mysmb.grepable = args.grepable
         mysmb.outfile = open(args.grepable, 'w')
 
     if args.csv:
-        mysmb.csv = True
+        mysmb.csv = args.csv
         mysmb.outfile = open(args.csv, 'w')
-        if args.recursive_dir_list != None:
+        if args.recursive_dir_list != None or args.dir_list != None:
             csv_fields = ['Host', 'Share', 'Privs', 'isDir', 'Path', 'fileSize', 'Date']
-        elif args.version:
-            csv_fields = ['Host', 'Version', 'Name', 'Domain']
-        elif args.signing:
-            csv_fields = ['Host', 'signing_status']
         else:
             csv_fields = ['Host', 'Share', 'Privs', 'Comment']
         mysmb.writer = csv.DictWriter(mysmb.outfile, csv_fields)
         mysmb.writer.writeheader()
 
     if args.pattern:
         mysmb.pattern = args.pattern
         mysmb.verbose = False
+        args.grepable = False
+        args.csv = False
 
     if args.verbose == False:
         mysmb.verbose = False
+    else:
+        VERBOSE = True
 
     if args.dir_only:
         mysmb.dir_only = True
 
     if args.recursive_dir_list != None:
         mysmb.recursive = True
+        mysmb.list_files = True
+        try:
+            lspath = args.recursive_dir_list.replace('/','\\').split('\\')
+            lsshare = lspath[0]
+            lspath = '\\'.join(lspath[1:])
+        except:
+            pass
+
+    elif args.dir_list != None:
+        mysmb.list_files = True
         try:
-            lspath = args.recursive_dir_list.split('/')
+            lspath = args.dir_list.replace('/','\\').split('\\')
             lsshare = lspath[0]
-            lspath = '/'.join(lspath[1:])
+            lspath = '\\'.join(lspath[1:])
         except:
-            lspath = '/'
             pass
+    socket.setdefaulttimeout(3)
 
     if args.exclude:
         for ex_share in args.exclude:
             mysmb.exclude.append(ex_share.lower())
 
-    if args.hostfile:
-        with args.hostfile as file:
-            for host in file.readlines():
-                host = host.strip()
-                if host.find('/') > 0:
-                    try:
-                        host_list = [ str(ip) for ip in ipaddress.ip_network(host, False).hosts() ]
-                    except Exception as e:
-                        print(f'[!] Invalid CIDR or host {host}')
-                else:
-                    try:
-                        if socket.gethostbyname(host):
-                            host_list.append(host)
-                    except socket.gaierror as e:
-                        print(f'[!] Name or service not known ({host})')
-
-    if args.host and not args.hostfile:
+    if args.host:
         if args.host.find('/') > 0:
             try:
-                host_list = [ str(ip) for ip in ipaddress.ip_network(args.host, False).hosts() ]
+                args.hostfile = [ str(ip) for ip in ipaddress.ip_network(args.host, False).hosts() ]
             except Exception as e:
-                print(f'[!] Invalid CIDR or host {args.host}')
-                sys.exit(1)
-        else:
-            try:
-                if socket.gethostbyname(args.host):
-                    host_list.append(args.host)
-            except socket.gaierror as e:
-                print(f'[!] Name or service not known ({args.host})')
+                print('[!] Invalid host...')
                 sys.exit(1)
 
-    mysmb.loader = Loader('Checking for open ports...')
-    mysmb.loading = True
-    mysmb.loader.start()
-    if len(host_list) > 0:
-        porty_time = Pool()
-        host_list = porty_time.map(find_open_ports, host_list)
-        print('[*]','Detected {} hosts serving SMB'.format(sum(im_open is not False for im_open in host_list)))
-    else:
-        mysmb.loader.terminate()
-        print('[!] No valid hosts provided')
-        sys.exit(1)
+    if args.hostfile:
+        print('[*]', 'Checking for open ports...')
+        porty_time = Pool(40)
+        args.hostfile = porty_time.map(find_open_ports, args.hostfile)
+        print('[*]','Detected {} hosts serving SMB'.format(sum(im_open is not False for im_open in args.hostfile)))
 
     if mysmb.is_ntlm(args.passwd):
         lmhash, nthash = args.passwd.split(':')
     else:
         lmhash, nthash = ('', '')
 
-    if args.dc_ip:
-        kdc_host = args.dc_ip
-    else:
-        kdc_host = ''
-
-    if args.no_pass:
-        global USE_CCACHE
-        USE_CCACHE = True
-
-    mysmb.loader.update('Initializing hosts...')
-    if host_list:
-        host_args = []
-        for ip in host_list:
+    if args.hostfile:
+        for ip in args.hostfile:
             if ip:
-                host_args.append({ 'ip' : ip.strip(), 'port' : args.port, 'user' : args.user, 'passwd' : args.passwd, 'domain' : args.domain, 'lmhash' : lmhash, 'nthash' : nthash, 'smbconn' : [] ,'kdc_host' : kdc_host })
-        init_hosts_pool = Pool()
-        hosts_auth = init_hosts_pool.map(init_host, host_args)
+                try:
+                    hosts.append({ 'ip' : ip.strip(), 'name' : socket.getnameinfo((ip.strip(), args.port),0)[0] , 'port' : args.port, 'user' : args.user, 'passwd' : args.passwd, 'domain' : args.domain, 'lmhash' : lmhash, 'nthash' : nthash })
+                except:
+                    hosts.append({ 'ip' : ip.strip(), 'name' : 'unknown', 'port' : 445, 'user' : args.user, 'passwd' : args.passwd, 'domain' : args.domain, 'lmhash' : lmhash, 'nthash' : nthash })
+                    continue
+    elif args.host and args.host.find('/') == -1:
+        if find_open_ports(args.host.strip()):
+            try:
+                hosts.append({ 'ip' : args.host.strip(), 'name' : socket.getnameinfo((args.host.strip(), args.port),0)[0], 'port' : args.port, 'user' : args.user, 'passwd' : args.passwd, 'domain' : args.domain, 'lmhash' : lmhash, 'nthash' : nthash})
+            except:
+                hosts.append({ 'ip' : args.host.strip(), 'name' : 'unknown', 'port' : args.port, 'user' : args.user, 'passwd' : args.passwd, 'domain' : args.domain, 'lmhash' : lmhash, 'nthash' : nthash })
 
     if args.admin:
-        mysmb.admin_only = True
+        mysmb.verbose = False
 
-    mysmb.loader.update('Authenticating...')
     connections = []
-    if args.kerberos_auth:
-        login_worker = Pool()
-        connections = login_worker.map(login_kerberos, hosts_auth)
-    else:
-        login_worker = Pool()
-        connections = login_worker.map(login, hosts_auth)
-    if len(connections) > 0:
-        print('[*] Established {} SMB connections(s) and {} authenticated session(s)'.format(len( [ True for conn in connections if conn != False ]), len([ True for conn in connections if ( conn != False and conn.getSessionKey()) ])))
-    mysmb.hosts = { value['ip']:value for value in hosts_auth }
-    for conn in connections:
-        if conn:
-            mysmb.hosts[ socket.gethostbyname(conn.getRemoteHost()) ]['smbconn'].append(conn)
-
+    login_worker = Pool(40)
+    connections = login_worker.map(login, hosts)
+    mysmb.hosts = { value['ip']:value for value in hosts }
+    mysmb.smbconn = { conn.getRemoteHost():conn for conn in connections if conn is not False}
     counter = 0
 
     if args.file_content_search:
-        smb_server = mysmb.start_smb_server()
-        mysmb.loader.update('Doing RCE things...')
+        mysmb.start_smb_server()
         for host in list(mysmb.hosts.keys()):
             if args.search_path[-1] == '\\':
                 search_path = args.search_path[:-1]
             else:
                 search_path = args.search_path
             try:
-                if len(mysmb.hosts[host]['smbconn'][0].listPath('ADMIN$', '/*')) > 0:
+                if len(mysmb.smbconn[host].listPath('ADMIN$', mysmb.pathify('/'))) > 0:
                     mysmb.start_file_search(host, args.file_content_search, args.share, search_path)
                     counter += 1
-            except Exception as e:
+            except:
                 pass
+            mysmb.kill_loader()
         print('[+] File search started on {} hosts in directory {}...this could take a while'.format(counter, search_path))
         mysmb.get_search_results(args.search_timeout)
-        mysmb.loader.update('Cleaning up!')
-        smb_server.stop()
+        if mysmb.loading:
+            mysmb.kill_loader()
+        for host in list(mysmb.hosts.keys()):
+            try:
+                mysmb.logout(host)
+            except:
+                continue
+
+    if mysmb.loading:
+        mysmb.kill_loader()
 
     if not args.file_content_search:
-        if not args.dlPath and not args.upload and not args.delFile and not args.list_drives and not args.command and not args.version and not args.signing:
+        for host in list(mysmb.smbconn.keys()):
+            is_admin = False
+            try:
+                if len(mysmb.smbconn[host].listPath('ADMIN$', mysmb.pathify('/'))) > 0:
+                    is_admin = True
+            except:
+                pass
 
-            share_pool = Pool()
-            share_args = [ { 'smbconn' : mysmb.hosts[host]['smbconn'][0] , 'host' : host, 'write_check' : args.write_check, 'exclude' : mysmb.exclude } for host in mysmb.hosts.keys() if len(mysmb.hosts[host]['smbconn']) > 0 ]
+            mysmb.loader = Loader()
+            mysmb.loading = True
+            mysmb.loader.start()
+
+            try:
+                if args.dlPath:
+                    mysmb.download_file(host, args.dlPath)
 
-            mysmb.loader.update('Enumerating shares...')
+                if args.upload:
+                    mysmb.upload_file(host, args.upload[0], args.upload[1])
 
-            # this call returns an array of dict objects
-            all_shares = share_pool.map(get_shares, share_args)
-
-            smb_tree = {}
-            all_paths_listed = []
-            list_path_args = []
-            if mysmb.recursive or mysmb.dir_only and all_shares:
-                for host_shares in all_shares:
-                    if len(host_shares.keys()) > 0:
-                        host = [ host for host in host_shares.keys() ][0]
+                if args.delFile:
+                    mysmb.delete_file(host, args.delFile)
+
+                if args.list_drives:
+                    if is_admin:
+                        mysmb.list_drives(host, args.share)
                     else:
-                        continue
-                    if len(host_shares[host].keys()) > 0:
-                        mysmb.hosts[host]['smbconn'][0].close()
-                        mysmb.hosts[host]['smbconn'].pop()
-                        share_conns = login_worker.map(login, [ mysmb.hosts[host] for index in range(0,len(host_shares[host].keys())) ] )
-                        mysmb.hosts[host]['smbconn'] = share_conns
-                        for index, share_name in enumerate(host_shares[host].keys()):
-                            if host_shares[host][share_name]['privs'] != 'NO ACCESS' and lsshare == '':
-                                list_path_args.append({ 'smbconn' : mysmb.hosts[host]['smbconn'][index] , 'host' : host, 'share' : share_name, 'path' : lspath, 'path_list' : None, 'depth' : args.depth , 'dir_only' : mysmb.dir_only, 'pattern' : mysmb.pattern })
-                            elif host_shares[host][share_name]['privs'] != 'NO ACCESS' and share_name.lower() == lsshare.lower():
-                                list_path_args.append({ 'smbconn' : mysmb.hosts[host]['smbconn'][index] , 'host' : host, 'share' : share_name, 'path' : lspath, 'path_list' : None, 'depth' : args.depth , 'dir_only' : mysmb.dir_only, 'pattern' : mysmb.pattern })
-                if args.pattern:
-                    print('[*] Performing file name pattern match! ')
-                list_path_pool = Pool()
-                mysmb.loader.update('Traversing shares...')
-                all_paths_listed = list_path_pool.map(list_path, list_path_args)
-                prev_hoat = None
-
-            for share_drives_list in all_shares:
-                if isinstance(share_drives_list, dict) and len(share_drives_list) > 0:
-                    host = [ host for host in share_drives_list.keys() ][0]
-                    smb_tree[host] = {}
-                    for share in share_drives_list[host]:
-                        smb_tree[host][share] = share_drives_list[host][share]
-                        smb_tree[host][share]['contents'] = {}
-
-            for path_list in all_paths_listed:
-                if path_list:
-                    host = [ host for host in path_list.keys() ][0]
-                    for share_drive_contents in path_list[host]:
-                        if path_list[host][share_drive_contents]:
-                            smb_tree[host][share_drive_contents]['contents'] = path_list[host][share_drive_contents]
-
-            mysmb.loader.update('Finished!')
-            mysmb.loader.pause()
-            to_string(smb_tree, mysmb)
-
-        if args.version:
-            mysmb.loader.update('Grabbing version info.')
-            mysmb.loader.pause()
-            version_args = [ { 'smbconn' : mysmb.hosts[host]['smbconn'][0] , 'host' : host } for host in mysmb.hosts.keys() if len(mysmb.hosts[host]['smbconn']) > 0 ]
-            version_pool = Pool()
-            versions = version_pool.map(get_version, version_args)
-            for version_info in versions:
-                print("[+] {:<16} is running {} (name:{}) (domain:{})".format(version_info['Host'], version_info['Version'], version_info['Name'], version_info['Domain']))
-                if args.csv:
-                    mysmb.writer.writerow(version_info)
-
-
-        if args.signing:
-            mysmb.loader.update('Checking for SMB signing.')
-            signing_args = [ { 'smbconn' : mysmb.hosts[host]['smbconn'][0] , 'host' : host } for host in mysmb.hosts.keys() if len(mysmb.hosts[host]['smbconn']) > 0 ]
-            signing_pool = Pool()
-            signing = signing_pool.map(check_smb_signing, signing_args)
-            mysmb.loader.pause()
-            for signing_info in signing:
-                print(f'[!] {signing_info["Host"]}\t{signing_info["signing_status"]}')
-                if args.csv:
-                    mysmb.writer.writerow(signing_info)
-
-        if True in [ isinstance(arg, str) for arg in (args.dlPath, args.upload, args.delFile, args.list_drives, args.command) ]:
-            for host in list(mysmb.hosts.keys()):
-                is_admin = False
-                try:
-                    if len(mysmb.hosts[host]['smbconn'][0].listPath('ADMIN$', pathify('/'))) > 0:
-                        is_admin = True
-                except Exception as e:
-                    pass
+                        mysmb.kill_loader()
 
-                try:
-                    if args.dlPath:
-                        download_file(mysmb.hosts[host]['smbconn'][0], args.dlPath)
+                if args.command:
+                    if is_admin:
+                        mysmb.exec_command(host, args.share, args.command, True, mysmb.hosts[host]['name'], args.mode)
+                    else:
+                        mysmb.kill_loader()
 
-                    if args.upload:
-                        mysmb.upload_file(host, args.upload[0], args.upload[1])
+                if args.version:
+                    mysmb.get_version(host)
 
-                    if args.delFile:
-                        mysmb.delete_file(host, args.delFile)
+                if not args.dlPath and not args.upload and not args.delFile and not args.list_drives and not args.command and not args.file_content_search and not args.version:
 
-                    if args.list_drives:
-                        if is_admin:
-                            mysmb.list_drives(host, args.share)
-
-                    if args.command:
-                        mysmb.loader.update('Executing {} command, hang tight...'.format(args.mode))
-                        if is_admin:
-                            cmd_output = mysmb.exec_command(host, args.share, args.command, False, mysmb.hosts[host]['name'], args.mode)
-                            if cmd_output:
-                                print(cmd_output)
+                    if mysmb.smbconn[host].isGuestSession() > 0:
+                        priv_status = 'Status: ' + colored('Guest session   \t', 'yellow')
+                    elif is_admin:
+                        priv_status = 'Status: ' + colored('ADMIN!!!', 'green', attrs=['bold','underline']) + '   \t'
+                    else:
+                        priv_status = 'Status: ' + colored ('Authenticated', 'green')
 
-                except Exception as e:
-                    print('[!]', e)
-                    sys.stdout.flush()
+                    if (not mysmb.grepable and not args.admin and not mysmb.csv) or (not mysmb.grepable and not mysmb.csv and args.admin and is_admin):
+                        print(' '*100)
+                        print('[+] IP: {}:{}\tName: {}\t{}'.format(host, mysmb.hosts[host]['port'], mysmb.hosts[host]['name'].ljust(20), priv_status ))
+                    tmp = mysmb.get_shares(host)
+                    if not args.admin and tmp is not None:
+                        mysmb.output_shares(host, lsshare, lspath, args.write_check, args.depth)
+
+                if mysmb.loading:
+                    mysmb.kill_loader()
+                mysmb.loader = None
+                try:
+                    mysmb.logout(host)
+                except:
                     pass
 
-        mysmb.loader.resume()
-        mysmb.loader.update('Closing connections..')
-        logoff_args = [ { 'smbconn' : mysmb.hosts[host]['smbconn'][0] , 'host' : host } for host in mysmb.hosts.keys() if len(mysmb.hosts[host]['smbconn']) > 0 ]
-        logoff_pool = Pool()
-        loggedoff = logoff_pool.map(close_smb_connection, logoff_args)
-        mysmb.loader.pause()
-        mysmb.kill_loader()
-        print('[*]','Closed {} connections'.format(len(loggedoff)))
+            except Exception as e:
+                exc_type, exc_obj, exc_tb = sys.exc_info()
+                fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                print('[!] Error: ', (exc_type, fname, exc_tb.tb_lineno))
+                sys.stdout.flush()
 
         if args.grepable or args.csv:
             print('[*]','Results output to: {}'.format(mysmb.outfile.name))
             mysmb.outfile.close()
 
-    sys.exit()
-
 
 if __name__ == "__main__":
     main()
```

