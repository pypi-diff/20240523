# Comparing `tmp/rskfd-0.5.0.tar.gz` & `tmp/rskfd-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rskfd-0.5.0.tar", last modified: Fri May 17 10:46:22 2024, max compression
+gzip compressed data, was "rskfd-0.5.1.tar", last modified: Thu May 23 06:23:24 2024, max compression
```

## Comparing `rskfd-0.5.0.tar` & `rskfd-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.482769 rskfd-0.5.0/
--rw-rw-rw-   0        0        0     2247 2024-05-17 10:46:22.482769 rskfd-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.444896 rskfd-0.5.0/examples/
--rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.5.0/examples/Wv2BinStream.py
--rw-rw-rw-   0        0        0     3001 2024-05-17 10:05:47.000000 rskfd-0.5.0/examples/fileopening.py
--rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.5.0/examples/instrumentexamples.py
--rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.5.0/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.446890 rskfd-0.5.0/rskfd/
--rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.5.0/rskfd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.460843 rskfd-0.5.0/rskfd/helper/
--rw-rw-rw-   0        0        0     4386 2024-05-17 07:08:58.000000 rskfd-0.5.0/rskfd/helper/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.463832 rskfd-0.5.0/rskfd/iq_data_handling/
--rw-rw-rw-   0        0        0    24739 2024-05-17 10:39:51.000000 rskfd-0.5.0/rskfd/iq_data_handling/iqdata.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.474796 rskfd-0.5.0/rskfd/remote_control/
--rw-rw-rw-   0        0        0    14935 2024-04-16 04:51:55.000000 rskfd-0.5.0/rskfd/remote_control/instrument.py
--rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRS.py
--rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRSExceptions.py
--rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRS_FSW.py
--rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.5.0/rskfd/remote_control/instrumentRS_VSE.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.476789 rskfd-0.5.0/rskfd/signal_generation/
--rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.5.0/rskfd/signal_generation/signal_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.478783 rskfd-0.5.0/rskfd/snp_handling/
--rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.5.0/rskfd/snp_handling/snpfiles.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:46:22.480777 rskfd-0.5.0/rskfd.egg-info/
--rw-rw-rw-   0        0        0     2247 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-17 10:46:22.000000 rskfd-0.5.0/rskfd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-17 10:46:22.484767 rskfd-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1438 2024-05-17 10:45:19.000000 rskfd-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.291204 rskfd-0.5.1/
+-rw-rw-rw-   0        0        0     2247 2024-05-23 06:23:24.290206 rskfd-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.256203 rskfd-0.5.1/examples/
+-rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.5.1/examples/Wv2BinStream.py
+-rw-rw-rw-   0        0        0     3001 2024-05-17 10:05:47.000000 rskfd-0.5.1/examples/fileopening.py
+-rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.5.1/examples/instrumentexamples.py
+-rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.5.1/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.258201 rskfd-0.5.1/rskfd/
+-rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.5.1/rskfd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.269203 rskfd-0.5.1/rskfd/helper/
+-rw-rw-rw-   0        0        0     4386 2024-05-17 07:08:58.000000 rskfd-0.5.1/rskfd/helper/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.271203 rskfd-0.5.1/rskfd/iq_data_handling/
+-rw-rw-rw-   0        0        0    24739 2024-05-17 10:39:51.000000 rskfd-0.5.1/rskfd/iq_data_handling/iqdata.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.281202 rskfd-0.5.1/rskfd/remote_control/
+-rw-rw-rw-   0        0        0    15063 2024-05-23 06:20:10.000000 rskfd-0.5.1/rskfd/remote_control/instrument.py
+-rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.5.1/rskfd/remote_control/instrumentRS.py
+-rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.5.1/rskfd/remote_control/instrumentRSExceptions.py
+-rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.5.1/rskfd/remote_control/instrumentRS_FSW.py
+-rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.5.1/rskfd/remote_control/instrumentRS_VSE.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.284204 rskfd-0.5.1/rskfd/signal_generation/
+-rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.5.1/rskfd/signal_generation/signal_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.285204 rskfd-0.5.1/rskfd/snp_handling/
+-rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.5.1/rskfd/snp_handling/snpfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:23:24.288205 rskfd-0.5.1/rskfd.egg-info/
+-rw-rw-rw-   0        0        0     2247 2024-05-23 06:23:24.000000 rskfd-0.5.1/rskfd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-05-23 06:23:24.000000 rskfd-0.5.1/rskfd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:23:24.000000 rskfd-0.5.1/rskfd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 06:23:24.000000 rskfd-0.5.1/rskfd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-23 06:23:24.000000 rskfd-0.5.1/rskfd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-23 06:23:24.292204 rskfd-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1438 2024-05-23 06:21:16.000000 rskfd-0.5.1/setup.py
```

### Comparing `rskfd-0.5.0/PKG-INFO` & `rskfd-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.5.0/README.md` & `rskfd-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/examples/Wv2BinStream.py` & `rskfd-0.5.1/examples/Wv2BinStream.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/examples/fileopening.py` & `rskfd-0.5.1/examples/fileopening.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/examples/instrumentexamples.py` & `rskfd-0.5.1/examples/instrumentexamples.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/license.txt` & `rskfd-0.5.1/license.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/__init__.py` & `rskfd-0.5.1/rskfd/__init__.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/helper/helper.py` & `rskfd-0.5.1/rskfd/helper/helper.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/iq_data_handling/iqdata.py` & `rskfd-0.5.1/rskfd/iq_data_handling/iqdata.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/remote_control/instrument.py` & `rskfd-0.5.1/rskfd/remote_control/instrument.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,28 +40,28 @@
         '''
         OpcQuery = 0
         Blocking = 1
         StbPoll = 2
 
 
     @staticmethod
-    def GetNumberOfDigits( number):
+    def GetNumberOfDigits(number):
         '''
         count number of digits
         '''
 
         if number < 0:
             number *= -1
         if number == 0:
             return 1
 
         return math.ceil(math.log10( number))
 
 
-    def __init__(self, IpAddress, port=5025, timeout = 2, sendcls = True):
+    def __init__(self, IpAddress, port=5025, timeout=2, sendcls=True):
         '''
         init method;
             IP Address is required
             port            : port to communicate with
             timeout         : timeout value
             sendcls         : clear error queue before communicating to instrument
         '''
@@ -98,15 +98,15 @@
         self.__Options.remove("")
 
 
     def GetOpt(self):
         '''
         return the instrument's option string
         '''
-        if self.__Options == None:
+        if self.__Options is None:
             self.__QueryOpt()
         return self.__Options
 
 
     def IsLocalHost(self):
         '''
         Return boolean true when instrument runs on localhost (e.g. VSE)
