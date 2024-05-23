# Comparing `tmp/python_115-0.0.7.4.tar.gz` & `tmp/python_115-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.7.4.tar", max compression
+gzip compressed data, was "python_115-0.0.8.tar", max compression
```

## Comparing `python_115-0.0.7.4.tar` & `python_115-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7.4/LICENSE
--rwxr-xr-x   0        0        0   289028 2024-04-29 10:57:10.671290 python_115-0.0.7.4/p115/__init__.py
--rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7.4/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7.4/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.4/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.4/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7.4/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8608 2024-04-29 10:59:39.380074 python_115-0.0.7.4/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7.4/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.4/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.4/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.4/p115/cmd/webdav_share.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7.4/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7.4/p115/py.typed
--rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7.4/p115/tool/__init__.py
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7.4/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7.4/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7.4/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7.4/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7.4/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7.4/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7.4/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7.4/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7.4/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7.4/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7.4/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7.4/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7.4/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7.4/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7.4/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7.4/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7.4/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-29 10:59:50.062321 python_115-0.0.7.4/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7.4/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.7.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   241057 2024-05-23 10:53:22.107922 python_115-0.0.8/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56834 2024-05-22 18:10:09.814988 python_115-0.0.8/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48067 2024-05-22 14:42:11.490047 python_115-0.0.8/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12216 2024-05-22 18:05:34.938601 python_115-0.0.8/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8/p115/component/offline.py
+-rwxr-xr-x   0        0        0     3877 2024-05-22 14:04:09.272894 python_115-0.0.8/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     4950 2024-05-22 14:04:19.641910 python_115-0.0.8/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8/p115/py.typed
+-rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1591 2024-05-23 14:39:19.584144 python_115-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8/readme.md
+-rw-r--r--   0        0        0    36270 1970-01-01 00:00:00.000000 python_115-0.0.8/PKG-INFO
```

### Comparing `python_115-0.0.7.4/LICENSE` & `python_115-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.4/p115/cmd/iterdir.py` & `python_115-0.0.8/p115/cmd/iterdir.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,27 +28,27 @@
         print(".".join(map(str, __version__)))
         raise SystemExit(0)
 
     from os.path import expanduser, dirname, join as joinpath
     from sys import stdout
     from typing import Callable
 
-    cookie = args.cookie
-    if not cookie:
+    cookies = args.cookies
+    if not cookies:
         for dir_ in (".", expanduser("~"), dirname(__file__)):
             try:
-                cookie = open(joinpath(dir_, "115-cookie.txt")).read()
-                if cookie:
+                cookies = open(joinpath(dir_, "115-cookies.txt")).read()
+                if cookies:
                     break
             except FileNotFoundError:
                 pass
 
-    fs = P115FileSystem.login(cookie)
-    if fs.client.cookie != cookie:
-        open("115-cookie.txt", "w").write(fs.client.cookie)
+    fs = P115FileSystem.login(cookies)
+    if fs.client.cookies != cookies:
+        open("115-cookies.txt", "w").write(fs.client.cookies)
 
     if args.password and not fs.hidden_mode:
         fs.hidden_switch(True, password=args.password)
 
     keys = args.keys or KEYS
     output_type = args.output_type
 
@@ -199,30 +199,30 @@
         from sys import stderr
         stderr.close()
     finally:
         file.close()
 
 
 parser.add_argument("path", nargs="?", default="0", help="文件夹路径或 id，默认值 0，即根目录")
