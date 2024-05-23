# Comparing `tmp/fuckbookwalker-0.1.1.tar.gz` & `tmp/fuckbookwalker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuckbookwalker-0.1.1.tar", max compression
+gzip compressed data, was "fuckbookwalker-0.1.3.tar", max compression
```

## Comparing `fuckbookwalker-0.1.1.tar` & `fuckbookwalker-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1061 2024-02-29 14:53:21.586404 fuckbookwalker-0.1.1/LICENSE
--rw-r--r--   0        0        0      860 2024-05-07 13:12:12.574987 fuckbookwalker-0.1.1/README.md
--rw-r--r--   0        0        0       25 2024-02-29 15:59:49.809023 fuckbookwalker-0.1.1/bookphucker/__init__.py
--rw-r--r--   0        0        0     4843 2024-05-07 13:27:40.743925 fuckbookwalker-0.1.1/bookphucker/__main__.py
--rw-r--r--   0        0        0      212 2024-05-07 06:45:05.569187 fuckbookwalker-0.1.1/bookphucker/commonvars.py
--rw-r--r--   0        0        0     2427 2024-05-07 12:49:52.903274 fuckbookwalker-0.1.1/bookphucker/config.py
--rw-r--r--   0        0        0       78 2024-05-07 10:10:03.986049 fuckbookwalker-0.1.1/bookphucker/exc.py
--rw-r--r--   0        0        0     7561 2024-05-07 12:49:31.202060 fuckbookwalker-0.1.1/bookphucker/jp.py
--rw-r--r--   0        0        0        0 2024-05-07 10:47:01.044614 fuckbookwalker-0.1.1/bookphucker/tw.py
--rw-r--r--   0        0        0     1680 2024-05-07 12:49:44.843728 fuckbookwalker-0.1.1/bookphucker/utils.py
--rw-r--r--   0        0        0     3643 2024-05-07 13:14:40.571801 fuckbookwalker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 fuckbookwalker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-29 14:53:21.586404 fuckbookwalker-0.1.3/LICENSE
+-rw-r--r--   0        0        0      884 2024-05-07 19:14:18.021998 fuckbookwalker-0.1.3/README.md
+-rw-r--r--   0        0        0       25 2024-02-29 15:59:49.809023 fuckbookwalker-0.1.3/bookphucker/__init__.py
+-rw-r--r--   0        0        0     5974 2024-05-23 08:57:34.791639 fuckbookwalker-0.1.3/bookphucker/__main__.py
+-rw-r--r--   0        0        0       47 2024-05-07 13:34:05.688660 fuckbookwalker-0.1.3/bookphucker/cli.py
+-rw-r--r--   0        0        0      212 2024-05-07 06:45:05.569187 fuckbookwalker-0.1.3/bookphucker/commonvars.py
+-rw-r--r--   0        0        0     2428 2024-05-07 17:58:26.734236 fuckbookwalker-0.1.3/bookphucker/config.py
+-rw-r--r--   0        0        0       78 2024-05-07 10:10:03.986049 fuckbookwalker-0.1.3/bookphucker/exc.py
+-rw-r--r--   0        0        0     7801 2024-05-23 08:58:02.911492 fuckbookwalker-0.1.3/bookphucker/jp.py
+-rw-r--r--   0        0        0     7326 2024-05-23 08:58:14.443431 fuckbookwalker-0.1.3/bookphucker/tw.py
+-rw-r--r--   0        0        0     1700 2024-05-23 08:58:23.259385 fuckbookwalker-0.1.3/bookphucker/utils.py
+-rw-r--r--   0        0        0     3756 2024-05-23 08:59:28.307039 fuckbookwalker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 fuckbookwalker-0.1.3/PKG-INFO
```

### Comparing `fuckbookwalker-0.1.1/LICENSE` & `fuckbookwalker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fuckbookwalker-0.1.1/README.md` & `fuckbookwalker-0.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Unpolished bookwalker.jp scraper
+# Unpolished bookwalker scraper
 
 > It just works. -- Todd Howard
 
 ## TODO List
 
 - [ ] Image `EPUB` export
 - [ ] `OCR` integration