@@ -114,35 +114,35 @@
         if self.__ipaddress.lower().find('localhost') >= 0 | self.__ipaddress.lower().find('127.0.0.1'):
             # missing check for same IP address
             return True
         else:
             return False
 
 
-    def SetTimeout( self, timeout):
+    def SetTimeout(self, timeout):
         '''
         Set the timeout for the connection (non blocking socket).
         For a blocking socket, use 'None'
         '''
         self.__timeout = timeout
         try:
             self.__msocket.settimeout( self.__timeout)
         except:
             pass
 
 
 
-    def GetTimeout( self):
+    def GetTimeout(self):
         '''
         Returns the specified timeout, 'None' meaning blocking socket
         '''
         return self.__msocket.gettimeout()
 
 
-    def Synchronize( self, method = SyncMethod.StbPoll, timeout = None ):
+    def Synchronize(self, method=SyncMethod.StbPoll, timeout=None):
         '''Function to synchronize with instruments.
         Input:
         SyncMethod:
             SyncMethod.OpcQUery:    Use *OPC? to synchronize, i.e. a blocking query
             SyncMethod.Blocking:    Use *WAI to synchronize, i.e. block execution of next command until finished, no query
             SyncMethod.StbPoll:     Poll *ESR? until bit 0 is set, i.e. non blocking query
         timeout:    Timeout value, before function returns with timeout error
@@ -150,78 +150,78 @@
         Output:
         SyncOk: returns 1 when sync was successful, or 0 on timeout
         '''
 
         SyncOk = 0
 
         # Save current timeout and set user timeout
