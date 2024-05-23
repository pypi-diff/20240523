# Comparing `tmp/scp-0.8.0.tar.gz` & `tmp/scp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scp-0.8.0.tar", last modified: Mon Apr 14 13:24:56 2014, max compression
+gzip compressed data, was "dist/scp-0.9.0.tar", last modified: Wed Mar  4 21:42:34 2015, max compression
```

## Comparing `scp-0.8.0.tar` & `scp-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jbardin  (114393230) 1920007995        0 2014-04-14 13:24:55.000000 scp-0.8.0/
--rw-r--r--   0 jbardin  (114393230) 1920007995      727 2013-04-08 14:46:22.000000 scp-0.8.0/LICENSE.txt
--rw-r--r--   0 jbardin  (114393230) 1920007995       38 2013-04-08 14:50:14.000000 scp-0.8.0/MANIFEST.in
--rw-r--r--   0 jbardin  (114393230) 1920007995      236 2014-04-14 13:24:55.000000 scp-0.8.0/PKG-INFO
--rw-r--r--   0 jbardin  (114393230) 1920007995      708 2013-11-13 19:42:19.000000 scp-0.8.0/README.md
-drwxr-xr-x   0 jbardin  (114393230) 1920007995        0 2014-04-14 13:24:55.000000 scp-0.8.0/scp.egg-info/
--rw-r--r--   0 jbardin  (114393230) 1920007995        1 2014-04-14 13:24:54.000000 scp-0.8.0/scp.egg-info/dependency_links.txt
--rw-r--r--   0 jbardin  (114393230) 1920007995      236 2014-04-14 13:24:54.000000 scp-0.8.0/scp.egg-info/PKG-INFO
--rw-r--r--   0 jbardin  (114393230) 1920007995        8 2014-04-14 13:24:54.000000 scp-0.8.0/scp.egg-info/requires.txt
--rw-r--r--   0 jbardin  (114393230) 1920007995      183 2014-04-14 13:24:55.000000 scp-0.8.0/scp.egg-info/SOURCES.txt
--rw-r--r--   0 jbardin  (114393230) 1920007995        4 2014-04-14 13:24:54.000000 scp-0.8.0/scp.egg-info/top_level.txt
--rw-r--r--   0 jbardin  (114393230) 1920007995    13990 2014-04-14 13:22:07.000000 scp-0.8.0/scp.py
--rw-r--r--   0 jbardin  (114393230) 1920007995       59 2014-04-14 13:24:55.000000 scp-0.8.0/setup.cfg
--rw-r--r--   0 jbardin  (114393230) 1920007995      398 2014-04-14 13:22:32.000000 scp-0.8.0/setup.py
+drwxr-xr-x   0 jbardin    (501) staff       (20)        0 2015-03-04 21:42:34.000000 scp-0.9.0/
+-rw-r--r--   0 jbardin    (501) staff       (20)      727 2014-04-08 17:22:58.000000 scp-0.9.0/LICENSE.txt
+-rw-r--r--   0 jbardin    (501) staff       (20)       38 2014-04-08 17:22:58.000000 scp-0.9.0/MANIFEST.in
+-rw-r--r--   0 jbardin    (501) staff       (20)      236 2015-03-04 21:42:34.000000 scp-0.9.0/PKG-INFO
+-rw-r--r--   0 jbardin    (501) staff       (20)      709 2015-03-02 16:15:35.000000 scp-0.9.0/README.md
+drwxr-xr-x   0 jbardin    (501) staff       (20)        0 2015-03-04 21:42:34.000000 scp-0.9.0/scp.egg-info/
+-rw-r--r--   0 jbardin    (501) staff       (20)        1 2015-03-04 21:42:33.000000 scp-0.9.0/scp.egg-info/dependency_links.txt
+-rw-r--r--   0 jbardin    (501) staff       (20)      236 2015-03-04 21:42:33.000000 scp-0.9.0/scp.egg-info/PKG-INFO
+-rw-r--r--   0 jbardin    (501) staff       (20)        9 2015-03-04 21:42:33.000000 scp-0.9.0/scp.egg-info/requires.txt
+-rw-r--r--   0 jbardin    (501) staff       (20)      183 2015-03-04 21:42:34.000000 scp-0.9.0/scp.egg-info/SOURCES.txt
+-rw-r--r--   0 jbardin    (501) staff       (20)        4 2015-03-04 21:42:33.000000 scp-0.9.0/scp.egg-info/top_level.txt
+-rw-r--r--   0 jbardin    (501) staff       (20)    15874 2015-03-04 15:00:22.000000 scp-0.9.0/scp.py
+-rw-r--r--   0 jbardin    (501) staff       (20)       59 2015-03-04 21:42:34.000000 scp-0.9.0/setup.cfg
+-rw-r--r--   0 jbardin    (501) staff       (20)      398 2015-03-04 14:52:16.000000 scp-0.9.0/setup.py
```

### Comparing `scp-0.8.0/LICENSE.txt` & `scp-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scp-0.8.0/README.md` & `scp-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 
 # SCPCLient takes a paramiko transport as its only argument
 scp = SCPClient(ssh.get_transport())
 
 scp.put('test.txt', 'test2.txt')
 scp.get('test2.txt')
 ```
-    $ md5sum test.xt test2.txt
+    $ md5sum test.txt test2.txt
     fc264c65fb17b7db5237cf7ce1780769 test.txt
     fc264c65fb17b7db5237cf7ce1780769 test2.txt
```

