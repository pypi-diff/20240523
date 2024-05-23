# Comparing `tmp/pytest_reserial-0.3.0.tar.gz` & `tmp/pytest_reserial-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_reserial-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_reserial-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_reserial-0.3.0.tar` & `pytest_reserial-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      578 2024-02-08 08:36:04.187567 pytest_reserial-0.3.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      910 2023-04-26 10:42:13.829488 pytest_reserial-0.3.0/.gitignore
--rw-r--r--   0        0        0     2263 2024-02-08 08:59:56.142516 pytest_reserial-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1057 2024-02-08 09:01:27.509513 pytest_reserial-0.3.0/LICENSE
--rw-r--r--   0        0        0     4224 2024-02-08 08:59:42.482068 pytest_reserial-0.3.0/README.md
--rw-r--r--   0        0        0     1649 2024-02-08 08:59:47.910246 pytest_reserial-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       93 2024-02-08 09:01:27.513513 pytest_reserial-0.3.0/src/pytest_reserial/__init__.py
--rw-r--r--   0        0        0     9923 2024-02-08 08:59:47.910246 pytest_reserial-0.3.0/src/pytest_reserial/reserial.py
--rw-r--r--   0        0        0       28 2022-11-24 14:07:04.692702 pytest_reserial-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     3458 2024-02-06 14:58:26.538543 pytest_reserial-0.3.0/tests/test_reserial.py
--rw-r--r--   0        0        0      553 2024-02-08 08:59:47.910246 pytest_reserial-0.3.0/tox.ini
--rw-r--r--   0        0        0     5411 1970-01-01 00:00:00.000000 pytest_reserial-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      578 2024-02-08 08:36:04.187567 pytest_reserial-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      910 2023-04-26 10:42:13.829488 pytest_reserial-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3214 2024-05-23 06:34:28.122663 pytest_reserial-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1057 2024-02-08 09:01:27.509513 pytest_reserial-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4117 2024-05-22 19:26:25.073545 pytest_reserial-0.4.0/README.md
+-rw-r--r--   0        0        0     1649 2024-02-08 08:59:47.910246 pytest_reserial-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-23 06:34:28.126663 pytest_reserial-0.4.0/src/pytest_reserial/__init__.py
+-rw-r--r--   0        0        0    10562 2024-05-22 19:26:25.073545 pytest_reserial-0.4.0/src/pytest_reserial/reserial.py
+-rw-r--r--   0        0        0      526 2024-05-23 06:24:15.014605 pytest_reserial-0.4.0/src/pytest_reserial/update_log.py
+-rw-r--r--   0        0        0       28 2022-11-24 14:07:04.692702 pytest_reserial-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     5273 2024-05-22 19:26:25.073545 pytest_reserial-0.4.0/tests/test_reserial.py
+-rw-r--r--   0        0        0      553 2024-02-08 08:59:47.910246 pytest_reserial-0.4.0/tox.ini
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 pytest_reserial-0.4.0/PKG-INFO
```

### Comparing `pytest_reserial-0.3.0/.github/workflows/main.yml` & `pytest_reserial-0.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_reserial-0.3.0/.gitignore` & `pytest_reserial-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_reserial-0.3.0/CHANGELOG.md` & `pytest_reserial-0.4.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 # Changelog
 