-        if timeout != None:
+        if timeout is None:
             timeoutstorage = self.__timeout
-            self.SetTimeout( timeout)
+            self.SetTimeout(timeout)
         else:
             timeout = self.GetTimeout()
 
         # OPC Query Sync mode
         if method == self.SyncMethod.OpcQuery:
-            self.Write( '*OPC?')
+            self.Write('*OPC?')
             try:
                 value = int(self.Read())
                 if value == 1:
                     SyncOk = 1
             except socket.timeout:
                 pass
 
         # *WAI blocking mode
         if method == self.SyncMethod.Blocking:
-            self.Write( '*WAI')
+            self.Write('*WAI')
 
-         # *ESR? polling mode
+        # *ESR? polling mode
         if method == self.SyncMethod.StbPoll:
-            self.Write( '*OPC')
+            self.Write('*OPC')
             start = timeit.default_timer()
-            while( not SyncOk and ((timeit.default_timer()-start)<=self.__timeout) ):
-                SyncOk = int(self.Query( '*ESR?')) & 1
-                #sleep for 2 ms, so we don't poll too often
-                time.sleep( .002)
+            while(not SyncOk and ((timeit.default_timer()-start) <= self.__timeout) ):
+                SyncOk = int(self.Query('*ESR?')) & 1
+                # sleep for 2 ms, so we don't poll too often
+                time.sleep(.002)
 
         # Restore timeout
         if timeout != self.__timeout:
-            self.SetTimeout( timeoutstorage)
+            self.SetTimeout(timeoutstorage)
 
         return SyncOk
 
 
-    def Connect( self, getID = True, getOptions = False, Preset = False):
+    def Connect(self, getID=True, getOptions=False, Preset=False):
         '''
         Connects to the specified instrument and opens the connection
         '''
 
         try:
             self.__msocket = socket.socket( socket.AF_INET, socket.SOCK_STREAM)
             self.__msocket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
             self.__msocket.connect( (self.__ipaddress, self.__port))
-            self.__msocket.settimeout( self.__timeout)
+            self.__msocket.settimeout(self.__timeout)
             if Preset:
-                self.Query( '*RST;*OPC?')
+                self.Query('*RST;*OPC?')
             #Clear Error Queue
             if self.__sendcls:
-                self.Write( '*CLS')
+                self.Write('*CLS')
             if getID:
                 self.__QueryID()
             if getOptions:
                 self.__QueryOpt()
         except ConnectionRefusedError:
             return -1
         except TimeoutError:
             return -1
 
         return 0
 
 
-    def Close( self):
+    def Close(self):
         '''
         Closes the connection
         '''
 
         self.CloseSocket()
         return
 
@@ -230,256 +230,262 @@
         '''
         Start logging into FileName
         ClearFile deletes file, if set to True
         '''
         FileMode = 'a'
         if ClearFile:
             FileMode = 'w'
-        self.__LogFile = open( FileName, FileMode)
+        self.__LogFile = open(FileName, FileMode)
         self.__LogReadings = LogReadings
         self.__TimeStamp = TimeStamp
 
 
-    def StopLogging( self):
+    def StopLogging(self):
         '''
         Stop logging
         '''
         self.__LogFile.close()
         self.__LogFile = None
 
 
-    def ___LogToFile( self, Command):
+    def UserCommentToLogFile(self, comment):
+        '''
+        Write a user comment to the log file
+        '''
+        comment = 'USERCOMMENT: ' + comment
+        self.___LogToFile(comment)
+
+
+    def ___LogToFile(self, Command):
         if self.__LogFile is None:
             return -1
 
         if self.__TimeStamp:
-            print()
             self.__LogFile.write('{:%Y-%m-%d %H:%M:%S.%f}   '.format(datetime.datetime.now())+Command+"\n")
         else:
             self.__LogFile.write(Command+"\n")
         return 0
 
 
-    def Write( self, Command, Binary = False, AddTermination = True):
+    def Write(self, Command, Binary=False, AddTermination=True):
         '''
         Write a command; termination character (\n) automatically added
         '''
-        
+
         if self.__msocket is None:
             raise Exception('Connection is closed, use connect first!')
-        
+
         self.___LogToFile( Command)
         if AddTermination:
             if Command.endswith("\n") is False:
                 Command = Command + "\n"
         if Binary:
-            self.__msocket.sendall( Command)
+            self.__msocket.sendall(Command)
         else:
-            self.__msocket.sendall( Command.encode('ASCII'))
+            self.__msocket.sendall(Command.encode('ASCII'))
 
-          
 
-    def Read( self, decode = True, NumberOfBytes = -1):
+    def Read(self, decode=True, NumberOfBytes=-1):
         '''
         Read back from the connected instrument
         '''
 
         if self.__msocket is None:
             raise Exception('Connection is closed, use connect first!')
 
         if NumberOfBytes == -1:
             NumberOfBytes = self._InBufferSize
 
         try:
             data = self.__msocket.recv(NumberOfBytes)
         except:
-            logging.warn("Timeout while reading data!")
+            message = "Timeout while reading data!"
+            if self.__LogReadings:
+                self.___LogToFile(message)
+            else:
+                logging.warn(message)
             return None
 
         if decode:
             try:
                 data = data.decode("ASCII")
                 if data.endswith("\n"):
                     data = data[:-1]
             except:
-                logging.warn("Binary data received!")
+                message = "Binary data received!"
+                if self.__LogReadings:
+                    self.___LogToFile(message)
+                else:
+                    logging.warn(message)
                 data = str(len(data)) + " binary bytes"
 
             if self.__LogReadings:
-                self.___LogToFile( data)
+                self.___LogToFile(data)
         else:
             if self.__LogReadings:
-                self.___LogToFile( "{} bytes of binary data read".format(len(data))) 
-        
+                self.___LogToFile("{} bytes of binary data read".format(len(data))) 
+
         return data
 
 
-    def Query( self, Command):
+    def Query(self, Command):
         """Write command and read result from connected instrument"""
-        
-        self.Write( Command)
+
+        self.Write(Command)
         data = self.Read()
-        
+
         return data
-    
-    
-    
-    def CloseSocket( self):
+
+
+    def CloseSocket(self):
         """Close the connection"""
         self.__msocket.close()
         self.__IDString = ""
         self.__Options = []
-        
-        
-        
+
+
     def OpenSocket( self):
         """Open the connection"""
         try:
-            self.__msocket.connect( (instrument.__ipaddress, instrument.__port))
-            self.__msocket.settimeout( self.__timeout)
+            self.__msocket.connect((instrument.__ipaddress, instrument.__port))
+            self.__msocket.settimeout(self.__timeout)
         except ConnectionRefusedError:
             pass
 
-    
-    
-    
-    def GetSystErr( self):
+
+    def GetSystErr(self):
         """Return system error as (integer,string)"""
-        self.Write( "SYST:ERR?")
+        self.Write("SYST:ERR?")
         result = self.Read()
         retlist = result.split(",")
-        
-        return int(retlist[0]),retlist[1]
 
+        return int(retlist[0]), retlist[1]
 
 
-    def UseNaN( self, vfcData):
+    def UseNaN(self, vfcData):
         """Replace the SCPI representation of NaN (9.91*10^37) by NaN"""
 
         return [math.nan if x > 9.909e37 else x for x in vfcData]
 
 