### Comparing `scp-0.8.0/scp.py` & `scp-0.9.0/scp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,76 @@
 # scp.py
 # Copyright (C) 2008 James Bardin <j.bardin@gmail.com>
 
 """
 Utilities for sending files over ssh using the scp1 protocol.
 """
 
+__version__ = '0.9.0'
+
+import locale
 import os
 import re
 from socket import timeout as SocketTimeout
 
-DEBUG = False
 
 # this is quote from the shlex module, added in py3.3
-_find_unsafe = re.compile(r'[^\w@%+=:,./~-]').search
+_find_unsafe = re.compile(br'[^\w@%+=:,./~-]').search
 
 
 def _sh_quote(s):
-    """Return a shell-escaped version of the string *s*."""
+    """Return a shell-escaped version of the string `s`."""
     if not s:
-        return ""
+        return b""
     if _find_unsafe(s) is None:
         return s
 
     # use single quotes, and put single quotes into double quotes
     # the string $'b is then quoted as '$'"'"'b'
-    return "'" + s.replace("'", "'\"'\"'") + "'"
+    return b"'" + s.replace(b"'", b"'\"'\"'") + b"'"
+
+
+# Unicode conversion functions; assume UTF-8
+
+def asbytes(s):
+    """Turns unicode into bytes, if needed.
+
+    Assumes UTF-8.
+    """
+    if isinstance(s, bytes):
+        return s
+    else:
+        return s.encode('utf-8')
+
+
+def asunicode(s):
+    """Turns bytes into unicode, if needed.
+
+    Uses UTF-8.
+    """
+    if isinstance(s, bytes):
+        return s.decode('utf-8', 'replace')
+    else:
+        return s
+
+
+# os.path.sep is unicode on Python 3, no matter the platform
+bytes_sep = asbytes(os.path.sep)
+
+
+# Unicode conversion function for Windows
+# Used to convert local paths if the local machine is Windows
+
+def asunicode_win(s):
+    """Turns bytes into unicode, if needed.
+    """
+    if isinstance(s, bytes):
+        return s.decode(locale.getpreferredencoding())
+    else:
+        return s
 
 
 class SCPClient(object):
     """
     An scp1 implementation, compatible with openssh scp.
     Raises SCPException for all transport related errors. Local filesystem
     and OS errors pass through.
@@ -60,21 +102,21 @@
         """
         self.transport = transport
         self.buff_size = buff_size
         self.socket_timeout = socket_timeout
         self.channel = None
         self.preserve_times = False
         self._progress = progress