@@ -26,14 +26,18 @@
 ```bash
 poetry run python bookphucker <url or uuid of books>
 ```
 
 You should see something like this.
 ![sample](./imgs/sample.png)
 
+### Configuration
+
+wip...
+
 By default, `bookphucker` will try to reuse previous `cookies`, using `--no-cache` to clear `cookies`.
 
 ## Common Issues
 
 ### Cannot log in
 
 You may encounter CAPTCHA during the login process.
```

### Comparing `fuckbookwalker-0.1.1/bookphucker/__main__.py` & `fuckbookwalker-0.1.3/bookphucker/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import sys
 import ujson as json
 import logging
+import requests
 from shutil import move, rmtree
 from urllib.parse import urlparse
 from getpass import getpass
 from pathlib import Path
 from contextlib import suppress
 from selenium.common.exceptions import WebDriverException
 from bookphucker import Config
@@ -13,55 +14,79 @@
 from bookphucker.commonvars import config_path, cache_path
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("book_pages", help="The page url or book uuid", nargs='+')
     parser.add_argument("-r", "--region", help="The region of the bookwalker site",
-                        default="jp", choices=["jp", "tw"])
+                        default="auto", choices=["jp", "tw", "auto"])
     parser.add_argument("--no-cache", help="Clear cache directory (cookies, etc.)",
                         action="store_true")
+    parser.add_argument("--overwrite", help="Overwrite existing files",
+                        action="store_true")
 
     args = parser.parse_args()
-    match args.region:
-        case "jp":
-            from bookphucker.jp import login, download_book, logout
-        case "tw":
-            raise NotImplementedError("TW region is not supported yet.")
-            # from bookphucker.tw import login, download_book, logout
     book_uuids = list[str]()
+    region = args.region
+
+    print(f"Book UUIDs:\n\n")
 
     for book_page in args.book_pages:
-        if book_page.startswith("http"):
+        if "bookwalker" in book_page:
+            if not book_page.startswith("http"):
+                book_page = "https://" + book_page
             book_url = urlparse(book_page)
-            book_uuid = book_url.path
+            if ".jp" in book_url.hostname:
+                if region == "auto":
+                    region = "jp"
+                book_uuid = book_url.path
+                print(f"{book_uuid}")
+            elif ".com.tw" in book_url.hostname:
+                if region == "auto":
+                    region = "tw"
+                book_id = ''
+                if book_url.path.startswith("/product/"):
+                    book_id = book_url.path.removeprefix("/product/").split("/")[0]
+                    r = requests.head(
+                        f"https://www.bookwalker.com.tw/browserViewer/{book_id}/trial")
+                    book_url = urlparse(r.headers["Location"])
+                query = book_url.query
+                book_uuid = dict([param.split("=")
+                                 for param in query.split("&")])["cid"]
+                print(f"{book_uuid}{f" ({book_id})" if book_id else ''}")
         else:
             book_uuid = book_page
         book_uuids.append(book_uuid.strip('/')[-36:])
 
-    print(f"Book UUIDs:\n{'\n'.join(book_uuids)}\n")
+    match region:
+        case "jp" | "auto":
+            from bookphucker.jp import login, download_book, logout
+        case "tw":
+            from bookphucker.tw import login, download_book, logout
 
     cfg = Config()
 
     if not config_path.exists():
         user_input = input(
             "Config file not found. Would you like to create one? (Y/n) ").strip().lower() or "y"
         if user_input == "y":
             username = input("Enter your username: ") or None
             password = getpass("Enter your password: ") or None
             cfg = Config(username=username, password=password)
-            config_path.write_text(json.dumps(cfg.model_dump(mode="json"), indent=2))
+            config_path.write_text(
+                json.dumps(cfg.model_dump(mode="json"), indent=2), encoding = "utf-8")
             print(f"Config file created at {config_path}")
     else:
         print(f"Config file found at {config_path}")
         d = json.loads(config_path.read_text())
         cfg, updated = Config.from_dict(d)
         if updated:
             move(config_path, config_path.with_suffix(".bak"))