-    
-    def ReadBinary( self, BytesPerValue = 4, IqRead = False, NaNCheck = False, ReturnSamples = True):
+    def ReadBinary(self, BytesPerValue=4, IqRead=False, NaNCheck=False, ReturnSamples=True):
         """Binary read of multiple values from the instrument, e.g. trace or I/Q data
         Input Values:
             BytesPerValue:  specifies the number of bytes that form a float; in format REAL,32 this is 4
             IqRead:         if set to true, complex I/Q pairs are returned; works only if instrument returns samples in iqiq order
             NaNCheck:       if set to true, the SCPI representation of NaN is replaced by Python's NaN
             ReturnSamples:  only set to false for interface tests; if set to false, function will only read back bytes and dump them
 
         Output Values:
             data vector when ReturnSamples is true
             byte counter when ReturnSamples is false
             """
 
-        digits = self.Read( NumberOfBytes = 2)
+        digits = self.Read(NumberOfBytes=2)
 
         if digits[1] == "(":
             # in this case we have more than 10 digits for the number of bytes enclosed by "(" and ")"
-            digits += self.Read( NumberOfBytes = 11)
+            digits += self.Read(NumberOfBytes=11)
             while digits[-1] != ")":
-                digits += self.Read( NumberOfBytes = 1)
+                digits += self.Read(NumberOfBytes=1)
             NumberOfBytesToRead = int(digits[2:-1])
         else:
             digits = int(digits[1])
-            NumberOfBytesToRead = int(self.Read( NumberOfBytes = digits))
-        
+            NumberOfBytesToRead = int(self.Read(NumberOfBytes=digits))
+
         if ReturnSamples:
             # This is the real code to read out samples
             NumericData = []
             oldData = b""
-    
+
             ReadCounter = 0
-            while ReadCounter <= NumberOfBytesToRead:   #we need to also read the closing character
-                RawData = self.Read( decode=False)
+            while ReadCounter <= NumberOfBytesToRead:   # we need to also read the closing character
+                RawData = self.Read(decode=False)
                 ReadCounter += len(RawData)
                 RawData = oldData + RawData
                 ReadSamples = len(RawData) // BytesPerValue
                 if BytesPerValue == 4:
-                    NumericData.extend(list(struct.unpack("f"*ReadSamples,RawData[0:ReadSamples*BytesPerValue])))
+                    NumericData.extend(list(struct.unpack("f"*ReadSamples, RawData[0:ReadSamples*BytesPerValue])))
                 elif BytesPerValue == 8:
-                    NumericData.extend(list(struct.unpack("d"*ReadSamples,RawData[0:ReadSamples*BytesPerValue])))
+                    NumericData.extend(list(struct.unpack("d"*ReadSamples, RawData[0:ReadSamples*BytesPerValue])))
                 else:
                     logging.error("Format currently not supported!")
                 oldData = RawData[ReadSamples*BytesPerValue:]
-            
+
             if NaNCheck:
                 NumericData = self.UseNaN( NumericData)
-            
+
             if IqRead:
                 from rskfd import Iqiq2Complex
                 NumericData = Iqiq2Complex( NumericData)
 
             return NumericData
         else:
             # Binary Read and Dump results section; only a byte counter is returned; transfer speed check only
             ReadCounter = 0
             while ReadCounter <= NumberOfBytesToRead:   #we need to also read the closing character
                 RawData = self.Read( decode=False)
                 ReadCounter += len(RawData)
-            
+
             return ReadCounter
-    
-    
-    def ReadBinaryToFile( self, FileName):
+
+
+    def ReadBinaryToFile(self, FileName):
         """Binary read of multiple values from the instrument directly into an iqw file.
         This function assumes 4 byte floating point format, usually commanded by
         FORM REAL,32"""
-        
-        digits = self.Read( NumberOfBytes = 2)
+
+        digits = self.Read(NumberOfBytes=2)
 
         if digits[1] == "(":
             # in this case we have more than 10 digits for the number of bytes enclosed by "(" and ")"
-            digits += self.Read( NumberOfBytes = 11)
+            digits += self.Read(NumberOfBytes=11)
             while digits[-1] != ")":