-parser.add_argument("-c", "--cookie", help="115 登录 cookie，如果缺失，则从 115-cookie.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
+parser.add_argument("-c", "--cookies", help="115 登录 cookie，如果缺失，则从 115-cookies.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
 parser.add_argument("-p", "--password", help="密码，用于进入隐藏模式，罗列隐藏文件")
+parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 p115.P115Path），用于对路径进行筛选")
 parser.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
+parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
+输出类型，默认为 log
+    - log   每行输出一条数据，每条数据输出为一个 json 的 object
+    - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
+    - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据""")
 parser.add_argument("-d", "--dump", default="", help="""\
-(优先级高于 -k/--keys 和 -t/--output-type) 提供一段代码，每次调用，用于输出。
+(优先级高于 -k/--keys 和 -t/--output-type) 提供一段代码，每次调用，再行输出，尾部会添加一个 b'\n'。
 如果结果 result 是
     - None，跳过
     - bytes，输出
     - 其它，先调用 `bytes(str(result), 'utf-8')`，再输出""")
 parser.add_argument("-de", "--dump-exec", action="store_true", help="对 dump 代码进行 exec 解析（必须生成一个变量 dump，用于调用），否则用 eval 解析（会注入一个变量 path，类型是 p115.P115Path）")
-parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 p115.P115Path），用于对路径进行筛选")
-parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
-输出类型，默认为 log
-    - log   每行输出一条数据，每条数据输出为一个 json 的 object
-    - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
-    - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据""")
 parser.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
 parser.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于或等于 0 时不限")
 parser.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
 parser.add_argument("-dfs", "--depth-first", action="store_true", help="使用深度优先搜索，否则使用广度优先")
 parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
 parser.set_defaults(func=main)
```

### Comparing `python_115-0.0.7.4/p115/cmd/qrcode.py` & `python_115-0.0.8/p115/cmd/qrcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__: list[str] = []
-__doc__ = "扫码获取 115 cookie"
+__doc__ = "扫码获取 115 cookies"
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
 
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
@@ -28,31 +28,31 @@
     outfile = args.output_file
     file: TextIO
     if outfile:
         file = open(outfile, "w")
     else:
         from sys import stdout as file
 
-    cookie: str
-    if args.cookie:
+    cookies: str
+    if args.cookies:
         from p115.tool import login_scan_cookie
 
-        client = P115Client(args.cookie)
-        cookie = login_scan_cookie(client, app=args.app)
+        client = P115Client(args.cookies)
+        cookies = login_scan_cookie(client, app=args.app)
     else:
-        client = P115Client(login_app=args.app)
-        cookie = client.cookie
+        client = P115Client(app=args.app)
+        cookies = client.cookies
     print()
-    print(cookie, file=file)
+    print(cookies, file=file)
 
 
 parser.add_argument("app", nargs="?", choices=("web", "android", "ios", "linux", "mac", "windows", "tv", "alipaymini", "wechatmini", "qandroid"), default="web", 
                     help="选择一个 app 进行登录，注意：这会把已经登录的相同 app 踢下线")
 parser.add_argument("-o", "--output-file", help="保存到文件，未指定时输出到 stdout")
-parser.add_argument("-c", "--cookie", help="115 登录 cookie，如果提供了，就可以用这个 cookie 进行自动扫码，否则需要你用手机来手动扫码")
+parser.add_argument("-c", "--cookies", help="115 登录 cookie，如果提供了，就可以用这个 cookies 进行自动扫码，否则需要你用手机来手动扫码")
 parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
 parser.set_defaults(func=main)
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     main(args)
```

### Comparing `python_115-0.0.7.4/p115/tool/__init__.py` & `python_115-0.0.8/p115/tool/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     uid = client.login_qrcode_token()["data"]["uid"]
     client.login_qrcode_scan(uid)
     client.login_qrcode_scan_confirm(uid)
     data = client.login_qrcode_result({"account": uid, "app": app})
     return "; ".join(f"{k}={v}" for k, v in data["data"]["cookie"].items())
 
 
+# TODO: 多线程下载图片，以加速破解
 def crack_captcha(
     client: str | P115Client, 
     sample_count: int = 16, 
     crack: None | Callable[[bytes], str] = None, 
 ) -> bool:
     """破解 115 的图片验证码。如果返回 True，则说明破解成功，否则失败。如果失败，就不妨多运行这个函数几次。
 
@@ -65,30 +66,30 @@
         except NameError:
             try:
                 # https://pypi.org/project/ddddocr/
                 from ddddocr import DdddOcr
             except ImportError:
                 from subprocess import run
                 from sys import executable
-                run([executable, "-m", "pip", "install", "-U", "ddddocr"], check=True)
+                run([executable, "-m", "pip", "install", "-U", "ddddocr==1.4.11"], check=True)
                 from ddddocr import DdddOcr # type: ignore
             crack = CAPTCHA_CRACK = cast(Callable[[bytes], str], DdddOcr(show_ad=False).classification)
     if isinstance(client, str):
         client = P115Client(client)
     while True:
         captcha = crack(client.captcha_code())
-        if len(captcha) == 4:
+        if len(captcha) == 4 and all("\u4E00" <= char <= "\u9FFF" for char in captcha):
             break
     l: list[str] = []
     for i in range(10):
         d: dict[str, int] = {}
         for _ in range(sample_count):
             while True:
                 char = crack(client.captcha_single(i))
-                if len(char) == 1:
+                if len(char) == 1 and "\u4E00" <= char <= "\u9FFF":
                     break
             try:
                 d[char] += 1
             except KeyError:
                 d[char] = 1
         l.append(max(d, key=lambda k: d[k]))
     try:
```

### Comparing `python_115-0.0.7.4/p115/util/cipher.py` & `python_115-0.0.8/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.4/p115/util/path.py` & `python_115-0.0.8/p115/component/recyclebin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,187 +1,136 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = [
-    "escape", "unescape", "joins", "splits", "normpath", "normpatht", 
-    "split", "join", "basename", "dirname", "commonpath", "commonpatht", 
-]
-
-from re import compile as re_compile, Match
-from typing import cast, Iterable, Sequence
-
-
-CRE_PART_match = re_compile(r"[^\\/]*(?:\\(?s:.)[^\\/]*)*/").match
-CRE_PART = re_compile(r"[^\\/]*(?:\\(?s:.)[^\\/]*)*$")
-
-
-def escape(name: str, /) -> str:
-    return "\\" + name if name in (".", "..") else name.replace("\\", r"\\").replace("/", r"\/")
-
-
-def unescape(name: str, /) -> str:
-    if name.startswith(r"\."):
-        name = name[1:]
-    return name.replace(r"\/", "/").replace(r"\\", "\\")
-
-
-def joins(patht: Sequence[str], parents: int = 0, /) -> str:
-    assert parents >= 0
-    if not patht:
-        if parents:
-            return "/".join(("..",) * parents)
-        return ""
-    path = "/".join(escape(p) for p in patht if p)
-    if not patht[0]:
-        path = "/" + path
-    elif parents:
-        path = "".join(("../",) * parents) + path
-    return path
-
-
-def splits(
-    path: str, 
-    /, 
-    parse_dots: bool = True, 
-    do_unescape: bool = True, 
-) -> tuple[list[str], int]:
-    parts: list[str] = []
-    add_part = parts.append
-    if path.startswith("/"):
-        add_part("")
-        l = 1
-        is_absolute = True
-    else:
-        l = 0
-        is_absolute = False
-    parents = 0
-    while (m := CRE_PART_match(path, l)):
-        p = m[0][:-1]
-        if p:
-            if p == "." and parse_dots:
-                pass
-            elif p == ".." and parse_dots:
-                if is_absolute:
-                    if len(parts) > 1:
-                        parts.pop()
-                elif parts:
-                    parts.pop()
-                else:
-                    parents += 1
-            elif do_unescape:
-                add_part(unescape(p))
-            else:
-                add_part(p)
-        l = m.end()
-    if l < len(path):
-        p = path[l:]
-        if p:
-            if p == "." and parse_dots:
-                pass
-            elif p == ".." and parse_dots:
-                if is_absolute:
-                    if len(parts) > 1:
-                        parts.pop()
-                elif parts:
-                    parts.pop()
-                else:
-                    parents += 1
-            elif do_unescape:
-                add_part(unescape(p))
-            else:
-                add_part(p)
-    return parts, parents
-
-
-def normpath(path: str, /) -> str:
-    return joins(*splits(path))
-
-
-def normpatht(patht: Sequence[str], /) -> list[str]:
-    return [patht[0], *filter(None, patht)]
-
-
-def split(path: str, /) -> tuple[str, str]:
-    stop = len(path)
-    if stop <= 1:
-        if path == "/":
-            return "/", ""
-        return "", path
-    parents = 0
-    while True:
-        match = cast(Match, CRE_PART.search(path, 0, stop))
-        idx = match.start()
-        value = path[idx:stop]
-        if value in ("", "."):
-            pass
-        elif value == "..":
-            parents += 1
-        elif parents:
-            parents -= 1
+__all__ = ["P115Recyclebin"]
+
+from collections.abc import Iterable, Iterator
+
+from .client import check_response, P115Client
+
+
+class P115Recyclebin:
+    __slots__ = ("client", "password")
+
+    def __init__(
+        self, 
+        client: str | P115Client, 
+        /, 
+        password: int | str = "", 
+    ):
+        if isinstance(client, str):
+            client = P115Client(client)
+        self.client = client
+        self.password = password
+
+    def __contains__(self, id: int | str, /) -> bool:
+        ids = str(id)
+        return any(item["id"] == ids for item in self)
+
+    def __delitem__(self, id: int | str, /):
+        return self.remove(id)
+
+    def __getitem__(self, id: int | str, /) -> dict:
+        ids = str(id)
+        for item in self:
+            if item["id"] == ids:
+                return item
+        raise LookupError(f"no such id: {id!r}")
+
+    def __iter__(self, /) -> Iterator[dict]:
+        return self.iter()
+
+    def __len__(self, /) -> int:
+        return int(check_response(self.client.recyclebin_list({"limit": 1}))["count"])
+
+    def __repr__(self, /) -> str:
+        cls = type(self)
+        module = cls.__module__
+        name = cls.__qualname__
+        if module != "__main__":
+            name = module + "." + name
+        return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
+
+    @check_response
+    def clear(
+        self, 
+        /, 
+        password: None | int | str = None, 
+    ) -> dict:
+        if password is None:
+            password = self.password
+        return self.client.recyclebin_clean({"password": password})
+
+    def get(
+        self, 
+        id: int | str, 
+        /, 
+        default=None, 
+    ):
+        ids = str(id)
+        return next((item for item in self if item["id"] == ids), default)
+
+    def iter(
+        self, 
+        /, 
+        offset: int = 0, 
+        page_size: int = 1 << 10, 
+    ) -> Iterator[dict]:
+        if offset < 0:
+            offset = 0
+        if page_size <= 0:
+            page_size = 1 << 10
+        payload = {"offset": offset, "limit": page_size}
+        count = 0
+        while True:
+            resp = check_response(self.client.recyclebin_list(payload))
+            if resp["offset"] != payload["offset"]:
+                return
+            if count == 0:
+                count = int(resp["count"])
+            elif count != int(resp["count"]):
+                raise RuntimeError("detected count changes during iteration")
+            yield from resp["data"]
+            if len(resp["data"]) < resp["page_size"]:
+                return
+            payload["offset"] += resp["page_size"]
+
+    def list(
+        self, 
+        /, 
+        offset: int = 0, 
+        limit: int = 0, 
+    ) -> list[dict]:
+        if limit <= 0:
+            return list(self.iter(offset))
+        resp = check_response(self.client.recyclebin_list({"offset": offset, "limit": limit}))
+        if resp["offset"] != offset:
+            return []
+        return resp["data"]
+
+    @check_response
+    def remove(
+        self, 
+        ids: int | str | Iterable[int | str], 
+        /, 
+        password: None | int | str = None, 
+    ) -> dict:
+        if isinstance(ids, (int, str)):
+            payload = {"rid[0]": ids}
+        else:
+            payload = {f"rid[{i}]": id for i, id in enumerate(ids)}
+        payload["password"] = self.password if password is None else password
+        return self.client.recyclebin_clean(payload)
+
+    @check_response
+    def revert(
+        self, 
+        ids: int | str | Iterable[int | str], 
+        /, 
+    ) -> dict:
+        if isinstance(ids, (int, str)):
+            payload = {"rid[0]": ids}
         else:
-            value = unescape(value)
-            if idx == 0:
-                return "", value
-            elif idx == 1:
-                return path[:idx], value
-            else:
-                return path[:idx-1], value
-        if idx == 0:
-            if path.startswith("/"):
-                return "/", ""
-            else:
-                return "", ""
-        stop = idx - 1
-
-
-def join(path: str, /, *parts: str) -> str:
-    if not parts:
-        return path
-    return "/".join((path, *map(escape, parts)))
-
-
-def basename(path: str, /) -> str:
-    return split(path)[1]
-
-
-def dirname(path: str, /) -> str:
-    return split(path)[0]
-
-
-def commonpath(pathit: Iterable[str], /) -> str:
-    ls = tuple(map(splits, pathit))
-    if not ls:
-        return ""
-    m = min(t[1] for t in ls)
-    M = max(t[1] for t in ls)
-    if m:
-        prefix = "/".join(("..",) * m)
-    else:
-        prefix = ""
-    if m != M:
-        return prefix
-    cm = commonpatht((t[0] for t in ls))
-    if not cm:
-        return prefix
-    path = joins(cm)
-    if prefix:
-        path = prefix + "/" + path
-    return path
-
-
-def commonpatht(pathtit: Iterable[Sequence[str]], /) -> list[str]:
-    ls = []
-    for n1, n2 in zip(*pathtit):
-        if n1 != n2:
-            break
-        ls.append(n1)
-    return ls
-
-# TODO
-# commonprefix
-# splitext
-# samefile
-# sameopenfile
-# samestat
-# stat
-# 另外参考 posixpath
+            payload = {f"rid[{i}]": id for i, id in enumerate(ids)}
+        return self.client.recyclebin_revert(payload)
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python_115-0.0.7.4/readme.md` & `python_115-0.0.8/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.4/PKG-INFO` & `python_115-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.7.4
+Version: 0.0.8
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
-Keywords: nas,115
+Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,22 +16,34 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: aiohttp
 Requires-Dist: cachetools
 Requires-Dist: ecdsa
+Requires-Dist: http_response
+Requires-Dist: httpx
+Requires-Dist: httpx_request
 Requires-Dist: lz4
 Requires-Dist: magnet2torrent
+Requires-Dist: multidict
+Requires-Dist: posixpatht
 Requires-Dist: pycryptodome
+Requires-Dist: python-asynctools
+Requires-Dist: python-cookietools
+Requires-Dist: python-filewrap
+Requires-Dist: python-hashtools
+Requires-Dist: python-http_request
+Requires-Dist: python-httpfile
+Requires-Dist: python-iterutils
+Requires-Dist: python-startfile
+Requires-Dist: python-urlopen
 Requires-Dist: qrcode
-Requires-Dist: requests
 Requires-Dist: yarl
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 Description-Content-Type: text/markdown
 
 # 115 网盘 Web API 的 Python 封装
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-115)
```