-        self._recv_dir = ''
+        self._recv_dir = b''
         self._rename = False
         self._utime = None
         self.sanitize = sanitize
         self._dirtimes = {}
 
-    def put(self, files, remote_path='.',
+    def put(self, files, remote_path=b'.',
             recursive=False, preserve_times=False):
         """
         Transfer files to remote host.
 
         @param files: A single path, or a list of paths to be transfered.
             recursive must be True to transfer directories.
         @type files: string OR list of strings
@@ -85,17 +127,19 @@
         @type recursive: bool
         @param preserve_times: preserve mtime and atime of transfered files
             and directories.
         @type preserve_times: bool
         """
         self.preserve_times = preserve_times
         self.channel = self.transport.open_session()
+        self._pushed = 0
         self.channel.settimeout(self.socket_timeout)
-        scp_command = ('scp -t %s', 'scp -r -t %s')[recursive]
-        self.channel.exec_command(scp_command % self.sanitize(remote_path))
+        scp_command = (b'scp -t ', b'scp -r -t ')[recursive]
+        self.channel.exec_command(scp_command +
+                                  self.sanitize(asbytes(remote_path)))
         self._recv_confirm()
 
         if not isinstance(files, (list, tuple)):
             files = [files]
 
         if recursive:
             self._send_recursive(files)
@@ -120,57 +164,64 @@
         @type recursive: bool
         @param preserve_times: preserve mtime and atime of transfered files
             and directories.
         @type preserve_times: bool
         """
         if not isinstance(remote_path, (list, tuple)):
             remote_path = [remote_path]
-        remote_path = [self.sanitize(r) for r in remote_path]
+        remote_path = [self.sanitize(asbytes(r)) for r in remote_path]
         self._recv_dir = local_path or os.getcwd()
-        self._rename = len(remote_path) == 1 and not os.path.isdir(local_path)
+        self._rename = (len(remote_path) == 1 and
+                        not os.path.isdir(os.path.abspath(local_path)))
         if len(remote_path) > 1:
             if not os.path.exists(self._recv_dir):
-                msg = "Local path '%s' does not exist" % self._recv_dir
-                raise SCPException(msg)
+                raise SCPException("Local path '%s' does not exist" %
+                                   asunicode(self._recv_dir))
             elif not os.path.isdir(self._recv_dir):
-                msg = "Local path '%s' is not a directory" % self._recv_dir
-                raise SCPException(msg)
-        rcsv = ('', ' -r')[recursive]
-        prsv = ('', ' -p')[preserve_times]
+                raise SCPException("Local path '%s' is not a directory" %
+                                   asunicode(self._recv_dir))
+        rcsv = (b'', b' -r')[recursive]
+        prsv = (b'', b' -p')[preserve_times]
         self.channel = self.transport.open_session()
+        self._pushed = 0
         self.channel.settimeout(self.socket_timeout)
-        self.channel.exec_command("scp%s%s -f %s" % (rcsv, prsv,
-                                                     ' '.join(remote_path)))
+        self.channel.exec_command(b"scp" +
+                                  rcsv +
+                                  prsv +
+                                  b" -f " +
+                                  b' '.join(remote_path))
         self._recv_all()
 
         if self.channel:
             self.channel.close()
 
     def _read_stats(self, name):
         """return just the file stats needed for scp"""
+        if os.name == 'nt':
+            name = asunicode(name)
         stats = os.stat(name)
         mode = oct(stats.st_mode)[-4:]
         size = stats.st_size
         atime = int(stats.st_atime)
         mtime = int(stats.st_mtime)
         return (mode, size, mtime, atime)
 
     def _send_files(self, files):
         for name in files:
-            basename = os.path.basename(name)
+            basename = asbytes(os.path.basename(name))
             (mode, size, mtime, atime) = self._read_stats(name)
             if self.preserve_times:
                 self._send_time(mtime, atime)
             file_hdl = open(name, 'rb')
 
             # The protocol can't handle \n in the filename.
             # Quote them as the control sequence \^J for now,
             # which is how openssh handles it.
-            self.channel.sendall("C%s %d %s\n" %
-                                 (mode, size, basename.replace('\n', '\\^J')))
+            self.channel.sendall(("C%s %d " % (mode, size)).encode('ascii') +
+                                 basename.replace(b'\n', b'\\^J') + b"\n")
             self._recv_confirm()
             file_pos = 0
             if self._progress:
                 if size == 0:
                     # avoid divide-by-zero
                     self._progress(basename, 1, 1)
                 else:
@@ -189,128 +240,138 @@
     def _chdir(self, from_dir, to_dir):
         # Pop until we're one level up from our next push.
         # Push *once* into to_dir.
         # This is dependent on the depth-first traversal from os.walk
 
         # add path.sep to each when checking the prefix, so we can use
         # path.dirname after
-        common = os.path.commonprefix([from_dir + os.path.sep,
-                                       to_dir + os.path.sep])
+        common = os.path.commonprefix([from_dir + bytes_sep,
+                                       to_dir + bytes_sep])
         # now take the dirname, since commonprefix is character based,
         # and we either have a seperator, or a partial name
         common = os.path.dirname(common)
-        cur_dir = from_dir.rstrip(os.path.sep)
+        cur_dir = from_dir.rstrip(bytes_sep)
         while cur_dir != common:
             cur_dir = os.path.split(cur_dir)[0]
             self._send_popd()
         # now we're in our common base directory, so on
         self._send_pushd(to_dir)
 
     def _send_recursive(self, files):
         for base in files:
             if not os.path.isdir(base):
                 # filename mixed into the bunch
                 self._send_files([base])
                 continue
-            last_dir = base
+            last_dir = asbytes(base)
             for root, dirs, fls in os.walk(base):
-                self._chdir(last_dir, root)
+                self._chdir(last_dir, asbytes(root))
                 self._send_files([os.path.join(root, f) for f in fls])
-                last_dir = root
+                last_dir = asbytes(root)
             # back out of the directory
-            for i in range(len(os.path.split(last_dir))):
+            while self._pushed > 0:
                 self._send_popd()
 
     def _send_pushd(self, directory):
         (mode, size, mtime, atime) = self._read_stats(directory)
-        basename = os.path.basename(directory)
+        basename = asbytes(os.path.basename(directory))
         if self.preserve_times:
             self._send_time(mtime, atime)
-        self.channel.sendall('D%s 0 %s\n' %
-                             (mode, basename.replace('\n', '\\^J')))
+        self.channel.sendall(('D%s 0 ' % mode).encode('ascii') +
+                             basename.replace(b'\n', b'\\^J') + b'\n')
         self._recv_confirm()
+        self._pushed += 1
 
     def _send_popd(self):
         self.channel.sendall('E\n')
         self._recv_confirm()
+        self._pushed -= 1
 
     def _send_time(self, mtime, atime):
-        self.channel.sendall('T%d 0 %d 0\n' % (mtime, atime))
+        self.channel.sendall(('T%d 0 %d 0\n' % (mtime, atime)).encode('ascii'))
         self._recv_confirm()
 
     def _recv_confirm(self):
         # read scp response
-        msg = ''
+        msg = b''
         try:
             msg = self.channel.recv(512)
         except SocketTimeout:
             raise SCPException('Timout waiting for scp response')
         # slice off the first byte, so this compare will work in python2 and python3
         if msg and msg[0:1] == b'\x00':
             return
         elif msg and msg[0:1] == b'\x01':
-            raise SCPException(msg[1:])
+            raise SCPException(asunicode(msg[1:]))
         elif self.channel.recv_stderr_ready():
             msg = self.channel.recv_stderr(512)
-            raise SCPException(msg)
+            raise SCPException(asunicode(msg))
         elif not msg:
             raise SCPException('No response from server')
         else:
             raise SCPException('Invalid response from server', msg)
 
     def _recv_all(self):
-        # loop over scp commands, and recive as necessary
+        # loop over scp commands, and receive as necessary
         command = {b'C': self._recv_file,
                    b'T': self._set_time,
                    b'D': self._recv_pushd,
                    b'E': self._recv_popd}
         while not self.channel.closed:
             # wait for command as long as we're open
             self.channel.sendall('\x00')
             msg = self.channel.recv(1024)
             if not msg:  # chan closed while recving
                 break
+            assert msg[-1:] == b'\n'
+            msg = msg[:-1]
             code = msg[0:1]
             try:
                 command[code](msg[1:])
             except KeyError:
-                raise SCPException(str(msg).strip())
+                raise SCPException(asunicode(msg[1:]))
         # directory times can't be set until we're done writing files
         self._set_dirtimes()
 
     def _set_time(self, cmd):
         try:
-            times = cmd.split()
+            times = cmd.split(b' ')
             mtime = int(times[0])
             atime = int(times[2]) or mtime
         except:
             self.channel.send(b'\x01')
             raise SCPException('Bad time format')
         # save for later
         self._utime = (atime, mtime)
 
     def _recv_file(self, cmd):
         chan = self.channel
-        parts = cmd.strip().split(' ', 2)
+        parts = cmd.strip().split(b' ', 2)
+
         try:
             mode = int(parts[0], 8)
             size = int(parts[1])
-            path = os.path.join(self._recv_dir, parts[2])
             if self._rename:
                 path = self._recv_dir
                 self._rename = False
+            elif os.name == 'nt':
+                path = os.path.join(asunicode_win(self._recv_dir),
+                                    parts[2].decode('utf-8'))
+            else:
+                path = os.path.join(asbytes(self._recv_dir),
+                                    parts[2])
         except:
             chan.send('\x01')
             chan.close()
             raise SCPException('Bad file format')
 
         try:
             file_hdl = open(path, 'wb')
         except IOError as e:
-            chan.send(b'\x01' + str(e).encode())
+            chan.send(b'\x01' + str(e).encode('utf-8'))
             chan.close()
             raise
 
         if self._progress:
             if size == 0:
                 # avoid divide-by-zero
                 self._progress(path, 1, 1)
@@ -327,15 +388,15 @@
                 file_hdl.write(chan.recv(buff_size))
                 pos = file_hdl.tell()
                 if self._progress:
                     self._progress(path, size, pos)
 
             msg = chan.recv(512)
             if msg and msg[0:1] != b'\x00':
-                raise SCPException(msg[1:])
+                raise SCPException(asunicode(msg[1:]))
         except SocketTimeout:
             chan.close()
             raise SCPException('Error receiving, socket.timeout')
 
         file_hdl.truncate()
         try:
             os.utime(path, self._utime)
@@ -343,36 +404,41 @@
             os.chmod(path, mode)
             # should we notify the other end?
         finally:
             file_hdl.close()
         # '\x00' confirmation sent in _recv_all
 
     def _recv_pushd(self, cmd):
-        parts = cmd.split()
+        parts = cmd.split(b' ', 2)
         try:
             mode = int(parts[0], 8)
-            path = os.path.join(self._recv_dir, parts[2])
             if self._rename:
                 path = self._recv_dir
                 self._rename = False
+            elif os.name == 'nt':
+                path = os.path.join(asunicode_win(self._recv_dir),
+                                    parts[2].decode('utf-8'))
+            else:
+                path = os.path.join(asbytes(self._recv_dir),
+                                    parts[2])
         except:
             self.channel.send(b'\x01')
             raise SCPException('Bad directory format')
         try:
             if not os.path.exists(path):
                 os.mkdir(path, mode)
             elif os.path.isdir(path):
                 os.chmod(path, mode)
             else:
                 raise SCPException('%s: Not a directory' % path)
             self._dirtimes[path] = (self._utime)
             self._utime = None
             self._recv_dir = path
         except (OSError, SCPException) as e:
-            self.channel.send(b'\x01' + str(e).encode())
+            self.channel.send(b'\x01' + asbytes(str(e)))
             raise
 
     def _recv_popd(self, *cmd):
         self._recv_dir = os.path.split(self._recv_dir)[0]
 
     def _set_dirtimes(self):
         try:
```