-            config_path.write_text(json.dumps(cfg.model_dump(mode="json"), indent=2))
+            config_path.write_text(
+                json.dumps(cfg.model_dump(mode="json"), indent=2), encoding = "utf-8")
             print(f"Config file updated at {config_path}")
 
     if args.no_cache and cache_path.exists():
         rmtree(cache_path)
         cache_path.mkdir()
         print(f"Cache directory cleared at {cache_path}")
 
@@ -75,47 +100,46 @@
             cfg.password or getpass("Enter your password: "))
         max_login_retries = 1
         login_retry = 0
         manual_login = cfg.manual_login or not any([username, password])
         if manual_login and cfg.headless:
             print("Manual login required, but browser is headless.")
             user_input = input(
-                "Would you like to continue with non-headless browser? (Y/n) ").strip().lower() or "y"
+                "Would you like to stay headless? (Y/n) ").strip().lower() or "y"
             if user_input != "y":
-                return 1
-            driver.quit()
-            cfg.headless = False
-            driver = cfg.get_webdriver()
+                driver.quit()
+                cfg.headless = False
+                driver = cfg.get_webdriver()
         while True:
             try:
                 login(driver, username, password, error_on_captcha=cfg.headless)
             except RequiresCapcha:
                 print("Captcha required, but browser is headless.")
                 user_input = input(
-                    "Would you like to continue with non-headless browser? (Y/n) ").strip().lower() or "y"
+                    "Would you like to continue with non-headless browser? (y/N) ").strip().lower() or "y"
                 if user_input != "y":
                     return 2
                 driver.quit()
                 cfg.headless = False
                 driver = cfg.get_webdriver()
                 login(driver, username, password)
 
             try:
                 for book_uuid in book_uuids:
-                    download_book(driver, cfg, book_uuid)
+                    download_book(driver, cfg, book_uuid, overwrite=args.overwrite)
             except Error998:
                 login_retry += 1
                 if login_retry > max_login_retries:
                     raise
                 logging.warning("Retrying login %s/%s", login_retry, max_login_retries)
                 logout(driver)
                 continue
             break
     except Exception as e:
-        Path("error.html").write_text(driver.page_source)
+        Path("error.html").write_text(driver.page_source, encoding = "utf-8")
         Path("error.png").write_bytes(driver.get_screenshot_as_png())
         logging.error(
             "An error occurred. Please check error.html and error.png for more information.")
         raise e
     except KeyboardInterrupt:
         print("Exiting...")
     finally:
```

### Comparing `fuckbookwalker-0.1.1/bookphucker/config.py` & `fuckbookwalker-0.1.3/bookphucker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     model_config = ConfigDict(extra="allow", validate_assignment=True)
     version: str = str(CURRENT_VERSION)
     browser: Literal["chrome", "chromium"] = "chrome"
     headless: bool = True
     username: str | None = None
     password: str | None = None
     manual_login: bool = False
-    viewer_size: tuple[int, int] = (960, 1360)
+    viewer_size: tuple[int, int] = (1400, 2140)
     user_agent: str | None = None
     logging_level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO"
 
     def get_webdriver(self):
         ua = self.user_agent or "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36"
         options = uc.ChromeOptions()
         options.set_capability("unhandledPromptBehavior", "accept")
```

### Comparing `fuckbookwalker-0.1.1/bookphucker/jp.py` & `fuckbookwalker-0.1.3/bookphucker/jp.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 domain = "bookwalker.jp"
 
 
 def validate_login(driver: webdriver.Chrome) -> bool:
     url = f"https://member.{domain}/app/03/my/profile"
     driver.get(url)
     with suppress(TimeoutException):
-        WebDriverWait(driver, 5).until(lambda x: "ES0001" in x.page_source)
+        WebDriverWait(driver, 1).until(lambda x: "ES0001" in x.page_source)
         return False
     try:
-        WebDriverWait(driver, 5).until(EC.url_to_be(url))
+        WebDriverWait(driver, 2).until(EC.url_to_be(url))
         return True
     except TimeoutException:
         return False
 
 
 def login(driver: webdriver.Chrome, username: str, password: str, error_on_captcha=False):
     """
@@ -106,25 +106,27 @@
     return f"NFBR.a6G.Initializer.{obj_name}.menu"
 
 
 def go2page(driver: webdriver.Chrome, menu_name: str, page: int):
     driver.execute_script(f"{menu_name}.options.a6l.moveToPage({page-1});")
 
 
-def download_book(driver: webdriver.Chrome, cfg: Config, book_uuid: str):
+def download_book(driver: webdriver.Chrome, cfg: Config, book_uuid: str, overwrite):
     logging.info("Downloading book %s", book_uuid)
     driver.get(f"https://{domain}/de{book_uuid}/")
     WebDriverWait(driver, 10).until(
         EC.presence_of_element_located((By.CLASS_NAME, "p-main__title")))
 
     soup = bs4.BeautifulSoup(driver.page_source, "lxml")
 
     title = soup.find(class_="p-main__title").text.strip()
     authors_ml = soup.find(class_="p-author").find_all("dd")
     authors = [a.text.strip() for a in authors_ml]
+    if not title:
+        raise ValueError("Title not found")
 
     logging.info("Titled %s by %s", title, ", ".join(authors))
 
     driver.set_window_size(*cfg.viewer_size)  # size of bw page
 
     with suppress(TimeoutException):
         WebDriverWait(driver, 3).until(EC.presence_of_element_located(
@@ -136,45 +138,47 @@
                f"?r=BROWSER_VIEWER/{book_uuid}/https%3A%2F%2Fbookwalker.jp%2Fde{book_uuid}%2F")
 
     save_dir = Path(f"babies/{title}")
     save_dir.mkdir(exist_ok=True, parents=True)
     meta_path = save_dir / "meta.json"
     meta_path.write_text(json.dumps(
         {"title": title, "authors": authors},
-        ensure_ascii=False, indent=2))
+        ensure_ascii=False, indent=2), encoding = "utf-8")
 
     driver.switch_to.window(driver.window_handles[-1])
 
-    wait4loading(driver)
-
     with suppress(TimeoutException):
         WebDriverWait(driver, 10).until(EC.presence_of_element_located(
             (By.ID, "pageSliderCounter"))
         )
 
     if "ERROR998" in driver.page_source:
         logging.error("Error 998: Must log out from another device")
         raise Error998()
 
-    _, total_pages = get_pages(driver)
-    prev_imgs = deque[bytes](maxlen=2)  # used for checking update for 2 buffers
-    max_retries = 30
-    logging.info("Total pages: %s", total_pages)
-
     WebDriverWait(driver, 30).until(
         EC.presence_of_element_located((By.CSS_SELECTOR, ".currentScreen canvas")))
-    menu_name = get_menu_name(driver)
 
     WebDriverWait(driver, 30).until(
         EC.invisibility_of_element_located((By.CLASS_NAME, "progressbar")))
 
+    _, total_pages = get_pages(driver)
+    prev_imgs = deque[bytes](maxlen=2)  # used for checking update for 2 buffers
+    max_retries = 30
+    logging.info("Total pages: %s", total_pages)
+
+    menu_name = get_menu_name(driver)
     go2page(driver, menu_name, 1)
 
     for current_page in track(range(1, total_pages + 1), description="Downloading", total=total_pages):
         retry = 0
+        savename = save_dir / f"page_{current_page}.png"
+        if savename.exists() and not overwrite:
+            logging.debug("Page %s already exists, skipping", current_page)
+            continue
         go2page(driver, menu_name, current_page)
         while current_page != get_pages(driver)[0]:
             sleep(0.1)
         wait4loading(driver)
         logging.debug("Getting page %s out of %s", current_page, total_pages)
         canvas = driver.find_element(By.CSS_SELECTOR, ".currentScreen canvas")
         while retry < max_retries:
@@ -188,9 +192,9 @@
                 prev_imgs.append(img_bytes)
                 break
             retry += 1
             logging.debug("Retrying page %s (%s/%s)", current_page, retry, max_retries)
             sleep(0.3)
         if retry == max_retries:
             logging.warning("Potentially repeated page %s", current_page)
-        img.save(save_dir / f"page_{current_page}.png")
+        img.save(savename)
         logging.debug("Saved page %s", current_page)
```

### Comparing `fuckbookwalker-0.1.1/bookphucker/utils.py` & `fuckbookwalker-0.1.3/bookphucker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     cookies = driver.get_cookies()
     if not cookies_path.exists():
         all_cookies = {}
     else:
         all_cookies = json.loads(cookies_path.read_text())
     netloc = urlparse(url).netloc
     all_cookies[netloc] = cookies
-    cookies_path.write_text(json.dumps(all_cookies, indent=2))
+    cookies_path.write_text(json.dumps(all_cookies, indent=2), encoding = "utf-8")
 
 
 def scroll_click(driver: webdriver.Chrome, element: WebElement, timeout: int = 10):
     WebDriverWait(driver, timeout).until(EC.element_to_be_clickable(element))
     webdriver.ActionChains(driver).scroll_to_element(element).perform()
     element.click()  # sending click event to element instead of clicking on element position with action chains
```

### Comparing `fuckbookwalker-0.1.1/pyproject.toml` & `fuckbookwalker-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fuckBookWalker"
-version = "0.1.1"
+version = "0.1.3"
 description = "Download books from bookwalker.jp"
 authors = ["VermiIIi0n <dungeon.behind0t@icloud.com>"]
 readme = "README.md"
 packages = [{ include = "bookphucker" }]
 license = "MIT"
 homepage = "https://github.com/VermiIIi0n/fuckBookWalker"
 
@@ -44,14 +44,15 @@
 lxml = "^5.1.0"
 types-ujson = "^5.9.0.0"
 undetected-chromedriver = "^3.5.5"
 setuptools = "^69.1.1"
 platformdirs = "^4.2.0"
 rich = "^13.7.1"
 semantic-version = "^2.10.0"
+requests = "^2.31.0"
 
 [tool.poetry.extras]
 
 [tool.poetry.group.dev.dependencies]
 
 # coveralls = ">3.3.1"
 # sphinx-autoapi = "^2.1.0"
@@ -60,14 +61,15 @@
 # pytest = "^8.0.0"
 # pytest-asyncio = "^0.23.5"
 # pytest-cov = "^4.1.0"
 # coverage = { extras = ["toml"], version = "^7.4.1" }
 mypy = "^1.8.0"
 # types-toml = "^0.10.8.7"
 autopep8 = "^2.0.4"
+types-requests = "^2.31.0.20240406"
 
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
@@ -150,7 +152,10 @@
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/VermiIIi0n/fuckBookWalker/issues"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+bookbaker = "bookphucker.cli:run"
```

### Comparing `fuckbookwalker-0.1.1/PKG-INFO` & `fuckbookwalker-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuckBookWalker
-Version: 0.1.1
+Version: 0.1.3
 Summary: Download books from bookwalker.jp
 Home-page: https://github.com/VermiIIi0n/fuckBookWalker
 License: MIT
 Keywords: utilities,bookwalker,automation,novel,webnovel,lightnovel,manga
 Author: VermiIIi0n
 Author-email: dungeon.behind0t@icloud.com
 Requires-Python: >=3.12,<4.0
@@ -21,26 +21,27 @@
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: ebooklib (>=0.18,<0.19)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: selenium (>=4.18.1,<5.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: setuptools (>=69.1.1,<70.0.0)
 Requires-Dist: types-ujson (>=5.9.0.0,<6.0.0.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Requires-Dist: undetected-chromedriver (>=3.5.5,<4.0.0)
 Requires-Dist: webdriver-manager (>=4.0.1,<5.0.0)
 Project-URL: Issues, https://github.com/VermiIIi0n/fuckBookWalker/issues
 Description-Content-Type: text/markdown
 
-# Unpolished bookwalker.jp scraper
+# Unpolished bookwalker scraper
 
 > It just works. -- Todd Howard
 
 ## TODO List
 
 - [ ] Image `EPUB` export
 - [ ] `OCR` integration
@@ -64,14 +65,18 @@
 ```bash
 poetry run python bookphucker <url or uuid of books>
 ```
 
 You should see something like this.
 ![sample](./imgs/sample.png)
 
+### Configuration
+
+wip...
+
 By default, `bookphucker` will try to reuse previous `cookies`, using `--no-cache` to clear `cookies`.
 
 ## Common Issues
 
 ### Cannot log in
 
 You may encounter CAPTCHA during the login process.
```