-## [0.3.1] - Development
+## [0.4.1] - Development
+
+## [0.4.0] - 2024-05-22
+
+_This release changes the format for traffic log files. Use the provided `update_log.py`-script to update old logs to the new format.
+
+### Changed
+
+- __Breaking__: Store test recordings as JSON Lines instead of JSON ([`2b047d7`](https://github.com/bessman/pytest-reserial/commit/2b047d7cc96a06b201e7d25d316492e079835a61))
+- __Breaking__: Store RX and TX bytes as base64 strings instead of lists ([`2b047d7`](https://github.com/bessman/pytest-reserial/commit/2b047d7cc96a06b201e7d25d316492e079835a61))
+
+### Added
+
+- Add script (`update_log.py`) to convert old log files to new format ([`ca14b9b`](https://github.com/bessman/pytest-reserial/commit/ca14b9be86ced3a58b417dc0d8b14afde97df86d))
+
+### Removed
+
+- Remove optional dependency on jsbeautifier ([`0ba5414`](https://github.com/bessman/pytest-reserial/commit/0ba54145e8362e187a479f8a61ac553263f7d8fa))
 
 ## [0.3.0] - 2024-02-07
 
 ### Changed
 
 - __Breaking__: Raise `_pytest.outcomes.Failed` instead of `ValueError` on mismatch ([`b72d304`](https://github.com/bessman/pytest-reserial/commit/b72d304c1b21db524fd1eaf79c9aab91d9542b79))
 - Split log files over multiple lines with `indent` ([`cd5aa41`](https://github.com/bessman/pytest-reserial/commit/cd5aa41d9be1877f68a45a4e069e1845dbb7f3c4))
@@ -42,13 +59,14 @@
 
 _Maintenance release._
 
 ## [0.2.0] - 2022-11-24
 
 _Initial release._
 
+[0.4.0]: https://github.com/bessman/pytest-reserial/releases/tag/0.4.0
 [0.3.0]: https://github.com/bessman/pytest-reserial/releases/tag/0.3.0
 [0.2.4]: https://github.com/bessman/pytest-reserial/releases/tag/v0.2.4
 [0.2.3]: https://github.com/bessman/pytest-reserial/releases/tag/v0.2.3
 [0.2.2]: https://github.com/bessman/pytest-reserial/releases/tag/v0.2.2
 [0.2.1]: https://github.com/bessman/pytest-reserial/releases/tag/v0.2.1
 [0.2.0]: https://github.com/bessman/pytest-reserial/releases/tag/v0.2.0
```

### Comparing `pytest_reserial-0.3.0/LICENSE` & `pytest_reserial-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_reserial-0.3.0/README.md` & `pytest_reserial-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,25 @@
 
 1.  Connect the device.
 2.  Run `pytest my_serial_app.py` and verify that the test passes with the device connected.
 3.  Run `pytest --record my_serial_app.py`. The test will run again, and the traffic will be recorded.
 4.  Disconnect the device.
 5.  Run `pytest --replay my_serial_app.py`. The test will pass!
 
-The logged traffic will be stored in JSON files in the same directory as your test files, and will have the same names as the test files except with a .json extension instead of .py. For example, if your project layout is:
+The logged traffic will be stored as JSON Lines, with one file per test file and one line per test, in the same directory as your test files. The files will have the same names as the test files except with a .jsonl extension instead of .py. For example, if your project layout is:
 
 ```shell
 ├── src
 │   ├── myproject
 │   │   ├── ...
 ├── tests
 │   ├── test_myproject.py
 ```
 
-Then after running `pytest --record`, the test/ directory will contain a new file, test_myproject.json, containing the recorded serial traffic from the tests.
+Then after running `pytest --record`, the test/ directory will contain a new file, test_myproject.jsonl, containing the recorded serial traffic from the tests.
 
 ## Why
 
 Have you ever tried to write tests for a program that talks to an external device over serial (like an Arduino or something)? You probably wrote the tests assuming that the device is question would always be connected when running the tests, right? And later you got bit by one or more of the pitfalls of that approach:
 
 -   You wanted to run the tests when the device wasn't connected. Perhaps you were travelling, or
     someone had borrowed it. Whatever the reason, you found yourself unable to run the tests, and
@@ -80,12 +80,10 @@
 
 With pytest-reserial, you don't have to worry about any of that. Just write your tests as if the device is always connected. Then, simply use the `reserial` fixture to record the serial traffic from passing tests, and replay it when the device isn't connected.
 
 ## Requirements
 
 pytest-reserial depends on pytest and pyserial.
 
-If jsbeautifier is installed, each test's recorded traffic is written on a single line in the log files. Otherwise, each recorded byte is written on a separate line.
-
 ## Copyright
 
 MIT License, (C) 2022 Alexander Bessman
```

### Comparing `pytest_reserial-0.3.0/pyproject.toml` & `pytest_reserial-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_reserial-0.3.0/src/pytest_reserial/reserial.py` & `pytest_reserial-0.4.0/src/pytest_reserial/reserial.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Record or replay serial traffic when running tests."""
 
 from __future__ import annotations
 
+import base64
 import json
 from enum import IntEnum
 from pathlib import Path
-from typing import Callable, Dict, Generator, List, Tuple
+from typing import Callable, Dict, Iterator, Literal, Tuple
 
 import pytest
 from serial import Serial  # type: ignore[import-untyped]
 
-TrafficLog = Dict[str, List[int]]
+TrafficLog = Dict[Literal["rx", "tx"], bytes]
 PatchMethods = Tuple[
     Callable[[Serial, int], bytes],
     Callable[[Serial, bytes], int],
     Callable[[Serial], None],
     Callable[[Serial], None],
 ]
 
@@ -56,85 +57,93 @@
     """
 
 
 @pytest.fixture()
 def reserial(
     monkeypatch: pytest.MonkeyPatch,
     request: pytest.FixtureRequest,
-) -> Generator[None, None, None]:
+) -> Iterator[None]:
     """Record or replay serial traffic.
 
     Raises
     ------
     _pytest.outcomes.Failed
         If less data than expected was read or written during replay.
     """
     record = request.config.getoption("--record")
     replay = request.config.getoption("--replay")
     mode = Mode(replay | record << 1)
 
-    logpath = Path(request.path).parent / (Path(request.path).stem + ".json")
-    testname = request.node.name
-    log = get_traffic_log(mode, logpath, testname)
+    log_path = Path(request.path).parent / (Path(request.path).stem + ".jsonl")
+    test_name = request.node.name
+    log = get_traffic_log(mode, log_path, test_name)
 
     read_patch, write_patch, open_patch, close_patch = get_patched_methods(mode, log)
     monkeypatch.setattr(Serial, "read", read_patch)
     monkeypatch.setattr(Serial, "write", write_patch)
     monkeypatch.setattr(Serial, "open", open_patch)
     monkeypatch.setattr(Serial, "close", close_patch)
     monkeypatch.setattr(Serial, "_reconfigure_port", reconfigure_port_patch)
 
     yield
 
     if mode == Mode.RECORD:
-        write_log(log, logpath, testname)
+        write_log(log, log_path, test_name)
         return
 
     if log["rx"] or log["tx"]:
         msg = (
             "Some messages where not replayed:}\n"
             f"Remaining RX: {len(log['rx'])}\n"
             f"Remaining TX: {len(log['tx'])}"
         )
         pytest.fail(msg)
 
 
-def get_traffic_log(mode: Mode, logpath: Path, testname: str) -> TrafficLog:
+def get_traffic_log(mode: Mode, log_path: Path, test_name: str) -> TrafficLog:
     """Load recorded traffic (replay) or create an empty log (record).
 
     Parameters
     ----------
     mode : Mode
         The requested mode of operation, i.e. `REPLAY`, `RECORD`, or `DONT_PATCH`.
-    logpath: str
+    log_path: str
         The name of the file where recorded traffic is logged.
-    testname: str
+    test_name: str
         The name of the currently running test, which is used as a key in the log file.
 
     Returns
     -------
     log : dict[str, list[int]]
         Dictionary with keys "rx" and "tx", with corresponding lists of received and
         transmitted data. If `mode` is `RECORD` or `DONT_PATCH`, the lists are empty.
 
     Raises
     ------
     ValueError
         If both '--replay' and '--record' were specified.
+        If no the test has no recorded traffic .
     """
     if mode == Mode.INVALID:
         msg = "Choose one of 'replay' or 'record', not both"
         raise ValueError(msg)
 
-    log: TrafficLog = {"rx": [], "tx": []}
+    log: TrafficLog = {"rx": b"", "tx": b""}
 
     if mode == Mode.REPLAY:
-        with Path.open(logpath) as logfile:
-            logs = json.load(logfile)
-        log = logs[testname]
+        with Path.open(log_path) as fin:
+            for line in fin:
+                if log := json.loads(line).get(test_name):
+                    break
+            else:
+                msg = f"No recorded traffic for test: {test_name}"
+                raise ValueError(msg)
+
+            log["rx"] = base64.b64decode(log["rx"])
+            log["tx"] = base64.b64decode(log["tx"])
 
     return log
 
 
 def get_patched_methods(mode: Mode, log: TrafficLog) -> PatchMethods:
     """Return patched read, write, open, and closed methods.
 
@@ -196,20 +205,20 @@
         return values are identical to Serial.write.
 
         Raises
         ------
         _pytest.outcomes.Failed
             If written data does not match recorded data.
         """
-        if list(data) == log["tx"][: len(data)]:
+        if data == log["tx"][: len(data)]:
             log["tx"] = log["tx"][len(data) :]
         else:
             msg = (
                 "Written data does not match recorded data: "
-                f"{list(data)} != {log['tx'][: len(data)]}"
+                f"{data!r} != {log['tx'][: len(data)]!r}"
             )
             pytest.fail(msg)
 
         return len(data)
 
     def replay_read(
         self: Serial,  # noqa: ARG001
@@ -263,61 +272,68 @@
 
     def record_write(self: Serial, data: bytes) -> int:
         """Record TX data before writing to the bus.
 
         Monkeypatch this method over Serial.write to record traffic. Parameters and
         return values are identical to Serial.write.
         """
-        log["tx"] += list(data)
+        log["tx"] += data
         written: int = real_write(self, data)
         return written
 
     def record_read(self: Serial, size: int = 1) -> bytes:
         """Record RX data after reading from the bus.
 
         Monkeypatch this method over Serial.read to record traffic. Parameters and
         return values are identical to Serial.read.
         """
         data: bytes = real_read(self, size)
-        log["rx"] += list(data)
+        log["rx"] += data
         return data
 
     return record_read, record_write, Serial.open, Serial.close
 
 
 def write_log(
     log: TrafficLog,
-    logpath: Path,
-    testname: str,
+    log_path: Path,
+    test_name: str,
 ) -> None:
     """Write recorded traffic to log file.
 
     Parameters
     ----------
     log: dict[str, list[int]]
         Dictionary holding recorded traffic.
-    logpath: str
+    log_path: str
         The name of the file where recorded traffic is logged.
-    testname: str
+    test_name: str
         The name of the currently running test, which is used as a key in the log file.
     """
-    try:
-        # If the file exists, read its contents.
-        with Path.open(logpath) as logfile:
-            logs = json.load(logfile)
-    except FileNotFoundError:
-        logs = {}
-
-    logs[testname] = log
-    logs_str = json.dumps(logs, indent=4)
-
-    # Print traffic logs on a single line if jsbeautifier is available.
-    try:
-        import jsbeautifier  # type: ignore[import-untyped]
-
-        logs_str = jsbeautifier.beautify(logs_str)
-    except ImportError:
-        pass
-
-    # Wipe the file if it exists, or create a new file if it doesn't.
-    with Path.open(logpath, mode="w") as logfile:
-        logfile.write(logs_str)
+    # Make sure log file exists.
+    log_path.touch()
+    # Write new data to temporary file.
+    tmp_path = Path(test_name + "_" + hex(abs(hash(test_name))).lstrip("0x"))
+
+    with log_path.open("r") as fin, tmp_path.open("w") as fout:
+        seen = False
+        rx = base64.b64encode(bytes(log["rx"])).decode("ascii")
+        tx = base64.b64encode(bytes(log["tx"])).decode("ascii")
+        new_line = json.dumps({test_name: {"rx": rx, "tx": tx}}) + "\n"
+
+        # Recorded traffic is stored as JSON Lines. Parse one line at a time.
+        for old_line in fin:
+            test_data = json.loads(old_line)
+
+            # Each record contains a single key.
+            if test_name in test_data:
+                fout.write(new_line)
+                seen = True
+                continue
+
+            fout.write(old_line)
+
+        if not seen:
+            fout.write(new_line)
+
+    # Overwrite old log file.
+    Path(tmp_path).rename(log_path)
```

### Comparing `pytest_reserial-0.3.0/tests/test_reserial.py` & `pytest_reserial-0.4.0/tests/test_reserial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 import json
 
 from serial import Serial
 
 TEST_RX = b"\x01"
+TEST_RX_ENC = "AQ=="
 TEST_TX = b"\x02"
+TEST_TX_ENC = "Ag=="
 TEST_FILE = f"""
             import serial
             def test_reserial(reserial):
                 s = serial.Serial(port="/dev/ttyUSB0")
-                s.write({TEST_TX})
-                assert s.read() == {TEST_RX}
+                s.write({TEST_TX!r})
+                assert s.read() == {TEST_RX!r}
             def test_reserial2(reserial):
                 s = serial.Serial(port="/dev/ttyUSB0")
-                s.write({TEST_TX})
-                assert s.read() == {TEST_RX}
+                s.write({TEST_TX!r})
+                assert s.read() == {TEST_RX!r}
             """
 TEST_FILE_BAD_TX = f"""
-            import serial
-            def test_reserial(reserial):
-                s = serial.Serial(port="/dev/ttyUSB0")
-                s.write({TEST_RX})
-                assert s.read() == {TEST_RX}
-            """
-TEST_JSON = f"""
-            {{
-                "test_reserial": {{
-                    "rx": {list(TEST_RX)},
-                    "tx": {list(TEST_TX)}
-                }},
-                "test_reserial2": {{
-                    "rx": {list(TEST_RX)},
-                    "tx": {list(TEST_TX)}
-                }}
-            }}
-            """
+                    import serial
+                    def test_reserial(reserial):
+                        s = serial.Serial(port="/dev/ttyUSB0")
+                        s.write({TEST_RX!r})
+                        assert s.read() == {TEST_RX!r}
+                    """
+TEST_JSONL = (
+    f'{{"test_reserial": {{"rx": "{TEST_RX_ENC}", "tx": "{TEST_TX_ENC}"}}}}\n'
+    f'{{"test_reserial2": {{"rx": "{TEST_RX_ENC}", "tx": "{TEST_TX_ENC}"}}}}\n'
+)
 
 
 def test_record(monkeypatch, pytester):
     pytester.makepyfile(TEST_FILE)
 
     def patch_write(self: Serial, data: bytes) -> int:
         return len(data)
@@ -53,23 +47,71 @@
 
     monkeypatch.setattr(Serial, "write", patch_write)
     monkeypatch.setattr(Serial, "read", patch_read)
     monkeypatch.setattr(Serial, "open", patch_open)
     monkeypatch.setattr(Serial, "close", patch_close)
     result = pytester.runpytest("--record")
 
-    with open("test_record.json", "r") as f:
-        recording = json.load(f)
+    with open("test_record.jsonl", "r") as f:
+        recording = [json.loads(line) for line in f.readlines()]
+
+    expected = [json.loads(line) for line in TEST_JSONL.splitlines()]
+
+    assert recording == expected
+    assert result.ret == 0
+
+
+def test_update_existing(monkeypatch, pytester):
+    pytester.makefile(".jsonl", test_update_existing=TEST_JSONL)
+    pytester.makepyfile(
+        f"""
+        import serial
+        def test_reserial(reserial):
+            s = serial.Serial(port="/dev/ttyUSB0")
+            s.write({2 * TEST_TX})
+            assert s.read() == {2 * TEST_RX}
+        """
+    )
+
+    def patch_write(self: Serial, data: bytes) -> int:
+        return len(data)
+
+    def patch_read(self: Serial, size: int = 1) -> bytes:
+        return 2 * TEST_RX
+
+    def patch_open(self: Serial) -> None:
+        self.is_open = True
+
+    def patch_close(self: Serial) -> None:
+        self.is_open = False
+
+    monkeypatch.setattr(Serial, "write", patch_write)
+    monkeypatch.setattr(Serial, "read", patch_read)
+    monkeypatch.setattr(Serial, "open", patch_open)
+    monkeypatch.setattr(Serial, "close", patch_close)
+    result = pytester.runpytest("--record")
+
+    with open("test_update_existing.jsonl", "r") as f:
+        recording = [json.loads(line) for line in f.readlines()]
 
-    assert recording == json.loads(TEST_JSON)
+    expected_rx_enc = "AQE="
+    expected_tx_enc = "AgI="
+    expected_jsonl = (
+        f'{{"test_reserial": {{"rx": "{expected_rx_enc}", "tx": "{expected_tx_enc}"}}}}\n'
+        f'{{"test_reserial2": {{"rx": "{TEST_RX_ENC}", "tx": "{TEST_TX_ENC}"}}}}\n'
+    )
+
+    expected = [json.loads(line) for line in expected_jsonl.splitlines()]
+
+    assert recording == expected
     assert result.ret == 0
 
 
 def test_replay(pytester):
-    pytester.makefile(".json", test_replay=TEST_JSON)
+    pytester.makefile(".jsonl", test_replay=TEST_JSONL)
     pytester.makepyfile(TEST_FILE)
     result = pytester.runpytest("--replay")
     assert result.ret == 0
 
 
 def test_dont_patch(pytester):
     pytester.makepyfile(
@@ -87,15 +129,15 @@
 def test_invalid_option(pytester):
     pytester.makepyfile(TEST_FILE)
     result = pytester.runpytest("--replay", "--record")
     result.assert_outcomes(errors=2)
 
 
 def test_bad_tx(pytester):
-    pytester.makefile(".json", test_bad_tx=TEST_JSON)
+    pytester.makefile(".jsonl", test_bad_tx=TEST_JSONL)
     pytester.makepyfile(TEST_FILE_BAD_TX)
     result = pytester.runpytest("--replay")
     result.assert_outcomes(errors=1, failed=1)
 
 
 def test_help_message(pytester):
     result = pytester.runpytest("--help")
@@ -107,20 +149,33 @@
         ]
     )
     assert result.ret == 0
 
 
 def test_change_settings(pytester):
     pytester.makefile(
-        ".json",
-        test_change_settings='{"test_reserial": {"tx": [], "rx": []}}',
+        ".jsonl",
+        test_change_settings='{"test_reserial": {"tx": "", "rx": ""}}',
     )
     pytester.makepyfile(
         """
             import serial
             def test_reserial(reserial):
                 s = serial.Serial(port="/dev/ttyUSB0")
                 s.timeout = 1
         """
     )
     result = pytester.runpytest("--replay")
     assert result.ret == 0
+
+
+def test_no_traffic_for_test(pytester):
+    pytester.makefile(".jsonl", test_no_traffic_for_test=TEST_JSONL)
+    pytester.makepyfile(
+        """
+            import serial
+            def test_reserial3(reserial):
+                pass
+        """
+    )
+    result = pytester.runpytest("--replay")
+    result.assert_outcomes(errors=1)
```

### Comparing `pytest_reserial-0.3.0/tox.ini` & `pytest_reserial-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest_reserial-0.3.0/PKG-INFO` & `pytest_reserial-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reserial
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pytest fixture for recording and replaying serial port traffic.
 Keywords: serial,testing,logging,mocking,patching,stubbing,record,replay
 Author-email: Alexander Bessman <alexander.bessman@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -70,25 +70,25 @@
 
 1.  Connect the device.
 2.  Run `pytest my_serial_app.py` and verify that the test passes with the device connected.
 3.  Run `pytest --record my_serial_app.py`. The test will run again, and the traffic will be recorded.
 4.  Disconnect the device.
 5.  Run `pytest --replay my_serial_app.py`. The test will pass!
 
-The logged traffic will be stored in JSON files in the same directory as your test files, and will have the same names as the test files except with a .json extension instead of .py. For example, if your project layout is:
+The logged traffic will be stored as JSON Lines, with one file per test file and one line per test, in the same directory as your test files. The files will have the same names as the test files except with a .jsonl extension instead of .py. For example, if your project layout is:
 
 ```shell
 ├── src
 │   ├── myproject
 │   │   ├── ...
 ├── tests
 │   ├── test_myproject.py
 ```
 
-Then after running `pytest --record`, the test/ directory will contain a new file, test_myproject.json, containing the recorded serial traffic from the tests.
+Then after running `pytest --record`, the test/ directory will contain a new file, test_myproject.jsonl, containing the recorded serial traffic from the tests.
 
 ## Why
 
 Have you ever tried to write tests for a program that talks to an external device over serial (like an Arduino or something)? You probably wrote the tests assuming that the device is question would always be connected when running the tests, right? And later you got bit by one or more of the pitfalls of that approach:
 
 -   You wanted to run the tests when the device wasn't connected. Perhaps you were travelling, or
     someone had borrowed it. Whatever the reason, you found yourself unable to run the tests, and
@@ -110,13 +110,11 @@
 
 With pytest-reserial, you don't have to worry about any of that. Just write your tests as if the device is always connected. Then, simply use the `reserial` fixture to record the serial traffic from passing tests, and replay it when the device isn't connected.
 
 ## Requirements
 
 pytest-reserial depends on pytest and pyserial.
 
-If jsbeautifier is installed, each test's recorded traffic is written on a single line in the log files. Otherwise, each recorded byte is written on a separate line.
-
 ## Copyright
 
 MIT License, (C) 2022 Alexander Bessman
```