-                digits += self.Read( NumberOfBytes = 1)
+                digits += self.Read(NumberOfBytes=1)
             NumberOfBytesToRead = int(digits[2:-1])
         else:
             digits = int(digits[1])
-            NumberOfBytesToRead = int(self.Read( NumberOfBytes = digits))
-        
-        file = open( FileName, "wb")
+            NumberOfBytesToRead = int(self.Read(NumberOfBytes=digits))
+
+        file = open(FileName, "wb")
 
         ReadCounter = 0
-        while ReadCounter <= NumberOfBytesToRead:   #we need to also read the closing character
-            RawData = self.Read( decode=False)
+        while ReadCounter <= NumberOfBytesToRead:   # we need to also read the closing character
+            RawData = self.Read(decode=False)
             ReadCounter += len(RawData)
             if ReadCounter <= NumberOfBytesToRead:
-                file.write( RawData)
+                file.write(RawData)
             else:
-                file.write( RawData[:(NumberOfBytesToRead-ReadCounter)])
+                file.write(RawData[:(NumberOfBytesToRead-ReadCounter)])
 
         file.close()
-        
-        
-        
-    def Reset( self):
+
+
+    def Reset(self):
         """Reset on the connection, includes sending an ABORt, a *CLS
         Close and Reconnect."""
         self.Write("ABORt;*CLS")
         self.CloseSocket()
         self.Connect()
 
 
 
-    def EmptyBuffer( self):
+    def EmptyBuffer(self):
         """Empty raw socket buffer. Work around needed if program terminated during raw socket transfer."""
 
         actualtimeout = self.GetTimeout()
-        self.SetTimeout( .1)
+        self.SetTimeout(.1)
         try:
-            while self.Read( decode = False, NumberOfBytes = 1000):
+            while self.Read(decode=False, NumberOfBytes=1000):
                 pass
         except:
             pass
-        self.SetTimeout( actualtimeout)
-        
+        self.SetTimeout(actualtimeout)
+
 
-           
 if __name__ == "__main__":
     # execute only if run as a script
-    fsw=instrument('localhost', port=5026, sendcls=False)
+    fsw = instrument('localhost', port=5026, sendcls=False)
     fsw.Connect()
     fsw.Query('*IDN?')
     fsw.Close()
-    #pass   
+    # pass
```

### Comparing `rskfd-0.5.0/rskfd/remote_control/instrumentRS.py` & `rskfd-0.5.1/rskfd/remote_control/instrumentRS.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/remote_control/instrumentRSExceptions.py` & `rskfd-0.5.1/rskfd/remote_control/instrumentRSExceptions.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/remote_control/instrumentRS_FSW.py` & `rskfd-0.5.1/rskfd/remote_control/instrumentRS_FSW.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/remote_control/instrumentRS_VSE.py` & `rskfd-0.5.1/rskfd/remote_control/instrumentRS_VSE.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/signal_generation/signal_generation.py` & `rskfd-0.5.1/rskfd/signal_generation/signal_generation.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd/snp_handling/snpfiles.py` & `rskfd-0.5.1/rskfd/snp_handling/snpfiles.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/rskfd.egg-info/PKG-INFO` & `rskfd-0.5.1/rskfd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.5.0/rskfd.egg-info/SOURCES.txt` & `rskfd-0.5.1/rskfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.5.0/setup.py` & `rskfd-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   long_description = filein.read()
 
 setuptools.setup(
   name = 'rskfd',
   #packages = ['rskfd','rskfd.remote_control','rskfd.iq_data_handling','rskfd.signal_generation','rskfd.helper'],
   #packages = setuptools.find_packages(),
   packages = setuptools.find_namespace_packages(),
-  version = '0.5.0',
+  version = '0.5.1',
   license='MIT',
   description = 'Python Package for Instrument Control and Data Handling',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = 'Florian Ramian', 
   author_email = 'gitlab@ramian.eu',
   url = 'https://gitlab.com/ramian/rskfd',   # gitlab
```

